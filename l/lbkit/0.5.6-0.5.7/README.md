# Comparing `tmp/lbkit-0.5.6.tar.gz` & `tmp/lbkit-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbkit-0.5.6.tar", last modified: Tue Apr 16 16:17:49 2024, max compression
+gzip compressed data, was "lbkit-0.5.7.tar", last modified: Sun Apr 28 16:23:16 2024, max compression
```

## Comparing `lbkit-0.5.6.tar` & `lbkit-0.5.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/
--rw-rw-r--   0 root         (0) root         (0)      122 2024-04-16 16:17:40.000000 lbkit-0.5.6/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-16 16:17:40.000000 lbkit-0.5.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      149 2024-04-16 16:17:40.000000 lbkit-0.5.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-16 16:17:49.214934 lbkit-0.5.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      388 2024-04-16 16:17:40.000000 lbkit-0.5.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 16:17:41.000000 lbkit-0.5.6/lbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/ci_robot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/ci_robot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/ci_robot/gitee.py
--rw-rw-r--   0 root         (0) root         (0)     8483 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/codegen/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4241 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/codegen.py
--rw-rw-r--   0 root         (0) root         (0)    17074 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/ctype_defination.py
--rw-rw-r--   0 root         (0) root         (0)    30770 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/idf_interface.py
--rw-rw-r--   0 root         (0) root         (0)      287 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/codegen/template/
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/client.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/client.h.mako
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/interface.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/interface.introspect.xml.mako
--rw-rw-r--   0 root         (0) root         (0)    26271 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/public.c.mako
--rw-rw-r--   0 root         (0) root         (0)     8106 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/public.h.mako
--rw-rw-r--   0 root         (0) root         (0)    12974 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/server.c.mako
--rw-rw-r--   0 root         (0) root         (0)     1492 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/server.h.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/component/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/arg_parser.py
--rw-rw-r--   0 root         (0) root         (0)    13224 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/component/template/
--rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/template/conanbase.mako
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/template/deploy.mako
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/test.py
--rw-rw-r--   0 root         (0) root         (0)     2119 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/errors.py
--rw-rw-r--   0 root         (0) root         (0)      829 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_manifest.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_prepare.py
--rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_rootfs.py
--rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/config.py
--rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit/integration/template/
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/template/conanfile.py.mako
--rw-rw-r--   0 root         (0) root         (0)      114 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/lbkit.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/log.py
--rw-rw-r--   0 root         (0) root         (0)     3561 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/misc.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1268 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 16:17:49.214934 lbkit-0.5.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-16 16:17:40.000000 lbkit-0.5.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-04-28 16:23:09.000000 lbkit-0.5.7/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-28 16:23:09.000000 lbkit-0.5.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      149 2024-04-28 16:23:09.000000 lbkit-0.5.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-28 16:23:16.106330 lbkit-0.5.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-04-28 16:23:09.000000 lbkit-0.5.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.102330 lbkit-0.5.7/lbkit/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-28 16:23:10.000000 lbkit-0.5.7/lbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/ci_robot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/ci_robot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/ci_robot/gitee.py
+-rw-rw-r--   0 root         (0) root         (0)     8483 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/codegen/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4241 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/codegen.py
+-rw-rw-r--   0 root         (0) root         (0)    22507 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/ctype_defination.py
+-rw-rw-r--   0 root         (0) root         (0)    33054 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/idf_interface.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/codegen/template/
+-rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/client.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/client.h.mako
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/interface.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/interface.introspect.xml.mako
+-rw-rw-r--   0 root         (0) root         (0)    40159 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/public.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     9070 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/public.h.mako
+-rw-rw-r--   0 root         (0) root         (0)    13180 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/server.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     1440 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/server.h.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/component/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/arg_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    13224 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/component/template/
+-rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/template/conanbase.mako
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/template/deploy.mako
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/errors.py
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/integration/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_prepare.py
+-rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_rootfs.py
+-rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/integration/template/
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/template/conanfile.py.mako
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/lbkit.py
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3551 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 16:23:16.106330 lbkit-0.5.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-28 16:23:09.000000 lbkit-0.5.7/setup.py
```

### Comparing `lbkit-0.5.6/LICENSE` & `lbkit-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/PKG-INFO` & `lbkit-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.6/lbkit/ci_robot/gitee.py` & `lbkit-0.5.7/lbkit/ci_robot/gitee.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/cli.py` & `lbkit-0.5.7/lbkit/cli.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/codegen/codegen.py` & `lbkit-0.5.7/lbkit/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/codegen/ctype_defination.py` & `lbkit-0.5.7/lbkit/codegen/ctype_defination.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 """语言相关类型定义"""
 import sys
+from lbkit.errors import OdfValidateException
 
 
 class IdfValidator():
-    def odf_schema(self, allow_ref, idf_validator):
+    validator = {}
+
+    def set_validator(self, value):
+        self.validator = value
+
+    def odf_validate(self):
+        idf_validator = idf_validator
+        return []
+
+    def odf_schema(self, allow_ref):
+        allow_ref = allow_ref
+        idf_validator = idf_validator
         return None
 
 
 class BoolValidator(IdfValidator):
