# Comparing `tmp/citation_crawler-2.9.4.tar.gz` & `tmp/citation_crawler-2.9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.9.4.tar", last modified: Mon Apr 22 23:28:01 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.4.1.tar", last modified: Mon Apr 22 23:34:01 2024, max compression
```

## Comparing `citation_crawler-2.9.4.tar` & `citation_crawler-2.9.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.673512 citation_crawler-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:28:01.673512 citation_crawler-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.669512 citation_crawler-2.9.4/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.669512 citation_crawler-2.9.4/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.673512 citation_crawler-2.9.4/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.673512 citation_crawler-2.9.4/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:01.669512 citation_crawler-2.9.4/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:28:01.000000 citation_crawler-2.9.4/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:28:01.000000 citation_crawler-2.9.4/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:28:01.000000 citation_crawler-2.9.4/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:28:01.000000 citation_crawler-2.9.4/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:28:01.000000 citation_crawler-2.9.4/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:28:01.673512 citation_crawler-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 23:27:55.000000 citation_crawler-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.077200 citation_crawler-2.9.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:34:01.073200 citation_crawler-2.9.4.1/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-22 23:34:01.000000 citation_crawler-2.9.4.1/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:34:01.000000 citation_crawler-2.9.4.1/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:34:01.000000 citation_crawler-2.9.4.1/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:34:01.000000 citation_crawler-2.9.4.1/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:34:01.000000 citation_crawler-2.9.4.1/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:34:01.077200 citation_crawler-2.9.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 23:33:55.000000 citation_crawler-2.9.4.1/setup.py
```

### Comparing `citation_crawler-2.9.4/LICENSE` & `citation_crawler-2.9.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/PKG-INFO` & `citation_crawler-2.9.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.9.4
+Version: 2.9.4.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.4/README.md` & `citation_crawler-2.9.4.1/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/__main__.py` & `citation_crawler-2.9.4.1/citation_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/arg.py` & `citation_crawler-2.9.4.1/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/crawlers/common.py` & `citation_crawler-2.9.4.1/citation_crawler/crawlers/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 async def download_item(url: str, path: str, cache_days: int, is_valid: Callable[[str], None]) -> Optional[Dict]:
     save_path = os.path.join("save", path)
     if os.path.isfile(save_path):
         if cache_days < 0 or datetime.now() < get_cache_datetime(save_path) + timedelta(days=cache_days):
             async with file_sem:
                 try:
                     async with async_open(save_path, 'r') as f:
-                        logger.info("use cache: %s -> %s" % (path, url))
+                        logger.debug("use cache: %s -> %s" % (path, url))
                         text = await f.read()
                     assert is_valid(text)
                     return text
                 except:
                     logger.info(" no cache: %s" % save_path)
                     if os.path.exists(save_path):
                         logger.info("err cache: %s" % save_path)
```

### Comparing `citation_crawler-2.9.4/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9.4.1/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/graph.py` & `citation_crawler-2.9.4.1/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/init/neo4j.py` & `citation_crawler-2.9.4.1/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/items.py` & `citation_crawler-2.9.4.1/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9.4.1/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9.4.1/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9.4.1/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.9.4
+Version: 2.9.4.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.4/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9.4.1/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.4/setup.py` & `citation_crawler-2.9.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.9.4',
+    version='2.9.4.1',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

