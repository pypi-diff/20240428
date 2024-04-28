# Comparing `tmp/certificate_watcher-0.1.1.tar.gz` & `tmp/certificate_watcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certificate_watcher-0.1.1.tar", last modified: Mon Oct  3 17:06:54 2022, max compression
+gzip compressed data, was "certificate_watcher-0.2.0.tar", last modified: Sun Apr 28 20:10:53 2024, max compression
```

## Comparing `certificate_watcher-0.1.1.tar` & `certificate_watcher-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-10-03 17:06:54.476503 certificate_watcher-0.1.1/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2069 2022-10-03 17:06:54.476503 certificate_watcher-0.1.1/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1420 2022-10-02 20:14:18.000000 certificate_watcher-0.1.1/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-10-03 17:06:54.476503 certificate_watcher-0.1.1/certificate_watcher.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2069 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      307 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       65 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       13 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       20 2022-10-03 17:06:54.000000 certificate_watcher-0.1.1/certificate_watcher.egg-info/top_level.txt
--rwxr-xr-x   0 mdk       (1000) mdk       (1000)     7339 2022-10-03 17:06:05.000000 certificate_watcher-0.1.1/certificate_watcher.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1109 2022-10-02 20:14:17.000000 certificate_watcher-0.1.1/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2022-10-03 17:06:54.476503 certificate_watcher-0.1.1/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-28 20:10:53.293398 certificate_watcher-0.2.0/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2054 2024-04-28 20:10:53.293398 certificate_watcher-0.2.0/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1377 2024-04-28 19:54:32.000000 certificate_watcher-0.2.0/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-28 20:10:53.293398 certificate_watcher-0.2.0/certificate_watcher.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2054 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      353 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       65 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       13 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       20 2024-04-28 20:10:53.000000 certificate_watcher-0.2.0/certificate_watcher.egg-info/top_level.txt
+-rwxr-xr-x   0 mdk       (1000) mdk       (1000)     7255 2024-04-28 19:55:21.000000 certificate_watcher-0.2.0/certificate_watcher.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1103 2024-04-28 19:48:21.000000 certificate_watcher-0.2.0/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2024-04-28 20:10:53.293398 certificate_watcher-0.2.0/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-28 20:10:53.293398 certificate_watcher-0.2.0/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      706 2022-10-03 16:57:33.000000 certificate_watcher-0.2.0/tests/test_badssl.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      690 2024-04-28 19:51:13.000000 certificate_watcher-0.2.0/tests/test_parse_spec.py
```

### Comparing `certificate_watcher-0.1.1/PKG-INFO` & `certificate_watcher-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: certificate_watcher
-Version: 0.1.1
+Version: 0.2.0
 Summary: Watch expiration of certificates of a bunch of websites.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
 Project-URL: homepage, https://github.com/JulienPalard/certificate_watcher
 Keywords: ssl,tls,certificate,https,watch,sysadmin,cron,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: ocsp-checker
 
 Lists expiration time of soon-to-be expired ssl certificates of all
 given domains like:
 
    ./certificate_watcher.py mdk.fr python.org duckduckgo.com
    mdk.fr:Certificate expires in 2 days
 
@@ -36,18 +37,16 @@
 
 A domain to be resolved can be used in this field to, like:
 
 ```
 ./certificate_watcher.py example.com@backend1.example.com example.com@backend2.example.com
 ```
 
-
-The `@host` and `:port` have no specific order, both
-`example.com:443@127.0.0.1` and `example.com@127.0.0.1:443` mean the
-same test.
+The `:port` must appear before `@host`, like:
+`example.com:443@fe80::5c5b:9f32:13b1:29c3`.
 
 Exemple domain file:
 
 ```
 # Our project
 example.com
 www.example.com
```

### Comparing `certificate_watcher-0.1.1/README.md` & `certificate_watcher-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 
 A domain to be resolved can be used in this field to, like:
 
 ```
 ./certificate_watcher.py example.com@backend1.example.com example.com@backend2.example.com
 ```
 
-
-The `@host` and `:port` have no specific order, both
-`example.com:443@127.0.0.1` and `example.com@127.0.0.1:443` mean the
-same test.
+The `:port` must appear before `@host`, like:
+`example.com:443@fe80::5c5b:9f32:13b1:29c3`.
 
 Exemple domain file:
 
 ```
 # Our project
 example.com
 www.example.com
```

