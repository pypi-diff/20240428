# Comparing `tmp/lotgi-0.0.0.tar.gz` & `tmp/lotgi-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.0.tar", last modified: Sat Apr 27 22:39:05 2024, max compression
+gzip compressed data, was "lotgi-0.0.1.tar", last modified: Sat Apr 27 23:12:31 2024, max compression
```

## Comparing `lotgi-0.0.0.tar` & `lotgi-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.852280 lotgi-0.0.0/
--rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 22:39:05.852135 lotgi-0.0.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      643 2024-04-27 22:25:50.000000 lotgi-0.0.0/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.850428 lotgi-0.0.0/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.851097 lotgi-0.0.0/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     3322 2024-04-27 22:29:55.000000 lotgi-0.0.0/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.0/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.0/python/lotgi/_openai.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.0/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.851771 lotgi-0.0.0/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.0/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     4366 2024-04-27 22:32:50.000000 lotgi-0.0.0/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.0/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.851997 lotgi-0.0.0/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       53 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 22:39:05.000000 lotgi-0.0.0/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 22:39:05.851863 lotgi-0.0.0/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.0/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 22:39:05.852309 lotgi-0.0.0/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300778 lotgi-0.0.1/
+-rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 23:12:31.300625 lotgi-0.0.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      637 2024-04-27 23:11:33.000000 lotgi-0.0.1/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.298519 lotgi-0.0.1/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.299227 lotgi-0.0.1/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     3322 2024-04-27 23:10:59.000000 lotgi-0.0.1/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.1/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.1/python/lotgi/_openai.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.1/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.299947 lotgi-0.0.1/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.1/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     5035 2024-04-27 23:06:34.000000 lotgi-0.0.1/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.1/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300453 lotgi-0.0.1/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       53 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300084 lotgi-0.0.1/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.1/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 23:12:31.300807 lotgi-0.0.1/setup.cfg
```

### Comparing `lotgi-0.0.0/pyproject.toml` & `lotgi-0.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "click",
   "pydantic",
   "requests",
   "tabulate",
   "transformers",
   "openai",
 ]
-dynamic = ["version"]
+version="0.0.1"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.0/python/lotgi/__init__.py` & `lotgi-0.0.1/python/lotgi/__init__.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.0/python/lotgi/_openai.py` & `lotgi-0.0.1/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.0/python/lotgi/models/rest.py` & `lotgi-0.0.1/python/lotgi/models/rest.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.0/python/lotgi/rest_client.py` & `lotgi-0.0.1/python/lotgi/rest_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -76,14 +76,17 @@
             huggingface_token=get_huggingface_credentials()
         )
 
         body = job_spec.dict()
 
         result = requests.post(url, headers=self.headers, json=body)
 
+        if result.status_code == 401:
+            raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
+
         if not result.ok:
             raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
 
         return rest.JobStatus.validate(result.json())
 
     def job_exection_options(self, *, job_execution_options_input : rest.JobExecutionOptionsInput) -> List[rest.JobExecutionTradeoffOption]:
         url = f"{self.endpoint}/job_execution_options"
@@ -103,25 +106,33 @@
         ]
 
 
     def list_jobs(self) -> List[rest.JobStatus]:
         url = f"{self.endpoint}/list_jobs"
         result = requests.get(url, headers=self.headers)
 
+        if result.status_code == 401:
+            raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
+
         if not result.ok:
-            raise RuntimeError(f"Request was not successfully submitted. {result.text}")
+            raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
 
         return [
             rest.JobStatus.validate(status)
             for status in result.json()
         ]
 
     def get_job_results(self, job_id : str) -> str:
         url = f"{self.endpoint}/get_job_results"
         result = requests.get(url, headers=self.headers, params={"job_id": job_id})
+
+        if result.status_code == 401:
+            raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
+
         if result.status_code == 404:
             raise KeyError(f"Job doesn't exist! {result.text}")
+
         if not result.ok:
             raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
         return result.json()
```

### Comparing `lotgi-0.0.0/python/lotgi/tokens.py` & `lotgi-0.0.1/python/lotgi/tokens.py`

 * *Files identical despite different names*

