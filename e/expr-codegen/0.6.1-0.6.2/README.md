# Comparing `tmp/expr_codegen-0.6.1.tar.gz` & `tmp/expr_codegen-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expr_codegen-0.6.1.tar", last modified: Sat Apr  6 05:08:13 2024, max compression
+gzip compressed data, was "expr_codegen-0.6.2.tar", last modified: Sun Apr 28 06:58:26 2024, max compression
```

## Comparing `expr_codegen-0.6.1.tar` & `expr_codegen-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/latex/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/template.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/polars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/template.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/latex/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/pandas/template.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/polars/template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/expr_codegen/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/expr_codegen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 06:58:26.000000 expr_codegen-0.6.2/expr_codegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-28 06:58:22.000000 expr_codegen-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:58:26.390576 expr_codegen-0.6.2/setup.cfg
```

### Comparing `expr_codegen-0.6.1/LICENSE` & `expr_codegen-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/PKG-INFO` & `expr_codegen-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.1
+Version: 0.6.2
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.1/README.md` & `expr_codegen-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/codes.py` & `expr_codegen-0.6.2/expr_codegen/codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import re
+from ast import expr
 
 from sympy import Add, Mul, Pow, Eq
 
 from expr_codegen.expr import register_symbols, dict_to_exprs
 
 
 class SympyTransformer(ast.NodeTransformer):
@@ -17,15 +18,15 @@
     funcs_new = set()
     args_new = set()
     targets_new = set()
 
     # 映射
     funcs_map = {}
     args_map = {}
-    targets_map = {}
+    targets_map = {}  # 只对非下划线开头的生效
 
     def config_map(self, funcs_map, args_map, targets_map):
         self.funcs_map = funcs_map
         self.args_map = args_map
         self.targets_map = targets_map
 
     def visit_Call(self, node):
@@ -39,26 +40,37 @@
                 self.args_old.add(arg.id)
                 arg.id = self.args_map.get(arg.id, arg.id)
                 self.args_new.add(arg.id)
 
         self.generic_visit(node)
         return node
 
+    def __visit_Assign(self, target: expr):
+        old_target_id = target.id
+        new_target_id = self.targets_map.get(old_target_id, old_target_id)
+        self.targets_old.add(old_target_id)
+
+        # 赋值给下划线开头代码时，对其进行重命名，方便重复书写表达式时不冲突
+        if old_target_id.startswith('_'):
+            new_target_id = f'{old_target_id}_{len(self.targets_new):03d}'
+
+        if old_target_id != new_target_id:
+            self.targets_new.add(new_target_id)
+            target.id = new_target_id
+            # 记录修改的变量名，之后会使用到
+            self.args_map[old_target_id] = new_target_id
+
     def visit_Assign(self, node):
         # 提取输出变量名
         for target in node.targets:
             if isinstance(target, ast.Tuple):
                 for t in target.elts:
-                    self.targets_old.add(t.id)
-                    t.id = self.targets_map.get(t.id, t.id)
-                    self.targets_new.add(t.id)
+                    self.__visit_Assign(t)
             else:
-                self.targets_old.add(target.id)
-                target.id = self.targets_map.get(target.id, target.id)
-                self.targets_new.add(target.id)
+                self.__visit_Assign(target)
 
         # 处理 alpha=close 这种情况
         if isinstance(node.value, ast.Name):
             self.args_old.add(node.value.id)
             node.value.id = self.args_map.get(node.value.id, node.value.id)
             self.args_new.add(node.value.id)
```

### Comparing `expr_codegen-0.6.1/expr_codegen/dag.py` & `expr_codegen-0.6.2/expr_codegen/dag.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/expr.py` & `expr_codegen-0.6.2/expr_codegen/expr.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/latex/printer.py` & `expr_codegen-0.6.2/expr_codegen/latex/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/model.py` & `expr_codegen-0.6.2/expr_codegen/model.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/pandas/code.py` & `expr_codegen-0.6.2/expr_codegen/pandas/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/pandas/printer.py` & `expr_codegen-0.6.2/expr_codegen/pandas/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/pandas/template.py.j2` & `expr_codegen-0.6.2/expr_codegen/pandas/template.py.j2`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 def main(df: pd.DataFrame) -> pd.DataFrame:
     # logger.info("start...")
     {% for key, value in groupbys.items() %}
     {{ value-}}
     {% endfor %}
 
     # drop intermediate columns
-    df = df.drop(columns=list(filter(lambda x: re.search(r"^_x_\d+", x), df.columns)))
+    # df = df.drop(columns=list(filter(lambda x: re.search(r"^_x_\d+", x), df.columns)))
+    df = df.drop(columns=list(filter(lambda x: x.startswith("_"), df.columns)))
 
     # logger.info('done')
 
     # save
     # df.to_parquet('output.parquet', compression='zstd')
 
     return df
```

### Comparing `expr_codegen-0.6.1/expr_codegen/polars/code.py` & `expr_codegen-0.6.2/expr_codegen/polars/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/polars/printer.py` & `expr_codegen-0.6.2/expr_codegen/polars/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen/polars/template.py.j2` & `expr_codegen-0.6.2/expr_codegen/polars/template.py.j2`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 def main(df: pl.DataFrame) -> pl.DataFrame:
     # logger.info("start...")
     {% for key, value in groupbys.items() %}
     {{ value-}}
     {% endfor %}
 
     # drop intermediate columns
-    df = df.select(pl.exclude(r'^_x_\d+$'))
+    # df = df.select(pl.exclude(r'^_x_\d+$'))
+    df = df.select(~cs.starts_with("_"))
 
     # shrink
     df = df.select(cs.all().shrink_dtype())
     df = df.shrink_to_fit()
 
     # logger.info('done')
```

### Comparing `expr_codegen-0.6.1/expr_codegen/tool.py` & `expr_codegen-0.6.2/expr_codegen/tool.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/expr_codegen.egg-info/PKG-INFO` & `expr_codegen-0.6.2/expr_codegen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.1
+Version: 0.6.2
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.1/expr_codegen.egg-info/SOURCES.txt` & `expr_codegen-0.6.2/expr_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.1/pyproject.toml` & `expr_codegen-0.6.2/pyproject.toml`

 * *Files identical despite different names*

