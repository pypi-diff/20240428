# Comparing `tmp/django-dans-api-toolkit-0.1.8.tar.gz` & `tmp/django-dans-api-toolkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dans-api-toolkit-0.1.8.tar", last modified: Sun Apr 28 20:15:03 2024, max compression
+gzip compressed data, was "django-dans-api-toolkit-0.1.9.tar", last modified: Sun Apr 28 20:16:54 2024, max compression
```

## Comparing `django-dans-api-toolkit-0.1.8.tar` & `django-dans-api-toolkit-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response_renderer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/serializers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/test/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:15:03.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 20:15:03.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:15:03.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 20:15:03.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 20:15:03.000000 django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/docs/release.md
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/docs/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-28 20:15:03.777112 django-dans-api-toolkit-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 20:14:53.000000 django-dans-api-toolkit-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.825891 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response_renderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/serializers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/test/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:16:54.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 20:16:54.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:16:54.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 20:16:54.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 20:16:54.000000 django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/docs/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-28 20:16:54.829891 django-dans-api-toolkit-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 20:16:44.000000 django-dans-api-toolkit-0.1.9/setup.py
```

### Comparing `django-dans-api-toolkit-0.1.8/LICENSE` & `django-dans-api-toolkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/PKG-INFO` & `django-dans-api-toolkit-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.8/README.md` & `django-dans-api-toolkit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response.py` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response_handler.py` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response_handler.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/api_response_renderer.py` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/api_response_renderer.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/serializers/base.py` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/serializers/base.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit/test/settings.py` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit/test/settings.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/PKG-INFO` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.8/django_dans_api_toolkit.egg-info/SOURCES.txt` & `django-dans-api-toolkit-0.1.9/django_dans_api_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/docs/release.md` & `django-dans-api-toolkit-0.1.9/docs/release.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/docs/tools.md` & `django-dans-api-toolkit-0.1.9/docs/tools.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.8/setup.cfg` & `django-dans-api-toolkit-0.1.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dans-api-toolkit
-version = 0.1.8
+version = 0.1.9
 description = A Django app to help make building APIs great.
 long_description = file: README.md
 url = https://www.github.com/dan1229/django_dans_api_toolkit
 author = Daniel Nazarian
 author_email = dnaz@danielnazarian.com
 license = BSD-3-Clause
 classifiers = 
@@ -33,14 +33,14 @@
 python_requires = >=3.8
 install_requires = 
 	Django >= 3.1
 	djangorestframework >= 3.12
 	coverage >= 6.4
 
 [options.package_data]
-django_dans_api_toolkit = *.pyi
+django_dans_api_toolkit = *.pyi, py.typed
 django_dans_api_toolkit.serializers = *.pyi
 
 [egg_info]
 tag_build = 
 tag_date = 0
```
