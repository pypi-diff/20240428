# Comparing `tmp/flet_contrib_runtime-2024.4.27.2303.tar.gz` & `tmp/flet_contrib_runtime-2024.4.27.2315.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_runtime-2024.4.27.2303.tar", max compression
+gzip compressed data, was "flet_contrib_runtime-2024.4.27.2315.tar", max compression
```

## Comparing `flet_contrib_runtime-2024.4.27.2303.tar` & `flet_contrib_runtime-2024.4.27.2315.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      204 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/README.md
--rw-r--r--   0        0        0      702 2024-04-27 23:03:53.683584 flet_contrib_runtime-2024.4.27.2303/pyproject.toml
--rw-r--r--   0        0        0      242 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    15878 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/app.py
--rw-r--r--   0        0        0      252 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0      493 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8684 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
--rw-r--r--   0        0        0      560 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
--rw-r--r--   0        0        0     2066 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1264 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
--rw-r--r--   0        0        0      571 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     9278 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1806 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0     7402 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/flet_socket_server.py
--rw-r--r--   0        0        0     2163 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/security/__init__.py
--rw-r--r--   0        0        0     1587 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/uploads.py
--rw-r--r--   0        0        0     4787 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__init__.py
--rw-r--r--   0        0        0     6018 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      743 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
--rw-r--r--   0        0        0     2719 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
--rw-r--r--   0        0        0      347 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/once.py
--rw-r--r--   0        0        0     3202 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/patch_index.py
--rw-r--r--   0        0        0      103 2024-04-27 23:03:01.623865 flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.4.27.2303/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/README.md
+-rw-r--r--   0        0        0      702 2024-04-27 23:15:46.812263 flet_contrib_runtime-2024.4.27.2315/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    15878 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/app.py
+-rw-r--r--   0        0        0      252 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8684 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
+-rw-r--r--   0        0        0      560 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
+-rw-r--r--   0        0        0     2066 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1264 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
+-rw-r--r--   0        0        0      571 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     9278 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1806 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0     7402 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/flet_socket_server.py
+-rw-r--r--   0        0        0     2163 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/security/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/uploads.py
+-rw-r--r--   0        0        0     4787 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6018 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      743 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
+-rw-r--r--   0        0        0     2719 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
+-rw-r--r--   0        0        0      347 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/once.py
+-rw-r--r--   0        0        0     3202 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/patch_index.py
+-rw-r--r--   0        0        0      103 2024-04-27 23:14:57.487631 flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.4.27.2315/PKG-INFO
```

### Comparing `flet_contrib_runtime-2024.4.27.2303/pyproject.toml` & `flet_contrib_runtime-2024.4.27.2315/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-runtime"
-version = "2024.04.27.2303"
+version = "2024.04.27.2315"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-flet-contrib-core = "2024.04.27.2303"
+flet-contrib-core = "2024.04.27.2315"
 oauthlib = "^3.2.2"
 httpx = "^0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/app.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/app.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/authorization.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/oauth_provider.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/oauth_token.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/flet_socket_server.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/flet_socket_server.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/security/__init__.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/security/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/uploads.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/uploads.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__init__.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/src/flet_runtime/utils/patch_index.py` & `flet_contrib_runtime-2024.4.27.2315/src/flet_runtime/utils/patch_index.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.4.27.2303/PKG-INFO` & `flet_contrib_runtime-2024.4.27.2315/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-contrib-runtime
-Version: 2024.4.27.2303
+Version: 2024.4.27.2315
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flet-contrib-core (==2024.04.27.2303)
+Requires-Dist: flet-contrib-core (==2024.04.27.2315)
 Requires-Dist: httpx (>=0,<1)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```

