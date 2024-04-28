# Comparing `tmp/medium_to_markdown_py-1.0.3.tar.gz` & `tmp/medium_to_markdown_py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.0.3.tar", last modified: Sun Apr 28 14:32:20 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.0.4.tar", last modified: Sun Apr 28 14:35:44 2024, max compression
```

## Comparing `medium_to_markdown_py-1.0.3.tar` & `medium_to_markdown_py-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:32:20.606641 medium_to_markdown_py-1.0.3/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.3/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:32:20.606574 medium_to_markdown_py-1.0.3/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.3/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:32:20.605169 medium_to_markdown_py-1.0.3/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:32:09.000000 medium_to_markdown_py-1.0.3/medium_to_markdown/__init__.py
--rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:27:56.000000 medium_to_markdown_py-1.0.3/medium_to_markdown/medium_to_markdown.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:32:20.606363 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      433 2024-04-28 14:32:20.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      376 2024-04-28 14:32:20.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:32:20.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:32:20.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-28 14:32:20.000000 medium_to_markdown_py-1.0.3/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:32:20.606859 medium_to_markdown_py-1.0.3/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      599 2024-04-28 14:32:10.000000 medium_to_markdown_py-1.0.3/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:35:44.710473 medium_to_markdown_py-1.0.4/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.4/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:35:44.710402 medium_to_markdown_py-1.0.4/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.4/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:35:44.708925 medium_to_markdown_py-1.0.4/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:35:33.000000 medium_to_markdown_py-1.0.4/medium_to_markdown/__init__.py
+-rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:27:56.000000 medium_to_markdown_py-1.0.4/medium_to_markdown/medium_to_markdown.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:35:44.710181 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:35:44.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      376 2024-04-28 14:35:44.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:35:44.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:35:44.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-28 14:35:44.000000 medium_to_markdown_py-1.0.4/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:35:44.710688 medium_to_markdown_py-1.0.4/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-28 14:35:30.000000 medium_to_markdown_py-1.0.4/setup.py
```

### Comparing `medium_to_markdown_py-1.0.3/LICENSE` & `medium_to_markdown_py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.3/README.md` & `medium_to_markdown_py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.3/medium_to_markdown/medium_to_markdown.py` & `medium_to_markdown_py-1.0.4/medium_to_markdown/medium_to_markdown.py`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.3/setup.py` & `medium_to_markdown_py-1.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='medium-to-markdown-py',
-    version='1.0.3',
-    description='medium-to-markdown-py is a Python package that converts Medium articles to Markdown format.',
+    name='medium_to_markdown_py',
+    version='1.0.4',
+    description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
     python_requires='>=3.6',
```
