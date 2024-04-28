# Comparing `tmp/zundler-0.0.0.tar.gz` & `tmp/zundler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zundler-0.0.0.tar", last modified: Mon Apr 22 18:46:04 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `zundler-0.0.0.tar` & `zundler-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,57 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.606800 zundler-0.0.0/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1071 2024-04-21 16:04:20.000000 zundler-0.0.0/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)       59 2024-04-21 16:04:20.000000 zundler-0.0.0/MANIFEST.in
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5562 2024-04-22 18:46:04.606800 zundler-0.0.0/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4242 2024-04-21 16:04:20.000000 zundler-0.0.0/README.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1759 2024-04-21 21:57:37.000000 zundler-0.0.0/pyproject.toml
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2024-04-22 18:46:04.606800 zundler-0.0.0/setup.cfg
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.598800 zundler-0.0.0/tests/
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.602800 zundler-0.0.0/tests/demo001/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      634 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/Makefile
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.602800 zundler-0.0.0/tests/demo001/_static/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      621 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/_static/custom.css
--rw-r--r--   0 adrian    (1000) adrian    (1000)      546 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/_static/logo-square.svg
--rw-r--r--   0 adrian    (1000) adrian    (1000)      530 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/_static/logo-wide.svg
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4515 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/conf.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2410 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/first.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)      301 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/index.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14145 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/paragraph-markup.rst
--rw-r--r--   0 adrian    (1000) adrian    (1000)       92 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/requirements.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2263 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/second.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3914 2024-04-21 16:04:20.000000 zundler-0.0.0/tests/demo001/third.md
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3339 2024-04-22 18:44:42.000000 zundler-0.0.0/tests/test_zundler.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.602800 zundler-0.0.0/zundler/
--rw-r--r--   0 adrian    (1000) adrian    (1000)        0 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      484 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/__main__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1591 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/args.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.606800 zundler-0.0.0/zundler/assets/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3299 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1211 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/init.css
--rw-r--r--   0 adrian    (1000) adrian    (1000)       76 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/init.html
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2970 2024-04-22 18:37:16.000000 zundler-0.0.0/zundler/assets/inject_post.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3688 2024-04-22 18:40:37.000000 zundler-0.0.0/zundler/assets/inject_pre.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)    44260 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/pako.min.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)      618 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/zundler_bootstrap.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3482 2024-04-22 18:41:20.000000 zundler-0.0.0/zundler/assets/zundler_common.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8020 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/assets/zundler_main.js
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10149 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/embed.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.606800 zundler-0.0.0/zundler/sphinxext/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2550 2024-04-21 16:04:20.000000 zundler-0.0.0/zundler/sphinxext/__init__.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-22 18:46:04.606800 zundler-0.0.0/zundler.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5562 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)      982 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/SOURCES.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/dependency_links.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)       97 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/entry_points.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2022-10-04 20:28:36.000000 zundler-0.0.0/zundler.egg-info/not-zip-safe
--rw-r--r--   0 adrian    (1000) adrian    (1000)       47 2023-09-30 15:41:53.000000 zundler-0.0.0/zundler.egg-info/pbr.json
--rw-r--r--   0 adrian    (1000) adrian    (1000)       93 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/requires.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2024-04-22 18:46:04.000000 zundler-0.0.0/zundler.egg-info/top_level.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zundler-0.1.0/.flake8
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 zundler-0.1.0/Makefile
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 zundler-0.1.0/_version.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 zundler-0.1.0/noxfile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/__main__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/args.py
+-rw-r--r--   0        0        0    10202 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/embed.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/LICENSE
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/init.css
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/init.html
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/inject_post.js
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/inject_pre.js
+-rw-r--r--   0        0        0    44260 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/pako.min.js
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/zundler_bootstrap.js
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/zundler_common.js
+-rw-r--r--   0        0        0    13851 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/assets/zundler_main.js
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 zundler-0.1.0/src/zundler/sphinxext/__init__.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/test_zundler.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/copy-button/conf.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/copy-button/index.rst
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/copy-button/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/dark-mode/conf.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/dark-mode/first.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/dark-mode/index.rst
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/dark-mode/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/Makefile
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/conf.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/first.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/index.md
+-rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/paragraph-markup.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/requirements.txt
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/second.md
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/third.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/_static/custom.css
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/_static/logo-square.svg
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo001/_static/logo-wide.svg
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo002/Makefile
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo002/conf.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo002/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/demo002/make.bat
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/mermaid/conf.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/mermaid/index.rst
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/mermaid/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/conf.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/first.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/index.rst
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/requirements.txt
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/second.rst
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 zundler-0.1.0/tests/multi-page/third.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 zundler-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 zundler-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zundler-0.1.0/README.md
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 zundler-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 zundler-0.1.0/PKG-INFO
```

### Comparing `zundler-0.0.0/LICENSE` & `zundler-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/PKG-INFO` & `zundler-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zundler
-Version: 0.0.0
+Version: 0.1.0
 Summary: Bundle assets of distributed HTML docs into one self-contained HTML file
