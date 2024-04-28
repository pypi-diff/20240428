# Comparing `tmp/realtime_operator-0.2.5.tar.gz` & `tmp/realtime_operator-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.2.5.tar", last modified: Sat Apr 27 22:04:26 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.6.tar", last modified: Sun Apr 28 19:18:38 2024, max compression
```

## Comparing `realtime_operator-0.2.5.tar` & `realtime_operator-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.796687 realtime_operator-0.2.5/
--rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     4367 2024-04-27 22:04:26.794899 realtime_operator-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/README.md
--rw-rw-rw-   0        0        0      695 2024-04-27 22:04:11.000000 realtime_operator-0.2.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.749045 realtime_operator-0.2.5/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0    13309 2024-04-27 21:12:33.000000 realtime_operator-0.2.5/realtime_operator/compression.py
--rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.5/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.787515 realtime_operator-0.2.5/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4367 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 22:04:26.000000 realtime_operator-0.2.5/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 22:04:26.796687 realtime_operator-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 22:04:26.787515 realtime_operator-0.2.5/tests/
--rw-rw-rw-   0        0        0     2720 2024-04-27 21:01:53.000000 realtime_operator-0.2.5/tests/test_compression.py
--rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.5/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.919562 realtime_operator-0.2.6/
+-rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/README.md
+-rw-rw-rw-   0        0        0      695 2024-04-28 19:17:22.000000 realtime_operator-0.2.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.874516 realtime_operator-0.2.6/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0    13298 2024-04-28 19:16:31.000000 realtime_operator-0.2.6/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.6/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 19:18:38.919562 realtime_operator-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/tests/
+-rw-rw-rw-   0        0        0     2805 2024-04-28 19:15:16.000000 realtime_operator-0.2.6/tests/test_compression.py
+-rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.6/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.2.5/LICENSE` & `realtime_operator-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.5/PKG-INFO` & `realtime_operator-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.5/README.md` & `realtime_operator-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.5/pyproject.toml` & `realtime_operator-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "realtime_operator"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `realtime_operator-0.2.5/realtime_operator/compression.py` & `realtime_operator-0.2.6/realtime_operator/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 1:
         state = np.zeros(3, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = minimum_timedelta(delta,state, t[i], z[i],0.0, 1.0e6)
+            tn_ , zn_, cn_ = minimum_timedelta(delta,state, t[i], z[i])
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 2:
         state = np.zeros(3, dtype=float)
         for i in range(n):
```

### Comparing `realtime_operator-0.2.5/realtime_operator/single_operator.py` & `realtime_operator-0.2.6/realtime_operator/single_operator.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.5/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.6/realtime_operator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.5/tests/test_compression.py` & `realtime_operator-0.2.6/tests/test_compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     swinging_door,
 )
 
 t = np.arange(1, 20, dtype=float) + 1
 z = np.arange(1, 20, dtype=float)
 state = np.zeros(4, dtype=float)
 
+def test_any_compression():
+    tn, zn, cn = any_compression(t, z,30.0,0)
+    a=1
 
 def test_interpolate_fast():
     t = np.arange(1, 20,1, dtype=float)
     tn= np.arange(0, 20,0.001, dtype=float) 
 
     zn=interpolate(tn,t,z)
     zm=interpolate_fast(tn,t,z)
```

### Comparing `realtime_operator-0.2.5/tests/test_single_operator.py` & `realtime_operator-0.2.6/tests/test_single_operator.py`

 * *Files identical despite different names*

