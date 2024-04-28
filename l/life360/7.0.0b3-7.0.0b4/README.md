# Comparing `tmp/life360-7.0.0b3.tar.gz` & `tmp/life360-7.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-7.0.0b3.tar", last modified: Fri Apr 26 16:09:58 2024, max compression
+gzip compressed data, was "life360-7.0.0b4.tar", last modified: Sun Apr 28 16:50:38 2024, max compression
```

## Comparing `life360-7.0.0b3.tar` & `life360-7.0.0b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:09:58.542959 life360-7.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 16:09:55.000000 life360-7.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 16:09:58.542959 life360-7.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 16:09:55.000000 life360-7.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:09:58.542959 life360-7.0.0b3/life360/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 16:09:55.000000 life360-7.0.0b3/life360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-04-26 16:09:55.000000 life360-7.0.0b3/life360/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 16:09:55.000000 life360-7.0.0b3/life360/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-26 16:09:55.000000 life360-7.0.0b3/life360/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 16:09:55.000000 life360-7.0.0b3/life360/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:09:58.542959 life360-7.0.0b3/life360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-26 16:09:58.000000 life360-7.0.0b3/life360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 16:09:58.000000 life360-7.0.0b3/life360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:09:58.000000 life360-7.0.0b3/life360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 16:09:58.000000 life360-7.0.0b3/life360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 16:09:58.000000 life360-7.0.0b3/life360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:09:58.542959 life360-7.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-26 16:09:55.000000 life360-7.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:50:38.599400 life360-7.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 16:50:36.000000 life360-7.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-28 16:50:38.599400 life360-7.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-28 16:50:36.000000 life360-7.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:50:38.595400 life360-7.0.0b4/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-28 16:50:36.000000 life360-7.0.0b4/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-28 16:50:36.000000 life360-7.0.0b4/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-28 16:50:36.000000 life360-7.0.0b4/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-28 16:50:36.000000 life360-7.0.0b4/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 16:50:36.000000 life360-7.0.0b4/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:50:38.599400 life360-7.0.0b4/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-28 16:50:38.000000 life360-7.0.0b4/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-28 16:50:38.000000 life360-7.0.0b4/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:50:38.000000 life360-7.0.0b4/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 16:50:38.000000 life360-7.0.0b4/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 16:50:38.000000 life360-7.0.0b4/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:50:38.599400 life360-7.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-28 16:50:36.000000 life360-7.0.0b4/setup.py
```

### Comparing `life360-7.0.0b3/LICENSE` & `life360-7.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b3/PKG-INFO` & `life360-7.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b3
+Version: 7.0.0b4
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b3/README.md` & `life360-7.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b3/life360/__init__.py` & `life360-7.0.0b4/life360/__init__.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b3/life360/api.py` & `life360-7.0.0b4/life360/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,20 +232,20 @@
     ) -> Any:
         """Make a request to server."""
         if authorization is None:
             authorization = self.authorization
         if authorization is None:
             raise LoginError("Must login")
 
-        headers = _HEADERS
+        headers: dict[str, str] = {}
         if authorization != "":
             headers["authorization"] = authorization
         if raise_not_modified and (etag := self._etags.get(url)):
             headers["if-none-match"] = etag
-        kwargs.setdefault("headers", {}).update(headers)
+        kwargs["headers"] = _HEADERS | headers | kwargs.pop("headers", {})
 
         for attempt in range(1, self._max_attempts + 1):
             resp: ClientResponse | None = None
             status: int | None = None
             try:
                 resp = cast(
                     ClientResponse,
```

### Comparing `life360-7.0.0b3/life360/const.py` & `life360-7.0.0b4/life360/const.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b3/life360/exceptions.py` & `life360-7.0.0b4/life360/exceptions.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b3/life360.egg-info/PKG-INFO` & `life360-7.0.0b4/life360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b3
+Version: 7.0.0b4
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b3/setup.py` & `life360-7.0.0b4/setup.py`

 * *Files identical despite different names*

