# Comparing `tmp/pathlib_next-0.1.3.tar.gz` & `tmp/pathlib_next-0.1.4.tar.gz`

## Comparing `pathlib_next-0.1.3.tar` & `pathlib_next-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/example.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/tests/test_local.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.4/PKG-INFO
```

### Comparing `pathlib_next-0.1.3/src/example.py` & `pathlib_next-0.1.4/src/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib_next import Path, glob
 from pathlib_next.mempath import MemPath
 from pathlib_next.uri import Query, Source, UriPath
 from pathlib_next.uri.schemes import *
 from pathlib_next.utils.sync import PathSyncer
 
-mempath = MemPath("test/test3")
+mempath = MemPath("test/test3") / "subpath"
 mempath.parent.mkdir(parents=True, exist_ok=True)
 mempath.write_text("test")
 check = mempath.read_text()
 mempath.parent.rm(recursive=True)
 
 pass
```

### Comparing `pathlib_next-0.1.3/src/pathlib_next/fspath.py` & `pathlib_next-0.1.4/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/mempath.py` & `pathlib_next-0.1.4/src/pathlib_next/mempath.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import posixpath as _posix
 from io import IOBase
 from urllib.parse import quote as _urlquote
 
-from .path import Path
+from .path import Path, Pathname
 from .utils.stat import FileStat, FileStatLike
 
 
 class MemPathBackend(dict): ...
 
 
 class MemBytesIO(io.BytesIO):
@@ -22,19 +22,41 @@
         return super().close()
 
 
 class MemPath(Path):
 
     __slots__ = ("_backend", "_segments", "_normalized")
 
-    def __init__(self, *segments: str, backend: MemPathBackend = None, **kwargs):
-        self._segments = "/".join(segments).split("/")
+    def __init__(
+        self, *segments: str | Pathname | Path, backend: MemPathBackend = None, **kwargs
+    ):
+        _segments = []
+        _backend = None
+        for segment in segments:
+            if isinstance(segment, MemPath):
+                _segments.extend(segment.segments)
+                _backend = segment.backend
+            elif isinstance(segment, Path):
+                raise NotImplementedError()
+            elif isinstance(segment, Pathname):
+                _segments.extend(segment.segments)
+            else:
+                _segments.append(segment)
+        self._segments = "/".join(_segments).split("/")
+        if _backend and backend is None:
+            backend = _backend
         self._backend = backend if backend is not None else MemPathBackend()
         self._normalized = None
 
+    def __repr__(self):
+        return "{}({!r})".format(type(self).__name__, self.as_uri())
+
+    def __str__(self) -> str:
+        return self.as_uri()
+
     @property
     def backend(self):
         return self._backend
 
     @property
     def normalized(self):
         if self._normalized is None:
```

### Comparing `pathlib_next-0.1.3/src/pathlib_next/path.py` & `pathlib_next-0.1.4/src/pathlib_next/path.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/query.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/source.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.1.4/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.1.4/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/utils/glob.py` & `pathlib_next-0.1.4/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/utils/stat.py` & `pathlib_next-0.1.4/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/src/pathlib_next/utils/sync.py` & `pathlib_next-0.1.4/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/tests/test_local.py` & `pathlib_next-0.1.4/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/tests/test_uri.py` & `pathlib_next-0.1.4/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/LICENSE` & `pathlib_next-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.3/pyproject.toml` & `pathlib_next-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.1.3/PKG-INFO` & `pathlib_next-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

