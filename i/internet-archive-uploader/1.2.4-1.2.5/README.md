# Comparing `tmp/internet-archive-uploader-1.2.4.tar.gz` & `tmp/internet_archive_uploader-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet-archive-uploader-1.2.4.tar", last modified: Mon Mar 18 03:06:24 2024, max compression
+gzip compressed data, was "internet_archive_uploader-1.2.5.tar", last modified: Sun Apr 28 18:04:06 2024, max compression
```

## Comparing `internet-archive-uploader-1.2.4.tar` & `internet_archive_uploader-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 03:06:24.103056 internet-archive-uploader-1.2.4/
-drwxrwxrwx   0        0        0        0 2024-03-18 03:06:24.081047 internet-archive-uploader-1.2.4/InternetArchiveUploader/
--rw-rw-rw-   0        0        0     2111 2024-03-18 03:05:38.000000 internet-archive-uploader-1.2.4/InternetArchiveUploader/InternetArchiveUploader.py
--rw-rw-rw-   0        0        0       62 2024-03-13 01:08:49.000000 internet-archive-uploader-1.2.4/InternetArchiveUploader/__init__.py
--rw-rw-rw-   0        0        0     1086 2024-03-11 22:53:01.000000 internet-archive-uploader-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     1842 2024-03-18 03:06:24.102052 internet-archive-uploader-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2024-03-15 02:37:17.000000 internet-archive-uploader-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 03:06:24.100052 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/
--rw-rw-rw-   0        0        0     1842 2024-03-18 03:06:24.000000 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-03-18 03:06:24.000000 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 03:06:24.000000 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-18 03:06:24.000000 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-18 03:06:24.000000 internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-03-11 22:58:58.000000 internet-archive-uploader-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 03:06:24.104054 internet-archive-uploader-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-03-18 03:03:44.000000 internet-archive-uploader-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.266933 internet_archive_uploader-1.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.255933 internet_archive_uploader-1.2.5/InternetArchiveUploader/
+-rw-rw-rw-   0        0        0     2111 2024-03-18 03:05:38.000000 internet_archive_uploader-1.2.5/InternetArchiveUploader/InternetArchiveUploader.py
+-rw-rw-rw-   0        0        0       62 2024-03-13 01:08:49.000000 internet_archive_uploader-1.2.5/InternetArchiveUploader/__init__.py
+-rw-rw-rw-   0        0        0     1086 2024-03-11 22:53:01.000000 internet_archive_uploader-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     1871 2024-04-28 18:04:06.265933 internet_archive_uploader-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2024-04-28 17:50:35.000000 internet_archive_uploader-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.265432 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/
+-rw-rw-rw-   0        0        0     1871 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-03-11 22:58:58.000000 internet_archive_uploader-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 18:04:06.267433 internet_archive_uploader-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-28 18:03:51.000000 internet_archive_uploader-1.2.5/setup.py
```

### Comparing `internet-archive-uploader-1.2.4/InternetArchiveUploader/InternetArchiveUploader.py` & `internet_archive_uploader-1.2.5/InternetArchiveUploader/InternetArchiveUploader.py`

 * *Files identical despite different names*

### Comparing `internet-archive-uploader-1.2.4/LICENSE` & `internet_archive_uploader-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `internet-archive-uploader-1.2.4/PKG-INFO` & `internet_archive_uploader-1.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-archive-uploader
-Version: 1.2.4
+Version: 1.2.5
 Summary: A wrapper around the internetarchive package for uploading files and directorys
 Home-page: https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md
 Author: James Gore
 Author-email: jgore077@gmail.com
 License: MIT
 Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 To install the library
 ```
 pip install internet-archive-uploader
 ```
 To use the library
 
 ```python
-import InternetArchiveUploader
+from InternetArchiveUploader import InternetArchiveUploader
 
 uploader= InternetArchiveUploader(
   'myUniqueIdentifier',
   {'metadataAttribute1':'something'},
   'Your Internet Archive username/email',
   'Your Internet Archive password',
 )
```

### Comparing `internet-archive-uploader-1.2.4/README.md` & `internet_archive_uploader-1.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 To install the library
 ```
 pip install internet-archive-uploader
 ```
 To use the library
 
 ```python
-import InternetArchiveUploader
+from InternetArchiveUploader import InternetArchiveUploader
 
 uploader= InternetArchiveUploader(
   'myUniqueIdentifier',
   {'metadataAttribute1':'something'},
   'Your Internet Archive username/email',
   'Your Internet Archive password',
 )
```

### Comparing `internet-archive-uploader-1.2.4/internet_archive_uploader.egg-info/PKG-INFO` & `internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-archive-uploader
-Version: 1.2.4
+Version: 1.2.5
 Summary: A wrapper around the internetarchive package for uploading files and directorys
 Home-page: https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md
 Author: James Gore
 Author-email: jgore077@gmail.com
 License: MIT
 Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 To install the library
 ```
 pip install internet-archive-uploader
 ```
 To use the library
 
 ```python
-import InternetArchiveUploader
+from InternetArchiveUploader import InternetArchiveUploader
 
 uploader= InternetArchiveUploader(
   'myUniqueIdentifier',
   {'metadataAttribute1':'something'},
   'Your Internet Archive username/email',
   'Your Internet Archive password',
 )
```

### Comparing `internet-archive-uploader-1.2.4/setup.py` & `internet_archive_uploader-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 import setuptools
 
 
 setuptools.setup(
     name="internet-archive-uploader",
-    version="1.2.4",
+    version="1.2.5",
     description="A wrapper around the internetarchive package for uploading files and directorys",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md",
     author="James Gore",
     author_email="jgore077@gmail.com",
     license='MIT',
```

