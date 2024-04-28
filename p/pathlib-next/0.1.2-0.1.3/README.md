# Comparing `tmp/pathlib_next-0.1.2.tar.gz` & `tmp/pathlib_next-0.1.3.tar.gz`

## Comparing `pathlib_next-0.1.2.tar` & `pathlib_next-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15461 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/example.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/tests/test_local.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.3/PKG-INFO
```

### Comparing `pathlib_next-0.1.2/src/example.py` & `pathlib_next-0.1.3/src/example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,65 @@
-from pathlib_next.uri import UriPath, Query, Source
+from pathlib_next import Path, glob
+from pathlib_next.mempath import MemPath
+from pathlib_next.uri import Query, Source, UriPath
 from pathlib_next.uri.schemes import *
 from pathlib_next.utils.sync import PathSyncer
-from pathlib_next import glob, Path
 
-local = Path('./_ssh')
+mempath = MemPath("test/test3")
+mempath.parent.mkdir(parents=True, exist_ok=True)
+mempath.write_text("test")
+check = mempath.read_text()
+mempath.parent.rm(recursive=True)
+
+pass
+
+local = Path("./_ssh")
 print(list(local.iterdir()))
-query = Query({'test':'://$#!1', 'test2&': [1,2]})
-q2 =  Query(str(query)).to_dict()
+query = Query({"test": "://$#!1", "test2&": [1, 2]})
+q2 = Query(str(query)).to_dict()
 for name, value in query:
     print(f"{name}: {value}")
-src = Source(scheme='scheme',userinfo='user', host='123.com', port=0)
+src = Source(scheme="scheme", userinfo="user", host="123.com", port=0)
 test = {**src}
 test2 = [*src]
-dest = UriPath('file:./_ssh')
+dest = UriPath("file:./_ssh")
 
 #
 # Norm test
 #
-with_dots = UriPath('a/b/c/d/../../test/.')
+with_dots = UriPath("a/b/c/d/../../test/.")
 print(with_dots.normalized_path)
 
-source_host = UriPath('file://test.com/path1/path2/path3/path4')
+source_host = UriPath("file://test.com/path1/path2/path3/path4")
 source_host.is_local()
 
-rel_to  = source_host.relative_to('/path1/path2')
+rel_to = source_host.relative_to("/path1/path2")
 dest = UriPath(dest)
-test_ = UriPath('file:') / 'test'
+test_ = UriPath("file:") / "test"
 empty = UriPath()
 uri = dest.as_uri()
 
-test1 = dest / 'test' / 'test2/'
+test1 = dest / "test" / "test2/"
 print(test1)
 
-sftp_root = UriPath('sftp://root@sftpexample/')
+sftp_root = UriPath("sftp://root@sftpexample/")
 print(sftp_root.as_posix())
-authkeys = sftp_root / 'root/.ssh/authorized_keys'
+authkeys = sftp_root / "root/.ssh/authorized_keys"
 print(authkeys.as_posix())
 
-def checksum(uri:UriPath):
+
+def checksum(uri: UriPath):
     stat = uri.stat()
     return hash(stat.st_size)
-syncer =PathSyncer(checksum, remove_missing=False)
-syncer.sync((sftp_root / 'root/.ssh'), dest, dry_run=True)
 
-rocky_repo = UriPath('http://dl.rockylinux.org/pub')
+
+syncer = PathSyncer(checksum, remove_missing=False)
+syncer.sync((sftp_root / "root/.ssh"), dest, dry_run=True)
+
+rocky_repo = UriPath("http://dl.rockylinux.org/pub")
 
 glob_test = UriPath("file:./**/*.py")
 
 for path in glob.glob(glob_test, recursive=True):
     print(path)
 
 print(rocky_repo.is_dir())
```

### Comparing `pathlib_next-0.1.2/src/pathlib_next/fspath.py` & `pathlib_next-0.1.3/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/path.py` & `pathlib_next-0.1.3/src/pathlib_next/path.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
-import typing as _ty
-import uritools
-import posixpath as _posix
 import pathlib as _pathlib
+import posixpath as _posix
+import typing as _ty
 
+import uritools
 
 if _ty.TYPE_CHECKING:
     from typing import Self
 
 from .. import utils as _utils
+from ..path import Path, Pathname
 from .query import Query
 from .source import Source
 
-from ..path import Path, Pathname
-
 UriLike: _ty.TypeAlias = "str | Uri | os.PathLike"
 
 _NOSOURCE = Source(None, None, None, None)
 
 _U = _ty.TypeVar("_U", bound="Uri")
```

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/query.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/source.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.1.3/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.1.3/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/utils/glob.py` & `pathlib_next-0.1.3/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/utils/stat.py` & `pathlib_next-0.1.3/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/src/pathlib_next/utils/sync.py` & `pathlib_next-0.1.3/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/tests/test_local.py` & `pathlib_next-0.1.3/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/tests/test_uri.py` & `pathlib_next-0.1.3/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/LICENSE` & `pathlib_next-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.2/pyproject.toml` & `pathlib_next-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.1.2/PKG-INFO` & `pathlib_next-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

