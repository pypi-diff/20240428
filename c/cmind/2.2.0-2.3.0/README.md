# Comparing `tmp/cmind-2.2.0.tar.gz` & `tmp/cmind-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.2.0.tar", last modified: Tue Apr 23 18:02:44 2024, max compression
+gzip compressed data, was "cmind-2.3.0.tar", last modified: Sun Apr 28 12:43:27 2024, max compression
```

## Comparing `cmind-2.2.0.tar` & `cmind-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-23 17:59:41.000000 cmind-2.2.0/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-23 18:02:44.541275 cmind-2.2.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11260 2024-04-23 17:59:41.000000 cmind-2.2.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28644 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/ckx/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/ckx/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.541275 cmind-2.2.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    38748 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    25437 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47067 2024-04-23 17:59:41.000000 cmind-2.2.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-23 18:02:44.531275 cmind-2.2.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1279 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-23 18:02:44.000000 cmind-2.2.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-23 18:02:44.541275 cmind-2.2.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2913 2024-04-23 17:59:41.000000 cmind-2.2.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-28 12:38:52.000000 cmind-2.3.0/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-28 12:43:27.024759 cmind-2.3.0/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11260 2024-04-28 12:38:52.000000 cmind-2.3.0/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      190 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      100 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4918 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47952 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6467 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3315 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28674 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9541 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2076 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2666 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4047 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8846 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/ckx/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1003 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1109 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1091 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      269 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10292 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      305 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    39862 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2038 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    25467 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47294 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1279 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-28 12:43:27.024759 cmind-2.3.0/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2913 2024-04-28 12:38:52.000000 cmind-2.3.0/setup.py
```

### Comparing `cmind-2.2.0/LICENSE.md` & `cmind-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.2.0/PKG-INFO` & `cmind-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.2.0
+Version: 2.3.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.2.0/README.md` & `cmind-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.2.0/cmind/artifact.py` & `cmind-2.3.0/cmind/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind artifact
+#
+# Written by Grigori Fursin
 
 import os
 
 from cmind import utils
 
 class Artifact:
     """
```

### Comparing `cmind-2.2.0/cmind/automation.py` & `cmind-2.3.0/cmind/automation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind automation
+#
+# Written by Grigori Fursin
 
 import os
 
 from cmind import utils
 from cmind.artifact import Artifact
 
 self_path = __file__
@@ -116,17 +118,17 @@
         print ('Path to CM internal repo:   {}'.format(self.cmind.repos.path_to_internal_repo))
 
         print ('')
         print ('Path to CM repositories:    {}'.format(self.cmind.repos_path))
 
         print ('')
         print ('GitHub for CM developments:        https://github.com/mlcommons/ck/tree/master/cm')
-        print ('GitHub for CM automation scripts:  https://github.com/mlcommons/ck/tree/master/cm-mlops')
+        print ('GitHub for CM automation scripts:  https://github.com/mlcommons/cm4mlops')
         print ('Reporting issues and ideas:        https://github.com/mlcommons/ck/issues')
-        print ('Joining the open MLPerf workgroup: https://cKnowledge.org/mlcommons-taskforce')
+        print ('MLCommons taskforce developing CM: https://github.com/mlcommons/ck/blob/master/docs/taskforce.md')
 
         return {'return':0}
 
     ############################################################
     def search(self, i):
         """
         Find CM artifacts (slow - we plan to accelerate it in the future using different indexing mechanisms)
```

### Comparing `cmind-2.2.0/cmind/cli.py` & `cmind-2.3.0/cmind/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Collective Mind command line wrapper
+#
+# Written by Grigori Fursin
 
 import sys
 
 ############################################################
 def run(argv = None):
     """
     Run CM automation actions from the command line.
```

### Comparing `cmind-2.2.0/cmind/config.py` & `cmind-2.3.0/cmind/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind configuration
+#
+# Written by Grigori Fursin
 
 import os
 
 class Config(object):
     """
     CM configuration class
     """
```

### Comparing `cmind-2.2.0/cmind/core.py` & `cmind-2.3.0/cmind/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Collective Mind core functions
+#
+# Written by Grigori Fursin
 
 from cmind.config import Config
 from cmind.repos import Repos
 from cmind.index import Index
 from cmind.automation import Automation
 from cmind import utils
```

### Comparing `cmind-2.2.0/cmind/index.py` & `cmind-2.3.0/cmind/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind index
+#
+# Written by Grigori Fursin
 
 import os
 import json
 
 from cmind import utils
 
 class Index:
```

### Comparing `cmind-2.2.0/cmind/net.py` & `cmind-2.3.0/cmind/net.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Reused from the CK framework for compatibility
+#
+# Written by Grigori Fursin
 
 import urllib
 import json
 import sys
 
 try:
     from urllib.parse import urlencode
```

### Comparing `cmind-2.2.0/cmind/repo/automation/automation/README.md` & `cmind-2.3.0/cmind/repo/automation/automation/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -60,8 +60,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-2.2.0/cmind/repo/automation/automation/module.py` & `cmind-2.3.0/cmind/repo/automation/automation/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# CM automation module to add or document all automations
+#
+# Written by Grigori Fursin
+
 import os
 
 from cmind.automation import Automation
 from cmind import utils
 
 class CAutomation(Automation):
     """
