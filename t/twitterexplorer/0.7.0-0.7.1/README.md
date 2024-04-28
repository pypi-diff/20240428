# Comparing `tmp/twitterexplorer-0.7.0.tar.gz` & `tmp/twitterexplorer-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitterexplorer-0.7.0.tar", last modified: Fri Apr 26 13:23:25 2024, max compression
+gzip compressed data, was "twitterexplorer-0.7.1.tar", last modified: Sun Apr 28 09:02:43 2024, max compression
```

## Comparing `twitterexplorer-0.7.0.tar` & `twitterexplorer-0.7.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.465667 twitterexplorer-0.7.0/
--rw-r--r--   0 ap         (501) staff       (20)    35149 2022-03-09 18:04:12.000000 twitterexplorer-0.7.0/LICENSE
--rw-r--r--   0 ap         (501) staff       (20)     6344 2024-04-26 13:23:25.464744 twitterexplorer-0.7.0/PKG-INFO
--rw-r--r--   0 ap         (501) staff       (20)     5766 2023-02-02 19:05:33.000000 twitterexplorer-0.7.0/README.md
--rw-r--r--   0 ap         (501) staff       (20)       38 2024-04-26 13:23:25.465867 twitterexplorer-0.7.0/setup.cfg
--rw-r--r--   0 ap         (501) staff       (20)     1310 2023-03-06 07:41:49.000000 twitterexplorer-0.7.0/setup.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.452182 twitterexplorer-0.7.0/twitterexplorer/
--rw-r--r--   0 ap         (501) staff       (20)       51 2023-01-29 12:30:05.000000 twitterexplorer-0.7.0/twitterexplorer/__init__.py
--rw-r--r--   0 ap         (501) staff       (20)       22 2024-04-26 13:07:18.000000 twitterexplorer-0.7.0/twitterexplorer/__version__.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.457044 twitterexplorer-0.7.0/twitterexplorer/apps/
--rw-r--r--   0 ap         (501) staff       (20)        0 2023-02-02 18:13:22.000000 twitterexplorer-0.7.0/twitterexplorer/apps/__init__.py
--rw-r--r--   0 ap         (501) staff       (20)    13876 2023-02-12 14:04:34.000000 twitterexplorer-0.7.0/twitterexplorer/apps/collector.py
--rw-r--r--   0 ap         (501) staff       (20)    16222 2024-04-21 08:33:31.000000 twitterexplorer-0.7.0/twitterexplorer/apps/visualizer.py
--rw-r--r--   0 ap         (501) staff       (20)     1654 2023-01-29 19:40:52.000000 twitterexplorer-0.7.0/twitterexplorer/constants.py
--rw-r--r--   0 ap         (501) staff       (20)     5510 2024-04-22 12:52:58.000000 twitterexplorer-0.7.0/twitterexplorer/converters.py
--rw-r--r--   0 ap         (501) staff       (20)     2279 2023-01-29 19:39:29.000000 twitterexplorer-0.7.0/twitterexplorer/d3networks.py
--rw-r--r--   0 ap         (501) staff       (20)      547 2023-01-29 19:14:21.000000 twitterexplorer-0.7.0/twitterexplorer/defaults.py
--rw-r--r--   0 ap         (501) staff       (20)     4599 2023-01-30 08:22:02.000000 twitterexplorer-0.7.0/twitterexplorer/helpers.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.462900 twitterexplorer-0.7.0/twitterexplorer/html/
--rw-r--r--   0 ap         (501) staff       (20)     2059 2022-03-24 14:02:48.000000 twitterexplorer-0.7.0/twitterexplorer/html/head.html
--rw-r--r--   0 ap         (501) staff       (20)     3701 2024-04-21 10:23:47.000000 twitterexplorer-0.7.0/twitterexplorer/html/htn_body.html
--rw-r--r--   0 ap         (501) staff       (20)    13099 2024-04-21 08:31:53.000000 twitterexplorer-0.7.0/twitterexplorer/html/htn_graph.js
--rw-r--r--   0 ap         (501) staff       (20)     5816 2023-04-06 10:02:16.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_body.html
--rw-r--r--   0 ap         (501) staff       (20)    20177 2024-04-19 14:50:09.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph.js
--rw-r--r--   0 ap         (501) staff       (20)    20204 2022-11-20 11:09:54.000000 twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph_private.js
--rw-r--r--   0 ap         (501) staff       (20)    10444 2022-11-20 11:10:00.000000 twitterexplorer-0.7.0/twitterexplorer/html/style.css
--rw-r--r--   0 ap         (501) staff       (20)     3644 2022-06-27 14:12:19.000000 twitterexplorer-0.7.0/twitterexplorer/languages.json
--rw-r--r--   0 ap         (501) staff       (20)      757 2023-02-02 18:25:51.000000 twitterexplorer-0.7.0/twitterexplorer/launcher.py
--rw-r--r--   0 ap         (501) staff       (20)     1367 2023-01-27 17:08:54.000000 twitterexplorer-0.7.0/twitterexplorer/legacy.py
--rw-r--r--   0 ap         (501) staff       (20)    23243 2024-04-21 08:35:00.000000 twitterexplorer-0.7.0/twitterexplorer/networks.py
--rw-r--r--   0 ap         (501) staff       (20)     3742 2023-03-27 20:39:36.000000 twitterexplorer-0.7.0/twitterexplorer/plotting.py
--rw-r--r--   0 ap         (501) staff       (20)     3622 2024-04-19 15:21:39.000000 twitterexplorer-0.7.0/twitterexplorer/streamlitutils.py
--rw-r--r--   0 ap         (501) staff       (20)    18521 2023-02-12 14:14:39.000000 twitterexplorer-0.7.0/twitterexplorer/tweetcollector.py
-drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-26 13:23:25.463723 twitterexplorer-0.7.0/twitterexplorer.egg-info/
--rw-r--r--   0 ap         (501) staff       (20)     6344 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/PKG-INFO
--rw-r--r--   0 ap         (501) staff       (20)     1052 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 ap         (501) staff       (20)        1 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 ap         (501) staff       (20)       66 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/entry_points.txt
--rw-r--r--   0 ap         (501) staff       (20)      124 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/requires.txt
--rw-r--r--   0 ap         (501) staff       (20)       16 2024-04-26 13:23:25.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/top_level.txt
--rw-r--r--   0 ap         (501) staff       (20)        1 2023-02-02 19:12:34.000000 twitterexplorer-0.7.0/twitterexplorer.egg-info/zip-safe
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-28 09:02:43.711410 twitterexplorer-0.7.1/
+-rw-r--r--   0 ap         (501) staff       (20)    35149 2022-03-09 18:04:12.000000 twitterexplorer-0.7.1/LICENSE
+-rw-r--r--   0 ap         (501) staff       (20)     6372 2024-04-28 09:02:43.710462 twitterexplorer-0.7.1/PKG-INFO
+-rw-r--r--   0 ap         (501) staff       (20)     5766 2023-02-02 19:05:33.000000 twitterexplorer-0.7.1/README.md
+-rw-r--r--   0 ap         (501) staff       (20)       38 2024-04-28 09:02:43.711625 twitterexplorer-0.7.1/setup.cfg
+-rw-r--r--   0 ap         (501) staff       (20)     1333 2024-04-28 08:55:44.000000 twitterexplorer-0.7.1/setup.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-28 09:02:43.694615 twitterexplorer-0.7.1/twitterexplorer/
+-rw-r--r--   0 ap         (501) staff       (20)       51 2023-01-29 12:30:05.000000 twitterexplorer-0.7.1/twitterexplorer/__init__.py
+-rw-r--r--   0 ap         (501) staff       (20)       22 2024-04-28 09:01:10.000000 twitterexplorer-0.7.1/twitterexplorer/__version__.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-28 09:02:43.702603 twitterexplorer-0.7.1/twitterexplorer/apps/
+-rw-r--r--   0 ap         (501) staff       (20)        0 2023-02-02 18:13:22.000000 twitterexplorer-0.7.1/twitterexplorer/apps/__init__.py
+-rw-r--r--   0 ap         (501) staff       (20)    13876 2023-02-12 14:04:34.000000 twitterexplorer-0.7.1/twitterexplorer/apps/collector.py
+-rw-r--r--   0 ap         (501) staff       (20)    16222 2024-04-21 08:33:31.000000 twitterexplorer-0.7.1/twitterexplorer/apps/visualizer.py
+-rw-r--r--   0 ap         (501) staff       (20)     1654 2023-01-29 19:40:52.000000 twitterexplorer-0.7.1/twitterexplorer/constants.py
+-rw-r--r--   0 ap         (501) staff       (20)     5510 2024-04-22 12:52:58.000000 twitterexplorer-0.7.1/twitterexplorer/converters.py
+-rw-r--r--   0 ap         (501) staff       (20)     2279 2023-01-29 19:39:29.000000 twitterexplorer-0.7.1/twitterexplorer/d3networks.py
+-rw-r--r--   0 ap         (501) staff       (20)      547 2023-01-29 19:14:21.000000 twitterexplorer-0.7.1/twitterexplorer/defaults.py
+-rw-r--r--   0 ap         (501) staff       (20)     4599 2023-01-30 08:22:02.000000 twitterexplorer-0.7.1/twitterexplorer/helpers.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-28 09:02:43.708278 twitterexplorer-0.7.1/twitterexplorer/html/
+-rw-r--r--   0 ap         (501) staff       (20)     2059 2022-03-24 14:02:48.000000 twitterexplorer-0.7.1/twitterexplorer/html/head.html
+-rw-r--r--   0 ap         (501) staff       (20)     3701 2024-04-21 10:23:47.000000 twitterexplorer-0.7.1/twitterexplorer/html/htn_body.html
+-rw-r--r--   0 ap         (501) staff       (20)    13099 2024-04-21 08:31:53.000000 twitterexplorer-0.7.1/twitterexplorer/html/htn_graph.js
+-rw-r--r--   0 ap         (501) staff       (20)     5816 2023-04-06 10:02:16.000000 twitterexplorer-0.7.1/twitterexplorer/html/rtn_body.html
+-rw-r--r--   0 ap         (501) staff       (20)    20177 2024-04-19 14:50:09.000000 twitterexplorer-0.7.1/twitterexplorer/html/rtn_graph.js
+-rw-r--r--   0 ap         (501) staff       (20)    20204 2022-11-20 11:09:54.000000 twitterexplorer-0.7.1/twitterexplorer/html/rtn_graph_private.js
+-rw-r--r--   0 ap         (501) staff       (20)    10444 2022-11-20 11:10:00.000000 twitterexplorer-0.7.1/twitterexplorer/html/style.css
+-rw-r--r--   0 ap         (501) staff       (20)     3644 2022-06-27 14:12:19.000000 twitterexplorer-0.7.1/twitterexplorer/languages.json
+-rw-r--r--   0 ap         (501) staff       (20)      757 2023-02-02 18:25:51.000000 twitterexplorer-0.7.1/twitterexplorer/launcher.py
+-rw-r--r--   0 ap         (501) staff       (20)     1367 2023-01-27 17:08:54.000000 twitterexplorer-0.7.1/twitterexplorer/legacy.py
+-rw-r--r--   0 ap         (501) staff       (20)    23243 2024-04-21 08:35:00.000000 twitterexplorer-0.7.1/twitterexplorer/networks.py
+-rw-r--r--   0 ap         (501) staff       (20)     3742 2023-03-27 20:39:36.000000 twitterexplorer-0.7.1/twitterexplorer/plotting.py
+-rw-r--r--   0 ap         (501) staff       (20)     3622 2024-04-19 15:21:39.000000 twitterexplorer-0.7.1/twitterexplorer/streamlitutils.py
+-rw-r--r--   0 ap         (501) staff       (20)    18521 2023-02-12 14:14:39.000000 twitterexplorer-0.7.1/twitterexplorer/tweetcollector.py
+drwxr-xr-x   0 ap         (501) staff       (20)        0 2024-04-28 09:02:43.709280 twitterexplorer-0.7.1/twitterexplorer.egg-info/
+-rw-r--r--   0 ap         (501) staff       (20)     6372 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 ap         (501) staff       (20)     1052 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 ap         (501) staff       (20)        1 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 ap         (501) staff       (20)       66 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/entry_points.txt
+-rw-r--r--   0 ap         (501) staff       (20)      137 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/requires.txt
+-rw-r--r--   0 ap         (501) staff       (20)       16 2024-04-28 09:02:43.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/top_level.txt
+-rw-r--r--   0 ap         (501) staff       (20)        1 2023-02-02 19:12:34.000000 twitterexplorer-0.7.1/twitterexplorer.egg-info/zip-safe
```

### Comparing `twitterexplorer-0.7.0/LICENSE` & `twitterexplorer-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/PKG-INFO` & `twitterexplorer-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitterexplorer
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python tool for interactive network visualizations of Twitter data.
 Home-page: http://github.com/pournaki/twitter-explorer
 Author: Armin Pournaki
 License: GPLv3
 Keywords: networks,social media
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Requires-Dist: streamlit<2,>=1.7.0
 Requires-Dist: tweepy<5,>=4.6.0
 Requires-Dist: pandas<2,>=1.3.4
 Requires-Dist: python-igraph<1,>=0.9.8
 Requires-Dist: twitwi>=0.15.0
 Requires-Dist: twarc<3,>=2.9.4
 Requires-Dist: louvain>=0.8.0
