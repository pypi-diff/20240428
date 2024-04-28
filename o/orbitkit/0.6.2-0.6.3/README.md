# Comparing `tmp/orbitkit-0.6.2.tar.gz` & `tmp/orbitkit-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.6.2.tar", last modified: Thu Apr 25 01:45:11 2024, max compression
+gzip compressed data, was "dist/orbitkit-0.6.3.tar", last modified: Sun Apr 28 02:19:22 2024, max compression
```

## Comparing `orbitkit-0.6.2.tar` & `orbitkit-0.6.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.2/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.2/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-25 01:45:11.000000 orbitkit-0.6.2/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.2/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2024-04-25 01:29:34.000000 orbitkit-0.6.2/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.2/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.2/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.2/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.2/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.2/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/pdf_embedding/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.2/orbitkit/pdf_embedding/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.2/orbitkit/pdf_embedding/pdf_txt_embedding.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
--rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_extractor_azure.py
--rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_extractor_orbit.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.2/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.2/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.2/orbitkit/util/util_aliyun.py
--rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.2/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.2/orbitkit/util/util_aws_s3_wrapper.py
--rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.2/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.2/orbitkit/util/util_html.py
--rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.2/orbitkit/util/util_md5.py
--rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.2/orbitkit/util/util_selenium.py
--rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.2/orbitkit/util/util_simple_timer.py
--rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.2/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    22654 2024-03-07 05:22:43.000000 orbitkit-0.6.2/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1119 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       74 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2024-04-25 01:45:11.000000 orbitkit-0.6.2/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2024-04-25 01:45:11.000000 orbitkit-0.6.2/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.2/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.3/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.3/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-28 02:19:22.000000 orbitkit-0.6.3/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.3/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2024-04-28 02:17:53.000000 orbitkit-0.6.3/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.3/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.3/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.3/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.3/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.3/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/pdf_embedding/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.3/orbitkit/pdf_embedding/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.3/orbitkit/pdf_embedding/pdf_txt_embedding.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.3/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.3/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.3/orbitkit/util/util_aliyun.py
+-rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.3/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.3/orbitkit/util/util_aws_s3_wrapper.py
+-rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.3/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.3/orbitkit/util/util_html.py
+-rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.3/orbitkit/util/util_md5.py
+-rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.3/orbitkit/util/util_selenium.py
+-rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.3/orbitkit/util/util_simple_timer.py
+-rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.3/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    22765 2024-04-28 02:17:53.000000 orbitkit-0.6.3/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1119 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       74 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2024-04-28 02:19:22.000000 orbitkit-0.6.3/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2024-04-28 02:19:22.000000 orbitkit-0.6.3/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.3/setup.py
```

### Comparing `orbitkit-0.6.2/LICENSE` & `orbitkit-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/PKG-INFO` & `orbitkit-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.2
+Version: 0.6.3
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.2/README.md` & `orbitkit-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/id_srv/id_gen.py` & `orbitkit-0.6.3/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/lark_send/lark.py` & `orbitkit-0.6.3/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_embedding/pdf_txt_embedding.py` & `orbitkit-0.6.3/orbitkit/pdf_embedding/pdf_txt_embedding.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/exceptions.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_extractor_azure.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_extractor_azure.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/pdf_extractor/pdf_extractor_orbit.py` & `orbitkit-0.6.3/orbitkit/pdf_extractor/pdf_extractor_orbit.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/__init__.py` & `orbitkit-0.6.3/orbitkit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/common.py` & `orbitkit-0.6.3/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_aws.py` & `orbitkit-0.6.3/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_aws_s3_wrapper.py` & `orbitkit-0.6.3/orbitkit/util/util_aws_s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_date.py` & `orbitkit-0.6.3/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_md5.py` & `orbitkit-0.6.3/orbitkit/util/util_md5.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_selenium.py` & `orbitkit-0.6.3/orbitkit/util/util_selenium.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_str.py` & `orbitkit-0.6.3/orbitkit/util/util_str.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/orbitkit/util/util_type_mapping.py` & `orbitkit-0.6.3/orbitkit/util/util_type_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     '''
     Useful constant variables
     '''
 
     EXTEN_OCTET_STREAM = 'application/octet-stream'
     # Application
     EXTEN_APPLI_PDF = 'application/pdf'
+    EXTEN_APPLI_XML = 'application/xml'
     EXTEN_APPLI_JSON = 'application/json'
     EXTEN_APPLI_JS = 'application/x-javascript'
     EXTEN_APPLI_DOC = 'application/msword'
     EXTEN_APPLI_DOCX = 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
     EXTEN_APPLI_XLS = 'application/vnd.ms-excel'
     EXTEN_APPLI_XLSX = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
     EXTEN_APPLI_PPT = 'application/vnd.ms-powerpoint'
@@ -39,14 +40,15 @@
 
 _content_file_mapping = {
     # MIME Types: Applications
     '*': {'application': 'Binary file', 'mine': 'application/octet-stream'},
     'pdf': {'application': 'pdf document', 'mine': 'application/pdf'},
     'json': {'application': 'json document', 'mine': 'application/json'},
     'evy': {'application': 'Corel Envoy', 'mine': 'application/envoy'},
+    'xml': {'application': 'XML document', 'mine': 'application/xml'},
     # Word related
     'dot': {'application': 'Word document template', 'mine': 'application/msword'},
     'doc': {'application': 'Word document', 'mine': 'application/msword'},
     'docx': {'application': 'docx document', 'mine': 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'},
     'docm': {'application': '', 'mine': 'application/vnd.ms-word.document.macroEnabled.12'},  # Added in 07 Mar, 2024
     'dotx': {'application': '', 'mine': 'application/vnd.openxmlformats-officedocument.wordprocessingml.template'},  # Added in 07 Mar, 2024
     'fif': {'application': 'fractal image file', 'mine': 'application/fractals'},
```

### Comparing `orbitkit-0.6.2/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.6.3/orbitkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.2
+Version: 0.6.3
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.2/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.6.3/orbitkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.2/setup.py` & `orbitkit-0.6.3/setup.py`

 * *Files identical despite different names*

