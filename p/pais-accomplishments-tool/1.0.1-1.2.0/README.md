# Comparing `tmp/pais_accomplishments_tool-1.0.1.tar.gz` & `tmp/pais_accomplishments_tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pais_accomplishments_tool-1.0.1.tar", max compression
+gzip compressed data, was "pais_accomplishments_tool-1.2.0.tar", max compression
```

## Comparing `pais_accomplishments_tool-1.0.1.tar` & `pais_accomplishments_tool-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    20849 2024-04-23 19:08:54.038516 pais_accomplishments_tool-1.0.1/LICENSE
--rw-r--r--   0        0        0     5053 2024-04-23 20:05:10.803931 pais_accomplishments_tool-1.0.1/pais-accomplishments-tool/paisAccTool.py
--rw-r--r--   0        0        0      926 2024-04-23 20:36:23.587750 pais_accomplishments_tool-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5967 2024-04-23 20:36:07.397871 pais_accomplishments_tool-1.0.1/readme.md
--rw-r--r--   0        0        0     6986 1970-01-01 00:00:00.000000 pais_accomplishments_tool-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    20849 2024-04-23 19:08:54.038516 pais_accomplishments_tool-1.2.0/LICENSE
+-rw-r--r--   0        0        0      261 2024-04-28 20:17:36.481225 pais_accomplishments_tool-1.2.0/pais-accomplishments-tool/config.default.yml
+-rw-r--r--   0        0        0     5145 2024-04-28 20:11:35.880967 pais_accomplishments_tool-1.2.0/pais-accomplishments-tool/paisAccTool.py
+-rw-r--r--   0        0        0      944 2024-04-28 20:28:14.033887 pais_accomplishments_tool-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7131 2024-04-28 20:27:31.999910 pais_accomplishments_tool-1.2.0/readme.md
+-rw-r--r--   0        0        0     8189 1970-01-01 00:00:00.000000 pais_accomplishments_tool-1.2.0/PKG-INFO
```

### Comparing `pais_accomplishments_tool-1.0.1/LICENSE` & `pais_accomplishments_tool-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pais_accomplishments_tool-1.0.1/pais-accomplishments-tool/paisAccTool.py` & `pais_accomplishments_tool-1.2.0/pais-accomplishments-tool/paisAccTool.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,76 +12,95 @@
 # limitations under the License.
 #
 # You should have received a copy of the License along with this program.
 # If not, see <https://creativecommons.org/licenses/by-nc-sa/4.0/>.
 #
 # GitHub repository <https://github.com/CuberHuber/pais-accomplishments-tool>
 import argparse
+import dataclasses
+import os
 
 import bibtexparser
+import yaml
 import pymorphy3
 from bibtexparser import Library
 
-DEF_TEMPLATE = '{prefix} {type} {title}, {author}, {organization}, {month}.{year}'
-DEF_MORPHS = ('type', 'organization')
+
+@dataclasses.dataclass
+class KindConf:
+    key: str
+    template: str
+    morphs: tuple[str]
 
 
 def library(file) -> Library:
     """
     Get a bibtex library object from a file.
     :param file:
     :return:
     """
     return bibtexparser.parse_file(file)
 
 
-def accomplishments(lib: Library, template: str, for_morphs: tuple[str]) -> list[str]:
+def config(file) -> dict[str, KindConf]:
+    _out = {}
+    with open(file, "r") as f:
+        yml = yaml.safe_load(f)
+        if yml.get('kinds'):
+            for kind, value in yml.get('kinds').items():
+                _out[kind] = (KindConf(kind, value.get('template'), value.get('morphs')))
+        else:
+            raise ValueError('No kinds found in config file')
+    return _out
+
+
+def accomplishments(lib: Library, config: dict[str, KindConf]) -> list[str]:
     """
     Generate accomplishments list from a bibtex library.
+    :param config:
     :param lib:
-    :param template:
-    :param for_morphs:
     :return:
     """
     output = []
     for entry in lib.entries:
         print(f' [ ]  {entry.entry_type} accomplishment: {entry.key}', end='\t')
         fields = {field.key: field.value for field in entry.fields}
+        cfg = config.get(entry.entry_type)
         morph = pymorphy3.MorphAnalyzer()
         for field in fields.items():
