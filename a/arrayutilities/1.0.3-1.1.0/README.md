# Comparing `tmp/arrayutilities-1.0.3.tar.gz` & `tmp/arrayutilities-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayutilities-1.0.3.tar", last modified: Sat Apr 27 17:49:42 2024, max compression
+gzip compressed data, was "arrayutilities-1.1.0.tar", last modified: Sat Apr 27 23:23:50 2024, max compression
```

## Comparing `arrayutilities-1.0.3.tar` & `arrayutilities-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/
--rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.3/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)    18918 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)    17127 2024-04-27 17:47:07.000000 arrayutilities-1.0.3/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.233993 arrayutilities-1.0.3/arrayutilities/
--rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.3/arrayutilities/__init__.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/arrayutilities.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    18918 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      664 2024-04-27 17:49:09.000000 arrayutilities-1.0.3/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:49:13.000000 arrayutilities-1.0.3/setup.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.3/tests/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_accessible.py
--rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add_prefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add_unprefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_array_visit_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_collapse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_dot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_exists.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_filter_prefixed.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_first.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_flatten.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_forget.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_get.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_has.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_insert_after_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_insert_before_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_is_dict.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_is_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_join.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_last.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_list_to_array.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_merge_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_only.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_prepend.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_pull.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_query.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_random.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_recursive_ksort.py
--rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_set.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_shape_filter.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_shuffle.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_sort_by_priority.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_sort_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_stringify_keys.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_strpos.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_to_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_undot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_usearch.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_where.py
--rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_where_not_none.py
--rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_wrap.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 23:23:50.258999 arrayutilities-1.1.0/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.1.0/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)    29651 2024-04-27 23:23:50.258999 arrayutilities-1.1.0/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)    27860 2024-04-27 23:22:33.000000 arrayutilities-1.1.0/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 23:23:50.248999 arrayutilities-1.1.0/arrayutilities/
+-rw-r--r--   0 matt      (1000) matt      (1000)    28944 2024-04-27 23:14:07.000000 arrayutilities-1.1.0/arrayutilities/__init__.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 23:23:50.258999 arrayutilities-1.1.0/arrayutilities.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    29651 2024-04-27 23:23:50.000000 arrayutilities-1.1.0/arrayutilities.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 23:23:50.000000 arrayutilities-1.1.0/arrayutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 23:23:50.000000 arrayutilities-1.1.0/arrayutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 23:23:50.000000 arrayutilities-1.1.0/arrayutilities.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      664 2024-04-27 23:23:19.000000 arrayutilities-1.1.0/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 23:23:50.258999 arrayutilities-1.1.0/setup.cfg
+-rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 23:23:14.000000 arrayutilities-1.1.0/setup.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 23:23:50.258999 arrayutilities-1.1.0/tests/
+-rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.1.0/tests/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.1.0/tests/test_accessible.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1176 2024-04-27 21:13:34.000000 arrayutilities-1.1.0/tests/test_add.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1670 2024-04-27 21:41:47.000000 arrayutilities-1.1.0/tests/test_add_prefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_add_unprefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.1.0/tests/test_collapse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.1.0/tests/test_dot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.1.0/tests/test_exists.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_filter_prefixed.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_first.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_flatten.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_forget.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2257 2024-04-27 21:10:51.000000 arrayutilities-1.1.0/tests/test_get.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_has.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1624 2024-04-27 22:42:12.000000 arrayutilities-1.1.0/tests/test_insert_after_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1147 2024-04-27 22:47:30.000000 arrayutilities-1.1.0/tests/test_insert_before_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_is_dict.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_is_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_join.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_last.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1125 2024-04-27 21:35:24.000000 arrayutilities-1.1.0/tests/test_list_to_dict.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1284 2024-04-27 23:13:34.000000 arrayutilities-1.1.0/tests/test_list_to_string.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_merge_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_only.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_prepend.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_pull.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_query.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_random.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_recursive_ksort.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_set.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_shape_filter.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_shuffle.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_sort_by_priority.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_sort_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1628 2024-04-27 21:29:40.000000 arrayutilities-1.1.0/tests/test_str_to_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_stringify_keys.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_strpos.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_undot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_usearch.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 21:58:03.000000 arrayutilities-1.1.0/tests/test_visit_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_where.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_where_not_none.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.1.0/tests/test_wrap.py
```

### Comparing `arrayutilities-1.0.3/LICENSE` & `arrayutilities-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/arrayutilities/__init__.py` & `arrayutilities-1.1.0/arrayutilities/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,38 +30,48 @@
             array: Array to manipulate.
             key: Key to use.
             value: Value to inject.
 
         Returns:
             Manipulated array
         """
-        if Arr.get(array, key) is None:
-            Arr.set(array, key, value)
+        if isinstance(array, list) and isinstance(key, int) and len(array) < key:
+            array.extend([value])
+        elif Arr.get(array, key) is None:
+            array = Arr.set(array, key, value)
         return array
 
     @staticmethod
     def add_prefixed_keys_to(array, recursive=False):
         """
         Duplicates any key not prefixed with '_' creating a prefixed duplicate one.
 
         Args:
             array: Array to manipulate.
             recursive (bool, optional): Whether to recursively change the array. Defaults to False.
 
         Returns:
             Manipulated array.
         """
-        if not isinstance(array, dict):
+        if not isinstance(array, dict) and not isinstance(array, list):
             return array
 
+        array = Arr.list_to_dict(array)
+
         prefixed = {}
         for key, value in array.items():
             if recursive and isinstance(value, dict):
                 value = Arr.add_prefixed_keys_to(value, True)
                 array[key] = {**array[key], **value}
+            elif recursive and isinstance(value, list):
+                value = Arr.add_prefixed_keys_to(value, True)
+                array[key] = {**array[key], **value}
+
+            if isinstance(key, int):
+                key = str(key)
 
             if not key.startswith('_'):
                 prefixed[f'_{key}'] = value
 
         return {**array, **prefixed}
 
     @staticmethod
@@ -92,42 +102,14 @@
                 to_update[new_key] = value
 
         # Update the array with unprefixed keys at the current level
         array.update(to_update)
         return array
 
     @staticmethod
-    def array_visit_recursive(input_array, visitor):
-        """
-        Recursively visits all elements of an array applying the specified callback to each element key and value.
-
-        Args:
-            input_array: The input array whose nodes should be visited.
-            visitor: A callback function that will be called on each array item; the callback will
-                        receive the item key and value as input and should return an array that contains
-                        the update key and value in the shape [ &lt;key&gt;, &lt;value&gt; ]. Returning a null
-                        key will cause the element to be removed from the array.
-
-        Returns:
-            Manipulated array.
-        """
-        if not isinstance(input_array, dict):
-            return input_array
-
-        result = {}
-        for key, value in input_array.items():
-            if isinstance(value, dict):
-                value = Arr.array_visit_recursive(value, visitor)
-            updated_key, updated_value = visitor(key, value)
-            if updated_key is not None:
-                result[updated_key] = updated_value
-
-        return result
-
-    @staticmethod
     def collapse(array):
         """
         Collapse an array of arrays into a single array.
 
         Args:
             array: Array of arrays to collapse.
 
