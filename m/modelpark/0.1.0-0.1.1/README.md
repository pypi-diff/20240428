# Comparing `tmp/modelpark-0.1.0.tar.gz` & `tmp/modelpark-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.0.tar", last modified: Sun Apr 28 09:37:25 2024, max compression
+gzip compressed data, was "modelpark-0.1.1.tar", last modified: Sun Apr 28 10:04:54 2024, max compression
```

## Comparing `modelpark-0.1.0.tar` & `modelpark-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 09:37:25.374085 modelpark-0.1.0/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.0/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.0/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 09:37:25.373862 modelpark-0.1.0/PKG-INFO
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1797 2024-04-28 09:08:05.000000 modelpark-0.1.0/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 09:37:25.372629 modelpark-0.1.0/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      420 2024-04-28 09:25:41.000000 modelpark-0.1.0/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3057 2024-04-28 09:08:05.000000 modelpark-0.1.0/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 09:37:25.373623 modelpark-0.1.0/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 09:37:25.000000 modelpark-0.1.0/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 09:37:25.000000 modelpark-0.1.0/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 09:37:25.000000 modelpark-0.1.0/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 09:37:25.000000 modelpark-0.1.0/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 09:37:25.000000 modelpark-0.1.0/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 09:37:25.374134 modelpark-0.1.0/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2279 2024-04-28 09:37:13.000000 modelpark-0.1.0/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.614601 modelpark-0.1.1/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.1/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.1/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:04:54.614375 modelpark-0.1.1/PKG-INFO
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1797 2024-04-28 09:08:05.000000 modelpark-0.1.1/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.613209 modelpark-0.1.1/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:03:46.000000 modelpark-0.1.1/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     3057 2024-04-28 09:08:05.000000 modelpark-0.1.1/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.614137 modelpark-0.1.1/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:04:54.614648 modelpark-0.1.1/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2279 2024-04-28 10:04:05.000000 modelpark-0.1.1/setup.py
```

### Comparing `modelpark-0.1.0/LICENSE` & `modelpark-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.0/PKG-INFO` & `modelpark-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.0
+Version: 0.1.1
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.0/README.md` & `modelpark-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.0/modelpark/modelpark.py` & `modelpark-0.1.1/modelpark/modelpark.py`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.0/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.1/modelpark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.0
+Version: 0.1.1
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.0/setup.py` & `modelpark-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         subprocess.check_call(['chmod', '+x', target_dir])
         print(f"Installed binary to {target_dir}")
 
 
 
 setup(
     name='modelpark',
-    version='0.1.0',
+    version='0.1.1',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
```

