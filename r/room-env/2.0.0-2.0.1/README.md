# Comparing `tmp/room_env-2.0.0.tar.gz` & `tmp/room_env-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "room_env-2.0.0.tar", last modified: Sat Apr 20 09:24:56 2024, max compression
+gzip compressed data, was "room_env-2.0.1.tar", last modified: Sun Apr 28 12:01:38 2024, max compression
```

## Comparing `room_env-2.0.0.tar` & `room_env-2.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 09:24:47.000000 room_env-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-20 09:24:56.143458 room_env-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-20 09:24:47.000000 room_env-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.131458 room_env-2.0.0/room_env/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/create_room2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/room_env/data/
--rw-r--r--   0 runner    (1001) docker     (127)   429221 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/conceptnet-data.json
--rw-r--r--   0 runner    (1001) docker     (127)    47857 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-l-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-m-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-s-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-xs-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-xxs-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/human-locations
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/human-names
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/ms-coco-80-categories
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/names-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   108782 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-dev-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)  3908646 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-foo-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-l-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-m-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-s-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   110149 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xl-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xs-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   411708 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xxl-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xxs-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/semantic-knowledge-small.json
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/semantic-knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/top-human-names
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/top-human-names-small
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/des.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/room_env/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room1.py
--rw-r--r--   0 runner    (1001) docker     (127)    35910 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.131458 room_env-2.0.0/room_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-20 09:24:56.143458 room_env-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:24:47.000000 room_env-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-20 09:24:47.000000 room_env-2.0.0/test/test_des.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-20 09:24:47.000000 room_env-2.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.906397 room_env-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 12:01:29.000000 room_env-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-28 12:01:38.906397 room_env-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-28 12:01:29.000000 room_env-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.894397 room_env-2.0.1/room_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/create_room_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.906397 room_env-2.0.1/room_env/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   429221 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/conceptnet-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47857 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/des-config-l-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/des-config-m-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/des-config-s-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/des-config-xs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/des-config-xxs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/human-locations
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/human-names
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/ms-coco-80-categories
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/names-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   108782 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-dev-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3908646 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-foo-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-l-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-m-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-s-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110149 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-xl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-xs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   411708 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-xxl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/room-config-xxs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/semantic-knowledge-small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/semantic-knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/top-human-names
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/data/top-human-names-small
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.906397 room_env-2.0.1/room_env/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/envs/room0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/envs/room1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35910 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/envs/room2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-04-28 12:01:29.000000 room_env-2.0.1/room_env/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.898397 room_env-2.0.1/room_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-28 12:01:38.000000 room_env-2.0.1/room_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-28 12:01:38.000000 room_env-2.0.1/room_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:01:38.000000 room_env-2.0.1/room_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-28 12:01:38.000000 room_env-2.0.1/room_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 12:01:38.000000 room_env-2.0.1/room_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-28 12:01:38.910397 room_env-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 12:01:29.000000 room_env-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:01:38.906397 room_env-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-28 12:01:29.000000 room_env-2.0.1/test/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-28 12:01:29.000000 room_env-2.0.1/test/test_utils.py
```

### Comparing `room_env-2.0.0/LICENSE` & `room_env-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/PKG-INFO` & `room_env-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: room_env
-Version: 2.0.0
+Version: 2.0.1
 Summary: The Room environment
 Home-page: https://github.com/humemai/room-env
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/room-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `room_env-2.0.0/README.md` & `room_env-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/create_room2.py` & `room_env-2.0.1/room_env/create_room_v2.py`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/conceptnet-data.json` & `room_env-2.0.1/room_env/data/conceptnet-data.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/des-config-l-v1.json` & `room_env-2.0.1/room_env/data/des-config-l-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/des-config-m-v1.json` & `room_env-2.0.1/room_env/data/des-config-m-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/des-config-s-v1.json` & `room_env-2.0.1/room_env/data/des-config-s-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/des-config-xs-v1.json` & `room_env-2.0.1/room_env/data/des-config-xs-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/des-config-xxs-v1.json` & `room_env-2.0.1/room_env/data/des-config-xxs-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/human-names` & `room_env-2.0.1/room_env/data/human-names`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/ms-coco-80-categories` & `room_env-2.0.1/room_env/data/ms-coco-80-categories`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/names-v2.json` & `room_env-2.0.1/room_env/data/names-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-dev-v2.json` & `room_env-2.0.1/room_env/data/room-config-dev-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-foo-v2.json` & `room_env-2.0.1/room_env/data/room-config-foo-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-l-v2.json` & `room_env-2.0.1/room_env/data/room-config-l-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-m-v2.json` & `room_env-2.0.1/room_env/data/room-config-m-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-s-v2.json` & `room_env-2.0.1/room_env/data/room-config-s-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-xl-v2.json` & `room_env-2.0.1/room_env/data/room-config-xl-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-xs-v2.json` & `room_env-2.0.1/room_env/data/room-config-xs-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-xxl-v2.json` & `room_env-2.0.1/room_env/data/room-config-xxl-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/room-config-xxs-v2.json` & `room_env-2.0.1/room_env/data/room-config-xxs-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/semantic-knowledge-small.json` & `room_env-2.0.1/room_env/data/semantic-knowledge-small.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/data/semantic-knowledge.json` & `room_env-2.0.1/room_env/data/semantic-knowledge.json`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/des.py` & `room_env-2.0.1/room_env/des.py`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/envs/room0.py` & `room_env-2.0.1/room_env/envs/room0.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,17 +241,14 @@
 
         With the chance of probs["switch_person"], two persons switch their spots.
 
         """
         room = []
         for head, relation, tail in self.room:
             name1, head = split_by_possessive(head)
-            # name2, tail = split_by_possessive(tail)
-
-            # assert name1 == name2, "we don't do name mixing at this moment."
 
             if random.random() < self.probs["new_object"]:
                 while True:
                     new_head = random.choice(self.heads)
                     if new_head != head:
                         head = new_head
                         tail = self.generate_tail(head, relation)
```

### Comparing `room_env-2.0.0/room_env/envs/room1.py` & `room_env-2.0.1/room_env/envs/room1.py`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/envs/room2.py` & `room_env-2.0.1/room_env/envs/room2.py`

 * *Files identical despite different names*

### Comparing `room_env-2.0.0/room_env/utils.py` & `room_env-2.0.1/room_env/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,27 +153,14 @@
 
 
 def argmax(iterable) -> int:
     """argmax"""
     return max(enumerate(iterable), key=lambda x: x[1])[0]
 
 
-def remove_posession(entity: str) -> str:
-    """Remove name from the entity.
-
-    Args:
-        entity: e.g., bob's laptop
-
-    Returns:
-        e.g., laptop
-
-    """
-    return entity.split("'s ")[-1]
-
-
 def split_by_possessive(name_entity: str) -> tuple[str, str]:
     """Separate name and entity from the given string.
 
     Args:
         name_entity: e.g., "tae's laptop"
 
     Returns:
```

### Comparing `room_env-2.0.0/room_env.egg-info/PKG-INFO` & `room_env-2.0.1/room_env.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: room-env
-Version: 2.0.0
+Version: 2.0.1
 Summary: The Room environment
 Home-page: https://github.com/humemai/room-env
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/room-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `room_env-2.0.0/room_env.egg-info/SOURCES.txt` & `room_env-2.0.1/room_env.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 room_env/__init__.py
-room_env/create_room2.py
+room_env/create_room_v2.py
 room_env/des.py
 room_env/utils.py
 room_env.egg-info/PKG-INFO
 room_env.egg-info/SOURCES.txt
 room_env.egg-info/dependency_links.txt
 room_env.egg-info/requires.txt
 room_env.egg-info/top_level.txt
```

### Comparing `room_env-2.0.0/setup.cfg` & `room_env-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = room_env
-version = 2.0.0
+version = 2.0.1
 author = Taewoon Kim
 author_email = info@humem.ai
 description = The Room environment
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/humemai/room-env
 project_urls =
```

### Comparing `room_env-2.0.0/test/test_utils.py` & `room_env-2.0.1/test/test_utils.py`

 * *Files identical despite different names*