@@ -210,15 +192,15 @@
     @staticmethod
     def flatten(array, depth=float('inf')):
         """
         Flatten a multi-dimensional array into a single level.
 
         Args:
             array: Array to flatten.
-            depth (number, optional): Number of nestings deep that should be flattened. Defaults to float('inf').
+            depth (int, optional): Number of nestings deep that should be flattened. Defaults to float('inf').
 
         Returns:
             Flattened array.
         """
         result = []
         for item in array:
             if isinstance(item, list) and depth >= 1:
@@ -281,48 +263,112 @@
         keys = Arr.wrap(keys)
         for key in keys:
             if key not in array:
                 return False
         return True
 
     @staticmethod
-    def insert_after_key(key, source_array, insert):
+    def insert_after_key(key, source, insert):
         """
-        Insert an array after a specified key within another array.
+        Insert an item or items after a specified key within a list or a dictionary.
 
         Args:
-            key (str|number): The key of the array to insert after.
-            source_array (array): The array to insert into.
+            key (str|int): The key or index of the item to insert after.
+            source (list|dict): The list or dictionary to insert into.
             insert (Any): Value or array to insert.
 
         Returns:
-            Manipulated array.
+            list|dict: Manipulated source with the insertions.
         """
-        if not isinstance(insert, list):
-            insert = [insert]
-        index = next((i for i, k in enumerate(source_array) if k == key), len(source_array))
-        return source_array[:index+1] + insert + source_array[index+1:]
+        if isinstance(source, list):
+            # Handle list
+            if isinstance(key, int) and 0 <= key < len(source):
+                insert_position = key + 1
+            else:
+                insert_position = len(source)  # Append at the end if out of bounds
+            if isinstance(insert, list):
+                source[insert_position:insert_position] = insert
+            else:
+                source.insert(insert_position, insert)
+
+        elif isinstance(source, dict):
+            # Handle dictionary
+            if key in source:
+                keys = list(source.keys())
+                index = keys.index(key) + 1
+                new_dict = {}
+                for k in keys[:index]:
+                    new_dict[k] = source[k]
+                if isinstance(insert, dict):
+                    new_dict.update(insert)
+                else:
+                    # Raise error for non-dict inserts into dicts
+                    raise TypeError("Insertion into a dictionary must be a dictionary")
+                for k in keys[index:]:
+                    new_dict[k] = source[k]
+                source = new_dict
+            else:
+                if isinstance(insert, dict):
+                    source.update(insert)
+                else:
+                    source[key] = insert  # Add at the end if key does not exist
+        else:
+            raise TypeError("Source must be either a list or a dictionary")
+
+        return source
 
     @staticmethod
