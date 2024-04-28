# Comparing `tmp/werag-0.0.3.tar.gz` & `tmp/werag-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "werag-0.0.3.tar", max compression
+gzip compressed data, was "werag-0.0.4.tar", max compression
```

## Comparing `werag-0.0.3.tar` & `werag-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.3/README.md
--rw-r--r--   0        0        0      622 2024-04-27 09:33:58.798577 werag-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.3/werag/.DS_Store
--rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.3/werag/__init__.py
--rw-r--r--   0        0        0     6198 2024-04-27 05:37:31.637845 werag-0.0.3/werag/client.py
--rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.3/werag/crud.py
--rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.3/werag/db.py
--rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.3/werag/schema.py
--rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.3/werag/schemas/__init__.py
--rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.3/werag/schemas/chunk.py
--rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.3/werag/utils.py
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 werag-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-27 05:08:57.889950 werag-0.0.4/README.md
+-rw-r--r--   0        0        0      593 2024-04-28 12:22:16.471342 werag-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-27 00:27:15.120287 werag-0.0.4/werag/.DS_Store
+-rw-r--r--   0        0        0       25 2024-04-27 03:23:00.642045 werag-0.0.4/werag/__init__.py
+-rw-r--r--   0        0        0     5945 2024-04-28 12:22:08.296656 werag-0.0.4/werag/client.py
+-rw-r--r--   0        0        0     3811 2024-04-27 04:23:52.514873 werag-0.0.4/werag/crud.py
+-rw-r--r--   0        0        0      397 2024-04-27 04:09:42.508612 werag-0.0.4/werag/db.py
+-rw-r--r--   0        0        0      976 2024-04-27 02:28:24.575438 werag-0.0.4/werag/schema.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:20:44.080530 werag-0.0.4/werag/schemas/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-27 00:20:44.080642 werag-0.0.4/werag/schemas/chunk.py
+-rw-r--r--   0        0        0      183 2024-04-27 02:33:17.900723 werag-0.0.4/werag/utils.py
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 werag-0.0.4/PKG-INFO
```

### Comparing `werag-0.0.3/pyproject.toml` & `werag-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "werag"
-version = "0.0.3"
+version = "0.0.4"
 description = "python rag for wechat application"
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "^2.3.0"
 langchain-chroma = "^0"
 langchain-community = "^0"
 langchain-openai = "^0.0.2.post1"
 keble-helpers = "^0"
 html2text = "^2024.2.26"
 tenacity = "^8.2.3"
-sentence-transformers = "^2"
 wechatpy = "^1.8.18"
 bs4 = "^0"
 
 [tool.poetry.group.test.dependencies]
 pydantic-settings = "^2.2.1"
 pytest = "^8.1.1"
```

### Comparing `werag-0.0.3/werag/.DS_Store` & `werag-0.0.4/werag/.DS_Store`

 * *Files identical despite different names*

### Comparing `werag-0.0.3/werag/client.py` & `werag-0.0.4/werag/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from typing import List
 from typing import Optional, Literal
 
 from langchain.chains import LLMChain
 from langchain.document_transformers import Html2TextTransformer
 from langchain_community.document_loaders import TextLoader
 from langchain_community.document_loaders.recursive_url_loader import RecursiveUrlLoader
-from langchain_community.embeddings.sentence_transformer import (
-    SentenceTransformerEmbeddings,
-)
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseChatModel
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from wechatpy import parse_message, create_reply
 
@@ -26,20 +23,18 @@
 
 class WeRag:
     """Core Client for werag service"""
 
     def __init__(self, *,
                  persist_directory: str,
                  collection_name: str = "werag",
-                 embedding_function: Optional[Embeddings] = None,
+                 embedding_function: Embeddings,
                  chunk_size: int = 1000,
                  chunk_overlap: int = 0):
         self._crud = CRUDChroma(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
-        if embedding_function is None:
-            embedding_function = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
         self._chroma = get_chroma(collection_name=collection_name, persist_directory=persist_directory,
                                   embedding_function=embedding_function)
 
     def as_retriever(self, *, user: str,
                      content_type: Optional[str] = None,
                      search_type: Literal["similarity", "mmr", "similarity_score_threshold"] = "similarity",
                      **kwargs):
```

### Comparing `werag-0.0.3/werag/crud.py` & `werag-0.0.4/werag/crud.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.3/werag/schema.py` & `werag-0.0.4/werag/schema.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.3/werag/schemas/chunk.py` & `werag-0.0.4/werag/schemas/chunk.py`

 * *Files identical despite different names*

### Comparing `werag-0.0.3/PKG-INFO` & `werag-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werag
-Version: 0.0.3
+Version: 0.0.4
 Summary: python rag for wechat application
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,13 +12,12 @@
 Requires-Dist: bs4 (>=0,<1)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: keble-helpers (>=0,<1)
 Requires-Dist: langchain-chroma (>=0,<1)
 Requires-Dist: langchain-community (>=0,<1)
 Requires-Dist: langchain-openai (>=0.0.2.post1,<0.0.3)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
-Requires-Dist: sentence-transformers (>=2,<3)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: wechatpy (>=1.8.18,<2.0.0)
 Description-Content-Type: text/markdown
```

