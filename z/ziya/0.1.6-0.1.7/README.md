# Comparing `tmp/ziya-0.1.6.tar.gz` & `tmp/ziya-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.6.tar", max compression
+gzip compressed data, was "ziya-0.1.7.tar", max compression
```

## Comparing `ziya-0.1.6.tar` & `ziya-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.6/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.6/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.6/app/agents/__init__.py
--rw-r--r--   0        0        0     4349 2024-04-27 03:42:52.802293 ziya-0.1.6/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.6/app/agents/prompts.py
--rw-r--r--   0        0        0     3146 2024-04-27 20:21:37.939016 ziya-0.1.6/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.6/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.6/app/utils/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.6/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.6/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      527 2024-04-27 20:33:01.898238 ziya-0.1.6/app/utils/langchain_validation_util.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.6/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.6/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      631 2024-04-27 19:40:53.572399 ziya-0.1.6/app/utils/version_util.py
--rw-r--r--   0        0        0      716 2024-04-27 20:33:49.088179 ziya-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.6/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.6/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.6/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.6/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.6/templates/index.html
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.7/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.7/app/agents/__init__.py
+-rw-r--r--   0        0        0     4382 2024-04-27 20:41:31.407791 ziya-0.1.7/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.7/app/agents/prompts.py
+-rw-r--r--   0        0        0     3146 2024-04-27 20:21:37.939016 ziya-0.1.7/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.7/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.7/app/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.7/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.7/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      527 2024-04-27 20:33:01.898238 ziya-0.1.7/app/utils/langchain_validation_util.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.7/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.7/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      631 2024-04-27 19:40:53.572399 ziya-0.1.7/app/utils/version_util.py
+-rw-r--r--   0        0        0      716 2024-04-27 20:42:21.704624 ziya-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-24 04:42:38.591520 ziya-0.1.7/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.7/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.7/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.7/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-23 01:33:44.760779 ziya-0.1.7/templates/index.html
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.7/PKG-INFO
```

### Comparing `ziya-0.1.6/LICENSE` & `ziya-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/README.md` & `ziya-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/agents/agent.py` & `ziya-0.1.7/app/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "haiku": "anthropic.claude-3-haiku-20240307-v1:0",
     "opus": "anthropic.claude-3-opus-20240229-v1:0",
 }[os.environ.get("ZIYA_AWS_MODEL", "haiku")]
 logger.info(f"Using Claude Model: {model_id}")
 
 model = ChatBedrock(
     model_id=model_id,
-    model_kwargs={"max_tokens": 4096},
+    model_kwargs={"max_tokens": 4096, "temperature": 0.3, "top_k": 15},
     credentials_profile_name=aws_profile if aws_profile else None,
     config=botocore.config.Config(
         read_timeout=900
     )
 )
```

### Comparing `ziya-0.1.6/app/agents/prompts.py` & `ziya-0.1.7/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/main.py` & `ziya-0.1.7/app/main.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/server.py` & `ziya-0.1.7/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/utils/directory_util.py` & `ziya-0.1.7/app/utils/directory_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/utils/gitignore_parser.py` & `ziya-0.1.7/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/utils/langchain_validation_util.py` & `ziya-0.1.7/app/utils/langchain_validation_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/utils/print_tree_util.py` & `ziya-0.1.7/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/app/utils/version_util.py` & `ziya-0.1.7/app/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/pyproject.toml` & `ziya-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.6/static/app.js` & `ziya-0.1.7/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/static/favicon.ico` & `ziya-0.1.7/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/static/sendPayload.js` & `ziya-0.1.7/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/static/ziya.css` & `ziya-0.1.7/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/templates/index.html` & `ziya-0.1.7/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.6/PKG-INFO` & `ziya-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