-    def odf_schema(self, allow_ref, idf_validator):
+    def odf_validate(self):
+        func = ["validate_odf_as_boolean(doc, node, prop, error_list)"]
+        return func
+
+    def odf_schema(self, allow_ref):
         if allow_ref:
             return {
                 "anyOf": [
                     {
                         "type": "boolean"
                     },
                     {
@@ -23,16 +39,20 @@
         else:
             return {
                 "type": "boolean"
             }
 
 
 class BoolArrayValidator(BoolValidator):
-    def odf_schema(self, allow_ref, idf_validator):
-        parent_schema = super().odf_schema(False, idf_validator)
+    def odf_validate(self):
+        func = ["validate_odf_as_boolean_v(doc, node, prop, error_list)"]
+        return func
+
+    def odf_schema(self, allow_ref):
+        parent_schema = super().odf_schema(False)
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "type": "array",
                         "item": parent_schema
                     },
@@ -50,54 +70,101 @@
         return schema
 
 
 class IntegerValidator(IdfValidator):
     maximum = sys.maxsize * 2
     minimum = -(sys.maxsize + 1) * 2
 
-    def __init__(self, max, min):
+    def __init__(self, max, min, signed=False):
         self.maximum = max
         self.minimum = min
+        self.signed = signed
+        if not self.signed and self.minimum < 0:
+            self.minimum = 0
+        if self.maximum < self.minimum:
+            raise OdfValidateException(f"The max value {self.maximum} less than or equal to {self.minimum}")
         super().__init__()
 
-    def odf_schema(self, allow_ref, idf_validator):
-        """
-            返回整数类型成员的ODF schema
-            idf_validator为IDF模型中加载的数据验证器的对象
-        """
-        max = idf_validator.get("max", self.maximum)
+    def set_validator(self, value):
+        super().set_validator(value)
+        max = self.validator.get("max", self.maximum)
         if max > self.maximum:
             max = self.maximum
-        min = idf_validator.get("min", self.minimum)
+        min = self.validator.get("min", self.minimum)
         if min < self.minimum:
             min = self.minimum
+        self.maximum = max
+        self.minimum = min
+        if not self.signed and self.minimum < 0:
+            self.minimum = 0
+        if self.maximum < self.minimum:
+            raise OdfValidateException(f"The max value {self.maximum} less than or equal to {self.minimum}")
+
+    def odf_validate(self):
+        func = []
+        if self.signed:
+            if self.minimum == -9223372036854775808:
+                func.append(f"validate_odf_as_signed(doc, node, prop, {self.maximum}, G_MININT64, error_list)")
+            else:
+                func.append(f"validate_odf_as_signed(doc, node, prop, {self.maximum}, {self.minimum}, error_list)")
+        else:
+            if self.maximum == 18446744073709551615:
+                func.append(f"validate_odf_as_unsigned(doc, node, prop, G_MAXUINT64, {self.minimum}, error_list)")
+            else:
+                func.append(f"validate_odf_as_unsigned(doc, node, prop, {self.maximum}, {self.minimum}, error_list)")
+        return func
+
+    def odf_schema(self, allow_ref):
+        """
+            返回整数类型成员的ODF schema
+            idf_validator为IDF模型中加载的数据验证器的对象
+        """
         if allow_ref:
             return {
                 "anyOf": [
                     {
                         "type": "integer",
-                        "maximum": max,
-                        "minimum": min
+                        "maximum": self.maximum,
+                        "minimum": self.minimum
                     },
                     {
                         "$ref": "#/$defs/ref_value"
                     }
                 ]
             }
         else:
             return {
                 "type": "integer",
-                "maximum": max,
-                "minimum": min
+                "maximum": self.maximum,
+                "minimum": self.minimum
             }
 
 
 class IntegerArrayValidator(IntegerValidator):
-    def odf_schema(self, allow_ref, idf_validator):
-        parent_schema = super().odf_schema(False, idf_validator)
+    def odf_validate(self):
+        func = []
+        min = self.minimum
+        max = self.maximum
+        if self.signed:
+            if self.minimum <= -0x8000_0000_0000_0000:
+                min = "G_MININT64"
+            if self.maximum >= 0x7fff_ffff_ffff_ffff:
+                max = "G_MAXINT64"
+        else:
+            if self.maximum >= 0xffff_ffff_ffff_ffff:
+                max = "G_MAXUINT64"
+
+        if self.signed:
+            func.append(f"validate_odf_as_signed_v(doc, node, prop, {max}, {min}, error_list)")
+        else:
+            func.append(f"validate_odf_as_unsigned_v(doc, node, prop, {max}, {min}, error_list)")
+        return func
+
+    def odf_schema(self, allow_ref):
+        parent_schema = super().odf_schema(False)
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "type": "array",
                         "item": parent_schema
                     },
@@ -115,60 +182,96 @@
         return schema
 
 
 class FloatValidator(IdfValidator):
     maximum = sys.float_info.max
     minimum = -sys.float_info.max
 
+    exclusive_max = None
+    exclusive_min = None
+
     def __init__(self):
+        self.max_key = "maximum"
+        self.max_val = self.maximum
+        self.min_key = "minimum"
+        self.min_val = self.minimum
         super().__init__()
 
-    def odf_schema(self, allow_ref, idf_validator):
+    def odf_validate(self):
+        func = ["validate_odf_as_double(doc, node, prop, error_list)"]
+        if self.exclusive_max is not None:
+            func.append(f"validate_odf_as_float_exclusive_max(doc, node, prop, {self.exclusive_max}, error_list)")
+        elif self.maximum != sys.float_info.max:
+            func.append(f"validate_odf_as_float_max(doc, node, prop, {self.maximum}, error_list)")
+
+        if self.exclusive_min is not None:
+            func.append(f"validate_odf_as_float_exclusive_min(doc, node, prop, {self.exclusive_min}, error_list)")
+        elif self.minimum != (-sys.float_info.max):
+            func.append(f"validate_odf_as_float_min(doc, node, prop, {self.minimum}, error_list)")
+        return func
+
+    def set_validator(self, value):
+        super().set_validator(value)
+        self.maximum = self.validator.get("max", self.maximum)
+        self.minimum = self.validator.get("min", self.minimum)
+        self.exclusive_max = self.validator.get("exclusive_max", None)
+        self.exclusive_min = self.validator.get("exclusive_min", None)
+        self.max_key = "maximum"
+        self.min_key = "minimum"
+        self.max_val = self.maximum
+        self.min_val = self.minimum
+        if self.exclusive_max is not None:
+            self.max_key = "exclusiveMaximum"
+            self.max_val = self.exclusive_max
+        if self.exclusive_min is not None:
+            self.max_key = "exclusiveMinimum"
+            self.min_val = self.exclusive_min
+
+    def odf_schema(self, allow_ref):
         """
             返回整数类型成员的ODF schema
             idf_validator为IDF模型中加载的数据验证器的对象
         """
-        max = idf_validator.get("max", self.maximum)
-        min = idf_validator.get("min", self.minimum)
-        exclusive_max = idf_validator.get("exclusive_max", None)
-        exclusive_min = idf_validator.get("exclusive_min", None)
-        max_key = "maximum"
-        max_val = max
-        min_key = "minimum"
-        min_val = min
-        if exclusive_max is not None:
-            max_key = "exclusiveMaximum"
-            max_val = exclusive_max
-        if exclusive_min is not None:
-            max_key = "exclusiveMinimum"
-            min_val = exclusive_min
         if allow_ref:
             return {
                 "anyOf": [
                     {
                         "type": "number",
-                        max_key: max_val,
-                        min_key: min_val
+                        self.max_key: self.max_val,
+                        self.min_key: self.min_val
                     },
                     {
                         "$ref": "#/$defs/ref_value"
                     }
                 ]
             }
         else:
             return {
                 "type": "number",
-                max_key: max_val,
-                min_key: min_val
+                self.max_key: self.max_val,
+                self.min_key: self.min_val
             }
 
 
 class FloatArrayValidator(FloatValidator):
-    def odf_schema(self, allow_ref, idf_validator):
-        parent_schema = super().odf_schema(False, idf_validator)
+    def odf_validate(self):
+        func = ["validate_odf_as_double_v(doc, node, prop, error_list)"]
+        if self.exclusive_max is not None:
+            func.append(f"validate_odf_as_float_exclusive_max_v(doc, node, prop, {self.exclusive_max}, error_list)")
+        elif self.maximum != sys.float_info.max:
+            func.append(f"validate_odf_as_float_max_v(doc, node, prop, {self.maximum}, error_list)")
+
+        if self.exclusive_min is not None:
+            func.append(f"validate_odf_as_float_exclusive_min_v(doc, node, prop, {self.exclusive_min}, error_list)")
+        elif self.minimum != (-sys.float_info.max):
+            func.append(f"validate_odf_as_float_min_v(doc, node, prop, {self.minimum}, error_list)")
+        return func
+
+    def odf_schema(self, allow_ref):
+        parent_schema = super().odf_schema(False)
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "type": "array",
                         "item": parent_schema
                     },
@@ -187,40 +290,62 @@
 
 class StringValidator(IdfValidator):
     pattern = None
     def __init__(self, pattern):
         self.pattern = pattern
         super().__init__()
 
-    def odf_schema(self, allow_ref, idf_validator):
-        pattern = idf_validator.get("pattern", self.pattern)
+    def set_validator(self, value):
+        self.pattern = self.validator.get("pattern", self.pattern)
+        super().set_validator(value)
+
+    def odf_validate(self):
+        func = []
+        if self.pattern is not None:
+            func.append(f"validate_odf_as_string(doc, node, prop, \"{self.pattern}\", error_list)")
+        else:
+            pattern = "^()|(((\\\\$)|[^$]).*)$"
+            func.append(f"validate_odf_as_string(doc, node, prop, \"{pattern}\", error_list)")
+        return func
+
+    def odf_schema(self, allow_ref):
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
-                        "type": "string"
+                        "type": "string",
+                        "pattern": "^()|(((\\\\$)|[^$]).*)$"
                     },
                     {
                         "$ref": "#/$defs/ref_value"
                     }
                 ]
             }