-    def insert_before_key(key, source_array, insert):
+    def insert_before_key(key, source, insert):
         """
-        Insert an array before a specified key within another array.
+        Insert an item or items before a specified key within a list or a dictionary.
 
         Args:
-            key (str|number): The key of the array to insert before.
-            source_array (array): The array to insert into.
+            key (str|int): The key or index of the item to insert before.
+            source (list|dict): The list or dictionary to insert into.
             insert (Any): Value or array to insert.
 
         Returns:
-            Manipulated array.
+            list|dict: Manipulated source with the insertions.
         """
-        if not isinstance(insert, list):
-            insert = [insert]
-        index = next((i for i, k in enumerate(source_array) if k == key), len(source_array))
-        return source_array[:index] + insert + source_array[index:]
+        if isinstance(source, list):
+            # Handle list
+            if isinstance(key, int) and 0 <= key < len(source):
+                insert_position = key
+            else:
+                # If the key is out of range, do not append it at the end; handle it as error or ignore
+                raise IndexError("List index out of range")
+            if isinstance(insert, list):
+                source[insert_position:insert_position] = insert
+            else:
+                source.insert(insert_position, insert)
+
+        elif isinstance(source, dict):
+            # Handle dictionary
+            if key in source:
+                keys = list(source.keys())
+                index = keys.index(key)
+                new_dict = {}
+                for k in keys[:index]:
+                    new_dict[k] = source[k]
+                if isinstance(insert, dict):
+                    new_dict.update(insert)
+                else:
+                    # Raise error for non-dict inserts into dicts
+                    raise TypeError("Insertion into a dictionary must be a dictionary")
+                for k in keys[index:]:
+                    new_dict[k] = source[k]
+                source = new_dict
+            else:
+                # If the key does not exist, handle as error or ignore
+                raise KeyError(f"Key '{key}' not found in dictionary")
+
+        else:
+            raise TypeError("Source must be either a list or a dictionary")
+
+        return source
 
     @staticmethod
     def is_dict(array):
         """
         Returns whether the array is a dict or not.
 
         Args:
@@ -388,33 +434,50 @@
 
         for element in reversed(array):
             if callback(element):
                 return element
 
         return default
 
+
     @staticmethod
-    def list_to_array(value, sep=','):
+    def list_to_dict(value):
         """
-        Converts a list to an array filtering out empty string elements.
+        Converts a list to a dict.
 
         Args:
