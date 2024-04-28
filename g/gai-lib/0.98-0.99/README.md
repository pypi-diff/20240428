# Comparing `tmp/gai-lib-0.98.tar.gz` & `tmp/gai-lib-0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gai-lib-0.98.tar", last modified: Mon Apr 22 11:26:09 2024, max compression
+gzip compressed data, was "gai-lib-0.99.tar", last modified: Tue Apr 23 04:56:37 2024, max compression
```

## Comparing `gai-lib-0.98.tar` & `gai-lib-0.99.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.074779 gai-lib-0.98/
--rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.98/MANIFEST.in
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-22 11:26:09.064779 gai-lib-0.98/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-22 11:26:02.000000 gai-lib-0.98/VERSION
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.054779 gai-lib-0.98/gai/
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.054779 gai-lib-0.98/gai/common/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1084 2024-04-22 09:25:34.000000 gai-lib-0.98/gai/common/StatusListener.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/constants.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.98/gai/common/errors.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.98/gai/common/file_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.98/gai/common/generators_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     8918 2024-04-22 09:37:38.000000 gai-lib-0.98/gai/common/http_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.98/gai/common/image_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.98/gai/common/logging.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.98/gai/common/overlap_splitter.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.98/gai/common/sound_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/utils.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/lib/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.98/gai/lib/ClientBase.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4144 2024-04-21 09:26:10.000000 gai-lib-0.98/gai/lib/GGG.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.98/gai/lib/ITTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5331 2024-04-22 09:33:44.000000 gai-lib-0.98/gai/lib/RAGClientAsync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.98/gai/lib/STTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.98/gai/lib/TTSClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/lib/ttt/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/AnthropicChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/ChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/OpenAIChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     7026 2024-04-16 11:50:57.000000 gai-lib-0.98/gai/lib/ttt/TTTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/tools/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.98/gai/tools/Chunker.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.98/gai/tools/Googler.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/PDFConvert.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/Scraper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3178 2024-04-21 08:24:16.000000 gai-lib-0.98/gai.yml
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai_lib.egg-info/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)      963 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/SOURCES.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/dependency_links.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/entry_points.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/requires.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/top_level.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.98/requirements.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-22 11:26:09.074779 gai-lib-0.98/setup.cfg
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.98/setup.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.679316 gai-lib-0.99/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.99/MANIFEST.in
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-23 04:56:37.679316 gai-lib-0.99/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-23 04:56:32.000000 gai-lib-0.99/VERSION
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.669316 gai-lib-0.99/gai/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.669316 gai-lib-0.99/gai/common/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1084 2024-04-22 09:25:34.000000 gai-lib-0.99/gai/common/StatusListener.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.99/gai/common/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.99/gai/common/constants.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.99/gai/common/errors.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4390 2024-04-22 15:45:01.000000 gai-lib-0.99/gai/common/file_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.99/gai/common/generators_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     8918 2024-04-22 09:37:38.000000 gai-lib-0.99/gai/common/http_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.99/gai/common/image_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.99/gai/common/logging.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.99/gai/common/overlap_splitter.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.99/gai/common/sound_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.99/gai/common/utils.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.669316 gai-lib-0.99/gai/lib/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.99/gai/lib/ClientBase.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4087 2024-04-22 16:23:39.000000 gai-lib-0.99/gai/lib/GGG.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.99/gai/lib/ITTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5448 2024-04-23 02:50:16.000000 gai-lib-0.99/gai/lib/RAGClientAsync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.99/gai/lib/STTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.99/gai/lib/TTSClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/lib/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.669316 gai-lib-0.99/gai/lib/ttt/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/lib/ttt/AnthropicChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/lib/ttt/ChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/lib/ttt/OpenAIChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     7026 2024-04-16 11:50:57.000000 gai-lib-0.99/gai/lib/ttt/TTTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/lib/ttt/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.669316 gai-lib-0.99/gai/tools/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.99/gai/tools/Chunker.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.99/gai/tools/Googler.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/tools/PDFConvert.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/tools/Scraper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.99/gai/tools/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3129 2024-04-23 04:06:40.000000 gai-lib-0.99/gai.yml
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-23 04:56:37.679316 gai-lib-0.99/gai_lib.egg-info/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      963 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/entry_points.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/requires.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-23 04:56:37.000000 gai-lib-0.99/gai_lib.egg-info/top_level.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.99/requirements.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-23 04:56:37.679316 gai-lib-0.99/setup.cfg
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.99/setup.py
```

### Comparing `gai-lib-0.98/PKG-INFO` & `gai-lib-0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.98
+Version: 0.99
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.98/gai/common/StatusListener.py` & `gai-lib-0.99/gai/common/StatusListener.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/errors.py` & `gai-lib-0.99/gai/common/errors.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/file_utils.py` & `gai-lib-0.99/gai/common/file_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import base64
 import hashlib
 import os, zipfile
 import tempfile,shutil,re
 from . import constants,utils
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
+import mimetypes
+
+def is_binary(file_name):
+    mime_type, encoding = mimetypes.guess_type(file_name)
+    return mime_type.startswith('text') if mime_type else False
+
+
 # Remove most non-alphanumeric characters from a filename
 def clean_paths(file_path_or_paths):
     if (isinstance(file_path_or_paths,list)):
         paths = []
         for file_path in file_path_or_paths:
             paths.append(clean_paths(file_path))
         return paths