-            if pattern is not None:
-                schema["anyOf"][0]["pattern"] = pattern
+            if self.pattern is not None:
+                schema["anyOf"][0]["pattern"] = self.pattern
         else:
             schema = {
                 "type": "string",
-                "pattern": pattern
+                "pattern": self.pattern
             }
         return schema
 
 
 class StringArrayValidator(StringValidator):
-    def odf_schema(self, allow_ref, idf_validator):
-        parent_schema = super().odf_schema(False, idf_validator)
+    def odf_validate(self):
+        func = []
+        if self.pattern is not None:
+            func.append(f"validate_odf_as_string_v(doc, node, prop, \"{self.pattern}\", error_list)")
+        else:
+            pattern = "^()|(((\\\\$)|[^$]).*)$"
+            func.append(f"validate_odf_as_string_v(doc, node, prop, \"{pattern}\", error_list)")
+        return func
+
+    def odf_schema(self, allow_ref):
+        parent_schema = super().odf_schema(False)
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "type": "array",
                         "item": parent_schema
                     },
@@ -236,15 +361,19 @@
             }
         return schema
 
 class RefObjValidator(IdfValidator):
     def __init__(self):
         super().__init__()
 
-    def odf_schema(self, allow_ref, idf_validator):
+    def odf_validate(self):
+        func = ["validate_odf_as_ref_obj(doc, node, prop, error_list)"]
+        return func
+
+    def odf_schema(self, allow_ref):
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/ref_obj"
                     },
                     {
@@ -256,15 +385,19 @@
             schema = {
                 "$ref": "#/$defs/ref_obj"
             }
         return schema
 
 
 class RefObjArrayValidator(RefObjValidator):
-    def odf_schema(self, allow_ref, idf_validator):
+    def odf_validate(self):
+        func = ["validate_odf_as_ref_obj_v(doc, node, prop, error_list)"]
+        return func
+
+    def odf_schema(self, allow_ref):
         if allow_ref:
             schema = {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/ref_obj_array"
                     },
                     {
@@ -306,43 +439,43 @@
         IntegerValidator(0xff, 0)
     ),
     "int16": CTypeBase(
         ["gint16 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_int16(<arg_name>)"],
         ["<arg_in> = g_variant_get_int16(<arg_name>)"],
-        IntegerValidator(0x7fff, -(0x8000))
+        IntegerValidator(0x7fff, -(0x8000), True)
     ),
     "uint16": CTypeBase(
         ["guint16 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_uint16(<arg_name>)"],
         ["<arg_in> = g_variant_get_uint16(<arg_name>)"],
         IntegerValidator(0xffff, 0)
     ),
     "int32": CTypeBase(
         ["gint32 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_int32(<arg_name>)"],
         ["<arg_in> = g_variant_get_int32(<arg_name>)"],
-        IntegerValidator(0x7fff_ffff, -(0x8000_0000))
+        IntegerValidator(0x7fff_ffff, -(0x8000_0000), True)
     ),
     "uint32": CTypeBase(
         ["guint32 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_uint32(<arg_name>)"],
         ["<arg_in> = g_variant_get_uint32(<arg_name>)"],
         IntegerValidator(0xffff_ffff, 0)
     ),
     "int64": CTypeBase(
         ["gint64 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_int64(<arg_name>)"],
         ["<arg_in> = g_variant_get_int64(<arg_name>)"],
-        IntegerValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000))
+        IntegerValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000), True)
     ),
     "uint64": CTypeBase(
         ["guint64 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_uint64(<arg_name>)"],
         ["<arg_in> = g_variant_get_uint64(<arg_name>)"],
         IntegerValidator(0xffff_ffff_ffff_ffff, 0)
@@ -355,29 +488,29 @@
         IntegerValidator(0xffff_ffff_ffff_ffff, 0)
     ),
     "ssize": CTypeBase(
         ["gssize <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_int64(<arg_name>)"],
         ["<arg_in> = g_variant_get_int64(<arg_name>)"],
-        IntegerValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000))
+        IntegerValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000), True)
     ),
     "double": CTypeBase(
         ["gdouble <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_double(<arg_name>)"],
         ["<arg_in> = g_variant_get_double(<arg_name>)"],
         FloatValidator()
     ),
     "unixfd": CTypeBase(
         ["gint32 <arg_name>"],
         [],
         ["<arg_out> = g_variant_new_handle(<arg_name>)"],
         ["<arg_in> = g_variant_get_handle(<arg_name>)"],
-        IntegerValidator(0x7fff_ffff_ffff_ffff, 0)
+        IntegerValidator(0x7fff_ffff_ffff_ffff, 0, True)
     ),
     "string": CTypeBase(
         ["<const>gchar *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_string_encode(<arg_name>)"],
         ["<arg_in> = g_strdup(g_variant_get_string(<arg_name>, NULL))"],
         StringValidator("^.*$")
@@ -390,15 +523,15 @@
         StringValidator("^(/[A-Z0-9a-z_]+)*$")
     ),
     "signature": CTypeBase(
         ["<const>gchar *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_signature_encode(<arg_name>)"],
         ["<arg_in> = g_strdup(g_variant_get_string(<arg_name>, NULL))"],
-        StringValidator("^([abynqiuxtdsogv\\{\\}\\(\\)])+$")
+        StringValidator("^([abynqiuxtdsogv\\\\{\\\\}\\\\(\\\\)])+$")
     ),
     "variant": CTypeBase(
         ["GVariant *<arg_name>"],
         ["gcl_unref_p((GVariant **)&<arg_name>)"],
         ["g_variant_take_ref(<arg_name>)", "<arg_out> = g_variant_new_variant(<arg_name>)"],
         ["<arg_in> = g_variant_get_variant(<arg_name>)"],
         IdfValidator()
@@ -418,94 +551,94 @@
         IntegerArrayValidator(0xff, 0)
     ),
     "array[int16]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gint16 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_int16_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_int16_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0x7fff, -(0x8000))
+        IntegerArrayValidator(0x7fff, -(0x8000), True)
     ),
     "array[uint16]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>guint16 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_uint16_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_uint16_decode(<arg_name>, &n_<arg_in>)"],
         IntegerArrayValidator(0xffff, 0)
     ),
     "array[int32]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gint32 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_int32_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_int32_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0x7fff_ffff, -(0x80000000))
+        IntegerArrayValidator(0x7fff_ffff, -(0x80000000), True)
     ),
     "array[uint32]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>guint32 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_uint32_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_uint32_decode(<arg_name>, &n_<arg_in>)"],
         IntegerArrayValidator(0xffff_ffff, 0)
     ),
     "array[int64]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gint64 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_int64_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_int64_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000))
+        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000), True)
     ),
     "array[uint64]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>guint64 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_uint64_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_uint64_decode(<arg_name>, &n_<arg_in>)"],
         IntegerArrayValidator(0xffff_ffff_ffff_ffff, 0)
     ),
     "array[ssize]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gssize *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_int64_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_int64_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0xffff_ffff_ffff_ffff, 0)
+        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000), True)
     ),
     "array[size]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gsize *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_uint64_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_uint64_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, -(0x8000_0000_0000_0000))