-Author-email: Adrian Vollmer <computerfluesterer@protonmail.com>
 Project-URL: Homepage, https://github.com/AdrianVollmer/Zundler
+Author-email: Adrian Vollmer <computerfluesterer@protonmail.com>
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -15,26 +16,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sphinx
 Requires-Dist: lxml
 Requires-Dist: python-magic
+Requires-Dist: sphinx
 Provides-Extra: tests
-Requires-Dist: pytest>=8; extra == "tests"
-Requires-Dist: selenium; extra == "tests"
-Requires-Dist: pytest-selenium; extra == "tests"
-Requires-Dist: pytest-docker; extra == "tests"
-Requires-Dist: black; extra == "tests"
-Requires-Dist: nox; extra == "tests"
+Requires-Dist: black; extra == 'tests'
+Requires-Dist: nox; extra == 'tests'
+Requires-Dist: pytest-docker; extra == 'tests'
+Requires-Dist: pytest-selenium; extra == 'tests'
+Requires-Dist: pytest>=8; extra == 'tests'
+Requires-Dist: selenium; extra == 'tests'
+Description-Content-Type: text/markdown
 
 Zundler
 =======
 
 Bundle assets of distributed HTML docs into one self-contained HTML file.
 It's built with Sphinx in mind, but can be used on all HTML docs.
 
@@ -97,15 +97,15 @@
 
 Zundler is a Python package and can be installed like any other Python
 package.
 
 The recommended way is to run this:
 
 ```shell-session
-$ pip install git+https://github.com/AdrianVollmer/Zundler@main
+$ pip install zundler
 ```
 
 If you prefer an alternative like `pipx`, `poetry` or manually handled
 `venv`s, you probably know what to do.
 
 An entry point called `zundler` will appear in `~/.local/bin`.