```

### Comparing `gai-lib-0.98/gai/common/generators_utils.py` & `gai-lib-0.99/gai/common/generators_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/http_utils.py` & `gai-lib-0.99/gai/common/http_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/image_utils.py` & `gai-lib-0.99/gai/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/logging.py` & `gai-lib-0.99/gai/common/logging.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/overlap_splitter.py` & `gai-lib-0.99/gai/common/overlap_splitter.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/sound_utils.py` & `gai-lib-0.99/gai/common/sound_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/common/utils.py` & `gai-lib-0.99/gai/common/utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/lib/GGG.py` & `gai-lib-0.99/gai/lib/GGG.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from gai.lib.ttt.TTTClient import TTTClient
 from gai.lib.STTClient import STTClient
 from gai.lib.TTSClient import TTSClient
 from gai.lib.ITTClient import ITTClient
-from gai.lib.RAGClientSync import RAGClientSync
 from PIL import Image
 import base64
 from io import BytesIO
 
 class GGG:
     client = None
 
@@ -90,11 +89,10 @@
                         {"type": "image_url", "image_url": image_url}
                     ]}
                 ]
                 return self.client(messages=messages, **model_params)
         elif category.lower() == "index":
             raise Exception("The 'index' command has deprecated in GGG. Use RAGClientAsync instead.")
         elif category.lower() == "retrieve":
-            self.client = RAGClientSync(self.config_path)
-            return self.client.retrieve(**model_params)
+            raise Exception("The 'retrieve' command has deprecated in GGG. Use RAGClientAsync instead.")
         else:
             raise Exception(f"Unknown category: {category}")
```

### Comparing `gai-lib-0.98/gai/lib/ITTClient.py` & `gai-lib-0.99/gai/lib/ITTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/lib/RAGClientAsync.py` & `gai-lib-0.99/gai/lib/RAGClientAsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         title="",
         source="",
         authors="",
         publisher="",
         published_date="",
         comments="",
         keywords="", 
-        ws_manager=None):
+        listener_callback=None):
         
         url=os.path.join(self.base_url,"index-file")
         metadata = {
             "title": title,
             "source": source,
             "authors": authors,
             "publisher": publisher,
@@ -75,26 +75,28 @@
                     }
                     response = await http_post_async(url=url, files=files)
                     return response
             except Exception as e:
                 logger.error(e)
                 raise e
     