### Comparing `certificate_watcher-0.1.1/certificate_watcher.egg-info/PKG-INFO` & `certificate_watcher-0.2.0/certificate_watcher.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: certificate-watcher
-Version: 0.1.1
+Name: certificate_watcher
+Version: 0.2.0
 Summary: Watch expiration of certificates of a bunch of websites.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
 Project-URL: homepage, https://github.com/JulienPalard/certificate_watcher
 Keywords: ssl,tls,certificate,https,watch,sysadmin,cron,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: ocsp-checker
 
 Lists expiration time of soon-to-be expired ssl certificates of all
 given domains like:
 
    ./certificate_watcher.py mdk.fr python.org duckduckgo.com
    mdk.fr:Certificate expires in 2 days
 
@@ -36,18 +37,16 @@
 
 A domain to be resolved can be used in this field to, like:
 
 ```
 ./certificate_watcher.py example.com@backend1.example.com example.com@backend2.example.com
 ```
 
-
-The `@host` and `:port` have no specific order, both
-`example.com:443@127.0.0.1` and `example.com@127.0.0.1:443` mean the
-same test.
+The `:port` must appear before `@host`, like:
+`example.com:443@fe80::5c5b:9f32:13b1:29c3`.
 
 Exemple domain file:
 
 ```
 # Our project
 example.com
 www.example.com
```

### Comparing `certificate_watcher-0.1.1/certificate_watcher.py` & `certificate_watcher-0.2.0/certificate_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python3
 
-"""Prints (on stderr) the list and expiration time ssl certificats of
+"""Prints (on stderr) the list and expiration time ssl certificates of
 all given domains like:
 
-   ./warn_expire.py mdk.fr python.org duckduckgo.com
+   certificate_watcher mdk.fr python.org duckduckgo.com
    mdk.fr expire in 2 days
 
 """
 
 import argparse
 import csv
 import re
 import socket
 import ssl
 import sys
 from datetime import datetime, timedelta
 
 from ocspchecker import ocspchecker
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 def get_server_certificate(service, timeout=10):
     """Retrieve the certificate from the server at the specified address" """
     context = ssl.create_default_context()
     context.options &= ssl.CERT_REQUIRED
     context.check_hostname = True
@@ -107,37 +107,45 @@
         s2 = Service("example.com@10.1.0.2")
 
     A domain name, to be resolved, can be used in this field too, like:
 
         s1 = Service("example.com@backend1.example.com")
         s2 = Service("example.com@backend2.example.com")
 
-    The `@host` and `:port` have no specific order, both
-    "example.com:443@127.0.0.1" and "example.com@127.0.0.1:443" are
-    parsed equally.
+    Beware, the port is only parsed on the host part, so:
+
+        example.com:443@127.0.0.1
+
+    is valid while:
+
+        example.com@127.0.0.1:443
+
+    is not.
+
+    This is to disambiguate IPv6, this is not ambiguous:
+
+        example.com:443@::1
+
+    while this is:
+
+        example.com@::1:443
     """
 
-    SPEC = "(?P<ip>@[^@:]+)|(?P<port>:[^@:]+)|(?P<hostname>[^@:]+)"
+    SPEC = "(?P<hostname>[^@:]+)(?P<port>:[0-9]+)?(?P<ip>@[0-9a-fA-F.:]+)?"
 
     def __init__(self, description):
         self.description = description
         self.ip_addr = None
         self.port = 443
-        self.hostname = None
-        for token in re.finditer(Service.SPEC, description):
-            kind = token.lastgroup
-            value = token.group()
-            if kind == "ip":
-                self.ip_addr = value[1:]
-            if kind == "port":
-                self.port = int(value[1:])
-            if kind == "hostname":
-                self.hostname = value
-        if self.hostname is None:
-            raise ValueError("A service cannot have no hostname.")
+        spec = re.match(Service.SPEC, description)
+        self.hostname = spec["hostname"]
+        if spec["port"]:
+            self.port = int(spec["port"][1:])
+        if spec["ip"]:
+            self.ip_addr = spec["ip"][1:]
 
     def __repr__(self):
         return self.description
 
     @property
     def address(self):
         """Return a 2-tuple (host, port).
```

### Comparing `certificate_watcher-0.1.1/pyproject.toml` & `certificate_watcher-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.2"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "certificate_watcher"
 description = "Watch expiration of certificates of a bunch of websites."
 authors = [{name = "Julien Palard", email = "julien@palard.fr"}]
 license = {text = "MIT license"}
```

