# Comparing `tmp/webviewpy-0.0.2.tar.gz` & `tmp/webviewpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webviewpy-0.0.2.tar", last modified: Tue Jan 23 22:37:22 2024, max compression
+gzip compressed data, was "webviewpy-0.0.3.tar", last modified: Sun Apr 28 09:21:30 2024, max compression
```

## Comparing `webviewpy-0.0.2.tar` & `webviewpy-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.630567 webviewpy-0.0.2/
--rw-rw-rw-   0        0        0       66 2024-01-23 14:39:21.000000 webviewpy-0.0.2/.gitattributes
--rw-rw-rw-   0        0        0       54 2024-01-23 18:25:54.000000 webviewpy-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1079 2024-01-23 17:10:07.000000 webviewpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1190 2024-01-23 22:37:22.629575 webviewpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      687 2024-01-23 18:55:06.000000 webviewpy-0.0.2/README.md
--rw-rw-rw-   0        0        0      835 2024-01-23 22:36:50.000000 webviewpy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-23 22:37:22.631568 webviewpy-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.577183 webviewpy-0.0.2/test/
--rw-rw-rw-   0        0        0     1788 2024-01-23 17:25:22.000000 webviewpy-0.0.2/test/test.py
--rw-rw-rw-   0        0        0      545 2024-01-23 22:36:33.000000 webviewpy-0.0.2/test/testpyqt.py
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.592809 webviewpy-0.0.2/webviewpy/
--rw-rw-rw-   0        0        0     6352 2024-01-23 22:36:06.000000 webviewpy-0.0.2/webviewpy/__init__.py
--rw-rw-rw-   0        0        0      476 2024-01-23 22:37:22.000000 webviewpy-0.0.2/webviewpy/__version__.py
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.554433 webviewpy-0.0.2/webviewpy/platform/
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.554433 webviewpy-0.0.2/webviewpy/platform/win32/
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.624566 webviewpy-0.0.2/webviewpy/platform/win32/x64/
--rw-rw-rw-   0        0        0   219648 2024-01-23 22:34:07.000000 webviewpy-0.0.2/webviewpy/platform/win32/x64/webview.dll
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.625569 webviewpy-0.0.2/webviewpy/platform/win32/x86/
--rw-rw-rw-   0        0        0   163328 2024-01-23 22:34:47.000000 webviewpy-0.0.2/webviewpy/platform/win32/x86/webview.dll
-drwxrwxrwx   0        0        0        0 2024-01-23 22:37:22.628568 webviewpy-0.0.2/webviewpy.egg-info/
--rw-rw-rw-   0        0        0     1190 2024-01-23 22:37:22.000000 webviewpy-0.0.2/webviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-01-23 22:37:22.000000 webviewpy-0.0.2/webviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-23 22:37:22.000000 webviewpy-0.0.2/webviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-01-23 22:37:22.000000 webviewpy-0.0.2/webviewpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:21:30.874230 webviewpy-0.0.3/
+-rw-rw-rw-   0        0        0       68 2024-04-28 07:27:46.000000 webviewpy-0.0.3/.gitattributes
+-rw-rw-rw-   0        0        0       72 2024-04-28 08:21:15.000000 webviewpy-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0       84 2024-04-28 08:12:02.000000 webviewpy-0.0.3/.gitmodules
+-rw-rw-rw-   0        0        0     1098 2024-04-28 07:27:46.000000 webviewpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      910 2024-04-28 09:21:30.874230 webviewpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-28 08:12:26.000000 webviewpy-0.0.3/README.md
+-rw-rw-rw-   0        0        0      835 2024-04-28 09:18:54.000000 webviewpy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:21:30.874230 webviewpy-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 09:21:30.865028 webviewpy-0.0.3/test/
+-rw-rw-rw-   0        0        0     2129 2024-04-28 07:43:09.000000 webviewpy-0.0.3/test/test.py
+-rw-rw-rw-   0        0        0      881 2024-04-28 08:10:09.000000 webviewpy-0.0.3/test/testpyqt.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:21:30.867473 webviewpy-0.0.3/webviewpy/
+-rw-rw-rw-   0        0        0    10496 2024-04-28 07:32:59.000000 webviewpy-0.0.3/webviewpy/__init__.py
+-rw-rw-rw-   0        0        0      458 2024-04-28 09:21:30.000000 webviewpy-0.0.3/webviewpy/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:21:30.874230 webviewpy-0.0.3/webviewpy/platform/
+-rw-rw-rw-   0        0        0        0 2024-04-28 09:19:22.000000 webviewpy-0.0.3/webviewpy/platform/.keepdir
+drwxrwxrwx   0        0        0        0 2024-04-28 09:21:30.874230 webviewpy-0.0.3/webviewpy.egg-info/
+-rw-rw-rw-   0        0        0      910 2024-04-28 09:21:30.000000 webviewpy-0.0.3/webviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-28 09:21:30.000000 webviewpy-0.0.3/webviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:21:30.000000 webviewpy-0.0.3/webviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-28 09:21:30.000000 webviewpy-0.0.3/webviewpy.egg-info/top_level.txt
```

### Comparing `webviewpy-0.0.2/LICENSE` & `webviewpy-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2013, Aldo Cortesi. All rights reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2013, Aldo Cortesi. All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `webviewpy-0.0.2/PKG-INFO` & `webviewpy-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviewpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: ctypes binding of webview
 Author-email: HIllya51 <1871535768@qq.com>
 Project-URL: Homepage, https://github.com/HIllya51/webviewpy
 Project-URL: Repository, https://github.com/HIllya51/webviewpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,20 +24,12 @@
 ### Install
 
 
 ``` bash
 pip install webviewpy
 ```
 
-### Additional operation for Linux or MacOS
-
-The runtime of webview for Linux or MacOS must build by yourself
-
-git clone [webview](https://github.com/webview/webview) and build the dynalib or so library
-
-copy the library file to webviewpy/platform/[linux or darwin]/[x86 or x64]
-
 ### Usage
 
-[Build a webview based app](https://github.com/HIllya51/webviewpy/tree/main/test)
+[Build a webview based app](https://github.com/HIllya51/webviewpy/tree/main/test/test.py)
 
 [Embed a webview in you window like QWidget](https://github.com/HIllya51/webviewpy/blob/main/test/testpyqt.py)
```

