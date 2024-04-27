# Comparing `tmp/arrayutilities-1.0.2.tar.gz` & `tmp/arrayutilities-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayutilities-1.0.2.tar", last modified: Sat Apr 27 17:48:13 2024, max compression
+gzip compressed data, was "arrayutilities-1.0.3.tar", last modified: Sat Apr 27 17:49:42 2024, max compression
```

## Comparing `arrayutilities-1.0.2.tar` & `arrayutilities-1.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/
--rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.2/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)    18908 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)    17127 2024-04-27 17:47:07.000000 arrayutilities-1.0.2/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.750130 arrayutilities-1.0.2/arrayutilities/
--rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.2/arrayutilities/__init__.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/arrayutilities.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    18908 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:48:13.000000 arrayutilities-1.0.2/arrayutilities.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      648 2024-04-27 17:47:48.000000 arrayutilities-1.0.2/pyproject.toml
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:47:45.000000 arrayutilities-1.0.2/setup.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:48:13.760130 arrayutilities-1.0.2/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.2/tests/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_accessible.py
--rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add_prefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_add_unprefixed_keys_to.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_array_visit_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_collapse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_dot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.2/tests/test_exists.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_filter_prefixed.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_first.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_flatten.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_forget.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_get.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_has.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_insert_after_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_insert_before_key.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_is_dict.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_is_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_join.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_last.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_list_to_array.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_merge_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_only.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_prepend.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_pull.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_query.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_random.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_recursive_ksort.py
--rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_set.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_shape_filter.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_shuffle.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_sort_by_priority.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_sort_recursive.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_stringify_keys.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_strpos.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_to_list.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_undot.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_usearch.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_where.py
--rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_where_not_none.py
--rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.2/tests/test_wrap.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1075 2024-04-27 13:08:28.000000 arrayutilities-1.0.3/LICENSE
+-rw-r--r--   0 matt      (1000) matt      (1000)    18918 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)    17127 2024-04-27 17:47:07.000000 arrayutilities-1.0.3/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.233993 arrayutilities-1.0.3/arrayutilities/
+-rw-r--r--   0 matt      (1000) matt      (1000)    25579 2024-04-27 17:13:16.000000 arrayutilities-1.0.3/arrayutilities/__init__.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/arrayutilities.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    18918 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1223 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       21 2024-04-27 17:49:42.000000 arrayutilities-1.0.3/arrayutilities.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      664 2024-04-27 17:49:09.000000 arrayutilities-1.0.3/pyproject.toml
+-rw-r--r--   0 matt      (1000) matt      (1000)       38 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/setup.cfg
+-rw-r--r--   0 matt      (1000) matt      (1000)      393 2024-04-27 17:49:13.000000 arrayutilities-1.0.3/setup.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2024-04-27 17:49:42.243993 arrayutilities-1.0.3/tests/
+-rw-r--r--   0 matt      (1000) matt      (1000)        0 2024-04-27 13:11:34.000000 arrayutilities-1.0.3/tests/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      818 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_accessible.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      968 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1312 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add_prefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1321 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_add_unprefixed_keys_to.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1589 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_array_visit_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1155 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_collapse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1536 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_dot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1559 2024-04-27 17:38:47.000000 arrayutilities-1.0.3/tests/test_exists.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1585 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_filter_prefixed.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1463 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_first.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     2058 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_flatten.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1634 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_forget.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1862 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_get.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1456 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_has.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1368 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_insert_after_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1389 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_insert_before_key.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1288 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_is_dict.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1035 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_is_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1695 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_join.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1666 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_last.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1642 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_list_to_array.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1699 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_merge_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1530 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_only.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1445 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_prepend.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1481 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_pull.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1658 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_query.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1448 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_random.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1106 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_recursive_ksort.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      998 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_set.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1103 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_shape_filter.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1045 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_shuffle.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1475 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_sort_by_priority.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1350 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_sort_recursive.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1076 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_stringify_keys.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1502 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_strpos.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1249 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_to_list.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1472 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_undot.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1216 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_usearch.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1303 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_where.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      996 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_where_not_none.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      903 2024-04-27 17:38:46.000000 arrayutilities-1.0.3/tests/test_wrap.py
```

### Comparing `arrayutilities-1.0.2/LICENSE` & `arrayutilities-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/PKG-INFO` & `arrayutilities-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/borkweb/python-arrayutilities
-Keywords: pipeline,library
+Keywords: list,dict,UserDict,library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `arrayutilities-1.0.2/README.md` & `arrayutilities-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/arrayutilities/__init__.py` & `arrayutilities-1.0.3/arrayutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/arrayutilities.egg-info/PKG-INFO` & `arrayutilities-1.0.3/arrayutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayutilities
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for list, dict, and UserDict manipulations.
 Author: Matthew Batchelder
 Author-email: Matthew Batchelder <borkweb@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew Batchelder
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/borkweb/python-arrayutilities
-Keywords: pipeline,library
+Keywords: list,dict,UserDict,library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `arrayutilities-1.0.2/arrayutilities.egg-info/SOURCES.txt` & `arrayutilities-1.0.3/arrayutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_accessible.py` & `arrayutilities-1.0.3/tests/test_accessible.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_add.py` & `arrayutilities-1.0.3/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_add_prefixed_keys_to.py` & `arrayutilities-1.0.3/tests/test_add_prefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_add_unprefixed_keys_to.py` & `arrayutilities-1.0.3/tests/test_add_unprefixed_keys_to.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_array_visit_recursive.py` & `arrayutilities-1.0.3/tests/test_array_visit_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_collapse.py` & `arrayutilities-1.0.3/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_dot.py` & `arrayutilities-1.0.3/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_exists.py` & `arrayutilities-1.0.3/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_filter_prefixed.py` & `arrayutilities-1.0.3/tests/test_filter_prefixed.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_first.py` & `arrayutilities-1.0.3/tests/test_first.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_flatten.py` & `arrayutilities-1.0.3/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_forget.py` & `arrayutilities-1.0.3/tests/test_forget.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_get.py` & `arrayutilities-1.0.3/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_has.py` & `arrayutilities-1.0.3/tests/test_has.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_insert_after_key.py` & `arrayutilities-1.0.3/tests/test_insert_after_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_insert_before_key.py` & `arrayutilities-1.0.3/tests/test_insert_before_key.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_is_dict.py` & `arrayutilities-1.0.3/tests/test_is_dict.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_is_list.py` & `arrayutilities-1.0.3/tests/test_is_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_join.py` & `arrayutilities-1.0.3/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_last.py` & `arrayutilities-1.0.3/tests/test_last.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_list_to_array.py` & `arrayutilities-1.0.3/tests/test_list_to_array.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_merge_recursive.py` & `arrayutilities-1.0.3/tests/test_merge_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_only.py` & `arrayutilities-1.0.3/tests/test_only.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_prepend.py` & `arrayutilities-1.0.3/tests/test_prepend.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_pull.py` & `arrayutilities-1.0.3/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_query.py` & `arrayutilities-1.0.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_random.py` & `arrayutilities-1.0.3/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_recursive_ksort.py` & `arrayutilities-1.0.3/tests/test_recursive_ksort.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_set.py` & `arrayutilities-1.0.3/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_shape_filter.py` & `arrayutilities-1.0.3/tests/test_shape_filter.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_shuffle.py` & `arrayutilities-1.0.3/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_sort_by_priority.py` & `arrayutilities-1.0.3/tests/test_sort_by_priority.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_sort_recursive.py` & `arrayutilities-1.0.3/tests/test_sort_recursive.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_stringify_keys.py` & `arrayutilities-1.0.3/tests/test_stringify_keys.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_strpos.py` & `arrayutilities-1.0.3/tests/test_strpos.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_to_list.py` & `arrayutilities-1.0.3/tests/test_to_list.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_undot.py` & `arrayutilities-1.0.3/tests/test_undot.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_usearch.py` & `arrayutilities-1.0.3/tests/test_usearch.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_where.py` & `arrayutilities-1.0.3/tests/test_where.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_where_not_none.py` & `arrayutilities-1.0.3/tests/test_where_not_none.py`

 * *Files identical despite different names*

### Comparing `arrayutilities-1.0.2/tests/test_wrap.py` & `arrayutilities-1.0.3/tests/test_wrap.py`

 * *Files identical despite different names*

