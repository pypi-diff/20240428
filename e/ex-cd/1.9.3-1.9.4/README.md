# Comparing `tmp/ex_cd-1.9.3.tar.gz` & `tmp/ex_cd-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_cd-1.9.3.tar", last modified: Sun Dec  3 23:15:13 2023, max compression
+gzip compressed data, was "ex_cd-1.9.4.tar", last modified: Sun Dec  3 23:31:39 2023, max compression
```

## Comparing `ex_cd-1.9.3.tar` & `ex_cd-1.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:15:13.384306 ex_cd-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-03 23:15:01.000000 ex_cd-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-12-03 23:15:13.384306 ex_cd-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-12-03 23:15:01.000000 ex_cd-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:15:13.384306 ex_cd-1.9.3/ex_cd/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/download_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/download_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/download_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/gallery_dl_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-03 23:15:01.000000 ex_cd-1.9.3/ex_cd/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:15:13.384306 ex_cd-1.9.3/ex_cd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-12-03 23:15:13.000000 ex_cd-1.9.3/ex_cd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-03 23:15:13.000000 ex_cd-1.9.3/ex_cd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 23:15:13.000000 ex_cd-1.9.3/ex_cd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-03 23:15:13.000000 ex_cd-1.9.3/ex_cd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-03 23:15:13.000000 ex_cd-1.9.3/ex_cd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-03 23:15:13.384306 ex_cd-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-03 23:15:01.000000 ex_cd-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:31:39.303546 ex_cd-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-03 23:31:31.000000 ex_cd-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-12-03 23:31:39.303546 ex_cd-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-03 23:31:31.000000 ex_cd-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:31:39.303546 ex_cd-1.9.4/ex_cd/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/download_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/download_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/download_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/gallery_dl_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-03 23:31:31.000000 ex_cd-1.9.4/ex_cd/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 23:31:39.303546 ex_cd-1.9.4/ex_cd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2023-12-03 23:31:39.000000 ex_cd-1.9.4/ex_cd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-03 23:31:39.000000 ex_cd-1.9.4/ex_cd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 23:31:39.000000 ex_cd-1.9.4/ex_cd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-03 23:31:39.000000 ex_cd-1.9.4/ex_cd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-03 23:31:39.000000 ex_cd-1.9.4/ex_cd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-03 23:31:39.303546 ex_cd-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-03 23:31:31.000000 ex_cd-1.9.4/setup.py
```

### Comparing `ex_cd-1.9.3/LICENSE` & `ex_cd-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/PKG-INFO` & `ex_cd-1.9.4/ex_cd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ex_cd
-Version: 1.9.3
+Name: ex-cd
+Version: 1.9.4
 Summary: 高效下载E站gallery的所有历史数据
 Home-page: https://github.com/yindaheng98/ex-cd
 Author: yindaheng98
 Author-email: yindaheng98@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,29 @@
 
 ## Usage
 
 ```sh
 python -m ex_cd -c .vscode/config.json https://exhentai.org/g/2635845/ecbc9d9681/
 ```
 
+```sh
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
 You can see the example config file: `.vscode/config.json`
 
+You can also set an `EXCD_CONFIG_FILE` env to specify a file, and the config in this file will be overridden by the config specified by `-c`:
+
+```sh
+export EXCD_CONFIG_FILE=".vscode/config.json"
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
+You can see the example command line: `.vscode/launch.json`
+
 ## How does it work?
 
 ### URL更新
 
 ```mermaid
 flowchart TD
```

### Comparing `ex_cd-1.9.3/README.md` & `ex_cd-1.9.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,29 @@
 
 ## Usage
 
 ```sh
 python -m ex_cd -c .vscode/config.json https://exhentai.org/g/2635845/ecbc9d9681/
 ```
 
