# Comparing `tmp/quasarpy-0.1.4.tar.gz` & `tmp/quasarpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.4.tar", max compression
+gzip compressed data, was "quasarpy-0.1.5.tar", max compression
```

## Comparing `quasarpy-0.1.4.tar` & `quasarpy-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31941 2024-04-28 18:54:34.904329 quasarpy-0.1.4/LICENSE
--rw-r--r--   0        0        0      700 2024-04-28 18:54:34.904329 quasarpy-0.1.4/README.md
--rw-r--r--   0        0        0  1387623 2024-04-28 18:54:34.908329 quasarpy-0.1.4/assets/logo_complete.png
--rw-r--r--   0        0        0   127970 2024-04-28 18:54:34.908329 quasarpy-0.1.4/assets/logo_complete_svg.svg
--rw-r--r--   0        0        0   182267 2024-04-28 18:54:34.908329 quasarpy-0.1.4/assets/logo_complete_tbg.png
--rw-r--r--   0        0        0   418415 2024-04-28 18:54:34.912329 quasarpy-0.1.4/assets/logo_icon.png
--rw-r--r--   0        0        0   166944 2024-04-28 18:54:34.912329 quasarpy-0.1.4/assets/logo_text.png
--rw-r--r--   0        0        0     1062 2024-04-28 18:54:34.916329 quasarpy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2748 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4494 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-04-28 18:54:34.916329 quasarpy-0.1.4/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 quasarpy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-04-28 19:43:19.608506 quasarpy-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1399 2024-04-28 19:43:19.608506 quasarpy-0.1.5/README.md
+-rw-r--r--   0        0        0  1387623 2024-04-28 19:43:19.612506 quasarpy-0.1.5/assets/logo_complete.png
+-rw-r--r--   0        0        0   127970 2024-04-28 19:43:19.612506 quasarpy-0.1.5/assets/logo_complete_svg.svg
+-rw-r--r--   0        0        0   182267 2024-04-28 19:43:19.612506 quasarpy-0.1.5/assets/logo_complete_tbg.png
+-rw-r--r--   0        0        0   418415 2024-04-28 19:43:19.616506 quasarpy-0.1.5/assets/logo_icon.png
+-rw-r--r--   0        0        0   166944 2024-04-28 19:43:19.616506 quasarpy-0.1.5/assets/logo_text.png
+-rw-r--r--   0        0        0     1062 2024-04-28 19:43:19.620506 quasarpy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2748 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4494 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-04-28 19:43:19.620506 quasarpy-0.1.5/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     2860 1970-01-01 00:00:00.000000 quasarpy-0.1.5/PKG-INFO
```

### Comparing `quasarpy-0.1.4/LICENSE` & `quasarpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/assets/logo_complete.png` & `quasarpy-0.1.5/assets/logo_complete.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/assets/logo_complete_svg.svg` & `quasarpy-0.1.5/assets/logo_complete_svg.svg`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/assets/logo_complete_tbg.png` & `quasarpy-0.1.5/assets/logo_complete_tbg.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/assets/logo_icon.png` & `quasarpy-0.1.5/assets/logo_icon.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/assets/logo_text.png` & `quasarpy-0.1.5/assets/logo_text.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/pyproject.toml` & `quasarpy-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.4"
+version = "0.1.5"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 include = ["assets", 'LICENSE']
 
 [tool.poetry.scripts]
```

### Comparing `quasarpy-0.1.4/quasarpy/__init__.py` & `quasarpy-0.1.5/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/algorithm/detector.py` & `quasarpy-0.1.5/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/algorithm/llm.py` & `quasarpy-0.1.5/quasarpy/algorithm/llm.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.1.5/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.1.5/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/cli/__init__.py` & `quasarpy-0.1.5/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/handler/issue.py` & `quasarpy-0.1.5/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/tests/test_handler.py` & `quasarpy-0.1.5/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/tests/test_utils.py` & `quasarpy-0.1.5/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/utils/analyser.py` & `quasarpy-0.1.5/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/utils/ascii.py` & `quasarpy-0.1.5/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/utils/prompt_template.py` & `quasarpy-0.1.5/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/utils/redis_server.py` & `quasarpy-0.1.5/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.4/quasarpy/utils/templates/report_template.html` & `quasarpy-0.1.5/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

