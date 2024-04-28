# Comparing `tmp/portabletab-0.3.4.tar.gz` & `tmp/portabletab-0.3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portabletab-0.3.4.tar", max compression
+gzip compressed data, was "portabletab-0.3.5.dev1.tar", max compression
```

## Comparing `portabletab-0.3.4.tar` & `portabletab-0.3.5.dev1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.4/LICENSE
--rw-r--r--   0        0        0      203 2024-04-15 01:24:23.588886 portabletab-0.3.4/PortableTab/__init__.py
--rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.4/PortableTab/__main__.py
--rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.4/PortableTab/base_table.py
--rw-r--r--   0        0        0     4697 2024-03-28 02:55:40.041699 portabletab-0.3.4/PortableTab/capnp_manager.py
--rw-r--r--   0        0        0    18443 2024-03-28 02:55:46.657808 portabletab-0.3.4/PortableTab/capnp_table.py
--rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.4/PortableTab/exceptions.py
--rw-r--r--   0        0        0     2432 2024-04-03 05:01:01.335427 portabletab-0.3.4/README.md
--rw-r--r--   0        0        0      730 2024-04-15 01:36:03.399047 portabletab-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 portabletab-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.5.dev1/LICENSE
+-rw-r--r--   0        0        0      208 2024-04-28 02:44:57.663393 portabletab-0.3.5.dev1/PortableTab/__init__.py
+-rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.5.dev1/PortableTab/__main__.py
+-rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.5.dev1/PortableTab/base_table.py
+-rw-r--r--   0        0        0     4697 2024-03-28 02:55:40.041699 portabletab-0.3.5.dev1/PortableTab/capnp_manager.py
+-rw-r--r--   0        0        0    19169 2024-04-28 01:02:48.253253 portabletab-0.3.5.dev1/PortableTab/capnp_table.py
+-rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.5.dev1/PortableTab/exceptions.py
+-rw-r--r--   0        0        0     2432 2024-04-03 05:01:01.335427 portabletab-0.3.5.dev1/README.md
+-rw-r--r--   0        0        0      735 2024-04-28 02:45:12.435728 portabletab-0.3.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 portabletab-0.3.5.dev1/PKG-INFO
```

### Comparing `portabletab-0.3.4/LICENSE` & `portabletab-0.3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.4/PortableTab/__main__.py` & `portabletab-0.3.5.dev1/PortableTab/__main__.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.4/PortableTab/base_table.py` & `portabletab-0.3.5.dev1/PortableTab/base_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.4/PortableTab/capnp_manager.py` & `portabletab-0.3.5.dev1/PortableTab/capnp_manager.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.4/PortableTab/capnp_table.py` & `portabletab-0.3.5.dev1/PortableTab/capnp_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -350,15 +350,19 @@
                     buf=mm, traversal_limit_in_words=2**64-1) as list_obj:
 
                 while pos < offset + limit:
                     page_path = self._get_page_path(pos)
                     if page_path != current_path:
                         break
 
-                    yield list_obj.records[pos % self.PAGE_SIZE]
+                    record = list_obj.records[pos % self.PAGE_SIZE]
+                    if as_dict:
+                        record = record.to_dict()
+
+                    yield record
                     pos += 1
 
             mm.close()
             f.close()
 
     def append_records(
             self,
@@ -466,26 +470,34 @@
                 page=current_page,
                 records=records
             )
 
     def create_trie_on(
         self,
         attr: str,
-        func: Optional[Callable] = None
+        key_func: Optional[Callable] = None,
+        filter_func: Optional[Callable] = None,
     ) -> None:
         """
         Create TRIE index on the specified attribute.
 
         Paramters
         ---------
         attr: str
             The name of target attribute.
-        func: Callable
-            Function to generate a set of strings to be indexed.
-            If not specified, 'str' will be used.
+        key_func: Callable, optional
+            A function that takes the attribute value as argument
+            used to generate a set of index key strings from each record.
+            If not specified, the 'str' function will be used.
+        filter_func: Callable, optional
+            A function that takes the record as argument to determine
+            if the record should be added to the index or not.
+            When the function returns true (in the context of Boolean
+            operation), the record will be indexed.
+            If not specified, all records will be indexed.
 
         Notes
         -----
         - The created index is saved in the same directory as
           the page files with the file name "<attr>.trie".
         """
 
@@ -494,18 +506,21 @@
             # attribute value and position.
             for pos in range(self.count_records()):
                 record = CapnpTable.get_record(
                     self, pos=pos)  # Call base class method
                 if pos == 0 and not hasattr(record, attr):
                     raise ValueError(f"Attribute '{attr}' doesn't exist.")
 
-                if func is None:
+                if filter_func and not filter_func(record):
+                    continue
+
+                if key_func is None:
                     strings = str(getattr(record, attr))
                 else:
-                    strings = func(getattr(record, attr))
+                    strings = key_func(getattr(record, attr))
 
                 if isinstance(strings, str) and strings != "":
                     yield (strings, (pos,))
                 else:
                     for string in strings:
                         if string != "":
                             yield (string, (pos,))
```

### Comparing `portabletab-0.3.4/README.md` & `portabletab-0.3.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.4/pyproject.toml` & `portabletab-0.3.5.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PortableTab"
-version = "0.3.4"
+version = "0.3.5.dev1"
 description = "Python package for serializing tables in portable format with Capnp."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "PortableTab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `portabletab-0.3.4/PKG-INFO` & `portabletab-0.3.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PortableTab
-Version: 0.3.4
+Version: 0.3.5.dev1
 Summary: Python package for serializing tables in portable format with Capnp.
 License: MIT
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

