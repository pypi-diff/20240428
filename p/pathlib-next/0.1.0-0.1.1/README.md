# Comparing `tmp/pathlib_next-0.1.0.tar.gz` & `tmp/pathlib_next-0.1.1.tar.gz`

## Comparing `pathlib_next-0.1.0.tar` & `pathlib_next-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0    18417 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15174 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/example.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15174 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/tests/test_local.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.1/PKG-INFO
```

### Comparing `pathlib_next-0.1.0/src/example.py` & `pathlib_next-0.1.1/src/example.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/fspath.py` & `pathlib_next-0.1.1/src/pathlib_next/fspath.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,34 +70,13 @@
             dironly = (
                 isinstance(pattern, str)
                 and pattern
                 and pattern[-1] in self._path_separators
             )
         yield from _proto.Path.glob(
             self,
-            self,
             pattern,
             case_sensitive=case_sensitive,
             include_hidden=include_hidden,
             recursive=recursive,
             dironly=dironly,
-        )
-
-    def rglob(
-        self,
-        pattern: str,
-        *,
-        case_sensitive: bool = None,
-        include_hidden: bool = False,
-        dironly: bool = False,
-    ):
-        """Recursively yield all existing files (of any kind, including
-        directories) matching the given relative pattern, anywhere in
-        this subtree.
-        """
-        yield from self.glob(
-            pattern,
-            case_sensitive=case_sensitive,
-            include_hidden=include_hidden,
-            recursive=True,
-            dironly=dironly,
-        )
+        )
```

### Comparing `pathlib_next-0.1.0/src/pathlib_next/path.py` & `pathlib_next-0.1.1/src/pathlib_next/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,34 +412,14 @@
             self / pattern,
             case_sensitive=case_sensitive,
             include_hidden=include_hidden,
             recursive=recursive,
             dironly=dironly,
         )
 
-    def rglob(
-        self,
-        pattern: str | _ty.Self,
-        *,
-        case_sensitive: bool = None,
-        include_hidden: bool = False,
-        dironly: bool = None,
-    ):
-        """Recursively yield all existing files (of any kind, including
-        directories) matching the given relative pattern, anywhere in
-        this subtree.
-        """
-        yield from self.glob(
-            pattern,
-            case_sensitive=case_sensitive,
-            include_hidden=include_hidden,
-            recursive=True,
-            dironly=dironly,
-        )
-
     def walk(
         self,
         top_down=True,
         on_error: _ty.Callable[[OSError], None] = None,
         follow_symlinks=False,
     ):
         """Walk the directory tree from this directory, similar to os.walk()."""
```

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/query.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/source.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.1.1/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.1.1/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/utils/glob.py` & `pathlib_next-0.1.1/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/utils/stat.py` & `pathlib_next-0.1.1/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/src/pathlib_next/utils/sync.py` & `pathlib_next-0.1.1/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/tests/test_local.py` & `pathlib_next-0.1.1/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/tests/test_uri.py` & `pathlib_next-0.1.1/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/LICENSE` & `pathlib_next-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.0/pyproject.toml` & `pathlib_next-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.1.0/PKG-INFO` & `pathlib_next-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