+        IntegerArrayValidator(0xffff_ffff_ffff_ffff, 0)
     ),
     "array[double]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gdouble *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_double_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_double_decode(<arg_name>, &n_<arg_in>)"],
         FloatArrayValidator()
     ),
     "array[unixfd]": CTypeBase(
         ["gsize n_<arg_name>" ,"<const>gint32 *<arg_name>"],
         ["gcl_free_p((void **)&<arg_name>)"],
         ["<arg_out> = gcl_array_handle_encode(<arg_name>, n_<arg_name>)"],
         ["<arg_in> = gcl_array_handle_decode(<arg_name>, &n_<arg_in>)"],
-        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, 0)
+        IntegerArrayValidator(0x7fff_ffff_ffff_ffff, 0, True)
     ),
     "array[string]": CTypeBase(
-        ["gchar * <const>*<arg_name>"],
+        ["gchar *<const>*<arg_name>"],
         ["gcl_strfreev_p(&<arg_name>)"],
         ["<arg_out> = gcl_array_string_encode(<arg_name>)"],
         ["<arg_in> = gcl_array_string_decode(<arg_name>)"],
         StringArrayValidator("^.*$")
     ),
     "array[object_path]": CTypeBase(
-        ["gchar * <const>*<arg_name>"],
+        ["gchar *<const>*<arg_name>"],
         ["gcl_strfreev_p(&<arg_name>)"],
         ["<arg_out> = gcl_array_object_path_encode(<arg_name>)"],
         ["<arg_in> = gcl_array_object_path_decode(<arg_name>)"],
         StringArrayValidator("^(/[A-Z0-9a-z_]+)*$")
     ),
     "array[signature]": CTypeBase(
-        ["gchar * <const>*<arg_name>"],
+        ["gchar *<const>*<arg_name>"],
         ["gcl_strfreev_p(&<arg_name>)"],
         ["<arg_out> = gcl_array_signature_encode(<arg_name>)"],
         ["<arg_in> = gcl_array_signature_decode(<arg_name>)"],
-        StringArrayValidator("^([abynqiuxtdsogv\\{\\}\\(\\)])+$")
+        StringArrayValidator("^([abynqiuxtdsogv\\\\{\\\\}\\\\(\\\\)])+$")
     )
 }
```

### Comparing `lbkit-0.5.6/lbkit/codegen/idf_interface.py` & `lbkit-0.5.7/lbkit/codegen/idf_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 from lbkit.misc import validate_yml_with_json_schema
 
 log = Logger("gen_interface")
 
 class IDFException(Exception):
     pass
 
+class IdfInterfacePlugin(Renderer):
+    actions = []
 
 class IdfInterfaceBase(Renderer):
     def __init__(self) -> None:
         super(Renderer, self).__init__()
         self.file: str = None
         self.properties = []
         self.methods = []
         self.signals = []
         self.structures = {}
         self.dictionaries = {}
         self.enumerations = {}
         self.annotations = []
+        self.plugin: IdfInterfacePlugin = None
         self.description = None
         self.version = None
         self.alias = None
 
 class IdfAnnotation():
     def __init__(self, name, value):
         self.name = name
@@ -131,32 +134,65 @@
     def __init__(self):
         # 非基础类型
         match = re.match(f"^(set\[enum\[(.*)\]\])$", self.ctype)
         # 如果set类型由转换成数组，当前不具备对set类型独立处理能力
         if match:
             self.ctype = f"array[enum[{match.group(1)}]]"
 
+    def odf_validate(self, allow_ref):
+        log.debug(f"Get odf validate info, name: {self.name}, ctype: {self.ctype}")
+        if "variant" == self.ctype:
+            return []
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
+        if match:
+            if "refobj" in self.flags:
+                valiator = RefObjArrayValidator()
+                return valiator.odf_validate()
+            ctype_obj = CTYPE_OBJS.get(self.ctype)
+            return ctype_obj.validator.odf_validate()
+        match = re.match(f"^({CTYPE_BASE_REG})$", self.ctype)
+        if match:
+            if "refobj" in self.flags:
+                valiator = RefObjValidator()
+                return valiator.odf_validate()
+            ctype_obj = CTYPE_OBJS.get(self.ctype)
+            return ctype_obj.validator.odf_validate()
+        # 非基础类型
+        is_array = False
+        ctype = self.ctype
+        match = re.match(f"^array\[(.*)\]$", ctype)
+        if match:
+            is_array = True
+            ctype = match.group(1)
+        match = re.match(f"^(struct|enum|dict)\[(.*)\]$", ctype)
+        _, stru_name = get_intfname_and_ctype(match.group(2))
+        if is_array:
+            return [f"_validate_odf_as_{match.group(1)}_{stru_name}_v(doc, node, prop, error_list)"]
+        else:
+            return [f"_validate_odf_as_{match.group(1)}_{stru_name}(doc, node, prop, error_list)"]
+
+
     def odf_schema(self, allow_ref):
         log.debug(f"Get odf schema info, name: {self.name}, ctype: {self.ctype}")
         if "variant" == self.ctype:
             return None
         match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             if "refobj" in self.flags:
                 valiator = RefObjArrayValidator()
-                return valiator.odf_schema(allow_ref, {})
+                return valiator.odf_schema(allow_ref)
             ctype_obj = CTYPE_OBJS.get(self.ctype)
-            return ctype_obj.validator.odf_schema(allow_ref, {})
+            return ctype_obj.validator.odf_schema(allow_ref)
         match = re.match(f"^({CTYPE_BASE_REG})$", self.ctype)
         if match:
             if "refobj" in self.flags:
                 valiator = RefObjValidator()
-                return valiator.odf_schema(allow_ref, {})
+                return valiator.odf_schema(allow_ref)
             ctype_obj = CTYPE_OBJS.get(self.ctype)
-            return ctype_obj.validator.odf_schema(allow_ref, {})
+            return ctype_obj.validator.odf_schema(allow_ref)
         # 非基础类型
         is_array = False
         ctype = self.ctype
         match = re.match(f"^array\[(.*)\]$", ctype)
         if match:
             is_array = True
             ctype = match.group(1)
@@ -227,15 +263,15 @@
             is_array = True
             ctype = match.group(1)
         match = re.match(f"^(struct|enum|dict)\[(.*)\]$", ctype)
         _, stru_name = get_intfname_and_ctype(match.group(2))
         if match.group(1) == "struct":
             if is_array:
                 # 结构体数组初始化时为二级空指针，以空指针结束
-                return [f"{stru_name} * <const>*<arg_name>"]
+                return [f"{stru_name} *<const>*<arg_name>"]
             else:
                 # 结构体成员初始化时为空结构体，由反序列化时填充内容
                 return [f"<const>{stru_name} *<arg_name>"]
         elif match.group(1) == "enum":
             if is_array:
                 # 枚举数组初始化时为数组空指针
                 return [f"gsize n_<arg_name>", f"<const>{stru_name} *<arg_name>"]
@@ -478,14 +514,15 @@
 
     @property
     def signature(self):
         return ""
 
 
 class IdfMethod(IdfBase):
+    is_plugin = False
     def __init__(self, intf: IdfInterfaceBase, method_data):
         super().__init__(intf, method_data)
         self.parameters: IdfParameters = IdfParameters(intf, method_data.get("parameters", []))
         self.returns: IdfParameters = IdfParameters(intf, method_data.get("returns", []))
 
     @property
     def in_signature(self):
@@ -525,14 +562,23 @@
             "type": "object",
             "additionalProperties": False,
             # "required": [],
             "properties": schema
         }
         return odf
 
