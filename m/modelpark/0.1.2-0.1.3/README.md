# Comparing `tmp/modelpark-0.1.2.tar.gz` & `tmp/modelpark-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.2.tar", last modified: Sun Apr 28 10:28:26 2024, max compression
+gzip compressed data, was "modelpark-0.1.3.tar", last modified: Sun Apr 28 10:47:48 2024, max compression
```

## Comparing `modelpark-0.1.2.tar` & `modelpark-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.896479 modelpark-0.1.2/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.2/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.2/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:28:26.896242 modelpark-0.1.2/PKG-INFO
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1797 2024-04-28 09:08:05.000000 modelpark-0.1.2/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.894964 modelpark-0.1.2/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:26:50.000000 modelpark-0.1.2/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3037 2024-04-28 10:24:28.000000 modelpark-0.1.2/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:28:26.895974 modelpark-0.1.2/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     2596 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:28:26.000000 modelpark-0.1.2/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:28:26.896530 modelpark-0.1.2/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2277 2024-04-28 10:26:50.000000 modelpark-0.1.2/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.779221 modelpark-0.1.3/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.3/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.3/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2574 2024-04-28 10:47:48.779002 modelpark-0.1.3/PKG-INFO
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1775 2024-04-28 10:34:12.000000 modelpark-0.1.3/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.777818 modelpark-0.1.3/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:41:20.000000 modelpark-0.1.3/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     3318 2024-04-28 10:47:08.000000 modelpark-0.1.3/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.778759 modelpark-0.1.3/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2574 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:47:48.779271 modelpark-0.1.3/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2277 2024-04-28 10:41:20.000000 modelpark-0.1.3/setup.py
```

### Comparing `modelpark-0.1.2/LICENSE` & `modelpark-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.2/PKG-INFO` & `modelpark-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.2
+Version: 0.1.3
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 
 ### Initialize and Login
 ```python
 from modelpark import ModelPark
 
 mp = ModelPark()
 mp.login(username="your_username", password="your_password")
-mp.init(port=8080, detach=True)
+mp.init()
 ```
 
 ### Register an Application
 ```python
 mp.register(port=3000, name="my-app", file_path="~/my-app/streamlit-app.py", access="public", framework="streamlit")
 ```
```

### Comparing `modelpark-0.1.2/README.md` & `modelpark-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ### Initialize and Login
 ```python
 from modelpark import ModelPark
 
 mp = ModelPark()
 mp.login(username="your_username", password="your_password")
-mp.init(port=8080, detach=True)
+mp.init()
 ```
 
 ### Register an Application
 ```python
 mp.register(port=3000, name="my-app", file_path="~/my-app/streamlit-app.py", access="public", framework="streamlit")
 ```
```

### Comparing `modelpark-0.1.2/modelpark/modelpark.py` & `modelpark-0.1.3/modelpark/modelpark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 import json
 import requests
 import subprocess
 import sys
 
+class CommandRunner:
+    """Executes system commands related to ModelPark CLI operations."""
+
+    @staticmethod
+    def run_command(command):
+        try:
+            process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+            stdout, stderr = process.communicate()
+            if process.returncode != 0:
+                print("Error:", stderr)
+                sys.exit(1)
+            return stdout
+        except subprocess.CalledProcessError as e:
+            print("Error:", e.stderr)
+            sys.exit(1)
+
+
 class ModelPark:
     def __init__(self):
         pass
 
     def login(self, token=None, username=None, password=None):
         command = "modelpark login"
         if token:
@@ -17,17 +34,20 @@
             command += f" -p {password}"
         CommandRunner.run_command(command)
 
     def init(self, port=None, detach=True):
         command = "modelpark init"
         if port:
             command += f" -p {port}"
-        if detach:
+
+        if detach !=True:
             command += f" -d {str(detach).lower()}"
-        CommandRunner.run_command(command)
+        print(f"Running command: {command}")  # Debug print
+        output = CommandRunner.run_command(command)
+        print("Initialization Output:", output)
 
     def stop(self):
         CommandRunner.run_command("modelpark stop")
 
     def logout(self):
         CommandRunner.run_command("modelpark logout")
 
@@ -47,25 +67,14 @@
             command += f" -n {name}"
         CommandRunner.run_command(command)
 
     def ls(self):
         result = CommandRunner.run_command("modelpark ls")
         print(result)
 
-class CommandRunner:
-    """Executes system commands related to ModelPark CLI operations."""
-
-    @staticmethod
-    def run_command(command):
-        try:
-            output = subprocess.check_output(command, stderr=subprocess.STDOUT, shell=True)
-            return output.decode('utf-8')
-        except subprocess.CalledProcessError as e:
-            print("Error:", e.output.decode('utf-8'))
-            sys.exit(1)
 
 class APIManager:
     """Manages API interactions for ModelPark."""
 
     @staticmethod
     def get_auth_token(user_credentials):
         url = "https://modelpark.app/api/auth/login"
```

### Comparing `modelpark-0.1.2/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.3/modelpark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.2
+Version: 0.1.3
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 
 ### Initialize and Login
 ```python
 from modelpark import ModelPark
 
 mp = ModelPark()
 mp.login(username="your_username", password="your_password")
-mp.init(port=8080, detach=True)
+mp.init()
 ```
 
 ### Register an Application
 ```python
 mp.register(port=3000, name="my-app", file_path="~/my-app/streamlit-app.py", access="public", framework="streamlit")
 ```
```

### Comparing `modelpark-0.1.2/setup.py` & `modelpark-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         os.makedirs(os.path.dirname(target_dir), exist_ok=True)
         subprocess.check_call(['curl', url, '-o', target_dir])
         subprocess.check_call(['chmod', '+x', target_dir])
         print(f"Installed binary to {target_dir}")
 
 setup(
     name='modelpark',
-    version='0.1.2',
+    version='0.1.3',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
```

