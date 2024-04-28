# Comparing `tmp/pyams_sequence-2.0.1.tar.gz` & `tmp/pyams_sequence-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_sequence-2.0.1.tar", last modified: Thu Feb  1 17:43:52 2024, max compression
+gzip compressed data, was "dist/pyams_sequence-2.1.0.tar", last modified: Sun Apr 28 15:21:01 2024, max compression
```

## Comparing `pyams_sequence-2.0.1.tar` & `pyams_sequence-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3067 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1150 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2657 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/api/
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4143 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10379 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/include.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
--rw-rw-rw-   0 root         (0) root         (0)     4850 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/locales/pyams_sequence.pot
--rw-rw-rw-   0 root         (0) root         (0)     4674 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/sequence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     6172 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/widget/
--rw-rw-rw-   0 root         (0) root         (0)     3925 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2134 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-02-01 17:43:25.000000 pyams_sequence-2.0.1/src/pyams_sequence/zmi/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3067 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:43:46.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-01 17:43:52.000000 pyams_sequence-2.0.1/src/pyams_sequence.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3175 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1258 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    11125 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/locales/pyams_sequence.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4674 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/sequence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6369 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2024-04-28 15:14:15.000000 pyams_sequence-2.1.0/src/pyams_sequence/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-02-01 17:49:22.000000 pyams_sequence-2.1.0/src/pyams_sequence/zmi/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3175 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:20:53.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-28 15:21:01.000000 pyams_sequence-2.1.0/src/pyams_sequence.egg-info/top_level.txt
```

### Comparing `pyams_sequence-2.0.1/LICENSE` & `pyams_sequence-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/PKG-INFO` & `pyams_sequence-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_sequence
-Version: 2.0.1
+Version: 2.1.0
 Summary: PyAMS sequences management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -51,14 +51,18 @@
 Custom schemas fields and forms widgets are available to select internal references into
 content management interface.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added optional arguments to references finder to check parent and disable params validation
+
 2.0.1
 -----
  - updated workflow transition handler to avoid references from broken objects
  - updated REST API route name and configuration setting name
  - added sortable class to internal references input widget
  - updated Buildout configuration
```

### Comparing `pyams_sequence-2.0.1/docs/HISTORY.rst` & `pyams_sequence-2.1.0/docs/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.1.0
+-----
+ - added optional arguments to references finder to check parent and disable params validation
+
 2.0.1
 -----
  - updated workflow transition handler to avoid references from broken objects
  - updated REST API route name and configuration setting name
  - added sortable class to internal references input widget
  - updated Buildout configuration
```

### Comparing `pyams_sequence-2.0.1/docs/README.rst` & `pyams_sequence-2.1.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/setup.py` & `pyams_sequence-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.0.1'
+version = '2.1.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/api/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,18 @@
 
 __docformat__ = 'restructuredtext'
 
 
 @view_config(name='find-references.json',
              permission=USE_INTERNAL_API_PERMISSION,
              renderer='json', xhr=True)
-def find_references(request):
+def find_references(request, parent=None):
     """Find all references matching given query"""
     query = request.params.get('term')
     if not query:
         return []
     sequence = get_utility(ISequentialIntIds)
     return sorted([
         get_sequence_dict(result)
-        for result in sequence.find_references(query,
-                                               request.params.get('content_type'),
-                                               request)
+        for result in sequence.find_references(query, request.params.get('content_type'),
+                                               request, parent)
     ], key=lambda x: x['text'])
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/api/rest.py` & `pyams_sequence-2.1.0/src/pyams_sequence/api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,26 +91,26 @@
     description="References search results")
 
 
 @references_service.get(permission=USE_INTERNAL_API_PERMISSION,
                         schema=ReferencesGetRequest(),
                         validators=(check_cors_origin, colander_validator, set_cors_headers),
                         response_schemas=references_get_responses)
-def find_references(request):
+def find_references(request, parent=None, validate=True):
     """Returns list of references matching given query"""
