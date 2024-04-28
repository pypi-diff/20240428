# Comparing `tmp/ascender-0.1.4.tar.gz` & `tmp/ascender-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascender-0.1.4.tar", max compression
+gzip compressed data, was "ascender-0.1.5.tar", max compression
```

## Comparing `ascender-0.1.4.tar` & `ascender-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.4/LICENSE
--rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.4/README.md
--rw-r--r--   0        0        0      146 2023-12-19 20:01:36.639816 ascender-0.1.4/ascender/app.py
--rw-r--r--   0        0        0     1534 2024-01-04 19:08:37.226570 ascender-0.1.4/ascender/commands/projects.py
--rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.4/ascender/commands/runner.py
--rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.4/ascender/launch.py
--rw-r--r--   0        0        0     5477 2024-01-04 19:12:41.147010 ascender-0.1.4/ascender/logic/projects.py
--rw-r--r--   0        0        0     2278 2023-12-19 20:29:16.219795 ascender-0.1.4/ascender/logic/runner.py
--rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.4/ascender/settings.py
--rw-r--r--   0        0        0      655 2024-01-04 19:06:39.736552 ascender-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.5/LICENSE
+-rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.5/README.md
+-rw-r--r--   0        0        0      146 2023-12-19 20:01:36.639816 ascender-0.1.5/ascender/app.py
+-rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.5/ascender/commands/projects.py
+-rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.5/ascender/commands/runner.py
+-rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.5/ascender/launch.py
+-rw-r--r--   0        0        0     7538 2024-04-28 14:57:02.938433 ascender-0.1.5/ascender/logic/projects.py
+-rw-r--r--   0        0        0     2278 2023-12-19 20:29:16.219795 ascender-0.1.5/ascender/logic/runner.py
+-rw-r--r--   0        0        0     2462 2024-04-28 15:09:06.733790 ascender-0.1.5/ascender/logic/versions.py
+-rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.5/ascender/settings.py
+-rw-r--r--   0        0        0      655 2024-04-27 18:35:11.387178 ascender-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.5/PKG-INFO
```

### Comparing `ascender-0.1.4/LICENSE` & `ascender-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ascender-0.1.4/README.md` & `ascender-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ascender-0.1.4/ascender/commands/runner.py` & `ascender-0.1.5/ascender/commands/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.4/ascender/logic/runner.py` & `ascender-0.1.5/ascender/logic/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.4/pyproject.toml` & `ascender-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascender"
-version = "0.1.4"
+version = "0.1.5"
 description = "The CLI tool for working with AscenderFramework: Installation, command execution and version management"
 authors = ["AscenderTeam"]
 repository = "https://github.com/AscenderTeam/AscenderCLI"
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ascender-0.1.4/PKG-INFO` & `ascender-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascender
-Version: 0.1.4
+Version: 0.1.5
 Summary: The CLI tool for working with AscenderFramework: Installation, command execution and version management
 Home-page: https://github.com/AscenderTeam/AscenderCLI
 License: GPL-3.0
 Author: AscenderTeam
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

