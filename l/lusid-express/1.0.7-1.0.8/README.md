# Comparing `tmp/lusid_express-1.0.7.tar.gz` & `tmp/lusid_express-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.7.tar", last modified: Sat Apr 27 19:37:26 2024, max compression
+gzip compressed data, was "lusid_express-1.0.8.tar", last modified: Sat Apr 27 19:41:53 2024, max compression
```

## Comparing `lusid_express-1.0.7.tar` & `lusid_express-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.164184 lusid_express-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:36:46.000000 lusid_express-1.0.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:36:46.000000 lusid_express-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:37:26.164184 lusid_express-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:36:46.000000 lusid_express-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:37:26.164184 lusid_express-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:36:46.000000 lusid_express-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.158186 lusid_express-1.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.160185 lusid_express-1.0.7/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.161185 lusid_express-1.0.7/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:37:25.000000 lusid_express-1.0.7/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.163184 lusid_express-1.0.7/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.164184 lusid_express-1.0.7/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    10739 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:36:46.000000 lusid_express-1.0.7/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:37:26.161185 lusid_express-1.0.7/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:37:26.000000 lusid_express-1.0.7/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.575486 lusid_express-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:41:12.000000 lusid_express-1.0.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:41:12.000000 lusid_express-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:41:53.575486 lusid_express-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:41:12.000000 lusid_express-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:41:53.575486 lusid_express-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:41:12.000000 lusid_express-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.569486 lusid_express-1.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.571486 lusid_express-1.0.8/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.573486 lusid_express-1.0.8/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.574486 lusid_express-1.0.8/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.575486 lusid_express-1.0.8/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.572486 lusid_express-1.0.8/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.7/LICENSE` & `lusid_express-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/PKG-INFO` & `lusid_express-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.7
+Version: 1.0.8
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.7/README.md` & `lusid_express-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/setup.py` & `lusid_express-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.7',
+    version='1.0.8',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.7/src/lusid_express/__main__.py` & `lusid_express-1.0.8/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.8/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.8/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/src/lusid_express/display/__init__.py` & `lusid_express-1.0.8/src/lusid_express/display/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,14 @@
     table = ""
     for key, value in data.items():
         table += get_rows(key, value)
 
     # Ensure the table ID is correctly set and used in the COPY_SCRIPT
     table_id = f"DATA_TABLE-{__uuid.uuid4()}"  # Unique ID for each table instance
     html_output = f"""<h1>{title}</h1> <table id='{table_id}'><tr><th>{col_name_key}</th><th>{col_name_value}</th></tr>{table}</table>{COPY_SCRIPT.replace('REPLACEMENT_HOOK', table_id)}"""
-    print(html_output)
     return html_output
 
 def render_table(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
     Renders table from data.
 
     Parameters:
```

### Comparing `lusid_express-1.0.7/src/lusid_express/load.le` & `lusid_express-1.0.8/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.7/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.8/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.7
+Version: 1.0.8
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

