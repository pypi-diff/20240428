# Comparing `tmp/mau_html_visitor-1.1.2.tar.gz` & `tmp/mau_html_visitor-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau_html_visitor-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau_html_visitor-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau_html_visitor-1.1.2.tar` & `mau_html_visitor-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,39 @@
--rw-r--r--   0        0        0      328 2023-11-13 17:09:55.781826 mau_html_visitor-1.1.2/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-1.1.2/LICENSE
--rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-1.1.2/README.md
--rw-r--r--   0        0        0     6840 2024-04-12 13:49:39.064573 mau_html_visitor-1.1.2/mau_html_visitor/__init__.py
--rw-r--r--   0        0        0     1950 2024-04-12 13:52:29.413956 mau_html_visitor-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 mau_html_visitor-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3077 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/.gitignore
+-rw-r--r--   0        0        0      493 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-2.0.0/LICENSE
+-rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-2.0.0/README.md
+-rw-r--r--   0        0        0     3572 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/__init__.py
+-rw-r--r--   0        0        0      210 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block.html
+-rw-r--r--   0        0        0      190 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block/admonition.html
+-rw-r--r--   0        0        0       82 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block/quote.html
+-rw-r--r--   0        0        0      143 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/block_group.html
+-rw-r--r--   0        0        0       42 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/callout.html
+-rw-r--r--   0        0        0       87 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/callouts_entry.html
+-rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/container.html
+-rw-r--r--   0        0        0      211 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/content_image.html
+-rw-r--r--   0        0        0       60 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/document.html
+-rw-r--r--   0        0        0       94 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnote.html
+-rw-r--r--   0        0        0       45 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnotes.html
+-rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/footnotes_entry.html
+-rw-r--r--   0        0        0       59 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/header.html
+-rw-r--r--   0        0        0        5 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/horizontal_rule.html
+-rw-r--r--   0        0        0      119 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/list.html
+-rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/list_item.html
+-rw-r--r--   0        0        0       61 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/class.html
+-rw-r--r--   0        0        0       49 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/header.html
+-rw-r--r--   0        0        0      102 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/image.html
+-rw-r--r--   0        0        0       41 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/macro/link.html
+-rw-r--r--   0        0        0       21 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/paragraph.html
+-rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/raw.html
+-rw-r--r--   0        0        0       14 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/sentence.html
+-rw-r--r--   0        0        0      467 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/source.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/caret.html
+-rw-r--r--   0        0        0       31 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/star.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/tilde.html
+-rw-r--r--   0        0        0       23 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/style/underscore.html
+-rw-r--r--   0        0        0       12 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/text.html
+-rw-r--r--   0        0        0       70 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/toc.html
+-rw-r--r--   0        0        0      107 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/toc_entry.html
+-rw-r--r--   0        0        0       25 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/mau_html_visitor/templates/verbatim.html
+-rw-r--r--   0        0        0     1949 2024-04-28 20:13:14.221030 mau_html_visitor-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 mau_html_visitor-2.0.0/PKG-INFO
```

### Comparing `mau_html_visitor-1.1.2/LICENSE` & `mau_html_visitor-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-1.1.2/README.md` & `mau_html_visitor-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-1.1.2/pyproject.toml` & `mau_html_visitor-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau_html_visitor"
-version = "1.1.2"
+version = "2.0.0"
 description = "A visitor for Mau that converts the AST into HTML"
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
+"mau>=4.0.0,<5.0.0",
 "pygments",
 ]
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/Project-Mau/mau-html-visitor"
 
@@ -81,8 +81,7 @@
 addopts = """\
 --cov mau \
 --cov tests \
 --cov-report term-missing \
 --no-cov-on-fail \
 """
 
-
```

### Comparing `mau_html_visitor-1.1.2/PKG-INFO` & `mau_html_visitor-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau_html_visitor
-Version: 1.1.2
+Version: 2.0.0
 Summary: A visitor for Mau that converts the AST into HTML
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
 Requires-Dist: pygments
 Project-URL: Home, https://github.com/Project-Mau/mau-html-visitor
 Provides-Extra: development
 Provides-Extra: testing
 
 # Mau HTML Visitor
```

