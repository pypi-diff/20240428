# Comparing `tmp/mlops_api_gemstack-0.3.9.tar.gz` & `tmp/mlops_api_gemstack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.9.tar", last modified: Sat Apr 27 17:06:28 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.4.0.tar", last modified: Sat Apr 27 17:31:28 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.9.tar` & `mlops_api_gemstack-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.824855 mlops_api_gemstack-0.3.9/
--rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.9/LICENSE
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:06:28.824211 mlops_api_gemstack-0.3.9/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.9/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.814924 mlops_api_gemstack-0.3.9/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    12224 2024-04-27 17:06:20.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:06:28.823366 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 17:06:28.000000 mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 17:06:28.825109 mlops_api_gemstack-0.3.9/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 17:06:14.000000 mlops_api_gemstack-0.3.9/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:31:28.656474 mlops_api_gemstack-0.4.0/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.4.0/LICENSE
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:31:28.655423 mlops_api_gemstack-0.4.0/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.4.0/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:31:28.645781 mlops_api_gemstack-0.4.0/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    12563 2024-04-27 17:30:17.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-27 17:31:28.653137 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-27 17:31:28.000000 mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-27 17:31:28.656656 mlops_api_gemstack-0.4.0/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-27 17:31:25.000000 mlops_api_gemstack-0.4.0/setup.py
```

### Comparing `mlops_api_gemstack-0.3.9/LICENSE` & `mlops_api_gemstack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.9/PKG-INFO` & `mlops_api_gemstack-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_api_gemstack
-Version: 0.3.9
+Version: 0.4.0
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.9/README.md` & `mlops_api_gemstack-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.9/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.4.0/mlops_api_gemstack/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -256,16 +256,16 @@
         else:
             click.echo(f"Failed to upload the file. Status code: {response.status_code}")
 
 @cli.command()
 @click.argument('topics_file', type=click.Path(exists=True))
 @click.argument('rosbag_file_name')
 @click.argument('source')
-@click.option('--delete_rosbag', is_flag=True, default=True, help='Keep the rosbag file after recording')
-def record_rosbag(topics_file, rosbag_file_name, source, delete_rosbag):
+@click.option('--keep_rosbag', is_flag=True, default=False, help='Keep the rosbag file after recording')
+def record_rosbag(topics_file, rosbag_file_name, source, keep_rosbag):
 
     with open(topics_file) as f:
         topics = [line.strip() for line in f.readlines()]
 
     if not topics:
         print(f"No topics found in {topics_file}")
         exit(1)
@@ -286,25 +286,35 @@
 
         pwd = os.getcwd()
         path = os.path.join(pwd, rosbag_file_name)
         print(f"Recording saved at: {path}")
 
         time.sleep(2)
 
-        # check connection
-        net = "IllinoisNet"
-        while(subprocess.check_output("iwgetid -r", shell=True).decode().strip() != net):
-            print("Not connected to IllinoisNet. Retrying in 5 second")
+        while (True):
+            try: 
+                response = requests.get(f"{base_url}")
+                if response.status_code == 404:
+                    break
+            except requests.ConnectionError:
+                print("No internet connection")
+            except requests.Timeout:
+                print("Request timed out")
+            except requests.RequestException as e:
+                print(f"An error occurred: {e}")
+            
+            print("Please check your internet connection")
+            print("Retrying in 5 seconds")
             time.sleep(5)
 
         # send rosbag file through api
         print("Uploading rosbag file")
         upload_bag(path, source)
        
-        if delete_rosbag:
+        if not keep_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
 
     signal.signal(signal.SIGINT, stop_recording)
 
     print("Recording rosbag. Press Ctrl+C to stop recording")
```

### Comparing `mlops_api_gemstack-0.3.9/mlops_api_gemstack.egg-info/PKG-INFO` & `mlops_api_gemstack-0.4.0/mlops_api_gemstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-api-gemstack
-Version: 0.3.9
+Version: 0.4.0
 Summary: An API package connect to a MLops server relating to the GEMstack project.
 Home-page: https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack
 Author: Haoming Sun
 Author-email: ricardosun990122@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mlops_api_gemstack-0.3.9/setup.py` & `mlops_api_gemstack-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3.9',
+    version='0.4.0',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```

