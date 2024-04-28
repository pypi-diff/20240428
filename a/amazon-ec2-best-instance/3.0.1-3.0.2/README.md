# Comparing `tmp/amazon-ec2-best-instance-3.0.1.tar.gz` & `tmp/amazon_ec2_best_instance-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-jnvwgw7_/amazon-ec2-best-instance-3.0.1.tar", last modified: Wed May 17 11:43:02 2023, max compression
+gzip compressed data, was "amazon_ec2_best_instance-3.0.2.tar", last modified: Sun Apr 28 10:03:29 2024, max compression
```

## Comparing `amazon-ec2-best-instance-3.0.1.tar` & `amazon_ec2_best_instance-3.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/
--rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     6791 2023-05-17 10:53:19.000000 amazon-ec2-best-instance-3.0.1/README.md
--rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/pyproject.toml
--rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-3.0.1/setup.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/
--rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/SpotUtils.py
--rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    22672 2023-05-17 11:42:14.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      809 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/top_level.txt
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/test/
--rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test.py
--rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test1.py
--rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test10.py
--rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test11.py
--rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test2.py
--rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test5.py
--rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test6.py
--rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test7.py
--rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test8.py
--rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test9.py
--rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_azs.py
--rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-3.0.1/test/test_cache.py
--rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_2.py
--rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_5.py
--rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_6.py
--rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_7.py
--rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_clients.py
--rw-r--r--   0 alexey     (501) staff       (20)     2145 2023-05-14 14:57:55.000000 amazon-ec2-best-instance-3.0.1/test/test_fast.py
--rw-r--r--   0 alexey     (501) staff       (20)     2186 2023-05-17 11:36:07.000000 amazon-ec2-best-instance-3.0.1/test/test_gpu.py
+drwxr-xr-x   0 aliaksei   (501) staff       (20)        0 2024-04-28 10:03:29.251818 amazon_ec2_best_instance-3.0.2/
+-rw-r--r--   0 aliaksei   (501) staff       (20)     7684 2024-04-28 10:03:29.251757 amazon_ec2_best_instance-3.0.2/PKG-INFO
+-rw-r--r--   0 aliaksei   (501) staff       (20)     7018 2024-04-28 09:45:52.000000 amazon_ec2_best_instance-3.0.2/README.md
+-rw-r--r--   0 aliaksei   (501) staff       (20)        0 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/pyproject.toml
+-rw-r--r--   0 aliaksei   (501) staff       (20)      812 2024-04-28 10:03:29.252057 amazon_ec2_best_instance-3.0.2/setup.cfg
+-rw-r--r--   0 aliaksei   (501) staff       (20)      797 2024-04-28 10:03:15.000000 amazon_ec2_best_instance-3.0.2/setup.py
+drwxr-xr-x   0 aliaksei   (501) staff       (20)        0 2024-04-28 10:03:29.247077 amazon_ec2_best_instance-3.0.2/src/
+drwxr-xr-x   0 aliaksei   (501) staff       (20)        0 2024-04-28 10:03:29.247973 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1677 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/SpotUtils.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)       67 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/__init__.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)    22672 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/main.py
+drwxr-xr-x   0 aliaksei   (501) staff       (20)        0 2024-04-28 10:03:29.251548 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/
+-rw-r--r--   0 aliaksei   (501) staff       (20)     7684 2024-04-28 10:03:29.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/PKG-INFO
+-rw-r--r--   0 aliaksei   (501) staff       (20)      809 2024-04-28 10:03:29.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 aliaksei   (501) staff       (20)        1 2024-04-28 10:03:29.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 aliaksei   (501) staff       (20)       58 2024-04-28 10:03:29.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/requires.txt
+-rw-r--r--   0 aliaksei   (501) staff       (20)       25 2024-04-28 10:03:29.000000 amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/top_level.txt
+drwxr-xr-x   0 aliaksei   (501) staff       (20)        0 2024-04-28 10:03:29.251386 amazon_ec2_best_instance-3.0.2/test/
+-rw-r--r--   0 aliaksei   (501) staff       (20)      914 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1822 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test1.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      870 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test10.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1008 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test11.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1250 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test2.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      242 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test3.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1257 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test4.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1397 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test5.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      804 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test6.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1720 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test7.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1154 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test8.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      517 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test9.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1086 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_azs.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1996 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1869 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_2.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      938 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_3.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1040 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_4.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     1028 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_5.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      638 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_6.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)      599 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_cache_7.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     2138 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_clients.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     2145 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_fast.py
+-rw-r--r--   0 aliaksei   (501) staff       (20)     2186 2024-04-27 10:13:14.000000 amazon_ec2_best_instance-3.0.2/test/test_gpu.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `amazon-ec2-best-instance-3.0.1/PKG-INFO` & `amazon_ec2_best_instance-3.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1
-Name: amazon-ec2-best-instance
-Version: 3.0.1
-Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
-Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
-Author: Aliaksei Kankou
-Author-email: aliaksei.kankou@gmail.com
-Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
-Requires-Python: >3.7.0
-Description-Content-Type: text/markdown
-
 # Amazon EC2 Best Instance (amazon-ec2-best-instance)
 
 Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 
+# Deprecation Notice
+
+> **Important**: This package is deprecated and should no longer be used. Please switch to the 'best-ec2' package by running:
+>
+> ```bash
+> pip install best-ec2
+> ```
+> https://pypi.org/project/best-ec2/
+
 # Prerequisites
 * python3
 * pip3
 * boto3  
 * AWS Account
 * AWS Credentials
 
@@ -190,8 +188,8 @@
     'is_best_price': True
 })
 
 print(response)
 '''
 [{'instance_type': 'r5a.8xlarge', 'price': '0.578100'}, ...]
 '''
-```
+```
```

