# Comparing `tmp/gtbook-0.0.8.tar.gz` & `tmp/gtbook-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtbook-0.0.8.tar", last modified: Sat Jan  8 22:30:40 2022, max compression
+gzip compressed data, was "gtbook-0.0.9.tar", last modified: Mon Jan 10 00:49:22 2022, max compression
```

## Comparing `gtbook-0.0.8.tar` & `gtbook-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-08 22:30:40.284991 gtbook-0.0.8/
--rw-r--r--   0 dellaert   (502) staff       (20)     2348 2022-01-07 03:14:53.000000 gtbook-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 dellaert   (502) staff       (20)    11357 2022-01-07 03:14:53.000000 gtbook-0.0.8/LICENSE
--rw-r--r--   0 dellaert   (502) staff       (20)      111 2022-01-07 03:14:53.000000 gtbook-0.0.8/MANIFEST.in
--rw-r--r--   0 dellaert   (502) staff       (20)     1729 2022-01-08 22:30:40.284824 gtbook-0.0.8/PKG-INFO
--rw-r--r--   0 dellaert   (502) staff       (20)      980 2022-01-08 22:28:30.000000 gtbook-0.0.8/README.md
-drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-08 22:30:40.283322 gtbook-0.0.8/gtbook/
--rw-r--r--   0 dellaert   (502) staff       (20)       22 2022-01-08 22:28:26.000000 gtbook-0.0.8/gtbook/__init__.py
--rw-r--r--   0 dellaert   (502) staff       (20)      546 2022-01-08 22:28:26.000000 gtbook-0.0.8/gtbook/_nbdev.py
--rw-r--r--   0 dellaert   (502) staff       (20)      966 2022-01-08 22:28:26.000000 gtbook-0.0.8/gtbook/cli.py
--rw-r--r--   0 dellaert   (502) staff       (20)     3426 2022-01-08 22:28:26.000000 gtbook-0.0.8/gtbook/discrete.py
--rw-r--r--   0 dellaert   (502) staff       (20)     1674 2022-01-08 22:28:26.000000 gtbook-0.0.8/gtbook/display.py
-drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-08 22:30:40.284605 gtbook-0.0.8/gtbook.egg-info/
--rw-r--r--   0 dellaert   (502) staff       (20)     1729 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/PKG-INFO
--rw-r--r--   0 dellaert   (502) staff       (20)      365 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/SOURCES.txt
--rw-r--r--   0 dellaert   (502) staff       (20)        1 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/dependency_links.txt
--rw-r--r--   0 dellaert   (502) staff       (20)      101 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/entry_points.txt
--rw-r--r--   0 dellaert   (502) staff       (20)        1 2022-01-08 21:45:40.000000 gtbook-0.0.8/gtbook.egg-info/not-zip-safe
--rw-r--r--   0 dellaert   (502) staff       (20)       51 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/requires.txt
--rw-r--r--   0 dellaert   (502) staff       (20)        7 2022-01-08 22:30:40.000000 gtbook-0.0.8/gtbook.egg-info/top_level.txt
--rw-r--r--   0 dellaert   (502) staff       (20)      754 2022-01-08 21:45:52.000000 gtbook-0.0.8/settings.ini
--rw-r--r--   0 dellaert   (502) staff       (20)       38 2022-01-08 22:30:40.285042 gtbook-0.0.8/setup.cfg
--rw-r--r--   0 dellaert   (502) staff       (20)     3094 2022-01-07 03:14:53.000000 gtbook-0.0.8/setup.py
+drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-10 00:49:22.227343 gtbook-0.0.9/
+-rw-r--r--   0 dellaert   (502) staff       (20)     2348 2022-01-07 03:14:53.000000 gtbook-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 dellaert   (502) staff       (20)    11357 2022-01-07 03:14:53.000000 gtbook-0.0.9/LICENSE
+-rw-r--r--   0 dellaert   (502) staff       (20)      111 2022-01-07 03:14:53.000000 gtbook-0.0.9/MANIFEST.in
+-rw-r--r--   0 dellaert   (502) staff       (20)     1729 2022-01-10 00:49:22.227138 gtbook-0.0.9/PKG-INFO
+-rw-r--r--   0 dellaert   (502) staff       (20)      980 2022-01-10 00:44:55.000000 gtbook-0.0.9/README.md
+drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-10 00:49:22.225227 gtbook-0.0.9/gtbook/
+-rw-r--r--   0 dellaert   (502) staff       (20)       22 2022-01-10 00:44:50.000000 gtbook-0.0.9/gtbook/__init__.py
+-rw-r--r--   0 dellaert   (502) staff       (20)      624 2022-01-10 00:44:50.000000 gtbook-0.0.9/gtbook/_nbdev.py
+-rw-r--r--   0 dellaert   (502) staff       (20)      904 2022-01-10 00:44:50.000000 gtbook-0.0.9/gtbook/cli.py
+-rw-r--r--   0 dellaert   (502) staff       (20)     3509 2022-01-10 00:44:50.000000 gtbook-0.0.9/gtbook/discrete.py
+-rw-r--r--   0 dellaert   (502) staff       (20)     2864 2022-01-10 00:44:50.000000 gtbook-0.0.9/gtbook/display.py
+drwxr-xr-x   0 dellaert   (502) staff       (20)        0 2022-01-10 00:49:22.226742 gtbook-0.0.9/gtbook.egg-info/
+-rw-r--r--   0 dellaert   (502) staff       (20)     1729 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/PKG-INFO
+-rw-r--r--   0 dellaert   (502) staff       (20)      365 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/SOURCES.txt
+-rw-r--r--   0 dellaert   (502) staff       (20)        1 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/dependency_links.txt
+-rw-r--r--   0 dellaert   (502) staff       (20)      101 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/entry_points.txt
+-rw-r--r--   0 dellaert   (502) staff       (20)        1 2022-01-08 21:45:40.000000 gtbook-0.0.9/gtbook.egg-info/not-zip-safe
+-rw-r--r--   0 dellaert   (502) staff       (20)       51 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/requires.txt
+-rw-r--r--   0 dellaert   (502) staff       (20)        7 2022-01-10 00:49:22.000000 gtbook-0.0.9/gtbook.egg-info/top_level.txt
+-rw-r--r--   0 dellaert   (502) staff       (20)      754 2022-01-09 22:20:07.000000 gtbook-0.0.9/settings.ini
+-rw-r--r--   0 dellaert   (502) staff       (20)       38 2022-01-10 00:49:22.227408 gtbook-0.0.9/setup.cfg
+-rw-r--r--   0 dellaert   (502) staff       (20)     3094 2022-01-07 03:14:53.000000 gtbook-0.0.9/setup.py
```

### Comparing `gtbook-0.0.8/CONTRIBUTING.md` & `gtbook-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gtbook-0.0.8/LICENSE` & `gtbook-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gtbook-0.0.8/PKG-INFO` & `gtbook-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtbook
-Version: 0.0.8
+Version: 0.0.9
 Summary: Frank Dellaerts book support lib, made with nbdev
 Home-page: https://github.com/gtbook/gtbook/tree/master/
 Author: Frank Dellaert
 Author-email: dellaert@gmail.com
 License: Apache Software License 2.0
 Keywords: python,nbdev
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gtbook Version: 0.0.8 Summary: Frank Dellaerts book
+Metadata-Version: 2.1 Name: gtbook Version: 0.0.9 Summary: Frank Dellaerts book
 support lib, made with nbdev Home-page: https://github.com/gtbook/gtbook/tree/
 master/ Author: Frank Dellaert Author-email: dellaert@gmail.com License: Apache
 Software License 2.0 Keywords: python,nbdev Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
