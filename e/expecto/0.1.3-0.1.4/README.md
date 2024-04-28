# Comparing `tmp/expecto-0.1.3.tar.gz` & `tmp/expecto-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expecto-0.1.3.tar", last modified: Thu Oct 26 15:50:31 2023, max compression
+gzip compressed data, was "expecto-0.1.4.tar", last modified: Sun Apr 28 18:18:51 2024, max compression
```

## Comparing `expecto-0.1.3.tar` & `expecto-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.772243 expecto-0.1.3/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.761021 expecto-0.1.3/.github/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.764216 expecto-0.1.3/.github/workflows/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1907 2023-10-26 15:44:04.000000 expecto-0.1.3/.github/workflows/ci_tests.yml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      764 2023-03-28 00:01:34.000000 expecto-0.1.3/.gitignore
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      225 2023-10-26 14:58:13.000000 expecto-0.1.3/.readthedocs.yaml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      325 2023-03-28 00:01:34.000000 expecto-0.1.3/MANIFEST.in
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1995 2023-10-26 15:50:31.772111 expecto-0.1.3/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1169 2023-10-26 14:58:13.000000 expecto-0.1.3/README.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.765980 expecto-0.1.3/docs/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6148 2023-03-28 11:17:30.000000 expecto-0.1.3/docs/.DS_Store
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      634 2023-03-28 00:01:34.000000 expecto-0.1.3/docs/Makefile
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.767113 expecto-0.1.3/docs/assets/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5786 2023-03-28 00:15:51.000000 expecto-0.1.3/docs/assets/logo.ico
--rw-------   0 bmmorris  (5602) STSCI\science  (1031)     4120 2023-03-28 00:14:50.000000 expecto-0.1.3/docs/assets/logo.png
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1173 2023-03-28 00:12:54.000000 expecto-0.1.3/docs/assets/logo.svg
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2722 2023-10-26 14:59:10.000000 expecto-0.1.3/docs/conf.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.767555 expecto-0.1.3/docs/expecto/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      113 2023-03-28 00:01:34.000000 expecto-0.1.3/docs/expecto/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1129 2023-10-26 14:58:13.000000 expecto-0.1.3/docs/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      760 2023-03-28 00:01:34.000000 expecto-0.1.3/docs/make.bat
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.768297 expecto-0.1.3/expecto/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      134 2023-03-28 00:01:34.000000 expecto-0.1.3/expecto/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6111 2023-10-26 14:58:13.000000 expecto-0.1.3/expecto/core.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.769950 expecto-0.1.3/expecto/data/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      245 2023-03-28 00:01:34.000000 expecto-0.1.3/expecto/data/README.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.770421 expecto-0.1.3/expecto/tests/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2023-03-28 00:01:34.000000 expecto-0.1.3/expecto/tests/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      985 2023-03-28 00:01:34.000000 expecto-0.1.3/expecto/tests/test_core.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      345 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto/version.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.769775 expecto-0.1.3/expecto.egg-info/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1995 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      668 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-03-28 00:04:58.000000 expecto-0.1.3/expecto.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      172 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto.egg-info/requires.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        8 2023-10-26 15:50:31.000000 expecto-0.1.3/expecto.egg-info/top_level.txt
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-10-26 15:50:31.771045 expecto-0.1.3/licenses/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1487 2023-03-28 00:01:34.000000 expecto-0.1.3/licenses/LICENSE.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2023-03-28 00:01:34.000000 expecto-0.1.3/licenses/README.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2023-03-28 00:01:34.000000 expecto-0.1.3/licenses/TEMPLATE_LICENSE.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      134 2023-03-28 00:01:34.000000 expecto-0.1.3/pyproject.toml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1312 2023-10-26 15:50:31.772681 expecto-0.1.3/setup.cfg
--rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)      658 2023-03-28 00:01:34.000000 expecto-0.1.3/setup.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2164 2023-10-26 14:59:25.000000 expecto-0.1.3/tox.ini
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.149284 expecto-0.1.4/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.133248 expecto-0.1.4/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.136613 expecto-0.1.4/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1907 2023-10-26 15:44:04.000000 expecto-0.1.4/.github/workflows/ci_tests.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      764 2023-03-28 00:01:34.000000 expecto-0.1.4/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      225 2023-10-26 14:58:13.000000 expecto-0.1.4/.readthedocs.yaml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      325 2023-03-28 00:01:34.000000 expecto-0.1.4/MANIFEST.in
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1995 2024-04-28 18:18:51.149165 expecto-0.1.4/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1169 2023-10-26 14:58:13.000000 expecto-0.1.4/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.142242 expecto-0.1.4/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6148 2023-03-28 11:17:30.000000 expecto-0.1.4/docs/.DS_Store
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      634 2023-03-28 00:01:34.000000 expecto-0.1.4/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.143021 expecto-0.1.4/docs/assets/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5786 2023-03-28 00:15:51.000000 expecto-0.1.4/docs/assets/logo.ico
+-rw-------   0 bmmorris  (5602) STSCI\science  (1031)     4120 2023-03-28 00:14:50.000000 expecto-0.1.4/docs/assets/logo.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1173 2023-03-28 00:12:54.000000 expecto-0.1.4/docs/assets/logo.svg
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2722 2023-10-26 14:59:10.000000 expecto-0.1.4/docs/conf.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.143375 expecto-0.1.4/docs/expecto/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      113 2023-03-28 00:01:34.000000 expecto-0.1.4/docs/expecto/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1129 2023-10-26 14:58:13.000000 expecto-0.1.4/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      760 2023-03-28 00:01:34.000000 expecto-0.1.4/docs/make.bat
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.144256 expecto-0.1.4/expecto/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      134 2023-03-28 00:01:34.000000 expecto-0.1.4/expecto/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6568 2024-04-28 17:53:44.000000 expecto-0.1.4/expecto/core.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.145809 expecto-0.1.4/expecto/data/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      245 2023-03-28 00:01:34.000000 expecto-0.1.4/expecto/data/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.146417 expecto-0.1.4/expecto/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2023-03-28 00:01:34.000000 expecto-0.1.4/expecto/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1706 2024-04-28 18:07:18.000000 expecto-0.1.4/expecto/tests/test_core.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      345 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.148212 expecto-0.1.4/expecto.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1995 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      668 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-03-28 00:04:58.000000 expecto-0.1.4/expecto.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      172 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        8 2024-04-28 18:18:51.000000 expecto-0.1.4/expecto.egg-info/top_level.txt
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2024-04-28 18:18:51.147569 expecto-0.1.4/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1487 2023-03-28 00:01:34.000000 expecto-0.1.4/licenses/LICENSE.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2023-03-28 00:01:34.000000 expecto-0.1.4/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2023-03-28 00:01:34.000000 expecto-0.1.4/licenses/TEMPLATE_LICENSE.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      134 2023-03-28 00:01:34.000000 expecto-0.1.4/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1312 2024-04-28 18:18:51.149703 expecto-0.1.4/setup.cfg
+-rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)      658 2023-03-28 00:01:34.000000 expecto-0.1.4/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2164 2023-10-26 14:59:25.000000 expecto-0.1.4/tox.ini
```

### Comparing `expecto-0.1.3/.github/workflows/ci_tests.yml` & `expecto-0.1.4/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/.gitignore` & `expecto-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/PKG-INFO` & `expecto-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expecto
-Version: 0.1.3
+Version: 0.1.4
 Summary: PHOENIX model spectrum retriever
 Home-page: https://github.com/bmorris3/expecto
 Author: Brett M. Morris
 Author-email: morrisbrettm@gmail.com
 License: BSD 3-Clause
 Requires-Python: >=3.5
 License-File: licenses/LICENSE.rst
