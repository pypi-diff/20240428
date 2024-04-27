# Comparing `tmp/lotgi-0.0.1.tar.gz` & `tmp/lotgi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.1.tar", last modified: Sat Apr 27 23:12:31 2024, max compression
+gzip compressed data, was "lotgi-0.0.2.tar", last modified: Sat Apr 27 23:41:37 2024, max compression
```

## Comparing `lotgi-0.0.1.tar` & `lotgi-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300778 lotgi-0.0.1/
--rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 23:12:31.300625 lotgi-0.0.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      637 2024-04-27 23:11:33.000000 lotgi-0.0.1/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.298519 lotgi-0.0.1/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.299227 lotgi-0.0.1/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     3322 2024-04-27 23:10:59.000000 lotgi-0.0.1/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.1/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.1/python/lotgi/_openai.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.1/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.299947 lotgi-0.0.1/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.1/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     5035 2024-04-27 23:06:34.000000 lotgi-0.0.1/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.1/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300453 lotgi-0.0.1/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      409 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       53 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 23:12:31.000000 lotgi-0.0.1/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:12:31.300084 lotgi-0.0.1/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.1/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 23:12:31.300807 lotgi-0.0.1/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.948219 lotgi-0.0.2/
+-rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:41:37.948023 lotgi-0.0.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      660 2024-04-27 23:40:58.000000 lotgi-0.0.2/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.945699 lotgi-0.0.2/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.946407 lotgi-0.0.2/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     3748 2024-04-27 23:40:16.000000 lotgi-0.0.2/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.2/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.2/python/lotgi/_openai.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.2/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947247 lotgi-0.0.2/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.2/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     5035 2024-04-27 23:06:34.000000 lotgi-0.0.2/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.2/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947813 lotgi-0.0.2/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       66 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947370 lotgi-0.0.2/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.2/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 23:41:37.948251 lotgi-0.0.2/setup.cfg
```

### Comparing `lotgi-0.0.1/pyproject.toml` & `lotgi-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 dependencies = [
   "click",
   "pydantic",
   "requests",
   "tabulate",
   "transformers",
   "openai",
+  "tomli",
+  "pandas",
 ]
-version="0.0.1"
+version="0.0.2"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.1/python/lotgi/__init__.py` & `lotgi-0.0.2/python/lotgi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from datetime import timedelta
 from typing import Optional
 import sys
 import requests
 
 @click.group
 def cli():
+    """
+    Lotgi CLI tool.
+    """
     init_logging()
 
 
 def format_duration(duration_s : int) -> str:
     total_hours = duration_s // (60 * 60)
     minutes = (duration_s // 60) % 60
     seconds = duration_s % 60
@@ -53,16 +56,19 @@
             print(f"Invalid tradeoff. Select from {rest.EXECUTION_TRADEOFFS}")
 
 @cli.command
 @click.option("--endpoint", default=None, hidden=True)
 @click.option("--model", required=True, help="The model to run inference with.")
 @click.option("--input-url", required=True, help="The model to run inference with.")
 @click.option("--field", required=True, help="The field within a row containing the data.")
-@click.option("--tradeoff", required=False, default=None, help="The tradeoff (Cheapest or ...).")
+@click.option("--tradeoff", required=True, default=None, help=f"The tradeoff ({rest.EXECUTION_TRADEOFFS}).")
 def submit(endpoint : str, model : str, input_url : str, field : str, tradeoff : Optional[str]):
+    """
+    Submit a new batch inference job.
+    """
     client = RestClient(endpoint)
 
     if tradeoff is None:
         print(f"Scanning job to estimate costs...")
         job_execution_options_input = estimate_token_usage(input_url=input_url, prompt="", model=model, field=field)
         options = client.job_exection_options(job_execution_options_input=job_execution_options_input)
 
@@ -74,24 +80,34 @@
     print("Success!")
     print(result)
 
 
 @cli.command
 @click.option("--endpoint", default=None, hidden=True)
 def list(endpoint : str):
+    """
+    List your batch inferences jobs.
+    """
     client = RestClient(endpoint)
     jobs = client.list_jobs()
 
     print(tabulate([job.model_dump() for job in jobs], headers="keys"))
 
 
 @cli.command
 @click.option("--endpoint", default=None, hidden=True)
 @click.argument("job_id", required=True)
 def get(endpoint : str, job_id : str):
+    """
+    Get the results of a specific job.
+
+    Job results are written to stdout. (Human readable text/errors are written to stderr).
+
+    To store your job results, consider redirecting the job output to a file. `lotg get <job_id> > saved_job_results.jsonl`
+    """
     client = RestClient(endpoint)
     url = None
     try:
         url = client.get_job_results(job_id)
     except KeyError:
         print("Job not found!", file=sys.stderr, flush=True)
         sys.exit(1)
```

### Comparing `lotgi-0.0.1/python/lotgi/_openai.py` & `lotgi-0.0.2/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.1/python/lotgi/models/rest.py` & `lotgi-0.0.2/python/lotgi/models/rest.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.1/python/lotgi/rest_client.py` & `lotgi-0.0.2/python/lotgi/rest_client.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.1/python/lotgi/tokens.py` & `lotgi-0.0.2/python/lotgi/tokens.py`

 * *Files identical despite different names*