```

### Comparing `gtbook-0.0.8/README.md` & `gtbook-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gtbook-0.0.8/gtbook/cli.py` & `gtbook-0.0.9/gtbook/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def rename(dir: str  # dir in which to rename files
            ):
     """Rename notebooks to base 1 for chapters."""
     path = Path(dir)
     assert path.exists(), f"dir '{dir}' not found"
     assert path.is_dir(), f"'{dir}' is not a directory"
     print("Renaming notebooks now.")
-    nbs = [x for x in path.iterdir() if x.suffix == '.ipynb']
     for ch in list(range(8, -1, -1)):
         print(f"Renaming chapter {ch}:")
         for x in path.glob(f"S{ch}*.ipynb"):
             new_name = path / x.name.replace(f"S{ch}", f"S{ch+1}")
             print(f"Renaming {x} to {new_name}")
             x.rename(new_name)
```

### Comparing `gtbook-0.0.8/gtbook/discrete.py` & `gtbook-0.0.9/gtbook/discrete.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,19 @@
 
         Args:
             assignment (gtsam.DiscreteValues): the values to render.
 
         Returns:
             str: a markdown string.
         """
-        converted = {self._variables[key][0]: self._variables[key][1][value] for (
-            key, value) in assignment.items()}
-        ss = "|Variable|value|\n|:-:|:-:|\n"
-        for key, value in assignment.items():
-            name, domain = self._variables[key]
-            ss += f"|{name}|{domain[value]}|\n"
-        return ss
+        return gtsam.markdown(assignment, self.keyFormatter(), self.names())
+
+    def values_html(self, assignment: gtsam.DiscreteValues) -> str:
+        """Render a DiscreteValues instance as html.
+
+        Args:
+            assignment (gtsam.DiscreteValues): the values to render.
+
+        Returns:
+            str: a html string.
+        """
+        return gtsam.html(assignment, self.keyFormatter(), self.names())
```

### Comparing `gtbook-0.0.8/gtbook.egg-info/PKG-INFO` & `gtbook-0.0.9/gtbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtbook
-Version: 0.0.8
+Version: 0.0.9
 Summary: Frank Dellaerts book support lib, made with nbdev
 Home-page: https://github.com/gtbook/gtbook/tree/master/
 Author: Frank Dellaert
 Author-email: dellaert@gmail.com
 License: Apache Software License 2.0
 Keywords: python,nbdev
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gtbook Version: 0.0.8 Summary: Frank Dellaerts book
+Metadata-Version: 2.1 Name: gtbook Version: 0.0.9 Summary: Frank Dellaerts book
 support lib, made with nbdev Home-page: https://github.com/gtbook/gtbook/tree/
 master/ Author: Frank Dellaert Author-email: dellaert@gmail.com License: Apache
 Software License 2.0 Keywords: python,nbdev Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
```

### Comparing `gtbook-0.0.8/settings.ini` & `gtbook-0.0.9/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 user = dellaert
 description = Frank Dellaerts book support lib, made with nbdev
 keywords = python, nbdev
 author = Frank Dellaert
 author_email = dellaert@gmail.com
 copyright = Frank Dellaert
 branch = master
-version = 0.0.8
+version = 0.0.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 conda_requirements = python-graphviz
-pip_requirements = fastcore>=1.3.27 gtsam==4.2a1
+pip_requirements = fastcore>=1.3.27 gtsam==4.2a2
 console_scripts = gtbook_rename=gtbook.cli:rename
 	gtbook_add_copyright=gtbook.cli:add_copyright
 nbs_path = .
 doc_path = docs
 recursive = False
 doc_host = https://gtbook.github.io/
 doc_baseurl = /gtbook/
```

### Comparing `gtbook-0.0.8/setup.py` & `gtbook-0.0.9/setup.py`

 * *Files identical despite different names*

