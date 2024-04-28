# Comparing `tmp/pelican_mau_reader-3.0.1.tar.gz` & `tmp/pelican_mau_reader-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Sep 11 06:40:08 2023, max compression
+gzip compressed data, was "pelican_mau_reader-4.0.0.tar", last modified: Sun Apr 28 20:49:58 2024, max compression
```

## Comparing `pelican_mau_reader-3.0.1.tar` & `pelican_mau_reader-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,8 @@
--rw-r--r--   0        0        0      201 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/.editorconfig
--rw-r--r--   0        0        0      737 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1261 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      563 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       65 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/RELEASE.md
--rw-r--r--   0        0        0     3168 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/tasks.py
--rw-r--r--   0        0        0       57 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/.github/FUNDING.yml
--rw-r--r--   0        0        0     2386 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       40 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/__init__.py
--rw-r--r--   0        0        0     3217 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/mau_reader.py
--rw-r--r--   0        0        0     2404 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/test_mau_reader.py
--rw-r--r--   0        0        0      196 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/test_data/article_with_content.html
--rw-r--r--   0        0        0      340 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/test_data/article_with_content.mau
--rw-r--r--   0        0        0      401 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/test_data/article_with_nonascii_metadata.mau
--rw-r--r--   0        0        0       21 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/.gitignore
--rw-r--r--   0        0        0     4707 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/README.md
--rw-r--r--   0        0        0     2983 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     6103 2023-09-11 06:40:08.000000 pelican_mau_reader-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1483 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      563 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4707 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/README.md
+-rw-r--r--   0        0        0       40 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/pelican/plugins/mau_reader/__init__.py
+-rw-r--r--   0        0        0     4461 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/pelican/plugins/mau_reader/mau_reader.py
+-rw-r--r--   0        0        0       26 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/pelican/plugins/mau_reader/test_mau_reader.py
+-rw-r--r--   0        0        0     2625 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6154 2024-04-28 20:49:52.000000 pelican_mau_reader-4.0.0/PKG-INFO
```

### Comparing `pelican_mau_reader-3.0.1/CHANGELOG.md` & `pelican_mau_reader-4.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGELOG
 =========
 