-            value (str|number|None): A string representing a list of values separated by the specified separator
-                            or an array. If the list is a string (e.g. a CSV list) then it will urldecoded
-                            before processing.
-            sep (str, optional): The char(s) separating the list elements; will be ignored if the list is an array. Defaults to ','.
+            value (list): A list to convert to a dict.
 
         Returns:
-            Manipulated array.
+            dict: Converted list.
         """
-        if not value:
-            return []
-        if isinstance(value, str):
-            value = value.split(sep)
-        return [v.strip() for v in value if v.strip()]
+        if isinstance(value, dict):
+            return value
+
+        value = Arr.wrap(value)
+
+        return dict(enumerate(value))
+
+    @staticmethod
+    def list_to_string(list_items, sep=','):
+        """
+        Returns a list separated by the specified separator.
+
+        Args:
+            list_items: Array of items.
+            sep (str, optional): Separator. Defaults to ','.
+
+        Returns:
+            The list separated by the specified separator or the original list if the list is empty.
+        """
+        if not list_items:
+            return list_items
+        if isinstance(list_items, list):
+            return sep.join(map(str, list_items))
+        return str(list_items)
 
     @staticmethod
     def merge_recursive(array1, array2):
         """
         Recursively merge two arrays preserving keys.
 
         Args:
@@ -450,15 +513,15 @@
     def prepend(array, value, key=None):
         """
         Push an item onto the beginning of an array.
 
         Args:
             array: Array to manipulate.
             value (Any): Value to prepend.
-            key (string|number, optional): Key value for the prepended item. Defaults to None.
+            key (string|int, optional): Key value for the prepended item. Defaults to None.
 
         Returns:
             Manipulated array.
         """
         if isinstance(array, list):
             array.insert(0, value)
         elif isinstance(array, dict):
@@ -471,15 +534,15 @@
     @staticmethod
     def pull(array, key, default=None):
         """
         Get a value from the array, and remove it.
 
         Args:
             array: Array to search and manipulate.
-            key (str|number): Key to look for and fetch.
+            key (str|int): Key to look for and fetch.
             default (Any, optional): Default value if none found. Defaults to None.
 
         Returns:
             Any: The found value or default.
         """
         value = Arr.get(array, key, default)
         Arr.forget(array, key)
@@ -518,15 +581,15 @@
     @staticmethod
     def random(array, number=None, preserve_keys=False):
         """
         Get one or a specified number of random values from an array.
 
         Args:
             array: Array to search through.
-            number (number, optional): Number of items to randomly grab. Defaults to None.
+            number (int, optional): Number of items to randomly grab. Defaults to None.
             preserve_keys (bool, optional): Whether the keys should be preserved or not. Defaults to False.
 
         Raises:
             ValueError
 
         Returns:
             Array with the random values.
@@ -709,30 +772,32 @@
         for needle in needles:
             position = haystack.find(needle, offset)
             if position != -1 and position < min_position:
                 min_position = position
         return min_position if min_position != len(haystack) else False
 
     @staticmethod
-    def to_list(list_items, sep=','):
+    def str_to_list(value, sep=','):
         """
-        Returns a list separated by the specified separator.
+        Converts a list to an array filtering out empty string elements.
 
         Args:
-            list_items: Array of items.
-            sep (str, optional): Separator. Defaults to ','.
+            value (str|int|None): A string representing a list of values separated by the specified separator
+                            or an array. If the list is a string (e.g. a CSV list) then it will urldecoded
+                            before processing.
+            sep (str, optional): The char(s) separating the list elements; will be ignored if the list is an array. Defaults to ','.
 
         Returns:
-            The list separated by the specified separator or the original list if the list is empty.
+            Manipulated array.
         """
-        if not list_items:
-            return list_items
-        if isinstance(list_items, list):
-            return sep.join(map(str, list_items))
-        return str(list_items)
+        if not value:
+            return []
+        if isinstance(value, str):
+            value = value.split(sep)
+        return [v.strip() for v in value if v.strip()]
 
     @staticmethod
     def undot(obj):
         """
         Convert a flatten "dot" notation array into an expanded array.
 
         Args:
