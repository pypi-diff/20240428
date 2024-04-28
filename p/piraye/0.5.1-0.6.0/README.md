# Comparing `tmp/piraye-0.5.1.tar.gz` & `tmp/piraye-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piraye-0.5.1.tar", last modified: Sun Apr 21 11:58:10 2024, max compression
+gzip compressed data, was "piraye-0.6.0.tar", last modified: Sun Apr 28 12:31:51 2024, max compression
```

## Comparing `piraye-0.5.1.tar` & `piraye-0.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-21 11:58:06.000000 piraye-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-21 11:58:10.294386 piraye-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 11:58:06.000000 piraye-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.286386 piraye-0.5.1/piraye/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/char_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/character_normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.286386 piraye-0.5.1/piraye/tasks/normalizer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/
--rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/en.json
--rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/fa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/digits/
--rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/digits/digits.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/others/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/deletions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/diacritics.json
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/others/spaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/normalizer/data/puncs/
--rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/data/puncs/puncs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/normalizer/normalizer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.290386 piraye-0.5.1/piraye/tasks/punc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/punc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/punc/punctuation_restoration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/piraye/tasks/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/nltk_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/punc_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tasks/tokenizer/spacy_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 11:58:06.000000 piraye-0.5.1/piraye/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/piraye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 11:58:10.000000 piraye-0.5.1/piraye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-21 11:58:06.000000 piraye-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:58:10.294386 piraye-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:58:10.294386 piraye-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_ml_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-21 11:58:06.000000 piraye-0.5.1/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-28 12:31:47.000000 piraye-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-28 12:31:51.362853 piraye-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-28 12:31:47.000000 piraye-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.358853 piraye-0.6.0/piraye/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.358853 piraye-0.6.0/piraye/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.358853 piraye-0.6.0/piraye/tasks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/char_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/character_normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.354853 piraye-0.6.0/piraye/tasks/normalizer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/
+-rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/fa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/normalizer/data/digits/
+-rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/digits/digits.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/normalizer/data/others/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/others/deletions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/others/diacritics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/others/spaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/normalizer/data/puncs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/data/puncs/puncs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/multi_lingual_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/normalizer/normalizer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/punc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/punc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/punc/punctuation_restoration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye/tasks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/tokenizer/nltk_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/tokenizer/punc_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tasks/tokenizer/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-28 12:31:47.000000 piraye-0.6.0/piraye/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/piraye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-28 12:31:51.000000 piraye-0.6.0/piraye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-28 12:31:51.000000 piraye-0.6.0/piraye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:31:51.000000 piraye-0.6.0/piraye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 12:31:51.000000 piraye-0.6.0/piraye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 12:31:51.000000 piraye-0.6.0/piraye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-28 12:31:47.000000 piraye-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:31:51.362853 piraye-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:31:51.362853 piraye-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-28 12:31:47.000000 piraye-0.6.0/tests/test_ml_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-28 12:31:47.000000 piraye-0.6.0/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-28 12:31:47.000000 piraye-0.6.0/tests/test_tokenizer.py
```

### Comparing `piraye-0.5.1/LICENSE` & `piraye-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/PKG-INFO` & `piraye-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.5.1
+Version: 0.6.0
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.5.1 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.6.0 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
```

### Comparing `piraye-0.5.1/README.md` & `piraye-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/__init__.py` & `piraye-0.6.0/piraye/__init__.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/normalizer.py` & `piraye-0.6.0/piraye/normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/char_config.py` & `piraye-0.6.0/piraye/tasks/normalizer/char_config.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/character_normalizer.py` & `piraye-0.6.0/piraye/tasks/normalizer/character_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/ar.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/ar.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/en.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/en.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/alphabets/fa.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/alphabets/fa.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/digits/digits.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/digits/digits.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/others/diacritics.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/others/diacritics.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/others/spaces.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/others/spaces.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/data/puncs/puncs.json` & `piraye-0.6.0/piraye/tasks/normalizer/data/puncs/puncs.json`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/mappings.py` & `piraye-0.6.0/piraye/tasks/normalizer/mappings.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer.py` & `piraye-0.6.0/piraye/tasks/normalizer/multi_lingual_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py` & `piraye-0.6.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/normalizer/normalizer_builder.py` & `piraye-0.6.0/piraye/tasks/normalizer/normalizer_builder.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/punc/punctuation_restoration.py` & `piraye-0.6.0/piraye/tasks/punc/punctuation_restoration.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/piraye/tasks/tokenizer/nltk_tokenizer.py` & `piraye-0.6.0/piraye/tasks/tokenizer/spacy_tokenizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,46 @@
-"""This module includes Tokenizer class for tokenizing texts"""
+"""This module includes a Tokenizer class for tokenizing texts"""
 from abc import ABC
 from typing import List, Tuple
 
-import nltk
-from nltk import NLTKWordTokenizer
-from nltk.tokenize.punkt import PunktSentenceTokenizer
+from spacy.lang.en import English
+from spacy.pipeline import Sentencizer
 
-from ..normalizer.mappings import MappingDict
 from ...tokenizer import Tokenizer
 
 
-class NltkTokenizer(Tokenizer, ABC):
+class SpacyTokenizer(Tokenizer, ABC):
     """
-    A class impl tokenizer with nltk
+    A class impl tokenizer with spacy
     ...
     Methods
     -------
     word_tokenize(text: str):
         return tokenized text
     sentence_tokenize(text: str):
         return sentence tokenized text
     """
 
-    def __init__(self, ):
+    def __init__(self):
         """
         constructor
         """
-        try:
-            nltk.data.find('tokenizers/punkt')
-        except LookupError:
-            print("downloading tokenizer data : ")
-            nltk.download('punkt')
-        self.__en_mapping = MappingDict.load_jsons(["digit_en", "punc_en"])
-        self.__tokenizer = NLTKWordTokenizer()
-        self.__sentence_tokenize = PunktSentenceTokenizer()
+        super().__init__()
+        self.__nlp = English()
+        self.__tokenizer = self.__nlp.tokenizer
+        self.__sentencizer = Sentencizer()
 
     def word_span_tokenize(self, text) -> List[Tuple[int, int, str]]:
-        text2 = self.__clean_text(text)
-        spans = self.__tokenizer.span_tokenize(text2)
-        return [(span[0], span[1], text[span[0]:span[1]]) for span in spans]
-
-    def sentence_span_tokenize(self, text) -> List[Tuple[int, int, str]]:
-        text2 = self.__clean_text(text)
-        spans = self.__sentence_tokenize.span_tokenize(text2)
-        return [(span[0], span[1], text[span[0]:span[1]]) for span in spans]
-
-    def __clean_text(self, text: str) -> str:
-        """
-        Clean the input text by replacing digits and punctuation with normalized versions.
-        :param text: he input text to clean.
-        :return: The cleaned text with normalized digits and punctuation.
-        """
-        return ''.join(
-            [char if not self.__en_mapping.get(char)
-             else self.__en_mapping.get(char).char for char in text])
+        text2 = self._clean_text(text)
+        spans = self.__tokenizer(text2)
+        return [(span.idx, span.idx + len(span.text), text[span.idx: span.idx + len(span.text)]) for span in spans]
+
+    def sentence_span_tokenize(self, text, clean_before_tokenize=True) -> List[Tuple[int, int, str]]:
+        text2 = self._clean_text(text) if clean_before_tokenize else text
+        spans = self.__sentencizer(self.__nlp(text2))
+        result = []
+        last_index = 0
+        for span in spans:
+            if span.is_sent_end:
+                result.append((last_index, span.idx + len(span.text), text[last_index:span.idx + len(span.text)]))
+                last_index = span.idx + len(span.text)
+        return result
```

