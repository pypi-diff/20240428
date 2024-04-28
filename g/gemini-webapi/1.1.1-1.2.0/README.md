# Comparing `tmp/gemini-webapi-1.1.1.tar.gz` & `tmp/gemini_webapi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini-webapi-1.1.1.tar", last modified: Fri Apr  5 03:32:45 2024, max compression
+gzip compressed data, was "gemini_webapi-1.2.0.tar", last modified: Sun Apr 28 09:01:25 2024, max compression
```

## Comparing `gemini-webapi-1.1.1.tar` & `gemini_webapi-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.438973 gemini-webapi-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.442973 gemini-webapi-1.1.1/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 03:32:45.000000 gemini-webapi-1.1.1/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:32:45.446973 gemini-webapi-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 03:32:40.000000 gemini-webapi-1.1.1/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.927631 gemini_webapi-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.927631 gemini_webapi-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_save_image.py
```

### Comparing `gemini-webapi-1.1.1/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.2.0/.github/workflows/pypi-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 name: Build and Publish
 
 on:
   push:
     tags:
-    - 'v[0-9]+.[0-9]+.[0-9]+'
+      - 'v[0-9]+.[0-9]+.[0-9]+'
   workflow_dispatch:
     inputs:
       logLevel:
         description: 'Log level'
         required: true
         default: 'warning'
         type: choice
         options:
-        - info
-        - warning
-        - debug
+          - info
+          - warning
+          - debug
 
 permissions:
   contents: read
 
 jobs:
   build:
     name: Build package
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
-    - name: Set up Python
-      uses: actions/setup-python@v5
-      with:
-        python-version: '3.x'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install build
-    - name: Build package
-      run: python -m build
-    - name: Archive production artifacts
-      uses: actions/upload-artifact@v4.0.0
-      with:
-        name: dist
-        path: dist
+      - uses: actions/checkout@v4
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: '3.x'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install build
+      - name: Build package
+        run: python -m build
+      - name: Archive production artifacts
+        uses: actions/upload-artifact@v4.0.0
+        with:
+          name: dist
+          path: dist
 
   pypi-publish:
     name: Upload release to PyPI
     needs: build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/gemini-webapi
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
-    - name: Retrieve built artifacts
-      uses: actions/download-artifact@v4.1.0
-      with:
-        name: dist
-        path: dist
-    - name: Publish package distributions to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.8.11
+      - name: Retrieve built artifacts
+        uses: actions/download-artifact@v4.1.0
+        with:
+          name: dist
+          path: dist
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@v1.8.11
```

### Comparing `gemini-webapi-1.1.1/.gitignore` & `gemini_webapi-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/LICENSE` & `gemini_webapi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/PKG-INFO` & `gemini_webapi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.1.1
+Version: 1.2.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini-webapi-1.1.1/README.md` & `gemini_webapi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/assets/banner.png` & `gemini_webapi-1.2.0/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/assets/logo.svg` & `gemini_webapi-1.2.0/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/pyproject.toml` & `gemini_webapi-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/client.py` & `gemini_webapi-1.2.0/src/gemini_webapi/client.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/constants.py` & `gemini_webapi-1.2.0/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.2.0/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.2.0/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/types/image.py` & `gemini_webapi-1.2.0/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.2.0/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.2.0/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.2.0/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import browser_cookie3 as bc3
-
 from .logger import logger
 
 
 def load_browser_cookies(domain_name: str = "", verbose=True) -> dict:
     """
     Try to load cookies from all supported browsers and return combined cookiejar.
     Optionally pass in a domain name to only load cookies from the specified domain.
@@ -16,14 +14,16 @@
         If `True`, will print more infomation in logs.
 
     Returns
     -------
     `dict`
         Dictionary with cookie name as key and cookie value as value.
     """
+    import browser_cookie3 as bc3
+
     cookies = {}
     for cookie_fn in [
         bc3.chrome,
         bc3.chromium,
         bc3.opera,
         bc3.opera_gx,
         bc3.brave,
```

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.2.0/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.2.0/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.2.0/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.2.0/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.1.1
+Version: 1.2.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini-webapi-1.1.1/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.2.0/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/tests/test_client_features.py` & `gemini_webapi-1.2.0/tests/test_client_features.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/tests/test_rotate_cookies.py` & `gemini_webapi-1.2.0/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini-webapi-1.1.1/tests/test_save_image.py` & `gemini_webapi-1.2.0/tests/test_save_image.py`

 * *Files identical despite different names*

