# Comparing `tmp/untanglepyut-2.1.7.tar.gz` & `tmp/untanglepyut-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untanglepyut-2.1.7.tar", last modified: Sun Mar 10 18:20:26 2024, max compression
+gzip compressed data, was "untanglepyut-2.1.8.tar", last modified: Sun Apr 28 20:25:03 2024, max compression
```

## Comparing `untanglepyut-2.1.7.tar` & `untanglepyut-2.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-10 18:20:26.391471 untanglepyut-2.1.7/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-2.1.7/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3776 2024-03-10 18:20:26.391271 untanglepyut-2.1.7/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3156 2023-10-04 16:52:55.000000 untanglepyut-2.1.7/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      910 2024-03-10 18:08:17.000000 untanglepyut-2.1.7/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-03-10 18:20:26.391517 untanglepyut-2.1.7/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-10 18:20:26.387462 untanglepyut-2.1.7/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-10 18:20:26.390411 untanglepyut-2.1.7/src/untanglepyut/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/BaseUnTangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5655 2024-01-14 22:38:56.000000 untanglepyut-2.1.7/src/untanglepyut/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1535 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleIO.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2154 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleOglClasses.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    16792 2024-01-14 22:05:49.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleOglLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2066 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleOglNotes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2313 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleOglTexts.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2308 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleProjectInformation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21218 2024-02-05 18:30:46.000000 untanglepyut-2.1.7/src/untanglepyut/UnTanglePyut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4574 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4647 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangleUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8020 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnTangler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/UnsupportedFileTypeException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3647 2024-01-15 02:11:32.000000 untanglepyut-2.1.7/src/untanglepyut/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       80 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/XmlVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-03-10 17:21:29.000000 untanglepyut-2.1.7/src/untanglepyut/_version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:30:45.000000 untanglepyut-2.1.7/src/untanglepyut/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-10 18:20:26.391076 untanglepyut-2.1.7/src/untanglepyut.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3776 2024-03-10 18:20:26.000000 untanglepyut-2.1.7/src/untanglepyut.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      865 2024-03-10 18:20:26.000000 untanglepyut-2.1.7/src/untanglepyut.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-03-10 18:20:26.000000 untanglepyut-2.1.7/src/untanglepyut.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       92 2024-03-10 18:20:26.000000 untanglepyut-2.1.7/src/untanglepyut.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2024-03-10 18:20:26.000000 untanglepyut-2.1.7/src/untanglepyut.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 20:25:03.715430 untanglepyut-2.1.8/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-2.1.8/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3776 2024-04-28 20:25:03.715257 untanglepyut-2.1.8/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3156 2023-10-04 16:52:55.000000 untanglepyut-2.1.8/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      910 2024-04-28 19:15:24.000000 untanglepyut-2.1.8/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-04-28 20:25:03.715468 untanglepyut-2.1.8/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 20:25:03.709142 untanglepyut-2.1.8/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 20:25:03.714382 untanglepyut-2.1.8/src/untanglepyut/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/BaseUnTangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5655 2024-01-14 22:38:56.000000 untanglepyut-2.1.8/src/untanglepyut/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1535 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleIO.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2154 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleOglClasses.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    16792 2024-01-14 22:05:49.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleOglLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2066 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleOglNotes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2313 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleOglTexts.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2308 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleProjectInformation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21438 2024-04-28 19:26:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTanglePyut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4574 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4647 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangleUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8020 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnTangler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/UnsupportedFileTypeException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3647 2024-01-15 02:11:32.000000 untanglepyut-2.1.8/src/untanglepyut/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       80 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/XmlVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-04-28 19:14:54.000000 untanglepyut-2.1.8/src/untanglepyut/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:30:45.000000 untanglepyut-2.1.8/src/untanglepyut/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 20:25:03.715051 untanglepyut-2.1.8/src/untanglepyut.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3776 2024-04-28 20:25:03.000000 untanglepyut-2.1.8/src/untanglepyut.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      865 2024-04-28 20:25:03.000000 untanglepyut-2.1.8/src/untanglepyut.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-04-28 20:25:03.000000 untanglepyut-2.1.8/src/untanglepyut.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       92 2024-04-28 20:25:03.000000 untanglepyut-2.1.8/src/untanglepyut.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2024-04-28 20:25:03.000000 untanglepyut-2.1.8/src/untanglepyut.egg-info/top_level.txt
```

### Comparing `untanglepyut-2.1.7/LICENSE` & `untanglepyut-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/PKG-INFO` & `untanglepyut-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 2.1.7
+Version: 2.1.8
 Summary: XML to Ogl Object Model
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/untanglepyut
 Keywords: pyut,graphical shapes,python,xml
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: untangle==1.2.1
 Requires-Dist: codeallybasic>=1.3.0
 Requires-Dist: codeallyadvanced>=1.3.1
 Requires-Dist: pyutmodelv2>=2.1.5
-Requires-Dist: ogl>=2.1.20
+Requires-Dist: ogl>=2.1.31
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-window=last-30-days&insights-snapshot=true)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/untanglepyut/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/untanglepyut/tree/master)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 2.1.7 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 2.1.8 Summary: XML to Ogl
 Object Model Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/untanglepyut Keywords: pyut,graphical
 shapes,python,xml Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: untangle==1.2.1 Requires-Dist: codeallybasic>=1.3.0 Requires-
 Dist: codeallyadvanced>=1.3.1 Requires-Dist: pyutmodelv2>=2.1.5 Requires-Dist:
