# Comparing `tmp/amino.light.py-0.1.6.tar.gz` & `tmp/amino.light.py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.6.tar", last modified: Sun Apr 28 15:39:45 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.7.tar", last modified: Sun Apr 28 16:02:40 2024, max compression
```

## Comparing `amino.light.py-0.1.6.tar` & `amino.light.py-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.344263 amino.light.py-0.1.6/
-drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.230541 amino.light.py-0.1.6/AminoLightPy/
--rw-rw-rw-   0        0        0      297 2024-04-19 03:59:31.000000 amino.light.py-0.1.6/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.6/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.6/AminoLightPy/amino_socket.py
--rw-rw-rw-   0        0        0    74156 2024-04-28 15:28:46.000000 amino.light.py-0.1.6/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.6/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.233543 amino.light.py-0.1.6/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.6/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.258287 amino.light.py-0.1.6/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    82921 2024-04-23 09:48:31.000000 amino.light.py-0.1.6/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0      184 2024-04-24 15:17:48.000000 amino.light.py-0.1.6/AminoLightPy/managers.py
--rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.6/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3630 2024-04-28 15:39:45.343260 amino.light.py-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 15:39:45.334749 amino.light.py-0.1.6/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     3630 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-04-28 15:39:44.000000 amino.light.py-0.1.6/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-28 15:39:43.000000 amino.light.py-0.1.6/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 15:39:45.350260 amino.light.py-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-04-19 03:21:12.000000 amino.light.py-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:02:40.510724 amino.light.py-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-04-28 16:02:40.442214 amino.light.py-0.1.7/AminoLightPy/
+-rw-rw-rw-   0        0        0      297 2024-04-19 03:59:31.000000 amino.light.py-0.1.7/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.7/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.7/AminoLightPy/amino_socket.py
+-rw-rw-rw-   0        0        0    74156 2024-04-28 15:28:46.000000 amino.light.py-0.1.7/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.7/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:02:40.444213 amino.light.py-0.1.7/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.7/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:02:40.475150 amino.light.py-0.1.7/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.7/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.7/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.7/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    82996 2024-04-28 16:02:35.000000 amino.light.py-0.1.7/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0      184 2024-04-24 15:17:48.000000 amino.light.py-0.1.7/AminoLightPy/managers.py
+-rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.7/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3630 2024-04-28 16:02:40.508722 amino.light.py-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 16:02:40.506725 amino.light.py-0.1.7/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     3630 2024-04-28 16:02:40.000000 amino.light.py-0.1.7/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-04-28 16:02:40.000000 amino.light.py-0.1.7/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 16:02:40.000000 amino.light.py-0.1.7/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-28 16:02:40.000000 amino.light.py-0.1.7/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 16:02:40.000000 amino.light.py-0.1.7/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 16:02:40.519728 amino.light.py-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-28 16:02:31.000000 amino.light.py-0.1.7/setup.py
```

### Comparing `amino.light.py-0.1.6/AminoLightPy/acm.py` & `amino.light.py-0.1.7/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/amino_socket.py` & `amino.light.py-0.1.7/AminoLightPy/amino_socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/client.py` & `amino.light.py-0.1.7/AminoLightPy/client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/constants.py` & `amino.light.py-0.1.7/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.7/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.7/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.7/AminoLightPy/lib/util/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -879,19 +879,24 @@
 	__slots__ = (
 		"json", "subCategory", "author", "itemsCount",
 		"parentCategoryId", "categoryId", "extensions",
 		"createdTime", "title", "mediaList", "icon", "parentType"
 	)
 
 	def __init__(self, data):
+		if not data:
+			for attr in self.__slots__:
+				setattr(self, attr, None)
+			return
+
 		_author = [x.get("author") for x in data]
 
 		self.json = data
 
-		self.author: UserProfileList = UserProfileList(_author).UserProfileList
+		self.author = UserProfileList(_author).UserProfileList
 		self.itemsCount = []
 		self.parentCategoryId = []
 		self.categoryId = []
 		self.extensions = []
 		self.createdTime = []
 		self.title = []
 		self.mediaList = []
```

### Comparing `amino.light.py-0.1.6/AminoLightPy/sub_client.py` & `amino.light.py-0.1.7/AminoLightPy/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/LICENSE` & `amino.light.py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/PKG-INFO` & `amino.light.py-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.6 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.7 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.6/README.md` & `amino.light.py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.7/amino.light.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.6 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.7 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.6/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.7/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.6/setup.py` & `amino.light.py-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "augustlight",
     "aminolightpy",
     "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.6",
+    version="0.1.7",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