```

#### html2text {}

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1 Name: zundler Version: 0.0.0 Summary: Bundle assets of
-distributed HTML docs into one self-contained HTML file Author-email: Adrian
-Vollmer
-protonmail.com> Project-URL: Homepage, https://github.com/AdrianVollmer/Zundler
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Documentation Classifier: Topic
-:: Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: sphinx Requires-Dist: lxml Requires-Dist:
-python-magic Provides-Extra: tests Requires-Dist: pytest>=8; extra == "tests"
-Requires-Dist: selenium; extra == "tests" Requires-Dist: pytest-selenium; extra
-== "tests" Requires-Dist: pytest-docker; extra == "tests" Requires-Dist: black;
-extra == "tests" Requires-Dist: nox; extra == "tests" Zundler ======= Bundle
-assets of distributed HTML docs into one self-contained HTML file. It's built
-with Sphinx in mind, but can be used on all HTML docs. > [!WARNING] > This is
-still experimental. Expect breakages! Feel free > to open an issue. Please
-provide everything that is necessary to reproduce > the problem. Naively
-building one HTML file out of a directory of HTML files that total dozens of
-megabytes quickly overwhelm modern browsers. Zundler solves this by taking the
-following approach: * Embed all assets that are referenced in CSS files, such
-as imports and fonts * Endow all HTML files with extra scripts that embed these
-resources at run time: * Convert `script` tags with a `src` attribute
-referencing a local JavaScript file to inline scripts * Convert `link` tags
-with an `href` attribute referencing a local CSS file to inline styles * Make
-all `img` tags with a `src` attribute referencing local images use a data URI *
-Monkey patch the JavaScript function `fetch` so requests to local files are
-turned into queries of the "virtual file tree" (see next item) * Monkey patch
-the JavaScript class `URLSearchParams` so GET requests to local files can be
-handeled; this is needed for Sphinx' search function, for example * Create a
-JSON structure (the "global context") out of all files in the directory (the
-"virtual file tree") and other data * Gzip the global context and base64-encode
-it * Bundle it all into a scuffolding file with this structure: ```html
+Metadata-Version: 2.3 Name: zundler Version: 0.1.0 Summary: Bundle assets of
+distributed HTML docs into one self-contained HTML file Project-URL: Homepage,
+https://github.com/AdrianVollmer/Zundler Author-email: Adrian Vollmer
+protonmail.com> License-File: LICENSE Classifier: Development Status :: 3 -
+Alpha Classifier: Environment :: Console Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Documentation Classifier: Topic :: Utilities Requires-Python: >=3.8
+Requires-Dist: lxml Requires-Dist: python-magic Requires-Dist: sphinx Provides-
+Extra: tests Requires-Dist: black; extra == 'tests' Requires-Dist: nox; extra
+== 'tests' Requires-Dist: pytest-docker; extra == 'tests' Requires-Dist:
+pytest-selenium; extra == 'tests' Requires-Dist: pytest>=8; extra == 'tests'
+Requires-Dist: selenium; extra == 'tests' Description-Content-Type: text/
+markdown Zundler ======= Bundle assets of distributed HTML docs into one self-
+contained HTML file. It's built with Sphinx in mind, but can be used on all
+HTML docs. > [!WARNING] > This is still experimental. Expect breakages! Feel
+free > to open an issue. Please provide everything that is necessary to
+reproduce > the problem. Naively building one HTML file out of a directory of
+HTML files that total dozens of megabytes quickly overwhelm modern browsers.
+Zundler solves this by taking the following approach: * Embed all assets that
+are referenced in CSS files, such as imports and fonts * Endow all HTML files
+with extra scripts that embed these resources at run time: * Convert `script`
+tags with a `src` attribute referencing a local JavaScript file to inline
+scripts * Convert `link` tags with an `href` attribute referencing a local CSS
+file to inline styles * Make all `img` tags with a `src` attribute referencing
+local images use a data URI * Monkey patch the JavaScript function `fetch` so
+requests to local files are turned into queries of the "virtual file tree" (see
+next item) * Monkey patch the JavaScript class `URLSearchParams` so GET
+requests to local files can be handeled; this is needed for Sphinx' search
+function, for example * Create a JSON structure (the "global context") out of
+all files in the directory (the "virtual file tree") and other data * Gzip the
+global context and base64-encode it * Bundle it all into a scuffolding file
+with this structure: ```html
 {body}
 ``` The global context is then unzipped using the Pako library, an `iframe` is
 created and the document is bootstrapped from the virtual file tree. The output
 file is usually smaller than the sum of all input files despite some resources
 being embedded redundantly and the 33% overhead of the base64 encoding.
 Limitations ----------- This approach is quite hacky, but it might work well
 enough for some purposes. * Some scripts may break as the execution flow is
 different than some scripts expect * HTML forms with `method="GET"` to local
 HTML files only work if the receiving code uses URLSearchParams, as same-origin
 policies forbid reading GET parameters otherwise * Opening links in a new tab
 won't work * Redirections won't work (yet) * Support of themes or extensions
 that require jQuery is wonky; fortunately Sphinx stopped supporting jQuery in
 version 6 Installation ------------ Zundler is a Python package and can be
 installed like any other Python package. The recommended way is to run this:
