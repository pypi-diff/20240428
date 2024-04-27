# Comparing `tmp/ao3statscraper-0.1.1.tar.gz` & `tmp/ao3statscraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ao3statscraper-0.1.1.tar", last modified: Thu Apr 25 08:56:05 2024, max compression
+gzip compressed data, was "ao3statscraper-0.1.2.tar", last modified: Sat Apr 27 23:33:36 2024, max compression
```

## Comparing `ao3statscraper-0.1.1.tar` & `ao3statscraper-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.1/LICENSE
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48513 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7135 2024-04-25 08:54:10.000000 ao3statscraper-0.1.1/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/ao3statscraper/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/ao3statscraper/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-25 08:55:59.000000 ao3statscraper-0.1.1/ao3statscraper/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2428 2024-04-24 23:01:50.000000 ao3statscraper-0.1.1/ao3statscraper/ao3requester.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6508 2024-04-24 22:59:18.000000 ao3statscraper-0.1.1/ao3statscraper/configuration.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/ao3statscraper/plotting.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/ao3statscraper/pw.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.1/ao3statscraper/scrape.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/ao3statscraper/statsdata.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/ao3statscraper/utils.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/ao3statscraper.egg-info/
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48513 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      558 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/entry_points.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-25 08:56:05.000000 ao3statscraper-0.1.1/ao3statscraper.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1586 2024-04-25 08:55:59.000000 ao3statscraper-0.1.1/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/setup.cfg
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-25 08:56:05.839746 ao3statscraper-0.1.1/tests/
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/tests/test_passwords.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.1/tests/test_writing_data.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.2/LICENSE
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48518 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7140 2024-04-25 15:35:41.000000 ao3statscraper-0.1.2/README.md
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/__init__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-04-27 23:33:23.000000 ao3statscraper-0.1.2/ao3statscraper/__version__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2428 2024-04-24 23:01:50.000000 ao3statscraper-0.1.2/ao3statscraper/ao3requester.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6508 2024-04-24 22:59:18.000000 ao3statscraper-0.1.2/ao3statscraper/configuration.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/plotting.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/pw.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.2/ao3statscraper/scrape.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper/scripts/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      177 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/__init__.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      905 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_hits_to_kudos.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3234 2024-04-24 21:11:36.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3_purge_stats_data.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3660 2024-04-24 21:10:58.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3plot.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3661 2024-04-24 22:55:08.000000 ao3statscraper-0.1.2/ao3statscraper/scripts/ao3scrape.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/statsdata.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/ao3statscraper/utils.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/ao3statscraper.egg-info/
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48518 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      754 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      109 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/requires.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-04-27 23:33:36.000000 ao3statscraper-0.1.2/ao3statscraper.egg-info/top_level.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1613 2024-04-27 23:33:23.000000 ao3statscraper-0.1.2/pyproject.toml
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-04-27 23:33:36.314817 ao3statscraper-0.1.2/setup.cfg
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-04-27 23:33:36.310817 ao3statscraper-0.1.2/tests/
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/tests/test_passwords.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.2/tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.1.1/LICENSE` & `ao3statscraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/PKG-INFO` & `ao3statscraper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -845,15 +845,15 @@
 
 
 
 ## Examples
 
 This is example output what `ao3get` will show you when you run it:
 
-![default running mode, diff](webdata/ao3get.png)
+![default running mode, diff](webdata/ao3get-diff.png)
 
 It will only list the works that have changes since you last cheked (i.e. stored
 a snapshot).
 
 But you can also view all your works:
 
 ![show all works](webdata/ao3get-all.png)
```

### Comparing `ao3statscraper-0.1.1/README.md` & `ao3statscraper-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
 
 
 ## Examples
 
 This is example output what `ao3get` will show you when you run it:
 
-![default running mode, diff](webdata/ao3get.png)
+![default running mode, diff](webdata/ao3get-diff.png)
 
 It will only list the works that have changes since you last cheked (i.e. stored
 a snapshot).
 
 But you can also view all your works:
 
 ![show all works](webdata/ao3get-all.png)
```

### Comparing `ao3statscraper-0.1.1/ao3statscraper/__init__.py` & `ao3statscraper-0.1.2/ao3statscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/ao3requester.py` & `ao3statscraper-0.1.2/ao3statscraper/ao3requester.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/configuration.py` & `ao3statscraper-0.1.2/ao3statscraper/configuration.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/plotting.py` & `ao3statscraper-0.1.2/ao3statscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/pw.py` & `ao3statscraper-0.1.2/ao3statscraper/pw.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/scrape.py` & `ao3statscraper-0.1.2/ao3statscraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/statsdata.py` & `ao3statscraper-0.1.2/ao3statscraper/statsdata.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper/utils.py` & `ao3statscraper-0.1.2/ao3statscraper/utils.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/ao3statscraper.egg-info/PKG-INFO` & `ao3statscraper-0.1.2/ao3statscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -845,15 +845,15 @@
 
 
 
 ## Examples
 
 This is example output what `ao3get` will show you when you run it:
 
-![default running mode, diff](webdata/ao3get.png)
+![default running mode, diff](webdata/ao3get-diff.png)
 
 It will only list the works that have changes since you last cheked (i.e. stored
 a snapshot).
 
 But you can also view all your works:
 
 ![show all works](webdata/ao3get-all.png)
```

### Comparing `ao3statscraper-0.1.1/pyproject.toml` & `ao3statscraper-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["ao3statscraper"]
+packages = ["ao3statscraper", "ao3statscraper.scripts"]
+
 
 [project]
 name = "ao3statscraper"
 description="Scrape stats from your AO3 stats page."
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 authors= [
     { name = "Lars Ikarion", email="lars.ikarion@gmail.com"},
     ]
 license = { file = "LICENSE" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -43,15 +44,15 @@
 ao3get= "ao3statscraper.scripts:ao3scrape"
 
 
 [project.urls]
 "Homepage" = "https://gitlab.com/athenaslilowl1/AO3StatScraper"
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ao3statscraper-0.1.1/tests/test_passwords.py` & `ao3statscraper-0.1.2/tests/test_passwords.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.1/tests/test_writing_data.py` & `ao3statscraper-0.1.2/tests/test_writing_data.py`

 * *Files identical despite different names*

