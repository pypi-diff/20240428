# Comparing `tmp/pypomes_core-0.9.1.tar.gz` & `tmp/pypomes_core-0.9.2.tar.gz`

## Comparing `pypomes_core-0.9.1.tar` & `pypomes_core-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.2/PKG-INFO
```

### Comparing `pypomes_core-0.9.1/src/pypomes_core/.ruff.toml` & `pypomes_core-0.9.2/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/__init__.py` & `pypomes_core-0.9.2/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/email_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/env_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/file_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/json_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/list_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/str_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.9.2/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/validation_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import date, datetime
 from logging import Logger
 from typing import Final
 from .datetime_pomes import TIMEZONE_LOCAL
 from .env_pomes import APP_PREFIX, env_get_str
 from .str_pomes import str_sanitize, str_find_whitespace
 
-VALIDATE_MSG_LANGUAGE: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_LANGUAGE", "pt")
+VALIDATE_MSG_LANGUAGE: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_LANGUAGE", "en")
 VALIDATE_MSG_PREFIX: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_PREFIX", APP_PREFIX)
 
 
 def validate_value(attr: str,
                    val: str | int | float,
                    min_val: int = None,
                    max_val: int = None,
```

### Comparing `pypomes_core-0.9.1/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.9.2/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/LICENSE` & `pypomes_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.1/pyproject.toml` & `pypomes_core-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.9.1/PKG-INFO` & `pypomes_core-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