+
+class IdfPluginAction(IdfMethod):
+    is_plugin = True
+
+    def __init__(self, intf: IdfInterfaceBase, method_data):
+        self.policy = method_data.get("policy", "continue_always")
+        super().__init__(intf, method_data)
+
+
 class IdfEnumeration(IdfBase):
     def __init__(self, intf: IdfInterfaceBase, enum_data):
         super().__init__(intf, enum_data)
         self.values: list[IdfParameter] = IdfParameters(intf, enum_data.get("values", []))
 
     @property
     def signature(self):
@@ -648,14 +694,15 @@
         self.properties: list[IdfProperty] = []
         self.methods: list[IdfMethod] = []
         self.signals: list[IdfSignal] = []
         self.structures: dict[str, IdfStructure] = {}
         self.dictionaries: dict[str, IdfDictionary] = {}
         self.enumerations: dict[str, IdfEnumeration] = {}
         self.annotations: list[IdfAnnotation] = []
+        self.plugin: IdfInterfacePlugin = IdfInterfacePlugin()
         self.description = None
         self.version = None
         self.alias = None
         self.load_elements()
 
     @property
     def signature(self):
@@ -717,14 +764,23 @@
                             }
                         ]
                     }
                 }
             }
         return odf
 
+    @property
+    def fake_methods(self):
+        methods = []
+        for method in self.methods:
+            methods.append(method)
+        for action in self.plugin.actions:
+            methods.append(action)
+        return methods
+
     def load_elements(self):
         # 使用schema校验数据，确保IDF文件符合格式要求，减少程序处理过程中的异常处理
         # 验证失败时抛异常，此处不用处理，由外层处理
         validate_yml_with_json_schema(self.file, "/usr/share/litebmc/schema/idf.v1.json")
         log.info(f"validate {self.file} successfully")
         with open(self.file, "r") as fp:
             idf = yaml.load(fp, yaml.FullLoader)
@@ -755,14 +811,20 @@
         for item in items:
             obj = IdfDictionary(self, item)
             self.dictionaries[obj.name] = obj
         items = idf.get("enumerations", [])
         for item in items:
             obj = IdfEnumeration(self, item)
             self.enumerations[obj.name] = obj
+        plugin = idf.get("plugin", None)
+        if plugin is not None:
+            items = plugin.get("actions", [])
+            for item in items:
+                obj = IdfPluginAction(self, item)
+                self.plugin.actions.append(obj)
         log.debug("interface signature: " + self.signature)
         for signal in self.signals:
             log.debug(f"{signal.name} signature: " + signal.signature)
         for method in self.methods:
             log.debug(f"{method.name} in signature: " + method.in_signature + ", out signature: " + method.out_signature)
         for name, stru in self.structures.items():
             log.debug(f"{name} signature: " + stru.signature)
