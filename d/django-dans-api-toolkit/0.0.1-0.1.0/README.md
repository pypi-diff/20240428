# Comparing `tmp/django-dans-api-toolkit-0.0.1.tar.gz` & `tmp/django-dans-api-toolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dans-api-toolkit-0.0.1.tar", last modified: Thu Apr 25 03:36:17 2024, max compression
+gzip compressed data, was "django-dans-api-toolkit-0.1.0.tar", last modified: Sun Apr 28 19:03:25 2024, max compression
```

## Comparing `django-dans-api-toolkit-0.0.1.tar` & `django-dans-api-toolkit-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/test/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 03:36:17.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 03:36:17.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:36:17.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 03:36:17.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 03:36:17.000000 django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/docs/release.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-25 03:36:17.586431 django-dans-api-toolkit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 03:36:08.000000 django-dans-api-toolkit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:25.657694 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/api_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/api_response_renderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/test/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:03:25.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-28 19:03:25.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:03:25.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:03:25.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:03:25.000000 django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/docs/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-28 19:03:25.661694 django-dans-api-toolkit-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:03:16.000000 django-dans-api-toolkit-0.1.0/setup.py
```

### Comparing `django-dans-api-toolkit-0.0.1/LICENSE` & `django-dans-api-toolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.0.1/PKG-INFO` & `django-dans-api-toolkit-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -77,14 +77,22 @@
     "PAGE_SIZE": 20,
     "DEFAULT_AUTHENTICATION_CLASSES": (
         "rest_framework.authentication.TokenAuthentication",
     ),
 }
 ```
 
+## Features
+
+This app is meant to be a collection of tools to help with common API tasks, and is not meant to be a full-fledged API solution. It is meant to be used in conjunction with Django Rest Framework, and is not a replacement for it.
+
+Some of the features include:
+- API response handler - `api_response_handler.py`
+- API response renderer - `api_response_renderer.py`
+- Base serializer - `serializers/base.py`
 
 -------------------------------------------------------
 
 ##### [https://danielnazarian.com](https://danielnazarian.com)
 
 ##### Copyright 2024 © Daniel Nazarian.
```

### Comparing `django-dans-api-toolkit-0.0.1/README.md` & `django-dans-api-toolkit-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -45,14 +45,22 @@
     "PAGE_SIZE": 20,
     "DEFAULT_AUTHENTICATION_CLASSES": (
         "rest_framework.authentication.TokenAuthentication",
     ),
 }
 ```
 
+## Features
+
+This app is meant to be a collection of tools to help with common API tasks, and is not meant to be a full-fledged API solution. It is meant to be used in conjunction with Django Rest Framework, and is not a replacement for it.
+
+Some of the features include:
+- API response handler - `api_response_handler.py`
+- API response renderer - `api_response_renderer.py`
+- Base serializer - `serializers/base.py`
 
 -------------------------------------------------------
 
 ##### [https://danielnazarian.com](https://danielnazarian.com)
 
 ##### Copyright 2024 © Daniel Nazarian.
```

### Comparing `django-dans-api-toolkit-0.0.1/django_dans_api_toolkit/test/settings.py` & `django-dans-api-toolkit-0.1.0/django_dans_api_toolkit/test/settings.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.0.1/django_dans_api_toolkit.egg-info/PKG-INFO` & `django-dans-api-toolkit-0.1.0/django_dans_api_toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -77,14 +77,22 @@
     "PAGE_SIZE": 20,
     "DEFAULT_AUTHENTICATION_CLASSES": (
         "rest_framework.authentication.TokenAuthentication",
     ),
 }
 ```
 
+## Features
+
+This app is meant to be a collection of tools to help with common API tasks, and is not meant to be a full-fledged API solution. It is meant to be used in conjunction with Django Rest Framework, and is not a replacement for it.
+
+Some of the features include:
+- API response handler - `api_response_handler.py`
+- API response renderer - `api_response_renderer.py`
+- Base serializer - `serializers/base.py`
 
 -------------------------------------------------------
 
 ##### [https://danielnazarian.com](https://danielnazarian.com)
 
 ##### Copyright 2024 © Daniel Nazarian.
```

### Comparing `django-dans-api-toolkit-0.0.1/docs/release.md` & `django-dans-api-toolkit-0.1.0/docs/release.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.0.1/setup.cfg` & `django-dans-api-toolkit-0.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dans-api-toolkit
-version = 0.0.1
+version = 0.1.0
 description = A Django app to help make building APIs great.
 long_description = file: README.md
 url = https://www.github.com/dan1229/django_dans_api_toolkit
 author = Daniel Nazarian
 author_email = dnaz@danielnazarian.com
 license = BSD-3-Clause
 classifiers =
```

