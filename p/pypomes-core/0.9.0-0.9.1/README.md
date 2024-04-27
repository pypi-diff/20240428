# Comparing `tmp/pypomes_core-0.9.0.tar.gz` & `tmp/pypomes_core-0.9.1.tar.gz`

## Comparing `pypomes_core-0.9.0.tar` & `pypomes_core-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,20 @@
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/make.bat
--rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/index.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/search.html
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/source/conf.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/docs/source/index.rst
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/PKG-INFO
```

### Comparing `pypomes_core-0.9.0/src/pypomes_core/.ruff.toml` & `pypomes_core-0.9.1/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/__init__.py` & `pypomes_core-0.9.1/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/email_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/env_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/file_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/json_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/list_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/str_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.9.1/src/pypomes_core/validation_msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,22 @@
         "en": "A value has not yet been assigned",
         "pt": "Valor ainda não foi atribuído",
     },
     116: {
         "en": "Value {} cannot be assigned for attributes {} at the same time",
         "pt": "Valor {} não pode ser atribuído aos atributos {} ao mesmo tempo",
     },
+    117: {
+        "en": "Invalid value {}: must be less than {}",
+        "pt": "Valor {} inválido: deve ser menor que {}",
+    },
+    118: {
+        "en": "Invalid value {}: must be greater than {}",
+        "pt": "Valor {} inválido: deve ser maior que {}",
+    },
     121: {
         "en": "Invalid value {}",
         "pt": "Valor {} inválido",
     },
     122: {
         "en": "Invalid value {}: length shorter than {}",
         "pt": "Valor {} inválido: comprimento menor que {}",
```

### Comparing `pypomes_core-0.9.0/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/validation_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,23 @@
             # 123: Invalid value {}: length longer than {}
             result = validate_format_error(123, val, max_val, f"@{attr}")
         elif min_val is not None and length < min_val:
             # 122: Invalid value {}: length shorter than {}
             result = validate_format_error(122, val, min_val, f"@{attr}")
     elif (min_val is not None and val < min_val) or \
          (max_val is not None and val > max_val):
-        # 127: Invalid value {}: must be in the range {}
-        result = validate_format_error(127, val, [min_val, max_val], f"@{attr}")
+        if min_val is not None and max_val is not None:
+            # 127: Invalid value {}: must be in the range {}
+            result = validate_format_error(127, val, [min_val, max_val], f"@{attr}")
+        elif min_val is not None:
+            # 118: Invalid value {}: must be greater than {}
+            result = validate_format_error(118, val, min_val, f"@{attr}")
+        else:
+            # 117: Invalid value {}: must be less than {}
+            result = validate_format_error(117, val, max_val, f"@{attr}")
 
     return result
 
 
 def validate_bool(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
```

### Comparing `pypomes_core-0.9.0/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.9.1/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/LICENSE` & `pypomes_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.0/pyproject.toml` & `pypomes_core-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.9.0/PKG-INFO` & `pypomes_core-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

