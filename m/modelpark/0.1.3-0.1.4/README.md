# Comparing `tmp/modelpark-0.1.3.tar.gz` & `tmp/modelpark-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.3.tar", last modified: Sun Apr 28 10:47:48 2024, max compression
+gzip compressed data, was "modelpark-0.1.4.tar", last modified: Sun Apr 28 12:15:09 2024, max compression
```

## Comparing `modelpark-0.1.3.tar` & `modelpark-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.779221 modelpark-0.1.3/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.3/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.3/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     2574 2024-04-28 10:47:48.779002 modelpark-0.1.3/PKG-INFO
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1775 2024-04-28 10:34:12.000000 modelpark-0.1.3/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.777818 modelpark-0.1.3/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 10:41:20.000000 modelpark-0.1.3/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3318 2024-04-28 10:47:08.000000 modelpark-0.1.3/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 10:47:48.778759 modelpark-0.1.3/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     2574 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 10:47:48.000000 modelpark-0.1.3/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 10:47:48.779271 modelpark-0.1.3/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2277 2024-04-28 10:41:20.000000 modelpark-0.1.3/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.354402 modelpark-0.1.4/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.4/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.4/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2676 2024-04-28 12:15:09.354179 modelpark-0.1.4/PKG-INFO
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1775 2024-04-28 10:34:12.000000 modelpark-0.1.4/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.352883 modelpark-0.1.4/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      311 2024-04-28 12:15:01.000000 modelpark-0.1.4/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     3427 2024-04-28 12:06:59.000000 modelpark-0.1.4/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 12:15:09.353963 modelpark-0.1.4/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2676 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 12:15:09.000000 modelpark-0.1.4/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 12:15:09.354444 modelpark-0.1.4/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2964 2024-04-28 12:15:01.000000 modelpark-0.1.4/setup.py
```

### Comparing `modelpark-0.1.3/LICENSE` & `modelpark-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.3/PKG-INFO` & `modelpark-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.3
+Version: 0.1.4
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 
 # ModelPark
```

### Comparing `modelpark-0.1.3/README.md` & `modelpark-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.3/modelpark/modelpark.py` & `modelpark-0.1.4/modelpark/modelpark.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 class CommandRunner:
     """Executes system commands related to ModelPark CLI operations."""
 
     @staticmethod
     def run_command(command):
         try:
             process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-            stdout, stderr = process.communicate()
-            if process.returncode != 0:
-                print("Error:", stderr)
-                sys.exit(1)
-            return stdout
+            print(f"Started process {process.pid}")
+            if 'init' not in command:
+                stdout, stderr = process.communicate()
+                if process.returncode != 0:
+                    print("Error:", stderr)
+                    sys.exit(1)
+                return stdout
         except subprocess.CalledProcessError as e:
             print("Error:", e.stderr)
             sys.exit(1)
 
-
 class ModelPark:
     def __init__(self):
         pass
 
     def login(self, token=None, username=None, password=None):
         command = "modelpark login"
         if token:
```

### Comparing `modelpark-0.1.3/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.4/modelpark.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.3
+Version: 0.1.4
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 
 # ModelPark
```

### Comparing `modelpark-0.1.3/setup.py` & `modelpark-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,48 @@
     """Custom handler for the 'install' command."""
 
     def run(self):
         install.run(self)
         self.install_system_specific_binary()
 
     def install_system_specific_binary(self):
-        """Download and install the correct binary for the current OS."""
-        system = platform.system().lower()
-        if system == 'linux':
+        """Install different binaries for different OS."""
+        os_type = platform.system().lower()
+        if os_type == "linux":
             url = "https://modelpark.app/dist-folder/modelpark-cli-linux"
             self.download_and_install(url)
-        elif system == 'darwin':  # macOS is identified as 'Darwin'
+        elif os_type == "darwin":  # macOS
             url = "https://modelpark.app/dist-folder/modelpark-cli-macos"
             self.download_and_install(url)
+        elif os_type == "windows":
+            url = "https://modelpark.app/dist/mpinstaller.exe"
+            self.download_and_install_windows(url)
         else:
-            raise Exception(f"Unsupported operating system: {system}")
+            raise Exception(f"Unsupported operating system: {os_type}")
 
     def download_and_install(self, url):
         """Download and install binary from a given URL."""
         target_dir = "/usr/local/bin/modelpark"
         os.makedirs(os.path.dirname(target_dir), exist_ok=True)
         subprocess.check_call(['curl', url, '-o', target_dir])
         subprocess.check_call(['chmod', '+x', target_dir])
         print(f"Installed binary to {target_dir}")
 
+    def download_and_install_windows(self, url):
+        """Specific method to handle Windows installation."""
+        install_path = os.environ.get("APPDATA") + "\\ModelPark"
+        if not os.path.exists(install_path):
+            os.makedirs(install_path)
+        command = f"powershell Invoke-WebRequest -Uri {url} -OutFile \"{install_path}\\modelpark-cli.exe\""
+        subprocess.check_call(command, shell=True)
+        print(f"Installed modelpark-cli to {install_path}")
+
 setup(
     name='modelpark',
-    version='0.1.3',
+    version='0.1.4',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
@@ -51,14 +63,16 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-    ],
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+],
     keywords='modelpark, deployment, cloud, api',
     cmdclass={
         'install': CustomInstall,
     }
 )
```

