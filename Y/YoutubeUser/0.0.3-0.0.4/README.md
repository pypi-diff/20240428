# Comparing `tmp/youtubeuser-0.0.3.tar.gz` & `tmp/youtubeuser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeuser-0.0.3.tar", last modified: Sun Apr 28 03:16:03 2024, max compression
+gzip compressed data, was "youtubeuser-0.0.4.tar", last modified: Sun Apr 28 03:31:20 2024, max compression
```

## Comparing `youtubeuser-0.0.3.tar` & `youtubeuser-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:16:03.310881 youtubeuser-0.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:16:03.306881 youtubeuser-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:16:03.302881 youtubeuser-0.0.3/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:16:02.000000 youtubeuser-0.0.3/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2024-04-28 03:16:02.000000 youtubeuser-0.0.3/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:16:02.000000 youtubeuser-0.0.3/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-28 03:16:02.000000 youtubeuser-0.0.3/YoutubeUser.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:16:02.000000 youtubeuser-0.0.3/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      584 2024-04-28 03:15:44.000000 youtubeuser-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:16:03.310881 youtubeuser-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      609 2024-04-28 03:15:49.000000 youtubeuser-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:31:20.112866 youtubeuser-0.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:31:20.112866 youtubeuser-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:31:20.112866 youtubeuser-0.0.4/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:31:19.000000 youtubeuser-0.0.4/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      197 2024-04-28 03:31:19.000000 youtubeuser-0.0.4/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:31:19.000000 youtubeuser-0.0.4/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-28 03:31:19.000000 youtubeuser-0.0.4/YoutubeUser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:31:19.000000 youtubeuser-0.0.4/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      607 2024-04-28 03:30:30.000000 youtubeuser-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:31:20.112866 youtubeuser-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      609 2024-04-28 03:31:01.000000 youtubeuser-0.0.4/setup.py
```

### Comparing `youtubeuser-0.0.3/setup.py` & `youtubeuser-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YoutubeUser",
-    version='0.0.3',
+    version='0.0.4',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
   
     long_description_content_type='text/markdown',
     url='https://github.com/R1TGAMING/YoutubeUser',
     packages=find_packages(),
```

