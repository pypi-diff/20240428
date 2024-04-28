# Comparing `tmp/lnurl_nostr1-0.5.0rc3.tar.gz` & `tmp/lnurl_nostr1-0.5.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl_nostr1-0.5.0rc3.tar", max compression
+gzip compressed data, was "lnurl_nostr1-0.5.0rc4.tar", max compression
```

## Comparing `lnurl_nostr1-0.5.0rc3.tar` & `lnurl_nostr1-0.5.0rc4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.0rc3/LICENSE
--rwxr-xr-x   0        0        0     6290 2024-04-28 16:27:06.935463 lnurl_nostr1-0.5.0rc3/README.md
--rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.0rc3/lnurl/__init__.py
--rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.0rc3/lnurl/cli.py
--rw-r--r--   0        0        0     4885 2024-04-28 16:18:44.299319 lnurl_nostr1-0.5.0rc3/lnurl/core.py
--rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.0rc3/lnurl/exceptions.py
--rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.0rc3/lnurl/helpers.py
--rw-r--r--   0        0        0     5568 2024-04-28 16:18:44.300097 lnurl_nostr1-0.5.0rc3/lnurl/models.py
--rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.0rc3/lnurl/py.typed
--rw-r--r--   0        0        0     9769 2024-04-28 16:18:44.300678 lnurl_nostr1-0.5.0rc3/lnurl/types.py
--rw-r--r--   0        0        0     1911 2024-04-28 16:56:57.606318 lnurl_nostr1-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.0rc4/LICENSE
+-rwxr-xr-x   0        0        0     6290 2024-04-28 16:27:06.935463 lnurl_nostr1-0.5.0rc4/README.md
+-rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.0rc4/lnurl/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.0rc4/lnurl/cli.py
+-rw-r--r--   0        0        0     4885 2024-04-28 16:18:44.299319 lnurl_nostr1-0.5.0rc4/lnurl/core.py
+-rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.0rc4/lnurl/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.0rc4/lnurl/helpers.py
+-rw-r--r--   0        0        0     5568 2024-04-28 16:18:44.300097 lnurl_nostr1-0.5.0rc4/lnurl/models.py
+-rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.0rc4/lnurl/py.typed
+-rw-r--r--   0        0        0     9769 2024-04-28 16:18:44.300678 lnurl_nostr1-0.5.0rc4/lnurl/types.py
+-rw-r--r--   0        0        0     1962 2024-04-28 17:12:29.576749 lnurl_nostr1-0.5.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.0rc4/PKG-INFO
```

### Comparing `lnurl_nostr1-0.5.0rc3/LICENSE` & `lnurl_nostr1-0.5.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/README.md` & `lnurl_nostr1-0.5.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/__init__.py` & `lnurl_nostr1-0.5.0rc4/lnurl/__init__.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/cli.py` & `lnurl_nostr1-0.5.0rc4/lnurl/cli.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/core.py` & `lnurl_nostr1-0.5.0rc4/lnurl/core.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/helpers.py` & `lnurl_nostr1-0.5.0rc4/lnurl/helpers.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/models.py` & `lnurl_nostr1-0.5.0rc4/lnurl/models.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/lnurl/types.py` & `lnurl_nostr1-0.5.0rc4/lnurl/types.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc3/pyproject.toml` & `lnurl_nostr1-0.5.0rc4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "lnurl_nostr1"
-version = "0.5.0rc3"
+version = "0.5.0rc4"
 description = "LNURL implementation for Python, with support for future nostr1 protocol."
 authors = ["Alan Bits <alan@lnbits.com>", "Oren <orenz0@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
-  {include = "*.py", from = "lnurl"},
-  {include = "py.typed", from = "lnurl"},
+  {include = "*.py", from = "lnurl", to = "lnurl_nostr1"},
+  {include = "py.typed", from = "lnurl", to = "lnurl_nostr1/py.typed"},
 ]
 
 [tool.poetry.scripts]
 lnurl = "lnurl_nostr1.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `lnurl_nostr1-0.5.0rc3/PKG-INFO` & `lnurl_nostr1-0.5.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnurl_nostr1
-Version: 0.5.0rc3
+Version: 0.5.0rc4
 Summary: LNURL implementation for Python, with support for future nostr1 protocol.
 License: MIT
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

