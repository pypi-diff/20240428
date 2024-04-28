# Comparing `tmp/bibfish-0.3.0.tar.gz` & `tmp/bibfish-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibfish-0.3.0.tar", last modified: Wed Mar 20 19:06:35 2024, max compression
+gzip compressed data, was "bibfish-0.3.1.tar", last modified: Sun Apr 28 11:00:19 2024, max compression
```

## Comparing `bibfish-0.3.0.tar` & `bibfish-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-03-20 19:06:35.994485 bibfish-0.3.0/
--rw-r--r--   0 jon        (501) staff       (20)     2017 2024-03-20 19:01:51.000000 bibfish-0.3.0/HISTORY.md
--rw-r--r--   0 jon        (501) staff       (20)     1094 2023-01-06 10:22:44.000000 bibfish-0.3.0/LICENSE.md
--rw-r--r--   0 jon        (501) staff       (20)     5436 2024-03-20 19:06:35.994266 bibfish-0.3.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     4779 2024-03-20 18:40:56.000000 bibfish-0.3.0/README.md
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-03-20 19:06:35.992326 bibfish-0.3.0/bibfish/
--rw-r--r--   0 jon        (501) staff       (20)     9324 2024-03-20 18:47:01.000000 bibfish-0.3.0/bibfish/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)       21 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish/_version.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-03-20 19:06:35.993993 bibfish-0.3.0/bibfish.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     5436 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      398 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       40 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/entry_points.txt
--rw-r--r--   0 jon        (501) staff       (20)       20 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)        8 2024-03-20 19:06:35.000000 bibfish-0.3.0/bibfish.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)      948 2024-03-20 16:56:12.000000 bibfish-0.3.0/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2024-03-20 19:06:35.994520 bibfish-0.3.0/setup.cfg
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-03-20 19:06:35.993836 bibfish-0.3.0/tests/
--rw-r--r--   0 jon        (501) staff       (20)        0 2024-03-20 17:59:42.000000 bibfish-0.3.0/tests/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    10028 2024-03-20 18:33:19.000000 bibfish-0.3.0/tests/bibfile1.bib
--rw-r--r--   0 jon        (501) staff       (20)     9230 2024-03-20 18:07:17.000000 bibfish-0.3.0/tests/bibfile2.bib
--rw-r--r--   0 jon        (501) staff       (20)    19627 2023-10-10 14:49:38.000000 bibfish-0.3.0/tests/expected_output1.bib
--rw-r--r--   0 jon        (501) staff       (20)    97663 2024-03-20 18:33:27.000000 bibfish-0.3.0/tests/manuscript1.tex
--rw-r--r--   0 jon        (501) staff       (20)      895 2024-03-20 18:17:59.000000 bibfish-0.3.0/tests/test_main.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-28 11:00:19.751683 bibfish-0.3.1/
+-rw-r--r--   0 jon        (501) staff       (20)     2161 2024-04-28 10:54:45.000000 bibfish-0.3.1/HISTORY.md
+-rw-r--r--   0 jon        (501) staff       (20)     1094 2023-01-06 10:22:44.000000 bibfish-0.3.1/LICENSE.md
+-rw-r--r--   0 jon        (501) staff       (20)     5436 2024-04-28 11:00:19.751421 bibfish-0.3.1/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     4779 2024-03-20 18:40:56.000000 bibfish-0.3.1/README.md
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-28 11:00:19.749081 bibfish-0.3.1/bibfish/
+-rw-r--r--   0 jon        (501) staff       (20)     9538 2024-04-28 10:43:32.000000 bibfish-0.3.1/bibfish/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)       21 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish/_version.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-28 11:00:19.751111 bibfish-0.3.1/bibfish.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)     5436 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      417 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       40 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (501) staff       (20)       20 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)        8 2024-04-28 11:00:19.000000 bibfish-0.3.1/bibfish.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)      948 2024-03-20 16:56:12.000000 bibfish-0.3.1/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2024-04-28 11:00:19.751727 bibfish-0.3.1/setup.cfg
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-28 11:00:19.750913 bibfish-0.3.1/tests/
+-rw-r--r--   0 jon        (501) staff       (20)        0 2024-03-20 17:59:42.000000 bibfish-0.3.1/tests/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    10028 2024-03-20 18:33:19.000000 bibfish-0.3.1/tests/bibfile1.bib
+-rw-r--r--   0 jon        (501) staff       (20)     9230 2024-03-20 18:07:17.000000 bibfish-0.3.1/tests/bibfile2.bib
+-rw-r--r--   0 jon        (501) staff       (20)    19627 2023-10-10 14:49:38.000000 bibfish-0.3.1/tests/expected_output1.bib
+-rw-r--r--   0 jon        (501) staff       (20)    97663 2024-03-20 18:33:27.000000 bibfish-0.3.1/tests/manuscript1.tex
+-rw-r--r--   0 jon        (501) staff       (20)     1949 2024-04-28 10:56:35.000000 bibfish-0.3.1/tests/test_init.py
+-rw-r--r--   0 jon        (501) staff       (20)      895 2024-03-20 18:17:59.000000 bibfish-0.3.1/tests/test_main.py
```

### Comparing `bibfish-0.3.0/HISTORY.md` & `bibfish-0.3.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+bibfish 0.3.1 - 2024-04-28
+==========================
+
+Changed
+-------
+
+- Bibfish will now ignore commented out lines in the manuscript file.
+
+
 bibfish 0.3 - 2024-03-20
 ========================
 
 Added
 -----
 
 - Support for crossrefs. Cross-referenced Bibtex entries will be extracted automatically and placed in the output bib file.
