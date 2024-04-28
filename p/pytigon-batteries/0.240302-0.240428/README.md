# Comparing `tmp/pytigon-batteries-0.240302.tar.gz` & `tmp/pytigon-batteries-0.240428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-batteries-0.240302.tar", last modified: Sat Mar  2 14:25:46 2024, max compression
+gzip compressed data, was "pytigon-batteries-0.240428.tar", last modified: Sun Apr 28 17:14:12 2024, max compression
```

## Comparing `pytigon-batteries-0.240302.tar` & `pytigon-batteries-0.240428.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:46.516799 pytigon-batteries-0.240302/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2024-03-02 14:22:05.000000 pytigon-batteries-0.240302/LICENSE
--rw-r--r--   0 sch       (1000) sch       (1000)     5450 2024-03-02 14:25:46.516799 pytigon-batteries-0.240302/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       53 2024-03-02 14:22:05.000000 pytigon-batteries-0.240302/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:46.508799 pytigon-batteries-0.240302/pytigon_batteries.egg-info/
--rw-r--r--   0 sch       (1000) sch       (1000)     5450 2024-03-02 14:25:46.000000 pytigon-batteries-0.240302/pytigon_batteries.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)      230 2024-03-02 14:25:46.000000 pytigon-batteries-0.240302/pytigon_batteries.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-03-02 14:25:46.000000 pytigon-batteries-0.240302/pytigon_batteries.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)     1168 2024-03-02 14:25:46.000000 pytigon-batteries-0.240302/pytigon_batteries.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-03-02 14:25:46.000000 pytigon-batteries-0.240302/pytigon_batteries.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-03-02 14:25:46.516799 pytigon-batteries-0.240302/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     2556 2024-03-02 14:22:05.000000 pytigon-batteries-0.240302/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:12.768771 pytigon-batteries-0.240428/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7652 2024-04-28 17:09:48.000000 pytigon-batteries-0.240428/LICENSE
+-rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-04-28 17:14:12.768771 pytigon-batteries-0.240428/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       53 2024-04-28 17:09:48.000000 pytigon-batteries-0.240428/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:12.760770 pytigon-batteries-0.240428/pytigon_batteries.egg-info/
+-rw-r--r--   0 sch       (1000) sch       (1000)     5530 2024-04-28 17:14:12.000000 pytigon-batteries-0.240428/pytigon_batteries.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)      230 2024-04-28 17:14:12.000000 pytigon-batteries-0.240428/pytigon_batteries.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-04-28 17:14:12.000000 pytigon-batteries-0.240428/pytigon_batteries.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1180 2024-04-28 17:14:12.000000 pytigon-batteries-0.240428/pytigon_batteries.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-04-28 17:14:12.000000 pytigon-batteries-0.240428/pytigon_batteries.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-04-28 17:14:12.768771 pytigon-batteries-0.240428/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2556 2024-04-28 17:09:48.000000 pytigon-batteries-0.240428/setup.py
```

### Comparing `pytigon-batteries-0.240302/LICENSE` & `pytigon-batteries-0.240428/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-batteries-0.240302/PKG-INFO` & `pytigon-batteries-0.240428/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.240302
+Version: 0.240428
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -80,14 +80,15 @@
 Provides-Extra: interface
 Requires-Dist: dulwich; extra == "interface"
 Requires-Dist: cffi; extra == "interface"
 Requires-Dist: wasmtime; extra == "interface"
 Requires-Dist: ziglang; extra == "interface"
 Requires-Dist: xonsh; extra == "interface"
 Requires-Dist: httpie; extra == "interface"
+Requires-Dist: pyzmq; extra == "interface"
 Provides-Extra: all
 Requires-Dist: redis; extra == "all"
 Requires-Dist: channels; extra == "all"
 Requires-Dist: channels-redis; extra == "all"
 Requires-Dist: daphne; extra == "all"
 Requires-Dist: easy_thumbnails; extra == "all"
 Requires-Dist: croniter; extra == "all"
@@ -124,7 +125,8 @@
 Requires-Dist: plotly; extra == "all"
 Requires-Dist: dulwich; extra == "all"
 Requires-Dist: cffi; extra == "all"
 Requires-Dist: wasmtime; extra == "all"
 Requires-Dist: ziglang; extra == "all"
 Requires-Dist: xonsh; extra == "all"
 Requires-Dist: httpie; extra == "all"
+Requires-Dist: pyzmq; extra == "all"
```

### Comparing `pytigon-batteries-0.240302/pytigon_batteries.egg-info/PKG-INFO` & `pytigon-batteries-0.240428/pytigon_batteries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-batteries
-Version: 0.240302
+Version: 0.240428
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -80,14 +80,15 @@
 Provides-Extra: interface
 Requires-Dist: dulwich; extra == "interface"
 Requires-Dist: cffi; extra == "interface"
 Requires-Dist: wasmtime; extra == "interface"
 Requires-Dist: ziglang; extra == "interface"
 Requires-Dist: xonsh; extra == "interface"
 Requires-Dist: httpie; extra == "interface"
+Requires-Dist: pyzmq; extra == "interface"
 Provides-Extra: all
 Requires-Dist: redis; extra == "all"
 Requires-Dist: channels; extra == "all"
 Requires-Dist: channels-redis; extra == "all"
 Requires-Dist: daphne; extra == "all"
 Requires-Dist: easy_thumbnails; extra == "all"
 Requires-Dist: croniter; extra == "all"
@@ -124,7 +125,8 @@
 Requires-Dist: plotly; extra == "all"
 Requires-Dist: dulwich; extra == "all"
 Requires-Dist: cffi; extra == "all"
 Requires-Dist: wasmtime; extra == "all"
 Requires-Dist: ziglang; extra == "all"
 Requires-Dist: xonsh; extra == "all"
 Requires-Dist: httpie; extra == "all"
+Requires-Dist: pyzmq; extra == "all"
```

### Comparing `pytigon-batteries-0.240302/pytigon_batteries.egg-info/requires.txt` & `pytigon-batteries-0.240428/pytigon_batteries.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 plotly
 dulwich
 cffi
 wasmtime
 ziglang
 xonsh
 httpie
+pyzmq
 
 [data]
 numpy
 pandas
 pyarrow
 duckdb
 plotly
@@ -67,14 +68,15 @@
 [interface]
 dulwich
 cffi
 wasmtime
 ziglang
 xonsh
 httpie
+pyzmq
 
 [server]
 redis
 channels
 channels-redis
 daphne
 easy_thumbnails
```

### Comparing `pytigon-batteries-0.240302/setup.py` & `pytigon-batteries-0.240428/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 extras_require["all"] = (
     extras_require["server"] + extras_require["data"] + extras_require["interface"]
 )
 
 setup(
     name="pytigon-batteries",
-    version="0.240302",
+    version="0.240428",
     description="Pytigon library",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={"": extra_files},
     install_requires=install_requires,
```

