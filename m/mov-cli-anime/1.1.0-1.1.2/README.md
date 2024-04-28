# Comparing `tmp/mov-cli-anime-1.1.0.tar.gz` & `tmp/mov_cli_anime-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-anime-1.1.0.tar", last modified: Tue Apr  9 23:45:55 2024, max compression
+gzip compressed data, was "mov_cli_anime-1.1.2.tar", last modified: Sun Apr 28 15:51:21 2024, max compression
```

## Comparing `mov-cli-anime-1.1.0.tar` & `mov_cli_anime-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:26:30.000000 mov-cli-anime-1.1.0/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-04-08 22:01:37.000000 mov-cli-anime-1.1.0/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.688726 mov-cli-anime-1.1.0/mov_cli_anime/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-04-09 23:41:30.000000 mov-cli-anime-1.1.0/mov_cli_anime/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.688726 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5232 2024-04-09 23:43:21.000000 mov-cli-anime-1.1.0/mov_cli_anime/anitaku/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2878 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-09 23:45:55.000000 mov-cli-anime-1.1.0/mov_cli_anime.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1324 2024-03-23 21:13:23.000000 mov-cli-anime-1.1.0/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:45:55.692059 mov-cli-anime-1.1.0/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-28 15:51:21.618591 mov_cli_anime-1.1.2/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1063 2024-04-28 15:35:00.000000 mov_cli_anime-1.1.2/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3084 2024-04-28 15:51:21.615258 mov_cli_anime-1.1.2/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      850 2024-04-28 15:49:40.000000 mov_cli_anime-1.1.2/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-28 15:51:21.615258 mov_cli_anime-1.1.2/mov_cli_anime/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      117 2024-04-28 15:46:27.000000 mov_cli_anime-1.1.2/mov_cli_anime/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-28 15:51:21.615258 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3084 2024-04-28 15:51:21.000000 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-04-28 15:51:21.000000 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-28 15:51:21.000000 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       86 2024-04-28 15:51:21.000000 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       28 2024-04-28 15:51:21.000000 mov_cli_anime-1.1.2/mov_cli_anime.egg-info/top_level.txt
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-28 15:51:21.615258 mov_cli_anime-1.1.2/otaku_watcher/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-04-28 15:35:40.000000 mov_cli_anime-1.1.2/otaku_watcher/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-28 15:51:21.615258 mov_cli_anime-1.1.2/otaku_watcher/anitaku/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 mov_cli_anime-1.1.2/otaku_watcher/anitaku/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5232 2024-04-09 23:43:21.000000 mov_cli_anime-1.1.2/otaku_watcher/anitaku/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1226 2024-04-28 15:51:16.000000 mov_cli_anime-1.1.2/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-28 15:51:21.618591 mov_cli_anime-1.1.2/setup.cfg
```

### Comparing `mov-cli-anime-1.1.0/LICENSE` & `mov_cli_anime-1.1.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 mov-cli
+Copyright (c) 2024 JDALab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mov-cli-anime-1.1.0/PKG-INFO` & `mov_cli_anime-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.1.0
-Summary: A mov-cli v4 plugin for watching anime.
-Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+Version: 1.1.2
+Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
-        Copyright (c) 2024 mov-cli
+        Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,60 +20,64 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-anime
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-anime/issues
+Project-URL: GitHub, https://github.com/JDALab/otaku-watcher
+Project-URL: BugTracker, https://github.com/JDALab/otaku-watcher/issues
 Keywords: amazing mov-cli plugin
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.1.6
+Requires-Dist: mov-cli>=4.3
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
-  # mov-cli-anime
-  <sub>A mov-cli v4 plugin for watching anime.</sub>
+  # otaku-watcher
+  <sub>A mov-cli plugin for watching anime.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
 
 </div>
 
-> [!NOTE]
-> Searching for maintainers
+> [!CRITICAL]
+> We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
+> [!WARNING]
+> Before installing this plugin make sure ``mov-cli-anime`` is not installed to lower the risks of a conflict.
+> ``pip uninstall mov-cli-anime``
+
 1. Install the pip package.
 ```sh
-pip install mov-cli-anime 
+pip install otaku-watcher
 ```
 2. Then add the plugin to your mov-cli config.
 ```sh
 mov-cli -e
 ```
 ```toml
 [mov-cli.plugins]
-anime = "mov-cli-anime"
+anime = "otaku-watcher"
 ```
 
 ## Usage
 ```sh
 mov-cli -s anime lycoris recoil
 ```
```

### Comparing `mov-cli-anime-1.1.0/mov_cli_anime/anitaku/scraper.py` & `mov_cli_anime-1.1.2/otaku_watcher/anitaku/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-anime-1.1.0/mov_cli_anime.egg-info/PKG-INFO` & `mov_cli_anime-1.1.2/mov_cli_anime.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: mov-cli-anime
-Version: 1.1.0
-Summary: A mov-cli v4 plugin for watching anime.
-Author-email: Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+Version: 1.1.2
+Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
-        Copyright (c) 2024 mov-cli
+        Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,60 +20,64 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-anime
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-anime/issues
+Project-URL: GitHub, https://github.com/JDALab/otaku-watcher
+Project-URL: BugTracker, https://github.com/JDALab/otaku-watcher/issues
 Keywords: amazing mov-cli plugin
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.1.6
+Requires-Dist: mov-cli>=4.3
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
-  # mov-cli-anime
-  <sub>A mov-cli v4 plugin for watching anime.</sub>
+  # otaku-watcher
+  <sub>A mov-cli plugin for watching anime.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
 
 </div>
 
-> [!NOTE]
-> Searching for maintainers
+> [!CRITICAL]
+> We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
 Here's how to install and add the plugin to mov-cli.
 
+> [!WARNING]
+> Before installing this plugin make sure ``mov-cli-anime`` is not installed to lower the risks of a conflict.
+> ``pip uninstall mov-cli-anime``
+
 1. Install the pip package.
 ```sh
-pip install mov-cli-anime 
+pip install otaku-watcher
 ```
 2. Then add the plugin to your mov-cli config.
 ```sh
 mov-cli -e
 ```
 ```toml
 [mov-cli.plugins]
-anime = "mov-cli-anime"
+anime = "otaku-watcher"
 ```
 
 ## Usage
 ```sh
 mov-cli -s anime lycoris recoil
 ```
```

