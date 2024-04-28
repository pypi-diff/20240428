# Comparing `tmp/yew-0.1.1.dev0.tar.gz` & `tmp/yew-0.1.1.dev1.tar.gz`

## Comparing `yew-0.1.1.dev0.tar` & `yew-0.1.1.dev1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/requirements.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/setup.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/test.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/base.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/item.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/npc.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/player.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/utils/__init__.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/utils/api.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/utils/format.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/utils/item_mapper.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/src/yew/utils/wiki.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/LICENSE
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/README.md
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 yew-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/requirements.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/setup.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/test.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/base.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/item.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/npc.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/player.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/__init__.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/api.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/format.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/item_mapper.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/wiki.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/LICENSE
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/PKG-INFO
```

### Comparing `yew-0.1.1.dev0/src/yew/item.py` & `yew-0.1.1.dev1/src/yew/item.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/src/yew/player.py` & `yew-0.1.1.dev1/src/yew/player.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/src/yew/utils/api.py` & `yew-0.1.1.dev1/src/yew/utils/api.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/src/yew/utils/item_mapper.py` & `yew-0.1.1.dev1/src/yew/utils/item_mapper.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/src/yew/utils/wiki.py` & `yew-0.1.1.dev1/src/yew/utils/wiki.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/LICENSE` & `yew-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/README.md` & `yew-0.1.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev0/pyproject.toml` & `yew-0.1.1.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yew"
-version = "0.1.1-dev"
+version = "0.1.1-dev1"
 authors = [
   { name="Bharat Nair", email="bharat@rubberducker.xyz" },
 ]
 description = "An OldSchool RuneScape API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.8"
+dependencies = [
+  "certifi==2024.2.2",
+  "charset-normalizer==3.3.2",
+  "idna==3.6",
+  "requests==2.31.0",
+  "urllib3==2.2.1",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Games/Entertainment",
```

### Comparing `yew-0.1.1.dev0/PKG-INFO` & `yew-0.1.1.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yew
-Version: 0.1.1.dev0
+Version: 0.1.1.dev1
 Summary: An OldSchool RuneScape API wrapper for Python.
 Project-URL: Homepage, https://github.com/bharat-nair/yew
 Project-URL: Issues, https://github.com/bharat-nair/yew/issues
 Author-email: Bharat Nair <bharat@rubberducker.xyz>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Role-Playing
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: idna==3.6
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3==2.2.1
 Description-Content-Type: text/markdown
 
 # ![yew-logs](https://oldschool.runescape.wiki/images/thumb/Yew_logs_detail.png/32px-Yew_logs_detail.png) yew
 
 `yew` is an OldSchool RuneScape API wrapper for Python. It lets you invoke entities of OSRS as Python objects.
 
 ## Installation
```

