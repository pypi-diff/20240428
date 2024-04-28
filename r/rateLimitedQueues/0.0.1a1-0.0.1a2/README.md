# Comparing `tmp/ratelimitedqueues-0.0.1a1.tar.gz` & `tmp/ratelimitedqueues-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratelimitedqueues-0.0.1a1.tar", last modified: Thu Apr 25 16:32:55 2024, max compression
+gzip compressed data, was "ratelimitedqueues-0.0.1a2.tar", last modified: Sun Apr 28 13:12:38 2024, max compression
```

## Comparing `ratelimitedqueues-0.0.1a1.tar` & `ratelimitedqueues-0.0.1a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:55.968539 ratelimitedqueues-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 16:32:55.968539 ratelimitedqueues-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 16:32:49.000000 ratelimitedqueues-0.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 16:32:49.000000 ratelimitedqueues-0.0.1a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:32:55.968539 ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 16:32:55.000000 ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 16:32:55.000000 ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:32:55.000000 ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 16:32:55.000000 ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-25 16:32:49.000000 ratelimitedqueues-0.0.1a1/rateLimitedQueues.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:32:55.968539 ratelimitedqueues-0.0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:12:38.162335 ratelimitedqueues-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 13:12:38.158336 ratelimitedqueues-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-28 13:12:33.000000 ratelimitedqueues-0.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-28 13:12:33.000000 ratelimitedqueues-0.0.1a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:12:38.158336 ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 13:12:38.000000 ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-28 13:12:38.000000 ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:12:38.000000 ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 13:12:38.000000 ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-28 13:12:33.000000 ratelimitedqueues-0.0.1a2/rateLimitedQueues.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:12:38.162335 ratelimitedqueues-0.0.1a2/setup.cfg
```

### Comparing `ratelimitedqueues-0.0.1a1/PKG-INFO` & `ratelimitedqueues-0.0.1a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a1
+# rateLimitedQueues v0.0.1a2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

### Comparing `ratelimitedqueues-0.0.1a1/README.md` & `ratelimitedqueues-0.0.1a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# rateLimitedQueues v0.0.1a1
+# rateLimitedQueues v0.0.1a2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

### Comparing `ratelimitedqueues-0.0.1a1/pyproject.toml` & `ratelimitedqueues-0.0.1a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateLimitedQueues"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence."
 readme = "README.md"
 maintainers = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `ratelimitedqueues-0.0.1a1/rateLimitedQueues.egg-info/PKG-INFO` & `ratelimitedqueues-0.0.1a2/rateLimitedQueues.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a1
+# rateLimitedQueues v0.0.1a2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