```

### Comparing `lbkit-0.5.6/lbkit/codegen/template/client.c.mako` & `lbkit-0.5.7/lbkit/codegen/template/client.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/codegen/template/client.h.mako` & `lbkit-0.5.7/lbkit/codegen/template/client.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/codegen/template/interface.introspect.xml.mako` & `lbkit-0.5.7/lbkit/codegen/template/interface.introspect.xml.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/codegen/template/public.c.mako` & `lbkit-0.5.7/lbkit/codegen/template/public.c.mako`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 #include "gcl_base.h"
 #include "${intf.name}.h"
 
 <% class_name = intf.alias %>\
+## 定义结构体ODF加载函数
+% for name, stru in intf.structures.items():
+/* ${name} structure object */
+/* START: 结构体${name}及其数组类型的ODF校验函数 */
+static gboolean _validate_odf_as_struct_${name}(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+static gboolean _validate_odf_as_struct_${name}_v(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+
+% endfor
+## 定义枚举ODF加载函数
+% for name, enum in intf.enumerations.items():
+/* START: 枚举${name}及其数组类型的ODF校验函数 */
+static gboolean _validate_odf_as_enum_${name}(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+static gboolean _validate_odf_as_enum_${name}_v(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+
+% endfor
+## 定义字典ODF加载函数
+% for name, dictionary in intf.dictionaries.items():
+static gboolean _validate_odf_as_dict_${name}(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+static gboolean _validate_odf_as_dict_${name}_v(yaml_document_t *doc, yaml_node_t *node, GString *prop, GSList **error_list);
+
+% endfor
 % for name, stru in intf.structures.items():
 /* ${name}结构体类型序列化（struct转GVariant）函数 */
 GVariant *${name}_encode(const ${name} *value)
 {
     % if stru.values.has_variant_value:
     g_assert(value);
 
@@ -127,14 +148,66 @@
     for (int i = 0; (*value)[i]; i++) {
         ${name}_free((*value) + i);
     }
     g_free(*value);
     *value = NULL;
 }
 
+gboolean _validate_odf_as_struct_${name}(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    g_assert(doc && node && prop && error_list);
+    if (node->type != YAML_MAPPING_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of property %s is not a mapping, get %s", prop->str, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+    gsize len = prop->len;
+    gboolean valid = TRUE;
+    yaml_node_t *val;
+    GHashTable *prop_table = load_yaml_mapping_to_hash_table(doc, node);
+    % for prop in stru.values.parameters:
+    val = g_hash_table_lookup(prop_table, "${prop.name}");
+    if (val) {
+        g_string_append(prop, ".${prop.name}");
+        % for func in prop.odf_validate(False):
+        if (!${func.replace("node,", "val,")})
+            valid = FALSE;
+        % endfor
+        g_string_truncate(prop, len);
+    }
+    % endfor
+    return valid;
+}
+
+gboolean _validate_odf_as_struct_${name}_v(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    g_assert(doc && node && prop && error_list);
+    if (node->type != YAML_SEQUENCE_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of property %s is not a sequence, get %s", prop->str, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+    gsize len = prop->len;
+    gint i = 0;
+    yaml_node_t *val = NULL;
+    gboolean valid = TRUE;
+    for (yaml_node_item_t *item = node->data.sequence.items.start; item < node->data.sequence.items.top; item++) {
+        g_string_append_printf(prop, ".%d", i);
+        val = yaml_document_get_node(doc, *item);
+        if (!_validate_odf_as_struct_${name}(doc, val, prop, error_list)) {
+            valid = FALSE;
+        }
+        g_string_truncate(prop, len);
+        i++;
+    }
+    return valid;
+}
+
 %endfor
 % for name, enum in intf.enumerations.items():
 ## 枚举序列化和反序列化函数
 static const gchar *_${name}StrMap[] = {
 % for value in enum.values.parameters:
     "${intf.name}.${name}.${value.name}",
 % endfor
@@ -213,14 +286,58 @@
                 output[id++] = (${name})i;
             }
         }
     }
     return output;
 }
 
+gboolean _validate_odf_as_enum_${name}(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    gboolean valid = validate_odf_as_string(doc, node, prop, "^.*$", error_list);
+    if (!valid) {
+        return FALSE;
+    }
+    const gchar *value = node->data.scalar.value;
+    for (int i = 0; i <= ${len(enum.values.parameters)}; i++) {
+        if (g_strcmp0(value, ${name}_as_string(i)) == 0) {
+            return TRUE;
+        }
+    }
+    *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+        "the value of property %s is is unsupportted, get %s", prop->str, value));
+    return FALSE;
+    return FALSE;
+}
+
+gboolean _validate_odf_as_enum_${name}_v(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    g_assert(doc && node && prop && error_list);
+    if (node->type != YAML_SEQUENCE_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of property %s is not a sequence, get %s", prop->str, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+    gsize len = prop->len;
+    gint i = 0;
+    yaml_node_t *val = NULL;
+    gboolean valid = TRUE;
+    for (yaml_node_item_t *item = node->data.sequence.items.start; item < node->data.sequence.items.top; item++) {
+        g_string_append_printf(prop, ".%d", i);
+        val = yaml_document_get_node(doc, *item);
+        if (!_validate_odf_as_enum_${name}(doc, val, prop, error_list)) {
+            valid = FALSE;
+        }
+        g_string_truncate(prop, len);
+        i++;
+    }
+    return valid;
+}
+
 % endfor
 ## 生成字典处理函数
 % for name, dictionary in intf.dictionaries.items():
 typedef struct {
     GHashTable *_hash;
     ${name} dict;
 } ${name}Real;
@@ -551,14 +668,88 @@
     for (int i = 0; (*value)[i]; i++) {
         ${name}_free((*value) + i);
     }
     g_free(*value);
     *value = NULL;
 }
 
+gboolean _validate_odf_as_dict_${name}(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    g_assert(doc && node && prop && error_list);
+    if (node->type != YAML_SEQUENCE_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of property %s is not a sequence, get %s", prop->str, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+
+    gboolean valid = TRUE;
+    GHashTable *prop_table = NULL;
+    yaml_node_t *val = NULL;
+    gsize len = prop->len;
+    yaml_node_item_t *top = node->data.sequence.items.top;
+    yaml_node_item_t *start = node->data.sequence.items.start;
+    for (yaml_node_item_t *item = start; item < top; item++) {
+        val = yaml_document_get_node(doc, *item);
+        ## 转换成hash表以获取key和properties
+        prop_table = load_yaml_mapping_to_hash_table(doc, val);
+        yaml_node_t *key = g_hash_table_lookup(prop_table, "key");
+        yaml_node_t *properties = g_hash_table_lookup(prop_table, "properties");
+        g_hash_table_destroy(prop_table);
+        g_string_append_printf(prop, ".key");
+        % for func in dictionary.key_obj.odf_validate(False):
+        if (!${func.replace("node,", "key,")})
+            valid = FALSE;
+        % endfor
+        g_string_truncate(prop, len);
+
+        ## 转换成hash表
+        prop_table = load_yaml_mapping_to_hash_table(doc, properties);
+        ## 迭代所有成员并从odf中还原数据
+        % for prop in dictionary.values.parameters:
+        val = g_hash_table_lookup(prop_table, "${prop.name}");
+        if (val) {
+            g_string_append(prop, ".properties.${prop.name}");
+            % for func in prop.odf_validate(False):
+            if (!${func.replace("node,", "val,")})
+                valid = FALSE;
+            % endfor
+            g_string_truncate(prop, len);
+        }
+        % endfor
+        g_hash_table_destroy(prop_table);
+    }
+    return valid;
+}
+
+gboolean _validate_odf_as_dict_${name}_v(yaml_document_t *doc, yaml_node_t *node,
+    GString *prop, GSList **error_list)
+{
+    g_assert(doc && node && prop && error_list);
+    if (node->type != YAML_SEQUENCE_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of property %s is not a sequence, get %s", prop->str, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+    gsize len = prop->len;
+    gint i = 0;
+    yaml_node_t *val = NULL;
+    gboolean valid = TRUE;
+    for (yaml_node_item_t *item = node->data.sequence.items.start; item < node->data.sequence.items.top; item++) {
+        g_string_append_printf(prop, ".%d", i);
+        val = yaml_document_get_node(doc, *item);
+        if (!_validate_odf_as_dict_${name}(doc, val, prop, error_list)) {
+            valid = FALSE;
+        }
+        g_string_truncate(prop, len);
+        i++;
+    }
+    return valid;
+}
+
 % endfor
 ## 生成每个属性的GDBus属性GDBusPropertyInfo对象name}
 % for prop in intf.properties:
     % if prop.private:
         % if len(prop.annotations) > 0:
 /* annotation for the property ${prop.name} */
 static GDBusAnnotationInfo ${class_name}_prop_${prop.name}_annotations_i[] = {
@@ -621,15 +812,16 @@
 };
 
 const ${class_name}_Properties *${class_name}_properties_const(void)
 {
     return &_${class_name}_properties;
 }
 
-% for method in intf.methods:
+% for method in intf.fake_methods:
+% if not method.is_plugin:
 ## 方法${method.name}的请求体序列化函数
 /* ${class_name}_${method.name}_Req请求结构体类型序列化（struct转GVariant）函数 */
 static GVariant *${class_name}_${method.name}_Req_encode(${class_name}_${method.name}_Req *value)
 {
     static ${class_name}_${method.name}_Req default_val;
     if (!value) {
         value = &default_val;
@@ -665,14 +857,15 @@
         % for line in prop.decode_func():
     ${line.replace("<arg_name>", "tmp").replace("n_<arg_in>", "output->n_" + prop.name).replace("<arg_in>", "output->" + prop.name)};
         % endfor
     g_variant_unref(tmp);
     % endfor
     return output;
 }
+% endif
 
 ## 方法${method.name}的请求体释放函数
 /* ${class_name}_${method.name}_Req结构体指针释放 */
 void ${class_name}_${method.name}_Req_free(${class_name}_${method.name}_Req **value)
 {
     if (!value || !(*value)) {
         return;
@@ -682,14 +875,15 @@
     ${line.replace("<arg_name>", "(*value)->" + prop.name)};
         % endfor
     % endfor
     g_free(*value);
     *value = NULL;
 }
 
+% if not method.is_plugin:
 /* ${class_name}_${method.name}_Rsp请求结构体类型序列化（struct转GVariant）函数 */
 static GVariant *${class_name}_${method.name}_Rsp_encode(${class_name}_${method.name}_Rsp *value)
 {
     static ${class_name}_${method.name}_Rsp default_val;
     if (!value) {
         value = &default_val;
     }
@@ -724,14 +918,15 @@
         % for line in prop.decode_func():
     ${line.replace("<arg_name>", "tmp").replace("n_<arg_in>", "output->n_" + prop.name).replace("<arg_in>", "output->" + prop.name)};
         % endfor
     g_variant_unref(tmp);
     % endfor
     return output;
 }
+% endif
 
 ## 方法${method.name}的响应体释放函数
 /* ${class_name}_${method.name}_Rsp结构体指针释放 */
 void ${class_name}_${method.name}_Rsp_free(${class_name}_${method.name}_Rsp **value)
 {
     if (!value || !(*value)) {
         return;
@@ -745,38 +940,126 @@
     *value = NULL;
 }
 
 % endfor
 static ${class_name}_Methods _${class_name}_methods =
 {
 % for method in intf.methods:
-    .${method.name} =
-{
+    .${method.name} = {
         .name = "${method.name}",
         .req_signature = "${method.in_signature}",
         .req_decode = (gcl_message_decode)${class_name}_${method.name}_Req_decode,
         .req_encode = (gcl_message_encode)${class_name}_${method.name}_Req_encode,
         .req_free = (gcl_message_free)${class_name}_${method.name}_Req_free,
         .rsp_signature = "${method.out_signature}",
         .rsp_decode = (gcl_message_decode)${class_name}_${method.name}_Rsp_decode,
         .rsp_encode = (gcl_message_encode)${class_name}_${method.name}_Rsp_encode,
         .rsp_free = (gcl_message_free)${class_name}_${method.name}_Rsp_free,
     },
 % endfor
-    .__reserved__ =
-{
+    .__reserved__ = {
         .name = NULL,
     }
 };
 
 ${class_name}_Methods *${class_name}_methods(void)
 {
     return &_${class_name}_methods;
 }
 
+% if len(intf.plugin.actions) > 0:
+    % for action in intf.plugin.actions:
+typedef struct {
+    gpointer user_data;
+    ${class_name}_${action.name}_action action;
+} _${class_name}_${action.name}_PluginAction;
+static GSList *_${class_name}_${action.name}_actions = NULL;
+static GMutex _${class_name}_${action.name}_lock;
+
+/* Register a new plugin action, can't register repeated with same action */
+int ${class_name}_${action.name}_register(const gchar *req_signature, const gchar *rsp_signature,
+    ${class_name}_${action.name}_action action, gpointer user_data)
+{
+    if (!req_signature) {
+        log_error("Register ${action.name} failed because parameter req_signature is NULL");
+        return -1;
+    }
+    if (!rsp_signature) {
+        log_error("Register ${action.name} failed because parameter rsp_signature is NULL");
+        return -1;
+    }
+    if (g_strcmp0(req_signature, "${action.in_signature}") != 0) {
+        log_error("Register ${action.name} failed because parameter "
+            "req_signature not match with \"{action.in_signature}\", get \"%s\"", req_signature);
+        return -1;
+    }
+    if (g_strcmp0(rsp_signature, "${action.out_signature}") != 0) {
+        log_error("Register ${action.name} failed because parameter "
+            "rsp_signature not match with \"{action.out_signature}\", get \"%s\"", rsp_signature);
+        return -1;
+    }
+    g_mutex_lock(&_${class_name}_${action.name}_lock);
+    for (GSList *item = _${class_name}_${action.name}_actions; item; item = item->next) {
+        _${class_name}_${action.name}_PluginAction *old_handler = (_${class_name}_${action.name}_PluginAction *)item->data;
+        if (action == old_handler->action || user_data == old_handler->user_data) {
+            g_mutex_unlock(&_${class_name}_${action.name}_lock);
+            return 0;
+        }
+    }
+    _${class_name}_${action.name}_PluginAction *handler = g_new0(_${class_name}_${action.name}_PluginAction, 1);
+    handler->user_data = user_data;
+    handler->action = action;
+    _${class_name}_${action.name}_actions = g_slist_append(_${class_name}_${action.name}_actions, handler);
+    g_mutex_unlock(&_${class_name}_${action.name}_lock);
+    return 0;
+}
+
+void ${class_name}_${action.name}_unregister(${class_name}_${action.name}_action action)
+{
+    g_mutex_lock(&_${class_name}_${action.name}_lock);
+    for (GSList *item = _${class_name}_${action.name}_actions; item; item = item->next) {
+        _${class_name}_${action.name}_PluginAction *old_handler = (_${class_name}_${action.name}_PluginAction *)item->data;
+        if (action == old_handler->action) {
+            _${class_name}_${action.name}_actions = g_slist_remove(_${class_name}_${action.name}_actions, old_handler);
+            g_free(old_handler);
+            break;
+        }
+        old_handler = NULL;
+    }
+    g_mutex_unlock(&_${class_name}_${action.name}_lock);
+}
+
+int ${class_name}_${action.name}_run(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp)
+{
+    gint result = 0;
+    g_mutex_lock(&_${class_name}_${action.name}_lock);
+    for (GSList *item = _${class_name}_${action.name}_actions; item; item = item->next) {
+        if (rsp && *rsp) {
+            ${class_name}_${action.name}_Rsp_free(rsp);
+        }
+        _${class_name}_${action.name}_PluginAction *handler = (_${class_name}_${action.name}_PluginAction *)item->data;
+        gint ret = handler->action(object, req, rsp, handler->user_data);
+        if (ret != 0)
+            result = ret;
+        % if action.policy == "return_any_success":
+        /* return when any action success(ret == 0) */
+        if (ret == 0)
+            break;
+        % elif action.policy == "return_any_fail":
+        /* return when any action failed(ret != 0) */
+        if (ret != 0)
+            break;
+        % endif
+    }
+    g_mutex_unlock(&_${class_name}_${action.name}_lock);
+    return result;
+}
+
+    % endfor
+% endif
 % for signal in intf.signals:
 ## 方法${method.name}的响应体序列化函数
 /* ${class_name}_${signal.name}_Msg请求结构体类型序列化（struct转GVariant）函数 */
 static GVariant *${class_name}_${signal.name}_Msg_encode(${class_name}_${signal.name}_Msg *value)
 {
     static ${class_name}_${signal.name}_Msg default_val;
     if (!value) {
@@ -851,7 +1134,71 @@
     }
 };
 
 ${class_name}_Signals *${class_name}_signals(void)
 {
     return &_${class_name}_signals;
 }
+
+% for prop in intf.properties:
+static gboolean _validate_odf_prop_${prop.name}(yaml_document_t *doc, GHashTable *prop_table,
+    GString *prop, GSList **error_list)
+{
+    gboolean valid = TRUE;
+    gsize len = prop->len;
+    yaml_node_t *node = g_hash_table_lookup(prop_table, "${prop.name}");
+    do {
+        if (!node)
+            break;
+        g_string_append(prop, ".${prop.name}");
+    % if "refobj" not in prop.flags:
+        if (validate_odf_as_ref_prop(doc, node, prop))
+            break;
+    % endif
+    % if len(prop.odf_validate(True)) > 1:
+        % for func in prop.odf_validate(True):
+        if (valid && !${func})
+            valid = FALSE;
+        % endfor
+    % else:
+        % for func in prop.odf_validate(True):
+        valid = ${func};
+        % endfor
+    % endif
+    } while (0);
+    g_string_truncate(prop, len);
+    return valid;
+}
+
+%endfor
+gboolean ${intf.name.replace(".", "_")}_validate_odf(yaml_document_t *doc, yaml_node_t *node,
+    const gchar *object_name, GSList **error_list)
+{
+    g_assert(doc && node && object_name && error_list);
+    if (!doc || !node || !object_name || !error_list) {
+        return FALSE;
+    }
+
+    if (node->type != YAML_MAPPING_NODE) {
+        *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
+            "the node type of object %s is not a mapping, get %s", object_name, gcl_yaml_node_type_str(node->type)));
+        return FALSE;
+    }
+    GString *prop = g_string_sized_new(128);
+    g_string_printf(prop, "%s", object_name);
+    gboolean valid = TRUE;
+    GHashTable *prop_table = load_yaml_mapping_to_hash_table(doc, node);
+    % for prop in stru.values.parameters:
+    valid = _validate_odf_prop_${prop.name}(doc, prop_table, prop, error_list) && valid;
+    % endfor
+    return valid;
+}
+
+% if len(intf.plugin.actions) > 0:
+static void __attribute__((constructor(101))) ${class_name}_public_register(void)
+{
+    % for action in intf.plugin.actions:
+    g_mutex_init(&_${class_name}_${action.name}_lock);
+    % endfor
+}
+
+% endif
```

