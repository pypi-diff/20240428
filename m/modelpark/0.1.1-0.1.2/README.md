# Comparing `tmp/modelpark-0.1.1.tar.gz` & `tmp/modelpark-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.1.tar", last modified: Sun Apr 28 10:04:54 2024, max compression
+gzip compressed data, was "modelpark-0.1.2.tar", last modified: Sun Apr 28 10:28:26 2024, max compression
```

## Comparing `modelpark-0.1.1.tar` & `modelpark-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.614601 modelpark-0.1.1/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.1/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.1/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:04:54.614375 modelpark-0.1.1/PKG-INFO
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1797 2024-04-28 09:08:05.000000 modelpark-0.1.1/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.613209 modelpark-0.1.1/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:03:46.000000 modelpark-0.1.1/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3057 2024-04-28 09:08:05.000000 modelpark-0.1.1/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:04:54.614137 modelpark-0.1.1/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:04:54.000000 modelpark-0.1.1/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:04:54.614648 modelpark-0.1.1/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2279 2024-04-28 10:04:05.000000 modelpark-0.1.1/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.896479 modelpark-0.1.2/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.2/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.2/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:28:26.896242 modelpark-0.1.2/PKG-INFO
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1797 2024-04-28 09:08:05.000000 modelpark-0.1.2/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.894964 modelpark-0.1.2/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:26:50.000000 modelpark-0.1.2/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     3037 2024-04-28 10:24:28.000000 modelpark-0.1.2/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.895974 modelpark-0.1.2/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:28:26.896530 modelpark-0.1.2/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2277 2024-04-28 10:26:50.000000 modelpark-0.1.2/setup.py
```

### Comparing `modelpark-0.1.1/LICENSE` & `modelpark-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.1/PKG-INFO` & `modelpark-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.1
+Version: 0.1.2
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.1/README.md` & `modelpark-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.1/modelpark/modelpark.py` & `modelpark-0.1.2/modelpark/modelpark.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
         CommandRunner.run_command(command)
 
     def init(self, port=None, detach=True):
         command = "modelpark init"
         if port:
             command += f" -p {port}"
         if detach:
-            command += " -d"
-        else:
-            command += " -D"
+            command += f" -d {str(detach).lower()}"
         CommandRunner.run_command(command)
 
     def stop(self):
         CommandRunner.run_command("modelpark stop")
 
     def logout(self):
         CommandRunner.run_command("modelpark logout")
```

### Comparing `modelpark-0.1.1/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.2/modelpark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.1
+Version: 0.1.2
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.1/setup.py` & `modelpark-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,17 @@
         """Download and install binary from a given URL."""
         target_dir = "/usr/local/bin/modelpark"
         os.makedirs(os.path.dirname(target_dir), exist_ok=True)
         subprocess.check_call(['curl', url, '-o', target_dir])
         subprocess.check_call(['chmod', '+x', target_dir])
         print(f"Installed binary to {target_dir}")
 
-
-
 setup(
     name='modelpark',
-    version='0.1.1',
+    version='0.1.2',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
```

