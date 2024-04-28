# Comparing `tmp/mau_tex_visitor-1.1.1.tar.gz` & `tmp/mau_tex_visitor-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau_tex_visitor-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau_tex_visitor-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau_tex_visitor-1.1.1.tar` & `mau_tex_visitor-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,41 @@
--rw-r--r--   0        0        0      225 2023-11-13 17:01:37.002662 mau_tex_visitor-1.1.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-15 11:48:05.519329 mau_tex_visitor-1.1.1/LICENSE
--rw-r--r--   0        0        0      890 2023-08-15 11:56:07.028986 mau_tex_visitor-1.1.1/README.md
--rw-r--r--   0        0        0     4172 2024-04-12 13:51:36.449526 mau_tex_visitor-1.1.1/mau_tex_visitor/__init__.py
--rw-r--r--   0        0        0     1933 2024-04-12 13:52:23.605909 mau_tex_visitor-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 mau_tex_visitor-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3077 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/.gitignore
+-rw-r--r--   0        0        0      390 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-15 11:48:05.519329 mau_tex_visitor-2.0.0/LICENSE
+-rw-r--r--   0        0        0      890 2023-08-15 11:56:07.028986 mau_tex_visitor-2.0.0/README.md
+-rw-r--r--   0        0        0     2197 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/block.tex
+-rw-r--r--   0        0        0       76 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/block/admonition.tex
+-rw-r--r--   0        0        0       57 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/block/quote.tex
+-rw-r--r--   0        0        0       63 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/block_group.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/callout.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/callouts_entry.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/command.tex
+-rw-r--r--   0        0        0       14 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/container.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/content.tex
+-rw-r--r--   0        0        0      196 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/content_image.tex
+-rw-r--r--   0        0        0       14 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/document.tex
+-rw-r--r--   0        0        0       27 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/footnote.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/footnotes.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/footnotes_entry.tex
+-rw-r--r--   0        0        0       48 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/header.tex
+-rw-r--r--   0        0        0       45 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/horizontal_rule.tex
+-rw-r--r--   0        0        0      253 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/list.tex
+-rw-r--r--   0        0        0       40 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/list_item.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/macro.tex
+-rw-r--r--   0        0        0       12 2024-04-28 20:15:12.765816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/macro/class.tex
+-rw-r--r--   0        0        0       30 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/macro/image.tex
+-rw-r--r--   0        0        0       36 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/macro/link.tex
+-rw-r--r--   0        0        0       44 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/paragraph.tex
+-rw-r--r--   0        0        0       12 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/raw.tex
+-rw-r--r--   0        0        0       14 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/sentence.tex
+-rw-r--r--   0        0        0       58 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/source.tex
+-rw-r--r--   0        0        0       34 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/style/caret.tex
+-rw-r--r--   0        0        0       25 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/style/star.tex
+-rw-r--r--   0        0        0       32 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/style/tilde.tex
+-rw-r--r--   0        0        0       25 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/style/underscore.tex
+-rw-r--r--   0        0        0       12 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/text.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/toc_entry.tex
+-rw-r--r--   0        0        0        0 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/tox.tex
+-rw-r--r--   0        0        0       23 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/mau_tex_visitor/templates/verbatim.tex
+-rw-r--r--   0        0        0     1935 2024-04-28 20:15:12.769816 mau_tex_visitor-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 mau_tex_visitor-2.0.0/PKG-INFO
```

### Comparing `mau_tex_visitor-1.1.1/LICENSE` & `mau_tex_visitor-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mau_tex_visitor-1.1.1/README.md` & `mau_tex_visitor-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mau_tex_visitor-1.1.1/pyproject.toml` & `mau_tex_visitor-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau_tex_visitor"
-version = "1.1.1"
+version = "2.0.0"
 description = "A visitor for Mau that converts the AST into TeX"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
@@ -19,15 +19,15 @@
 "Programming Language :: Python :: 3.8",
 "Programming Language :: Python :: 3.9",
 "Programming Language :: Python :: 3.10",
 "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
 dependencies = [
-"mau>=3.0.0,<4.0.0",
+    "mau>=4.0.0,<5.0.0",
 ]
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/Project-Mau/mau-tex-visitor"
 
 [project.optional-dependencies]
@@ -79,9 +79,7 @@
 [tool.pytest.ini_options]
 addopts = """\
 --cov mau \
 --cov tests \
 --cov-report term-missing \
 --no-cov-on-fail \
 """
-
-
```

### Comparing `mau_tex_visitor-1.1.1/PKG-INFO` & `mau_tex_visitor-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau_tex_visitor
-Version: 1.1.1
+Version: 2.0.0
 Summary: A visitor for Mau that converts the AST into TeX
 Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: mau>=3.0.0,<4.0.0
+Requires-Dist: mau>=4.0.0,<5.0.0
 Project-URL: Home, https://github.com/Project-Mau/mau-tex-visitor
 Provides-Extra: development
 Provides-Extra: testing
 
 # Mau TeX Visitor
 
 This is a plugin for the [Mau](https://github.com/Project-Mau/mau) markup language. The plugin provides the conversion from Mau source to TeX.
```

