# Comparing `tmp/Cemotion-2.1.1.tar.gz` & `tmp/cemotion-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cemotion-2.1.1.tar", last modified: Sun Mar 31 09:28:45 2024, max compression
+gzip compressed data, was "cemotion-2.2.1.tar", last modified: Sun Apr 28 12:20:52 2024, max compression
```

## Comparing `Cemotion-2.1.1.tar` & `cemotion-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:28:45.774909 Cemotion-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:28:45.774909 Cemotion-2.1.1/Cemotion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-31 09:28:45.000000 Cemotion-2.1.1/Cemotion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-31 09:28:45.000000 Cemotion-2.1.1/Cemotion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:28:45.000000 Cemotion-2.1.1/Cemotion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-31 09:28:45.000000 Cemotion-2.1.1/Cemotion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 09:28:45.000000 Cemotion-2.1.1/Cemotion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-31 09:28:37.000000 Cemotion-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-31 09:28:45.774909 Cemotion-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-31 09:28:37.000000 Cemotion-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:28:45.774909 Cemotion-2.1.1/cemotion/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-31 09:28:37.000000 Cemotion-2.1.1/cemotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-31 09:28:37.000000 Cemotion-2.1.1/cemotion/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-31 09:28:37.000000 Cemotion-2.1.1/cemotion/download.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:28:45.774909 Cemotion-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-31 09:28:37.000000 Cemotion-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/Cemotion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 12:20:52.000000 cemotion-2.2.1/Cemotion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-28 12:20:45.000000 cemotion-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-28 12:20:52.896203 cemotion-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-28 12:20:45.000000 cemotion-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:20:52.896203 cemotion-2.2.1/cemotion/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-28 12:20:45.000000 cemotion-2.2.1/cemotion/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:20:52.896203 cemotion-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 12:20:45.000000 cemotion-2.2.1/setup.py
```

### Comparing `Cemotion-2.1.1/LICENSE` & `cemotion-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Cemotion-2.1.1/cemotion/download.py` & `cemotion-2.2.1/cemotion/download.py`

 * *Files identical despite different names*

### Comparing `Cemotion-2.1.1/setup.py` & `cemotion-2.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Cemotion",
-    version="2.1.1",
+    version="2.2.1",
     author="Cyberbolt",
     author_email="dtconlyone@gmail.com",
-    description="基于 BERT 的中文情感倾向分析库，用于中文文本分类、中文情感分析",
+    description="Cemotion 是 Python 下的中文 NLP 库，可以进行中文情感倾向分析、通用领域中文分词。",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'tqdm>=4.64.1',
         'joblib>=1.0.0',
         'requests>=2.25.1',
         'numpy>=1.19.5',
         'torch>=2.0.0',
-        'transformers>=4.39.2',
+        'transformers>=4.24.0',
+        'modelscope>=1.14.0',
     ]    
 )
```

