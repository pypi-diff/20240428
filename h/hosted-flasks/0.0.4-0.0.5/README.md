# Comparing `tmp/hosted-flasks-0.0.4.tar.gz` & `tmp/hosted-flasks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.4.tar", last modified: Sat Apr 27 14:07:38 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.5.tar", last modified: Sun Apr 28 16:10:20 2024, max compression
```

## Comparing `hosted-flasks-0.0.4.tar` & `hosted-flasks-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.036513 hosted-flasks-0.0.4/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.032906 hosted-flasks-0.0.4/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.4/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 14:07:38.036401 hosted-flasks-0.0.4/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.033104 hosted-flasks-0.0.4/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.033660 hosted-flasks-0.0.4/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)       22 2024-04-27 14:06:27.000000 hosted-flasks-0.0.4/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      686 2024-04-27 09:34:49.000000 hosted-flasks-0.0.4/hosted_flasks/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.034467 hosted-flasks-0.0.4/hosted_flasks/frontpage/
--rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/index.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035489 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/
--rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-192x192.png
--rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-512x512.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/apple-touch-icon.png
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035731 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/default.css
--rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-27 13:14:19.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/style.css
--rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-16x16.png
--rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-32x32.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon.ico
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.035921 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/.gitkeep
--rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/logo.svg
--rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/robots.txt
--rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage/static/site.webmanifest
--rw-r--r--   0 xtof       (501) staff       (20)      859 2024-04-27 13:12:57.000000 hosted-flasks-0.0.4/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)     1696 2024-04-27 14:05:39.000000 hosted-flasks-0.0.4/hosted_flasks/scanner.py
--rw-r--r--   0 xtof       (501) staff       (20)      796 2024-04-27 14:02:43.000000 hosted-flasks-0.0.4/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.034349 hosted-flasks-0.0.4/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1107 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       29 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-27 14:07:38.000000 hosted-flasks-0.0.4/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-27 14:07:38.036552 hosted-flasks-0.0.4/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1627 2024-04-27 14:06:16.000000 hosted-flasks-0.0.4/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-27 14:07:38.036240 hosted-flasks-0.0.4/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.4/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      651 2024-04-25 19:07:50.000000 hosted-flasks-0.0.4/tests/test_config.py
--rw-r--r--   0 xtof       (501) staff       (20)     1440 2024-04-27 09:44:49.000000 hosted-flasks-0.0.4/tests/test_scanner.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.255424 hosted-flasks-0.0.5/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.251343 hosted-flasks-0.0.5/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.5/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.5/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.5/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-28 16:10:20.255306 hosted-flasks-0.0.5/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.251548 hosted-flasks-0.0.5/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.5/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.5/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.252290 hosted-flasks-0.0.5/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)      294 2024-04-28 16:09:56.000000 hosted-flasks-0.0.5/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.5/hosted_flasks/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.253179 hosted-flasks-0.0.5/hosted_flasks/frontpage/
+-rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/index.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.254326 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/
+-rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/android-chrome-192x192.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/android-chrome-512x512.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/apple-touch-icon.png
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.254575 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/css/default.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/css/style.css
+-rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon-16x16.png
+-rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon-32x32.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon.ico
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.254800 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/img/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/img/.gitkeep
+-rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/img/logo.svg
+-rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/robots.txt
+-rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage/static/site.webmanifest
+-rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.5/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2923 2024-04-28 16:07:41.000000 hosted-flasks-0.0.5/hosted_flasks/loader.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1556 2024-04-28 14:48:51.000000 hosted-flasks-0.0.5/hosted_flasks/monkeypatch.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1164 2024-04-28 12:33:30.000000 hosted-flasks-0.0.5/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.253048 hosted-flasks-0.0.5/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-28 16:10:20.000000 hosted-flasks-0.0.5/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-28 16:10:20.255470 hosted-flasks-0.0.5/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.5/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:10:20.255123 hosted-flasks-0.0.5/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.5/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-28 14:42:09.000000 hosted-flasks-0.0.5/tests/test_environ_get.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3250 2024-04-28 16:06:39.000000 hosted-flasks-0.0.5/tests/test_loader.py
```

### Comparing `hosted-flasks-0.0.4/.github/README.md` & `hosted-flasks-0.0.5/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/LICENSE.txt` & `hosted-flasks-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/PKG-INFO` & `hosted-flasks-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.4
+Version: 0.0.5
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.4/docs/conf.py` & `hosted-flasks-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/index.html` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/index.html`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-192x192.png` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/android-chrome-512x512.png` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/apple-touch-icon.png` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/default.css` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/css/default.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/css/style.css` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/css/style.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-16x16.png` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon-32x32.png` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/favicon.ico` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage/static/img/logo.svg` & `hosted-flasks-0.0.5/hosted_flasks/frontpage/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.4/hosted_flasks/frontpage.py` & `hosted-flasks-0.0.5/hosted_flasks/frontpage.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import os
 
 from pathlib import Path
 
 from flask import Flask, render_template
 
