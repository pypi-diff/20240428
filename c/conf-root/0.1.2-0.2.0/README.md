# Comparing `tmp/conf_root-0.1.2.tar.gz` & `tmp/conf_root-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.1.2.tar", last modified: Tue Mar 12 12:14:03 2024, max compression
+gzip compressed data, was "conf_root-0.2.0.tar", last modified: Sun Apr 28 15:48:48 2024, max compression
```

## Comparing `conf_root-0.1.2.tar` & `conf_root-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:14:03.939168 conf_root-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 12:13:57.000000 conf_root-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-12 12:14:03.939168 conf_root-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-12 12:13:57.000000 conf_root-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:14:03.935168 conf_root-0.1.2/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-12 12:13:57.000000 conf_root-0.1.2/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:14:03.935168 conf_root-0.1.2/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-12 12:13:57.000000 conf_root-0.1.2/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-12 12:13:57.000000 conf_root-0.1.2/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-12 12:13:57.000000 conf_root-0.1.2/conf_root/agents/YamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-12 12:13:57.000000 conf_root-0.1.2/conf_root/conf_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:14:03.939168 conf_root-0.1.2/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-12 12:14:03.000000 conf_root-0.1.2/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-12 12:14:03.000000 conf_root-0.1.2/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:14:03.000000 conf_root-0.1.2/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 12:14:03.000000 conf_root-0.1.2/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 12:14:03.939168 conf_root-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-12 12:13:57.000000 conf_root-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:14:03.939168 conf_root-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-12 12:13:57.000000 conf_root-0.1.2/tests/test_json_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-12 12:13:57.000000 conf_root-0.1.2/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-12 12:13:57.000000 conf_root-0.1.2/tests/test_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-12 12:13:57.000000 conf_root-0.1.2/tests/test_yaml_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:48:48.146382 conf_root-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 15:48:44.000000 conf_root-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-28 15:48:48.146382 conf_root-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-28 15:48:44.000000 conf_root-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:48:48.146382 conf_root-0.2.0/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/ArgparseConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:48:48.146382 conf_root-0.2.0/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/agents/YamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-28 15:48:44.000000 conf_root-0.2.0/conf_root/conf_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:48:48.146382 conf_root-0.2.0/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-28 15:48:48.000000 conf_root-0.2.0/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-28 15:48:48.000000 conf_root-0.2.0/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:48:48.000000 conf_root-0.2.0/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 15:48:48.000000 conf_root-0.2.0/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:48:48.146382 conf_root-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-28 15:48:44.000000 conf_root-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:48:48.146382 conf_root-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-28 15:48:44.000000 conf_root-0.2.0/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-28 15:48:44.000000 conf_root-0.2.0/tests/test_json_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-28 15:48:44.000000 conf_root-0.2.0/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-28 15:48:44.000000 conf_root-0.2.0/tests/test_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-28 15:48:44.000000 conf_root-0.2.0/tests/test_yaml_agent.py
```

### Comparing `conf_root-0.1.2/LICENSE` & `conf_root-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/conf_root/agents/BasicAgent.py` & `conf_root-0.2.0/conf_root/agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/conf_root/agents/JsonAgent.py` & `conf_root-0.2.0/conf_root/agents/JsonAgent.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     default_extension = 'json'
 
     def create(self, cls):
         # 将dataclass默认值转换为dict，便于序列化
         default_dict = self.dataclass_default_dict(cls)
 
         # 将dict转换为YAML并写入文件
-        with open(self.location, "w") as file:
-            json.dump(default_dict, file)
+        if len(default_dict.keys()) > 0:
+            with open(self.location, "w") as file:
+                json.dump(default_dict, file)
 
     def load(self, cls, obj):
         with open(self.location, encoding='utf-8') as file:
             data = json.load(file)
 
         # 将dict展开为对象。
         self.dict_to_dataclass(data, cls, obj)
```

### Comparing `conf_root-0.1.2/conf_root/agents/YamlAgent.py` & `conf_root-0.2.0/conf_root/agents/YamlAgent.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     default_extension = 'yml'
 
     def create(self, cls):
         # 将dataclass默认值转换为dict，便于序列化
         default_dict = self.dataclass_default_dict(cls)
 
         # 将dict转换为YAML并写入文件
-        with open(self.location, "w") as yaml_file:
-            yaml.dump(default_dict, yaml_file)
+        if len(default_dict.keys()) > 0:
+            with open(self.location, "w") as yaml_file:
+                yaml.dump(default_dict, yaml_file)
 
     def load(self, cls, obj):
         with open(self.location, encoding='utf-8') as yaml_file:
             data = yaml.safe_load(yaml_file)
 
         # 将dict展开为对象。
         self.dict_to_dataclass(data, cls, obj)
```

### Comparing `conf_root-0.1.2/conf_root/conf_root.py` & `conf_root-0.2.0/conf_root/conf_root.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/setup.py` & `conf_root-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.1.2",  # 版本号
+    version="0.2.0",  # 版本号
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的符合逻辑的配置取用方式。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ciaranchen/conf_root",
     packages=["conf_root", "conf_root.agents"],  # 包含的Python模块或子包
```

### Comparing `conf_root-0.1.2/tests/test_json_agent.py` & `conf_root-0.2.0/tests/test_json_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/tests/test_nested_dataclass.py` & `conf_root-0.2.0/tests/test_nested_dataclass.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/tests/test_normal.py` & `conf_root-0.2.0/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.1.2/tests/test_yaml_agent.py` & `conf_root-0.2.0/tests/test_yaml_agent.py`

 * *Files identical despite different names*