-            if field[0] in for_morphs:
+            if field[0] in cfg.morphs:
                 res = []
                 for word in field[1].split():
                     try:
                         _word = morph.parse(word.lower())[0].inflect({'gent'}).word
                         if word[0] == _word.capitalize()[0]:
                             res.append(_word.capitalize())
                         else:
                             res.append(_word)
                     except:
                         res.append(word)
                 fields[field[0]] = ' '.join(res)
-        output.append(template.format(**fields))
+        output.append(cfg.template.format(**fields))
         print('done')
     return output
 
 
 def formatting(_accomplishments: list[str], _is_capitalize: bool, _is_enumerate: bool) -> list[str]:
     """
     Format accomplishments according to the formatting rules.
     :param _accomplishments:
     :param _is_capitalize:
     :param _is_enumerate:
     :return:
     """
     if _is_capitalize:
-        _accomplishments = [acc[0].capitalize()+acc[1:] for acc in _accomplishments]
+        _accomplishments = [acc[0].capitalize() + acc[1:] for acc in _accomplishments]
 
     if _is_enumerate:
-        _accomplishments = [f'{i+1}. {acc}' for i, acc in enumerate(_accomplishments)]
+        _accomplishments = [f'{i + 1}. {acc}' for i, acc in enumerate(_accomplishments)]
 
     return _accomplishments
 
 
 def save(_accomplishments: list[str], _path: str) -> None:
     """
     Save accomplishments according to the text file
@@ -99,41 +118,37 @@
     :return:
     """
     parser = argparse.ArgumentParser(description='The micro tools for contain and formating accomplishments from '
                                                  'BibTex source')
     # Add arguments
     parser.add_argument('source', help='Path to source .bib file')
     parser.add_argument('-d', '--destination', required=False, help='Path to destination .bib file')
-    parser.add_argument('-t', '--template', required=False,
-                        help='A template string for generating accomplishment string. '
-                             'Default: ' + DEF_TEMPLATE)
-    parser.add_argument('-m', '--morphs', required=False, nargs='+',
-                        help=f'A list of fields for morphological transformations. '
-                             f'Default: {DEF_MORPHS}')
+    parser.add_argument('--config', required=False, help='Path to config.yml file')
     parser.add_argument('-c', '--capitalize', default=False, help=f'Flag', action='store_true')
     parser.add_argument('-en', '--enumerate', default=False, help=f'Flag', action='store_true')
     # Parse the arguments
     args = parser.parse_args()
 
-    template = args.template if args.template else DEF_TEMPLATE
-    morphs = tuple(args.morphs) if args.morphs else DEF_MORPHS
     if args.source is None:
         raise FileNotFoundError('Source path is required')
 
-    return template, morphs, args.source, args.destination, bool(args.capitalize), bool(args.enumerate)
+    if args.config is None:
+        _config = os.path.dirname(__file__) + '/config.default.yml'
+    else:
+        _config = str(args.config)
+
+    return _config, args.source, args.destination, bool(args.capitalize), bool(args.enumerate)
 
 
 def hello():
     print("""Hello everyone!
 This is the micro tools for contain and formating accomplishments from BibTex source""")
 
-
 if __name__ == '__main__':
-    template, morphs, source, destination, is_capitalize, is_enumerate = parameters()
+    _config_file, source, destination, is_capitalize, is_enumerate = parameters()
     hello()
-    accs = accomplishments(library(source), template, morphs)
+    accs = accomplishments(library(source), config(_config_file))
     accs = formatting(accs, is_capitalize, is_enumerate)
     if destination:
         save(accs, destination)
     else:
         print(*accs, sep='\n\r')