+from hosted_flasks.loader import get_apps
+
 logger = logging.getLogger(__name__)
 
 FRONTPAGE_FOLDER = os.environ.get("HOSTED_FLASKS_FRONTPAGE_FOLDER", None)
 if not FRONTPAGE_FOLDER:
   FRONTPAGE_FOLDER = Path(__file__).resolve().parent / "frontpage"
   logger.debug("📰 using default frontpage folder")
 else:
@@ -21,12 +23,10 @@
   template_folder=FRONTPAGE_FOLDER,
   static_folder=f"{FRONTPAGE_FOLDER}/static",
   static_url_path=""
 )
 
 app.config["TEMPLATES_AUTO_RELOAD"] = True
 
-apps = [] # to be filled externally with apps that are served, see server.py
-
 @app.route("/")
 def show_frontpage():
-  return render_template("index.html", apps=apps)
+  return render_template("index.html", apps=get_apps())
```

### Comparing `hosted-flasks-0.0.4/hosted_flasks/server.py` & `hosted-flasks-0.0.5/hosted_flasks/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import logging
 
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 
-from hosted_flasks import scanner
 from hosted_flasks import frontpage
+from hosted_flasks.loader import get_apps
 
-logger = logging.getLogger(__name__)
+# setup logging to stdout
+
+import os
+
+LOG_LEVEL = os.environ.get("LOG_LEVEL") or "INFO"
+FORMAT    = "[%(asctime)s] [%(process)d] [%(levelname)s] [%(name)s] %(message)s"
+DATEFMT   = "%Y-%m-%d %H:%M:%S %z"
 
-# load modules/apps dynamically
+logging.basicConfig(level=LOG_LEVEL, format=FORMAT, datefmt=DATEFMT)
+formatter = logging.Formatter(FORMAT, DATEFMT)
+logging.getLogger().handlers[0].setFormatter(formatter)
+
+logger = logging.getLogger(__name__)
 
-apps = scanner.find_apps()
-frontpage.apps = apps
+# dispatch apps based on path and/or hostname
 
 class DomainDispatcher:
   def __init__(self, apps, default=None):
     self.apps    = apps
     self.default = default
 
   def __call__(self, environ, start_response):
     return self.apps.get(environ["HTTP_HOST"], self.default)(environ, start_response)
 
 # combine the apps with the frontpage
 
-app = DomainDispatcher({ app.hostname : app.handler for app in apps },
+app = DomainDispatcher({ app.hostname : app.handler for app in get_apps() },
   default=DispatcherMiddleware(frontpage.app, {
-    app.path : app.handler for app in apps
+    app.path : app.handler for app in get_apps()
   })
 )
 
-logger.info(f"✅ {len(apps)} hosted flasks up & running...")
+logger.info(f"✅ {len(get_apps())} hosted flasks up & running...")
```

### Comparing `hosted-flasks-0.0.4/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.5/hosted_flasks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.4
+Version: 0.0.5
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.4/hosted_flasks.egg-info/SOURCES.txt` & `hosted-flasks-0.0.5/hosted_flasks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 setup.py
 .github/README.md
 docs/__init__.py
 docs/conf.py
 hosted_flasks/__init__.py
 hosted_flasks/__main__.py
 hosted_flasks/frontpage.py
-hosted_flasks/scanner.py
+hosted_flasks/loader.py
+hosted_flasks/monkeypatch.py
 hosted_flasks/server.py
 hosted_flasks.egg-info/PKG-INFO
 hosted_flasks.egg-info/SOURCES.txt
 hosted_flasks.egg-info/dependency_links.txt
 hosted_flasks.egg-info/entry_points.txt
 hosted_flasks.egg-info/requires.txt
 hosted_flasks.egg-info/top_level.txt
@@ -25,9 +26,9 @@
 hosted_flasks/frontpage/static/robots.txt
 hosted_flasks/frontpage/static/site.webmanifest
 hosted_flasks/frontpage/static/css/default.css
 hosted_flasks/frontpage/static/css/style.css
 hosted_flasks/frontpage/static/img/.gitkeep
 hosted_flasks/frontpage/static/img/logo.svg
 tests/__init__.py
-tests/test_config.py
-tests/test_scanner.py
+tests/test_environ_get.py
+tests/test_loader.py
```

### Comparing `hosted-flasks-0.0.4/setup.py` & `hosted-flasks-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "License :: OSI Approved :: MIT License",
   
 ]
 INSTALL_REQUIRES = [
   "Flask",
   "python-dotenv",
   "eventlet",
+  "pyyaml",
   
 ]
 ENTRY_POINTS = {
   "console_scripts" : [
     "hosted-flasks=hosted_flasks.__main__:cli",
     
   ]
```

