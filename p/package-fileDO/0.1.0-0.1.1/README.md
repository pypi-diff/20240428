# Comparing `tmp/package_filedo-0.1.0.tar.gz` & `tmp/package_filedo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_filedo-0.1.0.tar", last modified: Sun Apr 28 03:20:41 2024, max compression
+gzip compressed data, was "package_filedo-0.1.1.tar", last modified: Sun Apr 28 03:43:32 2024, max compression
```

## Comparing `package_filedo-0.1.0.tar` & `package_filedo-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 03:20:41.758838 package_filedo-0.1.0/
--rw-rw-rw-   0        0        0     1097 2024-04-28 03:12:23.000000 package_filedo-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1978 2024-04-28 03:20:41.757789 package_filedo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1333 2024-04-28 02:48:47.000000 package_filedo-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 03:20:41.725906 package_filedo-0.1.0/package_fileDO/
--rw-rw-rw-   0        0        0     2083 2024-04-28 03:00:04.000000 package_filedo-0.1.0/package_fileDO/FileDO.py
--rw-rw-rw-   0        0        0      309 2024-04-28 03:00:46.000000 package_filedo-0.1.0/package_fileDO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:20:41.755790 package_filedo-0.1.0/package_fileDO.egg-info/
--rw-rw-rw-   0        0        0     1978 2024-04-28 03:20:41.000000 package_filedo-0.1.0/package_fileDO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-28 03:20:41.000000 package_filedo-0.1.0/package_fileDO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 03:20:41.000000 package_filedo-0.1.0/package_fileDO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 03:20:41.000000 package_filedo-0.1.0/package_fileDO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-28 03:20:41.000000 package_filedo-0.1.0/package_fileDO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 03:20:41.758838 package_filedo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-04-28 03:20:19.000000 package_filedo-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:43:32.863697 package_filedo-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2024-04-28 03:12:23.000000 package_filedo-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1978 2024-04-28 03:43:32.861601 package_filedo-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1333 2024-04-28 02:48:47.000000 package_filedo-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 03:43:32.835049 package_filedo-0.1.1/package_fileDO/
+-rw-rw-rw-   0        0        0     2083 2024-04-28 03:00:04.000000 package_filedo-0.1.1/package_fileDO/FileDO.py
+-rw-rw-rw-   0        0        0      310 2024-04-28 03:40:06.000000 package_filedo-0.1.1/package_fileDO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 03:43:32.860601 package_filedo-0.1.1/package_fileDO.egg-info/
+-rw-rw-rw-   0        0        0     1978 2024-04-28 03:43:32.000000 package_filedo-0.1.1/package_fileDO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-28 03:43:32.000000 package_filedo-0.1.1/package_fileDO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 03:43:32.000000 package_filedo-0.1.1/package_fileDO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 03:43:32.000000 package_filedo-0.1.1/package_fileDO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-28 03:43:32.000000 package_filedo-0.1.1/package_fileDO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 03:43:32.864220 package_filedo-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      997 2024-04-28 03:43:17.000000 package_filedo-0.1.1/setup.py
```

### Comparing `package_filedo-0.1.0/LICENSE.txt` & `package_filedo-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `package_filedo-0.1.0/PKG-INFO` & `package_filedo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_fileDO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python SDK for ioc-ic
 Home-page: https://github.com/whalecui1014
 Author: Cui Jingyu
 Author-email: 1808662399@qq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `package_filedo-0.1.0/README.md` & `package_filedo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `package_filedo-0.1.0/package_fileDO/FileDO.py` & `package_filedo-0.1.1/package_fileDO/FileDO.py`

 * *Files identical despite different names*

### Comparing `package_filedo-0.1.0/package_fileDO.egg-info/PKG-INFO` & `package_filedo-0.1.1/package_fileDO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_fileDO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python SDK for ioc-ic
 Home-page: https://github.com/whalecui1014
 Author: Cui Jingyu
 Author-email: 1808662399@qq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `package_filedo-0.1.0/setup.py` & `package_filedo-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='package_fileDO',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     description='A python SDK for ioc-ic',
     long_description=long_description,
     long_description_content_type='text/markdown',  # 确保格式正确显示在 PyPI 上
     author='Cui Jingyu',
     author_email='1808662399@qq.com',
     url='https://github.com/whalecui1014',
```

