# Comparing `tmp/cirbreak-0.1.0.tar.gz` & `tmp/cirbreak-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirbreak-0.1.0.tar", last modified: Sun Apr 28 04:31:57 2024, max compression
+gzip compressed data, was "cirbreak-0.1.1.tar", last modified: Sun Apr 28 05:24:02 2024, max compression
```

## Comparing `cirbreak-0.1.0.tar` & `cirbreak-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 04:31:57.134658 cirbreak-0.1.0/
--rw-r--r--   0 mac        (501) staff       (20)     1062 2024-04-28 04:31:02.000000 cirbreak-0.1.0/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1803 2024-04-28 04:31:57.133595 cirbreak-0.1.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1303 2024-04-28 02:50:43.000000 cirbreak-0.1.0/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 04:31:57.102065 cirbreak-0.1.0/cirbreak/
--rw-r--r--   0 mac        (501) staff       (20)       69 2024-04-28 03:25:53.000000 cirbreak-0.1.0/cirbreak/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4206 2024-04-28 03:26:46.000000 cirbreak-0.1.0/cirbreak/cirbreak.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 04:31:57.132879 cirbreak-0.1.0/cirbreak.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1803 2024-04-28 04:31:57.000000 cirbreak-0.1.0/cirbreak.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      239 2024-04-28 04:31:57.000000 cirbreak-0.1.0/cirbreak.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-28 04:31:57.000000 cirbreak-0.1.0/cirbreak.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2024-04-28 04:31:57.000000 cirbreak-0.1.0/cirbreak.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-28 04:31:57.134734 cirbreak-0.1.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      654 2024-04-28 02:53:04.000000 cirbreak-0.1.0/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 04:31:57.130819 cirbreak-0.1.0/test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-28 03:18:36.000000 cirbreak-0.1.0/test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1579 2024-04-28 04:08:09.000000 cirbreak-0.1.0/test/test_cirbreak.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:24:02.824850 cirbreak-0.1.1/
+-rw-r--r--   0 mac        (501) staff       (20)     1062 2024-04-28 04:31:02.000000 cirbreak-0.1.1/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     2342 2024-04-28 05:24:02.817933 cirbreak-0.1.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1842 2024-04-28 05:21:24.000000 cirbreak-0.1.1/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:24:02.788894 cirbreak-0.1.1/cirbreak/
+-rw-r--r--   0 mac        (501) staff       (20)       69 2024-04-28 03:25:53.000000 cirbreak-0.1.1/cirbreak/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4206 2024-04-28 05:14:59.000000 cirbreak-0.1.1/cirbreak/cirbreak.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:24:02.816854 cirbreak-0.1.1/cirbreak.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2342 2024-04-28 05:24:02.000000 cirbreak-0.1.1/cirbreak.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      239 2024-04-28 05:24:02.000000 cirbreak-0.1.1/cirbreak.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-28 05:24:02.000000 cirbreak-0.1.1/cirbreak.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       14 2024-04-28 05:24:02.000000 cirbreak-0.1.1/cirbreak.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-28 05:24:02.824962 cirbreak-0.1.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      654 2024-04-28 05:23:50.000000 cirbreak-0.1.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-28 05:24:02.814471 cirbreak-0.1.1/test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-28 03:18:36.000000 cirbreak-0.1.1/test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1579 2024-04-28 04:08:09.000000 cirbreak-0.1.1/test/test_cirbreak.py
```

### Comparing `cirbreak-0.1.0/LICENSE.txt` & `cirbreak-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirbreak-0.1.0/PKG-INFO` & `cirbreak-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-Metadata-Version: 2.1
-Name: cirbreak
-Version: 0.1.0
-Summary: A Python library implementing a circuit breaker pattern
-Home-page: https://github.com/mario-barrientos-dev/cirbreak
-Author: Mario Alfonso Barrientos Benavides
-Author-email: mariobarrientos0303@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # CircuitBreaker
 
 This Python library provides a `circuit_breaker` decorator for implementing the circuit breaker pattern in your applications.
 
 The circuit breaker pattern is a resiliency mechanism that helps protect external dependencies from cascading failures. It works by monitoring the success and failure rates of calls to a function and taking preventive measures to avoid overloading the dependency.
 
 ### How it Works
 
 The `circuit_breaker` decorator takes several optional arguments:
 
 * `failure_threshold`: The number of consecutive failures allowed before the circuit opens (defaults to 3).
 * `recovery_timeout`: The time window in seconds after which the circuit attempts recovery (defaults to 10).