```

### Comparing `cmind-2.2.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.3.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.2.0/cmind/repo/automation/automation/module_misc.py` & `cmind-2.3.0/cmind/repo/automation/automation/module_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Documenting CM automations
+#
+# Written by Grigori Fursin
+
 import os
 from cmind import utils
     
 ############################################################
 def doc(i):
     """
     Document CM automations.
@@ -183,15 +187,15 @@
             line_number+=1
 
         md.append('\n')
 
         # Add maintainers
         md_script_readme.append('### Maintainers')
         md_script_readme.append('')
-        md_script_readme.append('* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)')
+        md_script_readme.append('* [MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)')
 
 
         # Check README and if it's already automatically generated
         path_readme = os.path.join(path, 'README.md')
         path_readme_extra = os.path.join(path, 'README-extra.md')
 
         if os.path.isfile(path_readme):
```

### Comparing `cmind-2.2.0/cmind/repo/automation/ckx/README.md` & `cmind-2.3.0/cmind/repo/automation/ckx/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-2.2.0/cmind/repo/automation/ckx/module.py` & `cmind-2.3.0/cmind/repo/automation/ckx/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# CM wrapper for older CK framework in case it is still needed
+#
+# Written by Grigori Fursin
+
 import os
 
 from cmind.automation import Automation
 from cmind import utils
 
 class CAutomation(Automation):
     """
```

### Comparing `cmind-2.2.0/cmind/repo/automation/core/README.md` & `cmind-2.3.0/cmind/repo/automation/core/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-2.2.0/cmind/repo/automation/core/module.py` & `cmind-2.3.0/cmind/repo/automation/core/module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# CM core automation with a few universal functions
+#
+# Written by Grigori Fursin
+
 import os
 
 from cmind.automation import Automation
 from cmind import utils
 
 # This is just an example of how to import extra files from such a package
 # We need to make it unique!
```

### Comparing `cmind-2.2.0/cmind/repo/automation/repo/README.md` & `cmind-2.3.0/cmind/repo/automation/repo/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -260,8 +260,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-2.2.0/cmind/repo/automation/repo/module.py` & `cmind-2.3.0/cmind/repo/automation/repo/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# CM automation to manage CM repositories
+#
+# Written by Grigori Fursin
+
 import os
 
 from cmind.automation import Automation
 from cmind import utils
 
 class CAutomation(Automation):
     """
@@ -95,18 +99,37 @@
                     # Pick it up from the path
 
                     repo_path = repo.path
 
                     pull_repos.append({'alias': os.path.basename(repo_path),
                                        'path_to_repo': repo_path})
         else:
+            # We are migrating cm-mlops repo from mlcommons@ck to a clean and new mlcommons@cm4mlops:
+            # https://github.com/mlcommons/ck/issues/1215
+            # As discussed, we should have a transparent redirect with a warning
+            # unless branch/checkout is used - in such case we keep old repository
+            # for backwards compatibility and reproducibility
+
+            branch = i.get('branch', '')
+            checkout = i.get('checkout', '')
+
+            if alias == 'mlcommons@ck' and branch == '' and checkout == '':
+                print ('=========================================================================')
+                print ('Warning: mlcommons@ck was automatically changed to mlcommons@cm4mlops.')
+                print ('If you want to use older mlcommons@ck repository, use branch or checkout.')
+                print ('=========================================================================')
+
+                alias = 'mlcommons@cm4mlops'
+                url = url.replace('mlcommons/ck', 'mlcommons/cm4mlops')
+
+
             pull_repos = [{'alias':alias,
                            'url':url,
-                           'branch': i.get('branch', ''),
-                           'checkout': i.get('checkout', ''),
+                           'branch': branch,
+                           'checkout': checkout,
                            'depth': i.get('depth', '')}]
 
 
         # Go through repositories and pull
         repo_meta = {}
         repo_metas = {}
```

### Comparing `cmind-2.2.0/cmind/repo.py` & `cmind-2.3.0/cmind/repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind repository
+#
+# Written by Grigori Fursin
 
 import os
 
 from cmind import utils
 
 class Repo:
     """
```

### Comparing `cmind-2.2.0/cmind/repos.py` & `cmind-2.3.0/cmind/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ﻿# Collective Mind repositories
+#
+# Written by Grigori Fursin
 
 import os
 
 from cmind.repo import Repo
 from cmind import utils
 
 class Repos:
```

### Comparing `cmind-2.2.0/cmind/utils.py` & `cmind-2.3.0/cmind/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Auxilary functions for CM
-
+#
 # Some functionality was reused from the CK framework for compatibility
+#
+# Written by Grigori Fursin
 
 import os
 
 ERROR_UNKNOWN_FILE_EXTENSION = 1
 ERROR_PATH_NOT_FOUND = 2
 ERROR_FILE_NOT_FOUND = 16
 
@@ -1211,15 +1213,16 @@
 
 ##############################################################################
 def get_current_date_time(i):
     """
     Get current date and time.
 
     Args:    
-       (CM input dict): empty dict
+       (CM input dict): 
+         - (timezone) (str): timezone in pytz format: "Europe/Paris"
 
     Returns: 
        (CM return dict):
 
        * return (int): return code == 0 if no error and >0 if error
        * (error) (str): error string if return>0
 
@@ -1235,15 +1238,22 @@
        * iso_datetime (str): date and time in ISO format
     """
 
     import datetime
 
     a = {}
 
-    now1 = datetime.datetime.now()
+    tz = None
+
+    tz_str = i.get('timezone', '').strip()
+    if tz_str != '':
+        import pytz
+        tz = pytz.timezone(tz_str)
+
+    now1 = datetime.datetime.now(tz)
     now = now1.timetuple()
 
     a['date_year'] = now[0]
     a['date_month'] = now[1]
     a['date_day'] = now[2]
     a['time_hour'] = now[3]
     a['time_minute'] = now[4]
```

### Comparing `cmind-2.2.0/cmind.egg-info/PKG-INFO` & `cmind-2.3.0/cmind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.2.0
+Version: 2.3.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.2.0/cmind.egg-info/SOURCES.txt` & `cmind-2.3.0/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-2.2.0/setup.py` & `cmind-2.3.0/setup.py`

 * *Files identical despite different names*