@@ -778,14 +843,42 @@
         """
         for key, value in haystack.items():
             if callback(needle, value, key):
                 return key
         return False
 
     @staticmethod
+    def visit_recursive(input_array, visitor):
+        """
+        Recursively visits all elements of an array applying the specified callback to each element key and value.
+
+        Args:
+            input_array: The input array whose nodes should be visited.
+            visitor: A callback function that will be called on each array item; the callback will
+                        receive the item key and value as input and should return an array that contains
+                        the update key and value in the shape [ &lt;key&gt;, &lt;value&gt; ]. Returning a null
+                        key will cause the element to be removed from the array.
+
+        Returns:
+            Manipulated array.
+        """
+        if not isinstance(input_array, dict):
+            return input_array
+
+        result = {}
+        for key, value in input_array.items():
+            if isinstance(value, dict):
+                value = Arr.visit_recursive(value, visitor)
+            updated_key, updated_value = visitor(key, value)
+            if updated_key is not None:
+                result[updated_key] = updated_value
+
+        return result
+
+    @staticmethod
     def where(array, callback):
         """
         Filter the array using the given callback.
 
         Args:
             array: Array to filter.
             callback (function): Function that returns True if the element should be retained, False otherwise.
```

### Comparing `arrayutilities-1.0.3/arrayutilities.egg-info/SOURCES.txt` & `arrayutilities-1.1.0/arrayutilities.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 arrayutilities.egg-info/dependency_links.txt
 arrayutilities.egg-info/top_level.txt
 tests/__init__.py
 tests/test_accessible.py
 tests/test_add.py
 tests/test_add_prefixed_keys_to.py
 tests/test_add_unprefixed_keys_to.py
-tests/test_array_visit_recursive.py
 tests/test_collapse.py
 tests/test_dot.py
 tests/test_exists.py
 tests/test_filter_prefixed.py
 tests/test_first.py
 tests/test_flatten.py
 tests/test_forget.py
@@ -24,28 +23,30 @@
 tests/test_has.py
 tests/test_insert_after_key.py
 tests/test_insert_before_key.py
 tests/test_is_dict.py
 tests/test_is_list.py
 tests/test_join.py
 tests/test_last.py
-tests/test_list_to_array.py
+tests/test_list_to_dict.py
+tests/test_list_to_string.py
 tests/test_merge_recursive.py
 tests/test_only.py
 tests/test_prepend.py
 tests/test_pull.py
 tests/test_query.py
 tests/test_random.py
 tests/test_recursive_ksort.py
 tests/test_set.py
 tests/test_shape_filter.py
 tests/test_shuffle.py
 tests/test_sort_by_priority.py
 tests/test_sort_recursive.py
+tests/test_str_to_list.py
 tests/test_stringify_keys.py
 tests/test_strpos.py
-tests/test_to_list.py
 tests/test_undot.py
 tests/test_usearch.py
+tests/test_visit_recursive.py
 tests/test_where.py
 tests/test_where_not_none.py
 tests/test_wrap.py