### Comparing `piraye-0.5.1/piraye.egg-info/PKG-INFO` & `piraye-0.6.0/piraye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.5.1
+Version: 0.6.0
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.5.1 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.6.0 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
```

### Comparing `piraye-0.5.1/piraye.egg-info/SOURCES.txt` & `piraye-0.6.0/piraye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/pyproject.toml` & `piraye-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "piraye"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
     { name = "Hamed Khademi Khaledi", email = "khaledihkh@gmail.com" },
     { name = "HosseiN Khademi khaeldi", email = "hossein@arusha.dev" },
     { name = "Majid Asgiar Bidhendi", email = "majid@arusha.dev" },
 ]
 maintainers = [
     { name = "Arusha Developers", email = "info@arusha.dev" },
```

### Comparing `piraye-0.5.1/tests/test_ml_normalizer.py` & `piraye-0.6.0/tests/test_ml_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/tests/test_normalizer.py` & `piraye-0.6.0/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.5.1/tests/test_tokenizer.py` & `piraye-0.6.0/tests/test_tokenizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,23 @@
 def test_sentence_tokenizer():
     text = "sentence1 sad. \n asd asd \n asdasd \n sentence 2."
     tokenizer = NltkTokenizer()
     assert len(tokenizer.sentence_tokenize(text)) == 2
     assert len(tokenizer.sentence_span_tokenize(text)) == 2
 
 
+def test_paragraph_tokenizer():
+    text = "par1 sen1 sad.  par1 \n sen2. par1 \n\n sen3.  \n par2 sen1.\n\n\n\n   par3 sen1.\n\n"
+    tokenizer = NltkTokenizer()
+    assert len(tokenizer.paragraph_tokenize(text)) == 3
+    assert len(tokenizer.paragraph_span_tokenize(text)) == 3
+    assert len(tokenizer.paragraph_tokenize("par1 sen1 sad.")) == 1
+    assert len(tokenizer.paragraph_tokenize("par1 sen1 sad. par1 \n sen2. ")) == 1
+
+
 def test_sentence_tokenizer_spacy():
     text = "sentence1 sad. \n asd asd \n asdasd \n sentence 2."
     tokenizer = SpacyTokenizer()
     assert len(tokenizer.sentence_tokenize(text)) == 2
     assert len(tokenizer.sentence_span_tokenize(text)) == 2
```

