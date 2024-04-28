# Comparing `tmp/pooledmysql-3.0.0.tar.gz` & `tmp/pooledmysql-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pooledmysql-3.0.0.tar", last modified: Tue Apr 23 17:31:07 2024, max compression
+gzip compressed data, was "pooledmysql-3.0.1.tar", last modified: Sun Apr 28 17:04:37 2024, max compression
```

## Comparing `pooledmysql-3.0.0.tar` & `pooledmysql-3.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:31:07.938815 pooledmysql-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 17:31:07.938815 pooledmysql-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-23 17:30:59.000000 pooledmysql-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:31:07.938815 pooledmysql-3.0.0/pooledMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 17:31:07.000000 pooledmysql-3.0.0/pooledMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 17:31:07.000000 pooledmysql-3.0.0/pooledMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:31:07.000000 pooledmysql-3.0.0/pooledMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:31:07.000000 pooledmysql-3.0.0/pooledMySQL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 17:31:07.000000 pooledmysql-3.0.0/pooledMySQL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-04-23 17:30:59.000000 pooledmysql-3.0.0/pooledMySQL.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 17:30:59.000000 pooledmysql-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:31:07.938815 pooledmysql-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/pooledMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 17:04:37.000000 pooledmysql-3.0.1/pooledMySQL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/pooledMySQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 17:04:33.000000 pooledmysql-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:04:37.541029 pooledmysql-3.0.1/setup.cfg
```

### Comparing `pooledmysql-3.0.0/PKG-INFO` & `pooledmysql-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pooledMySQL
-Version: 3.0.0
+Version: 3.0.1
 Summary: A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/pooledMySQL
 Keywords: mysql,pool,threadedmysql,pooledmysql,multithreaded,thread,database,sql
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mysql_connector_python
 Requires-Dist: customisedLogs
 
-# pooledMySQL v3.0.0
+# pooledMySQL v3.0.1
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.0/README.md` & `pooledmysql-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pooledMySQL v3.0.0
+# pooledMySQL v3.0.1
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.0/pooledMySQL.egg-info/PKG-INFO` & `pooledmysql-3.0.1/pooledMySQL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pooledMySQL
-Version: 3.0.0
+Version: 3.0.1
 Summary: A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 Author-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/pooledMySQL
 Keywords: mysql,pool,threadedmysql,pooledmysql,multithreaded,thread,database,sql
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: mysql_connector_python
 Requires-Dist: customisedLogs
 
-# pooledMySQL v3.0.0
+# pooledMySQL v3.0.1
 
 ```pip install pooledMySQL --upgrade```
 
 ###### <br>A well maintained program to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually.
 
 
 <br>To install:
```

### Comparing `pooledmysql-3.0.0/pooledMySQL.py` & `pooledmysql-3.0.1/pooledMySQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __packagename__ = "pooledmysql"
 
 
 def updatePackage():
     from time import sleep
     from json import loads
     import http.client
@@ -178,15 +178,14 @@
             """
             While connection object is alive, keep pinging after every fixed interval
             :return:
             """
             while self.alive:
                 while True:
                     timeUntilNextHeartbeat = max(self.minSendKeepAliveAfter, (self.maxSendKeepAliveAfter - (Imports.time() - self.lastUsed)))
-                    print(timeUntilNextHeartbeat)
                     if timeUntilNextHeartbeat>self.minSendKeepAliveAfter:
                         Imports.sleep(timeUntilNextHeartbeat)
                     else: break
                 self.idle = False
                 try:
                     self.raw.ping(True, 1, 1)
                     self.lastUsed = Imports.time()
```

### Comparing `pooledmysql-3.0.0/pyproject.toml` & `pooledmysql-3.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pooledMySQL"
-version = "3.0.0"
+version = "3.0.1"
 description = "A simple way to have MySQL connection pool which auto-scales infinitely as required. This would help remove problems caused by multithreading, also removed user hassle of manually creating and deleting connections manually."
 
 readme = "README.md"
 authors = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