-
```

### Comparing `pais_accomplishments_tool-1.0.1/pyproject.toml` & `pais_accomplishments_tool-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pais-accomplishments-tool"
-version = "1.0.1"
+version = "1.2.0"
 description = "A small tool for generating and transformation accomplishments from BibTex format files"
 authors = [
     "Roman Lupashko <mossy0.civets@icloud.com>",
 ]
 packages = [{include = "pais-accomplishments-tool"}]
 readme = "readme.md"
 classifiers = [
@@ -19,11 +19,12 @@
 repository = "https://github.com/CuberHuber/pais-accomplishments-tool"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 bibtexparser = "2.0.0b7"
 pymorphy3 = "2.0.1"
 pymorphy3-dicts-ru = "2.4.417150.4580142"
+pyyaml = "^6.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pais_accomplishments_tool-1.0.1/readme.md` & `pais_accomplishments_tool-1.2.0/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,60 +4,62 @@
 A small tool for generating and transformation accomplishments from BibTex format files.
 
 ## Homepage
 PYPI: https://pypi.org/project/pais-accomplishments-tool/
 
 ## Quick start
 
+### Table of Contents
+- [Install](#install)
+- [Simple usage](#simple-usage)
+- [Accomplishments format](#accomplishments-format)
+- [Config format](#config-file)
+
 ### Install
 
 For install package run it.
 ```shell
 pip install pais-accomplishments-tool
 ```
 
 ### Upgrade
 For upgrade tools to latest version run it
 ```shell
 pip install pais-accomplishments-tool --upgrade
 ```
 
-### Dependencies
-
-
-
 ### Add to PATH
 
 #### On Mac + zsh
 ```shell
 nano ~/.zshrc
 ```
 And the following line to the `.zshrc` with the actual path of the [package_name] script
 ```shell
 export PATH="/path/to/package:$PATH"
 ```
-For Python 3.15 on MacOS 14
+For Python 3.11.5 on MacOS 14
 ```shell
 export PATH="/Library/Frameworks/Python.framework/Versions/3.11/lib/python3.11/site-packages/pais-accomplishments-tool/paisAccTool.py:$PATH"
 ```
 
 #### On Mac and Linux + bash
 ```shell
 nano ~/.bash_profile
 ```
 And the following line to the `.bash_profile` with the actual path of the [package_name] script
 ```shell
 export PATH="/path/to/package:$PATH"
 ```
-For Python 3.15 on MacOS 14
+For Python 3.11.5 on MacOS 14
 ```shell
 export PATH="/Library/Frameworks/Python.framework/Versions/3.11/lib/python3.11/site-packages/pais-accomplishments-tool/paisAccTool.py:$PATH"
 ```
 
-### Simple use
+### Simple usage
 #### Help
 For watch help message run [paisAccTool.py](pais-accomplishments-tool/paisAccTool.py):
 ```shell
 python3 paisAccTool.py -h
 ```
 
 #### Sample
@@ -69,70 +71,65 @@
 ```shell
 Hello everyone!
 This is the micro tools for contain and formating accomplishments from BibTex source
  [ ]  misc accomplishment: rand1        done
  [ ]  misc accomplishment: rand2        done
  [ ]  misc accomplishment: rand3        done
  [ ]  misc accomplishment: rand4        done
-1. Наставник образовательной программы Звездный путь.Зима, Иван Иванов, Московского государственного университета, 2.2023
-2. Наставник образовательной программы Тёмная материя.Весна, Мария Петрова, Санкт-петербургского государственного университета, 4.2023
-3. Победитель образовательной программы Космос.Лето, Алексей Сидоров, Новосибирского государственного университета, 6.2023
-4. Участник олимпиады искусственный интеллект.Осень, Екатерина Кузнецова, Томского государственного университета, 9.2023
-
+ [ ]  conf accomplishment: conf1        done
+1. Наставник образовательной программы Звездный путь.Зима, разработка системы автоматизированного тестирования : Московского государственного университета : 15.02.2023
+2. Наставник образовательной программы Тёмная материя.Весна, Разработка системы машинного обучения : Санкт-петербургского государственного университета : 2023-04-10 00:00:00
+3. Победитель образовательной программы Космос.Лето, Разработка системы компьютерного зрения : Новосибирского государственного университета : 2023-06-20 00:00:00
+4. Участник олимпиады искусственный интеллект.Осень, Разработка системы естественного языка : Томского государственного университета : 2023-09-15 00:00:00
+5. Публикация "Система NLP для марсианского языка" : Екатерина Кузнецова : Студенческая конференция Масла и Камня, Банка Китая : 11.04.2023
 ```
 #### Common usage format
 ```shell
 python3 paisAccTool.py <source .bib file> [-d <destination>, -t "template string", -m "field" "for" "transformation", -c, -en]
 ```
 
--
-- `-t "template"` contain a python string template that will be used to generate the list of accomplishments. **Important, a template can only contain the bibtex field names of an object**;
-- `-m <"words", " " ..>` contain bibtex fields of the object, which are required to be put in the gent case;
+- `--config` path to config file.
 - `-c` mean that each new entry will start with a capital letter;
 - `-en` mean that the list of accomplishments will be output with numbering.
 
 ```shell
+usage: paisAccTool.py [-h] [-d DESTINATION] [--config CONFIG] [-c] [-en] source
+
 The micro tools for contain and formating accomplishments from BibTex source
 
 positional arguments:
   source                Path to source .bib file
 
 options:
   -h, --help            show this help message and exit
   -d DESTINATION, --destination DESTINATION
                         Path to destination .bib file
-  -t TEMPLATE, --template TEMPLATE
-                        A template string for generating accomplishment string. Default: {prefix} {type} {title}, {author}, {organization}, {month}.{year}
-  -m MORPHS [MORPHS ...], --morphs MORPHS [MORPHS ...]
-                        A list of fields for morphological transformations. Default: ('type', 'organization')
+  --config CONFIG       Path to config.yml file
   -c, --capitalize      Flag
   -en, --enumerate      Flag
 
+
 ```
 
 #### Other usage sample
 Command to output the list of accomplishments to a file
 ```shell
 python3 paisAccTool.py accomplishments_sample.bib -c -en -d output.txt
 ```
 
-Command with its own output template
+Command with its own custom config. You can make a config file along the [sample](#config-file).
 ```shell
-python3 paisAccTool.py accomplishments_sample.bib -t "{prefix} {type} {title}, {author}, {organization}, {location} {start}-{end}"
-```
-
-Command with its own morphological transformations fields
-```shell
-python3 paisAccTool.py accomplishments_sample.bib -m "title", "author", "type"
+python3 paisAccTool.py accomplishments_sample.bib --config /path/to/config.yml
 ```
 
 ### Accomplishments format
 
 Each accomplishment is stored in a .bib file in bibtex format.
-Below are the fields that are used to store achievements:
+
+**Below are the fields that are used to store misc achievements.**
 ```bibtex
 @misc{identifier,
 	prefix = {Твоя роль на мероприятии},
 	title = {Название мероприятия},
 	type = {Тип мероприятия},
 	author = {ФИО},
 	organization = {Организация, которая проводит мероприятие},
@@ -143,13 +140,57 @@
 	end = {дата окончания},
 	year = {год},
 	month = {месяц},
 	certificate = {результат, документ подтверждающий результат или участие (диплом, ...)},
 	order = {место в конкурсе или статус на мероприятии}
 }
 ```
+**Below are the fields that are used to store conf achievements.**
+```bibtex
+@conf{conf1,
+	prefix = {публикация},
+	title = {Студенческая конференция Масла и Камня},
+	type = {конференция},
+	author = {Екатерина Кузнецова},
+	organization = {Банк Китая},
+	topic = {Система NLP для марсианского языка},
+	section = {},
+	location = {Зотеро},
+	url = {some url},
+	start = {11.04.2023},
+	end = {15.04.2023},
+	year = {2023},
+	month = {4},
+	certificate = {сборник},
+	order = {}
+}
+```
 If you do not have a field to enter your specific information, you can add such a field:
 ```bibtex
     <key> = {value}
 ```
 The Accomplishments.bib file can be stored locally on your pc or in a remote git repository, so every commit means a new achievement (very convenient).
 
+### Config file
+The Config file represent as a yaml file.
+Its format:
+```yaml
+kinds:
+  <entry_type>:
+    template: 'template string'
+    morphs:
+      - <field 1>
+      - <field 2>
+```
+For example, you can look on the default config:
+```yaml
+kinds:
+  misc:
+    template: '{prefix} {type} {title}, {section} : {organization} : {start}'
+    morphs:
+      - type
+      - organization
+  conf:
+    template: '{prefix} "{topic}" : {author} : {title}, {organization} : {start}'
+    morphs:
+      - organization
+```
```

### Comparing `pais_accomplishments_tool-1.0.1/PKG-INFO` & `pais_accomplishments_tool-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pais-accomplishments-tool
-Version: 1.0.1
+Version: 1.2.0
 Summary: A small tool for generating and transformation accomplishments from BibTex format files
 Home-page: https://github.com/CuberHuber/pais-accomplishments-tool
 License: CC-BY-NC-SA-4.0
 Author: Roman Lupashko
 Author-email: mossy0.civets@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: End Users/Desktop
@@ -14,73 +14,76 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Markup
 Requires-Dist: bibtexparser (==2.0.0b7)
 Requires-Dist: pymorphy3 (==2.0.1)
 Requires-Dist: pymorphy3-dicts-ru (==2.4.417150.4580142)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Repository, https://github.com/CuberHuber/pais-accomplishments-tool
 Description-Content-Type: text/markdown
 
 # PAIS Accomplishments
 
 ## About
 A small tool for generating and transformation accomplishments from BibTex format files.
 
 ## Homepage
 PYPI: https://pypi.org/project/pais-accomplishments-tool/
 
 ## Quick start
 
+### Table of Contents
+- [Install](#install)
+- [Simple usage](#simple-usage)
+- [Accomplishments format](#accomplishments-format)
+- [Config format](#config-file)
+
 ### Install
 
 For install package run it.
 ```shell
 pip install pais-accomplishments-tool
 ```
 
 ### Upgrade
 For upgrade tools to latest version run it
 ```shell
 pip install pais-accomplishments-tool --upgrade
 ```
 
-### Dependencies
-
-
-
 ### Add to PATH
 
 #### On Mac + zsh
 ```shell
 nano ~/.zshrc
 ```
 And the following line to the `.zshrc` with the actual path of the [package_name] script
 ```shell
 export PATH="/path/to/package:$PATH"
 ```
-For Python 3.15 on MacOS 14
+For Python 3.11.5 on MacOS 14
 ```shell
 export PATH="/Library/Frameworks/Python.framework/Versions/3.11/lib/python3.11/site-packages/pais-accomplishments-tool/paisAccTool.py:$PATH"
 ```
 
 #### On Mac and Linux + bash
 ```shell
 nano ~/.bash_profile
 ```
 And the following line to the `.bash_profile` with the actual path of the [package_name] script
 ```shell
 export PATH="/path/to/package:$PATH"
 ```
-For Python 3.15 on MacOS 14
+For Python 3.11.5 on MacOS 14
 ```shell
 export PATH="/Library/Frameworks/Python.framework/Versions/3.11/lib/python3.11/site-packages/pais-accomplishments-tool/paisAccTool.py:$PATH"
 ```
 
-### Simple use
+### Simple usage
 #### Help
 For watch help message run [paisAccTool.py](pais-accomplishments-tool/paisAccTool.py):
 ```shell
 python3 paisAccTool.py -h
 ```
 
 #### Sample
@@ -92,70 +95,65 @@
 ```shell
 Hello everyone!
 This is the micro tools for contain and formating accomplishments from BibTex source
  [ ]  misc accomplishment: rand1        done
  [ ]  misc accomplishment: rand2        done
  [ ]  misc accomplishment: rand3        done
  [ ]  misc accomplishment: rand4        done
-1. Наставник образовательной программы Звездный путь.Зима, Иван Иванов, Московского государственного университета, 2.2023
-2. Наставник образовательной программы Тёмная материя.Весна, Мария Петрова, Санкт-петербургского государственного университета, 4.2023
-3. Победитель образовательной программы Космос.Лето, Алексей Сидоров, Новосибирского государственного университета, 6.2023
-4. Участник олимпиады искусственный интеллект.Осень, Екатерина Кузнецова, Томского государственного университета, 9.2023
-
+ [ ]  conf accomplishment: conf1        done
+1. Наставник образовательной программы Звездный путь.Зима, разработка системы автоматизированного тестирования : Московского государственного университета : 15.02.2023
+2. Наставник образовательной программы Тёмная материя.Весна, Разработка системы машинного обучения : Санкт-петербургского государственного университета : 2023-04-10 00:00:00
+3. Победитель образовательной программы Космос.Лето, Разработка системы компьютерного зрения : Новосибирского государственного университета : 2023-06-20 00:00:00
+4. Участник олимпиады искусственный интеллект.Осень, Разработка системы естественного языка : Томского государственного университета : 2023-09-15 00:00:00
+5. Публикация "Система NLP для марсианского языка" : Екатерина Кузнецова : Студенческая конференция Масла и Камня, Банка Китая : 11.04.2023
 ```
 #### Common usage format
 ```shell
 python3 paisAccTool.py <source .bib file> [-d <destination>, -t "template string", -m "field" "for" "transformation", -c, -en]
 ```
 
--
-- `-t "template"` contain a python string template that will be used to generate the list of accomplishments. **Important, a template can only contain the bibtex field names of an object**;
-- `-m <"words", " " ..>` contain bibtex fields of the object, which are required to be put in the gent case;
+- `--config` path to config file.
 - `-c` mean that each new entry will start with a capital letter;
 - `-en` mean that the list of accomplishments will be output with numbering.
 
 ```shell
+usage: paisAccTool.py [-h] [-d DESTINATION] [--config CONFIG] [-c] [-en] source
+
 The micro tools for contain and formating accomplishments from BibTex source
 
 positional arguments:
   source                Path to source .bib file
 
 options:
   -h, --help            show this help message and exit
   -d DESTINATION, --destination DESTINATION
                         Path to destination .bib file
-  -t TEMPLATE, --template TEMPLATE
-                        A template string for generating accomplishment string. Default: {prefix} {type} {title}, {author}, {organization}, {month}.{year}
-  -m MORPHS [MORPHS ...], --morphs MORPHS [MORPHS ...]
-                        A list of fields for morphological transformations. Default: ('type', 'organization')
+  --config CONFIG       Path to config.yml file
   -c, --capitalize      Flag
   -en, --enumerate      Flag
 
+
 ```
 
 #### Other usage sample
 Command to output the list of accomplishments to a file
 ```shell
 python3 paisAccTool.py accomplishments_sample.bib -c -en -d output.txt
 ```
 
-Command with its own output template
+Command with its own custom config. You can make a config file along the [sample](#config-file).
 ```shell
-python3 paisAccTool.py accomplishments_sample.bib -t "{prefix} {type} {title}, {author}, {organization}, {location} {start}-{end}"
-```
-
-Command with its own morphological transformations fields
-```shell
-python3 paisAccTool.py accomplishments_sample.bib -m "title", "author", "type"
+python3 paisAccTool.py accomplishments_sample.bib --config /path/to/config.yml
 ```
 
 ### Accomplishments format
 
 Each accomplishment is stored in a .bib file in bibtex format.
-Below are the fields that are used to store achievements:
+
+**Below are the fields that are used to store misc achievements.**
 ```bibtex
 @misc{identifier,
 	prefix = {Твоя роль на мероприятии},
 	title = {Название мероприятия},
 	type = {Тип мероприятия},
 	author = {ФИО},
 	organization = {Организация, которая проводит мероприятие},
@@ -166,14 +164,58 @@
 	end = {дата окончания},
 	year = {год},
 	month = {месяц},
 	certificate = {результат, документ подтверждающий результат или участие (диплом, ...)},
 	order = {место в конкурсе или статус на мероприятии}
 }
 ```
+**Below are the fields that are used to store conf achievements.**
+```bibtex
+@conf{conf1,
+	prefix = {публикация},
+	title = {Студенческая конференция Масла и Камня},
+	type = {конференция},
+	author = {Екатерина Кузнецова},
+	organization = {Банк Китая},
+	topic = {Система NLP для марсианского языка},
+	section = {},
+	location = {Зотеро},
+	url = {some url},
+	start = {11.04.2023},
+	end = {15.04.2023},
+	year = {2023},
+	month = {4},
+	certificate = {сборник},
+	order = {}
+}
+```
 If you do not have a field to enter your specific information, you can add such a field:
 ```bibtex
     <key> = {value}
 ```
 The Accomplishments.bib file can be stored locally on your pc or in a remote git repository, so every commit means a new achievement (very convenient).
 
+### Config file
+The Config file represent as a yaml file.
+Its format:
+```yaml
+kinds:
+  <entry_type>:
+    template: 'template string'
+    morphs:
+      - <field 1>
+      - <field 2>
+```
+For example, you can look on the default config:
+```yaml
+kinds:
+  misc:
+    template: '{prefix} {type} {title}, {section} : {organization} : {start}'
+    morphs:
+      - type
+      - organization
+  conf:
+    template: '{prefix} "{topic}" : {author} : {title}, {organization} : {start}'
+    morphs:
+      - organization
+```
```

