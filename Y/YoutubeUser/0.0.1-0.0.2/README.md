# Comparing `tmp/YoutubeUser-0.0.1.tar.gz` & `tmp/youtubeuser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YoutubeUser-0.0.1.tar", last modified: Sun Apr 28 02:03:06 2024, max compression
+gzip compressed data, was "youtubeuser-0.0.2.tar", last modified: Sun Apr 28 03:03:32 2024, max compression
```

## Comparing `YoutubeUser-0.0.1.tar` & `youtubeuser-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 02:03:06.213880 YoutubeUser-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-28 02:03:06.213880 YoutubeUser-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 02:03:06.213880 YoutubeUser-0.0.1/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-28 02:03:06.000000 YoutubeUser-0.0.1/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      163 2024-04-28 02:03:06.000000 YoutubeUser-0.0.1/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 02:03:06.000000 YoutubeUser-0.0.1/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 02:03:06.000000 YoutubeUser-0.0.1/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      584 2024-04-28 01:44:46.000000 YoutubeUser-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 02:03:06.213880 YoutubeUser-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      568 2024-04-28 02:02:54.000000 YoutubeUser-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:03:32.842211 youtubeuser-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-28 03:03:32.842211 youtubeuser-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:03:32.842211 youtubeuser-0.0.2/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-28 03:03:32.000000 youtubeuser-0.0.2/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      163 2024-04-28 03:03:32.000000 youtubeuser-0.0.2/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:03:32.000000 youtubeuser-0.0.2/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:03:32.000000 youtubeuser-0.0.2/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      584 2024-04-28 03:01:43.000000 youtubeuser-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:03:32.842211 youtubeuser-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      568 2024-04-28 03:02:35.000000 youtubeuser-0.0.2/setup.py
```

### Comparing `YoutubeUser-0.0.1/pyproject.toml` & `youtubeuser-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YoutubeUser"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Lib For Search Youtube Channels Or User"
 authors = ["R1TGAMING"]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12"
 requests = "^2.31.0"
```

### Comparing `YoutubeUser-0.0.1/setup.py` & `youtubeuser-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YoutubeUser",
-    version='0.0.1',
+    version='0.0.2',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
   
     long_description_content_type='text/markdown',
     url='https://github.com/R1TGAMING/YoutubeUser',
     packages=find_packages(),
```

