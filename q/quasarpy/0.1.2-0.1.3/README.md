# Comparing `tmp/quasarpy-0.1.2.tar.gz` & `tmp/quasarpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.2.tar", max compression
+gzip compressed data, was "quasarpy-0.1.3.tar", max compression
```

## Comparing `quasarpy-0.1.2.tar` & `quasarpy-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,34 @@
--rw-r--r--   0        0        0    31941 2024-04-28 12:24:29.197163 quasarpy-0.1.2/LICENSE
--rw-r--r--   0        0        0      628 2024-04-28 12:24:29.197163 quasarpy-0.1.2/README.md
--rw-r--r--   0        0        0     1044 2024-04-28 12:24:29.205163 quasarpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2748 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4494 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-04-28 12:24:29.205163 quasarpy-0.1.2/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 quasarpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-04-28 18:46:22.726652 quasarpy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      530 2024-04-28 18:46:22.726652 quasarpy-0.1.3/README.md
+-rw-r--r--   0        0        0  1387623 2024-04-28 18:46:22.726652 quasarpy-0.1.3/assets/logo_complete.png
+-rw-r--r--   0        0        0   127970 2024-04-28 18:46:22.730652 quasarpy-0.1.3/assets/logo_complete_svg.svg
+-rw-r--r--   0        0        0   182267 2024-04-28 18:46:22.730652 quasarpy-0.1.3/assets/logo_complete_tbg.png
+-rw-r--r--   0        0        0   418415 2024-04-28 18:46:22.730652 quasarpy-0.1.3/assets/logo_icon.png
+-rw-r--r--   0        0        0   166944 2024-04-28 18:46:22.730652 quasarpy-0.1.3/assets/logo_text.png
+-rw-r--r--   0        0        0     1062 2024-04-28 18:46:22.734652 quasarpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2748 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4494 2024-04-28 18:46:22.734652 quasarpy-0.1.3/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-04-28 18:46:22.738652 quasarpy-0.1.3/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 quasarpy-0.1.3/PKG-INFO
```

### Comparing `quasarpy-0.1.2/LICENSE` & `quasarpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/pyproject.toml` & `quasarpy-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
-license = "GNU GENERAL PUBLIC LICENSE"
+license = "GPL-3.0-or-later"
 readme = "README.md"
+include = ["assets", 'LICENSE']
 
 [tool.poetry.scripts]
-quasar = "quasarpy.cli:main"
+quasar = "quasarpy:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.2.6"
 click = "^8.1.7"
 pytest = "^8.0.0"
 python-dotenv = "^1.0.1"
```

### Comparing `quasarpy-0.1.2/quasarpy/__init__.py` & `quasarpy-0.1.3/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/algorithm/detector.py` & `quasarpy-0.1.3/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/algorithm/llm.py` & `quasarpy-0.1.3/quasarpy/algorithm/llm.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.1.3/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.1.3/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/cli/__init__.py` & `quasarpy-0.1.3/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/handler/issue.py` & `quasarpy-0.1.3/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/tests/test_handler.py` & `quasarpy-0.1.3/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/tests/test_utils.py` & `quasarpy-0.1.3/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/utils/analyser.py` & `quasarpy-0.1.3/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/utils/ascii.py` & `quasarpy-0.1.3/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/utils/prompt_template.py` & `quasarpy-0.1.3/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/utils/redis_server.py` & `quasarpy-0.1.3/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/quasarpy/utils/templates/report_template.html` & `quasarpy-0.1.3/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.2/PKG-INFO` & `quasarpy-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: quasarpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc.
-License: GNU GENERAL PUBLIC LICENSE
+License: GPL-3.0-or-later
 Author: Khushiyant
 Author-email: khushiyant2002@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
@@ -29,20 +29,20 @@
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: xgboost (>=2.0.3,<3.0.0)
 Requires-Dist: xhtml2pdf (>=0.2.15,<0.3.0)
 Description-Content-Type: text/markdown
 
-<img src="https://github.com/Khushiyant/quasarpy/tree/main/assets/logo_complete_svg.svg" width="300" height="300" />
+<img src="assets/logo_complete_svg.svg" width="300" height="300" />
 
 ## Overview
 ![GitHub](https://img.shields.io/github/license/Khushiyant/quasar?&style=for-the-badge)
 ![Python](https://img.shields.io/badge/Made%20With%20Python-lightblue?logo=python&&style=for-the-badge&logoColor=black)
 
 Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc. 
 
 
 
 ## License
 
-This project is licensed under the GPL License - see the [LICENSE](https://github.com/Khushiyant/quasarpy/blob/main/LICENSE) file for details
+This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details
```

