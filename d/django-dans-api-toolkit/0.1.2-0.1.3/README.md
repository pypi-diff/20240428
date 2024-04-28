# Comparing `tmp/django-dans-api-toolkit-0.1.2.tar.gz` & `tmp/django-dans-api-toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dans-api-toolkit-0.1.2.tar", last modified: Sun Apr 28 19:14:42 2024, max compression
+gzip compressed data, was "django-dans-api-toolkit-0.1.3.tar", last modified: Sun Apr 28 19:31:58 2024, max compression
```

## Comparing `django-dans-api-toolkit-0.1.2.tar` & `django-dans-api-toolkit-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_renderer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2497 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:14:42.000000 django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/docs/release.md
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/docs/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-28 19:14:42.646867 django-dans-api-toolkit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:14:33.000000 django-dans-api-toolkit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response_renderer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/serializers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2522 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/test/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 19:31:58.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-28 19:31:58.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:31:58.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 19:31:58.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 19:31:58.000000 django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/docs/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-28 19:31:58.431069 django-dans-api-toolkit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 19:31:49.000000 django-dans-api-toolkit-0.1.3/setup.py
```

### Comparing `django-dans-api-toolkit-0.1.2/LICENSE` & `django-dans-api-toolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/PKG-INFO` & `django-dans-api-toolkit-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.2/README.md` & `django-dans-api-toolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response.py` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_handler.py` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response_handler.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/api_response_renderer.py` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/api_response_renderer.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/serializers/base.py` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/serializers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any, List
+from typing import Any, Dict, List, Optional
 from rest_framework import serializers
 
 """
 # ===================================================================================
 # BASE SERIALIZER ===================================================================
 # ===================================================================================
 """
 
 
-class BaseSerializer(serializers.ModelSerializer):  # type: ignore[type-arg]
+class BaseSerializer(serializers.ModelSerializer):
     """
     BaseSerializer to inherit from
 
     :param bool masked:             If True, will mask the serializer.
                                     Based on `masked_fields` property. Fields in `masked_fields` will only
                                     show up if `masked` is False
     :param bool ref_serializer:     If True, will return a reference serializer.
@@ -20,41 +20,40 @@
                                     up if `ref_serializer` is False. If `ref_fields` is not provided,
                                     all fields will be returned.
     :param str[] fields:            Additional kwargs 'field' that controls which fields to include
     """
 
     ref_fields: List[str] = []
     masked_fields: List[str] = []
-    masked = True
-    ref_serializer = False
+    masked: bool = True
+    ref_serializer: bool = False
+    fields: Dict[str, serializers.Field]
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-        # save kwargs for later
-        self.kwargs = kwargs
+        self.kwargs = kwargs  # Save kwargs for later
 
         # handle 'fields' keyword argument
-        # Don't pass the 'fields' arg up to the superclass
-        fields = kwargs.pop("fields", None)
+        fields: Optional[List[str]] = kwargs.pop("fields", None)
 
         # if masked serializer, remove masked fields
         self.masked = kwargs.pop("masked", self.masked)
-        masked_fields = getattr(self.Meta, "masked_fields", [])
+        masked_fields = getattr(self.Meta, "masked_fields", self.masked_fields)
         if self.masked:
             for field in masked_fields:
-                self.fields.pop(field)
+                self.fields.pop(field, None)
 
         # if ref serializer, remove ref fields
         self.ref_serializer = kwargs.pop("ref_serializer", self.ref_serializer)
-        ref_fields = getattr(self.Meta, "ref_fields", [])
+        ref_fields = getattr(self.Meta, "ref_fields", self.ref_fields)
         if self.ref_serializer:
             for field in ref_fields:
-                self.fields.pop(field)
+                self.fields.pop(field, None)
 
         # Instantiate the superclass normally
-        super(BaseSerializer, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-        # Drop any fields that are not specified in the `fields` argument.
+        # Drop any fields that are not specified in the `fields` argument
         if fields is not None:
             allowed = set(fields)
-            existing = set(self.fields)
+            existing = set(self.fields.keys())
             for field_name in existing - allowed:
                 self.fields.pop(field_name)
```

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit/test/settings.py` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit/test/settings.py`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/PKG-INFO` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dans-api-toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app to help make building APIs great.
 Home-page: https://www.github.com/dan1229/django_dans_api_toolkit
 Author: Daniel Nazarian
 Author-email: dnaz@danielnazarian.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-dans-api-toolkit-0.1.2/django_dans_api_toolkit.egg-info/SOURCES.txt` & `django-dans-api-toolkit-0.1.3/django_dans_api_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/docs/release.md` & `django-dans-api-toolkit-0.1.3/docs/release.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/docs/tools.md` & `django-dans-api-toolkit-0.1.3/docs/tools.md`

 * *Files identical despite different names*

### Comparing `django-dans-api-toolkit-0.1.2/setup.cfg` & `django-dans-api-toolkit-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dans-api-toolkit
-version = 0.1.2
+version = 0.1.3
 description = A Django app to help make building APIs great.
 long_description = file: README.md
 url = https://www.github.com/dan1229/django_dans_api_toolkit
 author = Daniel Nazarian
 author_email = dnaz@danielnazarian.com
 license = BSD-3-Clause
 classifiers =
```

