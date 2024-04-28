# Comparing `tmp/pymatris-0.0.0.tar.gz` & `tmp/pymatris-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatris-0.0.0.tar", max compression
+gzip compressed data, was "pymatris-0.0.1.tar", max compression
```

## Comparing `pymatris-0.0.0.tar` & `pymatris-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-24 15:10:23.511842 pymatris-0.0.0/README.md
--rw-r--r--   0        0        0      219 2024-04-27 07:16:12.969026 pymatris-0.0.0/pymatris/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-27 14:16:42.070918 pymatris-0.0.0/pymatris/config.py
--rw-r--r--   0        0        0     9018 2024-04-27 14:13:26.255617 pymatris-0.0.0/pymatris/downloader.py
--rw-r--r--   0        0        0     2231 2024-04-26 19:42:44.665309 pymatris-0.0.0/pymatris/exceptions.py
--rw-r--r--   0        0        0     3262 2024-04-27 14:31:05.823231 pymatris-0.0.0/pymatris/main.py
--rw-r--r--   0        0        0      383 2024-04-27 07:15:55.830710 pymatris-0.0.0/pymatris/protocol_handler/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-27 07:02:20.960570 pymatris-0.0.0/pymatris/protocol_handler/base_handler.py
--rw-r--r--   0        0        0     3778 2024-04-27 14:11:10.977444 pymatris-0.0.0/pymatris/protocol_handler/ftp_handler.py
--rw-r--r--   0        0        0     6037 2024-04-27 14:11:03.287274 pymatris-0.0.0/pymatris/protocol_handler/http_handler.py
--rw-r--r--   0        0        0     4632 2024-04-27 14:11:15.838959 pymatris-0.0.0/pymatris/protocol_handler/sftp_handler.py
--rw-r--r--   0        0        0     2678 2024-04-27 14:26:25.268375 pymatris-0.0.0/pymatris/results.py
--rw-r--r--   0        0        0    11575 2024-04-27 13:34:05.879408 pymatris-0.0.0/pymatris/utils.py
--rw-r--r--   0        0        0      448 2024-04-27 07:13:12.702212 pymatris-0.0.0/pymatris/write_worker.py
--rw-r--r--   0        0        0     1199 2024-04-27 14:47:19.516583 pymatris-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 pymatris-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 15:10:23.511842 pymatris-0.0.1/README.md
+-rw-r--r--   0        0        0      219 2024-04-27 07:16:12.969026 pymatris-0.0.1/pymatris/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-27 14:16:42.070918 pymatris-0.0.1/pymatris/config.py
+-rw-r--r--   0        0        0     9018 2024-04-27 14:13:26.255617 pymatris-0.0.1/pymatris/downloader.py
+-rw-r--r--   0        0        0     2231 2024-04-26 19:42:44.665309 pymatris-0.0.1/pymatris/exceptions.py
+-rw-r--r--   0        0        0     3262 2024-04-27 14:31:05.823231 pymatris-0.0.1/pymatris/main.py
+-rw-r--r--   0        0        0      383 2024-04-27 07:15:55.830710 pymatris-0.0.1/pymatris/protocol_handler/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-27 07:02:20.960570 pymatris-0.0.1/pymatris/protocol_handler/base_handler.py
+-rw-r--r--   0        0        0     3778 2024-04-27 15:20:22.180014 pymatris-0.0.1/pymatris/protocol_handler/ftp_handler.py
+-rw-r--r--   0        0        0     6037 2024-04-27 14:11:03.287274 pymatris-0.0.1/pymatris/protocol_handler/http_handler.py
+-rw-r--r--   0        0        0     4632 2024-04-27 14:11:15.838959 pymatris-0.0.1/pymatris/protocol_handler/sftp_handler.py
+-rw-r--r--   0        0        0     2678 2024-04-27 14:26:25.268375 pymatris-0.0.1/pymatris/results.py
+-rw-r--r--   0        0        0    11575 2024-04-27 13:34:05.879408 pymatris-0.0.1/pymatris/utils.py
+-rw-r--r--   0        0        0      448 2024-04-27 07:13:12.702212 pymatris-0.0.1/pymatris/write_worker.py
+-rw-r--r--   0        0        0     1144 2024-04-27 15:39:13.347451 pymatris-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 pymatris-0.0.1/PKG-INFO
```

### Comparing `pymatris-0.0.0/pymatris/config.py` & `pymatris-0.0.1/pymatris/config.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/downloader.py` & `pymatris-0.0.1/pymatris/downloader.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/exceptions.py` & `pymatris-0.0.1/pymatris/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/main.py` & `pymatris-0.0.1/pymatris/main.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/protocol_handler/base_handler.py` & `pymatris-0.0.1/pymatris/protocol_handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/protocol_handler/ftp_handler.py` & `pymatris-0.0.1/pymatris/protocol_handler/ftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/protocol_handler/http_handler.py` & `pymatris-0.0.1/pymatris/protocol_handler/http_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/protocol_handler/sftp_handler.py` & `pymatris-0.0.1/pymatris/protocol_handler/sftp_handler.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/results.py` & `pymatris-0.0.1/pymatris/results.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/pymatris/utils.py` & `pymatris-0.0.1/pymatris/utils.py`

 * *Files identical despite different names*

### Comparing `pymatris-0.0.0/PKG-INFO` & `pymatris-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: pymatris
-Version: 0.0.0
-Summary: 
+Version: 0.0.1
+Summary: Parallel download manager for HTTP/HTTPS/FTP/SFTP protocols.
+Keywords: downloader,download-manager,http/https,sftp,ftp
 Author: zhuolisam
 Author-email: zhuolisam0627@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aioftp (>=0.22.3,<0.23.0)
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: asyncssh (>=2.14.2,<3.0.0)
 Requires-Dist: pytest-sftpserver (>=1.3.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Project-URL: Documentation, https://github.com/zhuolisam/pymatris
+Project-URL: Homepage, https://github.com/zhuolisam/pymatris
+Project-URL: Source Code, https://github.com/zhuolisam/pymatris
 Description-Content-Type: text/markdown
```