### Comparing `lbkit-0.5.6/lbkit/codegen/template/public.h.mako` & `lbkit-0.5.7/lbkit/codegen/template/public.h.mako`

 * *Files 21% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 ${name} **${name}_decode_v(GVariant *in);
 void ${name}_free_v(${name} ***value);
 /* END: 字典${name}及其数组类型的序列化、反序列化、释放函数 */
 
 % endfor
 
 ### 开始生成方法的请求体、响应体和处理函数
-% for method in intf.methods:
+% for method in intf.fake_methods:
 /* ${method.name}方法的请求体 */
 typedef struct {
         % for arg in method.parameters.parameters:
             % for dec in arg.declare():
     ${dec.replace("<arg_name>", arg.name).replace("<const>", "")};
             % endfor
         % endfor
@@ -144,15 +144,17 @@
         % for arg in method.returns.parameters:
             % for dec in arg.declare():
     ${dec.replace("<arg_name>", arg.name).replace("<const>", "")};
             % endfor
         % endfor
 } ${class_name}_${method.name}_Rsp;
 
+% if not method.is_plugin:
 typedef int (*${class_name}_${method.name}_Method)(const ${class_name} *object, const ${class_name}_${method.name}_Req *req, ${class_name}_${method.name}_Rsp **rsp, GError **error);
