# Comparing `tmp/ndarraybuffer-0.1.1.tar.gz` & `tmp/ndarraybuffer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndarraybuffer-0.1.1.tar", max compression
+gzip compressed data, was "ndarraybuffer-0.1.2.tar", max compression
```

## Comparing `ndarraybuffer-0.1.1.tar` & `ndarraybuffer-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1106 2024-03-12 03:13:22.711535 ndarraybuffer-0.1.1/README.md
--rw-r--r--   0        0        0       51 2024-03-12 02:51:07.154122 ndarraybuffer-0.1.1/ndarraybuffer/__init__.py
--rw-r--r--   0        0        0     8867 2024-03-12 03:41:02.969393 ndarraybuffer-0.1.1/ndarraybuffer/array_buffer.py
--rw-r--r--   0        0        0        0 2024-03-12 03:05:05.461557 ndarraybuffer-0.1.1/ndarraybuffer/py.typed
--rw-r--r--   0        0        0      556 2024-03-12 03:42:06.433194 ndarraybuffer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 ndarraybuffer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1106 2024-03-12 03:13:22.711535 ndarraybuffer-0.1.2/README.md
+-rw-r--r--   0        0        0       51 2024-03-12 02:51:07.154122 ndarraybuffer-0.1.2/ndarraybuffer/__init__.py
+-rw-r--r--   0        0        0     8913 2024-04-28 09:49:09.791567 ndarraybuffer-0.1.2/ndarraybuffer/array_buffer.py
+-rw-r--r--   0        0        0        0 2024-03-12 03:05:05.461557 ndarraybuffer-0.1.2/ndarraybuffer/py.typed
+-rw-r--r--   0        0        0      556 2024-04-28 09:50:52.657111 ndarraybuffer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1661 1970-01-01 00:00:00.000000 ndarraybuffer-0.1.2/PKG-INFO
```

### Comparing `ndarraybuffer-0.1.1/README.md` & `ndarraybuffer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ndarraybuffer-0.1.1/ndarraybuffer/array_buffer.py` & `ndarraybuffer-0.1.2/ndarraybuffer/array_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,27 +192,27 @@
         other = np.asarray(other)
         ol = len(other)
 
         self._check_enlarge(Side.RIGHT, ol)
         self._array[self._stop:self._stop + ol] = other[:]
         self._stop += ol
         if self.max_len is not None and len(self) > self.max_len:
-            self.popleft(1)
+            self.popleft(len(self) - self.max_len)
         return self
 
     def extendleft(self, other: ArrayLike) -> Self:
         other = np.asarray(other)
 
         ol = len(other)
 
         self._check_enlarge(Side.LEFT, ol)
         self._array[self._start - ol:self._start] = other[:]
         self._start -= ol
         if self.max_len is not None and len(self) > self.max_len:
-            self.pop(1)
+            self.pop(len(self) - self.max_len)
         return self
 
     def pop(self, count: int) -> NDArray:
 
         count = min(count, len(self))
 
         ret: NDArray = self[-count:]
```

### Comparing `ndarraybuffer-0.1.1/pyproject.toml` & `ndarraybuffer-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ndarraybuffer"
-version = "0.1.1"
+version = "0.1.2"
 description = "NDArray with both-side insertion/deletion and size limit"
 authors = ["Zeyan Li 李则言 <lizeyan.42@bytedance.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = ">=1.21"
-typing-extensions = "^4.10.0"
 
 [tool.poetry.group.dev.dependencies]
+typing-extensions = "^4.10.0"
 pytest = "^8.1.1"
 coverage = "^7.4.3"
 pyprof = ">=1.0.0"
 mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ndarraybuffer-0.1.1/PKG-INFO` & `ndarraybuffer-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ndarraybuffer
-Version: 0.1.1
+Version: 0.1.2
 Summary: NDArray with both-side insertion/deletion and size limit
 License: MIT
 Author: Zeyan Li 李则言
 Author-email: lizeyan.42@bytedance.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.21)
-Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![Coverage badge](https://raw.githubusercontent.com/lizeyan/ndarraybuffer/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/lizeyan/ndarraybuffer/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 ## Introduction
 Wrap `numpy.ndarray` to support fast both-side insertion/deletion and size limit.
```

