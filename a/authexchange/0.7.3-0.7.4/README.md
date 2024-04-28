# Comparing `tmp/authexchange-0.7.3.tar.gz` & `tmp/authexchange-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authexchange-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "authexchange-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `authexchange-0.7.3.tar` & `authexchange-0.7.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-04-28 18:39:30.428357 authexchange-0.7.3/LICENSE
--rw-r--r--   0        0        0       77 2024-04-28 18:39:30.428357 authexchange-0.7.3/README.md
--rw-r--r--   0        0        0      616 2024-04-28 18:39:30.440357 authexchange-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/__init__.py
--rw-r--r--   0        0        0     2131 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/__main__.py
--rw-r--r--   0        0        0       97 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/__init__.py
--rw-r--r--   0        0        0      762 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/__init__.py
--rw-r--r--   0        0        0       60 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/callback.py
--rw-r--r--   0        0        0      824 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/logout.py
--rw-r--r--   0        0        0     2207 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/refresh.py
--rw-r--r--   0        0        0     1688 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/signup_login.py
--rw-r--r--   0        0        0      538 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/user.py
--rw-r--r--   0        0        0      216 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/blueprints/ping/__init__.py
--rw-r--r--   0        0        0      617 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/config.py
--rw-r--r--   0        0        0     1499 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/server.py
--rw-r--r--   0        0        0        0 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/utils/__init__.py
--rw-r--r--   0        0        0      346 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/utils/b64.py
--rw-r--r--   0        0        0      337 2024-04-28 18:39:30.440357 authexchange-0.7.3/src/authexchange/utils/state.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 authexchange-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-28 19:04:00.210506 authexchange-0.7.4/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-28 19:04:00.210506 authexchange-0.7.4/README.md
+-rw-r--r--   0        0        0      616 2024-04-28 19:04:00.222506 authexchange-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/__init__.py
+-rw-r--r--   0        0        0     2131 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/__main__.py
+-rw-r--r--   0        0        0       97 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/__init__.py
+-rw-r--r--   0        0        0     2245 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/callback.py
+-rw-r--r--   0        0        0      824 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/logout.py
+-rw-r--r--   0        0        0     2207 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/refresh.py
+-rw-r--r--   0        0        0     1688 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/signup_login.py
+-rw-r--r--   0        0        0      538 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/user.py
+-rw-r--r--   0        0        0      216 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/blueprints/ping/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/config.py
+-rw-r--r--   0        0        0     1499 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/server.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/utils/__init__.py
+-rw-r--r--   0        0        0      346 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/utils/b64.py
+-rw-r--r--   0        0        0      337 2024-04-28 19:04:00.222506 authexchange-0.7.4/src/authexchange/utils/state.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 authexchange-0.7.4/PKG-INFO
```

### Comparing `authexchange-0.7.3/LICENSE` & `authexchange-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/pyproject.toml` & `authexchange-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/__main__.py` & `authexchange-0.7.4/src/authexchange/__main__.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/__init__.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/callback.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/callback.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/logout.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/logout.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/refresh.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/refresh.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/signup_login.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/signup_login.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/blueprints/auth/controllers/user.py` & `authexchange-0.7.4/src/authexchange/blueprints/auth/controllers/user.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/config.py` & `authexchange-0.7.4/src/authexchange/config.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/src/authexchange/server.py` & `authexchange-0.7.4/src/authexchange/server.py`

 * *Files identical despite different names*

### Comparing `authexchange-0.7.3/PKG-INFO` & `authexchange-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authexchange
-Version: 0.7.3
+Version: 0.7.4
 Summary: A server to handle the OAuth token exchange with FusionAuth.
 Author-email: Robert Adams <r0b4dams@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: Flask ~= 3.0.3
 Requires-Dist: Flask-Cors ~= 4.0.0
 Requires-Dist: gunicorn ~= 22.0.0
```

