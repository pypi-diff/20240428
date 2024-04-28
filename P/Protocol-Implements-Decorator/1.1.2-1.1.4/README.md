# Comparing `tmp/protocol_implements_decorator-1.1.2.tar.gz` & `tmp/protocol_implements_decorator-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protocol_implements_decorator-1.1.2.tar", last modified: Tue Apr 23 03:15:27 2024, max compression
+gzip compressed data, was "protocol_implements_decorator-1.1.4.tar", last modified: Sun Apr 28 15:44:44 2024, max compression
```

## Comparing `protocol_implements_decorator-1.1.2.tar` & `protocol_implements_decorator-1.1.4.tar`

### file list

```diff
@@ -1,56 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.564164 protocol_implements_decorator-1.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/gh_pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/check_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/create.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.560164 protocol_implements_decorator-1.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/source/protocolimplementsdecorator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.560164 protocol_implements_decorator-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/implements.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/tests/test_protocolimplementsdecorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:44.188429 protocol_implements_decorator-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-28 15:44:44.000000 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-28 15:44:44.000000 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:44:44.000000 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-28 15:44:44.000000 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 15:44:44.000000 protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/src/protocolimplementsdecorator/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/src/protocolimplementsdecorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/src/protocolimplementsdecorator/implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/src/protocolimplementsdecorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:44:44.192429 protocol_implements_decorator-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-28 15:44:40.000000 protocol_implements_decorator-1.1.4/tests/test_protocolimplementsdecorator.py
```

### Comparing `protocol_implements_decorator-1.1.2/LICENSE` & `protocol_implements_decorator-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `protocol_implements_decorator-1.1.2/PKG-INFO` & `protocol_implements_decorator-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Protocol-Implements-Decorator
-Version: 1.1.2
+Version: 1.1.4
 Summary: Adds the 'implements' decorator to make using protocols easier and more explicit
 Author: R.Broderick
 License: BSD 3-Clause License
         
         Copyright (c) 2021, rbroderi
         All rights reserved.
         
@@ -29,14 +29,21 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
+Project-URL: homepage, https://github.com/rbroderi/protocol_implements_decorator
+Project-URL: documentation, https://rbroderi.github.io/protocol_implements_decorator/
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions; python_version < "3.12"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: dapperdata; extra == "dev"
@@ -54,14 +61,15 @@
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
+Requires-Dist: pip-audit; extra == "dev"
 Provides-Extra: optional
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-rtd-size; extra == "docs"
 Requires-Dist: autodocsumm; extra == "docs"
@@ -143,16 +151,7 @@
 
   def other(self) -> str:
     return str(self)
 ```
 ```text
 NotImplementedError: test.<locals>.Printable requires implentation of ['to_string']
 ```
-
-
-
-<!-- pyscaffold-notes -->
-
-## Note
-
-This project has been set up using PyScaffold 4.1.1. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/PKG-INFO` & `protocol_implements_decorator-1.1.4/src/Protocol_Implements_Decorator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Protocol-Implements-Decorator
-Version: 1.1.2
+Version: 1.1.4
 Summary: Adds the 'implements' decorator to make using protocols easier and more explicit
 Author: R.Broderick
 License: BSD 3-Clause License
         
         Copyright (c) 2021, rbroderi
         All rights reserved.
         
@@ -29,14 +29,21 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
+Project-URL: homepage, https://github.com/rbroderi/protocol_implements_decorator
+Project-URL: documentation, https://rbroderi.github.io/protocol_implements_decorator/
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions; python_version < "3.12"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: dapperdata; extra == "dev"
@@ -54,14 +61,15 @@
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
+Requires-Dist: pip-audit; extra == "dev"
 Provides-Extra: optional
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: sphinx-rtd-size; extra == "docs"
 Requires-Dist: autodocsumm; extra == "docs"
@@ -143,16 +151,7 @@
 
   def other(self) -> str:
     return str(self)
 ```
 ```text
 NotImplementedError: test.<locals>.Printable requires implentation of ['to_string']
 ```
-
-
-
-<!-- pyscaffold-notes -->
-
-## Note
-
-This project has been set up using PyScaffold 4.1.1. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `protocol_implements_decorator-1.1.2/README.md` & `protocol_implements_decorator-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -74,16 +74,7 @@
 
   def other(self) -> str:
     return str(self)
 ```
 ```text
 NotImplementedError: test.<locals>.Printable requires implentation of ['to_string']
 ```
-
-
-
-<!-- pyscaffold-notes -->
-
-## Note
-
-This project has been set up using PyScaffold 4.1.1. For details and usage
-information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `protocol_implements_decorator-1.1.2/pyproject.toml` & `protocol_implements_decorator-1.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
+requires = ["setuptools>=67.0", "wheel"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Adds the 'implements' decorator to make using protocols easier and more explicit"
-version = "1.1.2"
+version = "1.1.4"
 license = {"file" = "LICENSE"}
 name = "Protocol-Implements-Decorator"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
+classifiers = [
+  "License :: OSI Approved :: BSD License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12"
+]
 
 [project.optional-dependencies]
 dev = [
   "build",
   "dapperdata",
   "glom",
   "mypy",
@@ -29,15 +36,16 @@
   "packaging",
   "snakeviz",
   "pre-commit",
   "tox",
   "tox-pyenv-redux",
   "pylint",
   "perflint",
-  "snakeviz"
+  "snakeviz",
+  "pip-audit"
 ]
 # pep725
 # [external]
 # build-requires = [
 # "virtual:compiler/rust",
 # "virtual:compiler/cargo",
 # ]
@@ -47,14 +55,18 @@
   "sphinx-autodoc-typehints",
   "sphinx-rtd-theme",
   "sphinx-rtd-size",
   "autodocsumm",
   "sphinx-pyproject"
 ]
 
+[project.urls]
+homepage = "https://github.com/rbroderi/protocol_implements_decorator"
+documentation = "https://rbroderi.github.io/protocol_implements_decorator/"
+
 [tool.dapperdata]
 exclude_paths = [".venv", ".mypy_cache", ".git", ".vscode"]
 
 [tool.pylint.format]
 max-line-length = 200
 
 [tool.pylint.main]
@@ -233,16 +245,17 @@
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
 [tool.setuptools.package-data]
 library = ["py.typed"]
 
-[tool.setuptools.packages]
-find = {}
+[tool.setuptools.packages.find]
+exclude = ["docs*", "tests*"]
+where = ["src"]
 
 [tool.sphinx-pyproject]
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 coverage_show_missing_items = true
 extensions = [
   "sphinx.ext.autodoc",
```

### Comparing `protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/implements.py` & `protocol_implements_decorator-1.1.4/src/protocolimplementsdecorator/implements.py`

 * *Files identical despite different names*

### Comparing `protocol_implements_decorator-1.1.2/tests/test_protocolimplementsdecorator.py` & `protocol_implements_decorator-1.1.4/tests/test_protocolimplementsdecorator.py`

 * *Files identical despite different names*