### Comparing `webviewpy-0.0.2/README.md` & `webviewpy-0.0.3/webviewpy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: webviewpy
+Version: 0.0.3
+Summary: ctypes binding of webview
+Author-email: HIllya51 <1871535768@qq.com>
+Project-URL: Homepage, https://github.com/HIllya51/webviewpy
+Project-URL: Repository, https://github.com/HIllya51/webviewpy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # webviewpy
 
 A tiny webview library for Python.
 
 Based on [webview](https://github.com/webview/webview)
 
 
@@ -10,20 +24,12 @@
 ### Install
 
 
 ``` bash
 pip install webviewpy
 ```
 
-### Additional operation for Linux or MacOS
-
-The runtime of webview for Linux or MacOS must build by yourself
-
-git clone [webview](https://github.com/webview/webview) and build the dynalib or so library
-
-copy the library file to webviewpy/platform/[linux or darwin]/[x86 or x64]
-
 ### Usage
 
-[Build a webview based app](https://github.com/HIllya51/webviewpy/tree/main/test)
+[Build a webview based app](https://github.com/HIllya51/webviewpy/tree/main/test/test.py)
 
-[Embed a webview in you window like QWidget](https://github.com/HIllya51/webviewpy/blob/main/test/testpyqt.py)
+[Embed a webview in you window like QWidget](https://github.com/HIllya51/webviewpy/blob/main/test/testpyqt.py)
```

### Comparing `webviewpy-0.0.2/pyproject.toml` & `webviewpy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webviewpy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="HIllya51", email="1871535768@qq.com" },
 ]
 
 description = "ctypes binding of webview"
 readme = "README.md"
```