+```sh
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
 You can see the example config file: `.vscode/config.json`
 
+You can also set an `EXCD_CONFIG_FILE` env to specify a file, and the config in this file will be overridden by the config specified by `-c`:
+
+```sh
+export EXCD_CONFIG_FILE=".vscode/config.json"
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
+You can see the example command line: `.vscode/launch.json`
+
 ## How does it work?
 
 ### URL更新
 
 ```mermaid
 flowchart TD
```

### Comparing `ex_cd-1.9.3/ex_cd/__init__.py` & `ex_cd-1.9.4/ex_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/common.py` & `ex_cd-1.9.4/ex_cd/common.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/config.py` & `ex_cd-1.9.4/ex_cd/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,17 +53,24 @@
     "gallery-dl-args": [],
     # Args for running gallery-dl commandline program for meta extraction
     "gallery-dl-meta-args": [],
 }
 
 
 def read_config(args, logger):
-    if len(args.config) <= 0:
-        logger.warn("Cannot read config from args, fall back to env EXCD_CONFIG_FILE")
-        args.config = os.environ["EXCD_CONFIG_FILE"]
+    if "EXCD_CONFIG_FILE" in os.environ:
+        try:
+            with open(os.environ["EXCD_CONFIG_FILE"], encoding='utf8') as f:
+                override = json.load(f)
+            for k in config:
+                if k in override:
+                    config[k] = override[k]
+        except Exception as e:
+            logger.warn("Cannot read EXCD_CONFIG_FILE %s: %s" % (os.environ["EXCD_CONFIG_FILE"], e))
+
     if os.path.isfile(args.config):
         try:
             with open(args.config, encoding='utf8') as f:
                 override = json.load(f)
         except Exception as e:
             logger.warn("Cannot read config %s: %s" % (args.config, e))
     else:
```

### Comparing `ex_cd-1.9.3/ex_cd/deprecate.py` & `ex_cd-1.9.4/ex_cd/deprecate.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/download_history.py` & `ex_cd-1.9.4/ex_cd/download_history.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/download_image.py` & `ex_cd-1.9.4/ex_cd/download_image.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/download_meta.py` & `ex_cd-1.9.4/ex_cd/download_meta.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/gallery_dl_exec.py` & `ex_cd-1.9.4/ex_cd/gallery_dl_exec.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/history.py` & `ex_cd-1.9.4/ex_cd/history.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd/output.py` & `ex_cd-1.9.4/ex_cd/output.py`

 * *Files identical despite different names*

### Comparing `ex_cd-1.9.3/ex_cd.egg-info/PKG-INFO` & `ex_cd-1.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ex-cd
-Version: 1.9.3
+Name: ex_cd
+Version: 1.9.4
 Summary: 高效下载E站gallery的所有历史数据
 Home-page: https://github.com/yindaheng98/ex-cd
 Author: yindaheng98
 Author-email: yindaheng98@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,29 @@
 
 ## Usage
 
 ```sh
 python -m ex_cd -c .vscode/config.json https://exhentai.org/g/2635845/ecbc9d9681/
 ```
 
+```sh
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
 You can see the example config file: `.vscode/config.json`
 
+You can also set an `EXCD_CONFIG_FILE` env to specify a file, and the config in this file will be overridden by the config specified by `-c`:
+
+```sh
+export EXCD_CONFIG_FILE=".vscode/config.json"
+python -m ex_cd -c <a json string> https://exhentai.org/g/2635845/ecbc9d9681/
+```
+
+You can see the example command line: `.vscode/launch.json`
+
 ## How does it work?
 
 ### URL更新
 
 ```mermaid
 flowchart TD
```

### Comparing `ex_cd-1.9.3/setup.py` & `ex_cd-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 package_dir = {
     'ex_cd': 'ex_cd'
 }
 
 setup(
     name='ex_cd',
-    version='1.9.3',
+    version='1.9.4',
     author='yindaheng98',
     author_email='yindaheng98@163.com',
     url='https://github.com/yindaheng98/ex-cd',
     description=u'高效下载E站gallery的所有历史数据',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

