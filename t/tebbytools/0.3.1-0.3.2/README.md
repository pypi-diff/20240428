# Comparing `tmp/tebbytools-0.3.1.tar.gz` & `tmp/tebbytools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tebbytools-0.3.1.tar", last modified: Sat Apr 27 22:31:16 2024, max compression
+gzip compressed data, was "tebbytools-0.3.2.tar", last modified: Sat Apr 27 22:40:11 2024, max compression
```

## Comparing `tebbytools-0.3.1.tar` & `tebbytools-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.323503 tebbytools-0.3.1/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:31:16.323280 tebbytools-0.3.1/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2783 2024-04-27 22:29:15.000000 tebbytools-0.3.1/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-27 22:31:16.323576 tebbytools-0.3.1/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-27 22:31:11.000000 tebbytools-0.3.1/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.320954 tebbytools-0.3.1/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.321678 tebbytools-0.3.1/src/tebbytools/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       99 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/__init__.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.322835 tebbytools-0.3.1/src/tebbytools/quickquiz/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       33 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2319 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/quickquiz.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1912 2024-04-27 22:29:15.000000 tebbytools-0.3.1/src/tebbytools/quickquiz/quiz.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.1/src/tebbytools/reviewlist.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.3.1/src/tebbytools/wordbank.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:31:16.323024 tebbytools-0.3.1/src/tebbytools.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      361 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-27 22:31:16.000000 tebbytools-0.3.1/src/tebbytools.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:40:11.701315 tebbytools-0.3.2/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      307 2024-04-27 22:40:11.701059 tebbytools-0.3.2/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2783 2024-04-27 22:29:15.000000 tebbytools-0.3.2/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-27 22:40:11.701364 tebbytools-0.3.2/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      519 2024-04-27 22:39:46.000000 tebbytools-0.3.2/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:40:11.697846 tebbytools-0.3.2/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:40:11.698802 tebbytools-0.3.2/src/tebbytools/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       99 2024-04-27 22:29:15.000000 tebbytools-0.3.2/src/tebbytools/__init__.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:40:11.700441 tebbytools-0.3.2/src/tebbytools/quickquiz/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       33 2024-04-27 22:29:15.000000 tebbytools-0.3.2/src/tebbytools/quickquiz/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2319 2024-04-27 22:29:15.000000 tebbytools-0.3.2/src/tebbytools/quickquiz/quickquiz.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1912 2024-04-27 22:29:15.000000 tebbytools-0.3.2/src/tebbytools/quickquiz/quiz.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.3.2/src/tebbytools/reviewlist.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.3.2/src/tebbytools/wordbank.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-27 22:40:11.700778 tebbytools-0.3.2/src/tebbytools.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      307 2024-04-27 22:40:11.000000 tebbytools-0.3.2/src/tebbytools.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      398 2024-04-27 22:40:11.000000 tebbytools-0.3.2/src/tebbytools.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-27 22:40:11.000000 tebbytools-0.3.2/src/tebbytools.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        6 2024-04-27 22:40:11.000000 tebbytools-0.3.2/src/tebbytools.egg-info/requires.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-27 22:40:11.000000 tebbytools-0.3.2/src/tebbytools.egg-info/top_level.txt
```

### Comparing `tebbytools-0.3.1/README.md` & `tebbytools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tebbytools-0.3.1/src/tebbytools/quickquiz/quickquiz.py` & `tebbytools-0.3.2/src/tebbytools/quickquiz/quickquiz.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.3.1/src/tebbytools/quickquiz/quiz.py` & `tebbytools-0.3.2/src/tebbytools/quickquiz/quiz.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.3.1/src/tebbytools/reviewlist.py` & `tebbytools-0.3.2/src/tebbytools/reviewlist.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.3.1/src/tebbytools/wordbank.py` & `tebbytools-0.3.2/src/tebbytools/wordbank.py`

 * *Files identical despite different names*

