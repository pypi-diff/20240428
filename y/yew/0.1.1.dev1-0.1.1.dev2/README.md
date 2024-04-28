# Comparing `tmp/yew-0.1.1.dev1.tar.gz` & `tmp/yew-0.1.1.dev2.tar.gz`

## Comparing `yew-0.1.1.dev1.tar` & `yew-0.1.1.dev2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/requirements.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/setup.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/test.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/base.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/item.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/npc.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/player.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/__init__.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/api.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/format.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/item_mapper.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/src/yew/utils/wiki.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/LICENSE
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/README.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yew-0.1.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/test.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/base.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/item.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/npc.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/player.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/utils/__init__.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/utils/api.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/utils/format.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/utils/item_mapper.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/src/yew/utils/wiki.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/LICENSE
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yew-0.1.1.dev2/PKG-INFO
```

### Comparing `yew-0.1.1.dev1/src/yew/item.py` & `yew-0.1.1.dev2/src/yew/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,19 +49,18 @@
         self.high_price = 0
         self.low_price = 0
         self.high_price_time = None
         self.low_price_time = None
         self.high_price_volume = 0
         self.low_price_volume = 0
         self.since = None
-
         prices_data = fetch_item_prices(self.item_id, self.interval)
 
         if self.interval == "latest":
-            prices_data = prices_data.get(self.item_id, {})
+            prices_data = prices_data.get(str(self.item_id), {})
 
             if self.friendly_units:
                 self.high_price = get_friendly_unit(prices_data.get("high", 0))
                 self.low_price = get_friendly_unit(prices_data.get("low", 0))
             else:
                 self.high_price = prices_data.get("high", 0)
                 self.low_price = prices_data.get("low", 0)
```

### Comparing `yew-0.1.1.dev1/src/yew/player.py` & `yew-0.1.1.dev2/src/yew/player.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/src/yew/utils/api.py` & `yew-0.1.1.dev2/src/yew/utils/api.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/src/yew/utils/item_mapper.py` & `yew-0.1.1.dev2/src/yew/utils/item_mapper.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/src/yew/utils/wiki.py` & `yew-0.1.1.dev2/src/yew/utils/wiki.py`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/LICENSE` & `yew-0.1.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/README.md` & `yew-0.1.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `yew-0.1.1.dev1/pyproject.toml` & `yew-0.1.1.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yew"
-version = "0.1.1-dev1"
+version = "0.1.1-dev2"
 authors = [
   { name="Bharat Nair", email="bharat@rubberducker.xyz" },
 ]
 description = "An OldSchool RuneScape API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `yew-0.1.1.dev1/PKG-INFO` & `yew-0.1.1.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yew
-Version: 0.1.1.dev1
+Version: 0.1.1.dev2
 Summary: An OldSchool RuneScape API wrapper for Python.
 Project-URL: Homepage, https://github.com/bharat-nair/yew
 Project-URL: Issues, https://github.com/bharat-nair/yew/issues
 Author-email: Bharat Nair <bharat@rubberducker.xyz>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

