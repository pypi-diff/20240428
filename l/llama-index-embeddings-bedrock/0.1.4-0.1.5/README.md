# Comparing `tmp/llama_index_embeddings_bedrock-0.1.4.tar.gz` & `tmp/llama_index_embeddings_bedrock-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_bedrock-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_embeddings_bedrock-0.1.5.tar", max compression
```

## Comparing `llama_index_embeddings_bedrock-0.1.4.tar` & `llama_index_embeddings_bedrock-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2024-03-03 21:08:07.153082 llama_index_embeddings_bedrock-0.1.4/README.md
--rw-r--r--   0        0        0      115 2024-03-03 21:08:07.153082 llama_index_embeddings_bedrock-0.1.4/llama_index/embeddings/bedrock/__init__.py
--rw-r--r--   0        0        0    15287 2024-03-03 21:08:07.153082 llama_index_embeddings_bedrock-0.1.4/llama_index/embeddings/bedrock/base.py
--rw-r--r--   0        0        0     1471 2024-03-03 21:08:07.153082 llama_index_embeddings_bedrock-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_embeddings_bedrock-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/README.md
+-rw-r--r--   0        0        0      115 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/__init__.py
+-rw-r--r--   0        0        0    15391 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/base.py
+-rw-r--r--   0        0        0     1471 2024-04-28 02:57:16.818756 llama_index_embeddings_bedrock-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_embeddings_bedrock-0.1.5/PKG-INFO
```

### Comparing `llama_index_embeddings_bedrock-0.1.4/llama_index/embeddings/bedrock/base.py` & `llama_index_embeddings_bedrock-0.1.5/llama_index/embeddings/bedrock/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,17 +392,19 @@
                 raise ValueError("Amazon provider does not support list of texts")
             request_body = json.dumps({"inputText": payload})
         elif provider == PROVIDERS.COHERE:
             input_types = {
                 "text": "search_document",
                 "query": "search_query",
             }
+            payload = [payload] if isinstance(payload, str) else payload
+            payload = [p[:2048] if len(p) > 2048 else p for p in payload]
             request_body = json.dumps(
                 {
-                    "texts": [payload] if isinstance(payload, str) else payload,
+                    "texts": payload,
                     "input_type": input_types[input_type],
                     "truncate": "NONE",
                 }
             )
         else:
             raise ValueError("Provider not supported")
         return request_body
```

### Comparing `llama_index_embeddings_bedrock-0.1.4/pyproject.toml` & `llama_index_embeddings_bedrock-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings bedrock integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-bedrock"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 boto3 = "^1.34.23"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_embeddings_bedrock-0.1.4/PKG-INFO` & `llama_index_embeddings_bedrock-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-bedrock
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index embeddings bedrock integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

