# Comparing `tmp/oresat-gps-1.3.0.tar.gz` & `tmp/oresat_gps-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-gps-1.3.0.tar", last modified: Sun Jan  7 02:57:06 2024, max compression
+gzip compressed data, was "oresat_gps-1.4.0.tar", last modified: Sun Apr 28 03:21:48 2024, max compression
```

## Comparing `oresat-gps-1.3.0.tar` & `oresat_gps-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 02:57:06.981150 oresat-gps-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-07 02:57:06.981150 oresat-gps-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 02:57:06.977150 oresat-gps-1.3.0/oresat_gps/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/oresat_gps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/oresat_gps/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/oresat_gps/gps_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/oresat_gps/skytraq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 02:57:06.981150 oresat-gps-1.3.0/oresat_gps/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/oresat_gps/templates/skytraq.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 02:57:06.981150 oresat-gps-1.3.0/oresat_gps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-07 02:57:06.000000 oresat-gps-1.3.0/oresat_gps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-07 02:56:49.000000 oresat-gps-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 02:57:06.981150 oresat-gps-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.790771 oresat_gps-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.786771 oresat_gps-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.786771 oresat_gps-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 03:21:48.790771 oresat_gps-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.786771 oresat_gps-1.4.0/oresat_gps/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/oresat_gps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/oresat_gps/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/oresat_gps/gps_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/oresat_gps/skytraq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.790771 oresat_gps-1.4.0/oresat_gps/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/oresat_gps/templates/skytraq.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:21:48.790771 oresat_gps-1.4.0/oresat_gps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-28 03:21:48.000000 oresat_gps-1.4.0/oresat_gps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 03:21:43.000000 oresat_gps-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 03:21:48.790771 oresat_gps-1.4.0/setup.cfg
```

### Comparing `oresat-gps-1.3.0/LICENSE` & `oresat_gps-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.3.0/PKG-INFO` & `oresat_gps-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-gps
-Version: 1.3.0
+Version: 1.4.0
 Summary: OreSat GPS OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat-gps-1.3.0/README.md` & `oresat_gps-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.3.0/oresat_gps/__main__.py` & `oresat_gps-1.4.0/oresat_gps/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """GPS OLAF app main"""
 
 import os
 
-from olaf import Gpio, app, olaf_run, olaf_setup, render_olaf_template, rest_api
+from olaf import app, olaf_run, olaf_setup, render_olaf_template, rest_api
 
 from . import __version__
 from .gps_service import GpsService
-from .skytraq import SkyTraq
 
 
 @rest_api.app.route("/skytraq")
 def skytraq_template():
     """Render skytraq webpage."""
 
     return render_olaf_template("skytraq.html", name="SkyTraq")
@@ -23,19 +22,15 @@
 
     args, _ = olaf_setup("gps")
     mock_args = [i.lower() for i in args.mock_hw]
     mock_skytraq = "skytraq" in mock_args or "all" in mock_args
 
     app.od["versions"]["sw_version"].value = __version__
 
-    skytraq = SkyTraq("/dev/ttyS2", mock_skytraq)
-    gpio_lna = Gpio("MAX_EN", mock_skytraq)
-    gpio_skytraq = Gpio("STQ_EN", mock_skytraq)
-
-    app.add_service(GpsService(skytraq, gpio_lna, gpio_skytraq))
+    app.add_service(GpsService(app.node, mock_skytraq))
 
     rest_api.add_template(f"{path}/templates/skytraq.html")
 
     olaf_run()
 
 
 if __name__ == "__main__":
```

### Comparing `oresat-gps-1.3.0/oresat_gps/skytraq.py` & `oresat_gps-1.4.0/oresat_gps/skytraq.py`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.3.0/oresat_gps/templates/skytraq.html` & `oresat_gps-1.4.0/oresat_gps/templates/skytraq.html`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.3.0/oresat_gps.egg-info/PKG-INFO` & `oresat_gps-1.4.0/oresat_gps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-gps
-Version: 1.3.0
+Version: 1.4.0
 Summary: OreSat GPS OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat-gps-1.3.0/pyproject.toml` & `oresat_gps-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oresat-gps"
 description = "OreSat GPS OLAF app"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -23,25 +23,25 @@
     "oresat-configs",
     "oresat-olaf>=3.2.0",
     "pyserial",
 ]
 dynamic = ["version"]
 
 [project.scripts]
-oresat-c3 = "oresat_gps.__main__:main"
-
-[tool.setuptools.dynamic]
-version = {attr = "oresat_gps.__version__"}
+oresat-gps = "oresat_gps.__main__:main"
 
 [tool.setuptools.packages.find]
 exclude = ["docs*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.html"]
 
+[tool.setuptools_scm]
+write_to = "oresat_gps/_version.py"
+
 [tool.black]
 line_length = 100
 
 [tool.pylama]
 format = "pylint"
 skip = "*/.tox/*,*/.env/,*/.git/*,*/.github/*,*/build/*"
 linters = "pycodestyle,pyflakes,pylint,mccabe,mypy,radon"
```

