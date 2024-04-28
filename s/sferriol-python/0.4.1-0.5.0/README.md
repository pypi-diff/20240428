# Comparing `tmp/sferriol-python-0.4.1.tar.gz` & `tmp/sferriol_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sferriol-python-0.4.1.tar", last modified: Tue Apr  9 09:06:11 2024, max compression
+gzip compressed data, was "sferriol_python-0.5.0.tar", last modified: Sun Apr 28 09:30:48 2024, max compression
```

## Comparing `sferriol-python-0.4.1.tar` & `sferriol_python-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:06:11.150912 sferriol-python-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-09 09:06:11.150912 sferriol-python-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-04-09 09:06:11.162913 sferriol-python-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:06:11.134910 sferriol-python-0.4.1/sferriol/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:06:11.149912 sferriol-python-0.4.1/sferriol/python/
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:06:11.149912 sferriol-python-0.4.1/sferriol/python/dictionary/
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/dictionary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/json.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/object.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-09 08:53:59.000000 sferriol-python-0.4.1/sferriol/python/os.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:06:11.150912 sferriol-python-0.4.1/sferriol_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-09 09:06:11.000000 sferriol-python-0.4.1/sferriol_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-09 09:06:11.000000 sferriol-python-0.4.1/sferriol_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:06:11.000000 sferriol-python-0.4.1/sferriol_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-09 09:06:11.000000 sferriol-python-0.4.1/sferriol_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-04-28 09:30:48.093427 sferriol_python-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.087427 sferriol_python-0.5.0/sferriol/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.089427 sferriol_python-0.5.0/sferriol/python/
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.089427 sferriol_python-0.5.0/sferriol/python/dictionary/
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/dictionary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/object.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-28 09:30:36.000000 sferriol_python-0.5.0/sferriol/python/os.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 09:30:48.090427 sferriol_python-0.5.0/sferriol_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-28 09:30:48.000000 sferriol_python-0.5.0/sferriol_python.egg-info/top_level.txt
```

### Comparing `sferriol-python-0.4.1/LICENSE` & `sferriol_python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/PKG-INFO` & `sferriol_python-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: sferriol-python
-Version: 0.4.1
+Version: 0.5.0
 Summary: python utilities
 Home-page: https://gitlab.in2p3.fr/sferriol-ip2i/sferriol-python
 Author: Sylvain Ferriol
 Author-email: s.ferriol@ipnl.in2p3.fr
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: click; extra == "dev"
+Requires-Dist: yapf; extra == "dev"
 
 # sferriol-python
 
 sferriol-python is a set of useful python libraries.
 
 Clone the project
```

### Comparing `sferriol-python-0.4.1/setup.cfg` & `sferriol_python-0.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,16 @@
 [options]
 packages = find_namespace:
 
 [options.packages.find]
 exclude = *.test
 include = sferriol.*
 
+[options.extras_require]
+dev = 
+	click
+	yapf
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sferriol-python-0.4.1/sferriol/python/__init__.py` & `sferriol_python-0.5.0/sferriol/python/__init__.py`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/sferriol/python/dictionary/__init__.py` & `sferriol_python-0.5.0/sferriol/python/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/sferriol/python/json.py` & `sferriol_python-0.5.0/sferriol/python/json.py`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/sferriol/python/net.py` & `sferriol_python-0.5.0/sferriol/python/net.py`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/sferriol/python/object.py` & `sferriol_python-0.5.0/sferriol/python/object.py`

 * *Files identical despite different names*

### Comparing `sferriol-python-0.4.1/sferriol_python.egg-info/PKG-INFO` & `sferriol_python-0.5.0/sferriol_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: sferriol-python
-Version: 0.4.1
+Version: 0.5.0
 Summary: python utilities
 Home-page: https://gitlab.in2p3.fr/sferriol-ip2i/sferriol-python
 Author: Sylvain Ferriol
 Author-email: s.ferriol@ipnl.in2p3.fr
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: click; extra == "dev"
+Requires-Dist: yapf; extra == "dev"
 
 # sferriol-python
 
 sferriol-python is a set of useful python libraries.
 
 Clone the project
```

