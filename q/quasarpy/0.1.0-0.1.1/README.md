# Comparing `tmp/quasarpy-0.1.0.tar.gz` & `tmp/quasarpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.0.tar", max compression
+gzip compressed data, was "quasarpy-0.1.1.tar", max compression
```

## Comparing `quasarpy-0.1.0.tar` & `quasarpy-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    31941 2024-04-28 11:57:25.732647 quasarpy-0.1.0/LICENSE
--rw-r--r--   0        0        0      530 2024-04-28 11:57:25.732647 quasarpy-0.1.0/README.md
--rw-r--r--   0        0        0      992 2024-04-28 11:57:25.740647 quasarpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2549 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-04-28 11:57:25.740647 quasarpy-0.1.0/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4494 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-04-28 11:57:25.744647 quasarpy-0.1.0/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 quasarpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-04-28 12:15:31.480987 quasarpy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      628 2024-04-28 12:15:31.480987 quasarpy-0.1.1/README.md
+-rw-r--r--   0        0        0      992 2024-04-28 12:15:31.492987 quasarpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2549 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4494 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-04-28 12:15:31.492987 quasarpy-0.1.1/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 quasarpy-0.1.1/PKG-INFO
```

### Comparing `quasarpy-0.1.0/LICENSE` & `quasarpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/pyproject.toml` & `quasarpy-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GNU GENERAL PUBLIC LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `quasarpy-0.1.0/quasarpy/__init__.py` & `quasarpy-0.1.1/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/algorithm/detector.py` & `quasarpy-0.1.1/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/algorithm/llm.py` & `quasarpy-0.1.1/quasarpy/algorithm/llm.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.1.1/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.1.1/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/cli/__init__.py` & `quasarpy-0.1.1/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/handler/issue.py` & `quasarpy-0.1.1/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/tests/test_handler.py` & `quasarpy-0.1.1/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/tests/test_utils.py` & `quasarpy-0.1.1/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/utils/analyser.py` & `quasarpy-0.1.1/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/utils/ascii.py` & `quasarpy-0.1.1/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/utils/prompt_template.py` & `quasarpy-0.1.1/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/utils/redis_server.py` & `quasarpy-0.1.1/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/quasarpy/utils/templates/report_template.html` & `quasarpy-0.1.1/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.0/PKG-INFO` & `quasarpy-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasarpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc.
 License: GNU GENERAL PUBLIC LICENSE
 Author: Khushiyant
 Author-email: khushiyant2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -29,20 +29,20 @@
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: xgboost (>=2.0.3,<3.0.0)
 Requires-Dist: xhtml2pdf (>=0.2.15,<0.3.0)
 Description-Content-Type: text/markdown
 
-<img src="assets/logo_complete_svg.svg" width="300" height="300" />
+<img src="https://github.com/Khushiyant/quasarpy/tree/main/assets/logo_complete_svg.svg" width="300" height="300" />
 
 ## Overview
 ![GitHub](https://img.shields.io/github/license/Khushiyant/quasar?&style=for-the-badge)
 ![Python](https://img.shields.io/badge/Made%20With%20Python-lightblue?logo=python&&style=for-the-badge&logoColor=black)
 
 Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc. 
 
 
 
 ## License
 
-This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details
+This project is licensed under the GPL License - see the [LICENSE](https://github.com/Khushiyant/quasarpy/blob/main/LICENSE) file for details
```

