# Comparing `tmp/lnurl_nostr1-0.5.0rc1.tar.gz` & `tmp/lnurl_nostr1-0.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl_nostr1-0.5.0rc1.tar", max compression
+gzip compressed data, was "lnurl_nostr1-0.5.0rc2.tar", max compression
```

## Comparing `lnurl_nostr1-0.5.0rc1.tar` & `lnurl_nostr1-0.5.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.0rc1/LICENSE
--rwxr-xr-x   0        0        0     6248 2024-04-28 16:18:32.818930 lnurl_nostr1-0.5.0rc1/README.md
--rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.0rc1/lnurl/__init__.py
--rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.0rc1/lnurl/cli.py
--rw-r--r--   0        0        0     4885 2024-04-28 16:18:44.299319 lnurl_nostr1-0.5.0rc1/lnurl/core.py
--rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.0rc1/lnurl/exceptions.py
--rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.0rc1/lnurl/helpers.py
--rw-r--r--   0        0        0     5568 2024-04-28 16:18:44.300097 lnurl_nostr1-0.5.0rc1/lnurl/models.py
--rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.0rc1/lnurl/py.typed
--rw-r--r--   0        0        0     9769 2024-04-28 16:18:44.300678 lnurl_nostr1-0.5.0rc1/lnurl/types.py
--rw-r--r--   0        0        0     1879 2024-04-28 16:18:36.267855 lnurl_nostr1-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7014 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-04-28 13:26:56.996166 lnurl_nostr1-0.5.0rc2/LICENSE
+-rwxr-xr-x   0        0        0     6290 2024-04-28 16:27:06.935463 lnurl_nostr1-0.5.0rc2/README.md
+-rw-r--r--   0        0        0      816 2024-04-28 13:26:56.996790 lnurl_nostr1-0.5.0rc2/lnurl/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-04-28 13:26:56.996959 lnurl_nostr1-0.5.0rc2/lnurl/cli.py
+-rw-r--r--   0        0        0     4885 2024-04-28 16:18:44.299319 lnurl_nostr1-0.5.0rc2/lnurl/core.py
+-rw-r--r--   0        0        0      486 2024-04-28 13:26:56.997326 lnurl_nostr1-0.5.0rc2/lnurl/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-04-28 13:26:56.997479 lnurl_nostr1-0.5.0rc2/lnurl/helpers.py
+-rw-r--r--   0        0        0     5568 2024-04-28 16:18:44.300097 lnurl_nostr1-0.5.0rc2/lnurl/models.py
+-rw-r--r--   0        0        0       26 2024-04-28 13:26:56.997833 lnurl_nostr1-0.5.0rc2/lnurl/py.typed
+-rw-r--r--   0        0        0     9769 2024-04-28 16:18:44.300678 lnurl_nostr1-0.5.0rc2/lnurl/types.py
+-rw-r--r--   0        0        0     1937 2024-04-28 16:30:57.969556 lnurl_nostr1-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 lnurl_nostr1-0.5.0rc2/PKG-INFO
```

### Comparing `lnurl_nostr1-0.5.0rc1/LICENSE` & `lnurl_nostr1-0.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/README.md` & `lnurl_nostr1-0.5.0rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: lnurl_nostr1
+Version: 0.5.0rc2
+Summary: LNURL implementation for Python, with support for future nostr1 protocol.
+License: MIT
+Author: Alan Bits
+Author-email: alan@lnbits.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bech32 (>=1.2.0,<2.0.0)
+Requires-Dist: bolt11 (>=2.0.5,<3.0.0)
+Requires-Dist: ecdsa (>=0.19.0,<0.20.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: pydantic (>=1,<2)
+Description-Content-Type: text/markdown
+
 LNURL implementation for Python
 ===============================
 
 [![github-tests-badge]][github-tests]
 [![github-mypy-badge]][github-mypy]
 [![codecov-badge]][codecov]
 [![pypi-badge]][pypi]
@@ -74,23 +95,23 @@
 r = requests.get(lnurl.url)
 ```
 
 If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
->>> import lnurl
->>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
+>>> import lnurl_nostr1
+>>> lnurl_nostr1.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
 You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
 ```python
->>> import lnurl
->>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+>>> import lnurl_nostr1
+>>> lnurl_nostr1.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
 ```
 
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
 
@@ -134,21 +155,22 @@
 [lnurl-spec]: https://github.com/btcontract/lnurl-rfc/blob/master/spec.md
 [pydantic]: https://github.com/samuelcolvin/pydantic/
 
 
 CLI
 ---------
 ```console
-$ poetry run lnurl
-Usage: lnurl [OPTIONS] COMMAND [ARGS]...
+$ poetry run lnurl_nostr1
+Usage: lnurl_nostr1 [OPTIONS] COMMAND [ARGS]...
 
   Python CLI for LNURL decode and encode lnurls
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   decode           decode a LNURL
   encode           encode a URL
   handle           handle a LNURL
   execute          execute a LNURL
 ```
+
```

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/__init__.py` & `lnurl_nostr1-0.5.0rc2/lnurl/__init__.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/cli.py` & `lnurl_nostr1-0.5.0rc2/lnurl/cli.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/core.py` & `lnurl_nostr1-0.5.0rc2/lnurl/core.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/helpers.py` & `lnurl_nostr1-0.5.0rc2/lnurl/helpers.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/models.py` & `lnurl_nostr1-0.5.0rc2/lnurl/models.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/lnurl/types.py` & `lnurl_nostr1-0.5.0rc2/lnurl/types.py`

 * *Files identical despite different names*

### Comparing `lnurl_nostr1-0.5.0rc1/pyproject.toml` & `lnurl_nostr1-0.5.0rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "lnurl_nostr1"
-version = "0.5.0rc1"
+version = "0.5.0rc2"
 description = "LNURL implementation for Python, with support for future nostr1 protocol."
 authors = ["Alan Bits <alan@lnbits.com>", "Oren <orenz0@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
-  {include = "lnurl"},
-  {include = "lnurl/py.typed"},
+  {include = "lnurl", to = "lnurl_nostr1"},
+  {include = "lnurl/py.typed", to = "lnurl_nostr1/py.typed"},
 ]
 
 [tool.poetry.scripts]
-lnurl = "lnurl.cli:main"
+lnurl = "lnurl_nostr1.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1"
 bech32 = "^1.2.0"
 ecdsa = "^0.19.0"
 bolt11 = "^2.0.5"
```

### Comparing `lnurl_nostr1-0.5.0rc1/PKG-INFO` & `lnurl_nostr1-0.5.0rc2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: lnurl_nostr1
-Version: 0.5.0rc1
-Summary: LNURL implementation for Python, with support for future nostr1 protocol.
-License: MIT
-Author: Alan Bits
-Author-email: alan@lnbits.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bech32 (>=1.2.0,<2.0.0)
-Requires-Dist: bolt11 (>=2.0.5,<3.0.0)
-Requires-Dist: ecdsa (>=0.19.0,<0.20.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: pydantic (>=1,<2)
-Description-Content-Type: text/markdown
-
 LNURL implementation for Python
 ===============================
 
 [![github-tests-badge]][github-tests]
 [![github-mypy-badge]][github-mypy]
 [![codecov-badge]][codecov]
 [![pypi-badge]][pypi]
@@ -95,23 +74,23 @@
 r = requests.get(lnurl.url)
 ```
 
 If you have already `httpx` installed, you can also use the `.handle()` function directly.
 It will return the appropriate response for a LNURL.
 
 ```python
->>> import lnurl
->>> lnurl.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
+>>> import lnurl_nostr1
+>>> lnurl_nostr1.handle('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF')
 LnurlPayResponse(tag='payRequest', callback=WebUrl('https://lnurl.bigsun.xyz/lnurl-pay/callback/2169831', scheme='https', host='lnurl.bigsun.xyz', tld='xyz', host_type='domain', path='/lnurl-pay/callback/2169831'), min_sendable=10000, max_sendable=10000, metadata=LnurlPayMetadata('[["text/plain","NgHaEyaZNDnW iI DsFYdkI"],["image/png;base64","iVBOR...uQmCC"]]'))
 ```
 
 You can execute and LNURL with either payRequest, withdrawRequest or login tag using the `execute` function.
 ```python
->>> import lnurl
->>> lnurl.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
+>>> import lnurl_nostr1
+>>> lnurl_nostr1.execute('lightning:LNURL1DP68GURN8GHJ7MRWW4EXCTNZD9NHXATW9EU8J730D3H82UNV94CXZ7FLWDJHXUMFDAHR6V33XCUNSVE38QV6UF', 100000)
 ```
 
 Building your own LNURL responses
 ---------------------------------
 
 For LNURL services, the `lnurl` package can be used to build **valid** responses.
 
@@ -155,22 +134,21 @@
 [lnurl-spec]: https://github.com/btcontract/lnurl-rfc/blob/master/spec.md
 [pydantic]: https://github.com/samuelcolvin/pydantic/
 
 
 CLI
 ---------
 ```console
-$ poetry run lnurl
-Usage: lnurl [OPTIONS] COMMAND [ARGS]...
+$ poetry run lnurl_nostr1
+Usage: lnurl_nostr1 [OPTIONS] COMMAND [ARGS]...
 
   Python CLI for LNURL decode and encode lnurls
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   decode           decode a LNURL
   encode           encode a URL
   handle           handle a LNURL
   execute          execute a LNURL
 ```
-
```

