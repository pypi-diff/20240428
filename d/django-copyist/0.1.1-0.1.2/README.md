# Comparing `tmp/django_copyist-0.1.1.tar.gz` & `tmp/django_copyist-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_copyist-0.1.1.tar", max compression
+gzip compressed data, was "django_copyist-0.1.2.tar", max compression
```

## Comparing `django_copyist-0.1.1.tar` & `django_copyist-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11342 2024-04-27 10:29:34.355724 django_copyist-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0    12100 2024-04-28 08:53:23.336200 django_copyist-0.1.1/README.rst
--rw-r--r--   0        0        0        0 2024-04-24 19:00:14.434540 django_copyist-0.1.1/django_copyist/__init__.py
--rw-r--r--   0        0        0    20047 2024-04-28 09:06:41.939500 django_copyist-0.1.1/django_copyist/config.py
--rw-r--r--   0        0        0     4178 2024-04-28 09:01:02.827118 django_copyist-0.1.1/django_copyist/copy_request.py
--rw-r--r--   0        0        0    48952 2024-04-28 09:07:17.131379 django_copyist-0.1.1/django_copyist/copyist.py
--rw-r--r--   0        0        0      567 2024-04-28 10:01:15.035548 django_copyist-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12566 1970-01-01 00:00:00.000000 django_copyist-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-04-28 10:41:38.262925 django_copyist-0.1.2/CHANGELOG.rst
+-rw-r--r--   0        0        0    11342 2024-04-28 10:41:38.262925 django_copyist-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0    12100 2024-04-28 10:41:38.262925 django_copyist-0.1.2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-28 10:41:38.262925 django_copyist-0.1.2/django_copyist/__init__.py
+-rw-r--r--   0        0        0    20047 2024-04-28 10:41:38.262925 django_copyist-0.1.2/django_copyist/config.py
+-rw-r--r--   0        0        0     4178 2024-04-28 10:41:38.262925 django_copyist-0.1.2/django_copyist/copy_request.py
+-rw-r--r--   0        0        0    48952 2024-04-28 10:41:38.262925 django_copyist-0.1.2/django_copyist/copyist.py
+-rw-r--r--   0        0        0      894 2024-04-28 10:41:38.266925 django_copyist-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12794 1970-01-01 00:00:00.000000 django_copyist-0.1.2/PKG-INFO
```

### Comparing `django_copyist-0.1.1/LICENSE.txt` & `django_copyist-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_copyist-0.1.1/README.rst` & `django_copyist-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_copyist-0.1.1/django_copyist/config.py` & `django_copyist-0.1.2/django_copyist/config.py`

 * *Files identical despite different names*

### Comparing `django_copyist-0.1.1/django_copyist/copy_request.py` & `django_copyist-0.1.2/django_copyist/copy_request.py`

 * *Files identical despite different names*

### Comparing `django_copyist-0.1.1/django_copyist/copyist.py` & `django_copyist-0.1.2/django_copyist/copyist.py`

 * *Files identical despite different names*

### Comparing `django_copyist-0.1.1/pyproject.toml` & `django_copyist-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 [tool.poetry]
 name = "django-copyist"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tool for precise and efficient django model copying"
 authors = ["abondar"]
 license = "Apache-2.0"
 readme = "README.rst"
+homepage = "https://github.com/abondar/django-copyist"
+repository = "https://github.com/abondar/django-copyist.git"
+documentation = "https://abondar.github.io/django-copyist/"
+keywords = ["django", "copy", "clone", "model"]
+packages = [
+    { include = "django_copyist" }
+]
+include = ["CHANGELOG.rst", "LICENSE", "README.rst"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 Django = ">=3.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
```

### Comparing `django_copyist-0.1.1/PKG-INFO` & `django_copyist-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: django-copyist
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool for precise and efficient django model copying
+Home-page: https://github.com/abondar/django-copyist
 License: Apache-2.0
+Keywords: django,copy,clone,model
 Author: abondar
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
+Project-URL: Documentation, https://abondar.github.io/django-copyist/
+Project-URL: Repository, https://github.com/abondar/django-copyist.git
 Description-Content-Type: text/x-rst
 
 django-copyist
 ==========================================
 
 Tool for precise and efficient copying of Django models instances.
```