```

### Comparing `bibfish-0.3.0/LICENSE.md` & `bibfish-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/PKG-INFO` & `bibfish-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibfish
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extract entries from a .bib file that are cited in a .tex file
 Author-email: Jon Carr <jon.carr@rhul.ac.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcarr/bibfish
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bibfish-0.3.0/README.md` & `bibfish-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/bibfish/__init__.py` & `bibfish-0.3.1/bibfish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,22 @@
     Search manuscript_file for any cite commands and return the citekeys they
     make reference to. If the manuscript has any nested files (through input,
     import, or include), these will be resursively expanded.
     """
     if len(cite_commands) == 0:
         return []
     with open(manuscript_file, "r") as file:
-        manuscript = file.read()
+        full_manuscript = file.read()
+
+    uncommented_lines = []
+    for line in full_manuscript.splitlines():
+        if not line.strip().startswith("%"):
+            uncommented_lines.append(line)
+    manuscript = "\n".join(uncommented_lines)
+
     citekeys = []
     try:
         manuscript = manuscript.split(r"\begin{document}")[1]
     except IndexError:
         pass
     for nestfile in find_imported_files(manuscript):
         try:
```

### Comparing `bibfish-0.3.0/bibfish.egg-info/PKG-INFO` & `bibfish-0.3.1/bibfish.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibfish
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extract entries from a .bib file that are cited in a .tex file
 Author-email: Jon Carr <jon.carr@rhul.ac.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcarr/bibfish
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bibfish-0.3.0/pyproject.toml` & `bibfish-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/tests/bibfile1.bib` & `bibfish-0.3.1/tests/bibfile1.bib`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/tests/bibfile2.bib` & `bibfish-0.3.1/tests/bibfile2.bib`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/tests/expected_output1.bib` & `bibfish-0.3.1/tests/expected_output1.bib`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/tests/manuscript1.tex` & `bibfish-0.3.1/tests/manuscript1.tex`

 * *Files identical despite different names*

### Comparing `bibfish-0.3.0/tests/test_main.py` & `bibfish-0.3.1/tests/test_main.py`

 * *Files identical despite different names*

