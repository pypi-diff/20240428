# Comparing `tmp/django-dans-api-toolkit-0.1.5.tar.gz` & `tmp/django-dans-api-toolkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dans-api-toolkit-0.1.5.tar", last modified: Sun Apr 28 19:41:50 2024, max compression
+gzip compressed data, was "django-dans-api-toolkit-0.1.7.tar", last modified: Sun Apr 28 19:47:42 2024, max compression
```

## Comparing `django-dans-api-toolkit-0.1.5.tar` & `django-dans-api-toolkit-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.480798 django-dans-api-toolkit-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:41:50.480798 django-dans-api-toolkit-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.476798 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response_renderer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.476798 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/serializers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.480798 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/test/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.476798 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:41:50.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 19:41:50.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:41:50.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:41:50.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:41:50.000000 django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:41:50.480798 django-dans-api-toolkit-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/docs/release.md
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/docs/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-28 19:41:50.480798 django-dans-api-toolkit-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:41:42.000000 django-dans-api-toolkit-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response_renderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/serializers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/test/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:47:42.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 19:47:42.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:47:42.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:47:42.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:47:42.000000 django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/docs/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-28 19:47:42.827096 django-dans-api-toolkit-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:47:33.000000 django-dans-api-toolkit-0.1.7/setup.py
```

### Comparing `django-dans-api-toolkit-0.1.5/LICENSE` & `django-dans-api-toolkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/PKG-INFO` & `django-dans-api-toolkit-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.5
+Version: 0.1.7
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.5/README.md` & `django-dans-api-toolkit-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response.py` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response_handler.py` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response_handler.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/api_response_renderer.py` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/api_response_renderer.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/serializers/base.py` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/serializers/base.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit/test/settings.py` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit/test/settings.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/PKG-INFO` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.5
+Version: 0.1.7
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.5/django_dans_api_toolkit.egg-info/SOURCES.txt` & `django-dans-api-toolkit-0.1.7/django_dans_api_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/docs/release.md` & `django-dans-api-toolkit-0.1.7/docs/release.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/docs/tools.md` & `django-dans-api-toolkit-0.1.7/docs/tools.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.5/setup.cfg` & `django-dans-api-toolkit-0.1.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dans-api-toolkit
-version = 0.1.5
+version = 0.1.7
 description = A Django app to help make building APIs great.
 long_description = file: README.md
 url = https://www.github.com/dan1229/django_dans_api_toolkit
 author = Daniel Nazarian
 author_email = dnaz@danielnazarian.com
 license = BSD-3-Clause
 classifiers = 
@@ -31,14 +31,16 @@
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	Django >= 3.1
 	djangorestframework >= 3.12
 	coverage >= 6.4
+
+[options.package_data]
 django_dans_api_toolkit = *.pyi
 django_dans_api_toolkit.serializers = *.pyi
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