### Comparing `amazon-ec2-best-instance-3.0.1/README.md` & `amazon_ec2_best_instance-3.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,34 @@
+Metadata-Version: 2.1
+Name: amazon-ec2-best-instance
+Version: 3.0.2
+Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
+Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
+Author: Aliaksei Kankou
+Author-email: aliaksei.kankou@gmail.com
+Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: boto3>=1.23.10
+Requires-Dist: lambda-thread-pool>=0.0.2
+Requires-Dist: requests>=2.30.0
+
 # Amazon EC2 Best Instance (amazon-ec2-best-instance)
 
 Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 
+# Deprecation Notice
+
+> **Important**: This package is deprecated and should no longer be used. Please switch to the 'best-ec2' package by running:
+>
+> ```bash
+> pip install best-ec2
+> ```
+> https://pypi.org/project/best-ec2/
+
 # Prerequisites
 * python3
 * pip3
 * boto3  
 * AWS Account
 * AWS Credentials
 
@@ -179,8 +202,8 @@
     'is_best_price': True
 })
 
 print(response)
 '''
 [{'instance_type': 'r5a.8xlarge', 'price': '0.578100'}, ...]
 '''
-```
+```
```

### Comparing `amazon-ec2-best-instance-3.0.1/setup.cfg` & `amazon_ec2_best_instance-3.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amazon-ec2-best-instance
-version = 3.0.1
+version = 3.0.2
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 project_urls =
```

### Comparing `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/SpotUtils.py` & `amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/SpotUtils.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/main.py` & `amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance/main.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/PKG-INFO` & `amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 3.0.1
+Version: 3.0.2
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
-Requires-Python: >3.7.0
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: boto3>=1.23.10
+Requires-Dist: lambda-thread-pool>=0.0.2
+Requires-Dist: requests>=2.30.0
 
 # Amazon EC2 Best Instance (amazon-ec2-best-instance)
 
 Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 
+# Deprecation Notice
+
+> **Important**: This package is deprecated and should no longer be used. Please switch to the 'best-ec2' package by running:
+>
+> ```bash
+> pip install best-ec2
+> ```
+> https://pypi.org/project/best-ec2/
+
 # Prerequisites
 * python3
 * pip3
 * boto3  
 * AWS Account
 * AWS Credentials
```

### Comparing `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/SOURCES.txt` & `amazon_ec2_best_instance-3.0.2/src/amazon_ec2_best_instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test.py` & `amazon_ec2_best_instance-3.0.2/test/test.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test1.py` & `amazon_ec2_best_instance-3.0.2/test/test1.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test10.py` & `amazon_ec2_best_instance-3.0.2/test/test10.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test11.py` & `amazon_ec2_best_instance-3.0.2/test/test11.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test2.py` & `amazon_ec2_best_instance-3.0.2/test/test2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test4.py` & `amazon_ec2_best_instance-3.0.2/test/test4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test5.py` & `amazon_ec2_best_instance-3.0.2/test/test5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test6.py` & `amazon_ec2_best_instance-3.0.2/test/test6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test7.py` & `amazon_ec2_best_instance-3.0.2/test/test7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test8.py` & `amazon_ec2_best_instance-3.0.2/test/test8.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test9.py` & `amazon_ec2_best_instance-3.0.2/test/test9.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_azs.py` & `amazon_ec2_best_instance-3.0.2/test/test_azs.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_2.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_3.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_3.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_4.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_5.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_6.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_cache_7.py` & `amazon_ec2_best_instance-3.0.2/test/test_cache_7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_clients.py` & `amazon_ec2_best_instance-3.0.2/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_fast.py` & `amazon_ec2_best_instance-3.0.2/test/test_fast.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.1/test/test_gpu.py` & `amazon_ec2_best_instance-3.0.2/test/test_gpu.py`

 * *Files identical despite different names*

