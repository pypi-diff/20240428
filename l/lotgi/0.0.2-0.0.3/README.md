# Comparing `tmp/lotgi-0.0.2.tar.gz` & `tmp/lotgi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.2.tar", last modified: Sat Apr 27 23:41:37 2024, max compression
+gzip compressed data, was "lotgi-0.0.3.tar", last modified: Sat Apr 27 23:49:33 2024, max compression
```

## Comparing `lotgi-0.0.2.tar` & `lotgi-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.948219 lotgi-0.0.2/
--rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:41:37.948023 lotgi-0.0.2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      660 2024-04-27 23:40:58.000000 lotgi-0.0.2/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.945699 lotgi-0.0.2/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.946407 lotgi-0.0.2/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     3748 2024-04-27 23:40:16.000000 lotgi-0.0.2/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.2/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.2/python/lotgi/_openai.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.2/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947247 lotgi-0.0.2/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.2/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     5035 2024-04-27 23:06:34.000000 lotgi-0.0.2/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.2/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947813 lotgi-0.0.2/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       66 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 23:41:37.000000 lotgi-0.0.2/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:41:37.947370 lotgi-0.0.2/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.2/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 23:41:37.948251 lotgi-0.0.2/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.568106 lotgi-0.0.3/
+-rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:49:33.567898 lotgi-0.0.3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      660 2024-04-27 23:49:16.000000 lotgi-0.0.3/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.565422 lotgi-0.0.3/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.566213 lotgi-0.0.3/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     4418 2024-04-27 23:48:47.000000 lotgi-0.0.3/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.3/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.3/python/lotgi/_openai.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.3/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.566989 lotgi-0.0.3/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     1753 2024-04-23 04:44:17.000000 lotgi-0.0.3/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     5035 2024-04-27 23:06:34.000000 lotgi-0.0.3/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.3/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.567629 lotgi-0.0.3/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       66 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-27 23:49:33.000000 lotgi-0.0.3/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-27 23:49:33.567112 lotgi-0.0.3/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.3/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-27 23:49:33.568150 lotgi-0.0.3/setup.cfg
```

### Comparing `lotgi-0.0.2/pyproject.toml` & `lotgi-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "requests",
   "tabulate",
   "transformers",
   "openai",
   "tomli",
   "pandas",
 ]
-version="0.0.2"
+version="0.0.3"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.2/python/lotgi/__init__.py` & `lotgi-0.0.3/python/lotgi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,14 +60,25 @@
 @click.option("--model", required=True, help="The model to run inference with.")
 @click.option("--input-url", required=True, help="The model to run inference with.")
 @click.option("--field", required=True, help="The field within a row containing the data.")
 @click.option("--tradeoff", required=True, default=None, help=f"The tradeoff ({rest.EXECUTION_TRADEOFFS}).")
 def submit(endpoint : str, model : str, input_url : str, field : str, tradeoff : Optional[str]):
     """
     Submit a new batch inference job.
+
+    Your job file is expected to be formatted as a jsonl file. Each line corresponds to a request and should be a json object. Use the `--field` argument to specify which field of the json object contains the text to complete.
+
+    For example, if a file stored at `example.com/dataset.jsonl` contains the contents
+
+    ```\n
+    {"my_completion_text": "hello"}\n
+    {"my_completion_text": "lorem"}\n
+    ```
+
+    You can run `lotgi submit --model mistralai/Mistral-7B-Instruct-v0.2 --input-url example.com/dataset.jsonl --field "my_completion_text" --tradeoff Cheapest`. This will run the mistral-7b model against the inputs "hello" and "lorem", optimizing for cost.
     """
     client = RestClient(endpoint)
 
     if tradeoff is None:
         print(f"Scanning job to estimate costs...")
         job_execution_options_input = estimate_token_usage(input_url=input_url, prompt="", model=model, field=field)
         options = client.job_exection_options(job_execution_options_input=job_execution_options_input)
```

### Comparing `lotgi-0.0.2/python/lotgi/_openai.py` & `lotgi-0.0.3/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.2/python/lotgi/models/rest.py` & `lotgi-0.0.3/python/lotgi/models/rest.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.2/python/lotgi/rest_client.py` & `lotgi-0.0.3/python/lotgi/rest_client.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.2/python/lotgi/tokens.py` & `lotgi-0.0.3/python/lotgi/tokens.py`

 * *Files identical despite different names*

