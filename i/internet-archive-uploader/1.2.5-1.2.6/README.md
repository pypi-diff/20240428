# Comparing `tmp/internet_archive_uploader-1.2.5.tar.gz` & `tmp/internet_archive_uploader-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet_archive_uploader-1.2.5.tar", last modified: Sun Apr 28 18:04:06 2024, max compression
+gzip compressed data, was "internet_archive_uploader-1.2.6.tar", last modified: Sun Apr 28 19:39:49 2024, max compression
```

## Comparing `internet_archive_uploader-1.2.5.tar` & `internet_archive_uploader-1.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.266933 internet_archive_uploader-1.2.5/
-drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.255933 internet_archive_uploader-1.2.5/InternetArchiveUploader/
--rw-rw-rw-   0        0        0     2111 2024-03-18 03:05:38.000000 internet_archive_uploader-1.2.5/InternetArchiveUploader/InternetArchiveUploader.py
--rw-rw-rw-   0        0        0       62 2024-03-13 01:08:49.000000 internet_archive_uploader-1.2.5/InternetArchiveUploader/__init__.py
--rw-rw-rw-   0        0        0     1086 2024-03-11 22:53:01.000000 internet_archive_uploader-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     1871 2024-04-28 18:04:06.265933 internet_archive_uploader-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2024-04-28 17:50:35.000000 internet_archive_uploader-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 18:04:06.265432 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/
--rw-rw-rw-   0        0        0     1871 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-28 18:04:06.000000 internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-03-11 22:58:58.000000 internet_archive_uploader-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 18:04:06.267433 internet_archive_uploader-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-28 18:03:51.000000 internet_archive_uploader-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:39:49.291220 internet_archive_uploader-1.2.6/
+drwxrwxrwx   0        0        0        0 2024-04-28 19:39:49.279720 internet_archive_uploader-1.2.6/InternetArchiveUploader/
+-rw-rw-rw-   0        0        0     2111 2024-03-18 03:05:38.000000 internet_archive_uploader-1.2.6/InternetArchiveUploader/InternetArchiveUploader.py
+-rw-rw-rw-   0        0        0       62 2024-03-13 01:08:49.000000 internet_archive_uploader-1.2.6/InternetArchiveUploader/__init__.py
+-rw-rw-rw-   0        0        0     1086 2024-03-11 22:53:01.000000 internet_archive_uploader-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     1872 2024-04-28 19:39:49.290219 internet_archive_uploader-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2024-04-28 17:50:35.000000 internet_archive_uploader-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 19:39:49.289218 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/
+-rw-rw-rw-   0        0        0     1872 2024-04-28 19:39:49.000000 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-28 19:39:49.000000 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 19:39:49.000000 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-28 19:39:49.000000 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 19:39:49.000000 internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-03-11 22:58:58.000000 internet_archive_uploader-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 19:39:49.291719 internet_archive_uploader-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-04-28 19:39:18.000000 internet_archive_uploader-1.2.6/setup.py
```

### Comparing `internet_archive_uploader-1.2.5/InternetArchiveUploader/InternetArchiveUploader.py` & `internet_archive_uploader-1.2.6/InternetArchiveUploader/InternetArchiveUploader.py`

 * *Files identical despite different names*

### Comparing `internet_archive_uploader-1.2.5/LICENSE` & `internet_archive_uploader-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `internet_archive_uploader-1.2.5/PKG-INFO` & `internet_archive_uploader-1.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internet-archive-uploader
-Version: 1.2.5
+Version: 1.2.6
 Summary: A wrapper around the internetarchive package for uploading files and directorys
 Home-page: https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md
 Author: James Gore
 Author-email: jgore077@gmail.com
 License: MIT
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: internetarchive>=3.6.0
 
 # Internet Archive Uploader
  This project is a simple wrapper for file/directory uploads built around the [Internet Archive](https://archive.org/developers/internetarchive/) library. To use it you must have an existing account on the Internet Archive.
```

### Comparing `internet_archive_uploader-1.2.5/README.md` & `internet_archive_uploader-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `internet_archive_uploader-1.2.5/internet_archive_uploader.egg-info/PKG-INFO` & `internet_archive_uploader-1.2.6/internet_archive_uploader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internet-archive-uploader
-Version: 1.2.5
+Version: 1.2.6
 Summary: A wrapper around the internetarchive package for uploading files and directorys
 Home-page: https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md
 Author: James Gore
 Author-email: jgore077@gmail.com
 License: MIT
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: internetarchive>=3.6.0
 
 # Internet Archive Uploader
  This project is a simple wrapper for file/directory uploads built around the [Internet Archive](https://archive.org/developers/internetarchive/) library. To use it you must have an existing account on the Internet Archive.
```

### Comparing `internet_archive_uploader-1.2.5/setup.py` & `internet_archive_uploader-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 
 import setuptools
 
 
 setuptools.setup(
     name="internet-archive-uploader",
-    version="1.2.5",
+    version="1.2.6",
     description="A wrapper around the internetarchive package for uploading files and directorys",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/jgore077/Internet-Archive-Uploader/blob/master/README.md",
     author="James Gore",
     author_email="jgore077@gmail.com",
     license='MIT',
     project_urls={
         
     },
-    python_requires=">=3.6,<3.12",
+    python_requires=">=3.6,<=3.12",
     install_requires=[
         'internetarchive>=3.6.0'
     ],
     packages=setuptools.find_packages(),
     include_package_data=True,
     
 )
```