-* `replace_function`: A function to execute during circuit open state (optional).
+* `replace_function`:  A function to execute during the circuit open state. This function should accept the same arguments as the decorated function (optional).
 * `consecutive`: A flag indicating whether consecutive failures trigger opening (defaults to False).
 
 Here's a basic example of using the decorator:
 
 ```python
+import time
 from cirbreak import circuit_breaker
 
-@circuit_breaker(failure_threshold=5)
-def external_call():
-    # Simulate a call to an external service
-    if random.random() > 0.5:
-        raise Exception("External service error")
-    return "Success!"
-
-try:
-    response = external_call()
-    print(response)
-except Exception as e:
-    print(f"Error: {e}")
+def replace(number):
+    print("Another function", number)
+
+@circuit_breaker(
+    failure_threshold=5, recovery_timeout=10, replace_function=replace, consecutive=False
+)
+def test_circuit_breaker(number):
+    if number % 3 == 0:
+        raise Exception("Number is divisible by 3")
+    else:
+        print(number)
+
+for i in range(1, 30):
+    try:
+        test_circuit_breaker(i)
+    except Exception as e:
+        print(e)
+    time.sleep(1)
+```
+
+In this example, the replace function is provided as the replace_function argument to the circuit_breaker decorator. The replacement function should receive the same arguments as the decorated function. This setup allows for custom handling during the circuit open state, such as logging or alternative processing.
```

### Comparing `cirbreak-0.1.0/cirbreak/cirbreak.py` & `cirbreak-0.1.1/cirbreak/cirbreak.py`

 * *Files identical despite different names*

### Comparing `cirbreak-0.1.0/cirbreak.egg-info/PKG-INFO` & `cirbreak-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirbreak
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library implementing a circuit breaker pattern
 Home-page: https://github.com/mario-barrientos-dev/cirbreak
 Author: Mario Alfonso Barrientos Benavides
 Author-email: mariobarrientos0303@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,27 +20,37 @@
 
 ### How it Works
 
 The `circuit_breaker` decorator takes several optional arguments:
 
 * `failure_threshold`: The number of consecutive failures allowed before the circuit opens (defaults to 3).
 * `recovery_timeout`: The time window in seconds after which the circuit attempts recovery (defaults to 10).
-* `replace_function`: A function to execute during circuit open state (optional).
+* `replace_function`:  A function to execute during the circuit open state. This function should accept the same arguments as the decorated function (optional).
 * `consecutive`: A flag indicating whether consecutive failures trigger opening (defaults to False).
 
 Here's a basic example of using the decorator:
 
 ```python
+import time
 from cirbreak import circuit_breaker
 
-@circuit_breaker(failure_threshold=5)
-def external_call():
-    # Simulate a call to an external service
-    if random.random() > 0.5:
-        raise Exception("External service error")
-    return "Success!"
-
-try:
-    response = external_call()
-    print(response)
-except Exception as e:
-    print(f"Error: {e}")
+def replace(number):
+    print("Another function", number)
+
+@circuit_breaker(
+    failure_threshold=5, recovery_timeout=10, replace_function=replace, consecutive=False
+)
+def test_circuit_breaker(number):
+    if number % 3 == 0:
+        raise Exception("Number is divisible by 3")
+    else:
+        print(number)
+
+for i in range(1, 30):
+    try:
+        test_circuit_breaker(i)
+    except Exception as e:
+        print(e)
+    time.sleep(1)
+```
+
+In this example, the replace function is provided as the replace_function argument to the circuit_breaker decorator. The replacement function should receive the same arguments as the decorated function. This setup allows for custom handling during the circuit open state, such as logging or alternative processing.
```

### Comparing `cirbreak-0.1.0/setup.py` & `cirbreak-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cirbreak",
-    version="0.1.0",
+    version="0.1.1",
     description="A Python library implementing a circuit breaker pattern",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mario-barrientos-dev/cirbreak",
     author="Mario Alfonso Barrientos Benavides",
     author_email="mariobarrientos0303@gmail.com",
     packages=find_packages(),
```

### Comparing `cirbreak-0.1.0/test/test_cirbreak.py` & `cirbreak-0.1.1/test/test_cirbreak.py`

 * *Files identical despite different names*

