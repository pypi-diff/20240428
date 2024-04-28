# Comparing `tmp/pyxevil-1.0.0.tar.gz` & `tmp/pyxevil-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxevil-1.0.0.tar", last modified: Sun Apr 28 07:33:08 2024, max compression
+gzip compressed data, was "pyxevil-1.0.1.tar", last modified: Sun Apr 28 07:51:34 2024, max compression
```

## Comparing `pyxevil-1.0.0.tar` & `pyxevil-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 07:33:08.974835 pyxevil-1.0.0/
--rw-rw-rw-   0        0        0      875 2024-04-28 07:33:08.972835 pyxevil-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-04-28 07:26:24.000000 pyxevil-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 07:33:08.975835 pyxevil-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1290 2024-04-28 07:29:37.000000 pyxevil-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:33:08.933843 pyxevil-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 07:33:08.941840 pyxevil-1.0.0/src/pyxevil/
--rw-rw-rw-   0        0        0       26 2024-04-28 07:23:48.000000 pyxevil-1.0.0/src/pyxevil/__init__.py
--rw-rw-rw-   0        0        0      248 2024-04-28 07:31:24.000000 pyxevil-1.0.0/src/pyxevil/__version__.py
--rw-rw-rw-   0        0        0     4458 2024-04-28 05:56:30.000000 pyxevil-1.0.0/src/pyxevil/pyxevil.py
-drwxrwxrwx   0        0        0        0 2024-04-28 07:33:08.970835 pyxevil-1.0.0/src/pyxevil.egg-info/
--rw-rw-rw-   0        0        0      875 2024-04-28 07:33:08.000000 pyxevil-1.0.0/src/pyxevil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-28 07:33:08.000000 pyxevil-1.0.0/src/pyxevil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 07:33:08.000000 pyxevil-1.0.0/src/pyxevil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 07:33:08.000000 pyxevil-1.0.0/src/pyxevil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 07:33:08.000000 pyxevil-1.0.0/src/pyxevil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:34.746290 pyxevil-1.0.1/
+-rw-rw-rw-   0        0        0      875 2024-04-28 07:51:34.739291 pyxevil-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-04-28 07:26:24.000000 pyxevil-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 07:51:34.746290 pyxevil-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2024-04-28 07:29:37.000000 pyxevil-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:34.692300 pyxevil-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:34.704297 pyxevil-1.0.1/src/pyxevil/
+-rw-rw-rw-   0        0        0       26 2024-04-28 07:23:48.000000 pyxevil-1.0.1/src/pyxevil/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-04-28 07:51:17.000000 pyxevil-1.0.1/src/pyxevil/__version__.py
+-rw-rw-rw-   0        0        0     4549 2024-04-28 07:51:03.000000 pyxevil-1.0.1/src/pyxevil/pyxevil.py
+drwxrwxrwx   0        0        0        0 2024-04-28 07:51:34.737291 pyxevil-1.0.1/src/pyxevil.egg-info/
+-rw-rw-rw-   0        0        0      875 2024-04-28 07:51:34.000000 pyxevil-1.0.1/src/pyxevil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-28 07:51:34.000000 pyxevil-1.0.1/src/pyxevil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 07:51:34.000000 pyxevil-1.0.1/src/pyxevil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 07:51:34.000000 pyxevil-1.0.1/src/pyxevil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 07:51:34.000000 pyxevil-1.0.1/src/pyxevil.egg-info/top_level.txt
```

### Comparing `pyxevil-1.0.0/PKG-INFO` & `pyxevil-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxevil
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial python library to use service of xevil telegram
 Home-page: https://github.com/akasakaid/pyxevil
 Author: AkasakaID
 Author-email: akasakaid.gov@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxevil-1.0.0/setup.py` & `pyxevil-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyxevil-1.0.0/src/pyxevil/pyxevil.py` & `pyxevil-1.0.1/src/pyxevil/pyxevil.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         }
         res = requests.get(self.url_res, params=params)
         self.log(res.text)
         return True, res.text
 
     def anti_bot(self, data):
         data["method"] = "antibot"
+        data["key"] = self.key
         res = self.send_req(data)
         if res.find("|") >= 0:
             task_id = res.split("|")[1]
             res = self.get_result(task_id=task_id)
             return res
 
         return res
@@ -118,25 +119,27 @@
 
         return res
 
     def upside_down(self, base64_image):
         data = {
             "method": "viefaucet",
             "body": base64_image,
+            "key": self.key
         }
         res = self.send_req(data)
         if res.find("|") >= 0:
             task_id = res.split("|")[1]
             res = self.get_result(task_id=task_id)
             return res
 
         return res
 
     def authkong(self, site_url, site_key):
         data = {
+            "key": self.key,
             "method": "authkong",
             "pageurl": site_url,
             "sitekey": site_key,
         }
         res = self.send_req(data)
         if res.find('|') >= 0:
             task_id = res.split('|')[1]
```

### Comparing `pyxevil-1.0.0/src/pyxevil.egg-info/PKG-INFO` & `pyxevil-1.0.1/src/pyxevil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxevil
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial python library to use service of xevil telegram
 Home-page: https://github.com/akasakaid/pyxevil
 Author: AkasakaID
 Author-email: akasakaid.gov@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

