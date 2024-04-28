# Comparing `tmp/aikicore-1.0.0a4.tar.gz` & `tmp/aikicore-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikicore-1.0.0a4.tar", last modified: Thu Apr 25 22:52:31 2024, max compression
+gzip compressed data, was "aikicore-1.0.0a5.tar", last modified: Sat Apr 27 02:59:46 2024, max compression
```

## Comparing `aikicore-1.0.0a4.tar` & `aikicore-1.0.0a5.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996775 aikicore-1.0.0a4/
--rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a4/LICENSE
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-25 22:52:31.996558 aikicore-1.0.0a4/PKG-INFO
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.994487 aikicore-1.0.0a4/aikicore/
--rw-r--r--   0 ashatz     (501) staff       (20)     2503 2024-04-24 01:08:35.000000 aikicore-1.0.0a4/aikicore/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)       55 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/activity.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996160 aikicore-1.0.0a4/aikicore/config/
--rw-r--r--   0 ashatz     (501) staff       (20)     3115 2024-04-25 22:51:55.000000 aikicore-1.0.0a4/aikicore/config/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/config/json.py
--rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/config/yaml.py
--rw-r--r--   0 ashatz     (501) staff       (20)      334 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/constants.py
--rw-r--r--   0 ashatz     (501) staff       (20)      575 2024-04-24 01:05:56.000000 aikicore-1.0.0a4/aikicore/containers.py
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/domain.py
--rw-r--r--   0 ashatz     (501) staff       (20)     1784 2024-04-25 22:40:31.000000 aikicore-1.0.0a4/aikicore/error.py
--rw-r--r--   0 ashatz     (501) staff       (20)     5762 2024-04-24 22:01:58.000000 aikicore-1.0.0a4/aikicore/routing.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996354 aikicore-1.0.0a4/aikicore.egg-info/
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/PKG-INFO
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/SOURCES.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/dependency_links.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/requires.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/top_level.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-25 22:52:31.996822 aikicore-1.0.0a4/setup.cfg
--rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-25 22:52:11.000000 aikicore-1.0.0a4/setup.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-27 02:59:46.141390 aikicore-1.0.0a5/
+-rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a5/LICENSE
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-27 02:59:46.141158 aikicore-1.0.0a5/PKG-INFO
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-27 02:59:46.138226 aikicore-1.0.0a5/aikicore/
+-rw-r--r--   0 ashatz     (501) staff       (20)     2434 2024-04-27 02:55:04.000000 aikicore-1.0.0a5/aikicore/__init__.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-27 02:59:46.140317 aikicore-1.0.0a5/aikicore/config/
+-rw-r--r--   0 ashatz     (501) staff       (20)     3115 2024-04-25 22:51:55.000000 aikicore-1.0.0a5/aikicore/config/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a5/aikicore/config/json.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a5/aikicore/config/yaml.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      559 2024-04-27 02:47:15.000000 aikicore-1.0.0a5/aikicore/constants.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-27 02:59:46.140862 aikicore-1.0.0a5/aikicore.egg-info/
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-27 02:59:46.000000 aikicore-1.0.0a5/aikicore.egg-info/PKG-INFO
+-rw-r--r--   0 ashatz     (501) staff       (20)      294 2024-04-27 02:59:46.000000 aikicore-1.0.0a5/aikicore.egg-info/SOURCES.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-27 02:59:46.000000 aikicore-1.0.0a5/aikicore.egg-info/dependency_links.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-27 02:59:46.000000 aikicore-1.0.0a5/aikicore.egg-info/requires.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-27 02:59:46.000000 aikicore-1.0.0a5/aikicore.egg-info/top_level.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-27 02:59:46.141443 aikicore-1.0.0a5/setup.cfg
+-rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-27 02:59:01.000000 aikicore-1.0.0a5/setup.py
```

### Comparing `aikicore-1.0.0a4/LICENSE` & `aikicore-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a4/aikicore/__init__.py` & `aikicore-1.0.0a5/aikicore/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from typing import Dict
 
 from .constants import APP_CONFIGURATION_FILE
 from .config import load_app_config_reader, AppConfigurationReader, AppConfiguration
-from .error import *
-from .containers import *
-from .routing import *
-from .domain import *
+from .objects import *
 
 
 class AppContext():
 
     name: str = None
     interface: str = None
     container_config: ContainerConfiguration = None
```

### Comparing `aikicore-1.0.0a4/aikicore/config/__init__.py` & `aikicore-1.0.0a5/aikicore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a4/setup.py` & `aikicore-1.0.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 config = {
     'description': 'The Core Library for the Spirit of Harmony',
     'author': 'Andrew Shatz',
     'url': r'https://github.com/Great-Strength-Studios/aikicore',
     'download_url': r'https://github.com/Great-Strength-Studios/aikicore',
     'author_email': 'andrew@greatstrength.me',
-    'version': '1.0.0-alpha.4',
+    'version': '1.0.0-alpha.5',
     'license': 'BSD 3',
     'install_requires': [
         'schematics>=2.1.1',
         'pyyaml>=6.0.1'
     ],
     'packages': [
         'aikicore',
```