```

### Comparing `arrayutilities-1.0.3/pyproject.toml` & `arrayutilities-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-sysetm]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrayutilities"
-version = "1.0.3"
+version = "1.1.0"
 description = "A library for list, dict, and UserDict manipulations."
 readme = "README.md"
 authors = [{ name = "Matthew Batchelder", email = "borkweb@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `arrayutilities-1.0.3/tests/test_accessible.py` & `arrayutilities-1.1.0/tests/test_accessible.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_add.py` & `arrayutilities-1.1.0/tests/test_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,24 @@
         self.assertEqual(result, {'a': 1, 'b': 2}, "Should add a new key-value pair")
 
     def test_add_existing_key(self):
         test_dict = {'a': 1}
         result = Arr.add(test_dict, 'a', 3)
         self.assertEqual(result, {'a': 1}, "Should not modify existing key")
 
-    def test_add_with_non_dict(self):
+    def test_no_add_with_overlap_and_non_dict(self):
         test_list = [1, 2, 3]
         result = Arr.add(test_list, 1, 4)
         self.assertEqual(result, [1, 2, 3], "Should return the original list unmodified")
 
+    def test_add_with_non_dict(self):
+        test_list = [1, 2, 3]
+        result = Arr.add(test_list, 4, 4)
+        self.assertEqual(result, [1, 2, 3, 4], "Should add a new key-value pair")
+
     def test_add_none_value(self):
         test_dict = {'a': 1}
         result = Arr.add(test_dict, 'b', None)
         self.assertEqual(result, {'a': 1, 'b': None}, "Should add key with None as value")
 
 # This allows the test to be run from the command line
 if __name__ == '__main__':
```

### Comparing `arrayutilities-1.0.3/tests/test_add_prefixed_keys_to.py` & `arrayutilities-1.1.0/tests/test_add_prefixed_keys_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import unittest
 from arrayutilities import Arr
 
 class TestArr(unittest.TestCase):
     def test_add_prefixed_keys_non_dict(self):
+        test_list = [1, 2, 3]
+        expected = {0: 1, 1: 2, 2: 3, '_0': 1, '_1': 2, '_2': 3}
         result = Arr.add_prefixed_keys_to([1, 2, 3])
-        self.assertEqual(result, [1, 2, 3], "Should return the original list unmodified")
+        self.assertEqual(result, expected, "Should return a dict with prefixed keys added")
 
     def test_add_prefixed_keys_simple_dict(self):
         test_dict = {'a': 1, 'b': 2}
         expected = {'a': 1, 'b': 2, '_a': 1, '_b': 2}
         result = Arr.add_prefixed_keys_to(test_dict)
         self.assertEqual(result, expected, "Should add prefixed keys to dictionary")
 
@@ -20,10 +22,16 @@
 
     def test_add_prefixed_keys_recursive(self):
         test_dict = {'a': {'c': 3}, 'b': 2}
         expected = {'a': {'c': 3, '_c': 3}, 'b': 2, '_a': {'c': 3, '_c': 3}, '_b': 2}
         result = Arr.add_prefixed_keys_to(test_dict, recursive=True)
         self.assertEqual(result, expected, "Should add prefixed keys recursively to nested dictionaries")
 
+    def test_add_prefixed_keys_list(self):
+        test_dict = [ 1, 2 ]
+        expected = {0: 1, 1: 2, '_0': 1, '_1': 2}
+        result = Arr.add_prefixed_keys_to(test_dict)
+        self.assertEqual(result, expected, "Should add prefixed keys to dictionary")
+
 # This allows the test to be run from the command line
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arrayutilities-1.0.3/tests/test_add_unprefixed_keys_to.py` & `arrayutilities-1.1.0/tests/test_add_unprefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_array_visit_recursive.py` & `arrayutilities-1.1.0/tests/test_visit_recursive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import unittest
 from arrayutilities import Arr
 
 class TestArr(unittest.TestCase):
     def test_non_dict_input(self):
-        result = Arr.array_visit_recursive([1, 2, 3], lambda k, v: (k, v))
+        result = Arr.visit_recursive([1, 2, 3], lambda k, v: (k, v))
         self.assertEqual(result, [1, 2, 3], "Should return non-dict input as is")
 
     def test_simple_dict(self):
         test_dict = {'a': 1, 'b': 2}
-        result = Arr.array_visit_recursive(test_dict, lambda k, v: (k, v * 2))
+        result = Arr.visit_recursive(test_dict, lambda k, v: (k, v * 2))
         expected = {'a': 2, 'b': 4}
         self.assertEqual(result, expected, "Should process simple dictionary and apply visitor to values")
 
     def test_recursive_dict(self):
         test_dict = {'a': {'c': 3}, 'b': 2}
-        result = Arr.array_visit_recursive(test_dict, lambda k, v: (k, v if isinstance(v, dict) else v * 3))
+        result = Arr.visit_recursive(test_dict, lambda k, v: (k, v if isinstance(v, dict) else v * 3))
         expected = {'a': {'c': 9}, 'b': 6}
         self.assertEqual(result, expected, "Should process nested dictionary recursively")
 
     def test_ignore_none_keys(self):
         test_dict = {'a': 1, 'b': 2}
-        result = Arr.array_visit_recursive(test_dict, lambda k, v: (None, v * 2) if k == 'a' else (k, v * 2))
+        result = Arr.visit_recursive(test_dict, lambda k, v: (None, v * 2) if k == 'a' else (k, v * 2))
         expected = {'b': 4}
         self.assertEqual(result, expected, "Should exclude keys where visitor returns None for key")
 
     def test_key_modification(self):
         test_dict = {'a': 1, 'b': 2}
-        result = Arr.array_visit_recursive(test_dict, lambda k, v: (k.upper(), v))
+        result = Arr.visit_recursive(test_dict, lambda k, v: (k.upper(), v))
         expected = {'A': 1, 'B': 2}
         self.assertEqual(result, expected, "Should modify keys based on visitor output")
 
 # This allows the test to be run from the command line
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arrayutilities-1.0.3/tests/test_collapse.py` & `arrayutilities-1.1.0/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_dot.py` & `arrayutilities-1.1.0/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_exists.py` & `arrayutilities-1.1.0/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_filter_prefixed.py` & `arrayutilities-1.1.0/tests/test_filter_prefixed.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_first.py` & `arrayutilities-1.1.0/tests/test_first.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_flatten.py` & `arrayutilities-1.1.0/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_forget.py` & `arrayutilities-1.1.0/tests/test_forget.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_get.py` & `arrayutilities-1.1.0/tests/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,22 @@
         self.assertEqual(result, 2, "Should return the value of key 'b'")
 
     def test_get_nested_key(self):
         test_dict = {'a': 1, 'b': {'c': 2, 'd': 3}}
         result = Arr.get(test_dict, ['b', 'c'])
         self.assertEqual(result, 2, "Should return the value of nested key 'c' under 'b'")
 
+    def test_get_deep_nested_key(self):
+        test_dict = {'a': 1, 'b': {'c': { 'e': 2}, 'd': 3}}
+        result = Arr.get(test_dict, ['b', 'c', 'e'])
+        self.assertEqual(result, 2, "Should return the value of nested key 'e' under 'c' under 'b'")
+
+        result = Arr.get(test_dict, ['b', 'd'])
+        self.assertEqual(result, 3, "Should return the value of nested key 'd' under 'b'")
+
     def test_get_non_existent_key_returns_default(self):
         test_dict = {'a': 1, 'b': 2}
         result = Arr.get(test_dict, 'c', default='Not Found')
         self.assertEqual(result, 'Not Found', "Should return the default value when key does not exist")
 
     def test_get_nested_non_existent_key_returns_default(self):
         test_dict = {'a': {'b': 2}}
```

### Comparing `arrayutilities-1.0.3/tests/test_has.py` & `arrayutilities-1.1.0/tests/test_has.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_is_dict.py` & `arrayutilities-1.1.0/tests/test_is_dict.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_is_list.py` & `arrayutilities-1.1.0/tests/test_is_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_join.py` & `arrayutilities-1.1.0/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_last.py` & `arrayutilities-1.1.0/tests/test_last.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_list_to_array.py` & `arrayutilities-1.1.0/tests/test_str_to_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from arrayutilities import Arr
 import unittest
 
 class TestArr(unittest.TestCase):
     def test_list_to_array_with_default_separator(self):
-        result = Arr.list_to_array("apple, banana, cherry")
+        result = Arr.str_to_list("apple, banana, cherry")
         self.assertEqual(result, ["apple", "banana", "cherry"], "Should convert string with default separator to list")
 
     def test_list_to_array_with_custom_separator(self):
-        result = Arr.list_to_array("apple|banana|cherry", sep="|")
+        result = Arr.str_to_list("apple|banana|cherry", sep="|")
         self.assertEqual(result, ["apple", "banana", "cherry"], "Should convert string with custom separator to list")
 
     def test_list_to_array_empty_string(self):
-        result = Arr.list_to_array("")
+        result = Arr.str_to_list("")
         self.assertEqual(result, [], "Should return an empty list for empty string")
 
     def test_list_to_array_with_empty_elements(self):
-        result = Arr.list_to_array("apple,,banana,")
+        result = Arr.str_to_list("apple,,banana,")
         self.assertEqual(result, ["apple", "banana"], "Should remove empty elements from string")
 
     def test_list_to_array_list_input(self):
-        result = Arr.list_to_array(["apple", "banana", "cherry"])
+        result = Arr.str_to_list(["apple", "banana", "cherry"])
         self.assertEqual(result, ["apple", "banana", "cherry"], "Should return the input list unchanged")
 
     def test_list_to_array_whitespace_elements(self):
-        result = Arr.list_to_array(" apple , banana , cherry ")
+        result = Arr.str_to_list(" apple , banana , cherry ")
         self.assertEqual(result, ["apple", "banana", "cherry"], "Should remove leading/trailing whitespace from elements")
 
     def test_list_to_array_whitespace_string(self):
-        result = Arr.list_to_array("  ")
+        result = Arr.str_to_list("  ")
         self.assertEqual(result, [], "Should return an empty list for string with only whitespace")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arrayutilities-1.0.3/tests/test_merge_recursive.py` & `arrayutilities-1.1.0/tests/test_merge_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_only.py` & `arrayutilities-1.1.0/tests/test_only.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_prepend.py` & `arrayutilities-1.1.0/tests/test_prepend.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_pull.py` & `arrayutilities-1.1.0/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_query.py` & `arrayutilities-1.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_random.py` & `arrayutilities-1.1.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_recursive_ksort.py` & `arrayutilities-1.1.0/tests/test_recursive_ksort.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_set.py` & `arrayutilities-1.1.0/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_shape_filter.py` & `arrayutilities-1.1.0/tests/test_shape_filter.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_shuffle.py` & `arrayutilities-1.1.0/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_sort_by_priority.py` & `arrayutilities-1.1.0/tests/test_sort_by_priority.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_sort_recursive.py` & `arrayutilities-1.1.0/tests/test_sort_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_stringify_keys.py` & `arrayutilities-1.1.0/tests/test_stringify_keys.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_strpos.py` & `arrayutilities-1.1.0/tests/test_strpos.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_to_list.py` & `arrayutilities-1.1.0/tests/test_list_to_string.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from arrayutilities import Arr
 import unittest
 
 class TestArrToList(unittest.TestCase):
     def test_to_list_with_list_input(self):
         list_items = ['apple', 'banana', 'cherry']
-        result = Arr.to_list(list_items)
+        result = Arr.list_to_string(list_items)
         self.assertEqual(result, 'apple,banana,cherry', "Should join list items with comma by default")
 
     def test_to_list_with_list_input_and_custom_sep(self):
         list_items = ['apple', 'banana', 'cherry']
-        result = Arr.to_list(list_items, sep=';')
+        result = Arr.list_to_string(list_items, sep=';')
         self.assertEqual(result, 'apple;banana;cherry', "Should join list items with custom separator")
 
     def test_to_list_with_string_input(self):
         list_items = 'apple, banana, cherry'
-        result = Arr.to_list(list_items)
+        result = Arr.list_to_string(list_items)
         self.assertEqual(result, 'apple, banana, cherry', "Should return the input string as is")
 
     def test_to_list_with_empty_input(self):
         list_items = ''
-        result = Arr.to_list(list_items)
+        result = Arr.list_to_string(list_items)
         self.assertEqual(result, '', "Should return empty string for empty input")
 
     def test_to_list_with_none_input(self):
         list_items = None
-        result = Arr.to_list(list_items)
+        result = Arr.list_to_string(list_items)
         self.assertIsNone(result, "Should return None for None input")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arrayutilities-1.0.3/tests/test_undot.py` & `arrayutilities-1.1.0/tests/test_undot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_usearch.py` & `arrayutilities-1.1.0/tests/test_usearch.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_where.py` & `arrayutilities-1.1.0/tests/test_where.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_where_not_none.py` & `arrayutilities-1.1.0/tests/test_where_not_none.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.3/tests/test_wrap.py` & `arrayutilities-1.1.0/tests/test_wrap.py`

 * *Files identical despite different names*

