# Comparing `tmp/thrift_pyi-0.8.0.tar.gz` & `tmp/thrift_pyi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thrift_pyi-0.8.0.tar", max compression
+gzip compressed data, was "thrift_pyi-0.9.0.tar", max compression
```

## Comparing `thrift_pyi-0.8.0.tar` & `thrift_pyi-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-11-02 19:34:19.477861 thrift_pyi-0.8.0/LICENSE
--rw-r--r--   0        0        0     3470 2023-11-02 19:34:19.477861 thrift_pyi-0.8.0/README.rst
--rw-r--r--   0        0        0     1280 2023-11-02 19:34:19.477861 thrift_pyi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-02 19:34:19.477861 thrift_pyi-0.8.0/src/thriftpyi/__init__.py
--rw-r--r--   0        0        0       92 2023-11-02 19:34:19.477861 thrift_pyi-0.8.0/src/thriftpyi/__main__.py
--rw-r--r--   0        0        0     1091 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/cli.py
--rw-r--r--   0        0        0      183 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/compat.py
--rw-r--r--   0        0        0     5035 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/entities.py
--rw-r--r--   0        0        0      391 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/files.py
--rw-r--r--   0        0        0     1664 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/main.py
--rw-r--r--   0        0        0     5636 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/proxies.py
--rw-r--r--   0        0        0        0 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/py.typed
--rw-r--r--   0        0        0     2679 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/stubs.py
--rw-r--r--   0        0        0     2694 2023-11-02 19:34:19.481860 thrift_pyi-0.8.0/src/thriftpyi/utils.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 thrift_pyi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-04-28 08:15:01.459256 thrift_pyi-0.9.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1074 2024-04-28 08:15:01.459256 thrift_pyi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3470 2024-04-28 08:15:01.459256 thrift_pyi-0.9.0/README.rst
+-rw-r--r--   0        0        0     1280 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/__main__.py
+-rw-r--r--   0        0        0     1091 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/cli.py
+-rw-r--r--   0        0        0      183 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/compat.py
+-rw-r--r--   0        0        0     5035 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/entities.py
+-rw-r--r--   0        0        0      391 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/files.py
+-rw-r--r--   0        0        0     1664 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/main.py
+-rw-r--r--   0        0        0     5888 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/proxies.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/py.typed
+-rw-r--r--   0        0        0     2679 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/stubs.py
+-rw-r--r--   0        0        0     3422 2024-04-28 08:15:01.463256 thrift_pyi-0.9.0/src/thriftpyi/utils.py
+-rw-r--r--   0        0        0     4521 1970-01-01 00:00:00.000000 thrift_pyi-0.9.0/PKG-INFO
```

### Comparing `thrift_pyi-0.8.0/LICENSE` & `thrift_pyi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.8.0/README.rst` & `thrift_pyi-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.8.0/pyproject.toml` & `thrift_pyi-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thrift-pyi"
-version = "0.8.0"
+version = "0.9.0"
 description = "This is simple `.pyi` stubs generator from thrift interfaces"
 readme = "README.rst"
 repository = "https://github.com/unmade/thrift-pyi"
 authors = ["Aleksei Maslakov <lesha.maslakov@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "thriftpyi", from = "src" },
```

### Comparing `thrift_pyi-0.8.0/src/thriftpyi/cli.py` & `thrift_pyi-0.9.0/src/thriftpyi/cli.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.8.0/src/thriftpyi/entities.py` & `thrift_pyi-0.9.0/src/thriftpyi/entities.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.8.0/src/thriftpyi/main.py` & `thrift_pyi-0.9.0/src/thriftpyi/main.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.8.0/src/thriftpyi/proxies.py` & `thrift_pyi-0.9.0/src/thriftpyi/proxies.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,20 +48,26 @@
 
     def has_structs(self) -> bool:
         return len(self.tmodule.__thrift_meta__["structs"]) > 0
 
     def has_enums(self) -> bool:
         return len(self.tmodule.__thrift_meta__["enums"]) > 0
 
-    @staticmethod
-    def _make_const(tconst) -> Field:
+    def _make_const(self, tconst) -> Field:
         name, value = tconst
         return Field(
             name=name,
-            type=guess_type(value),
+            type=guess_type(
+                value,
+                known_modules={
+                    module.__name__
+                    for module in self.tmodule.__thrift_meta__["includes"]
+                },
+                known_structs=self.tmodule.__thrift_meta__["structs"],
+            ),
             value=value,
             required=True,
         )
 
     @staticmethod
     def _make_enum(tenum) -> ModuleItem:
         fields = tenum._NAMES_TO_VALUES  # pylint: disable=protected-access
```

### Comparing `thrift_pyi-0.8.0/src/thriftpyi/stubs.py` & `thrift_pyi-0.9.0/src/thriftpyi/stubs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 def build(
     proxy: TModuleProxy, is_async: bool, strict_fields: bool, strict_methods: bool
 ) -> ast.Module:
     return ast.Module(
         body=[
             *_make_imports(proxy),
-            *_make_consts(proxy),
             *_make_exceptions(proxy, strict=strict_fields),
             *_make_enums(proxy),
             *_make_structs(proxy, strict=strict_fields),
+            *_make_consts(proxy),
             *_make_service(proxy, is_async, strict=strict_methods),
         ],
         type_ignores=[],
     )
 
 
 def build_init(imports: Iterable[str]) -> ast.Module:
```

### Comparing `thrift_pyi-0.8.0/PKG-INFO` & `thrift_pyi-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: thrift-pyi
-Version: 0.8.0
+Version: 0.9.0
 Summary: This is simple `.pyi` stubs generator from thrift interfaces
 Home-page: https://github.com/unmade/thrift-pyi
 License: MIT
 Author: Aleksei Maslakov
 Author-email: lesha.maslakov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: astunparse (>=1.6.3,<2.0.0) ; python_full_version < "3.9.0"
 Requires-Dist: autoflake
 Requires-Dist: black
 Requires-Dist: thriftpy2 (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/unmade/thrift-pyi
 Description-Content-Type: text/x-rst
```