+Requires-Dist: ebbe>=1.13.2
 
 [![twitter explorer][title-img]][title-url]<br/>
 
 An interface to explore Twitter data through interactive network visualizations.
 
 ## Features
```

### Comparing `twitterexplorer-0.7.0/README.md` & `twitterexplorer-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/setup.py` & `twitterexplorer-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,11 +27,12 @@
         "streamlit>=1.7.0,<2",
         "tweepy>=4.6.0,<5",        
         "pandas>=1.3.4,<2",        
         "python-igraph>=0.9.8,<1",
         "twitwi>=0.15.0",
         "twarc>=2.9.4,<3",
         "louvain>=0.8.0",
+        "ebbe>=1.13.2"
     ],
     entry_points={"console_scripts": ["twitterexplorer=twitterexplorer.launcher:main"]},
     zip_safe=True,
 )
```

### Comparing `twitterexplorer-0.7.0/twitterexplorer/apps/collector.py` & `twitterexplorer-0.7.1/twitterexplorer/apps/collector.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/apps/visualizer.py` & `twitterexplorer-0.7.1/twitterexplorer/apps/visualizer.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/constants.py` & `twitterexplorer-0.7.1/twitterexplorer/constants.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/converters.py` & `twitterexplorer-0.7.1/twitterexplorer/converters.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/d3networks.py` & `twitterexplorer-0.7.1/twitterexplorer/d3networks.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/defaults.py` & `twitterexplorer-0.7.1/twitterexplorer/defaults.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/helpers.py` & `twitterexplorer-0.7.1/twitterexplorer/helpers.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/head.html` & `twitterexplorer-0.7.1/twitterexplorer/html/head.html`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/htn_body.html` & `twitterexplorer-0.7.1/twitterexplorer/html/htn_body.html`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/htn_graph.js` & `twitterexplorer-0.7.1/twitterexplorer/html/htn_graph.js`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/rtn_body.html` & `twitterexplorer-0.7.1/twitterexplorer/html/rtn_body.html`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph.js` & `twitterexplorer-0.7.1/twitterexplorer/html/rtn_graph.js`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/rtn_graph_private.js` & `twitterexplorer-0.7.1/twitterexplorer/html/rtn_graph_private.js`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/html/style.css` & `twitterexplorer-0.7.1/twitterexplorer/html/style.css`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/languages.json` & `twitterexplorer-0.7.1/twitterexplorer/languages.json`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/launcher.py` & `twitterexplorer-0.7.1/twitterexplorer/launcher.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/legacy.py` & `twitterexplorer-0.7.1/twitterexplorer/legacy.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/networks.py` & `twitterexplorer-0.7.1/twitterexplorer/networks.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/plotting.py` & `twitterexplorer-0.7.1/twitterexplorer/plotting.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/streamlitutils.py` & `twitterexplorer-0.7.1/twitterexplorer/streamlitutils.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer/tweetcollector.py` & `twitterexplorer-0.7.1/twitterexplorer/tweetcollector.py`

 * *Files identical despite different names*

### Comparing `twitterexplorer-0.7.0/twitterexplorer.egg-info/PKG-INFO` & `twitterexplorer-0.7.1/twitterexplorer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitterexplorer
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python tool for interactive network visualizations of Twitter data.
 Home-page: http://github.com/pournaki/twitter-explorer
 Author: Armin Pournaki
 License: GPLv3
 Keywords: networks,social media
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Requires-Dist: streamlit<2,>=1.7.0
 Requires-Dist: tweepy<5,>=4.6.0
 Requires-Dist: pandas<2,>=1.3.4
 Requires-Dist: python-igraph<1,>=0.9.8
 Requires-Dist: twitwi>=0.15.0
 Requires-Dist: twarc<3,>=2.9.4
 Requires-Dist: louvain>=0.8.0
+Requires-Dist: ebbe>=1.13.2
 
 [![twitter explorer][title-img]][title-url]<br/>
 
 An interface to explore Twitter data through interactive network visualizations.
 
 ## Features
```

### Comparing `twitterexplorer-0.7.0/twitterexplorer.egg-info/SOURCES.txt` & `twitterexplorer-0.7.1/twitterexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

