# Comparing `tmp/jupyterlab_athena_analytics-0.4.2.tar.gz` & `tmp/jupyterlab_athena_analytics-0.5.0.tar.gz`

## Comparing `jupyterlab_athena_analytics-0.4.2.tar` & `jupyterlab_athena_analytics-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/babel.config.js
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jest.config.js
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/tsconfig.test.json
--rw-r--r--   0        0        0   369604 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/yarn.lock
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/_version.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/package.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/static/496.a7ce35ddfa7cd6cd9920.js
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/static/736.1c2d46418a08bbb03c03.js
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/static/remoteEntry.e52194f51058e212e41a.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/src/.gitignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/src/.yarnrc.yml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/src/index.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/src/__tests__/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/yarn.lock
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/LICENSE
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/README.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7712 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/babel.config.js
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jest.config.js
+-rw-r--r--   0        0        0   356405 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/package-lock.json
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/tsconfig.test.json
+-rw-r--r--   0        0        0   369604 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/yarn.lock
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/_version.py
+-rw-r--r--   0        0        0    22457 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/build_log.json
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/package.json
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/lib_index_js.d31b135968cc3d787f4f.js
+-rw-r--r--   0        0        0     6945 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/lib_index_js.d31b135968cc3d787f4f.js.map
+-rw-r--r--   0        0        0    27657 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/remoteEntry.addacb8d9a5c62fa881a.js
+-rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/remoteEntry.addacb8d9a5c62fa881a.js.map
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/style.js
+-rw-r--r--   0        0        0    19371 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/style_index_js.a55924b249d8032e17e5.js
+-rw-r--r--   0        0        0    14868 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/static/style_index_js.a55924b249d8032e17e5.js.map
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/src/.gitignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/src/.yarnrc.yml
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/src/index.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/src/__tests__/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.0/PKG-INFO
```

### Comparing `jupyterlab_athena_analytics-0.4.2/RELEASE.md` & `jupyterlab_athena_analytics-0.5.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/jest.config.js` & `jupyterlab_athena_analytics-0.5.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/package.json` & `jupyterlab_athena_analytics-0.5.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'0.5.0'"}*

```diff
@@ -172,12 +172,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.2",
+    "version": "0.5.0",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.4.2/tsconfig.json` & `jupyterlab_athena_analytics-0.5.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/yarn.lock` & `jupyterlab_athena_analytics-0.5.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/jupyterlab_athena_analytics/labextension/package.json` & `jupyterlab_athena_analytics-0.5.0/jupyterlab_athena_analytics/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802350427350427%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.addacb8d9a5c62fa881a.js'}}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -103,15 +103,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_athena_analytics",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e52194f51058e212e41a.js",
+            "load": "static/remoteEntry.addacb8d9a5c62fa881a.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_athena_analytics/labextension"
     },
     "keywords": [
         "jupyter",
@@ -177,12 +177,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.2",
+    "version": "0.5.0",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.4.2/ui-tests/README.md` & `jupyterlab_athena_analytics-0.5.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/ui-tests/tests/jupyterlab_athena_analytics.spec.ts` & `jupyterlab_athena_analytics-0.5.0/ui-tests/tests/jupyterlab_athena_analytics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/.gitignore` & `jupyterlab_athena_analytics-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/LICENSE` & `jupyterlab_athena_analytics-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/README.md` & `jupyterlab_athena_analytics-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# DEVELOP
+
+### Build Extension
+```
+cd jupyterlab_athena_analytics
+pip install -e .
+```
+
+
+### Serve to view in jupyter
+```
+cd ~/workspace/notebooks
+pyenv activate jupyter_env
+jupyter lab --ServerApp.tornado_settings="{\"headers\": {\"Content-Security-Policy\": \"frame-ancestors 'self' https://app.athenaintelligence.ai https://staging-app.athenaintelligence.ai http://localhost:8081;\"}}"
+```
+
+
+
+
+
 # BG Notes
 
 # Workflow
 1. Bump a version using hatch
 2. Follow the release instructions
 
 ## Bump Version
```

### Comparing `jupyterlab_athena_analytics-0.4.2/pyproject.toml` & `jupyterlab_athena_analytics-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.4.2/PKG-INFO` & `jupyterlab_athena_analytics-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_athena_analytics
-Version: 0.4.2
+Version: 0.5.0
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_athena_analytics
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_athena_analytics/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_athena_analytics.git
 Author-email: Athena Intelligence <team@athenaintelligence.ai>
 License: BSD 3-Clause License
         
@@ -47,14 +47,34 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
+# DEVELOP
+
+### Build Extension
+```
+cd jupyterlab_athena_analytics
+pip install -e .
+```
+
+
+### Serve to view in jupyter
+```
+cd ~/workspace/notebooks
+pyenv activate jupyter_env
+jupyter lab --ServerApp.tornado_settings="{\"headers\": {\"Content-Security-Policy\": \"frame-ancestors 'self' https://app.athenaintelligence.ai https://staging-app.athenaintelligence.ai http://localhost:8081;\"}}"
+```
+
+
+
+
+
 # BG Notes
 
 # Workflow
 1. Bump a version using hatch
 2. Follow the release instructions
 
 ## Bump Version
```