```

### Comparing `expecto-0.1.3/README.rst` & `expecto-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/.DS_Store` & `expecto-0.1.4/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/Makefile` & `expecto-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/assets/logo.ico` & `expecto-0.1.4/docs/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/assets/logo.png` & `expecto-0.1.4/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/assets/logo.svg` & `expecto-0.1.4/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/conf.py` & `expecto-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/index.rst` & `expecto-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/docs/make.bat` & `expecto-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/expecto/core.py` & `expecto-0.1.4/expecto/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,24 +105,47 @@
         z_sign = '-'
 
     if closest_grid_alpha > 0.1:
         alpha_sign = '+'
     else:
         alpha_sign = '-'
 
+    directory_term = (
+        'Z' + z_sign + '{Z:1.1f}'
+    ).format(
+        Z=abs(closest_grid_Z)
+    )
+
+    metallicity_term = (
+        z_sign + '{Z:1.1f}'
+    ).format(
+        Z=abs(closest_grid_Z)
+    )
+
+    if closest_grid_alpha != 0:
+        alpha_term = (
+            'Alpha=' + alpha_sign + '{alpha:1.2f}'
+        ).format(
+            alpha=abs(closest_grid_alpha)
+        )
+
+        directory_term += '.' + alpha_term
+        metallicity_term += '.' + alpha_term + '.'
+    else:
+        metallicity_term += '.'
+
     url = (
         phoenix_base_url +
-        'Z' + z_sign +
-        '{Z:1.1f}/lte{T_eff:05d}-{log_g:1.2f}' + alpha_sign +
-        '{alpha:1.1f}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'
+        directory_term +
+        '/lte{T_eff:05d}-{log_g:1.2f}' +
+        metallicity_term +
+        'PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'
     ).format(
         T_eff=closest_grid_temperature,
         log_g=closest_grid_logg,
-        Z=abs(closest_grid_Z),
-        alpha=closest_grid_alpha
     )
     return url
 
 
 def get_spectrum(
         T_eff, log_g, Z=0, alpha=0, cache=False, vacuum=True
 ):
```

### Comparing `expecto-0.1.3/expecto.egg-info/PKG-INFO` & `expecto-0.1.4/expecto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expecto
-Version: 0.1.3
+Version: 0.1.4
 Summary: PHOENIX model spectrum retriever
 Home-page: https://github.com/bmorris3/expecto
 Author: Brett M. Morris
 Author-email: morrisbrettm@gmail.com
 License: BSD 3-Clause
 Requires-Python: >=3.5
 License-File: licenses/LICENSE.rst
```

### Comparing `expecto-0.1.3/expecto.egg-info/SOURCES.txt` & `expecto-0.1.4/expecto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/licenses/LICENSE.rst` & `expecto-0.1.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/licenses/TEMPLATE_LICENSE.rst` & `expecto-0.1.4/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/setup.cfg` & `expecto-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/setup.py` & `expecto-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `expecto-0.1.3/tox.ini` & `expecto-0.1.4/tox.ini`

 * *Files identical despite different names*

