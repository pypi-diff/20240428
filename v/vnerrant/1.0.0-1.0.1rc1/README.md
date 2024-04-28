# Comparing `tmp/vnerrant-1.0.0.tar.gz` & `tmp/vnerrant-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnerrant-1.0.0.tar", last modified: Tue Feb 13 07:40:54 2024, max compression
+gzip compressed data, was "vnerrant-1.0.1rc1.tar", last modified: Sun Apr 28 07:09:41 2024, max compression
```

## Comparing `vnerrant-1.0.0.tar` & `vnerrant-1.0.1rc1.tar`

### file list

```diff
@@ -1,56 +1,63 @@
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.264263 vnerrant-1.0.0/
--rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-13 06:51:25.000000 vnerrant-1.0.0/MANIFEST.in
--rw-r--r--   0 manred1997   (501) staff       (20)     9555 2024-02-13 07:40:54.263957 vnerrant-1.0.0/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     8613 2024-02-13 07:33:13.000000 vnerrant-1.0.0/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-02-13 07:40:54.264317 vnerrant-1.0.0/setup.cfg
--rw-r--r--   0 manred1997   (501) staff       (20)     1524 2024-02-13 07:38:22.000000 vnerrant-1.0.0/setup.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.252178 vnerrant-1.0.0/vnerrant/
--rw-r--r--   0 manred1997   (501) staff       (20)     1076 2024-02-13 07:38:08.000000 vnerrant-1.0.0/vnerrant/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10483 2024-02-13 07:24:36.000000 vnerrant-1.0.0/vnerrant/annotator.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.254076 vnerrant-1.0.0/vnerrant/cli/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/cli/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-13 07:24:36.000000 vnerrant-1.0.0/vnerrant/cli/convert.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-08 10:06:36.000000 vnerrant-1.0.0/vnerrant/cli/evaluate.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.256446 vnerrant-1.0.0/vnerrant/components/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-07 05:25:14.000000 vnerrant-1.0.0/vnerrant/components/alignment.py
--rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-08 10:02:08.000000 vnerrant-1.0.0/vnerrant/components/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6246 2024-02-13 05:49:43.000000 vnerrant-1.0.0/vnerrant/components/converter.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.258225 vnerrant-1.0.0/vnerrant/components/en/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/en/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    30380 2024-02-13 07:24:36.000000 vnerrant-1.0.0/vnerrant/components/en/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-13 07:24:36.000000 vnerrant-1.0.0/vnerrant/components/en/constants.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/en/lancaster.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10873 2024-02-08 10:02:09.000000 vnerrant-1.0.0/vnerrant/components/en/merger.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.258951 vnerrant-1.0.0/vnerrant/components/en/resources/
--rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/en/resources/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/en/resources/en-ptb_map
--rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/components/en/resources/en_GB-large.txt
--rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-08 09:32:17.000000 vnerrant-1.0.0/vnerrant/components/en/utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-08 10:02:11.000000 vnerrant-1.0.0/vnerrant/components/evaluater.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3083 2024-02-08 10:02:07.000000 vnerrant-1.0.0/vnerrant/components/merger.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-13 07:24:36.000000 vnerrant-1.0.0/vnerrant/components/tokenizer.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.260766 vnerrant-1.0.0/vnerrant/config/
--rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-13 07:24:07.000000 vnerrant-1.0.0/vnerrant/config/mapping_type_error.yaml
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-04 18:37:39.000000 vnerrant-1.0.0/vnerrant/config.py
--rw-r--r--   0 manred1997   (501) staff       (20)      785 2024-02-13 07:24:08.000000 vnerrant-1.0.0/vnerrant/constants.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.261231 vnerrant-1.0.0/vnerrant/metrics/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/metrics/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-04 18:37:39.000000 vnerrant-1.0.0/vnerrant/metrics/criteria.py
--rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/metrics/stats.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.261833 vnerrant-1.0.0/vnerrant/model/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/model/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6791 2024-02-04 18:42:59.000000 vnerrant-1.0.0/vnerrant/model/edit.py
--rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-08 10:02:13.000000 vnerrant-1.0.0/vnerrant/run_cli.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.263139 vnerrant-1.0.0/vnerrant/utils/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/utils/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-04 03:13:59.000000 vnerrant-1.0.0/vnerrant/utils/helper.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-08 10:02:09.000000 vnerrant-1.0.0/vnerrant/utils/pretty_results.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-09 04:16:28.000000 vnerrant-1.0.0/vnerrant/utils/utils.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-02-13 07:40:54.263623 vnerrant-1.0.0/vnerrant.egg-info/
--rw-r--r--   0 manred1997   (501) staff       (20)     9555 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     1258 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/SOURCES.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/dependency_links.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/entry_points.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/requires.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-02-13 07:40:54.000000 vnerrant-1.0.0/vnerrant.egg-info/top_level.txt
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.127676 vnerrant-1.0.1rc1/
+-rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-04-28 07:09:41.127067 vnerrant-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-04-28 07:09:41.127716 vnerrant-1.0.1rc1/setup.cfg
+-rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-04-28 07:09:29.000000 vnerrant-1.0.1rc1/setup.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.111078 vnerrant-1.0.1rc1/tests/
+-rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/tests/test_vnerrant.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.112774 vnerrant-1.0.1rc1/vnerrant/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-04-28 07:09:25.000000 vnerrant-1.0.1rc1/vnerrant/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    11910 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/annotator.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.114196 vnerrant-1.0.1rc1/vnerrant/cli/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/convert.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/evaluate.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.116223 vnerrant-1.0.1rc1/vnerrant/components/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/alignment.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/converter.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.118517 vnerrant-1.0.1rc1/vnerrant/components/en/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/constants.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/lancaster.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/merger.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.119985 vnerrant-1.0.1rc1/vnerrant/components/en/resources/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/en-ptb_map
+-rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/en_GB-large.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/evaluater.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/merger.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/tokenizer.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.123707 vnerrant-1.0.1rc1/vnerrant/config/
+-rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/config/errant_verbose.json
+-rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/config/mapping_type_error.yaml
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/config.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/constants.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.124123 vnerrant-1.0.1rc1/vnerrant/metrics/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/criteria.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/stats.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.124556 vnerrant-1.0.1rc1/vnerrant/model/
+-rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/model/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/model/edit.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/run_cli.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.126653 vnerrant-1.0.1rc1/vnerrant/utils/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6734 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/utils/edit_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/helper.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/pretty_results.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/utils/string_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/utils.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.126838 vnerrant-1.0.1rc1/vnerrant.egg-info/
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/SOURCES.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/dependency_links.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/entry_points.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/requires.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/top_level.txt
```

### Comparing `vnerrant-1.0.0/PKG-INFO` & `vnerrant-1.0.1rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.0
+Version: 1.0.1rc1
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,19 @@
 Requires-Dist: spacy>=3
 Requires-Dist: rapidfuzz>=2.0.0
 
 # VNERRANT v1.0.0
 
 ## Overview
 
-The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information. Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the former to the latter and classify them according to a rule-based error type framework. This can be used to standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in M2 format and an evaluation script is provided.
+The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information.
+Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the
+former to the latter and classify them according to a rule-based error type framework. This can be used to
+standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in
+M2 format and an evaluation script is provided.
 
 ### Example
 
 **Original**: This are gramamtical sentence .
 **Corrected**: This is a grammatical sentence .
 **Output M2**:
 
@@ -54,18 +58,18 @@
 - Option 1: Install VNERRANT using pip with the following commands:
 
 ```bash
 pip install -U pip setuptools wheel
 pip install vnerrant
 ```
 
-- Option 2: Alternatively, if you want to install ERRANT from the source, you can follow these steps:
+- Option 2: Alternatively, if you want to install VNERRANT from the source, you can follow these steps:
 
 ```bash
-git clone https://gitlab.testsprep.online/nlp/research/errant
+git clone https://gitlab.testsprep.online/nlp/research/vnerrant
 cd vnerrant
 pip install -U pip setuptools wheel
 pip install -e .
 ```
 
 Please obtain a Spacy model by using the following command:
 
@@ -111,51 +115,57 @@
 vnerrant evaluate m2 -hyp <hyp_m2> -ref <ref_m2> -ds -cat {1,2,3}
 ```
 
 All these scripts also have additional advanced command line options which can be displayed using the `-h` flag.
 
 ### API
 
-As of v3.0.0, ERRANT now also comes with an API.
+As of v3.0.0, VNERRANT now also comes with an API.
 
 ### Quick Start
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 
 orig = 'My    name    is   the     John'
 cor = 'My name is John'
-edits = annotator.annotate_with_pre_and_post_processing(orig, cor)
+edits = annotator.annotate_raw(orig, cor)
 
 for e in edits:
-    print(e.o_start, e.o_end, e.o_str, e.c_start, e.c_end, e.c_str, e.type)
-    print(e.o_toks.start_char, e.o_toks.end_char)
-    # assert e.o_str == orig[e.o_toks.start_char:e.o_toks.end_char]
+    print(e.original.start_token, e.original.end_token, e.original.text)
+    print(e.corrected.start_token, e.corrected.end_token, e.corrected.text)
+    print(e.original.start_char, e.original.end_char, e.edit_type)
 ```
 
 ### Loading
 
 `vnerrant.load(lang, model_name)`
 
-Instantiate an ERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent ERRANT from loading it redundantly.
+Instantiate an VNERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent VNERRANT from loading it redundantly.
 
 ### Annotator Objects
 