-        if ws_manager:
-
-            # Create listener
-            ws_url=os.path.join(self.base_url,f"index-file/ws").replace("http","ws")
-            listener = StatusListener(ws_url, collection_name)
-
-            # Start both tasks and return when first task completes then cancel the other
-            send_task=asyncio.create_task(send())
-            listen_task=asyncio.create_task(listener.listen(ws_manager))
-            pending, done = await asyncio.wait([send_task, listen_task], return_when=asyncio.FIRST_COMPLETED)
-            for task in pending:
-                task.cancel()
+        if listener_callback:
+            try:
+                # Create listener
+                ws_url=os.path.join(self.base_url,f"index-file/ws").replace("http","ws")
+                listener = StatusListener(ws_url, collection_name)
+
+                # Start both tasks and return when first task completes then cancel the other
+                send_task=asyncio.create_task(send())
+                listen_task=asyncio.create_task(listener.listen(listener_callback))
+                pending, done = await asyncio.wait([send_task], return_when=asyncio.FIRST_COMPLETED)
+                listen_task.cancel()
+            except Exception as e:
+                logger.error(e)
+                raise e
         else:
             await send()
 
         logger.info("Indexing complete.")
 
     ### ----------------- RETRIEVAL ----------------- ###
```

### Comparing `gai-lib-0.98/gai/lib/STTClient.py` & `gai-lib-0.99/gai/lib/STTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/lib/TTSClient.py` & `gai-lib-0.99/gai/lib/TTSClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/lib/ttt/ChunkWrapper.py` & `gai-lib-0.99/gai/lib/ttt/ChunkWrapper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/lib/ttt/TTTClient.py` & `gai-lib-0.99/gai/lib/ttt/TTTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/tools/Chunker.py` & `gai-lib-0.99/gai/tools/Chunker.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/tools/Googler.py` & `gai-lib-0.99/gai/tools/Googler.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai/tools/Scraper.py` & `gai-lib-0.99/gai/tools/Scraper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/gai.yml` & `gai-lib-0.99/gai.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 default_generator: mistral7b-exllama
 gai_url: "http://localhost:12031"
-#gai_url: "https://gaiaio.ai/api/gen"
+#gai_url: "https://gaiaio.ai/api"
 generators:
     mistral7b-exllama:
         type: ttt
         url: "/gen/v1/chat/completions"
-        #url: "/v1/chat/completions"
         whitelist:
             - temperature
             - top_p
             - min_p
             - top_k
             - max_new_tokens
             - typical
@@ -31,15 +30,15 @@
             token_repetition_penalty_decay: 128
             beams: 1
             beam_length: 1
         env:
             gai_api_key: "gai_api_key"
     mistral7b_128k-exllama:
         type: ttt
-        url: "/v1/longchat/completions"
+        url: "/gen/v1/longchat/completions"
         whitelist:
             - temperature
             - top_p
             - min_p
             - top_k
             - max_new_tokens
             - typical
@@ -96,24 +95,23 @@
             top_p: 0.15
             top_k: 50
             max_tokens_to_sample: 1000
         env:
             anthropic_api_key: "anthropic_api_key"
     whisper-transformers:
         type: stt
-        url: "/v1/audio/transcriptions"
+        url: "/gen/v1/audio/transcriptions"
         env:
             gai_api_key: "gai_api_key"
     xtts-2:
         type: tts
-        url: "/v1/audio/speech"
+        url: "/gen/v1/audio/speech"
         env:
             gai_api_key: "gai_api_key"
     llava-transformers:
         type: itt
-        url: "/v1/vision/completions"
+        url: "/gen/v1/vision/completions"
     rag:
         type: rag
         url: "/gen/v1/rag"
-        #url: "/v1/rag"
         env:
             gai_api_key: "gai_api_key"
```

### Comparing `gai-lib-0.98/gai_lib.egg-info/PKG-INFO` & `gai-lib-0.99/gai_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.98
+Version: 0.99
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.98/gai_lib.egg-info/SOURCES.txt` & `gai-lib-0.99/gai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gai-lib-0.98/setup.py` & `gai-lib-0.99/setup.py`

 * *Files identical despite different names*

