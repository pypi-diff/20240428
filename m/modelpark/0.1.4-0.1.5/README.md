# Comparing `tmp/modelpark-0.1.4.tar.gz` & `tmp/modelpark-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.4.tar", last modified: Sun Apr 28 12:15:09 2024, max compression
+gzip compressed data, was "modelpark-0.1.5.tar", last modified: Sun Apr 28 19:56:00 2024, max compression
```

## Comparing `modelpark-0.1.4.tar` & `modelpark-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.354402 modelpark-0.1.4/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.4/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.4/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     2676 2024-04-28 12:15:09.354179 modelpark-0.1.4/PKG-INFO
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1775 2024-04-28 10:34:12.000000 modelpark-0.1.4/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.352883 modelpark-0.1.4/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 12:15:01.000000 modelpark-0.1.4/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3427 2024-04-28 12:06:59.000000 modelpark-0.1.4/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.353963 modelpark-0.1.4/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     2676 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 12:15:09.354444 modelpark-0.1.4/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2964 2024-04-28 12:15:01.000000 modelpark-0.1.4/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 19:56:00.846286 modelpark-0.1.5/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.5/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.5/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3024 2024-04-28 19:56:00.846064 modelpark-0.1.5/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2123 2024-04-28 19:54:56.000000 modelpark-0.1.5/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 19:56:00.845101 modelpark-0.1.5/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      345 2024-04-28 19:55:51.000000 modelpark-0.1.5/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     3427 2024-04-28 12:06:59.000000 modelpark-0.1.5/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 19:56:00.845843 modelpark-0.1.5/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3024 2024-04-28 19:56:00.000000 modelpark-0.1.5/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 19:56:00.000000 modelpark-0.1.5/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 19:56:00.000000 modelpark-0.1.5/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 19:56:00.000000 modelpark-0.1.5/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 19:56:00.000000 modelpark-0.1.5/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 19:56:00.846330 modelpark-0.1.5/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2964 2024-04-28 19:55:49.000000 modelpark-0.1.5/setup.py
```

### Comparing `modelpark-0.1.4/LICENSE` & `modelpark-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.4/PKG-INFO` & `modelpark-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.4
+Version: 0.1.5
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,20 @@
 Requires-Dist: requests
 
 
 # ModelPark
 
 ModelPark provides a versatile platform to share and manage your ML models directly from your machine, offering a convenient Python API to manage these tasks programmatically, including controlling access and publishing applications.
 
+See [ModelPark](https://modelpark.app/) website and platform for more details.
+
+![image](https://github.com/model-park/modelpark/assets/25637056/6eac80e7-91e9-477a-bcce-bd7d369d932e)
+
+![image](https://github.com/model-park/modelpark/assets/25637056/be495106-915d-4989-818d-dad7bb5abc71)
+
 ## Features
 
 - Share models directly from the Python API.
 - Publish and manage applications using the ModelPark Python API.
 - Configure access management according to your needs through Python methods.
 
 ## Installation
@@ -65,20 +71,23 @@
 ### List Registered Applications
 ```python
 mp.ls()
 ```
 
 ### Make an API Call to a Registered Application
 ```python
+from modelpark import APIManager
+mp_api = APIManager()
+
 user_credentials = {'username': 'your_username', 'password': 'your_password'}
 app_name = 'my-app'
 payload = {'key': 'value'}  # Payload required by the application
 
 # Make the API call
-response = mp.make_api_call(app_name, user_credentials, payload)
+response = mp_api.make_api_call(app_name, user_credentials, payload)
 print(response.json())  # Assuming the response is in JSON format
 ```
 
 ### Stop and Logout
 ```python
 mp.stop()
 mp.logout()
```

### Comparing `modelpark-0.1.4/README.md` & `modelpark-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 
 # ModelPark
 
 ModelPark provides a versatile platform to share and manage your ML models directly from your machine, offering a convenient Python API to manage these tasks programmatically, including controlling access and publishing applications.
 
+See [ModelPark](https://modelpark.app/) website and platform for more details.
+
+![image](https://github.com/model-park/modelpark/assets/25637056/6eac80e7-91e9-477a-bcce-bd7d369d932e)
+
+![image](https://github.com/model-park/modelpark/assets/25637056/be495106-915d-4989-818d-dad7bb5abc71)
+
 ## Features
 
 - Share models directly from the Python API.
 - Publish and manage applications using the ModelPark Python API.
 - Configure access management according to your needs through Python methods.
 
 ## Installation
@@ -41,20 +47,23 @@
 ### List Registered Applications
 ```python
 mp.ls()
 ```
 
 ### Make an API Call to a Registered Application
 ```python
+from modelpark import APIManager
+mp_api = APIManager()
+
 user_credentials = {'username': 'your_username', 'password': 'your_password'}
 app_name = 'my-app'
 payload = {'key': 'value'}  # Payload required by the application
 
 # Make the API call
-response = mp.make_api_call(app_name, user_credentials, payload)
+response = mp_api.make_api_call(app_name, user_credentials, payload)
 print(response.json())  # Assuming the response is in JSON format
 ```
 
 ### Stop and Logout
 ```python
 mp.stop()
 mp.logout()
```

### Comparing `modelpark-0.1.4/modelpark/modelpark.py` & `modelpark-0.1.5/modelpark/modelpark.py`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.4/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.5/modelpark.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.4
+Version: 0.1.5
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,20 @@
 Requires-Dist: requests
 
 
 # ModelPark
 
 ModelPark provides a versatile platform to share and manage your ML models directly from your machine, offering a convenient Python API to manage these tasks programmatically, including controlling access and publishing applications.
 
+See [ModelPark](https://modelpark.app/) website and platform for more details.
+
+![image](https://github.com/model-park/modelpark/assets/25637056/6eac80e7-91e9-477a-bcce-bd7d369d932e)
+
+![image](https://github.com/model-park/modelpark/assets/25637056/be495106-915d-4989-818d-dad7bb5abc71)
+
 ## Features
 
 - Share models directly from the Python API.
 - Publish and manage applications using the ModelPark Python API.
 - Configure access management according to your needs through Python methods.
 
 ## Installation
@@ -65,20 +71,23 @@
 ### List Registered Applications
 ```python
 mp.ls()
 ```
 
 ### Make an API Call to a Registered Application
 ```python
+from modelpark import APIManager
+mp_api = APIManager()
+
 user_credentials = {'username': 'your_username', 'password': 'your_password'}
 app_name = 'my-app'
 payload = {'key': 'value'}  # Payload required by the application
 
 # Make the API call
-response = mp.make_api_call(app_name, user_credentials, payload)
+response = mp_api.make_api_call(app_name, user_credentials, payload)
 print(response.json())  # Assuming the response is in JSON format
 ```
 
 ### Stop and Logout
 ```python
 mp.stop()
 mp.logout()
```

### Comparing `modelpark-0.1.4/setup.py` & `modelpark-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             os.makedirs(install_path)
         command = f"powershell Invoke-WebRequest -Uri {url} -OutFile \"{install_path}\\modelpark-cli.exe\""
         subprocess.check_call(command, shell=True)
         print(f"Installed modelpark-cli to {install_path}")
 
 setup(
     name='modelpark',
-    version='0.1.4',
+    version='0.1.5',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
```

