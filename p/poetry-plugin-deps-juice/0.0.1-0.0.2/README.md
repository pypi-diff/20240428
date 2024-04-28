# Comparing `tmp/poetry_plugin_deps_juice-0.0.1.tar.gz` & `tmp/poetry_plugin_deps_juice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_deps_juice-0.0.1.tar", max compression
+gzip compressed data, was "poetry_plugin_deps_juice-0.0.2.tar", max compression
```

## Comparing `poetry_plugin_deps_juice-0.0.1.tar` & `poetry_plugin_deps_juice-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-28 15:51:07.325741 poetry_plugin_deps_juice-0.0.1/LICENSE
--rw-r--r--   0        0        0     2423 2024-04-28 19:50:49.790946 poetry_plugin_deps_juice-0.0.1/README.md
--rw-r--r--   0        0        0     3281 2024-04-28 19:49:55.985948 poetry_plugin_deps_juice-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      171 2024-04-28 16:30:53.364609 poetry_plugin_deps_juice-0.0.1/src/poetry_plugin_deps_juice/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-28 19:17:23.962056 poetry_plugin_deps_juice-0.0.1/src/poetry_plugin_deps_juice/command.py
--rw-r--r--   0        0        0      899 2024-04-28 18:20:53.815244 poetry_plugin_deps_juice-0.0.1/src/poetry_plugin_deps_juice/plugins.py
--rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 poetry_plugin_deps_juice-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-28 15:51:07.325741 poetry_plugin_deps_juice-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3400 2024-04-29 10:48:52.167890 poetry_plugin_deps_juice-0.0.2/README.md
+-rw-r--r--   0        0        0     3281 2024-04-28 21:05:35.552697 poetry_plugin_deps_juice-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      171 2024-04-28 16:30:53.364609 poetry_plugin_deps_juice-0.0.2/src/poetry_plugin_deps_juice/__init__.py
+-rw-r--r--   0        0        0     4023 2024-04-29 10:42:49.275911 poetry_plugin_deps_juice-0.0.2/src/poetry_plugin_deps_juice/command.py
+-rw-r--r--   0        0        0      899 2024-04-28 21:25:59.670630 poetry_plugin_deps_juice-0.0.2/src/poetry_plugin_deps_juice/plugins.py
+-rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 poetry_plugin_deps_juice-0.0.2/PKG-INFO
```

### Comparing `poetry_plugin_deps_juice-0.0.1/LICENSE` & `poetry_plugin_deps_juice-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_deps_juice-0.0.1/README.md` & `poetry_plugin_deps_juice-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,49 @@
 ## Poetry Dependency Juice Plugin
 
 This plugin simplifies the process of managing dependencies in your Poetry projects by allowing you to mix dependencies from specified groups and wrap the `poetry build` command into `poetry jbuild`.
 It provides an easy way to create custom mixes of dependencies and execute the build command with those mixes.
 
+See difference:
+
+#### Poetry build:
+```bash
+poetry build && pkginfo -f requires_dist dist/*.whl
+```
+
+#### output:
+```plaintext
+Building poetry-plugin-deps-juice (0.0.2)
+  - Building sdist
+  - Built poetry_plugin_deps_juice-0.0.2.tar.gz
+  - Building wheel
+  - Built poetry_plugin_deps_juice-0.0.2-py3-none-any.whl
+requires_dist: ['poetry (>=1.8.0,<2.0.0)']
+```
+
+#### Juice build:
+```bash
+poetry jbuild && pkginfo -f requires_dist dist/*.whl
+```
+
+#### output:
+```plaintext
+Mixing juice..
+base -> poetry
+        {'poetry-core': '^1.7.0', 'wheel': '^0.42.0'}
+setup -> poetry
+        {'build': '^1.0.3', 'setuptools': '^69.0.3'}
+Building poetry-plugin-deps-juice (0.0.2)
+  - Building sdist
+  - Built poetry_plugin_deps_juice-0.0.2.tar.gz
+  - Building wheel
+  - Built poetry_plugin_deps_juice-0.0.2-py3-none-any.whl
+requires_dist: ['build (>=1.0.3,<2.0.0)', 'poetry (>=1.8.0,<2.0.0)', 'poetry-core (>=1.7.0,<2.0.0)', 'setuptools (>=69.0.3,<70.0.0)', 'wheel (>=0.42.0,<0.43.0)']
+```
+
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
```

### Comparing `poetry_plugin_deps_juice-0.0.1/pyproject.toml` & `poetry_plugin_deps_juice-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-deps-juice"
-version = "0.0.1"
+version = "0.0.2"
 description = "Poetry plugin for simple mix dependencies from toml option and wrap poetry 'build' command."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