-ogl>=2.1.20 ![](https://github.com/hasii2011/code-ally-basic/blob/master/
+ogl>=2.1.31 ![](https://github.com/hasii2011/code-ally-basic/blob/master/
 developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [![CircleCI]
 (https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/master/
 main/badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/
 untanglepyut/workflows/main/overview?branch=master&reporting-window=last-30-
 days&insights-snapshot=true) [![CircleCI](https://dl.circleci.com/status-badge/
 img/gh/hasii2011/untanglepyut/tree/master.svg?style=shield)](https://
 dl.circleci.com/status-badge/redirect/gh/hasii2011/untanglepyut/tree/master) [!
```

### Comparing `untanglepyut-2.1.7/README.md` & `untanglepyut-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/pyproject.toml` & `untanglepyut-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 keywords    = ['pyut', 'graphical shapes', 'python', 'xml']
 
 dependencies = [
   'untangle==1.2.1',
   'codeallybasic>=1.3.0',
   'codeallyadvanced>=1.3.1',
   'pyutmodelv2>=2.1.5',
-  'ogl>=2.1.20',
+  'ogl>=2.1.31',
 ]
 
 [project.urls]
 Repository = 'https://github.com/hasii2011/untanglepyut'
 
 
 [tool.setuptools.packages.find]
```

### Comparing `untanglepyut-2.1.7/src/untanglepyut/BaseUnTangle.py` & `untanglepyut-2.1.8/src/untanglepyut/BaseUnTangle.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/Types.py` & `untanglepyut-2.1.8/src/untanglepyut/Types.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleIO.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleIO.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleOglClasses.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleOglClasses.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleOglLinks.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleOglLinks.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleOglNotes.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleOglNotes.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleOglTexts.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleOglTexts.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleProjectInformation.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleProjectInformation.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTanglePyut.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTanglePyut.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     destinationId: int           = -1
 
 
 class UnTanglePyut:
     """
     Converts pyutmodel Version 11 XML to Pyut Objects
     """
+    NOTE_NAME:   str = 'Note'
+    noteCounter: int = 0
 
     def __init__(self, xmlVersion: XmlVersion):
 
         self.logger: Logger = getLogger(__name__)
 
         self._xmlVersion: XmlVersion = xmlVersion
         if self._xmlVersion == XmlVersion.V10:
@@ -479,18 +481,21 @@
         Args:
             pyutElement:    pyutElement XML with common keys
             pyutObject:     The PyutObject to update
 
         Returns:  The updated pyutObject as
         """
 
-        pyutObject.id      = int(pyutElement[self._attrId])    # TODO revisit this when we start using UUIDs
-        pyutObject.name    = pyutElement['name']
+        pyutObject.id       = int(pyutElement[self._attrId])    # TODO revisit this when we start using UUIDs
+        pyutObject.name     = pyutElement['name']
         pyutObject.fileName = pyutElement[self._attrFileName]
 
+        if pyutObject.name is None:
+            UnTanglePyut.noteCounter += 1
+            pyutObject.name = f'{UnTanglePyut.NOTE_NAME}-{UnTanglePyut.noteCounter}'
         return pyutObject
 
     def _securePyutDisplayMethods(self, displayStr: str) -> PyutDisplayMethods:
 
         if displayStr is not None:
             pyutDisplayMethods: PyutDisplayMethods = PyutDisplayMethods(displayStr)
         else:
```

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleSequenceDiagram.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangleUseCaseDiagram.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangleUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/UnTangler.py` & `untanglepyut-2.1.8/src/untanglepyut/UnTangler.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut/XmlConstants.py` & `untanglepyut-2.1.8/src/untanglepyut/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-2.1.7/src/untanglepyut.egg-info/PKG-INFO` & `untanglepyut-2.1.8/src/untanglepyut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: untanglepyut
-Version: 2.1.7
+Version: 2.1.8
 Summary: XML to Ogl Object Model
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/untanglepyut
 Keywords: pyut,graphical shapes,python,xml
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: untangle==1.2.1
 Requires-Dist: codeallybasic>=1.3.0
 Requires-Dist: codeallyadvanced>=1.3.1
 Requires-Dist: pyutmodelv2>=2.1.5
-Requires-Dist: ogl>=2.1.20
+Requires-Dist: ogl>=2.1.31
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![CircleCI](https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/master/main/badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/untanglepyut/workflows/main/overview?branch=master&reporting-window=last-30-days&insights-snapshot=true)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/untanglepyut/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/untanglepyut/tree/master)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: untanglepyut Version: 2.1.7 Summary: XML to Ogl
+Metadata-Version: 2.1 Name: untanglepyut Version: 2.1.8 Summary: XML to Ogl
 Object Model Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/untanglepyut Keywords: pyut,graphical
 shapes,python,xml Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: untangle==1.2.1 Requires-Dist: codeallybasic>=1.3.0 Requires-
 Dist: codeallyadvanced>=1.3.1 Requires-Dist: pyutmodelv2>=2.1.5 Requires-Dist:
-ogl>=2.1.20 ![](https://github.com/hasii2011/code-ally-basic/blob/master/
+ogl>=2.1.31 ![](https://github.com/hasii2011/code-ally-basic/blob/master/
 developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [![CircleCI]
 (https://dl.circleci.com/insights-snapshot/gh/hasii2011/untanglepyut/master/
 main/badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/
 untanglepyut/workflows/main/overview?branch=master&reporting-window=last-30-
 days&insights-snapshot=true) [![CircleCI](https://dl.circleci.com/status-badge/
 img/gh/hasii2011/untanglepyut/tree/master.svg?style=shield)](https://
 dl.circleci.com/status-badge/redirect/gh/hasii2011/untanglepyut/tree/master) [!
```

### Comparing `untanglepyut-2.1.7/src/untanglepyut.egg-info/SOURCES.txt` & `untanglepyut-2.1.8/src/untanglepyut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