-An Annotator object is the main interface for ERRANT.
+An Annotator object is the main interface for VNERRANT.
 
 #### Methods
 
 <details>
 <summary>annotator.parse</summary>
 
-`annotator.parse(string, tokenise=False)`
+`annotator.parse(string, tokenize_type='string')`
 
-Lemmatise, POS tag, and parse a text string with spacy. Set `tokenise` to True to also word tokenise with spacy. Returns a spacy Doc object.
+Lemmatise, POS tag, and parse a text string with spacy. Returns a spacy Doc object.
+
+`tokenize_type` must be in `["spacy", "split", "string"]`
+
+- `spacy`: tokenizing by default spacy tokenizer.
+- `split`: tokenizing by split function.
+- `string`: tokenizing by spacy and string tokenizer.
 
 </details>
 
 <details>
 <summary>annotator.align</summary>
 
 `annotator.align(orig, cor, lev=False)`
@@ -189,36 +199,63 @@
 </details>
 
 <details>
 <summary>annotator.annotate</summary>
 
 `annotator.annotate(orig, cor, lev=False, merging='rules')`
 
-Run the full annotation pipeline to align two sequences and extract and classify the edits. Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence. Returns a list of Edit objects.
+Run the full annotation pipeline to align two sequences and extract and classify the edits.
+Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
 
 ```python
-import errant
+import vnerrant
 
-annotator = errant.load(lang="en", model_name="en_core_web_sm")
-orig = annotator.parse('This are gramamtical sentence .')
-cor = annotator.parse('This is a grammatical sentence .')
-alignment = annotator.align(orig, cor)
-edits = annotator.merge(alignment)
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = annotator.parse("My   name   is    the    John")
+cor = annotator.parse("My name is John")
+edits = annotator.annotate(orig, cor)
+for e in edits:
+    print(e)
+```
+
+</details>
+
+<details>
+<summary>annotator.annotate_raw</summary>
+
+`annotator.annotate_raw(orig: str, cor: str, lev=False, merging='rules', tokenize_type='string')`
+
+Run the full annotation pipeline to align two strings, extract and classify the edits.
+Equivalent to running `annotator.parse`, `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
+
+```python
+import vnerrant
+
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = "My   name   is    the    John"
+cor = "My name is John"
+edits = annotator.annotate_raw(orig, cor)
 for e in edits:
-    e = annotator.classify(e)
+    print(e)
 ```
 
 </details>
 
 <details>
 <summary>annotator.import_edit</summary>
 
 `annotator.import_edit(orig, cor, edit, min=True, old_cat=False)`
 
-Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form: `[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True to preserve the old error type category (i.e. turn off the classifier).
+Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form:
+`[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end
+offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type
+of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True
+to preserve the old error type category (i.e. turn off the classifier).
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 orig = annotator.parse('This are gramamtical sentence .')
 cor = annotator.parse('This is a grammatical sentence .')
```

### Comparing `vnerrant-1.0.0/README.md` & `vnerrant-1.0.1rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # VNERRANT v1.0.0
 
 ## Overview
 
-The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information. Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the former to the latter and classify them according to a rule-based error type framework. This can be used to standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in M2 format and an evaluation script is provided.
+The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information.
+Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the
+former to the latter and classify them according to a rule-based error type framework. This can be used to
+standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in
+M2 format and an evaluation script is provided.
 
 ### Example
 
 **Original**: This are gramamtical sentence .
 **Corrected**: This is a grammatical sentence .
 **Output M2**:
 
@@ -32,18 +36,18 @@
 - Option 1: Install VNERRANT using pip with the following commands:
 
 ```bash
 pip install -U pip setuptools wheel
 pip install vnerrant
 ```
 
-- Option 2: Alternatively, if you want to install ERRANT from the source, you can follow these steps:
+- Option 2: Alternatively, if you want to install VNERRANT from the source, you can follow these steps:
 
 ```bash
-git clone https://gitlab.testsprep.online/nlp/research/errant
+git clone https://gitlab.testsprep.online/nlp/research/vnerrant
 cd vnerrant
 pip install -U pip setuptools wheel
 pip install -e .
 ```
 
 Please obtain a Spacy model by using the following command:
 
@@ -89,51 +93,57 @@
 vnerrant evaluate m2 -hyp <hyp_m2> -ref <ref_m2> -ds -cat {1,2,3}
 ```
 
 All these scripts also have additional advanced command line options which can be displayed using the `-h` flag.
 
 ### API
 
-As of v3.0.0, ERRANT now also comes with an API.
+As of v3.0.0, VNERRANT now also comes with an API.
 
 ### Quick Start
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 
 orig = 'My    name    is   the     John'
 cor = 'My name is John'
-edits = annotator.annotate_with_pre_and_post_processing(orig, cor)
+edits = annotator.annotate_raw(orig, cor)
 
 for e in edits:
-    print(e.o_start, e.o_end, e.o_str, e.c_start, e.c_end, e.c_str, e.type)
-    print(e.o_toks.start_char, e.o_toks.end_char)
-    # assert e.o_str == orig[e.o_toks.start_char:e.o_toks.end_char]
+    print(e.original.start_token, e.original.end_token, e.original.text)
+    print(e.corrected.start_token, e.corrected.end_token, e.corrected.text)
+    print(e.original.start_char, e.original.end_char, e.edit_type)
 ```
 
 ### Loading
 
 `vnerrant.load(lang, model_name)`
 
-Instantiate an ERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent ERRANT from loading it redundantly.
+Instantiate an VNERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent VNERRANT from loading it redundantly.
 
 ### Annotator Objects
 
-An Annotator object is the main interface for ERRANT.
+An Annotator object is the main interface for VNERRANT.
 
 #### Methods
 
 <details>
 <summary>annotator.parse</summary>
 
-`annotator.parse(string, tokenise=False)`
+`annotator.parse(string, tokenize_type='string')`
 
-Lemmatise, POS tag, and parse a text string with spacy. Set `tokenise` to True to also word tokenise with spacy. Returns a spacy Doc object.
+Lemmatise, POS tag, and parse a text string with spacy. Returns a spacy Doc object.
+
+`tokenize_type` must be in `["spacy", "split", "string"]`
+
+- `spacy`: tokenizing by default spacy tokenizer.
+- `split`: tokenizing by split function.
+- `string`: tokenizing by spacy and string tokenizer.
 
 </details>
 
 <details>
 <summary>annotator.align</summary>
 
 `annotator.align(orig, cor, lev=False)`
@@ -167,36 +177,63 @@
 </details>
 
 <details>
 <summary>annotator.annotate</summary>
 
 `annotator.annotate(orig, cor, lev=False, merging='rules')`
 
-Run the full annotation pipeline to align two sequences and extract and classify the edits. Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence. Returns a list of Edit objects.
+Run the full annotation pipeline to align two sequences and extract and classify the edits.
+Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
 
 ```python
-import errant
+import vnerrant
 
-annotator = errant.load(lang="en", model_name="en_core_web_sm")
-orig = annotator.parse('This are gramamtical sentence .')
-cor = annotator.parse('This is a grammatical sentence .')
-alignment = annotator.align(orig, cor)
-edits = annotator.merge(alignment)
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = annotator.parse("My   name   is    the    John")
+cor = annotator.parse("My name is John")
+edits = annotator.annotate(orig, cor)
+for e in edits:
+    print(e)
+```
+
+</details>
+
+<details>
+<summary>annotator.annotate_raw</summary>
+
+`annotator.annotate_raw(orig: str, cor: str, lev=False, merging='rules', tokenize_type='string')`
+
+Run the full annotation pipeline to align two strings, extract and classify the edits.
+Equivalent to running `annotator.parse`, `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
+
+```python
+import vnerrant
+
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = "My   name   is    the    John"
+cor = "My name is John"
+edits = annotator.annotate_raw(orig, cor)
 for e in edits:
-    e = annotator.classify(e)
+    print(e)
 ```
 
 </details>
 
 <details>
 <summary>annotator.import_edit</summary>
 
 `annotator.import_edit(orig, cor, edit, min=True, old_cat=False)`
 
-Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form: `[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True to preserve the old error type category (i.e. turn off the classifier).
+Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form:
+`[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end
+offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type
+of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True
+to preserve the old error type category (i.e. turn off the classifier).
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 orig = annotator.parse('This are gramamtical sentence .')
 cor = annotator.parse('This is a grammatical sentence .')
```

### Comparing `vnerrant-1.0.0/setup.py` & `vnerrant-1.0.1rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
+
 # Get base working directory.
 base_dir = Path(__file__).resolve().parent
 
 # Readme text for long description
 with open(base_dir / "README.md") as f:
     readme = f.read()
 
 setup(
     name="vnerrant",
-    version="v1.0.0",
+    version="1.0.1rc1",
     license="MIT",
     description="The ERRor ANnotation Toolkit (ERRANT). \
         Automatically extract and classify edits in parallel sentences.",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=[
         "automatic annotation",
```

### Comparing `vnerrant-1.0.0/vnerrant/__init__.py` & `vnerrant-1.0.1rc1/vnerrant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import spacy
 
 from vnerrant.annotator import Annotator
 from vnerrant.utils.utils import get_spacy_models_for_language
 
-__version__ = "v1.0.0"
+__version__ = "v1.0.1rc1"
 
 
 def load(
     lang: str = "en",
     model_name: str = "en_core_web_sm",
     nlp: Any = None,
 ) -> Annotator:
```

### Comparing `vnerrant-1.0.0/vnerrant/annotator.py` & `vnerrant-1.0.1rc1/vnerrant/annotator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 from __future__ import annotations
 
 import importlib
 from pathlib import Path
-from typing import Any
+from typing import Any, List
 
-from spacy.tokens import Doc
+from spacy.tokens import Doc, Token
 
 from vnerrant.components.alignment import Alignment
 from vnerrant.components.classifier import BaseClassifer
+from vnerrant.components.explainer import BaseExplainer
 from vnerrant.components.merger import BaseMerger
-from vnerrant.constants import (
-    MAPPING_TYPE_ERROR,
-    MERGING_ALL_EQUAL,
-    MERGING_ALL_MERGE,
-    MERGING_ALL_SPLIT,
-    MERGING_RULES,
-    Operator,
-    SeparatorTypes,
-)
-from vnerrant.model.edit import Edit
+from vnerrant.constants import MERGING_ALL_EQUAL, MERGING_ALL_MERGE, MERGING_ALL_SPLIT, MERGING_RULES, TokenizeTypes
+from vnerrant.model.edit import Edit, EditCollection
+from vnerrant.utils import edit_utils
+from vnerrant.utils.string_utils import StringTokenizer
+
+Token.set_extension("full_text", default=None, force=True)
+
+
+def update_doc(doc: Doc, tokens: List[str]):
+    """
+    Update the full_text attribute of the tokens in a spacy Doc object.
+    Args:
+        doc (Doc): A spacy Doc object
+        tokens (list[str]): A list of token texts with whitespace
+    """
+    assert len(doc) == len(tokens)
+    for token, text in zip(doc, tokens):
+        token._.full_text = text
 
 
 class Annotator:
     """
     Annotator class for automatic annotation of parallel text with ERRANT edits.
     """
 
     def __init__(
         self,
         lang: str,
         nlp: Any = None,
         merger: BaseMerger = None,
         classifier: BaseClassifer = None,
+        explainer: BaseExplainer = None,
     ):
         """
         Initialise the annotator with a language id, spacy processing object,
         merging module, and classifier module.
         :param lang: A string language id: e.g. "en"
         :param nlp: A spacy processing object for the language
         :param merger: A merging module for the language
         :param classifier: A classifier module for the language
         """
         self.lang = lang
         self.nlp = nlp
 
-        self.merger = (
-            self._import_module(merger, "merger") if merger is None else merger
-        )
-        self.classifier = (
-            self._import_module(classifier, "classifier")
-            if classifier is None
-            else classifier
-        )
+        self.merger = self._import_module(merger, "merger") if merger is None else merger
+        self.classifier = self._import_module(classifier, "classifier") if classifier is None else classifier
+        self.explainer = self._import_module(explainer, "explainer") if explainer is None else explainer
 
     def _import_module(self, module, module_type):
         """
-        Import a module from the components directory.
+        Import a module from the components' directory.
         :param module: A module object
         :param module_type: A string module type
         :return: A module object
         """
         base_path = Path(__file__).resolve().parent
         module_name = f"vnerrant.components.{self.lang}.{module_type}"
         module_path = base_path / "components" / self.lang / f"{module_type}.py"
@@ -68,54 +73,46 @@
             Module = importlib.import_module(module_name).__getattribute__(
                 module_type.capitalize(),
             )
             return Module()
         else:
             raise ValueError(f"No {module_type} available for language: {self.lang}")
 
-    @staticmethod
-    def normalised_text(text: str, **kwargs) -> str:
-        """
-        Normalise a text string.
-        :param text: A text string
-        :return: A normalised text string
-        """
-        if kwargs.get("lowercase"):
-            text = text.lower()
-
-        # Remove new lines and tabs
-        text = text.replace("\n", " ")
-        text = text.replace("\t", " ")
-
-        return text
-
-    def preprocess_by_rule(self, text: str, **kwargs) -> Doc | str:
-        text = self.normalised_text(text, **kwargs)
-
-        doc = self.nlp(text)
-        tokens = [token.text for token in doc if not token.is_space]
-        return doc, " ".join(tokens)
-
-    def parse(self, text: str, tokenise: bool = False) -> Doc:
+    def parse(self, text: str, tokenize_type: str = TokenizeTypes.SPLIT) -> Doc:
         """
         Parse a text string with spacy.
         :param text: A text string
-        :param tokenise: A flag to tokenise the text string
+        :param tokenize_type: A flag to tokenize the text string
         :return: A spacy Doc object
         """
-        if tokenise:
+        if tokenize_type == TokenizeTypes.SPACY:
             text = self.nlp(text)
-        else:
+        elif tokenize_type == TokenizeTypes.SPLIT:
             text = Doc(self.nlp.vocab, text.split())
-            # self.nlp.tagger(text)
-            # self.nlp.parser(text)
             text = self.nlp(text)
+        elif tokenize_type == TokenizeTypes.STRING:
+            doc = self.nlp(text)
+            tokens = [token.text_with_ws for token in doc]
+            words = []
+            for token in tokens:
+                tokenizer = StringTokenizer(token, return_delimiter=True)
+                sub_tokens = []
+                while tokenizer.has_more_tokens():
+                    sub_tokens.append(tokenizer.next_token())
+                words.extend(sub_tokens)
+
+            spaces = [False] * len(words)
+            text = Doc(self.nlp.vocab, words=words, spaces=spaces)
+            text = self.nlp(text)
+        else:
+            raise ValueError(f"Tokenize Type {tokenize_type} is not supported")
+
         return text
 
-    def align(self, orig: str, cor: str, lev: bool = False) -> Alignment:
+    def align(self, orig: Doc, cor: Doc, lev: bool = False) -> Alignment:
         """
         Align an original and corrected text string.
         :param orig: An original text string
         :param cor: A corrected text string
         :param lev: A flag to use levenshtein alignment
         :return: An Alignment object
         """
@@ -155,27 +152,34 @@
                 alignment.orig,
                 alignment.cor,
                 alignment.align_seq,
             )
         # Unknown
         else:
             raise Exception(
-                "Unknown merging strategy. Choose from: "
-                "rules, all-split, all-merge, all-equal.",
+                "Unknown merging strategy. Choose from: rules, all-split, all-merge, all-equal.",
             )
         return edits
 
     def classify(self, edit: Edit) -> Edit:
         """
         Classify an edit with the classifier.
         :param edit: An Edit object
         :return: An Edit object
         """
         return self.classifier.classify(edit)
 
+    def explain(self, edit: Edit) -> Edit:
+        """
+        Explain an edit with the explainer.
+        :param edit: An Edit object
+        :return: An Edit object
+        """
+        return self.explainer.explain(edit)
+
     def annotate(
         self,
         orig: Doc,
         cor: Doc,
         lev: bool = False,
         merging: str = "rules",
     ) -> list[Edit]:
@@ -186,107 +190,114 @@
         :param lev: A flag to use levenshtein alignment
         :param merging: A string merging strategy
         :return: A list of Edit objects
         """
         alignment = self.align(orig, cor, lev)
         edits = self.merge(alignment, merging)
         for edit in edits:
-            edit = self.classify(edit)
+            self.classify(edit)
+            self.explain(edit)
         return edits
 
-    def annotate_with_pre_and_post_processing(
+    def annotate_raw(
         self,
         orig: str,
         cor: str,
         lev: bool = False,
         merging: str = "rules",
+        tokenize_type: str = TokenizeTypes.SPACY,
     ) -> list[Edit]:
         """
-        Annotate a pair of original and corrected text strings with pre-processing and post-processing.
-        :param orig: An original text string
-        :param cor: A corrected text string
+        Annotate a pair of original and corrected string objects.
+        :param orig: An original text
+        :param cor: A corrected text
         :param lev: A flag to use levenshtein alignment
         :param merging: A string merging strategy
+        :param tokenize_type: A string tokenize type strategy
         :return: A list of Edit objects
         """
-
-        doc_orig, normalized_orig = self.preprocess_by_rule(orig)
-        doc_corr, normalized_corr = self.preprocess_by_rule(cor)
-
-        processed_text = self.parse(normalized_orig)
-        corrected_text = self.parse(normalized_corr)
-        alignment = self.align(processed_text, corrected_text, lev)
+        # Normalise text and get list of token texts with whitespace
+        processed_orig, orig_tokens = self.preprocess(orig)
+        processed_cor, cor_tokens = self.preprocess(cor)
+
+        # Parse text
+        orig_doc = self.parse(processed_orig, tokenize_type=tokenize_type)
+        cor_doc = self.parse(processed_cor, tokenize_type=tokenize_type)
+
+        # Update the full_text attribute of the tokens in the spacy Doc object
+        update_doc(orig_doc, orig_tokens)
+        update_doc(cor_doc, cor_tokens)
+
+        # Get edits and match edits
+        alignment = self.align(orig_doc, cor_doc, lev)
+        match_edits = edit_utils.get_match_edits(alignment)
         edits = self.merge(alignment, merging)
+
+        # Classify and explain edits
         for edit in edits:
-            edit = self.classify(edit)
-            start_token = edit.o_start
-            end_token = edit.o_end
-
-            count_idx = 0
-            add_space = 0
-            for token in doc_orig:
-                if token.is_space:
-                    add_space += 1
-                    continue
-                else:
-                    if count_idx == start_token:
-                        break
-                    else:
-                        count_idx += 1
-
-            orig_tokens = doc_orig[start_token + add_space : end_token + add_space]
-            edit.o_toks.start_char = orig_tokens.start_char
-            edit.o_toks.end_char = orig_tokens.end_char
+            self.classify(edit)
+            self.explain(edit)
 
-        edits = self.postprocess_by_rule(orig, edits)
-        return edits
+        edit_collection = EditCollection(orig, cor, orig_doc, cor_doc, edits, match_edits)
+        self.postprocess(edit_collection)
 
-    def postprocess_by_rule(
-        self,
-        orig: str,
-        edits: list[Edit] | Edit,
-    ) -> list[Edit]:
+        return edit_collection.edits
+
+    def preprocess(self, text: str, **kwargs) -> tuple[str, list[str]]:
         """
-        Postprocess a list of edits.
-        :param orig: An original text string
-        :param edits: A list of Edit objects
-        :return: A list of Edit objects
+        Normalise a text string.
+        :param text: A text string
+        :return: A normalised text string and a list of token texts with whitespace
         """
+        doc = self.nlp(text)
+        token_with_ws_texts = [token.text_with_ws for token in doc]
 
-        if isinstance(edits, Edit):
-            edits = [edits]
+        # Merge space token to the previous token
+        merged_token_with_ws_texts = []
+        for index in range(len(doc)):
+            if index == 0:
+                merged_token_with_ws_texts.append(token_with_ws_texts[index])
+                continue
 
-        for edit in edits:
-            operator = edit.type[0]
-            type_error = edit.type[2:]
-            type_error = MAPPING_TYPE_ERROR[type_error]
-
-            edit.type = operator + SeparatorTypes.COLON + type_error
-
-            if operator == Operator.MISSING:
-                if edit.o_toks.start_char == 0:
-                    edit.o_toks.end_char = edit.o_toks.start_char
-                    edit.c_str = edit.c_str + " "
-                else:
-                    edit.o_toks.end_char = edit.o_toks.start_char - 1
-                if "PUNC" in type_error and edit.o_toks.start_char != len(orig):
-                    edit.o_toks.start_char = edit.o_toks.start_char - 1
-                elif "PUNC" in type_error and edit.o_toks.start_char == len(
-                    orig,
-                ):
-                    edit.o_toks.end_char = edit.o_toks.start_char
-            elif operator == Operator.UNNECESSARY:
-                if "PUNC" not in type_error:
-                    edit.o_toks.end_char = edit.o_toks.end_char + 1
-        return edits
+            if doc[index].is_space:
+                merged_token_with_ws_texts[-1] += token_with_ws_texts[index]
+            else:
+                merged_token_with_ws_texts.append(token_with_ws_texts[index])
+
+        assert "".join(merged_token_with_ws_texts) == text, "Error in normalised text processing"
+
+        processed_text = " ".join([token for token in text.split() if token.strip()])
+        if not merged_token_with_ws_texts[0].strip():
+            processed_text = merged_token_with_ws_texts[0] + processed_text
+
+        return processed_text, merged_token_with_ws_texts
+
+    def postprocess(self, edit_collection: EditCollection):
+        """
+        Postprocess the edit collection.
+        :param edit_collection: An EditCollection object
+        :return: None
+        """
+        edit_utils.update_edits(edit_collection.orig_doc, edit_collection.cor_doc, edit_collection.edits)
+        edit_utils.update_edits(edit_collection.orig_doc, edit_collection.cor_doc, edit_collection.match_edits)
+
+        space_edits = []
+        for edit in edit_collection.match_edits:
+            if edit.original.text == edit.corrected.text:
+                continue
+
+            space_edits.append(edit_utils.process_space_edit(edit))
+
+        edit_utils.merge_edit_collection_with_space_edits(edit_collection, space_edits)
+        edit_utils.update_operator(edit_collection.edits)
 
     def import_edit(
         self,
-        orig: str,
-        cor: str,
+        orig: Doc,
+        cor: Doc,
         edit: list,
         min: bool = True,
         old_cat: bool = False,
     ) -> Edit:
         """
         Import an edit from an external source.
         :param orig: An original text string
@@ -294,18 +305,18 @@
         :param edit: An edit list of the form: [o_start, o_end, c_start, c_end]
         :param min: A flag to minimise the edit
         :param old_cat: A flag to use the old error type classification
         :return: An Edit object
         """
         # Undefined error type
         if len(edit) == 4:
-            edit_obj = Edit(orig, cor, edit)
+            edit_obj = Edit.from_original_and_correction(orig, cor, edit)
         # Existing error type
         elif len(edit) == 5:
-            edit_obj = Edit(orig, cor, edit[:4], edit[4])
+            edit_obj = Edit.from_original_and_correction(orig, cor, edit[:4], edit[4])
         # Unknown edit format
         else:
             raise Exception(
                 "Edit not of the form: " "[o_start, o_end, c_start, c_end, (cat)]",
             )
         # Minimise edit
         if min:
```

### Comparing `vnerrant-1.0.0/vnerrant/cli/convert.py` & `vnerrant-1.0.1rc1/vnerrant/cli/convert.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/cli/evaluate.py` & `vnerrant-1.0.1rc1/vnerrant/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/alignment.py` & `vnerrant-1.0.1rc1/vnerrant/components/alignment.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/converter.py` & `vnerrant-1.0.1rc1/vnerrant/components/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import re
 
 from vnerrant.annotator import Annotator
+from vnerrant.constants import TokenizeTypes
 from vnerrant.model.edit import noop_edit
 
 
 class Converter:
     """
     Convert between M2 and parallel formats. This is a wrapper for the
     M2Processor class.
@@ -133,24 +134,25 @@
          ['S This is another test .'
           'A 2 3|||R:DET|||a|||REQUIRED|||-NONE-|||0'
           'A 4 4|||M:ADV|||too|||REQUIRED|||-NONE-|||0']
         ]
         """
         assert len(origs) == len(corrs)
         assert merge in ["rules", "all-split", "all-merge"]
+        tokenize_type = TokenizeTypes.SPACY if tokenise else TokenizeTypes.SPLIT
         out_m2 = []
 
         for orig, corr in zip(origs, corrs):
             m2 = []
             # Skip empty lines
             orig = orig.strip()
             corr = corr.strip()
             # Parse orig and corr with spacy
-            orig = self.annotator.parse(orig, tokenise)
-            corr = self.annotator.parse(corr, tokenise)
+            orig = self.annotator.parse(orig, tokenize_type)
+            corr = self.annotator.parse(corr, tokenize_type)
             # Write orig to the output m2 file
             m2.append(" ".join(["S"] + [token.text for token in orig]))
             # Align the texts and extract and classify the edits
             if orig.text.strip() == corr.text.strip():
                 m2.append(noop_edit(0))  # 0 is the id of the annotator
             else:
                 edits = self.annotator.annotate(orig, corr, lev, merge)
```

### Comparing `vnerrant-1.0.0/vnerrant/components/en/classifier.py` & `vnerrant-1.0.1rc1/vnerrant/components/en/classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 import spacy.symbols as POS
 from rapidfuzz.distance import Levenshtein
 from spacy.tokens import Token
 
 from vnerrant.components.classifier import BaseClassifer
-from vnerrant.components.en.constants import (
-    ChildrenErrorType,
-    ParentErrorType,
-    dependency_resources,
-    language_resources,
-    pos_resources,
-)
-from vnerrant.constants import Operator, SeparatorTypes
+from vnerrant.components.en.constants import ChildrenErrorType
+from vnerrant.components.en.constants import dependency_resources
+from vnerrant.components.en.constants import language_resources
+from vnerrant.components.en.constants import ParentErrorType
+from vnerrant.components.en.constants import pos_resources
+from vnerrant.constants import Operator
+from vnerrant.constants import SeparatorTypes
 from vnerrant.model.edit import Edit
 
 
 class Classifier(BaseClassifer):
     """
     Classifier class for English
     """
@@ -28,16 +27,16 @@
     def only_orth_change(o_toks: list[Token], c_toks: list[Token]) -> bool:
         """
         Check if the difference between two lists of tokens is only whitespace or case.
         :param o_toks: A list of spacy tokens.
         :param c_toks: A list of spacy tokens.
         :return: Boolean.
         """
-        o_join = "".join([o.lower_ for o in o_toks])
-        c_join = "".join([c.lower_ for c in c_toks])
+        o_join = ''.join([o.lower_ for o in o_toks])
+        c_join = ''.join([c.lower_ for c in c_toks])
         if o_join == c_join:
             return True
         return False
 
     @staticmethod
     def exact_reordering(o_toks: list[Token], c_toks: list[Token]) -> bool:
         """
@@ -58,44 +57,44 @@
         """
         Check if two tokens are preceded by an auxiliary verb.
         :param o_toks: A list of spacy tokens.
         :param c_toks: A list of spacy tokens.
         :return: Boolean.
         """
         # If the toks are aux, we need to check if they are the first aux.
-        if o_toks[0].dep_.startswith("aux") and c_toks[0].dep_.startswith("aux"):
+        if o_toks[0].dep_.startswith('aux') and c_toks[0].dep_.startswith('aux'):
             # Find the parent verb
             o_head = o_toks[0].head
             c_head = c_toks[0].head
             # Find the children of the parent
             o_children = o_head.children
             c_children = c_head.children
             # Check the orig children.
             for o_child in o_children:
                 # Look at the first aux...
-                if o_child.dep_.startswith("aux"):
+                if o_child.dep_.startswith('aux'):
                     # Check if the string matches o_tok
                     if o_child.text != o_toks[0].text:
                         # If it doesn't, o_tok is not first so check cor
                         for c_child in c_children:
                             # Find the first aux in cor...
-                            if c_child.dep_.startswith("aux"):
+                            if c_child.dep_.startswith('aux'):
                                 # If that doesn't match either, neither are first aux
                                 if c_child.text != c_toks[0].text:
                                     return True
                                 # Break after the first cor aux
                                 break
                     # Break after the first orig aux.
                     break
         # Otherwise, the toks are main verbs so we need to look for any aux.
         else:
             o_deps = [o_dep.dep_ for o_dep in o_toks[0].children]
             c_deps = [c_dep.dep_ for c_dep in c_toks[0].children]
-            if "aux" in o_deps or "auxpass" in o_deps:
-                if "aux" in c_deps or "auxpass" in c_deps:
+            if 'aux' in o_deps or 'auxpass' in o_deps:
+                if 'aux' in c_deps or 'auxpass' in c_deps:
                     return True
         return False
 
     @staticmethod
     def get_pos_and_dep(toks: list[Token]) -> tuple[list[str], list[str]]:
         """
         Extract POS and dependency parse info from a list of spacy tokens.
@@ -141,51 +140,51 @@
         Classify an edit with only one side of tokens.
         :param toks: A list of spacy tokens.
         :return: An error type string.
         """
         # Special cases
         if len(toks) == 1:
             # Possessive noun suffixes; e.g. ' -> 's
-            if toks[0].tag_ == "POS":
+            if toks[0].tag_ == 'POS':
                 return (
                     ParentErrorType.NOUN
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.POSSESSIVE
                 )
             # Contractions. Rule must come after possessive
             if toks[0].lower_ in dependency_resources.conts:
                 return ParentErrorType.CONTRACTION
             # Infinitival "to" is treated as part of a verb form
             if (
-                toks[0].lower_ == "to"
+                toks[0].lower_ == 'to'
                 and toks[0].pos == POS.PART
-                and toks[0].dep_ != "prep"
+                and toks[0].dep_ != 'prep'
             ):
                 return (
                     ParentErrorType.VERB + SeparatorTypes.COLON + ChildrenErrorType.FORM
                 )
         # Extract pos tags and parse info from the toks
         pos_list, dep_list = self.get_pos_and_dep(toks)
         # Auxiliary verbs
-        if set(dep_list).issubset({"aux", "auxpass"}):
+        if set(dep_list).issubset({'aux', 'auxpass'}):
             return ParentErrorType.VERB + SeparatorTypes.COLON + ChildrenErrorType.TENSE
         # POS-based tags. Ignores rare, uninformative categories
         if len(set(pos_list)) == 1 and pos_list[0] not in pos_resources.rare_pos:
             return pos_list[0]  # TODO: check if this is correct
         # More POS-based tags using special dependency labels
         if (
             len(set(dep_list)) == 1
             and dep_list[0] in dependency_resources.dep_map.keys()
         ):
             return dependency_resources.dep_map[dep_list[0]]
         # To-infinitives and phrasal verbs
-        if set(pos_list) == {"PART", "VERB"}:
+        if set(pos_list) == {'PART', 'VERB'}:
             return ParentErrorType.VERB
         # Tricky cases
-        else:
+        else: # TODO: Get more specific error type
             return ParentErrorType.OTHER
 
     def _get_two_sided_type(self, o_toks: list[Token], c_toks: list[Token]) -> str:
         """
         Classify an edit with two sides of tokens.
         :param o_toks: A list of spacy tokens.
         :param c_toks: A list of spacy tokens.
@@ -202,15 +201,15 @@
         if self.is_exact_reordering(o_toks, c_toks):
             return ParentErrorType.WORD_ORDER
 
         # 1:1 replacements (very common)
         if len(o_toks) == len(c_toks) == 1:
             # 1. SPECIAL CASES
             # Possessive noun suffixes; e.g. ' -> 's
-            if o_toks[0].tag_ == "POS" or c_toks[0].tag_ == "POS":
+            if o_toks[0].tag_ == 'POS' or c_toks[0].tag_ == 'POS':
                 return (
                     ParentErrorType.NOUN
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.POSSESSIVE
                 )
             # Contraction. Rule must come after possessive.
             if (
@@ -235,15 +234,15 @@
             ):
                 return (
                     ParentErrorType.VERB
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.TENSE
                 )
             # Special: "was" and "were" are the only past tense SVA
-            if {o_toks[0].lower_, c_toks[0].lower_} == {"was", "were"}:
+            if {o_toks[0].lower_, c_toks[0].lower_} == {'was', 'were'}:
                 return (
                     ParentErrorType.VERB
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.SUBJECT_VERB_AGREEMENT
                 )
 
             # 2. SPELLING AND INFLECTION
@@ -255,15 +254,15 @@
                 if (
                     o_toks[0].text not in language_resources.spell
                     and o_toks[0].lower_ not in language_resources.spell
                 ):
                     # Check if both sides have a common lemma
                     if o_toks[0].lemma == c_toks[0].lemma:
                         # Inflection; often count vs mass nouns or e.g. got vs getted
-                        if o_pos == c_pos and o_pos[0] in {"NOUN", "VERB"}:
+                        if o_pos == c_pos and o_pos[0] in {'NOUN', 'VERB'}:
                             return (
                                 o_pos[0]
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.INFLECTION
                             )
                         # Unknown morphology; i.e. we cannot be more specific.
                         else:
@@ -299,98 +298,98 @@
                 o_toks[0].lemma == c_toks[0].lemma
                 and o_pos[0] in pos_resources.open_pos2
                 and c_pos[0] in pos_resources.open_pos2
             ):
                 # Same POS on both sides
                 if o_pos == c_pos:
                     # Adjective form; e.g. comparatives
-                    if o_pos[0] == "ADJ":
+                    if o_pos[0] == 'ADJ':
                         return (
                             ParentErrorType.ADJECTIVE
                             + SeparatorTypes.COLON
                             + ChildrenErrorType.FORM
                         )
                     # Noun number
-                    if o_pos[0] == "NOUN":
+                    if o_pos[0] == 'NOUN':
                         return (
                             ParentErrorType.NOUN
                             + SeparatorTypes.COLON
                             + ChildrenErrorType.NUMBER
                         )
                     # Verbs - various types
-                    if o_pos[0] == "VERB":
+                    if o_pos[0] == 'VERB':
                         # NOTE: These rules are carefully ordered.
                         # Use the dep parse to find some form errors.
                         # Main verbs preceded by aux cannot be tense or SVA.
                         if self.is_preceded_by_aux(o_toks, c_toks):
                             return (
                                 ParentErrorType.VERB
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.FORM
                             )
                         # Use fine PTB tags to find various errors.
                         # FORM errors normally involve VBG or VBN.
-                        if o_toks[0].tag_ in {"VBG", "VBN"} or c_toks[0].tag_ in {
-                            "VBG",
-                            "VBN",
+                        if o_toks[0].tag_ in {'VBG', 'VBN'} or c_toks[0].tag_ in {
+                            'VBG',
+                            'VBN',
                         }:
                             return (
                                 ParentErrorType.VERB
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.FORM
                             )
                         # Of what's left, TENSE errors normally involved VBD.
-                        if o_toks[0].tag_ == "VBD" or c_toks[0].tag_ == "VBD":
+                        if o_toks[0].tag_ == 'VBD' or c_toks[0].tag_ == 'VBD':
                             return (
                                 ParentErrorType.VERB
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.TENSE
                             )
                         # Of what's left, SVA errors normally involve VBZ.
-                        if o_toks[0].tag_ == "VBZ" or c_toks[0].tag_ == "VBZ":
+                        if o_toks[0].tag_ == 'VBZ' or c_toks[0].tag_ == 'VBZ':
                             return (
                                 ParentErrorType.VERB
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.SUBJECT_VERB_AGREEMENT
                             )
                         # Any remaining aux verbs are called TENSE.
-                        if o_dep[0].startswith("aux") and c_dep[0].startswith("aux"):
+                        if o_dep[0].startswith('aux') and c_dep[0].startswith('aux'):
                             return (
                                 ParentErrorType.VERB
                                 + SeparatorTypes.COLON
                                 + ChildrenErrorType.TENSE
                             )
                 # Use dep labels to find some more ADJ:FORM
-                if set(o_dep + c_dep).issubset({"acomp", "amod"}):
+                if set(o_dep + c_dep).issubset({'acomp', 'amod'}):
                     return (
                         ParentErrorType.ADJECTIVE
                         + SeparatorTypes.COLON
                         + ChildrenErrorType.FORM
                     )
                 # Adj to plural noun is usually noun number; e.g. musical -> musicals.
-                if o_pos[0] == "ADJ" and c_toks[0].tag_ == "NNS":
+                if o_pos[0] == 'ADJ' and c_toks[0].tag_ == 'NNS':
                     return (
                         ParentErrorType.NOUN
                         + SeparatorTypes.COLON
                         + ChildrenErrorType.NUMBER
                     )
                 # For remaining verb errors (rare), rely on c_pos
-                if c_toks[0].tag_ in {"VBG", "VBN"}:
+                if c_toks[0].tag_ in {'VBG', 'VBN'}:
                     return (
                         ParentErrorType.VERB
                         + SeparatorTypes.COLON
                         + ChildrenErrorType.FORM
                     )
-                if c_toks[0].tag_ == "VBD":
+                if c_toks[0].tag_ == 'VBD':
                     return (
                         ParentErrorType.VERB
                         + SeparatorTypes.COLON
                         + ChildrenErrorType.TENSE
                     )
-                if c_toks[0].tag_ == "VBZ":
+                if c_toks[0].tag_ == 'VBZ':
                     return (
                         ParentErrorType.VERB
                         + SeparatorTypes.COLON
                         + ChildrenErrorType.SUBJECT_VERB_AGREEMENT
                     )
                 # Tricky cases that all have the same lemma.
                 else:
@@ -402,51 +401,51 @@
                 and o_pos[0] in pos_resources.open_pos2
                 and c_pos[0] in pos_resources.open_pos2
             ):
                 return ParentErrorType.MORPHOLOGY
 
             # 4. GENERAL
             # Auxiliaries with different lemmas
-            if o_dep[0].startswith("aux") and c_dep[0].startswith("aux"):
+            if o_dep[0].startswith('aux') and c_dep[0].startswith('aux'):
                 return (
                     ParentErrorType.VERB
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.TENSE
                 )
             # POS-based tags. Some of these are context sensitive mispellings.
             if o_pos == c_pos and o_pos[0] not in pos_resources.rare_pos:
                 return o_pos[0]
             # Some dep labels map to POS-based tags.
             if o_dep == c_dep and o_dep[0] in dependency_resources.dep_map.keys():
                 return dependency_resources.dep_map[o_dep[0]]
             # Phrasal verb particles.
-            if set(o_pos + c_pos) == {"PART", "PREP"} or set(o_dep + c_dep) == {
-                "prt",
-                "prep",
+            if set(o_pos + c_pos) == {'PART', 'PREP'} or set(o_dep + c_dep) == {
+                'prt',
+                'prep',
             }:
                 return ParentErrorType.PARTICLE
             # Can use dep labels to resolve DET + PRON combinations.
-            if set(o_pos + c_pos) == {"DET", "PRON"}:
+            if set(o_pos + c_pos) == {'DET', 'PRON'}:
                 # DET cannot be a subject or object.
-                if c_dep[0] in {"nsubj", "nsubjpass", "dobj", "pobj"}:
+                if c_dep[0] in {'nsubj', 'nsubjpass', 'dobj', 'pobj'}:
                     return ParentErrorType.PRONOUN
                 # "poss" indicates possessive determiner
-                if c_dep[0] == "poss":
+                if c_dep[0] == 'poss':
                     return ParentErrorType.DETERMINER
             # NUM and DET are usually DET; e.g. a <-> one
-            if set(o_pos + c_pos) == {"NUM", "DET"}:
+            if set(o_pos + c_pos) == {'NUM', 'DET'}:
                 return ParentErrorType.DETERMINER
             # Special: other <-> another
-            if {o_toks[0].lower_, c_toks[0].lower_} == {"other", "another"}:
+            if {o_toks[0].lower_, c_toks[0].lower_} == {'other', 'another'}:
                 return ParentErrorType.DETERMINER
             # Special: your (sincerely) -> yours (sincerely)
-            if o_toks[0].lower_ == "your" and c_toks[0].lower_ == "yours":
+            if o_toks[0].lower_ == 'your' and c_toks[0].lower_ == 'yours':
                 return ParentErrorType.PRONOUN
             # Special: no <-> not; this is very context sensitive
-            if {o_toks[0].lower_, c_toks[0].lower_} == {"no", "not"}:
+            if {o_toks[0].lower_, c_toks[0].lower_} == {'no', 'not'}:
                 return ParentErrorType.OTHER
 
             # 5. STRING SIMILARITY
             # These rules are quite language specific.
             if o_toks[0].text.isalpha() and c_toks[0].text.isalpha():
                 # Normalised Lev distance works better than Lev ratio
                 str_sim = Levenshtein.normalized_similarity(
@@ -462,31 +461,31 @@
                         return ParentErrorType.SPELLING
                 if len(o_toks[0].text) == 2:
                     # in -> is, he -> the, to -> too
                     if 2 <= len(c_toks[0].text) <= 3 and str_sim >= 0.5:
                         return ParentErrorType.SPELLING
                 if len(o_toks[0].text) == 3:
                     # Special: the -> that (relative pronoun)
-                    if o_toks[0].lower_ == "the" and c_toks[0].lower_ == "that":
+                    if o_toks[0].lower_ == 'the' and c_toks[0].lower_ == 'that':
                         return ParentErrorType.PRONOUN
                     # Special: all -> everything
-                    if o_toks[0].lower_ == "all" and c_toks[0].lower_ == "everything":
+                    if o_toks[0].lower_ == 'all' and c_toks[0].lower_ == 'everything':
                         return ParentErrorType.PRONOUN
                     # off -> of, too -> to, out -> our, now -> know
                     if 2 <= len(c_toks[0].text) <= 4 and str_sim >= 0.5:
                         return ParentErrorType.SPELLING
                 # B. Longer sequences are also likely to include content word errors
                 if len(o_toks[0].text) == 4:
                     # Special: that <-> what
-                    if {o_toks[0].lower_, c_toks[0].lower_} == {"that", "what"}:
+                    if {o_toks[0].lower_, c_toks[0].lower_} == {'that', 'what'}:
                         return ParentErrorType.PRONOUN
                     # Special: well <-> good
                     if {o_toks[0].lower_, c_toks[0].lower_} == {
-                        "good",
-                        "well",
+                        'good',
+                        'well',
                     } and c_pos[0] not in pos_resources.rare_pos:
                         return c_pos[0]
                     # knew -> new,
                     if len(c_toks[0].text) == 3 and str_sim > 0.5:
                         return ParentErrorType.SPELLING
                     # then <-> than, form -> from
                     if len(c_toks[0].text) == 4 and str_sim >= 0.5:
@@ -500,16 +499,16 @@
                         and str_sim > 0.5
                         and c_pos[0] not in pos_resources.rare_pos
                     ):
                         return c_pos[0]
                 if len(o_toks[0].text) == 5:
                     # Special: after -> later
                     if {o_toks[0].lower_, c_toks[0].lower_} == {
-                        "after",
-                        "later",
+                        'after',
+                        'later',
                     } and c_pos[0] not in pos_resources.rare_pos:
                         return c_pos[0]
                     # where -> were, found -> fund
                     if len(c_toks[0].text) == 4 and str_sim == 0.8:
                         return ParentErrorType.SPELLING
                     # thing <-> think, quite -> quiet, their <-> there
                     if len(c_toks[0].text) == 5 and str_sim >= 0.6:
@@ -520,20 +519,20 @@
                         and c_pos[0] not in pos_resources.rare_pos
                     ):
                         return c_pos[0]
                 # C. Longest sequences include MORPH errors
                 if len(o_toks[0].text) > 5 and len(c_toks[0].text) > 5:
                     # Special: therefor -> therefore
                     if (
-                        o_toks[0].lower_ == "therefor"
-                        and c_toks[0].lower_ == "therefore"
+                        o_toks[0].lower_ == 'therefor'
+                        and c_toks[0].lower_ == 'therefore'
                     ):
                         return ParentErrorType.SPELLING
                     # Special: though <-> thought
-                    if {o_toks[0].lower_, c_toks[0].lower_} == {"though", "thought"}:
+                    if {o_toks[0].lower_, c_toks[0].lower_} == {'though', 'thought'}:
                         return ParentErrorType.SPELLING
                     # Morphology errors: stress -> stressed, health -> healthy
                     if (
                         o_toks[0].text.startswith(c_toks[0].text)
                         or c_toks[0].text.startswith(o_toks[0].text)
                     ) and str_sim >= 0.66:
                         return ParentErrorType.MORPHOLOGY
@@ -546,20 +545,20 @@
                     # NOTE: Errors between 0.55 and 0.8 are a mix of SPELL, MORPH and POS
             # Tricky cases
             else:
                 return ParentErrorType.OTHER
 
         # Multi-token replacements (uncommon)
         # All auxiliaries
-        if set(o_dep + c_dep).issubset({"aux", "auxpass"}):
+        if set(o_dep + c_dep).issubset({'aux', 'auxpass'}):
             return ParentErrorType.VERB + SeparatorTypes.COLON + ChildrenErrorType.TENSE
         # All same POS
         if len(set(o_pos + c_pos)) == 1:
             # Final verbs with the same lemma are tense; e.g. eat -> has eaten
-            if o_pos[0] == "VERB" and o_toks[-1].lemma == c_toks[-1].lemma:
+            if o_pos[0] == 'VERB' and o_toks[-1].lemma == c_toks[-1].lemma:
                 return (
                     ParentErrorType.VERB
                     + SeparatorTypes.COLON
                     + ChildrenErrorType.TENSE
                 )
             # POS-based tags.
             elif o_pos[0] not in pos_resources.rare_pos:
@@ -567,37 +566,37 @@
         # All same special dep labels.
         if (
             len(set(o_dep + c_dep)) == 1
             and o_dep[0] in dependency_resources.dep_map.keys()
         ):
             return dependency_resources.dep_map[o_dep[0]]
         # Infinitives, gerunds, phrasal verbs.
-        if set(o_pos + c_pos) == {"PART", "VERB"}:
+        if set(o_pos + c_pos) == {'PART', 'VERB'}:
             # Final verbs with the same lemma are form; e.g. to eat -> eating
             if o_toks[-1].lemma == c_toks[-1].lemma:
                 return (
                     ParentErrorType.VERB + SeparatorTypes.COLON + ChildrenErrorType.FORM
                 )
             # Remaining edits are often verb; e.g. to eat -> consuming, look at -> see
             else:
                 return ParentErrorType.VERB
         # Possessive nouns; e.g. friends -> friend 's
-        if (o_pos == ["NOUN", "PART"] or c_pos == ["NOUN", "PART"]) and o_toks[
+        if (o_pos == ['NOUN', 'PART'] or c_pos == ['NOUN', 'PART']) and o_toks[
             0
         ].lemma == c_toks[0].lemma:
             return (
                 ParentErrorType.NOUN
                 + SeparatorTypes.COLON
                 + ChildrenErrorType.POSSESSIVE
             )
         # Adjective forms with "most" and "more"; e.g. more free -> freer
         if (
             (
-                o_toks[0].lower_ in {"most", "more"}
-                or c_toks[0].lower_ in {"most", "more"}
+                o_toks[0].lower_ in {'most', 'more'}
+                or c_toks[0].lower_ in {'most', 'more'}
             )
             and o_toks[-1].lemma == c_toks[-1].lemma
             and len(o_toks) <= 2
             and len(c_toks) <= 2
         ):
             return (
                 ParentErrorType.ADJECTIVE
@@ -607,57 +606,77 @@
 
         # Tricky cases.
         else:
             return ParentErrorType.OTHER
 
     def classify(self, edit: Edit) -> Edit:
         """
+        Classify an edit into a specific error type with preprocessing the delimiters in edit.
+        :param edit: An Edit object.
+        :return: The error type of the edit.
+        """
+        clone_edit = edit.copy()
+
+        if clone_edit.original.text.strip() or clone_edit.corrected.text.strip():
+            clone_edit.original.strip()
+            clone_edit.corrected.strip()
+
+        clone_edit = self._classify(clone_edit)
+
+        edit.edit_type = clone_edit.edit_type
+        return edit
+
+    def _classify(self, edit: Edit) -> Edit:
+        """
         Classify an edit into a specific error type.
         :param edit: An Edit object.
         :return: The error type of the edit.
         """
         # Nothing to nothing is a detected but not corrected edit
-        if not edit.o_toks and not edit.c_toks:
-            edit.type = ParentErrorType.UNK
+        if not edit.original.tokens and not edit.corrected.tokens:
+            edit.edit_type = ParentErrorType.UNK
         # Missing
-        elif not edit.o_toks and edit.c_toks:
+        elif not edit.original.tokens and edit.corrected.tokens:
             op = Operator.MISSING
-            cat = self._get_one_sided_type(edit.c_toks)
-            edit.type = op + SeparatorTypes.COLON + cat
+            cat = self._get_one_sided_type(edit.corrected.tokens)
+            edit.edit_type = op + SeparatorTypes.COLON + cat
         # Unnecessary
-        elif edit.o_toks and not edit.c_toks:
+        elif edit.original.tokens and not edit.corrected.tokens:
             op = Operator.UNNECESSARY
-            cat = self._get_one_sided_type(edit.o_toks)
-            edit.type = op + SeparatorTypes.COLON + cat
-            if edit.c_str != "":
+            cat = self._get_one_sided_type(edit.original.tokens)
+            edit.edit_type = op + SeparatorTypes.COLON + cat
+            if edit.corrected.text != '':
                 op = Operator.REPLACE
-                edit.type = op + SeparatorTypes.COLON + cat
+                edit.edit_type = op + SeparatorTypes.COLON + cat
         # Replacement and special cases
         else:
             # Same to same is a detected but not corrected edit
-            if edit.o_str == edit.c_str:
-                edit.type = ParentErrorType.UNK
+            if edit.original.text == edit.corrected.text:
+                # ' hello' -> 'hello ' # TODO: Dicussion needed for this case
+                # edit.edit_type = ParentErrorType.UNK
+                edit.edit_type = Operator.REPLACE + SeparatorTypes.COLON + ParentErrorType.OTHER
             # Special: Ignore case change at the end of multi token edits
             # E.g. [Doctor -> The doctor], [, since -> . Since]
             # Classify the edit as if the last token wasn't there
-            elif edit.o_toks[-1].lower == edit.c_toks[-1].lower and (
-                len(edit.o_toks) > 1 or len(edit.c_toks) > 1
+            elif edit.original.tokens[-1].lower == edit.corrected.tokens[-1].lower and (
+                len(edit.original.tokens) > 1 or len(edit.corrected.tokens) > 1
             ):
                 # Store a copy of the full orig and cor toks
-                all_o_toks = edit.o_toks[:]
-                all_c_toks = edit.c_toks[:]
+                all_o_toks = edit.original.tokens[:]
+                all_c_toks = edit.corrected.tokens[:]
                 # Truncate the instance toks for classification
-                edit.o_toks = edit.o_toks[:-1]
-                edit.c_toks = edit.c_toks[:-1]
+                edit.original.tokens = edit.original.tokens[:-1]
+                edit.corrected.tokens = edit.corrected.tokens[:-1]
                 # Classify the truncated edit
-                edit = self.classify(edit)
+                edit = self._classify(edit)
                 # Restore the full orig and cor toks
-                edit.o_toks = all_o_toks
-                edit.c_toks = all_c_toks
+                edit.original.tokens = all_o_toks
+                edit.corrected.tokens = all_c_toks
             # Replacement
             else:
                 op = Operator.REPLACE
-                cat = self._get_two_sided_type(edit.o_toks, edit.c_toks)
-                if cat == ParentErrorType.CONTRACTION and "'" in edit.o_str:
-                    edit.c_str = " " + edit.c_str
-                edit.type = op + SeparatorTypes.COLON + cat
+                cat = self._get_two_sided_type(
+                    edit.original.tokens, edit.corrected.tokens)
+                # if cat == ParentErrorType.CONTRACTION and "'" in edit.original.text:
+                #     edit.corrected.text = " " + edit.corrected.text
+                edit.edit_type = op + SeparatorTypes.COLON + cat
         return edit
```

### Comparing `vnerrant-1.0.0/vnerrant/components/en/constants.py` & `vnerrant-1.0.1rc1/vnerrant/components/en/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/en/lancaster.py` & `vnerrant-1.0.1rc1/vnerrant/components/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/en/merger.py` & `vnerrant-1.0.1rc1/vnerrant/components/en/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,26 @@
             group = list(group)
             # Ignore M
             if op == "M":
                 continue
             # T is always split
             elif op == "T":
                 for seq in group:
-                    edits.append(Edit(orig, corr, seq[1:]))
+                    edits.append(Edit.from_original_and_correction(orig, corr, seq[1:]))
             # Process D, I and S subsequence
             else:
                 processed = self.get_rule_merge_edits(
                     orig,
                     corr,
                     group_edits=group,
                     align_edits=align_edits,
                 )
                 # Turn the processed sequence into edits
                 for seq in processed:
-                    edits.append(Edit(orig, corr, seq[1:]))
+                    edits.append(Edit.from_original_and_correction(orig, corr, seq[1:]))
         return edits
 
     def get_rule_merge_edits(self, orig, corr, group_edits, align_edits):
         """
         Merge adjacent edits according to a set of rules.
         :param orig: The original spacy Doc.
         :param corr: The corrected spacy Doc.
```

### Comparing `vnerrant-1.0.0/vnerrant/components/en/resources/README.md` & `vnerrant-1.0.1rc1/vnerrant/components/en/resources/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/en/resources/en_GB-large.txt` & `vnerrant-1.0.1rc1/vnerrant/components/en/resources/en_GB-large.txt`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/en/utils.py` & `vnerrant-1.0.1rc1/vnerrant/components/en/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/evaluater.py` & `vnerrant-1.0.1rc1/vnerrant/components/evaluater.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/components/merger.py` & `vnerrant-1.0.1rc1/vnerrant/components/merger.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     def __init__(self):
         pass
 
     @staticmethod
     def merge_edits(edits: list[tuple]) -> list[tuple]:
         """
         Merge a list of edits into a single edit.
-        :param edit: A list of edits to merge.
+        :param edits: A list of edits to merge.
         :return: A single merged edit.
         """
         if not edits:
             return edits
         return [("X", edits[0][1], edits[-1][2], edits[0][3], edits[-1][4])]
 
     @abstractmethod
-    def get_all_rule_merge_edits(self):
+    def get_all_rule_merge_edits(self, *args, **kwargs):
         """
         Get all edits from the alignment sequence. Each edit is a span of
         tokens from the original and corrected sentences.
         """
         raise NotImplementedError
 
     def get_all_split_edits(
@@ -49,15 +49,15 @@
         :param align_edits: A list of edits from the alignment sequence.
         :return: A list of Edit objects.
         """
 
         edits = []
         for align in align_edits:
             if align[0] != "M":
-                edits.append(Edit(orig, corr, align[1:]))
+                edits.append(Edit.from_original_and_correction(orig, corr, align[1:]))
         return edits
 
     def get_all_merge_edits(
         self,
         orig: Doc,
         corr: Doc,
         align_edits: list[tuple],
@@ -72,15 +72,15 @@
         edits = []
         for op, group in itertools.groupby(
             align_edits,
             lambda x: True if x[0] != "M" else False,
         ):
             if op:
                 merged = self.merge_edits(list(group))
-                edits.append(Edit(orig, corr, merged[0][1:]))
+                edits.append(Edit.from_original_and_correction(orig, corr, merged[0][1:]))
         return edits
 
     def get_all_equal_edits(
         self,
         orig: Doc,
         corr: Doc,
         align_edits: list[tuple],
@@ -93,9 +93,9 @@
         :return: A list of Edit objects.
         """
 
         edits = []
         for op, group in itertools.groupby(align_edits, lambda x: x[0]):
             if op != "M":
                 merged = self.merge_edits(list(group))
-                edits.append(Edit(orig, corr, merged[0][1:]))
+                edits.append(Edit.from_original_and_correction(orig, corr, merged[0][1:]))
         return edits
```

### Comparing `vnerrant-1.0.0/vnerrant/components/tokenizer.py` & `vnerrant-1.0.1rc1/vnerrant/components/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/config/mapping_type_error.yaml` & `vnerrant-1.0.1rc1/vnerrant/config/mapping_type_error.yaml`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/metrics/criteria.py` & `vnerrant-1.0.1rc1/vnerrant/metrics/criteria.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/run_cli.py` & `vnerrant-1.0.1rc1/vnerrant/run_cli.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/utils/helper.py` & `vnerrant-1.0.1rc1/vnerrant/utils/helper.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/utils/pretty_results.py` & `vnerrant-1.0.1rc1/vnerrant/utils/pretty_results.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant/utils/utils.py` & `vnerrant-1.0.1rc1/vnerrant/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.0/vnerrant.egg-info/PKG-INFO` & `vnerrant-1.0.1rc1/vnerrant.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.0
+Version: 1.0.1rc1
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,19 @@
 Requires-Dist: spacy>=3
 Requires-Dist: rapidfuzz>=2.0.0
 
 # VNERRANT v1.0.0
 
 ## Overview
 
-The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information. Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the former to the latter and classify them according to a rule-based error type framework. This can be used to standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in M2 format and an evaluation script is provided.
+The main aim of VNERRANT is to automatically annotate parallel English sentences with error type information.
+Specifically, given an original and corrected sentence pair, VNERRANT will extract the edits that transform the
+former to the latter and classify them according to a rule-based error type framework. This can be used to
+standardise parallel datasets or facilitate detailed error type evaluation. Annotated output files are in
+M2 format and an evaluation script is provided.
 
 ### Example
 
 **Original**: This are gramamtical sentence .
 **Corrected**: This is a grammatical sentence .
 **Output M2**:
 
@@ -54,18 +58,18 @@
 - Option 1: Install VNERRANT using pip with the following commands:
 
 ```bash
 pip install -U pip setuptools wheel
 pip install vnerrant
 ```
 
-- Option 2: Alternatively, if you want to install ERRANT from the source, you can follow these steps:
+- Option 2: Alternatively, if you want to install VNERRANT from the source, you can follow these steps:
 
 ```bash
-git clone https://gitlab.testsprep.online/nlp/research/errant
+git clone https://gitlab.testsprep.online/nlp/research/vnerrant
 cd vnerrant
 pip install -U pip setuptools wheel
 pip install -e .
 ```
 
 Please obtain a Spacy model by using the following command:
 
@@ -111,51 +115,57 @@
 vnerrant evaluate m2 -hyp <hyp_m2> -ref <ref_m2> -ds -cat {1,2,3}
 ```
 
 All these scripts also have additional advanced command line options which can be displayed using the `-h` flag.
 
 ### API
 
-As of v3.0.0, ERRANT now also comes with an API.
+As of v3.0.0, VNERRANT now also comes with an API.
 
 ### Quick Start
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 
 orig = 'My    name    is   the     John'
 cor = 'My name is John'
-edits = annotator.annotate_with_pre_and_post_processing(orig, cor)
+edits = annotator.annotate_raw(orig, cor)
 
 for e in edits:
-    print(e.o_start, e.o_end, e.o_str, e.c_start, e.c_end, e.c_str, e.type)
-    print(e.o_toks.start_char, e.o_toks.end_char)
-    # assert e.o_str == orig[e.o_toks.start_char:e.o_toks.end_char]
+    print(e.original.start_token, e.original.end_token, e.original.text)
+    print(e.corrected.start_token, e.corrected.end_token, e.corrected.text)
+    print(e.original.start_char, e.original.end_char, e.edit_type)
 ```
 
 ### Loading
 
 `vnerrant.load(lang, model_name)`
 
-Instantiate an ERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent ERRANT from loading it redundantly.
+Instantiate an VNERRANT Annotator object. Presently, the lang parameter exclusively accepts 'en' for English, though we aspire to broaden its language support in future iterations. The model_name corresponds to the name of the SpaCy model being utilized. Optionally, you can provide the nlp parameter if you've previously loaded SpaCy and wish to prevent VNERRANT from loading it redundantly.
 
 ### Annotator Objects
 
-An Annotator object is the main interface for ERRANT.
+An Annotator object is the main interface for VNERRANT.
 
 #### Methods
 
 <details>
 <summary>annotator.parse</summary>
 
-`annotator.parse(string, tokenise=False)`
+`annotator.parse(string, tokenize_type='string')`
 
-Lemmatise, POS tag, and parse a text string with spacy. Set `tokenise` to True to also word tokenise with spacy. Returns a spacy Doc object.
+Lemmatise, POS tag, and parse a text string with spacy. Returns a spacy Doc object.
+
+`tokenize_type` must be in `["spacy", "split", "string"]`
+
+- `spacy`: tokenizing by default spacy tokenizer.
+- `split`: tokenizing by split function.
+- `string`: tokenizing by spacy and string tokenizer.
 
 </details>
 
 <details>
 <summary>annotator.align</summary>
 
 `annotator.align(orig, cor, lev=False)`
@@ -189,36 +199,63 @@
 </details>
 
 <details>
 <summary>annotator.annotate</summary>
 
 `annotator.annotate(orig, cor, lev=False, merging='rules')`
 
-Run the full annotation pipeline to align two sequences and extract and classify the edits. Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence. Returns a list of Edit objects.
+Run the full annotation pipeline to align two sequences and extract and classify the edits.
+Equivalent to running `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
 
 ```python
-import errant
+import vnerrant
 
-annotator = errant.load(lang="en", model_name="en_core_web_sm")
-orig = annotator.parse('This are gramamtical sentence .')
-cor = annotator.parse('This is a grammatical sentence .')
-alignment = annotator.align(orig, cor)
-edits = annotator.merge(alignment)
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = annotator.parse("My   name   is    the    John")
+cor = annotator.parse("My name is John")
+edits = annotator.annotate(orig, cor)
+for e in edits:
+    print(e)
+```
+
+</details>
+
+<details>
+<summary>annotator.annotate_raw</summary>
+
+`annotator.annotate_raw(orig: str, cor: str, lev=False, merging='rules', tokenize_type='string')`
+
+Run the full annotation pipeline to align two strings, extract and classify the edits.
+Equivalent to running `annotator.parse`, `annotator.align`, `annotator.merge` and `annotator.classify` in sequence.
+Returns a list of Edit objects.
+
+```python
+import vnerrant
+
+annotator = vnerrant.load(lang="en", model_name="en_core_web_sm")
+orig = "My   name   is    the    John"
+cor = "My name is John"
+edits = annotator.annotate_raw(orig, cor)
 for e in edits:
-    e = annotator.classify(e)
+    print(e)
 ```
 
 </details>
 
 <details>
 <summary>annotator.import_edit</summary>
 
 `annotator.import_edit(orig, cor, edit, min=True, old_cat=False)`
 
-Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form: `[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True to preserve the old error type category (i.e. turn off the classifier).
+Load an Edit object from a list. `orig` and `cor` must be spacy-parsed Doc objects and the edit must be of the form:
+`[o_start, o_end, c_start, c_end(, type)]`. The values must be integers that correspond to the token start and end
+offsets in the original and corrected Doc objects. The `type` value is an optional string that denotes the error type
+of the edit (if known). Set `min` to True to minimise the edit (e.g. [a b -> a c] = [b -> c]) and `old_cat` to True
+to preserve the old error type category (i.e. turn off the classifier).
 
 ```python
 import vnerrant
 
 annotator = vnerrant.load('en')
 orig = annotator.parse('This are gramamtical sentence .')
 cor = annotator.parse('This is a grammatical sentence .')
```

### Comparing `vnerrant-1.0.0/vnerrant.egg-info/SOURCES.txt` & `vnerrant-1.0.1rc1/vnerrant.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
+tests/test_vnerrant.py
 vnerrant/__init__.py
 vnerrant/annotator.py
 vnerrant/config.py
 vnerrant/constants.py
 vnerrant/run_cli.py
 vnerrant.egg-info/PKG-INFO
 vnerrant.egg-info/SOURCES.txt
@@ -16,28 +17,33 @@
 vnerrant/cli/convert.py
 vnerrant/cli/evaluate.py
 vnerrant/components/__init__.py
 vnerrant/components/alignment.py
 vnerrant/components/classifier.py
 vnerrant/components/converter.py
 vnerrant/components/evaluater.py
+vnerrant/components/explainer.py
 vnerrant/components/merger.py
 vnerrant/components/tokenizer.py
 vnerrant/components/en/__init__.py
 vnerrant/components/en/classifier.py
 vnerrant/components/en/constants.py
+vnerrant/components/en/explainer.py
 vnerrant/components/en/lancaster.py
 vnerrant/components/en/merger.py
 vnerrant/components/en/utils.py
 vnerrant/components/en/resources/README.md
 vnerrant/components/en/resources/en-ptb_map
 vnerrant/components/en/resources/en_GB-large.txt
+vnerrant/config/errant_verbose.json
 vnerrant/config/mapping_type_error.yaml
 vnerrant/metrics/__init__.py
 vnerrant/metrics/criteria.py
 vnerrant/metrics/stats.py
 vnerrant/model/__init__.py
 vnerrant/model/edit.py
 vnerrant/utils/__init__.py
+vnerrant/utils/edit_utils.py
 vnerrant/utils/helper.py
 vnerrant/utils/pretty_results.py
+vnerrant/utils/string_utils.py
 vnerrant/utils/utils.py
```