-```shell-session $ pip install git+https://github.com/AdrianVollmer/
-Zundler@main ``` If you prefer an alternative like `pipx`, `poetry` or manually
-handled `venv`s, you probably know what to do. An entry point called `zundler`
-will appear in `~/.local/bin`. Bundling Sphinx docs -------------------- The
-Zundler package provides a Sphinx extension that adds an appropriate builder.
-The builder is a thin wrapper around the HTML builder, which runs `zundler` at
-the end. It can be used with `sphinx-build -b zundler` or, if there is a
-suitable Makefile, with `make zundler`. Jupyter-Books can be built with
-`jupyter-book build --custom-builder zundler --builder custom .`. You may have
-to add a render priority for Zundler like [here](https://jupyterbook.org/en/
-stable/content/code-outputs.html#render-priority): ```yaml sphinx: config:
-nb_mime_priority_overrides: [ ["zundler", "application/vnd.jupyter.widget-
-view+json", 10], ["zundler", "application/javascript", 20], ["zundler", "text/
-html", 30], ["zundler", "image/svg+xml", 40], ["zundler", "image/png", 50],
-["zundler", "image/jpeg", 60], ["zundler", "text/markdown", 70], ["zundler",
-"text/latex", 80], ["zundler", "text/plain", 90] ] ``` Demos ----- Some demo
-documents are available here:
+```shell-session $ pip install zundler ``` If you prefer an alternative like
+`pipx`, `poetry` or manually handled `venv`s, you probably know what to do. An
+entry point called `zundler` will appear in `~/.local/bin`. Bundling Sphinx
+docs -------------------- The Zundler package provides a Sphinx extension that
+adds an appropriate builder. The builder is a thin wrapper around the HTML
+builder, which runs `zundler` at the end. It can be used with `sphinx-build -
+b zundler` or, if there is a suitable Makefile, with `make zundler`. Jupyter-
+Books can be built with `jupyter-book build --custom-builder zundler --builder
+custom .`. You may have to add a render priority for Zundler like [here](https:
+//jupyterbook.org/en/stable/content/code-outputs.html#render-priority): ```yaml
+sphinx: config: nb_mime_priority_overrides: [ ["zundler", "application/
+vnd.jupyter.widget-view+json", 10], ["zundler", "application/javascript", 20],
+["zundler", "text/html", 30], ["zundler", "image/svg+xml", 40], ["zundler",
+"image/png", 50], ["zundler", "image/jpeg", 60], ["zundler", "text/markdown",
+70], ["zundler", "text/latex", 80], ["zundler", "text/plain", 90] ] ``` Demos -
+---- Some demo documents are available here:
 adrianvollmer.github.io/Zundler> Copyright --------- Adrian Vollmer, 2022. MIT
 licensed; see `LICENSE` for details.
```

### Comparing `zundler-0.0.0/README.md` & `zundler-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 Zundler is a Python package and can be installed like any other Python
 package.
 
 The recommended way is to run this:
 
 ```shell-session
-$ pip install git+https://github.com/AdrianVollmer/Zundler@main
+$ pip install zundler
 ```
 
 If you prefer an alternative like `pipx`, `poetry` or manually handled
 `venv`s, you probably know what to do.
 
 An entry point called `zundler` will appear in `~/.local/bin`.
```

#### html2text {}

```diff
@@ -28,26 +28,25 @@
 different than some scripts expect * HTML forms with `method="GET"` to local
 HTML files only work if the receiving code uses URLSearchParams, as same-origin
 policies forbid reading GET parameters otherwise * Opening links in a new tab
 won't work * Redirections won't work (yet) * Support of themes or extensions
 that require jQuery is wonky; fortunately Sphinx stopped supporting jQuery in
 version 6 Installation ------------ Zundler is a Python package and can be
 installed like any other Python package. The recommended way is to run this:
-```shell-session $ pip install git+https://github.com/AdrianVollmer/
-Zundler@main ``` If you prefer an alternative like `pipx`, `poetry` or manually
-handled `venv`s, you probably know what to do. An entry point called `zundler`
-will appear in `~/.local/bin`. Bundling Sphinx docs -------------------- The
-Zundler package provides a Sphinx extension that adds an appropriate builder.
-The builder is a thin wrapper around the HTML builder, which runs `zundler` at
-the end. It can be used with `sphinx-build -b zundler` or, if there is a
-suitable Makefile, with `make zundler`. Jupyter-Books can be built with
-`jupyter-book build --custom-builder zundler --builder custom .`. You may have
-to add a render priority for Zundler like [here](https://jupyterbook.org/en/
-stable/content/code-outputs.html#render-priority): ```yaml sphinx: config:
-nb_mime_priority_overrides: [ ["zundler", "application/vnd.jupyter.widget-
-view+json", 10], ["zundler", "application/javascript", 20], ["zundler", "text/
-html", 30], ["zundler", "image/svg+xml", 40], ["zundler", "image/png", 50],
-["zundler", "image/jpeg", 60], ["zundler", "text/markdown", 70], ["zundler",
-"text/latex", 80], ["zundler", "text/plain", 90] ] ``` Demos ----- Some demo
-documents are available here:
+```shell-session $ pip install zundler ``` If you prefer an alternative like
+`pipx`, `poetry` or manually handled `venv`s, you probably know what to do. An
+entry point called `zundler` will appear in `~/.local/bin`. Bundling Sphinx
+docs -------------------- The Zundler package provides a Sphinx extension that
+adds an appropriate builder. The builder is a thin wrapper around the HTML
+builder, which runs `zundler` at the end. It can be used with `sphinx-build -
+b zundler` or, if there is a suitable Makefile, with `make zundler`. Jupyter-
+Books can be built with `jupyter-book build --custom-builder zundler --builder
+custom .`. You may have to add a render priority for Zundler like [here](https:
+//jupyterbook.org/en/stable/content/code-outputs.html#render-priority): ```yaml
+sphinx: config: nb_mime_priority_overrides: [ ["zundler", "application/
+vnd.jupyter.widget-view+json", 10], ["zundler", "application/javascript", 20],
+["zundler", "text/html", 30], ["zundler", "image/svg+xml", 40], ["zundler",
+"image/png", 50], ["zundler", "image/jpeg", 60], ["zundler", "text/markdown",
+70], ["zundler", "text/latex", 80], ["zundler", "text/plain", 90] ] ``` Demos -
+---- Some demo documents are available here:
 adrianvollmer.github.io/Zundler> Copyright --------- Adrian Vollmer, 2022. MIT
 licensed; see `LICENSE` for details.
```

### Comparing `zundler-0.0.0/pyproject.toml` & `zundler-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
-requires = ["setuptools>=61.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
 
 [project]
 name = "zundler"
 description = "Bundle assets of distributed HTML docs into one self-contained HTML file"
 readme = 'README.md'
 authors = [{name = "Adrian Vollmer", email = "computerfluesterer@protonmail.com"}]
 requires-python = ">=3.8"
@@ -28,46 +28,45 @@
 dependencies = [
     "sphinx",
     "lxml",
     "python-magic",
 ]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+tests = [
+    'pytest>=8',
+    'selenium',
+    'pytest-selenium',
+    'pytest-docker',
+    'black',
+    'nox',
+]
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "_version.py"
+
 [project.entry-points]
 "sphinx.builders" = {zundler = "zundler.sphinxext"}
 
 [project.scripts]
 zundler = "zundler.__main__:main"
 
-[tool.setuptools]
-zip-safe = false
-include-package-data = true
-
-[tool.setuptools.packages]
-find = {namespaces = false}
-
 [tool.mypy]
 python_version = "3.8"
 show_column_numbers = true
 show_error_context = true
 ignore_missing_imports = true
 follow_imports = "skip"
 incremental = true
 check_untyped_defs = true
 warn_unused_ignores = true
 
-[project.optional-dependencies]
-tests = [
-    'pytest>=8',
-    'selenium',
-    'pytest-selenium',
-    'pytest-docker',
-    'black',
-    'nox',
-]
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
```

### Comparing `zundler-0.0.0/tests/demo001/Makefile` & `zundler-0.1.0/tests/demo001/Makefile`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/_static/custom.css` & `zundler-0.1.0/tests/demo001/_static/custom.css`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/_static/logo-square.svg` & `zundler-0.1.0/tests/demo001/_static/logo-square.svg`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/_static/logo-wide.svg` & `zundler-0.1.0/tests/demo001/_static/logo-wide.svg`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/conf.py` & `zundler-0.1.0/tests/demo001/conf.py`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/first.md` & `zundler-0.1.0/tests/demo001/first.md`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/paragraph-markup.rst` & `zundler-0.1.0/tests/demo001/paragraph-markup.rst`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/second.md` & `zundler-0.1.0/tests/demo001/second.md`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/demo001/third.md` & `zundler-0.1.0/tests/demo001/third.md`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/tests/test_zundler.py` & `zundler-0.1.0/tests/test_zundler.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,18 +66,35 @@
 
     second_link = selenium.find_element(
         By.XPATH, "//a[text() = 'Second' and @class = 'reference internal']"
     )
 
     second_link.click()
 
+    selenium.switch_to.parent_frame()
     time.sleep(1)
 
     assert selenium.title.startswith("Second")
 
+    # Check link with anchor
+
+    selenium.switch_to.frame("zundler-iframe")
+
+    third_link = selenium.find_element(By.CSS_SELECTOR, "#second a.internal")
+
+    third_link.click()
+
+    selenium.switch_to.parent_frame()
+    time.sleep(1)
+    selenium.switch_to.frame("zundler-iframe")
+
+    assert selenium.title.startswith("Third")
+    scroll_height = int(selenium.execute_script("return window.pageYOffset"))
+    assert scroll_height > 1000
+
 
 def test_multi_page_search(selenium_drivers):
     path = Path("//mnt//multi-page//_build//zundler//index.html")
     selenium = selenium_drivers["firefox"]
     selenium.get(path.as_uri())
 
     time.sleep(1)
@@ -121,7 +138,17 @@
     hide_link = selenium.find_element(By.CSS_SELECTOR, "#searchbox a")
 
     hide_link.click()
 
     span = selenium.find_elements(By.CSS_SELECTOR, "span.highlighted")
 
     assert span == []
+
+
+def test_dark_mode(selenium_drivers):
+    path = Path("//mnt//dark-mode//_build//zundler//index.html")
+    selenium = selenium_drivers["firefox"]
+    selenium.get(path.as_uri())
+
+    time.sleep(1)
+
+    assert "dark-mode documentation" in selenium.title
```

### Comparing `zundler-0.0.0/zundler/args.py` & `zundler-0.1.0/src/zundler/args.py`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/zundler/assets/LICENSE` & `zundler-0.1.0/src/zundler/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/zundler/assets/inject_post.js` & `zundler-0.1.0/src/zundler/assets/inject_post.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -31,15 +31,15 @@
     }, '*');
     evnt.preventDefault();
     evnt.stopPropagation();
     return false;
 };
 
 
-var onScrollToAnchor = function(argument) {
+var onScrollToAnchor = function() {
     if (window.globalContext.anchor) {
         document.location.replace("about:srcdoc#" + window.globalContext.anchor);
     }
 }
 
 
 var monkeyPatch = function() {
@@ -82,16 +82,16 @@
     };
 }
 
 monkeyPatch();
 
 // Set up message listener
 window.addEventListener("message", (evnt) => {
-    console.log("Received message in iframe", evnt);
-    if (evnt.data.action == 'scroll_to_anchor') {
+    console.log("Received message in iframe", evnt.data);
+    if (evnt.data.action == 'scrollToAnchor') {
         onScrollToAnchor(evnt.data.argument);
     }
 }, false);
 
 window.parent.postMessage({
     action: "ready",
 }, '*');
```

### Comparing `zundler-0.0.0/zundler/assets/inject_pre.js` & `zundler-0.1.0/src/zundler/assets/inject_pre.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -12,28 +12,14 @@
  * creative.
  *
  * Here, we patch the `URLSearchParams` class so it returns the information
  * stored in `window.globalContext.getParameters`.
  *
  */
 
-var _base64ToArrayBuffer = function(base64) {
-    if (!base64) {
-        return []
-    }
-    var binary_string = window.atob(base64);
-    var len = binary_string.length;
-    var bytes = new Uint8Array(len);
-    for (var i = 0; i < len; i++) {
-        bytes[i] = binary_string.charCodeAt(i);
-    }
-    return bytes.buffer;
-};
-
-
 const originalGet = URLSearchParams.prototype.get;
 
 var myGet = function(arg) {
     // If searchtools.js of sphinx is used
     if (
         window.globalContext &&
         window.globalContext.getParameters &&
@@ -66,67 +52,92 @@
  * Monkeypatch window.fetch
  */
 
 const {
     fetch: originalFetch
 } = window;
 
-async function waitFor(predicate, timeout) {
+function waitForParentResponse(path) {
     return new Promise((resolve, reject) => {
-        const check = () => {
-            if (!predicate()) return;
-            clearInterval(interval);
-            resolve();
-        };
-        const interval = setInterval(check, 100);
-        check();
-
-        if (!timeout) return;
-        setTimeout(() => {
-            clearInterval(interval);
-            reject();
-        }, timeout);
+        retrieveFileFromParent(path, file => {
+            resolve(file);
+        });
     });
 }
 
-window.fetch = async (...args) => {
-    // wait until globalContext is ready
-    try {
-        await waitFor(() => window.hasOwnProperty("globalContext"), 10000);
-    } catch (err) {
-        throw err;
-    }
 
+window.fetch = async (...args) => {
     let [resource, config] = args;
     var path = normalizePath(resource);
     var response;
     if (isVirtual(path)) {
-        var file = retrieveFile(path);
+        var file = await waitForParentResponse(path);
         var data = file.data;
         if (file.base64encoded) {
             data = _base64ToArrayBuffer(data);
         }
         response = new Response(data);
         response.headers.set("content-type", file.mime_type);
     } else {
         response = await originalFetch(resource, config);
     }
     return response;
 };
 
 
+var retrieveFileFromParent = function(path, callback) {
+    // Get the file into the iframe by messaging the parent document
+    // console.log("Retrieving file from parent: " + path);
+
+    function messageHandler(event) {
+        if (event.data.action === "sendFile" && event.data.argument.path === path) {
+            callback(event.data.argument.file);
+            window.removeEventListener('message', messageHandler);
+        }
+    }
+
+    window.addEventListener('message', messageHandler);
+
+    window.parent.postMessage({
+        action: "retrieveFile",
+        argument: {
+            path: path,
+        }
+    }, '*');
+};
+
+
+var embedImgFromParent = function(img) {
+    function setSrc(img, file) {
+        if (file.mime_type == 'image/svg+xml') {
+            img.setAttribute('src', "data:image/svg+xml;charset=utf-8;base64, " + btoa(file.data));
+        } else {
+            img.setAttribute('src', `data:${file.mime_type};base64, ${file.data}`);
+        }
+    };
+
+    if (img.hasAttribute('src')) {
+        const src = img.getAttribute('src');
+        if (isVirtual(src)) {
+            var path = normalizePath(src);
+            retrieveFileFromParent(path, file => setSrc(img, file));
+        };
+    };
+};
+
+
 const observer = new MutationObserver((mutationList) => {
     // console.log("Fix mutated elements...", mutationList);
     mutationList.forEach((mutation) => {
         if (mutation.type == 'childList') {
             Array.from(mutation.target.querySelectorAll("a")).forEach(a => {
                 fixLink(a);
             });
             Array.from(mutation.target.querySelectorAll("img")).forEach(img => {
-                embedImg(img);
+                embedImgFromParent(img);
             });
             Array.from(mutation.target.querySelectorAll("form")).forEach(form => {
                 fixForm(form);
             });
         }
     });
 });
```

### Comparing `zundler-0.0.0/zundler/assets/pako.min.js` & `zundler-0.1.0/src/zundler/assets/pako.min.js`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/zundler/assets/zundler_bootstrap.js` & `zundler-0.1.0/src/zundler/assets/zundler_bootstrap.js`

 * *Files identical despite different names*

### Comparing `zundler-0.0.0/zundler/assets/zundler_common.js` & `zundler-0.1.0/src/zundler/assets/zundler_common.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,22 @@
 /*
  * Functions that will be needed by several files
  */
 
-var retrieveFile = function(path) {
-    // console.log("Retrieving file: " + path);
-    var fileTree = window.globalContext.fileTree;
-    var file = fileTree[path];
-    if (!file) {
-        console.warn("File not found: " + path);
-        return "";
-    } else {
-        return file;
+var _base64ToArrayBuffer = function(base64) {
+    if (!base64) {
+        return []
     }
+    var binary_string = window.atob(base64);
+    var len = binary_string.length;
+    var bytes = new Uint8Array(len);
+    for (var i = 0; i < len; i++) {
+        bytes[i] = binary_string.charCodeAt(i);
+    }
+    return bytes.buffer;
 };
 
 
 var isVirtual = function(url) {
     // Return true if the url should be retrieved from the virtual file tree
     var _url = url.toString().toLowerCase();
     return (!(
@@ -67,36 +68,23 @@
     var href = form.getAttribute('action');
     if (isVirtual(href) && form.getAttribute('method').toLowerCase() == 'get') {
         form.setAttribute("onsubmit", "virtualClick(event)");
     }
 };
 
 
-var embedImg = function(img) {
-    if (img.hasAttribute('src')) {
-        const src = img.getAttribute('src');
-        if (isVirtual(src)) {
-            var path = normalizePath(src);
-            const file = retrieveFile(path);
-            const mime_type = file.mime_type;
-            if (mime_type == 'image/svg+xml') {
-                img.setAttribute('src', "data:image/svg+xml;charset=utf-8;base64, " + btoa(file.data));
-            } else {
-                img.setAttribute('src', `data:${mime_type};base64, ${file.data}`);
-            }
-        };
-    };
-};
-
-
 var normalizePath = function(path) {
     // make relative paths absolute
     var result = window.globalContext.current_path;
     result = result.split('/');
     result.pop();
+    // path can be a request object
+    if (!(typeof path === 'string' || path instanceof String)) {
+        path = path.href;
+    };
     result = result.concat(path.split('/'));
 
     // resolve relative directories
     var array = [];
     Array.from(result).forEach(component => {
         if (component == '..') {
             if (array) {
```

### Comparing `zundler-0.0.0/zundler/embed.py` & `zundler-0.1.0/src/zundler/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 This document has been prepared using Zundler {version}. You can use zundler to
 inspect the files embedded below: `zundler -R <file>`
 https://github.com/AdrianVollmer/Zundler
 -->
 <html>
 <head><style>{style}</style></head>
 <body>{body}
+<script>const zundler_version = "{version}"</script>
 <script>window.globalContext = "{global_context}"</script>
 <script>{pako} \n//# sourceURL=pako.js</script>
 <script>{bootstrap} \n//# sourceURL=zundler_boostrap.js</script>
 </body><!-- {license} --></html>
 """.format(
         style=init_files["init.css"],
         body=init_files["init.html"],
```

### Comparing `zundler-0.0.0/zundler/sphinxext/__init__.py` & `zundler-0.1.0/src/zundler/sphinxext/__init__.py`

 * *Files identical despite different names*

