# Comparing `tmp/django_hierarchical_models-1.2.0.tar.gz` & `tmp/django_hierarchical_models-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hierarchical_models-1.2.0.tar", max compression
+gzip compressed data, was "django_hierarchical_models-2.0.0.tar", max compression
```

## Comparing `django_hierarchical_models-1.2.0.tar` & `django_hierarchical_models-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/LICENSE
--rw-r--r--   0        0        0     3627 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/README.md
--rw-r--r--   0        0        0       22 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/__init__.py
--rw-r--r--   0        0        0      499 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/__init__.py
--rw-r--r--   0        0        0     2028 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/alm.py
--rw-r--r--   0        0        0      754 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/exceptions.py
--rw-r--r--   0        0        0    14702 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/interface.py
--rw-r--r--   0        0        0     1104 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/node.py
--rw-r--r--   0        0        0    12977 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/nsm.py
--rw-r--r--   0        0        0     2958 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/django_hierarchical_models/models/pem.py
--rw-r--r--   0        0        0     1141 2024-04-26 23:00:57.580664 django_hierarchical_models-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 django_hierarchical_models-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4920 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/exceptions.py
+-rw-r--r--   0        0        0     6132 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/hierarchical_model.py
+-rw-r--r--   0        0        0      900 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/node.py
+-rw-r--r--   0        0        0     1116 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5712 1970-01-01 00:00:00.000000 django_hierarchical_models-2.0.0/PKG-INFO
```

### Comparing `django_hierarchical_models-1.2.0/LICENSE` & `django_hierarchical_models-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.2.0/pyproject.toml` & `django_hierarchical_models-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-hierarchical-models"
-version = "1.2.0"
+version = "2.0.0"
 description = "Adds hierarchical models to Django"
 authors = ["Josh Bedwell <rcxwhiz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rcxwhiz/django-hierarchical-models"
 packages = [{include = "django_hierarchical_models"}]
 classifiers = [
@@ -24,15 +24,14 @@
 flake8 = "^7.0.0"
 pytest = "^8.1.1"
 pytest-django = "^4.8.0"
 isort = "^5.13.2"
 psycopg2-binary = "^2.9.9"
 mypy = "^1.9.0"
 django-stubs = "^4.2.7"
-parameterized = "^0.9.0"
 pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

