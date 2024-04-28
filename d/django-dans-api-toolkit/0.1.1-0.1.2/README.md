# Comparing `tmp/django-dans-api-toolkit-0.1.1.tar.gz` & `tmp/django-dans-api-toolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dans-api-toolkit-0.1.1.tar", last modified: Sun Apr 28 19:11:30 2024, max compression
+gzip compressed data, was "django-dans-api-toolkit-0.1.2.tar", last modified: Sun Apr 28 19:14:42 2024, max compression
```

## Comparing `django-dans-api-toolkit-0.1.1.tar` & `django-dans-api-toolkit-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:30.432720 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response_renderer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/test/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:11:30.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-28 19:11:30.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:11:30.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:11:30.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:11:30.000000 django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/docs/release.md
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/docs/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-28 19:11:30.436720 django-dans-api-toolkit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:11:22.000000 django-dans-api-toolkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_renderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2497 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/docs/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/setup.py
```

### Comparing `django-dans-api-toolkit-0.1.1/LICENSE` & `django-dans-api-toolkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/PKG-INFO` & `django-dans-api-toolkit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.1/README.md` & `django-dans-api-toolkit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response.py` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response_handler.py` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_handler.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/api_response_renderer.py` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_renderer.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit/test/settings.py` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/settings.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/PKG-INFO` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.1/django_dans_api_toolkit.egg-info/SOURCES.txt` & `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,13 @@
 django_dans_api_toolkit/api_response_renderer.py
 django_dans_api_toolkit/apps.py
 django_dans_api_toolkit.egg-info/PKG-INFO
 django_dans_api_toolkit.egg-info/SOURCES.txt
 django_dans_api_toolkit.egg-info/dependency_links.txt
 django_dans_api_toolkit.egg-info/requires.txt
 django_dans_api_toolkit.egg-info/top_level.txt
+django_dans_api_toolkit/serializers/__init__.py
+django_dans_api_toolkit/serializers/base.py
 django_dans_api_toolkit/test/__init__.py
 django_dans_api_toolkit/test/settings.py
 docs/release.md
 docs/tools.md
```

### Comparing `django-dans-api-toolkit-0.1.1/docs/release.md` & `django-dans-api-toolkit-0.1.2/docs/release.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/docs/tools.md` & `django-dans-api-toolkit-0.1.2/docs/tools.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.1/setup.cfg` & `django-dans-api-toolkit-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dans-api-toolkit
-version = 0.1.1
+version = 0.1.2
 description = A Django app to help make building APIs great.
 long_description = file: README.md
 url = https://www.github.com/dan1229/django_dans_api_toolkit
 author = Daniel Nazarian
 author_email = dnaz@danielnazarian.com
 license = BSD-3-Clause
 classifiers =
```