+4.0.0 - 2024-04-28
+------------------
+
+Update the reader to the Mau 4.0.0 interface.
+
+Contributed by [Leonardo Giordani](https://github.com/lgiordani) via [PR #32](https://github.com/pelican-plugins/mau-reader/pull/32/)
+
+
 3.0.1 - 2023-09-11
 ------------------
 
 Fix incorrect management of file extensions
 
 Contributed by [Leonardo Giordani](https://github.com/lgiordani) via [PR #30](https://github.com/pelican-plugins/mau-reader/pull/30/)
```

### Comparing `pelican_mau_reader-3.0.1/CONTRIBUTING.md` & `pelican_mau_reader-4.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pelican_mau_reader-3.0.1/pelican/plugins/mau_reader/mau_reader.py` & `pelican_mau_reader-4.0.0/pelican/plugins/mau_reader/mau_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from pelican import signals
 from pelican.readers import BaseReader
 from pelican.utils import pelican_open
 
 try:
     from mau import Mau, load_visitors
+    from mau.environment.environment import Environment
+    from mau.errors import MauErrorException, print_error
 
     visitor_classes = load_visitors()
     mau_enabled = True
 except ImportError:
     visitor_classes = []
     mau_enabled = False
 
@@ -27,68 +29,106 @@
     def __init__(self, output_format):
         super().__init__(
             f"Output format {output_format} is not supported by Mau. "
             "You might have to install a plugin."
         )
 
 
+class ErrorInSourceFile(Exception):
+    """Exception to signal an error parsing the source file."""
+
+    def __init__(self, filename):
+        super().__init__(f"The file {filename} cannot be parsed")
+
+
 class MauReader(BaseReader):
     """Mau Reader class method."""
 
     enabled = mau_enabled
     file_extensions = ("mau",)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def read(self, source_path):
+        self.environment = Environment()
         config = self.settings.get("MAU", {})
 
         output_format = config.get("output_format", "html")
 
         if output_format not in visitors:
             raise OutputFormatNotSupported(output_format)
 
-        custom_templates = config.get("custom_templates", {})
-        templates_directory = config.get("templates_directory", None)
         visitor_class = visitors[output_format]
+        self.environment.setvar("mau.visitor.class", visitor_class)
+        self.environment.setvar("mau.visitor.format", output_format)
+
+        # Import Mau settings from Pelican settings
+        self.environment.update(self.settings.get("MAU", {}))
 
         self._source_path = source_path
-        self._mau = Mau(
+
+        mau = Mau(
             source_path,
-            visitor_class=visitor_class,
-            config=config,
-            custom_templates=custom_templates,
-            templates_directory=templates_directory,
+            self.environment,
         )
 
-        with pelican_open(source_path) as text:
-            lexer = self._mau.run_lexer(text)
+        try:
+            with pelican_open(source_path) as text:
+                mau.run_lexer(text)
+
+            # Run the Mau parser
+            mau.run_parser(mau.lexer.tokens)
+
+            # These are the templates prefixes
+            prefixes = [
+                self.environment.getvar("pelican.series"),
+                self.environment.getvar("pelican.template"),
+            ]
+            prefixes = [i for i in prefixes if i is not None]
+            self.environment.setvar("mau.visitor.prefixes", prefixes)
+
+            # Run the visitor on the main content
+            content = mau.run_visitor(mau.parser.output["content"])
+            if visitor_class.transform:
+                content = visitor_class.transform(content)
+
+            metadata = self._parse_metadata()
+
+            prefixes = [f"{i}.page" for i in prefixes] + ["page"]
+            self.environment.setvar("mau.visitor.prefixes", prefixes)
 
-        parser = self._mau.run_parser(lexer.tokens)
-        content = self._mau.process(parser.nodes, parser.environment)
+            metadata["mau"] = {}
+            metadata["mau"]["toc"] = mau.run_visitor(mau.parser.output["toc"])
 
-        if visitor_class.transform:
-            content = visitor_class.transform(content)
+        except MauErrorException as exception:
+            print_error(exception.error)
 
-        metadata = self._parse_metadata(self._mau.environment.asdict()["pelican"])
+            raise ErrorInSourceFile(source_path) from exception
 
         return content, metadata
 
-    def _parse_metadata(self, meta):
+    def _parse_metadata(self):
         """Return the dict containing document metadata."""
+        meta = self.environment.getvar("pelican").asdict()
+
         formatted_fields = self.settings["FORMATTED_FIELDS"]
 
+        mau = Mau(
+            self._source_path,
+            self.environment,
+        )
+
         output = {}
         for name, value in meta.items():
             name = name.lower()
             if name in formatted_fields:
-                lexer = self._mau.run_lexer(value)
-                parser = self._mau.run_parser(lexer.tokens)
-                formatted = self._mau.process(parser.nodes, parser.environment)
+                mau.run_lexer(value)
+                mau.run_parser(mau.lexer.tokens)
+                formatted = mau.run_visitor(mau.parser.output["content"])
                 output[name] = self.process_metadata(name, formatted)
             elif len(value) > 1:
                 # handle list metadata as list of string
                 output[name] = self.process_metadata(name, value)
             else:
                 # otherwise, handle metadata as single string
                 output[name] = self.process_metadata(name, value[0])
```

### Comparing `pelican_mau_reader-3.0.1/README.md` & `pelican_mau_reader-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican_mau_reader-3.0.1/pyproject.toml` & `pelican_mau_reader-4.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,135 @@
 [project]
 name = "pelican-mau-reader"
-version = "3.0.1"
+version = "4.0.0"
 description = "Pelican plugin that converts Mau-formatted content into HTML"
-authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}, {name = "Justin Mayer", email = "entroP@gmail.com"}]
-license = {text = "MIT"}
+authors = [
+    { name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com" },
+    { name = "Justin Mayer", email = "entroP@gmail.com" },
+]
 readme = "README.md"
-keywords = ["pelican", "plugin"]
+keywords = [
+    "pelican",
+    "plugin",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Pelican",
     "Framework :: Pelican :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8.1,<4.0"
 dependencies = [
     "pelican>=4.5",
-    "mau>=3.0.0,<4.0.0",
-    "mau-html-visitor>=1.0.0"
+    "mau>=4.0.0,<5.0.0",
+    "mau-html-visitor>=2.0.0",
 ]
 
+[project.license]
+text = "MIT"
+
 [project.urls]
 Homepage = "https://github.com/pelican-plugins/mau-reader"
 "Issue Tracker" = "https://github.com/pelican-plugins/mau-reader/issues"
 Funding = "https://donate.getpelican.com/"
 
 [project.optional-dependencies]
-markdown = ["markdown>=3.4"]
+markdown = [
+    "markdown>=3.4",
+]
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black>=23.7.0",
     "invoke>=2.2.0",
-    "ruff>=0.0.280",
+    "ruff>=0.1.8",
 ]
 test = [
     "markdown>=3.4",
     "pytest>=7.0",
     "pytest-cov>=4.0",
     "pytest-sugar>=0.9.7",
+    "mau>=4.0.0,<5.0.0",
+    "mau-html-visitor>=2.0.0",
+]
+
+[tool.pdm.build]
+source-includes = [
+    "CHANGELOG.md",
+    "CONTRIBUTING.md",
+]
+includes = [
+    "pelican/",
+]
+excludes = [
+    "tasks.py",
 ]
 
 [tool.autopub]
 project-name = "Mau Reader"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
 select = [
-  "B",   # flake8-bugbear
-  "BLE", # flake8-blind-except
-  "C4",  # flake8-comprehensions
-  "D",   # pydocstyle
-  "E",   # pycodestyle
-  "F",   # pyflakes
-  "I",   # isort
-  "ICN", # flake8-import-conventions
-  "ISC", # flake8-implicit-str-concat
-  "PGH", # pygrep-hooks
-  "PL",  # pylint
-  "RET", # flake8-return
-  "RUF", # ruff-specific rules
-  "SIM", # flake8-simplify
-  "T10", # flake8-debugger
-  "T20", # flake8-print
-  "TID", # flake8-tidy-imports
-  "TRY", # tryceratops
-  "UP",  # pyupgrade
-  "W",   # pycodestyle
-  "YTT", # flake8-2020
+    "B",
+    "BLE",
+    "C4",
+    "D",
+    "E",
+    "F",
+    "I",
+    "ICN",
+    "ISC",
+    "PGH",
+    "PL",
+    "RET",
+    "RUF",
+    "SIM",
+    "T10",
+    "T20",
+    "TID",
+    "TRY",
+    "UP",
+    "W",
+    "YTT",
 ]
-
 ignore = [
-  "D100",    # missing docstring in public module
-  "D102",    # missing docstring in public method
-  "D104",    # missing docstring in public package
-  "D107",    # missing docstring in `__init__` function
-  "D203",    # blank line before class docstring
-  "D213",    # multi-line docstring summary should start at the second line
-  "PLW2901", # `for` loop variable overwritten by assignment target
+    "D100",
+    "D102",
+    "D104",
+    "D107",
+    "D203",
+    "D213",
+    "PLW2901",
 ]
 
-target-version = "py38"
-
 [tool.ruff.per-file-ignores]
-"**/test_mau_reader.py" = ["D103", "E501"]
+"**/test_mau_reader.py" = [
+    "D103",
+    "E501",
+]
 
 [tool.ruff.isort]
 combine-as-imports = true
 force-sort-within-sections = true
-known-first-party = ["pelican"]
+known-first-party = [
+    "pelican",
+]
 
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `pelican_mau_reader-3.0.1/PKG-INFO` & `pelican_mau_reader-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pelican-mau-reader
-Version: 3.0.1
+Version: 4.0.0
 Summary: Pelican plugin that converts Mau-formatted content into HTML
-Project-URL: Homepage, https://github.com/pelican-plugins/mau-reader
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/mau-reader/issues
-Project-URL: Funding, https://donate.getpelican.com/
-Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>, Justin Mayer <entroP@gmail.com>
-License: MIT
 Keywords: pelican,plugin
+Author-Email: Leonardo Giordani <giordani.leonardo@gmail.com>, Justin Mayer <entroP@gmail.com>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Homepage, https://github.com/pelican-plugins/mau-reader
+Project-URL: Issue tracker, https://github.com/pelican-plugins/mau-reader/issues
+Project-URL: Funding, https://donate.getpelican.com/
 Requires-Python: <4.0,>=3.8.1
-Requires-Dist: mau-html-visitor>=1.0.0
-Requires-Dist: mau<4.0.0,>=3.0.0
 Requires-Dist: pelican>=4.5
+Requires-Dist: mau<5.0.0,>=4.0.0
+Requires-Dist: mau-html-visitor>=2.0.0
+Requires-Dist: markdown>=3.4; extra == "markdown"
 Provides-Extra: markdown
-Requires-Dist: markdown>=3.4; extra == 'markdown'
 Description-Content-Type: text/markdown
 
 # Mau Reader: A Plugin for Pelican
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/mau-reader/main.yml?branch=main)](https://github.com/pelican-plugins/mau-reader/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-mau-reader)](https://pypi.org/project/pelican-mau-reader/)
 [![Downloads](https://img.shields.io/pypi/dm/pelican-mau-reader)](https://pypi.org/project/pelican-mau-reader/)
```