-    params = request.params if TEST_MODE else request.validated.get('querystring', {})
+    params = request.params if (TEST_MODE or not validate) else request.validated.get('querystring', {})
     query = params.get('term')
     if not query:
         return {
             'status': STATUS.ERROR.value,
             'message': 'Missing arguments',
             'results': []
         }
     content_type = params.get('content_type')
     sequence = query_utility(ISequentialIntIds)
     return {
         'status': STATUS.SUCCESS.value,
         'results': sorted([
             get_sequence_dict(result)
-            for result in sequence.find_references(query, content_type, request)
+            for result in sequence.find_references(query, content_type, request, parent)
         ], key=lambda x: x['text'])
     }
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/doctests/README.rst` & `pyams_sequence-2.1.0/src/pyams_sequence/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,30 @@
             <option></option>
     </select>
     <input name="form.widgets.reference-empty-marker" type="hidden" value="1" />
 
 Select options list is actually empty in this test because we don't have a testing catalog
 with "content_type" name!
 
+You can set widget target URL, for example from an "update_widgets" form method:
+
+    >>> form.widgets['reference'].ajax_url = '/context/get-references.json'
+    >>> print(form.widgets['reference'].render())
+    <select id="form-widgets-reference"
+            name="form.widgets.reference"
+            class="form-control select2 select-widget required internalreferencefield-field"
+            size="1"
+            data-placeholder="No selected reference"
+            data-ajax--url="/context/get-references.json"
+            data-ajax--params='{"content_type": "MyContent"}'
+            data-minimum-input-length="2">
+            <option></option>
+    </select>
+    <input name="form.widgets.reference-empty-marker" type="hidden" value="1" />
+
 
 Workflow related functions
 --------------------------
 
 Sequences have been designed with workflow in mind. But workflow related functions should
 return correct results even when working with contents which are not managed by a workflow:
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/generations/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/include.py` & `pyams_sequence-2.1.0/src/pyams_sequence/include.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/interfaces.py` & `pyams_sequence-2.1.0/src/pyams_sequence/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def get_internal_id(self, oid):
         """Get internal ID matching given OID"""
 
     def query_object_from_oid(self, oid):
         """Query object with given OID"""
 