+% endif
 void ${class_name}_${method.name}_Req_free(${class_name}_${method.name}_Req **value);
 void ${class_name}_${method.name}_Rsp_free(${class_name}_${method.name}_Rsp **value);
 %endfor
 
 /* ${intf.name}的方法集合 */
 typedef struct {
 % for method in intf.methods:
@@ -168,14 +170,26 @@
         gcl_message_free rsp_free;
         ${class_name}_${method.name}_Method handler;
     } ${method.name};
 % endfor
     GclMethod __reserved__;
 } ${class_name}_Methods;
 
+% if len(intf.plugin.actions) > 0:
+% for action in intf.plugin.actions:
+typedef int (*${class_name}_${action.name}_action)(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp, gpointer user_data);
+
+/* Register a new plugin action, can't register repeated with same action and user_data */
+int ${class_name}_${action.name}_register(const gchar *req_signature, const gchar *rsp_signature,
+    ${class_name}_${action.name}_action action, gpointer user_data);
+void ${class_name}_${action.name}_unregister(${class_name}_${action.name}_action action);
+int ${class_name}_${action.name}_run(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp);
+
+% endfor
+% endif
 ### 开始生成方法的请求体、响应体和处理函数
 % for signal in intf.signals:
 /* ${signal.name}信号的消息体 */
 typedef struct {
         % for arg in signal.properties.parameters:
             % for dec in arg.declare():
     ${dec.replace("<arg_name>", arg.name).replace("<const>", "")};
@@ -216,14 +230,17 @@
 typedef struct {
 % for prop in intf.properties:
     GclProperty ${prop.name};
 % endfor
     GclProperty __reserved__;
 } ${class_name}_Properties;
 
+
+gboolean ${intf.name.replace(".", "_")}_validate_odf(yaml_document_t *doc, yaml_node_t *node,
+    const gchar *object_name, GSList **error_list);
 // 不要使用此函数返回的对象，需要使用${class_name}_properties() 或${class_name}_Cli_properties()
 const ${class_name}_Properties *${class_name}_properties_const(void);
 // 同时加载客户端和服务端时Processer是共享的，因此可以直接调用Processer定义的handler函数
 ${class_name}_Signals *${class_name}_signals(void);
 ${class_name}_Methods *${class_name}_methods(void);
 /* Interface ${intf.name} codegen finish */
```

### Comparing `lbkit-0.5.6/lbkit/codegen/template/server.c.mako` & `lbkit-0.5.7/lbkit/codegen/template/server.c.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<% from lbkit.codegen.ctype_defination import StringValidator %>\
 #include "gcl_base.h"
 #include "${intf.name}.h"
 
 <%
 class_name = intf.alias
 properties = "_" + class_name + "_properties"
 signal_processer = "_" + class_name + "_signals"
@@ -232,23 +233,26 @@
         (const GclSignal *)&${signal_processer}->${signal.name}, msg, error);
 }
 
 % endfor
 static GclObject *_${class_name}_create(const gchar *obj_name, gpointer opaque);
 static void _load_from_odf(yaml_document_t *doc, yaml_node_t *node, GclObject *gcl_obj,
     property_reference_loaded ref_loaded, gpointer user_data);
+static void _valid_from_odf(yaml_document_t *doc, yaml_node_t *node, const gchar *object_name);
+
 /*
  * interface: ${intf.name}
 % for c in intf.description.split("\n"):
  * ${c}
 % endfor
  */
 static GclInterface _${class_name}_interface = {
     .create = _${intf.alias}_create,
-    .load_from_odf = (object_load_from_odf)_load_from_odf,
+    .validate_odf = ${intf.name.replace(".", "_")}_validate_odf,
+    .load_from_odf = _load_from_odf,
     .is_remote = 0,
     .name = "${intf.name}",
     .properties = (GclProperty *)&${properties},
     .interface = NULL,  /* load from usr/share/dbus-1/interfaces/${intf.name} by gcl_init */
 };
 
 % for prop in intf.properties:
```

### Comparing `lbkit-0.5.6/lbkit/codegen/template/server.h.mako` & `lbkit-0.5.7/lbkit/codegen/template/server.h.mako`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 % for prop in intf.properties:
 #define ${class_name.upper()}_${prop.name}_NAME    "${prop.name}"
 % endfor
 
 GclInterface *${class_name}_interface(void);
 #define ${class_name.upper()}_INTERFACE ${class_name}_interface()
 ${class_name}_Properties *${class_name}_properties(void);
-${class_name}_Methods *${class_name}_methods(void);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* __${"_".join(intf.name.upper().split(".", -1))}_H__ */
```

### Comparing `lbkit-0.5.6/lbkit/component/arg_parser.py` & `lbkit-0.5.7/lbkit/component/arg_parser.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/component/build.py` & `lbkit-0.5.7/lbkit/component/build.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/component/template/conanbase.mako` & `lbkit-0.5.7/lbkit/component/template/conanbase.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/component/template/deploy.mako` & `lbkit-0.5.7/lbkit/component/template/deploy.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/component/test.py` & `lbkit-0.5.7/lbkit/component/test.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/errors.py` & `lbkit-0.5.7/lbkit/errors.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/helper.py` & `lbkit-0.5.7/lbkit/helper.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/build_manifest.py` & `lbkit-0.5.7/lbkit/integration/build_manifest.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/build_prepare.py` & `lbkit-0.5.7/lbkit/integration/build_prepare.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/build_rootfs.py` & `lbkit-0.5.7/lbkit/integration/build_rootfs.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/config.py` & `lbkit-0.5.7/lbkit/integration/config.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/task.py` & `lbkit-0.5.7/lbkit/integration/task.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/integration/template/conanfile.py.mako` & `lbkit-0.5.7/lbkit/integration/template/conanfile.py.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/log.py` & `lbkit-0.5.7/lbkit/log.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit/misc.py` & `lbkit-0.5.7/lbkit/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
         fp = open(yml_file, "r")
         data = yaml.safe_load(fp)
         fp.close()
         validate(data, schema)
     except ValidationError as exc:
         raise PackageConfigException(f"validate {yml_file} failed, schema file is {schema_file}, "
                                      f"message: {exc.message}\n"
-                                     "installing redhat.vscode-yaml plugin in vscode will help you write odf files") from exec
+                                     "installing redhat.vscode-yaml plugin in vscode will help you write odf files")
```

### Comparing `lbkit-0.5.6/lbkit/tools.py` & `lbkit-0.5.7/lbkit/tools.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/lbkit.egg-info/PKG-INFO` & `lbkit-0.5.7/lbkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.6/lbkit.egg-info/SOURCES.txt` & `lbkit-0.5.7/lbkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.6/setup.py` & `lbkit-0.5.7/setup.py`

 * *Files identical despite different names*

