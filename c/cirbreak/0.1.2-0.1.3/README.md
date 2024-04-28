# Comparing `tmp/cirbreak-0.1.2.tar.gz` & `tmp/cirbreak-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirbreak-0.1.2.tar", last modified: Sun Apr 28 05:27:43 2024, max compression
+gzip compressed data, was "cirbreak-0.1.3.tar", last modified: Sun Apr 28 06:28:09 2024, max compression
```

## Comparing `cirbreak-0.1.2.tar` & `cirbreak-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:27:43.046280 cirbreak-0.1.2/
--rw-r--r--   0 mac        (501) staff       (20)     1062 2024-04-28 04:31:02.000000 cirbreak-0.1.2/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     2336 2024-04-28 05:27:43.040899 cirbreak-0.1.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1836 2024-04-28 05:27:20.000000 cirbreak-0.1.2/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:27:43.012164 cirbreak-0.1.2/cirbreak/
--rw-r--r--   0 mac        (501) staff       (20)       69 2024-04-28 03:25:53.000000 cirbreak-0.1.2/cirbreak/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4206 2024-04-28 05:14:59.000000 cirbreak-0.1.2/cirbreak/cirbreak.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:27:43.039397 cirbreak-0.1.2/cirbreak.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2336 2024-04-28 05:27:42.000000 cirbreak-0.1.2/cirbreak.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      239 2024-04-28 05:27:42.000000 cirbreak-0.1.2/cirbreak.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-28 05:27:42.000000 cirbreak-0.1.2/cirbreak.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2024-04-28 05:27:42.000000 cirbreak-0.1.2/cirbreak.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-28 05:27:43.046396 cirbreak-0.1.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      654 2024-04-28 05:27:40.000000 cirbreak-0.1.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:27:43.037052 cirbreak-0.1.2/test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-28 03:18:36.000000 cirbreak-0.1.2/test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1579 2024-04-28 04:08:09.000000 cirbreak-0.1.2/test/test_cirbreak.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 06:28:09.933831 cirbreak-0.1.3/
+-rw-r--r--   0 mac        (501) staff       (20)     1062 2024-04-28 04:31:02.000000 cirbreak-0.1.3/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     2336 2024-04-28 06:28:09.932544 cirbreak-0.1.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1836 2024-04-28 05:27:20.000000 cirbreak-0.1.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 06:28:09.905950 cirbreak-0.1.3/cirbreak/
+-rw-r--r--   0 mac        (501) staff       (20)       69 2024-04-28 03:25:53.000000 cirbreak-0.1.3/cirbreak/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4511 2024-04-28 06:23:30.000000 cirbreak-0.1.3/cirbreak/cirbreak.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 06:28:09.931741 cirbreak-0.1.3/cirbreak.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2336 2024-04-28 06:28:09.000000 cirbreak-0.1.3/cirbreak.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      239 2024-04-28 06:28:09.000000 cirbreak-0.1.3/cirbreak.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-28 06:28:09.000000 cirbreak-0.1.3/cirbreak.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       14 2024-04-28 06:28:09.000000 cirbreak-0.1.3/cirbreak.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-28 06:28:09.934071 cirbreak-0.1.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      654 2024-04-28 06:28:07.000000 cirbreak-0.1.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 06:28:09.930619 cirbreak-0.1.3/test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-28 03:18:36.000000 cirbreak-0.1.3/test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1579 2024-04-28 04:08:09.000000 cirbreak-0.1.3/test/test_cirbreak.py
```

### Comparing `cirbreak-0.1.2/LICENSE.txt` & `cirbreak-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirbreak-0.1.2/PKG-INFO` & `cirbreak-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirbreak
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library implementing a circuit breaker pattern
 Home-page: https://github.com/mario-barrientos-dev/cirbreak
 Author: Mario Alfonso Barrientos Benavides
 Author-email: mariobarrientos0303@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cirbreak-0.1.2/README.md` & `cirbreak-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cirbreak-0.1.2/cirbreak/cirbreak.py` & `cirbreak-0.1.3/cirbreak/cirbreak.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,33 +82,36 @@
         self.failure_threshold = failure_threshold
         self.recovery_timeout = recovery_timeout
         self.failure_count = 0
         self.last_failure_time = 0
         self.in_recovery = False
         self.consecutive = False
         self.consecutive = consecutive
+        self.message_error = ''
 
     def call(
         self,
         function: Callable,
         *args: Any,
         replace_function: Optional[Callable] = None,
         **kwargs: Any
     ) -> Any:
         if self.is_open() and not self.attempt_recovery(
             replace_function, *args, **kwargs
         ):
-            raise Exception("Circuit breaker is open (failed).")
+            time_remaining = self.recovery_timeout - (time.time() - self.last_failure_time)
+            raise Exception(f"Circuit breaker is open (failed). Redirecting to another function. Time remaining: {time_remaining} seconds. Function Name: {function.__name__}. Error : {self.message_error}")
         try:
             result = function(*args, **kwargs)
             if self.consecutive:
                 self.reset()
             return result
         except Exception as e:
             self.record_failure()
+            self.message_error = str(e)
             raise e
 
     def is_open(self) -> bool:
         return self.failure_count >= self.failure_threshold
 
     def reset(self) -> None:
         self.failure_count = 0
```

### Comparing `cirbreak-0.1.2/cirbreak.egg-info/PKG-INFO` & `cirbreak-0.1.3/cirbreak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirbreak
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library implementing a circuit breaker pattern
 Home-page: https://github.com/mario-barrientos-dev/cirbreak
 Author: Mario Alfonso Barrientos Benavides
 Author-email: mariobarrientos0303@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cirbreak-0.1.2/setup.py` & `cirbreak-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cirbreak",
-    version="0.1.2",
+    version="0.1.3",
     description="A Python library implementing a circuit breaker pattern",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mario-barrientos-dev/cirbreak",
     author="Mario Alfonso Barrientos Benavides",
     author_email="mariobarrientos0303@gmail.com",
     packages=find_packages(),
```

### Comparing `cirbreak-0.1.2/test/test_cirbreak.py` & `cirbreak-0.1.3/test/test_cirbreak.py`

 * *Files identical despite different names*