-    def find_references(self, query, content_type=None, request=None):
+    def find_references(self, query, content_type=None, request=None, parent=None):
         """Find references matching given query"""
 
 
 class ISequentialIdInfo(Interface):
     """Sequential ID info interface"""
 
     oid = Int(title=_("Sequential ID"),
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo` & `pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po` & `pyams_sequence-2.1.0/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/locales/pyams_sequence.pot` & `pyams_sequence-2.1.0/src/pyams_sequence/locales/pyams_sequence.pot`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/reference.py` & `pyams_sequence-2.1.0/src/pyams_sequence/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/schema.py` & `pyams_sequence-2.1.0/src/pyams_sequence/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/sequence.py` & `pyams_sequence-2.1.0/src/pyams_sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/tests/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/tests/test_utilsdocs.py` & `pyams_sequence-2.1.0/src/pyams_sequence/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/tests/test_utilsdocstrings.py` & `pyams_sequence-2.1.0/src/pyams_sequence/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/utility.py` & `pyams_sequence-2.1.0/src/pyams_sequence/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 """
 
 from hypatia.catalog import CatalogQuery
 from hypatia.interfaces import ICatalog
 from hypatia.query import Contains, Eq
 from zope.interface import Invalid
 from zope.intid import IntIds
+from zope.intid.interfaces import IIntIds
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_catalog.query import CatalogResultSet
 from pyams_i18n.interfaces import INegotiator
 from pyams_sequence.interfaces import ISequentialIdTarget, ISequentialIntIds
 from pyams_sequence.workflow import get_last_version
 from pyams_utils.adapter import ContextAdapter, adapter_config
 from pyams_utils.factory import factory_config
-
-
-__docformat__ = 'restructuredtext'
-
-from pyams_sequence import _  # pylint: disable=ungrouped-imports
 from pyams_utils.interfaces.intids import IIndexLength
 from pyams_utils.list import unique
 from pyams_utils.registry import get_utility
 from pyams_utils.request import check_request
 
+__docformat__ = 'restructuredtext'
+
+from pyams_sequence import _  # pylint: disable=ungrouped-imports
+
 
 @factory_config(ISequentialIntIds)
 class SequentialIntIds(IntIds):
     """Sequential IntIds utility"""
 
     prefix = FieldProperty(ISequentialIntIds['prefix'])
     hex_oid_length = FieldProperty(ISequentialIntIds['hex_oid_length'])
@@ -118,15 +118,15 @@
         return int(oid, 16)
 
     def query_object_from_oid(self, oid):
         """Query object matching given OID"""
         internal_id = self.get_internal_id(oid)
         return self.queryObject(internal_id)
 
-    def find_references(self, query, content_type=None, request=None):
+    def find_references(self, query, content_type=None, request=None, parent=None):
         """Find internal references matching given query"""
         if not query:
             return
         if request is None:
             request = check_request()
         catalog = get_utility(ICatalog)
         if query.startswith('+'):
@@ -144,14 +144,17 @@
                     index = catalog[index_name]
                     if index.check_query(query):
                         query_params |= Contains(index,
                                                  ' and '.join((w + '*' for w in query.split())))
             params = query_params
         if content_type:
             params &= Eq(catalog['content_type'], content_type)
+        if parent is not None:
+            intids = get_utility(IIntIds)
+            params &= Eq(catalog['parents'], intids.register(parent))
         yield from unique(filter(lambda x: x is not None,
                                  map(get_last_version,
                                      CatalogResultSet(CatalogQuery(catalog).query(params)))))
 
 
 @adapter_config(required=ISequentialIntIds,
                 provides=IIndexLength)
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/widget/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/widget/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,21 +65,27 @@
         return super().to_widget_value(value)
 
 
 @implementer_only(IInternalReferenceWidget)
 class InternalReferenceWidget(SelectWidget):
     """Internal reference widget"""
 
+    _ajax_url = None
     placeholder = _("No selected reference")
 
     @property
     def ajax_url(self):
         """AJAX URL getter"""
-        return self.request.registry.settings.get(f'{REST_REFERENCES_SEARCH_ROUTE}_route.path',
-                                                  REST_REFERENCES_SEARCH_PATH)
+        return self._ajax_url or self.request.registry.settings.get(f'{REST_REFERENCES_SEARCH_ROUTE}_route.path',
+                                                                    REST_REFERENCES_SEARCH_PATH)
+
+    @ajax_url.setter
+    def ajax_url(self, value):
+        """AJAX URL setter"""
+        self._ajax_url = value
 
     @property
     def ajax_params(self):
         """AJAX params getter"""
         if self.field.content_type:
             return json.dumps({'content_type': self.field.content_type})
         return None
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/workflow.py` & `pyams_sequence-2.1.0/src/pyams_sequence/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/zmi/__init__.py` & `pyams_sequence-2.1.0/src/pyams_sequence/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence/zmi/reference.py` & `pyams_sequence-2.1.0/src/pyams_sequence/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence.egg-info/PKG-INFO` & `pyams_sequence-2.1.0/src/pyams_sequence.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-sequence
-Version: 2.0.1
+Version: 2.1.0
 Summary: PyAMS sequences management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -51,14 +51,18 @@
 Custom schemas fields and forms widgets are available to select internal references into
 content management interface.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added optional arguments to references finder to check parent and disable params validation
+
 2.0.1
 -----
  - updated workflow transition handler to avoid references from broken objects
  - updated REST API route name and configuration setting name
  - added sortable class to internal references input widget
  - updated Buildout configuration
```

### Comparing `pyams_sequence-2.0.1/src/pyams_sequence.egg-info/SOURCES.txt` & `pyams_sequence-2.1.0/src/pyams_sequence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

