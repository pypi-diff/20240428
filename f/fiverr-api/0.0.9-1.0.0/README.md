# Comparing `tmp/fiverr-api-0.0.9.tar.gz` & `tmp/fiverr_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiverr-api-0.0.9.tar", last modified: Thu Aug 31 17:03:05 2023, max compression
+gzip compressed data, was "fiverr_api-1.0.0.tar", last modified: Sun Apr 28 11:45:47 2024, max compression
```

## Comparing `fiverr-api-0.0.9.tar` & `fiverr_api-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,18 @@
-drwxr-xr-x   0 codix     (1000) codix     (1000)        0 2023-08-31 17:03:05.502211 fiverr-api-0.0.9/
--rw-r--r--   0 codix     (1000) codix     (1000)    35148 2023-08-31 10:33:34.000000 fiverr-api-0.0.9/LICENCE
--rw-r--r--   0 codix     (1000) codix     (1000)     4546 2023-08-31 17:03:05.502211 fiverr-api-0.0.9/PKG-INFO
--rw-r--r--   0 codix     (1000) codix     (1000)     3903 2023-08-31 17:00:21.000000 fiverr-api-0.0.9/README.md
-drwxr-xr-x   0 codix     (1000) codix     (1000)        0 2023-08-31 17:03:05.499211 fiverr-api-0.0.9/fiverr_api/
--rw-r--r--   0 codix     (1000) codix     (1000)        0 2023-08-31 12:16:20.000000 fiverr-api-0.0.9/fiverr_api/__init__.py
-drwxr-xr-x   0 codix     (1000) codix     (1000)        0 2023-08-31 17:03:05.501212 fiverr-api-0.0.9/fiverr_api/scrapers/
--rw-r--r--   0 codix     (1000) codix     (1000)       78 2023-08-31 12:44:20.000000 fiverr-api-0.0.9/fiverr_api/scrapers/__init__.py
--rw-r--r--   0 codix     (1000) codix     (1000)     3761 2023-08-31 14:59:45.000000 fiverr-api-0.0.9/fiverr_api/scrapers/gig_scrape.py
--rw-r--r--   0 codix     (1000) codix     (1000)     8319 2023-08-31 14:59:41.000000 fiverr-api-0.0.9/fiverr_api/scrapers/profile_scrape.py
-drwxr-xr-x   0 codix     (1000) codix     (1000)        0 2023-08-31 17:03:05.501212 fiverr-api-0.0.9/fiverr_api/utils/
--rw-r--r--   0 codix     (1000) codix     (1000)        0 2023-08-31 12:16:20.000000 fiverr-api-0.0.9/fiverr_api/utils/__init__.py
--rw-r--r--   0 codix     (1000) codix     (1000)     1187 2023-08-31 11:23:56.000000 fiverr-api-0.0.9/fiverr_api/utils/actions.py
--rw-r--r--   0 codix     (1000) codix     (1000)     1102 2023-08-31 14:59:07.000000 fiverr-api-0.0.9/fiverr_api/utils/scrape_utils.py
-drwxr-xr-x   0 codix     (1000) codix     (1000)        0 2023-08-31 17:03:05.500211 fiverr-api-0.0.9/fiverr_api.egg-info/
--rw-r--r--   0 codix     (1000) codix     (1000)     4546 2023-08-31 17:03:05.000000 fiverr-api-0.0.9/fiverr_api.egg-info/PKG-INFO
--rw-r--r--   0 codix     (1000) codix     (1000)      412 2023-08-31 17:03:05.000000 fiverr-api-0.0.9/fiverr_api.egg-info/SOURCES.txt
--rw-r--r--   0 codix     (1000) codix     (1000)        1 2023-08-31 17:03:05.000000 fiverr-api-0.0.9/fiverr_api.egg-info/dependency_links.txt
--rw-r--r--   0 codix     (1000) codix     (1000)      173 2023-08-31 17:03:05.000000 fiverr-api-0.0.9/fiverr_api.egg-info/requires.txt
--rw-r--r--   0 codix     (1000) codix     (1000)       11 2023-08-31 17:03:05.000000 fiverr-api-0.0.9/fiverr_api.egg-info/top_level.txt
--rw-r--r--   0 codix     (1000) codix     (1000)       38 2023-08-31 17:03:05.502211 fiverr-api-0.0.9/setup.cfg
--rw-r--r--   0 codix     (1000) codix     (1000)     1214 2023-08-31 12:42:30.000000 fiverr-api-0.0.9/setup.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-04-28 11:45:47.059829 fiverr_api-1.0.0/
+-rw-r--r--   0 codie     (1000) codie     (1000)    35148 2024-04-09 16:46:37.000000 fiverr_api-1.0.0/LICENCE
+-rw-r--r--   0 codie     (1000) codie     (1000)     2866 2024-04-28 11:45:47.058829 fiverr_api-1.0.0/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)     1900 2024-04-28 11:42:30.000000 fiverr_api-1.0.0/README.md
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-04-28 11:45:47.057829 fiverr_api-1.0.0/fiverr_api/
+-rw-r--r--   0 codie     (1000) codie     (1000)       41 2024-04-28 11:30:03.000000 fiverr_api-1.0.0/fiverr_api/__init__.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-04-28 11:45:47.058829 fiverr_api-1.0.0/fiverr_api/utils/
+-rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-04-09 16:46:37.000000 fiverr_api-1.0.0/fiverr_api/utils/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     2111 2024-04-28 11:24:19.000000 fiverr_api-1.0.0/fiverr_api/utils/req.py
+-rw-r--r--   0 codie     (1000) codie     (1000)      531 2024-04-28 11:24:36.000000 fiverr_api-1.0.0/fiverr_api/utils/scrape_utils.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-04-28 11:45:47.058829 fiverr_api-1.0.0/fiverr_api.egg-info/
+-rw-r--r--   0 codie     (1000) codie     (1000)     2866 2024-04-28 11:45:47.000000 fiverr_api-1.0.0/fiverr_api.egg-info/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)      304 2024-04-28 11:45:47.000000 fiverr_api-1.0.0/fiverr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-04-28 11:45:47.000000 fiverr_api-1.0.0/fiverr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)      173 2024-04-28 11:45:47.000000 fiverr_api-1.0.0/fiverr_api.egg-info/requires.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       11 2024-04-28 11:45:47.000000 fiverr_api-1.0.0/fiverr_api.egg-info/top_level.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-04-28 11:45:47.059829 fiverr_api-1.0.0/setup.cfg
+-rw-r--r--   0 codie     (1000) codie     (1000)     1214 2024-04-28 11:43:22.000000 fiverr_api-1.0.0/setup.py
```

### Comparing `fiverr-api-0.0.9/LICENCE` & `fiverr_api-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `fiverr-api-0.0.9/setup.py` & `fiverr_api-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="fiverr-api",
-    version="0.0.9",
+    version="1.0.0",
     description="Fiverr API - Scrape Fiverr gigs, ratings, reviews, prices, profiles, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bishwas-py/fiverr-scraping-api",
     author="Bishwas Bhandari",
     author_email="yo@bishwas.net",
     py_modules=["fiverr_api"],
```