@@ -146,21 +146,21 @@
 [tool.poetry.group.fancy.dependencies]
 rich = "^13.7.1"
 
 [tool.poetry.group.base]
 
 [tool.poetry.group.base.dependencies]
 poetry-core = "^1.7.0"
+wheel = "^0.42.0"
 
 [tool.poetry.group.setup]
 
 [tool.poetry.group.setup.dependencies]
 build = "^1.0.3"
 setuptools = "^69.0.3"
-wheel = "^0.42.0"
 
 [tool.poetry.group.test]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-dependency = "^0.5.1"
```

### Comparing `poetry_plugin_deps_juice-0.0.1/src/poetry_plugin_deps_juice/plugins.py` & `poetry_plugin_deps_juice-0.0.2/src/poetry_plugin_deps_juice/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_deps_juice-0.0.1/PKG-INFO` & `poetry_plugin_deps_juice-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-deps-juice
-Version: 0.0.1
+Version: 0.0.2
 Summary: Poetry plugin for simple mix dependencies from toml option and wrap poetry 'build' command.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,25 +21,66 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: build (>=1.0.3,<2.0.0)
 Requires-Dist: poetry (>=1.8.0,<2.0.0)
+Requires-Dist: poetry-core (>=1.7.0,<2.0.0)
+Requires-Dist: setuptools (>=69.0.3,<70.0.0)
+Requires-Dist: wheel (>=0.42.0,<0.43.0)
 Project-URL: Documentation, https://github.com/BlackCatDevel0per/poetry-plugin-deps-juice
 Project-URL: Homepage, https://github.com/BlackCatDevel0per/poetry-plugin-deps-juice
 Project-URL: Repository, https://github.com/BlackCatDevel0per/poetry-plugin-deps-juice
 Description-Content-Type: text/markdown
 
 ## Poetry Dependency Juice Plugin
 
 This plugin simplifies the process of managing dependencies in your Poetry projects by allowing you to mix dependencies from specified groups and wrap the `poetry build` command into `poetry jbuild`.
 It provides an easy way to create custom mixes of dependencies and execute the build command with those mixes.
 
+See difference:
+
+#### Poetry build:
+```bash
+poetry build && pkginfo -f requires_dist dist/*.whl
+```
+
+#### output:
+```plaintext
+Building poetry-plugin-deps-juice (0.0.2)
+  - Building sdist
+  - Built poetry_plugin_deps_juice-0.0.2.tar.gz
+  - Building wheel
+  - Built poetry_plugin_deps_juice-0.0.2-py3-none-any.whl
+requires_dist: ['poetry (>=1.8.0,<2.0.0)']
+```
+
+#### Juice build:
+```bash
+poetry jbuild && pkginfo -f requires_dist dist/*.whl
+```
+
+#### output:
+```plaintext
+Mixing juice..
+base -> poetry
+        {'poetry-core': '^1.7.0', 'wheel': '^0.42.0'}
+setup -> poetry
+        {'build': '^1.0.3', 'setuptools': '^69.0.3'}
+Building poetry-plugin-deps-juice (0.0.2)
+  - Building sdist
+  - Built poetry_plugin_deps_juice-0.0.2.tar.gz
+  - Building wheel
+  - Built poetry_plugin_deps_juice-0.0.2-py3-none-any.whl
+requires_dist: ['build (>=1.0.3,<2.0.0)', 'poetry (>=1.8.0,<2.0.0)', 'poetry-core (>=1.7.0,<2.0.0)', 'setuptools (>=69.0.3,<70.0.0)', 'wheel (>=0.42.0,<0.43.0)']
+```
+
 ### Usage
 
 1. **Installation**:
 
    Install the plugin using Poetry:
 
    ```bash
```

