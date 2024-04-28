# Comparing `tmp/minijinja-1.0.8.tar.gz` & `tmp/minijinja-2.0.1.tar.gz`

## Comparing `minijinja-1.0.8.tar` & `minijinja-2.0.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 minijinja-1.0.8/local_dependencies/minijinja/Cargo.toml
--rw-r--r--   0     1001      127    10847 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/LICENSE
--rw-r--r--   0     1001      127     5439 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/README.md
--rw-r--r--   0     1001      127      598 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/doc-header.html
--rw-r--r--   0     1001      127    17406 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/ast.rs
--rw-r--r--   0     1001      127    31229 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/codegen.rs
--rw-r--r--   0     1001      127    12009 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/instructions.rs
--rw-r--r--   0     1001      127    24878 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/lexer.rs
--rw-r--r--   0     1001      127     9285 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/meta.rs
--rw-r--r--   0     1001      127      193 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/mod.rs
--rw-r--r--   0     1001      127    41209 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/parser.rs
--rw-r--r--   0     1001      127     4282 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/compiler/tokens.rs
--rw-r--r--   0     1001      127     4336 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/custom_syntax.rs
--rw-r--r--   0     1001      127     2777 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/debug.rs
--rw-r--r--   0     1001      127     8816 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/defaults.rs
--rw-r--r--   0     1001      127    26582 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/environment.rs
--rw-r--r--   0     1001      127    13157 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/error.rs
--rw-r--r--   0     1001      127     3152 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/expression.rs
--rw-r--r--   0     1001      127    43381 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/filters.rs
--rw-r--r--   0     1001      127    10204 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/functions.rs
--rw-r--r--   0     1001      127    10977 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/lib.rs
--rw-r--r--   0     1001      127     6774 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/loader.rs
--rw-r--r--   0     1001      127    10146 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/macros.rs
--rw-r--r--   0     1001      127     5073 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/output.rs
--rw-r--r--   0     1001      127    25393 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/syntax.rs
--rw-r--r--   0     1001      127    14087 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/template.rs
--rw-r--r--   0     1001      127    14232 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/tests.rs
--rw-r--r--   0     1001      127    12149 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/utils.rs
--rw-r--r--   0     1001      127    31462 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/argtypes.rs
--rw-r--r--   0     1001      127    14511 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/deserialize.rs
--rw-r--r--   0     1001      127     4129 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/keyref.rs
--rw-r--r--   0     1001      127     1121 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/merge_object.rs
--rw-r--r--   0     1001      127    52037 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/mod.rs
--rw-r--r--   0     1001      127    21927 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/object.rs
--rw-r--r--   0     1001      127    12260 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/ops.rs
--rw-r--r--   0     1001      127    11674 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/value/serialize.rs
--rw-r--r--   0     1001      127     1468 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/closure_object.rs
--rw-r--r--   0     1001      127    10451 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/context.rs
--rw-r--r--   0     1001      127     2236 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/fuel.rs
--rw-r--r--   0     1001      127     4433 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/loop_object.rs
--rw-r--r--   0     1001      127     5861 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/macro_object.rs
--rw-r--r--   0     1001      127    38397 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/mod.rs
--rw-r--r--   0     1001      127    13285 2023-09-17 10:43:20.000000 minijinja-1.0.8/local_dependencies/minijinja/src/vm/state.rs
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 minijinja-1.0.8/Cargo.toml
--rw-r--r--   0     1001      127       47 2023-09-17 10:43:20.000000 minijinja-1.0.8/.gitignore
--rw-r--r--   0     1001      127       45 2023-09-17 10:43:20.000000 minijinja-1.0.8/.vscode/settings.json
--rw-r--r--   0     1001      127    10847 2023-09-17 10:43:20.000000 minijinja-1.0.8/LICENSE
--rw-r--r--   0     1001      127      399 2023-09-17 10:43:20.000000 minijinja-1.0.8/Makefile
--rw-r--r--   0     1001      127     7495 2023-09-17 10:43:20.000000 minijinja-1.0.8/README.md
--rw-r--r--   0     1001      127      571 2023-09-17 10:43:20.000000 minijinja-1.0.8/hello.py
--rw-r--r--   0     1001      127     1145 2023-09-17 10:43:20.000000 minijinja-1.0.8/pyproject.toml
--rw-r--r--   0     1001      127     5016 2023-09-17 10:43:20.000000 minijinja-1.0.8/python/minijinja/__init__.py
--rw-r--r--   0     1001      127      558 2023-09-17 10:43:20.000000 minijinja-1.0.8/python/minijinja/_internal.py
--rw-r--r--   0     1001      127    21936 2023-09-17 10:43:20.000000 minijinja-1.0.8/src/environment.rs
--rw-r--r--   0     1001      127     2740 2023-09-17 10:43:20.000000 minijinja-1.0.8/src/error_support.rs
--rw-r--r--   0     1001      127      303 2023-09-17 10:43:20.000000 minijinja-1.0.8/src/lib.rs
--rw-r--r--   0     1001      127     2745 2023-09-17 10:43:20.000000 minijinja-1.0.8/src/state.rs
--rw-r--r--   0     1001      127    10976 2023-09-17 10:43:20.000000 minijinja-1.0.8/src/typeconv.rs
--rw-r--r--   0     1001      127     7618 2023-09-17 10:43:20.000000 minijinja-1.0.8/tests/test_basic.py
--rw-r--r--   0     1001      127      541 2023-09-17 10:43:20.000000 minijinja-1.0.8/tests/test_security.py
--rw-r--r--   0     1001      127     2304 2023-09-17 10:43:20.000000 minijinja-1.0.8/tests/test_state.py
--rw-r--r--   0     1001      127    88032 2023-09-17 10:43:25.000000 minijinja-1.0.8/Cargo.lock
--rw-r--r--   0        0        0     8497 1970-01-01 00:00:00.000000 minijinja-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1981 1970-01-01 00:00:00.000000 minijinja-2.0.1/local_dependencies/minijinja/Cargo.toml
+-rw-r--r--   0     1001      127    10847 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/LICENSE
+-rw-r--r--   0     1001      127     6124 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/README.md
+-rw-r--r--   0     1001      127      598 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/doc-header.html
+-rw-r--r--   0     1001      127    17325 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/ast.rs
+-rw-r--r--   0     1001      127    31626 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/codegen.rs
+-rw-r--r--   0     1001      127    12083 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/instructions.rs
+-rw-r--r--   0     1001      127    32488 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/lexer.rs
+-rw-r--r--   0     1001      127     9896 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/meta.rs
+-rw-r--r--   0     1001      127      193 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    41594 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/parser.rs
+-rw-r--r--   0     1001      127     4282 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/compiler/tokens.rs
+-rw-r--r--   0     1001      127     2777 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/debug.rs
+-rw-r--r--   0     1001      127     9359 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/defaults.rs
+-rw-r--r--   0     1001      127    33050 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/environment.rs
+-rw-r--r--   0     1001      127    13925 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/error.rs
+-rw-r--r--   0     1001      127     3865 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/expression.rs
+-rw-r--r--   0     1001      127    47333 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/filters.rs
+-rw-r--r--   0     1001      127    13875 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/functions.rs
+-rw-r--r--   0     1001      127    11711 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/lib.rs
+-rw-r--r--   0     1001      127     7409 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/loader.rs
+-rw-r--r--   0     1001      127    10011 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/macros.rs
+-rw-r--r--   0     1001      127     5115 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/output.rs
+-rw-r--r--   0     1001      127    40565 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/syntax.rs
+-rw-r--r--   0     1001      127    14899 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/template.rs
+-rw-r--r--   0     1001      127    15412 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/tests.rs
+-rw-r--r--   0     1001      127    12548 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/utils.rs
+-rw-r--r--   0     1001      127    32894 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/argtypes.rs
+-rw-r--r--   0     1001      127    14376 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/deserialize.rs
+-rw-r--r--   0     1001      127     1111 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/merge_object.rs
+-rw-r--r--   0     1001      127    57869 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/mod.rs
+-rw-r--r--   0     1001      127      994 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/namespace_object.rs
+-rw-r--r--   0     1001      127    29258 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/object.rs
+-rw-r--r--   0     1001      127    13313 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/ops.rs
+-rw-r--r--   0     1001      127    11237 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/serialize.rs
+-rw-r--r--   0     1001      127     1427 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/string_interning.rs
+-rw-r--r--   0     1001      127     5813 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/value/type_erase.rs
+-rw-r--r--   0     1001      127     2108 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/closure_object.rs
+-rw-r--r--   0     1001      127    10505 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/context.rs
+-rw-r--r--   0     1001      127     2236 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/fuel.rs
+-rw-r--r--   0     1001      127     4655 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/loop_object.rs
+-rw-r--r--   0     1001      127     5486 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/macro_object.rs
+-rw-r--r--   0     1001      127    40203 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/mod.rs
+-rw-r--r--   0     1001      127    13628 2024-04-28 18:38:51.000000 minijinja-2.0.1/local_dependencies/minijinja/src/vm/state.rs
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 minijinja-2.0.1/Cargo.toml
+-rw-r--r--   0     1001      127       47 2024-04-28 18:38:51.000000 minijinja-2.0.1/.gitignore
+-rw-r--r--   0     1001      127       45 2024-04-28 18:38:51.000000 minijinja-2.0.1/.vscode/settings.json
+-rw-r--r--   0     1001      127    10847 2024-04-28 18:38:51.000000 minijinja-2.0.1/LICENSE
+-rw-r--r--   0     1001      127      399 2024-04-28 18:38:51.000000 minijinja-2.0.1/Makefile
+-rw-r--r--   0     1001      127     7790 2024-04-28 18:38:51.000000 minijinja-2.0.1/README.md
+-rw-r--r--   0     1001      127      571 2024-04-28 18:38:51.000000 minijinja-2.0.1/hello.py
+-rw-r--r--   0     1001      127     1145 2024-04-28 18:38:51.000000 minijinja-2.0.1/pyproject.toml
+-rw-r--r--   0     1001      127     5380 2024-04-28 18:38:51.000000 minijinja-2.0.1/python/minijinja/__init__.py
+-rw-r--r--   0     1001      127      558 2024-04-28 18:38:51.000000 minijinja-2.0.1/python/minijinja/_internal.py
+-rw-r--r--   0     1001      127    25007 2024-04-28 18:38:51.000000 minijinja-2.0.1/src/environment.rs
+-rw-r--r--   0     1001      127     2773 2024-04-28 18:38:51.000000 minijinja-2.0.1/src/error_support.rs
+-rw-r--r--   0     1001      127      314 2024-04-28 18:38:51.000000 minijinja-2.0.1/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-28 18:38:51.000000 minijinja-2.0.1/src/state.rs
+-rw-r--r--   0     1001      127     9970 2024-04-28 18:38:51.000000 minijinja-2.0.1/src/typeconv.rs
+-rw-r--r--   0     1001      127     9649 2024-04-28 18:38:51.000000 minijinja-2.0.1/tests/test_basic.py
+-rw-r--r--   0     1001      127      541 2024-04-28 18:38:51.000000 minijinja-2.0.1/tests/test_security.py
+-rw-r--r--   0     1001      127     2304 2024-04-28 18:38:51.000000 minijinja-2.0.1/tests/test_state.py
+-rw-r--r--   0     1001      127    91884 2024-04-28 18:38:51.000000 minijinja-2.0.1/Cargo.lock
+-rw-r--r--   0        0        0     8792 1970-01-01 00:00:00.000000 minijinja-2.0.1/PKG-INFO
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/Cargo.toml` & `minijinja-2.0.1/local_dependencies/minijinja/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "minijinja"
-version = "1.0.8"
+version = "2.0.1"
 edition = "2021"
 license = "Apache-2.0"
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 description = "a powerful template engine for Rust with minimal dependencies"
 homepage = "https://github.com/mitsuhiko/minijinja"
 repository = "https://github.com/mitsuhiko/minijinja"
 keywords = ["jinja", "jinja2", "templates"]
@@ -21,23 +21,25 @@
 default = [
     "builtins",
     "debug",
     "deserialization",
     "macros",
     "multi_template",
     "adjacent_loop_items",
+    "std_collections",
 ]
 
 # API features
 preserve_order = ["indexmap"]
 deserialization = []
 debug = []
 loader = ["self_cell", "memo-map"]
 unicode = ["unicode-ident", "unicase"]
 custom_syntax = ["dep:aho-corasick"]
+std_collections = []
 
 # Speedups
 key_interning = []
 speedups = ["v_htmlescape"]
 
 # Engine Features
 builtins = []
@@ -62,7 +64,8 @@
 self_cell = { version = "1.0.0", optional = true }
 serde_json = { version = "1.0.68", optional = true }
 percent-encoding = { version = "2.2.0", optional = true }
 indexmap = { version = "1.9.0", optional = true }
 memo-map = { version = "0.3.1", optional = true }
 unicode-ident = { version = "1.0.5", optional = true }
 unicase = { version = "2.6.0", optional = true }
+stacker = { version = "0.1.15", optional = true }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/LICENSE` & `minijinja-2.0.1/local_dependencies/minijinja/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/README.md` & `minijinja-2.0.1/local_dependencies/minijinja/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dependencies for a small problem.  Additionally it tries not to re-invent
 something but stay in line with prior art to leverage an already existing
 ecosystem of editor integrations.
 
 ```
 $ cargo tree
 minimal v0.1.0 (examples/minimal)
-└── minijinja v1.0.8 (minijinja)
+└── minijinja v2.0.1 (minijinja)
     └── serde v1.0.144
 ```
 
 You can play with MiniJinja online [in the browser playground](https://mitsuhiko.github.io/minijinja-playground/)
 powered by a WASM build of MiniJinja.
 
 **Goals:**
@@ -70,24 +70,35 @@
 ```
 
 ## Getting Help
 
 If you are stuck with `MiniJinja`, have suggestions or need help, you can use the
 [GitHub Discussions](https://github.com/mitsuhiko/minijinja/discussions).
 
+## Upgrading from MiniJinja 1.x
+
+There are two major versions of MiniJinja both of which are currently maintained.  Most users should
+upgrade to 2.x which has a much improved object system.  However if you have been using dynamic
+objects in the past the upgrade might be quite involved.  For upgrade informations refer to
+[UPDATING](UPDATING.md) which has a guide with examples of what the changes between the two engine
+versions are.
+
+To see examples and code from MiniJinja 1.x, you can browse the [minijinja-1.x branch](https://github.com/mitsuhiko/minijinja/tree/minijinja-1.x).
+
 ## Related Crates
 
 * [minijinja-autoreload](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-autoreload): provides
   auto reloading functionality of environments
+* [minijinja-embed](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-embed): provides
+  utilities for embedding templates in a binary
 * [minijinja-contrib](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-contrib): provides
   additional utilities too specific for the core
-* [minijinja-stack-ref](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-stack-ref): provides
-  functionality to pass values from the stack
 * [minijinja-py](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-py): makes MiniJinja
   available to Python
+* [minijinja-cli](https://github.com/mitsuhiko/minijinja/tree/main/minijinja-cli): a command line utility.
 
 ## Similar Projects
 
 These are related template engines for Rust:
 
 * [Askama](https://crates.io/crates/askama): Jinja inspired, type-safe, requires template
   precompilation. Has significant divergence from Jinja syntax in parts.
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/doc-header.html` & `minijinja-2.0.1/local_dependencies/minijinja/doc-header.html`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/ast.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/ast.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::ops::Deref;
 
 #[cfg(feature = "internal_debug")]
 use std::fmt;
 
 use crate::compiler::tokens::Span;
-use crate::value::{value_map_with_capacity, KeyRef, MapType, Value, ValueRepr};
+use crate::value::{value_map_with_capacity, Value};
 
 /// Container for nodes with location info.
 ///
 /// This container fulfills two purposes: it adds location information
 /// to nodes, but it also ensures the nodes is heap allocated.  The
 /// latter is useful to ensure that enum variants do not cause the enum
 /// to become too large.
@@ -475,15 +475,15 @@
 
         let items = self.items.iter();
         let sequence = items.filter_map(|expr| match expr {
             Expr::Const(v) => Some(v.value.clone()),
             _ => None,
         });
 
-        Some(sequence.collect())
+        Some(Value::from(sequence.collect::<Vec<_>>()))
     }
 }
 
 /// Creates a map of kwargs
 #[cfg_attr(feature = "internal_debug", derive(Debug))]
 #[cfg_attr(feature = "unstable_machinery_serde", derive(serde::Serialize))]
 pub struct Kwargs<'a> {
@@ -495,19 +495,19 @@
         if !self.pairs.iter().all(|x| matches!(x.1, Expr::Const(_))) {
             return None;
         }
 
         let mut rv = value_map_with_capacity(self.pairs.len());
         for (key, value) in &self.pairs {
             if let Expr::Const(value) = value {
-                rv.insert(KeyRef::Value(Value::from(*key)), value.value.clone());
+                rv.insert(Value::from(*key), value.value.clone());
             }
         }
 
-        Some(Value(ValueRepr::Map(rv.into(), MapType::Kwargs)))
+        Some(crate::value::Kwargs::wrap(rv))
     }
 }
 
 /// Creates a map of values.
 #[cfg_attr(feature = "internal_debug", derive(Debug))]
 #[cfg_attr(feature = "unstable_machinery_serde", derive(serde::Serialize))]
 pub struct Map<'a> {
@@ -522,19 +522,19 @@
         {
             return None;
         }
 
         let mut rv = value_map_with_capacity(self.keys.len());
         for (key, value) in self.keys.iter().zip(self.values.iter()) {
             if let (Expr::Const(maybe_key), Expr::Const(value)) = (key, value) {
-                rv.insert(KeyRef::Value(maybe_key.value.clone()), value.value.clone());
+                rv.insert(maybe_key.value.clone(), value.value.clone());
             }
         }
 
-        Some(Value(ValueRepr::Map(rv.into(), MapType::Normal)))
+        Some(Value::from_object(rv))
     }
 }
 
 /// Defines the specific type of call.
 #[cfg_attr(feature = "internal_debug", derive(Debug))]
 #[cfg_attr(feature = "unstable_machinery_serde", derive(serde::Serialize))]
 pub enum CallType<'ast, 'source> {
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/codegen.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/codegen.rs`

 * *Files 1% similar despite different names*

```diff
@@ -175,33 +175,33 @@
     }
 
     /// Closes the current if block.
     pub fn end_if(&mut self) {
         self.end_condition(self.next_instruction());
     }
 
-    /// Starts a short cirquited bool block.
+    /// Starts a short-circuited bool block.
     pub fn start_sc_bool(&mut self) {
         self.pending_block.push(PendingBlock::ScBool(vec![]));
     }
 
-    /// Emits a short circuited bool operator.
+    /// Emits a short-circuited bool operator.
     pub fn sc_bool(&mut self, and: bool) {
         if let Some(PendingBlock::ScBool(ref mut instructions)) = self.pending_block.last_mut() {
             instructions.push(self.instructions.add(if and {
                 Instruction::JumpIfFalseOrPop(!0)
             } else {
                 Instruction::JumpIfTrueOrPop(!0)
             }));
         } else {
             unreachable!();
         }
     }
 
-    /// Ends a short circuited bool block.
+    /// Ends a short-circuited bool block.
     pub fn end_sc_bool(&mut self) {
         let end = self.next_instruction();
         if let Some(PendingBlock::ScBool(instructions)) = self.pending_block.pop() {
             for instr in instructions {
                 match self.instructions.get_mut(instr) {
                     Some(Instruction::JumpIfFalseOrPop(ref mut target))
                     | Some(Instruction::JumpIfTrueOrPop(ref mut target)) => {
@@ -364,15 +364,14 @@
         self.blocks.insert(block.name, instructions);
         self.add(Instruction::CallBlock(block.name));
     }
 
     #[cfg(feature = "macros")]
     fn compile_macro_expression(&mut self, macro_decl: &ast::Spanned<ast::Macro<'source>>) {
         use crate::compiler::instructions::MACRO_CALLER;
-        use crate::value::ValueRepr;
         self.set_line_from_span(macro_decl.span());
         let instr = self.add(Instruction::Jump(!0));
         let mut defaults_iter = macro_decl.defaults.iter().rev();
         for arg in macro_decl.args.iter().rev() {
             if let Some(default) = defaults_iter.next() {
                 self.add(Instruction::DupTop);
                 self.add(Instruction::IsUndefined);
@@ -390,25 +389,24 @@
         let mut undeclared = crate::compiler::meta::find_macro_closure(macro_decl);
         let caller_reference = undeclared.remove("caller");
         let macro_instr = self.next_instruction();
         for name in &undeclared {
             self.add(Instruction::Enclose(name));
         }
         self.add(Instruction::GetClosure);
-        self.add(Instruction::LoadConst(Value::from(ValueRepr::Seq(
+        self.add(Instruction::LoadConst(Value::from_object(
             macro_decl
                 .args
                 .iter()
                 .map(|x| match x {
                     ast::Expr::Var(var) => Value::from(var.id),
                     _ => unreachable!(),
                 })
-                .collect::<Vec<_>>()
-                .into(),
-        ))));
+                .collect::<Vec<Value>>(),
+        )));
         let mut flags = 0;
         if caller_reference {
             flags |= MACRO_CALLER;
         }
         self.add(Instruction::BuildMacro(macro_decl.name, instr + 1, flags));
         if let Some(Instruction::Jump(ref mut target)) = self.instructions.get_mut(instr) {
             *target = macro_instr;
@@ -473,33 +471,39 @@
         }
         self.compile_expr(&expr.expr);
         self.add(Instruction::Emit);
     }
 
     fn compile_for_loop(&mut self, for_loop: &ast::Spanned<ast::ForLoop<'source>>) {
         self.set_line_from_span(for_loop.span());
+
+        // filter expressions work like a nested for loop without
+        // the special loop variable. in one loop, the condition is checked and
+        // passing items accumlated into a list. in the second, that list is
+        // iterated over normally
         if let Some(ref filter_expr) = for_loop.filter_expr {
-            // filter expressions work like a nested for loop without
-            // the special loop variable that append into a new list
-            // just outside of the loop.
-            self.add(Instruction::BuildList(0));
+            self.add(Instruction::LoadConst(Value::from(0usize)));
             self.compile_expr(&for_loop.iter);
             self.start_for_loop(false, false);
             self.add(Instruction::DupTop);
             self.compile_assignment(&for_loop.target);
             self.compile_expr(filter_expr);
             self.start_if();
-            self.add(Instruction::ListAppend);
+            self.add(Instruction::Swap);
+            self.add(Instruction::LoadConst(Value::from(1usize)));
+            self.add(Instruction::Add);
             self.start_else();
             self.add(Instruction::DiscardTop);
             self.end_if();
             self.end_for_loop(false);
+            self.add(Instruction::BuildList(None));
         } else {
             self.compile_expr(&for_loop.iter);
         }
+
         self.start_for_loop(true, for_loop.recursive);
         self.compile_assignment(&for_loop.target);
         for node in &for_loop.body {
             self.compile_stmt(node);
         }
         self.end_for_loop(!for_loop.else_body.is_empty());
         if !for_loop.else_body.is_empty() {
@@ -521,14 +525,19 @@
                 self.push_span(list.span());
                 self.add(Instruction::UnpackList(list.items.len()));
                 for expr in &list.items {
                     self.compile_assignment(expr);
                 }
                 self.pop_span();
             }
+            ast::Expr::GetAttr(attr) => {
+                self.push_span(attr.span());
+                self.compile_expr(&attr.expr);
+                self.add(Instruction::SetAttr(attr.name));
+            }
             _ => unreachable!(),
         }
     }
 
     /// Compiles an expression.
     pub fn compile_expr(&mut self, expr: &ast::Expr<'source>) {
         match expr {
@@ -641,15 +650,15 @@
                 if let Some(val) = l.as_const() {
                     self.add(Instruction::LoadConst(val));
                 } else {
                     self.set_line_from_span(l.span());
                     for item in &l.items {
                         self.compile_expr(item);
                     }
-                    self.add(Instruction::BuildList(l.items.len()));
+                    self.add(Instruction::BuildList(Some(l.items.len())));
                 }
             }
             ast::Expr::Map(m) => {
                 if let Some(val) = m.as_const() {
                     self.add(Instruction::LoadConst(val));
                 } else {
                     self.set_line_from_span(m.span());
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/instructions.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/instructions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
     /// Load a variable,
     Lookup(&'source str),
 
     /// Looks up an attribute.
     GetAttr(&'source str),
 
+    /// Sets an attribute.
+    SetAttr(&'source str),
+
     /// Looks up an item.
     GetItem,
 
     /// Performs a slice operation.
     Slice,
 
     /// Loads a constant value.
@@ -54,22 +57,19 @@
     /// Builds a map of the last n pairs on the stack.
     BuildMap(usize),
 
     /// Builds a kwargs map of the last n pairs on the stack.
     BuildKwargs(usize),
 
     /// Builds a list of the last n pairs on the stack.
-    BuildList(usize),
+    BuildList(Option<usize>),
 
     /// Unpacks a list into N stack items.
     UnpackList(usize),
 
-    /// Appends to the list.
-    ListAppend,
-
     /// Add the top two values
     Add,
 
     /// Subtract the top two values
     Sub,
 
     /// Multiply the top two values
@@ -191,14 +191,17 @@
 
     /// A fast super instruction without intermediate capturing.
     FastSuper,
 
     /// A fast loop recurse instruction without intermediate capturing.
     FastRecurse,
 
+    /// Swaps the top two items in the stack.
+    Swap,
+
     /// Call into a block.
     #[cfg(feature = "multi_template")]
     CallBlock(&'source str),
 
     /// Loads block from a template with name on stack ("extends")
     #[cfg(feature = "multi_template")]
     LoadBlocks,
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/lexer.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/lexer.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,173 @@
+use std::borrow::Cow;
+use std::ops::ControlFlow;
+
 use crate::compiler::tokens::{Span, Token};
 use crate::error::{Error, ErrorKind};
+use crate::syntax::SyntaxConfig;
 use crate::utils::{memchr, memstr, unescape};
 
-#[cfg(feature = "custom_syntax")]
-pub use crate::custom_syntax::SyntaxConfig;
+/// Internal config struct to control whitespace in the engine.
+#[derive(Copy, Clone, Debug, Default)]
+pub struct WhitespaceConfig {
+    pub keep_trailing_newline: bool,
+    pub lstrip_blocks: bool,
+    pub trim_blocks: bool,
+}
 
-/// Non configurable syntax config
-#[cfg(not(feature = "custom_syntax"))]
-#[derive(Debug, Clone, Default)]
-pub struct SyntaxConfig;
+/// Tokenizes jinja templates.
+pub struct Tokenizer<'s> {
+    stack: Vec<LexerState>,
+    source: &'s str,
+    current_line: u32,
+    current_col: u32,
+    current_offset: usize,
+    trim_leading_whitespace: bool,
+    pending_start_marker: Option<(StartMarker, usize)>,
+    #[cfg(feature = "custom_syntax")]
+    paren_balance: isize,
+    syntax_config: SyntaxConfig,
+    ws_config: WhitespaceConfig,
+}
 
 enum LexerState {
     Template,
-    InVariable,
-    InBlock,
+    Variable,
+    Block,
+    #[cfg(feature = "custom_syntax")]
+    LineStatement,
 }
 
 /// Utility enum that defines a marker.
-#[derive(Debug, Copy, Clone)]
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum StartMarker {
     Variable,
     Block,
     Comment,
+    #[cfg(feature = "custom_syntax")]
+    LineStatement,
+    #[cfg(feature = "custom_syntax")]
+    LineComment,
 }
 
-struct TokenizerState<'s> {
-    stack: Vec<LexerState>,
-    rest: &'s str,
-    failed: bool,
-    current_line: u32,
-    current_col: u32,
-    current_offset: u32,
+/// What ends this block tokenization?
+#[derive(Debug, Copy, Clone)]
+enum BlockSentinel {
+    Variable,
+    Block,
+    #[cfg(feature = "custom_syntax")]
+    LineStatement,
 }
 
-fn find_start_marker_memchr(a: &str) -> Option<(usize, bool)> {
+#[derive(Copy, Clone, Debug, Eq, PartialEq)]
+enum Whitespace {
+    Default,
+    Preserve,
+    Remove,
+}
+
+impl Whitespace {
+    fn from_byte(b: Option<u8>) -> Whitespace {
+        match b {
+            Some(b'-') => Whitespace::Remove,
+            Some(b'+') => Whitespace::Preserve,
+            _ => Whitespace::Default,
+        }
+    }
+
+    fn len(&self) -> usize {
+        match self {
+            Whitespace::Default => 0,
+            Whitespace::Preserve | Whitespace::Remove => 1,
+        }
+    }
+}
+
+fn find_start_marker_memchr(a: &str) -> Option<(usize, StartMarker, usize, Whitespace)> {
     let bytes = a.as_bytes();
     let mut offset = 0;
     loop {
         let idx = match memchr(&bytes[offset..], b'{') {
             Some(idx) => idx,
             None => return None,
         };
-        if let Some(b'{' | b'%' | b'#') = bytes.get(offset + idx + 1).copied() {
-            return Some((
-                offset + idx,
-                bytes.get(offset + idx + 2).copied() == Some(b'-'),
-            ));
-        }
-        offset += idx + 1;
+        let marker = match bytes.get(offset + idx + 1).copied() {
+            Some(b'{') => StartMarker::Variable,
+            Some(b'%') => StartMarker::Block,
+            Some(b'#') => StartMarker::Comment,
+            _ => {
+                offset += idx + 1;
+                continue;
+            }
+        };
+        let ws = Whitespace::from_byte(bytes.get(offset + idx + 2).copied());
+        return Some((offset + idx, marker, 2 + ws.len(), ws));
     }
 }
 
 #[cfg(feature = "custom_syntax")]
-fn find_start_marker(a: &str, syntax_config: &SyntaxConfig) -> Option<(usize, bool)> {
+fn find_start_marker(
+    a: &str,
+    offset: usize,
+    syntax_config: &SyntaxConfig,
+) -> Option<(usize, StartMarker, usize, Whitespace)> {
     // If we have a custom delimiter we need to use the aho-corasick
     // otherwise we can use internal memchr.
-    match syntax_config.aho_corasick {
-        Some(ref ac) => {
-            let bytes = a.as_bytes();
-            ac.find(bytes).map(|m| {
-                (
-                    m.start(),
-                    bytes.get(m.start() + m.len()).copied() == Some(b'-'),
-                )
-            })
-        }
-        None => find_start_marker_memchr(a),
-    }
-}
-
-#[cfg(not(feature = "custom_syntax"))]
-fn find_start_marker(a: &str, _syntax_config: &SyntaxConfig) -> Option<(usize, bool)> {
-    find_start_marker_memchr(a)
-}
+    let ac = match syntax_config.aho_corasick {
+        Some(ref ac) => ac,
+        None => return find_start_marker_memchr(&a[offset..]),
+    };
 
-fn match_start_marker(rest: &str, syntax_config: &SyntaxConfig) -> Option<(StartMarker, usize)> {
-    #[cfg(not(feature = "custom_syntax"))]
-    {
-        let _ = syntax_config;
-        match_start_marker_default(rest)
-    }
+    let bytes = &a.as_bytes()[offset..];
+    let mut state = aho_corasick::automaton::OverlappingState::start();
+    let mut longest_match = None::<(usize, StartMarker, usize, Whitespace)>;
 
-    #[cfg(feature = "custom_syntax")]
-    {
-        if syntax_config.aho_corasick.is_none() {
-            return match_start_marker_default(rest);
-        }
+    loop {
+        ac.find_overlapping(bytes, &mut state);
+        let m = match state.get_match() {
+            None => break,
+            Some(m) => m,
+        };
 
-        for delimiter in syntax_config.start_delimiters_order {
-            let marker = match delimiter {
-                StartMarker::Variable => &syntax_config.syntax.variable_start as &str,
-                StartMarker::Block => &syntax_config.syntax.block_start as &str,
-                StartMarker::Comment => &syntax_config.syntax.comment_start as &str,
-            };
-            if rest.get(..marker.len()) == Some(marker) {
-                return Some((delimiter, marker.len()));
+        let marker = syntax_config.pattern_to_marker(m.pattern());
+        let ws = if matches!(marker, StartMarker::LineStatement) {
+            let prefix = &a.as_bytes()[..offset + m.start()];
+            if matches!(
+                prefix
+                    .iter()
+                    .copied()
+                    .rev()
+                    .find(|&x| x != b' ' && x != b'\t'),
+                None | Some(b'\r') | Some(b'\n')
+            ) {
+                Whitespace::Default
+            } else {
+                continue;
             }
-        }
+        } else {
+            Whitespace::from_byte(bytes.get(m.start() + m.len()).copied())
+        };
+        let new_match = (m.start(), marker, m.len() + ws.len(), ws);
 
-        None
+        if longest_match.as_ref().map_or(false, |x| new_match.0 > x.0) {
+            break;
+        }
+        longest_match = Some(new_match);
     }
+
+    longest_match
 }
 
-fn match_start_marker_default(rest: &str) -> Option<(StartMarker, usize)> {
-    match rest.get(..2) {
-        Some("{{") => Some((StartMarker::Variable, 2)),
-        Some("{%") => Some((StartMarker::Block, 2)),
-        Some("{#") => Some((StartMarker::Comment, 2)),
-        _ => None,
-    }
+#[cfg(not(feature = "custom_syntax"))]
+fn find_start_marker(
+    a: &str,
+    offset: usize,
+    _syntax_config: &SyntaxConfig,
+) -> Option<(usize, StartMarker, usize, Whitespace)> {
+    find_start_marker_memchr(&a[offset..])
 }
 
 #[cfg(feature = "unicode")]
 fn lex_identifier(s: &str) -> usize {
     s.chars()
         .enumerate()
         .map_while(|(idx, c)| {
@@ -141,149 +196,306 @@
             } else {
                 c.is_ascii_alphanumeric()
             }
         })
         .count()
 }
 
-fn skip_basic_tag(block_str: &str, name: &str, block_end: &str) -> Option<(usize, bool)> {
+fn is_nl(c: char) -> bool {
+    c == '\r' || c == '\n'
+}
+
+#[cfg(feature = "custom_syntax")]
+fn skip_nl(mut rest: &str) -> (bool, usize) {
+    let mut skip = 0;
+    let mut was_nl = false;
+    if let Some(new_rest) = rest.strip_prefix('\n') {
+        rest = new_rest;
+        skip += 1;
+        was_nl = true;
+    }
+    if let Some(new_rest) = rest.strip_prefix('\r') {
+        rest = new_rest;
+        skip += 1;
+        was_nl = true;
+    }
+    (was_nl || rest.is_empty(), skip)
+}
+
+fn lstrip_block(s: &str) -> &str {
+    let trimmed = s.trim_end_matches(|x: char| x.is_whitespace() && !is_nl(x));
+    if trimmed.is_empty() || trimmed.as_bytes().get(trimmed.len() - 1) == Some(&b'\n') {
+        trimmed
+    } else {
+        s
+    }
+}
+
+fn should_lstrip_block(flag: bool, marker: StartMarker) -> bool {
+    if flag && !matches!(marker, StartMarker::Variable) {
+        return true;
+    }
+    #[cfg(feature = "custom_syntax")]
+    {
+        if matches!(
+            marker,
+            StartMarker::LineStatement | StartMarker::LineComment
+        ) {
+            return true;
+        }
+    }
+    false
+}
+
+fn skip_basic_tag(
+    block_str: &str,
+    name: &str,
+    block_end: &str,
+    skip_ws_control: bool,
+) -> Option<(usize, Whitespace)> {
     let mut ptr = block_str;
-    let mut trim = false;
 
-    if let Some(rest) = ptr.strip_prefix('-') {
-        ptr = rest;
+    if skip_ws_control {
+        if let Some(rest) = ptr.strip_prefix(['-', '+']) {
+            ptr = rest;
+        }
     }
     while let Some(rest) = ptr.strip_prefix(|x: char| x.is_ascii_whitespace()) {
         ptr = rest;
     }
 
-    ptr = match ptr.strip_prefix(name) {
-        Some(ptr) => ptr,
-        None => return None,
-    };
+    ptr = some!(ptr.strip_prefix(name));
 
     while let Some(rest) = ptr.strip_prefix(|x: char| x.is_ascii_whitespace()) {
         ptr = rest;
     }
-    if let Some(rest) = ptr.strip_prefix('-') {
+
+    let ws = if let Some(rest) = ptr.strip_prefix('-') {
         ptr = rest;
-        trim = true;
-    }
-    ptr = match ptr.strip_prefix(block_end) {
-        Some(ptr) => ptr,
-        None => return None,
+        Whitespace::Remove
+    } else if let Some(rest) = ptr.strip_prefix('+') {
+        ptr = rest;
+        Whitespace::Preserve
+    } else {
+        Whitespace::Default
     };
 
-    Some((block_str.len() - ptr.len(), trim))
+    ptr.strip_prefix(block_end)
+        .map(|ptr| (block_str.len() - ptr.len(), ws))
 }
 
-impl<'s> TokenizerState<'s> {
+impl<'s> Tokenizer<'s> {
+    /// Creates a new tokenizer.
+    pub fn new(
+        input: &'s str,
+        in_expr: bool,
+        syntax_config: SyntaxConfig,
+        whitespace_config: WhitespaceConfig,
+    ) -> Tokenizer<'s> {
+        let mut source = input;
+        if !whitespace_config.keep_trailing_newline {
+            if source.ends_with('\n') {
+                source = &source[..source.len() - 1];
+            }
+            if source.ends_with('\r') {
+                source = &source[..source.len() - 1];
+            }
+        }
+        Tokenizer {
+            source,
+            stack: vec![if in_expr {
+                LexerState::Variable
+            } else {
+                LexerState::Template
+            }],
+            current_line: 1,
+            current_col: 0,
+            current_offset: 0,
+            #[cfg(feature = "custom_syntax")]
+            paren_balance: 0,
+            trim_leading_whitespace: false,
+            pending_start_marker: None,
+            syntax_config,
+            ws_config: whitespace_config,
+        }
+    }
+
+    /// Produces the next token from the tokenizer.
+    pub fn next_token(&mut self) -> Result<Option<(Token<'s>, Span)>, Error> {
+        loop {
+            if self.rest_bytes().is_empty() {
+                // line statements normally close with newlines.  At the end of the file
+                // however we need to use the stack to close out the block instead.
+                #[cfg(feature = "custom_syntax")]
+                {
+                    if matches!(self.stack.pop(), Some(LexerState::LineStatement)) {
+                        return Ok(Some((Token::BlockEnd, self.span(self.loc()))));
+                    }
+                }
+                return Ok(None);
+            }
+            let outcome = match self.stack.last() {
+                Some(LexerState::Template) => self.tokenize_root(),
+                Some(LexerState::Block) => self.tokenize_block_or_var(BlockSentinel::Block),
+                #[cfg(feature = "custom_syntax")]
+                Some(LexerState::LineStatement) => {
+                    self.tokenize_block_or_var(BlockSentinel::LineStatement)
+                }
+                Some(LexerState::Variable) => self.tokenize_block_or_var(BlockSentinel::Variable),
+                None => panic!("empty lexer stack"),
+            };
+            match ok!(outcome) {
+                ControlFlow::Break(rv) => return Ok(Some(rv)),
+                ControlFlow::Continue(()) => continue,
+            }
+        }
+    }
+
+    #[inline]
+    fn rest(&self) -> &'s str {
+        &self.source[self.current_offset..]
+    }
+
+    #[inline]
+    fn rest_bytes(&self) -> &'s [u8] {
+        &self.source.as_bytes()[self.current_offset..]
+    }
+
     fn advance(&mut self, bytes: usize) -> &'s str {
-        let (skipped, new_rest) = self.rest.split_at(bytes);
+        let skipped = &self.rest()[..bytes];
         for c in skipped.chars() {
             match c {
                 '\n' => {
                     self.current_line += 1;
                     self.current_col = 0;
                 }
                 _ => self.current_col += 1,
             }
         }
-        self.current_offset += bytes as u32;
-        self.rest = new_rest;
+        self.current_offset += bytes;
         skipped
     }
 
-    #[inline(always)]
+    #[inline]
     fn loc(&self) -> (u32, u32, u32) {
-        (self.current_line, self.current_col, self.current_offset)
+        (
+            self.current_line,
+            self.current_col,
+            self.current_offset as u32,
+        )
     }
 
-    fn span(&self, start: (u32, u32, u32)) -> Span {
-        let (start_line, start_col, start_offset) = start;
+    #[inline]
+    fn span(&self, (start_line, start_col, start_offset): (u32, u32, u32)) -> Span {
         Span {
             start_line,
             start_col,
             start_offset,
             end_line: self.current_line,
             end_col: self.current_col,
-            end_offset: self.current_offset,
+            end_offset: self.current_offset as u32,
         }
     }
 
+    #[inline]
     fn syntax_error(&mut self, msg: &'static str) -> Error {
-        self.failed = true;
         Error::new(ErrorKind::SyntaxError, msg)
     }
 
     fn eat_number(&mut self) -> Result<(Token<'s>, Span), Error> {
         #[derive(Copy, Clone)]
         enum State {
+            RadixInteger, // 0x10
             Integer,      // 123
             Fraction,     // .123
             Exponent,     // E | e
             ExponentSign, // +|-
         }
 
         let old_loc = self.loc();
-        let mut state = State::Integer;
+
+        let radix = match self.rest_bytes().get(..2) {
+            Some(b"0b" | b"0B") => 2,
+            Some(b"0o" | b"0O") => 8,
+            Some(b"0x" | b"0X") => 16,
+            _ => 10,
+        };
+
+        let mut state = if radix == 10 {
+            State::Integer
+        } else {
+            self.advance(2);
+            State::RadixInteger
+        };
+
         let mut num_len = self
-            .rest
-            .as_bytes()
+            .rest_bytes()
             .iter()
             .take_while(|&c| c.is_ascii_digit())
             .count();
-        for c in self.rest.as_bytes()[num_len..].iter().copied() {
+        let mut has_underscore = false;
+        for c in self.rest_bytes()[num_len..].iter().copied() {
             state = match (c, state) {
                 (b'.', State::Integer) => State::Fraction,
                 (b'E' | b'e', State::Integer | State::Fraction) => State::Exponent,
                 (b'+' | b'-', State::Exponent) => State::ExponentSign,
                 (b'0'..=b'9', State::Exponent) => State::ExponentSign,
                 (b'0'..=b'9', state) => state,
+                (b'a'..=b'f' | b'A'..=b'F', State::RadixInteger) if radix == 16 => state,
+                (b'_', _) => {
+                    has_underscore = true;
+                    state
+                }
                 _ => break,
             };
             num_len += 1;
         }
-        let is_float = !matches!(state, State::Integer);
+        let is_float = !matches!(state, State::Integer | State::RadixInteger);
+
+        let mut num = Cow::Borrowed(self.advance(num_len));
+        if has_underscore {
+            if num.ends_with('_') {
+                return Err(self.syntax_error("'_' may not occur at end of number"));
+            }
+            num = Cow::Owned(num.replace('_', ""));
+        }
 
-        let num = self.advance(num_len);
         Ok((
             ok!(if is_float {
                 num.parse()
                     .map(Token::Float)
                     .map_err(|_| self.syntax_error("invalid float"))
-            } else if let Ok(int) = num.parse() {
+            } else if let Ok(int) = u64::from_str_radix(&num, radix) {
                 Ok(Token::Int(int))
             } else {
-                num.parse()
+                u128::from_str_radix(&num, radix)
                     .map(Token::Int128)
                     .map_err(|_| self.syntax_error("invalid integer"))
             }),
             self.span(old_loc),
         ))
     }
 
     fn eat_identifier(&mut self) -> Result<(Token<'s>, Span), Error> {
-        let ident_len = lex_identifier(self.rest);
+        let ident_len = lex_identifier(self.rest());
         if ident_len > 0 {
             let old_loc = self.loc();
             let ident = self.advance(ident_len);
             Ok((Token::Ident(ident), self.span(old_loc)))
         } else {
             Err(self.syntax_error("unexpected character"))
         }
     }
 
     fn eat_string(&mut self, delim: u8) -> Result<(Token<'s>, Span), Error> {
         let old_loc = self.loc();
         let mut escaped = false;
         let mut has_escapes = false;
         let str_len = self
-            .rest
-            .as_bytes()
+            .rest_bytes()
             .iter()
             .skip(1)
             .take_while(|&&c| match (escaped, c) {
                 (true, _) => {
                     escaped = false;
                     true
                 }
@@ -292,15 +504,15 @@
                     has_escapes = true;
                     true
                 }
                 (_, c) if c == delim => false,
                 _ => true,
             })
             .count();
-        if escaped || self.rest.as_bytes().get(str_len + 1) != Some(&delim) {
+        if escaped || self.rest_bytes().get(str_len + 1) != Some(&delim) {
             return Err(self.syntax_error("unexpected end of string"));
         }
         let s = self.advance(str_len + 2);
         Ok(if has_escapes {
             (
                 Token::String(match unescape(&s[1..s.len() - 1]) {
                     Ok(unescaped) => unescaped,
@@ -310,345 +522,428 @@
             )
         } else {
             (Token::Str(&s[1..s.len() - 1]), self.span(old_loc))
         })
     }
 
     fn skip_whitespace(&mut self) {
-        let skip = self
-            .rest
+        let skipped = self
+            .rest()
             .chars()
             .map_while(|c| c.is_whitespace().then(|| c.len_utf8()))
-            .sum::<usize>();
-        if skip > 0 {
-            self.advance(skip);
+            .sum();
+        if skipped > 0 {
+            self.advance(skipped);
         }
     }
-}
 
-/// Tokenizes the source.
-pub fn tokenize(
-    input: &str,
-    in_expr: bool,
-    syntax_config: SyntaxConfig,
-) -> impl Iterator<Item = Result<(Token<'_>, Span), Error>> {
-    let mut state = TokenizerState {
-        rest: input,
-        stack: vec![if in_expr {
-            LexerState::InVariable
-        } else {
-            LexerState::Template
-        }],
-        failed: false,
-        current_line: 1,
-        current_col: 0,
-        current_offset: 0,
-    };
-    let mut trim_leading_whitespace = false;
-
-    std::iter::from_fn(move || {
-        let (variable_end, block_start, block_end, comment_end) = {
-            #[cfg(feature = "custom_syntax")]
-            {
-                (
-                    &syntax_config.syntax.variable_end as &str,
-                    &syntax_config.syntax.block_start as &str,
-                    &syntax_config.syntax.block_end as &str,
-                    &syntax_config.syntax.comment_end as &str,
-                )
+    fn skip_newline_if_trim_blocks(&mut self) {
+        if self.ws_config.trim_blocks {
+            if self.rest_bytes().get(0) == Some(&b'\r') {
+                self.advance(1);
             }
-            #[cfg(not(feature = "custom_syntax"))]
-            {
-                // hardcode them here again, so the compiler can optimize
-                ("}}", "{%", "%}", "#}")
+            if self.rest_bytes().get(0) == Some(&b'\n') {
+                self.advance(1);
             }
-        };
+        }
+    }
 
-        loop {
-            if state.rest.is_empty() || state.failed {
-                return None;
+    fn handle_tail_ws(&mut self, ws: Whitespace) {
+        match ws {
+            Whitespace::Preserve => {}
+            Whitespace::Default => {
+                self.skip_newline_if_trim_blocks();
             }
+            Whitespace::Remove => {
+                self.trim_leading_whitespace = true;
+            }
+        }
+    }
 
-            let mut old_loc = state.loc();
-            match state.stack.last() {
-                Some(LexerState::Template) => {
-                    match match_start_marker(state.rest, &syntax_config) {
-                        Some((StartMarker::Comment, skip)) => {
-                            if let Some(end) =
-                                memstr(&state.rest.as_bytes()[skip..], comment_end.as_bytes())
-                            {
-                                if state
-                                    .rest
-                                    .as_bytes()
-                                    .get(end.saturating_sub(1) + skip)
-                                    .copied()
-                                    == Some(b'-')
-                                {
-                                    trim_leading_whitespace = true;
-                                }
-                                state.advance(end + skip + comment_end.len());
-                                continue;
-                            } else {
-                                return Some(Err(state.syntax_error("unexpected end of comment")));
-                            }
-                        }
-                        Some((StartMarker::Variable, skip)) => {
-                            if state.rest.as_bytes().get(skip) == Some(&b'-') {
-                                state.advance(skip + 1);
-                            } else {
-                                state.advance(skip);
-                            }
-                            state.stack.push(LexerState::InVariable);
-                            return Some(Ok((Token::VariableStart, state.span(old_loc))));
-                        }
-                        Some((StartMarker::Block, skip)) => {
-                            // raw blocks require some special handling.  If we are at the beginning of a raw
-                            // block we want to skip everything until {% endraw %} completely ignoring iterior
-                            // syntax and emit the entire raw block as TemplateData.
-                            if let Some((raw, trim_start)) =
-                                skip_basic_tag(&state.rest[skip..], "raw", block_end)
-                            {
-                                state.advance(raw + skip);
-                                let mut ptr = 0;
-                                while let Some(block) =
-                                    memstr(&state.rest.as_bytes()[ptr..], block_start.as_bytes())
-                                {
-                                    ptr += block + block_start.len();
-                                    let trim_end = state.rest.as_bytes().get(ptr) == Some(&b'-');
-                                    if let Some((endraw, trim_next)) =
-                                        skip_basic_tag(&state.rest[ptr..], "endraw", block_end)
-                                    {
-                                        let mut result = &state.rest[..ptr - block_start.len()];
-                                        if trim_start {
-                                            result = result.trim_start();
-                                        }
-                                        if trim_end {
-                                            result = result.trim_end();
-                                        }
-                                        state.advance(ptr + endraw);
-                                        trim_leading_whitespace = trim_next;
-                                        return Some(Ok((
-                                            Token::TemplateData(result),
-                                            state.span(old_loc),
-                                        )));
-                                    }
-                                }
-                                return Some(
-                                    Err(state.syntax_error("unexpected end of raw block")),
-                                );
-                            }
-
-                            if state.rest.as_bytes().get(skip) == Some(&b'-') {
-                                state.advance(skip + 1);
-                            } else {
-                                state.advance(skip);
-                            }
+    fn variable_end(&self) -> &str {
+        self.syntax_config.variable_delimiters().1
+    }
 
-                            state.stack.push(LexerState::InBlock);
-                            return Some(Ok((Token::BlockStart, state.span(old_loc))));
-                        }
-                        None => {}
-                    }
+    fn block_start(&self) -> &str {
+        self.syntax_config.block_delimiters().0
+    }
 
-                    if trim_leading_whitespace {
-                        trim_leading_whitespace = false;
-                        state.skip_whitespace();
-                    }
-                    old_loc = state.loc();
+    fn block_end(&self) -> &str {
+        self.syntax_config.block_delimiters().1
+    }
 
-                    let (lead, span) = match find_start_marker(state.rest, &syntax_config) {
-                        Some((start, false)) => (state.advance(start), state.span(old_loc)),
-                        Some((start, _)) => {
-                            let peeked = &state.rest[..start];
-                            let trimmed = peeked.trim_end();
-                            let lead = state.advance(trimmed.len());
-                            let span = state.span(old_loc);
-                            state.advance(peeked.len() - trimmed.len());
+    fn comment_end(&self) -> &str {
+        self.syntax_config.comment_delimiters().1
+    }
+
+    fn tokenize_root(&mut self) -> Result<ControlFlow<(Token<'s>, Span)>, Error> {
+        if let Some((marker, len)) = self.pending_start_marker.take() {
+            return self.handle_start_marker(marker, len);
+        }
+        if self.trim_leading_whitespace {
+            self.trim_leading_whitespace = false;
+            self.skip_whitespace();
+        }
+        let old_loc = self.loc();
+        let (lead, span) =
+            match find_start_marker(self.source, self.current_offset, &self.syntax_config) {
+                Some((start, marker, len, whitespace)) => {
+                    self.pending_start_marker = Some((marker, len));
+                    match whitespace {
+                        Whitespace::Default
+                            if should_lstrip_block(self.ws_config.lstrip_blocks, marker) =>
+                        {
+                            let peeked = &self.rest()[..start];
+                            let trimmed = lstrip_block(peeked);
+                            let lead = self.advance(trimmed.len());
+                            let span = self.span(old_loc);
+                            self.advance(peeked.len() - trimmed.len());
                             (lead, span)
                         }
-                        None => (state.advance(state.rest.len()), state.span(old_loc)),
-                    };
-                    if lead.is_empty() {
-                        continue;
-                    }
-                    return Some(Ok((Token::TemplateData(lead), span)));
-                }
-                Some(LexerState::InBlock | LexerState::InVariable) => {
-                    // in blocks whitespace is generally ignored, skip it.
-                    match state
-                        .rest
-                        .as_bytes()
-                        .iter()
-                        .position(|&x| !x.is_ascii_whitespace())
-                    {
-                        Some(0) => {}
-                        None => {
-                            state.advance(state.rest.len());
-                            continue;
+                        Whitespace::Default | Whitespace::Preserve => {
+                            (self.advance(start), self.span(old_loc))
                         }
-                        Some(offset) => {
-                            state.advance(offset);
-                            continue;
+                        Whitespace::Remove => {
+                            let peeked = &self.rest()[..start];
+                            let trimmed = peeked.trim_end();
+                            let lead = self.advance(trimmed.len());
+                            let span = self.span(old_loc);
+                            self.advance(peeked.len() - trimmed.len());
+                            (lead, span)
                         }
                     }
+                }
+                None => (self.advance(self.rest().len()), self.span(old_loc)),
+            };
 
-                    // look out for the end of blocks
-                    if let Some(&LexerState::InBlock) = state.stack.last() {
-                        if state.rest.get(..1) == Some("-")
-                            && state.rest.get(1..block_end.len() + 1) == Some(block_end)
-                        {
-                            state.stack.pop();
-                            trim_leading_whitespace = true;
-                            state.advance(block_end.len() + 1);
-                            return Some(Ok((Token::BlockEnd, state.span(old_loc))));
-                        }
-                        if state.rest.get(..block_end.len()) == Some(block_end) {
-                            state.stack.pop();
-                            state.advance(block_end.len());
-                            return Some(Ok((Token::BlockEnd, state.span(old_loc))));
-                        }
-                    } else {
-                        if state.rest.get(..1) == Some("-")
-                            && state.rest.get(1..variable_end.len() + 1) == Some(variable_end)
-                        {
-                            state.stack.pop();
-                            state.advance(variable_end.len() + 1);
-                            trim_leading_whitespace = true;
-                            return Some(Ok((Token::VariableEnd, state.span(old_loc))));
+        if lead.is_empty() {
+            Ok(ControlFlow::Continue(()))
+        } else {
+            Ok(ControlFlow::Break((Token::TemplateData(lead), span)))
+        }
+    }
+
+    fn handle_start_marker(
+        &mut self,
+        marker: StartMarker,
+        skip: usize,
+    ) -> Result<ControlFlow<(Token<'s>, Span)>, Error> {
+        match marker {
+            StartMarker::Comment => {
+                if let Some(end) = memstr(&self.rest_bytes()[skip..], self.comment_end().as_bytes())
+                {
+                    let ws = Whitespace::from_byte(
+                        self.rest_bytes().get(end.saturating_sub(1) + skip).copied(),
+                    );
+                    self.advance(end + skip + self.comment_end().len());
+                    self.handle_tail_ws(ws);
+                    Ok(ControlFlow::Continue(()))
+                } else {
+                    Err(self.syntax_error("unexpected end of comment"))
+                }
+            }
+            StartMarker::Variable => {
+                let old_loc = self.loc();
+                self.advance(skip);
+                self.stack.push(LexerState::Variable);
+                Ok(ControlFlow::Break((
+                    Token::VariableStart,
+                    self.span(old_loc),
+                )))
+            }
+            StartMarker::Block => {
+                // raw blocks require some special handling.  If we are at the beginning of a raw
+                // block we want to skip everything until {% endraw %} completely ignoring interior
+                // syntax and emit the entire raw block as TemplateData.
+                if let Some((raw, ws_start)) =
+                    skip_basic_tag(&self.rest()[skip..], "raw", self.block_end(), false)
+                {
+                    self.advance(raw + skip);
+                    self.handle_raw_tag(ws_start)
+                } else {
+                    let old_loc = self.loc();
+                    self.advance(skip);
+                    self.stack.push(LexerState::Block);
+                    Ok(ControlFlow::Break((Token::BlockStart, self.span(old_loc))))
+                }
+            }
+            #[cfg(feature = "custom_syntax")]
+            StartMarker::LineStatement => {
+                let old_loc = self.loc();
+                self.advance(skip);
+                self.stack.push(LexerState::LineStatement);
+                Ok(ControlFlow::Break((Token::BlockStart, self.span(old_loc))))
+            }
+            #[cfg(feature = "custom_syntax")]
+            StartMarker::LineComment => {
+                let comment_skip = self.rest_bytes()[skip..]
+                    .iter()
+                    .take_while(|&&c| c != b'\r' && c != b'\n')
+                    .count();
+                let (_, nl_skip) = skip_nl(&self.rest()[skip + comment_skip..]);
+                self.advance(skip + comment_skip + nl_skip);
+                Ok(ControlFlow::Continue(()))
+            }
+        }
+    }
+
+    fn handle_raw_tag(
+        &mut self,
+        ws_start: Whitespace,
+    ) -> Result<ControlFlow<(Token<'s>, Span)>, Error> {
+        let old_loc = self.loc();
+        let mut ptr = 0;
+        while let Some(block) = memstr(&self.rest_bytes()[ptr..], self.block_start().as_bytes()) {
+            ptr += block + self.block_start().len();
+            if let Some((endraw, ws_next)) =
+                skip_basic_tag(&self.rest()[ptr..], "endraw", self.block_end(), true)
+            {
+                let ws = Whitespace::from_byte(self.rest_bytes().get(ptr).copied());
+                let end = ptr - self.block_start().len();
+                let mut result = &self.rest()[..end];
+                self.advance(end);
+                let span = self.span(old_loc);
+                self.advance(self.block_start().len() + endraw);
+                match ws_start {
+                    Whitespace::Default if self.ws_config.trim_blocks => {
+                        if result.starts_with('\r') {
+                            result = &result[1..];
                         }
-                        if state.rest.get(..variable_end.len()) == Some(variable_end) {
-                            state.stack.pop();
-                            state.advance(variable_end.len());
-                            return Some(Ok((Token::VariableEnd, state.span(old_loc))));
+                        if result.starts_with('\n') {
+                            result = &result[1..];
                         }
                     }
-
-                    // two character operators
-                    let op = match state.rest.as_bytes().get(..2) {
-                        Some(b"//") => Some(Token::FloorDiv),
-                        Some(b"**") => Some(Token::Pow),
-                        Some(b"==") => Some(Token::Eq),
-                        Some(b"!=") => Some(Token::Ne),
-                        Some(b">=") => Some(Token::Gte),
-                        Some(b"<=") => Some(Token::Lte),
-                        _ => None,
-                    };
-                    if let Some(op) = op {
-                        state.advance(2);
-                        return Some(Ok((op, state.span(old_loc))));
+                    Whitespace::Remove => {
+                        result = result.trim_start();
                     }
+                    _ => {}
+                }
+                result = match ws {
+                    Whitespace::Default if self.ws_config.lstrip_blocks => lstrip_block(result),
+                    Whitespace::Remove => result.trim_end(),
+                    _ => result,
+                };
+                self.handle_tail_ws(ws_next);
+                return Ok(ControlFlow::Break((Token::TemplateData(result), span)));
+            }
+        }
+        Err(self.syntax_error("unexpected end of raw block"))
+    }
 
-                    // single character operators (and strings)
-                    let op = match state.rest.as_bytes().get(0) {
-                        Some(b'+') => Some(Token::Plus),
-                        Some(b'-') => Some(Token::Minus),
-                        Some(b'*') => Some(Token::Mul),
-                        Some(b'/') => Some(Token::Div),
-                        Some(b'%') => Some(Token::Mod),
-                        Some(b'!') => Some(Token::Bang),
-                        Some(b'.') => Some(Token::Dot),
-                        Some(b',') => Some(Token::Comma),
-                        Some(b':') => Some(Token::Colon),
-                        Some(b'~') => Some(Token::Tilde),
-                        Some(b'|') => Some(Token::Pipe),
-                        Some(b'=') => Some(Token::Assign),
-                        Some(b'>') => Some(Token::Gt),
-                        Some(b'<') => Some(Token::Lt),
-                        Some(b'(') => Some(Token::ParenOpen),
-                        Some(b')') => Some(Token::ParenClose),
-                        Some(b'[') => Some(Token::BracketOpen),
-                        Some(b']') => Some(Token::BracketClose),
-                        Some(b'{') => Some(Token::BraceOpen),
-                        Some(b'}') => Some(Token::BraceClose),
-                        Some(b'\'') => {
-                            return Some(state.eat_string(b'\''));
-                        }
-                        Some(b'"') => {
-                            return Some(state.eat_string(b'"'));
-                        }
-                        Some(c) if c.is_ascii_digit() => return Some(state.eat_number()),
-                        _ => None,
-                    };
-                    if let Some(op) = op {
-                        state.advance(1);
-                        return Some(Ok((op, state.span(old_loc))));
+    fn tokenize_block_or_var(
+        &mut self,
+        sentinel: BlockSentinel,
+    ) -> Result<ControlFlow<(Token<'s>, Span)>, Error> {
+        let old_loc = self.loc();
+        let rest = self.rest();
+
+        // special case for looking for the end of a line statements if there are no
+        // open parens, braces etc.  This can only happen with custom syntax
+        #[cfg(feature = "custom_syntax")]
+        {
+            if matches!(sentinel, BlockSentinel::LineStatement)
+                && self.paren_balance == 0
+                && self.syntax_config.line_statement_prefix().is_some()
+            {
+                let skip = rest
+                    .chars()
+                    .take_while(|&x| x.is_whitespace() && !is_nl(x))
+                    .map(|x| x.len_utf8())
+                    .sum();
+                let (was_nl, nl_skip) = skip_nl(&rest[skip..]);
+                if was_nl {
+                    self.advance(skip + nl_skip);
+                    self.stack.pop();
+                    return Ok(ControlFlow::Break((Token::BlockEnd, self.span(old_loc))));
+                }
+            }
+        }
+
+        // in blocks whitespace is generally ignored, skip it.
+        match rest
+            .as_bytes()
+            .iter()
+            .position(|&x| !x.is_ascii_whitespace())
+        {
+            Some(0) => {}
+            None => {
+                self.advance(rest.len());
+                return Ok(ControlFlow::Continue(()));
+            }
+            Some(offset) => {
+                self.advance(offset);
+                return Ok(ControlFlow::Continue(()));
+            }
+        }
+
+        // look out for the end of blocks
+        match sentinel {
+            BlockSentinel::Block => {
+                if matches!(rest.get(..1), Some("-" | "+"))
+                    && rest[1..].starts_with(self.block_end())
+                {
+                    self.stack.pop();
+                    let was_minus = &rest[..1] == "-";
+                    self.advance(self.block_end().len() + 1);
+                    let span = self.span(old_loc);
+                    if was_minus {
+                        self.trim_leading_whitespace = true;
                     }
+                    return Ok(ControlFlow::Break((Token::BlockEnd, span)));
+                }
+                if rest.starts_with(self.block_end()) {
+                    self.stack.pop();
+                    self.advance(self.block_end().len());
+                    let span = self.span(old_loc);
+                    self.skip_newline_if_trim_blocks();
+                    return Ok(ControlFlow::Break((Token::BlockEnd, span)));
+                }
+            }
+            BlockSentinel::Variable => {
+                if matches!(rest.get(..1), Some("-" | "+"))
+                    && rest[1..].starts_with(self.variable_end())
+                {
+                    self.stack.pop();
+                    let was_minus = &rest[..1] == "-";
+                    self.advance(self.variable_end().len() + 1);
+                    let span = self.span(old_loc);
+                    if was_minus {
+                        self.trim_leading_whitespace = true;
+                    }
+                    return Ok(ControlFlow::Break((Token::VariableEnd, span)));
+                }
+                if rest.starts_with(self.variable_end()) {
+                    self.stack.pop();
+                    self.advance(self.variable_end().len());
+                    return Ok(ControlFlow::Break((Token::VariableEnd, self.span(old_loc))));
+                }
+            }
+            // line statements are handled above
+            #[cfg(feature = "custom_syntax")]
+            BlockSentinel::LineStatement => {}
+        }
 
-                    return Some(state.eat_identifier());
+        // two character operators
+        let op = match rest.as_bytes().get(..2) {
+            Some(b"//") => Some(Token::FloorDiv),
+            Some(b"**") => Some(Token::Pow),
+            Some(b"==") => Some(Token::Eq),
+            Some(b"!=") => Some(Token::Ne),
+            Some(b">=") => Some(Token::Gte),
+            Some(b"<=") => Some(Token::Lte),
+            _ => None,
+        };
+        if let Some(op) = op {
+            self.advance(2);
+            return Ok(ControlFlow::Break((op, self.span(old_loc))));
+        }
+
+        macro_rules! with_paren_balance {
+            ($delta:expr, $tok:expr) => {{
+                #[cfg(feature = "custom_syntax")]
+                {
+                    self.paren_balance += $delta;
                 }
-                None => panic!("empty lexer state"),
+                Some($tok)
+            }};
+        }
+
+        // single character operators (and strings)
+        let op = match rest.as_bytes().get(0) {
+            Some(b'+') => Some(Token::Plus),
+            Some(b'-') => Some(Token::Minus),
+            Some(b'*') => Some(Token::Mul),
+            Some(b'/') => Some(Token::Div),
+            Some(b'%') => Some(Token::Mod),
+            Some(b'!') => Some(Token::Bang),
+            Some(b'.') => Some(Token::Dot),
+            Some(b',') => Some(Token::Comma),
+            Some(b':') => Some(Token::Colon),
+            Some(b'~') => Some(Token::Tilde),
+            Some(b'|') => Some(Token::Pipe),
+            Some(b'=') => Some(Token::Assign),
+            Some(b'>') => Some(Token::Gt),
+            Some(b'<') => Some(Token::Lt),
+            Some(b'(') => with_paren_balance!(1, Token::ParenOpen),
+            Some(b')') => with_paren_balance!(-1, Token::ParenClose),
+            Some(b'[') => with_paren_balance!(1, Token::BracketOpen),
+            Some(b']') => with_paren_balance!(-1, Token::BracketClose),
+            Some(b'{') => with_paren_balance!(1, Token::BraceOpen),
+            Some(b'}') => with_paren_balance!(-1, Token::BraceClose),
+            Some(b'\'') => {
+                return Ok(ControlFlow::Break(ok!(self.eat_string(b'\''))));
+            }
+            Some(b'"') => {
+                return Ok(ControlFlow::Break(ok!(self.eat_string(b'"'))));
             }
+            Some(c) if c.is_ascii_digit() => return Ok(ControlFlow::Break(ok!(self.eat_number()))),
+            _ => None,
+        };
+        if let Some(op) = op {
+            self.advance(1);
+            Ok(ControlFlow::Break((op, self.span(old_loc))))
+        } else {
+            Ok(ControlFlow::Break(ok!(self.eat_identifier())))
         }
-    })
+    }
+}
+
+/// Utility function to quickly tokenize into an iterator.
+#[cfg(any(test, feature = "unstable_machinery"))]
+pub fn tokenize(
+    input: &str,
+    in_expr: bool,
+    syntax_config: SyntaxConfig,
+    whitespace_config: WhitespaceConfig,
+) -> impl Iterator<Item = Result<(Token<'_>, Span), Error>> {
+    // This function is unused in minijinja itself, it's only used in tests and in the
+    // unstable machinery as a convenient alternative to the tokenizer.
+    let mut tokenizer = Tokenizer::new(input, in_expr, syntax_config, whitespace_config);
+    std::iter::from_fn(move || tokenizer.next_token().transpose())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     use similar_asserts::assert_eq;
 
     #[test]
-    fn test_find_marker() {
-        let syntax = SyntaxConfig::default();
-        assert!(find_start_marker("{", &syntax).is_none());
-        assert!(find_start_marker("foo", &syntax).is_none());
-        assert!(find_start_marker("foo {", &syntax).is_none());
-        assert_eq!(find_start_marker("foo {{", &syntax), Some((4, false)));
-        assert_eq!(find_start_marker("foo {{-", &syntax), Some((4, true)));
-    }
-
-    #[test]
-    #[cfg(feature = "custom_syntax")]
-    fn test_find_marker_custom_syntax() {
-        use crate::Syntax;
-
-        let syntax = Syntax {
-            block_start: "%{".into(),
-            block_end: "}%".into(),
-            variable_start: "[[".into(),
-            variable_end: "]]".into(),
-            comment_start: "/*".into(),
-            comment_end: "*/".into(),
-        };
-
-        let syntax_config = syntax.compile().expect("failed to create syntax config");
-
-        assert_eq!(find_start_marker("%{", &syntax_config), Some((0, false)));
-        assert!(find_start_marker("/", &syntax_config).is_none());
-        assert!(find_start_marker("foo [", &syntax_config).is_none());
+    fn test_is_basic_tag() {
         assert_eq!(
-            find_start_marker("foo /*", &syntax_config),
-            Some((4, false))
+            skip_basic_tag(" raw %}", "raw", "%}", false),
+            Some((7, Whitespace::Default))
         );
+        assert_eq!(skip_basic_tag(" raw %}", "endraw", "%}", false), None);
         assert_eq!(
-            find_start_marker("foo [[-", &syntax_config),
-            Some((4, true))
+            skip_basic_tag("  raw  %}", "raw", "%}", false),
+            Some((9, Whitespace::Default))
+        );
+        assert_eq!(
+            skip_basic_tag("  raw  -%}", "raw", "%}", false),
+            Some((10, Whitespace::Remove))
+        );
+        assert_eq!(
+            skip_basic_tag("  raw  +%}", "raw", "%}", false),
+            Some((10, Whitespace::Preserve))
         );
-    }
-
-    #[test]
-    fn test_is_basic_tag() {
-        assert_eq!(skip_basic_tag(" raw %}", "raw", "%}"), Some((7, false)));
-        assert_eq!(skip_basic_tag(" raw %}", "endraw", "%}"), None);
-        assert_eq!(skip_basic_tag("  raw  %}", "raw", "%}"), Some((9, false)));
-        assert_eq!(skip_basic_tag("-  raw  -%}", "raw", "%}"), Some((11, true)));
     }
 
     #[test]
     fn test_basic_identifiers() {
         fn assert_ident(s: &str) {
-            match tokenize(s, true, Default::default()).next() {
+            match tokenize(s, true, Default::default(), Default::default()).next() {
                 Some(Ok((Token::Ident(ident), _))) if ident == s => {}
                 _ => panic!("did not get a matching token result: {s:?}"),
             }
         }
 
         fn assert_not_ident(s: &str) {
-            let res = tokenize(s, true, Default::default()).collect::<Result<Vec<_>, _>>();
+            let res = tokenize(s, true, Default::default(), Default::default())
+                .collect::<Result<Vec<_>, _>>();
             if let Ok(tokens) = res {
                 if let &[(Token::Ident(_), _)] = &tokens[..] {
                     panic!("got a single ident for {s:?}")
                 }
             }
         }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/meta.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/meta.rs`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,15 @@
 #[cfg(feature = "macros")]
 pub fn find_macro_closure<'a>(m: &ast::Macro<'a>) -> HashSet<&'a str> {
     let mut state = AssignmentTracker {
         out: HashSet::new(),
         nested_out: None,
         assigned: vec![Default::default()],
     };
-    m.args.iter().for_each(|arg| track_assign(arg, &mut state));
-    m.body.iter().for_each(|node| track_walk(node, &mut state));
+    tracker_visit_macro(m, &mut state);
     state.out
 }
 
 /// Finds all variables that are undeclared in a template.
 pub fn find_undeclared(t: &ast::Stmt<'_>, track_nested: bool) -> HashSet<String> {
     let mut state = AssignmentTracker {
         out: HashSet::new(),
@@ -69,14 +68,23 @@
 
 fn tracker_visit_expr_opt<'a>(expr: &Option<ast::Expr<'a>>, state: &mut AssignmentTracker<'a>) {
     if let Some(expr) = expr {
         tracker_visit_expr(expr, state);
     }
 }
 
+#[cfg(feature = "macros")]
+fn tracker_visit_macro<'a>(m: &ast::Macro<'a>, state: &mut AssignmentTracker<'a>) {
+    m.args.iter().for_each(|arg| track_assign(arg, state));
+    m.defaults
+        .iter()
+        .for_each(|expr| tracker_visit_expr(expr, state));
+    m.body.iter().for_each(|node| track_walk(node, state));
+}
+
 fn tracker_visit_expr<'a>(expr: &ast::Expr<'a>, state: &mut AssignmentTracker<'a>) {
     match expr {
         ast::Expr::Var(var) => {
             if !state.is_assigned(var.id) {
                 state.out.insert(var.id);
                 // if we are not tracking nested assignments, we can consider a variable
                 // to be assigned the first time we perform a lookup.
@@ -119,14 +127,16 @@
                             if !state.is_assigned(var.id) {
                                 let mut rv = var.id.to_string();
                                 for attr in attrs.iter().rev() {
                                     write!(rv, ".{}", attr).ok();
                                 }
                                 state.assign_nested(rv);
                                 return;
+                            } else {
+                                break;
                             }
                         }
                         ast::Expr::GetAttr(expr) => {
                             attrs.push(expr.name);
                             ptr = &expr.expr;
                             continue;
                         }
@@ -243,17 +253,25 @@
         #[cfg(feature = "multi_template")]
         ast::Stmt::FromImport(stmt) => stmt.names.iter().for_each(|(arg, alias)| {
             track_assign(alias.as_ref().unwrap_or(arg), state);
         }),
         #[cfg(feature = "macros")]
         ast::Stmt::Macro(stmt) => {
             state.assign(stmt.name);
+            tracker_visit_macro(stmt, state);
         }
         #[cfg(feature = "macros")]
-        ast::Stmt::CallBlock(_) => {}
+        ast::Stmt::CallBlock(stmt) => {
+            tracker_visit_expr(&stmt.call.expr, state);
+            stmt.call
+                .args
+                .iter()
+                .for_each(|x| tracker_visit_expr(x, state));
+            tracker_visit_macro(&stmt.macro_decl, state);
+        }
         ast::Stmt::Do(stmt) => {
             tracker_visit_expr(&stmt.call.expr, state);
             stmt.call
                 .args
                 .iter()
                 .for_each(|x| tracker_visit_expr(x, state));
         }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/parser.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/parser.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use std::borrow::Cow;
 use std::collections::BTreeSet;
 use std::fmt;
 
 use crate::compiler::ast::{self, Spanned};
-use crate::compiler::lexer::{tokenize, SyntaxConfig};
+use crate::compiler::lexer::{Tokenizer, WhitespaceConfig};
 use crate::compiler::tokens::{Span, Token};
 use crate::error::{Error, ErrorKind};
+use crate::syntax::SyntaxConfig;
 use crate::value::Value;
 
 const MAX_RECURSION: usize = 150;
 const RESERVED_NAMES: [&str; 8] = [
     "true", "True", "false", "False", "none", "None", "loop", "self",
 ];
 
@@ -89,35 +90,40 @@
 
 enum SetParseResult<'a> {
     Set(ast::Set<'a>),
     SetBlock(ast::SetBlock<'a>),
 }
 
 struct TokenStream<'a> {
-    iter: Box<dyn Iterator<Item = Result<(Token<'a>, Span), Error>> + 'a>,
+    tokenizer: Tokenizer<'a>,
     current: Option<Result<(Token<'a>, Span), Error>>,
     last_span: Span,
 }
 
 impl<'a> TokenStream<'a> {
     /// Tokenize a template
-    pub fn new(source: &'a str, in_expr: bool, syntax: SyntaxConfig) -> TokenStream<'a> {
-        let mut iter = Box::new(tokenize(source, in_expr, syntax)) as Box<dyn Iterator<Item = _>>;
-        let current = iter.next();
+    pub fn new(
+        source: &'a str,
+        in_expr: bool,
+        syntax_config: SyntaxConfig,
+        whitespace_config: WhitespaceConfig,
+    ) -> TokenStream<'a> {
+        let mut tokenizer = Tokenizer::new(source, in_expr, syntax_config, whitespace_config);
+        let current = tokenizer.next_token().transpose();
         TokenStream {
-            iter,
+            tokenizer,
             current,
             last_span: Span::default(),
         }
     }
 
     /// Advance the stream.
     pub fn next(&mut self) -> Result<Option<(Token<'a>, Span)>, Error> {
         let rv = self.current.take();
-        self.current = self.iter.next();
+        self.current = self.tokenizer.next_token().transpose();
         if let Some(Ok((_, span))) = rv {
             self.last_span = span;
         }
         rv.transpose()
     }
 
     /// Look at the current token
@@ -217,17 +223,22 @@
         let rv = $expr;
         $parser.depth -= 1;
         rv
     }};
 }
 
 impl<'a> Parser<'a> {
-    pub fn new(source: &'a str, in_expr: bool, syntax: SyntaxConfig) -> Parser<'a> {
+    pub fn new(
+        source: &'a str,
+        in_expr: bool,
+        syntax_config: SyntaxConfig,
+        whitespace_config: WhitespaceConfig,
+    ) -> Parser<'a> {
         Parser {
-            stream: TokenStream::new(source, in_expr, syntax),
+            stream: TokenStream::new(source, in_expr, syntax_config, whitespace_config),
             in_macro: false,
             blocks: BTreeSet::new(),
             depth: 0,
         }
     }
 
     fn parse_ifexpr(&mut self) -> Result<ast::Expr<'a>, Error> {
@@ -520,24 +531,35 @@
         with_recursion_guard!(self, self.parse_primary_impl())
     }
 
     fn parse_primary_impl(&mut self) -> Result<ast::Expr<'a>, Error> {
         let (token, span) = expect_token!(self, "expression");
         macro_rules! const_val {
             ($expr:expr) => {
-                make_const(Value::from($expr), span)
+                make_const(Value::from($expr), self.stream.expand_span(span))
             };
         }
 
         match token {
             Token::Ident("true" | "True") => Ok(const_val!(true)),
             Token::Ident("false" | "False") => Ok(const_val!(false)),
             Token::Ident("none" | "None") => Ok(const_val!(())),
             Token::Ident(name) => Ok(ast::Expr::Var(Spanned::new(ast::Var { id: name }, span))),
-            Token::Str(val) => Ok(const_val!(val)),
+            Token::Str(val) => {
+                if matches_token!(self, Token::Str(_)) {
+                    let mut buf = String::from(val);
+                    while let Some((Token::Str(s), _)) = ok!(self.stream.current()) {
+                        buf.push_str(s);
+                        ok!(self.stream.next());
+                    }
+                    Ok(const_val!(buf))
+                } else {
+                    Ok(const_val!(val))
+                }
+            }
             Token::String(val) => Ok(const_val!(val)),
             Token::Int(val) => Ok(const_val!(val)),
             Token::Int128(val) => Ok(const_val!(val)),
             Token::Float(val) => Ok(const_val!(val)),
             Token::ParenOpen => self.parse_tuple_or_expression(span),
             Token::BracketOpen => self.parse_list_expr(span),
             Token::BraceOpen => self.parse_map_expr(span),
@@ -671,20 +693,33 @@
             #[cfg(feature = "macros")]
             "call" => ast::Stmt::CallBlock(respan!(ok!(self.parse_call_block()))),
             "do" => ast::Stmt::Do(respan!(ok!(self.parse_do()))),
             name => syntax_error!("unknown statement {}", name),
         })
     }
 
-    fn parse_assign_name(&mut self) -> Result<ast::Expr<'a>, Error> {
+    fn parse_assign_name(&mut self, dotted: bool) -> Result<ast::Expr<'a>, Error> {
         let (id, span) = expect_token!(self, Token::Ident(name) => name, "identifier");
         if RESERVED_NAMES.contains(&id) {
             syntax_error!("cannot assign to reserved variable name {}", id);
         }
-        Ok(ast::Expr::Var(ast::Spanned::new(ast::Var { id }, span)))
+        let mut rv = ast::Expr::Var(ast::Spanned::new(ast::Var { id }, span));
+        if dotted {
+            while skip_token!(self, Token::Dot) {
+                let (attr, span) = expect_token!(self, Token::Ident(name) => name, "identifier");
+                rv = ast::Expr::GetAttr(ast::Spanned::new(
+                    ast::GetAttr {
+                        expr: rv,
+                        name: attr,
+                    },
+                    span,
+                ));
+            }
+        }
+        Ok(rv)
     }
 
     fn parse_assignment(&mut self) -> Result<ast::Expr<'a>, Error> {
         let span = self.stream.current_span();
         let mut items = Vec::new();
         let mut is_tuple = false;
 
@@ -699,15 +734,15 @@
                 break;
             }
             items.push(if skip_token!(self, Token::ParenOpen) {
                 let rv = ok!(self.parse_assignment());
                 expect_token!(self, Token::ParenClose, "`)`");
                 rv
             } else {
-                ok!(self.parse_assign_name())
+                ok!(self.parse_assign_name(false))
             });
             if matches_token!(self, Token::Comma) {
                 is_tuple = true;
             } else {
                 break;
             }
         }
@@ -785,15 +820,15 @@
                 expect_token!(self, Token::Comma, "comma");
             }
             let target = if skip_token!(self, Token::ParenOpen) {
                 let assign = ok!(self.parse_assignment());
                 expect_token!(self, Token::ParenClose, "`)`");
                 assign
             } else {
-                ok!(self.parse_assign_name())
+                ok!(self.parse_assign_name(false))
             };
             expect_token!(self, Token::Assign, "assignment operator");
             let expr = ok!(self.parse_expr());
             assignments.push((target, expr));
         }
 
         expect_token!(self, Token::BlockEnd, "end of block");
@@ -804,15 +839,15 @@
 
     fn parse_set(&mut self) -> Result<SetParseResult<'a>, Error> {
         let (target, in_paren) = if skip_token!(self, Token::ParenOpen) {
             let assign = ok!(self.parse_assignment());
             expect_token!(self, Token::ParenClose, "`)`");
             (assign, true)
         } else {
-            (ok!(self.parse_assign_name()), false)
+            (ok!(self.parse_assign_name(true)), false)
         };
 
         if !in_paren && matches_token!(self, Token::BlockEnd | Token::Pipe) {
             let filter = if skip_token!(self, Token::Pipe) {
                 Some(ok!(self.parse_filter_chain()))
             } else {
                 None
@@ -951,17 +986,17 @@
             }
             if !names.is_empty() {
                 expect_token!(self, Token::Comma, "`,`");
             }
             if matches_token!(self, Token::BlockEnd) {
                 break;
             }
-            let name = ok!(self.parse_assign_name());
+            let name = ok!(self.parse_assign_name(false));
             let alias = if skip_token!(self, Token::Ident("as")) {
-                Some(ok!(self.parse_assign_name()))
+                Some(ok!(self.parse_assign_name(false)))
             } else {
                 None
             };
             names.push((name, alias));
         }
         Ok(ast::FromImport { expr, names })
     }
@@ -978,15 +1013,15 @@
             }
             if !args.is_empty() {
                 expect_token!(self, Token::Comma, "`,`");
                 if skip_token!(self, Token::ParenClose) {
                     break;
                 }
             }
-            args.push(ok!(self.parse_assign_name()));
+            args.push(ok!(self.parse_assign_name(false)));
             if skip_token!(self, Token::Assign) {
                 defaults.push(ok!(self.parse_expr()));
             } else if !defaults.is_empty() {
                 expect_token!(self, Token::Assign, "`=`");
             }
         }
         Ok(())
@@ -1101,53 +1136,33 @@
                 children: ok!(self.subparse(&|_| false)),
             },
             self.stream.expand_span(span),
         )))
     }
 }
 
-/// Parses a template
-#[cfg(feature = "unstable_machinery")]
-pub fn parse<'source>(source: &'source str, filename: &str) -> Result<ast::Stmt<'source>, Error> {
-    parse_with_syntax(source, filename, Default::default(), false)
-}
-
-/// Parses a template with a specific syntax
-pub fn parse_with_syntax<'source>(
+/// Parses a template.
+pub fn parse<'source>(
     source: &'source str,
     filename: &str,
-    syntax: SyntaxConfig,
-    keep_trailing_newline: bool,
+    syntax_config: SyntaxConfig,
+    whitespace_config: WhitespaceConfig,
 ) -> Result<ast::Stmt<'source>, Error> {
-    // we want to chop off a single newline at the end.  This means that a template
-    // by default does not end in a newline which is a useful property to allow
-    // inline templates to work.  If someone wants a trailing newline the expectation
-    // is that the user adds it themselves for achieve consistency.
-    let mut source = source;
-    if !keep_trailing_newline {
-        if source.ends_with('\n') {
-            source = &source[..source.len() - 1];
-        }
-        if source.ends_with('\r') {
-            source = &source[..source.len() - 1];
-        }
-    }
-
-    let mut parser = Parser::new(source, false, syntax);
+    let mut parser = Parser::new(source, false, syntax_config, whitespace_config);
     parser.parse().map_err(|mut err| {
         if err.line().is_none() {
             err.set_filename_and_span(filename, parser.stream.last_span())
         }
         err
     })
 }
 
 /// Parses an expression
-pub fn parse_expr(source: &str, syntax: SyntaxConfig) -> Result<ast::Expr<'_>, Error> {
-    let mut parser = Parser::new(source, true, syntax);
+pub fn parse_expr(source: &str) -> Result<ast::Expr<'_>, Error> {
+    let mut parser = Parser::new(source, true, Default::default(), Default::default());
     parser
         .parse_expr()
         .and_then(|result| {
             if ok!(parser.stream.next()).is_some() {
                 syntax_error!("unexpected input after expression")
             } else {
                 Ok(result)
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/compiler/tokens.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/compiler/tokens.rs`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/debug.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/debug.rs`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/defaults.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/defaults.rs`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         rv.insert("items".into(), BoxedFilter::new(filters::items));
         rv.insert("reverse".into(), BoxedFilter::new(filters::reverse));
         rv.insert("trim".into(), BoxedFilter::new(filters::trim));
         rv.insert("join".into(), BoxedFilter::new(filters::join));
         rv.insert("default".into(), BoxedFilter::new(filters::default));
         rv.insert("round".into(), BoxedFilter::new(filters::round));
         rv.insert("abs".into(), BoxedFilter::new(filters::abs));
+        rv.insert("int".into(), BoxedFilter::new(filters::int));
+        rv.insert("float".into(), BoxedFilter::new(filters::float));
         rv.insert("attr".into(), BoxedFilter::new(filters::attr));
         rv.insert("first".into(), BoxedFilter::new(filters::first));
         rv.insert("last".into(), BoxedFilter::new(filters::last));
         rv.insert("min".into(), BoxedFilter::new(filters::min));
         rv.insert("max".into(), BoxedFilter::new(filters::max));
         rv.insert("sort".into(), BoxedFilter::new(filters::sort));
         rv.insert("d".into(), BoxedFilter::new(filters::default));
@@ -117,16 +119,20 @@
     rv.insert("safe".into(), is_safe.clone());
     rv.insert("escaped".into(), is_safe);
     #[cfg(feature = "builtins")]
     {
         rv.insert("odd".into(), BoxedTest::new(tests::is_odd));
         rv.insert("even".into(), BoxedTest::new(tests::is_even));
         rv.insert("number".into(), BoxedTest::new(tests::is_number));
+        rv.insert("integer".into(), BoxedTest::new(tests::is_integer));
+        rv.insert("int".into(), BoxedTest::new(tests::is_integer));
+        rv.insert("float".into(), BoxedTest::new(tests::is_float));
         rv.insert("string".into(), BoxedTest::new(tests::is_string));
         rv.insert("sequence".into(), BoxedTest::new(tests::is_sequence));
+        rv.insert("iterable".into(), BoxedTest::new(tests::is_iterable));
         rv.insert("mapping".into(), BoxedTest::new(tests::is_mapping));
         rv.insert(
             "startingwith".into(),
             BoxedTest::new(tests::is_startingwith),
         );
         rv.insert("endingwith".into(), BoxedTest::new(tests::is_endingwith));
 
@@ -175,14 +181,18 @@
             "dict".into(),
             BoxedFunction::new(functions::dict).to_value(),
         );
         rv.insert(
             "debug".into(),
             BoxedFunction::new(functions::debug).to_value(),
         );
+        rv.insert(
+            "namespace".into(),
+            BoxedFunction::new(functions::namespace).to_value(),
+        );
     }
 
     rv
 }
 
 #[cfg(test)]
 mod unit_tests {
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/environment.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/environment.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 use std::collections::BTreeMap;
 use std::fmt;
 use std::sync::Arc;
 
 use serde::Serialize;
 
 use crate::compiler::codegen::CodeGenerator;
-use crate::compiler::lexer::SyntaxConfig;
+use crate::compiler::instructions::Instructions;
 use crate::compiler::parser::parse_expr;
 use crate::error::{attach_basic_debug_info, Error, ErrorKind};
 use crate::expression::Expression;
 use crate::output::Output;
-use crate::template::{CompiledTemplate, CompiledTemplateRef, Template};
+use crate::template::{CompiledTemplate, CompiledTemplateRef, Template, TemplateConfig};
 use crate::utils::{AutoEscape, BTreeMapKeysDebug, UndefinedBehavior};
 use crate::value::{FunctionArgs, FunctionResult, Value};
 use crate::vm::State;
 use crate::{defaults, filters, functions, tests};
 
-type AutoEscapeFunc = dyn Fn(&str) -> AutoEscape + Sync + Send;
 type FormatterFunc = dyn Fn(&mut Output, &State, &Value) -> Result<(), Error> + Sync + Send;
 type PathJoinFunc = dyn for<'s> Fn(&'s str, &'s str) -> Cow<'s, str> + Sync + Send;
+type UnknownMethodFunc =
+    dyn Fn(&State, &Value, &str, &[Value]) -> Result<Value, Error> + Sync + Send;
+
+/// The maximum recursion in the VM.  Normally each stack frame
+/// adds one to this counter (eg: every time a frame is added).
+/// However in some situations more depth is pushed if the cost
+/// of the stack frame is higher.  Raising this above this limit
+/// requires enabling the `stacker` feature.
+const MAX_RECURSION: usize = 500;
 
 /// An abstraction that holds the engine configuration.
 ///
 /// This object holds the central configuration state for templates.  It is also
 /// the container for all loaded templates.
 ///
 /// The environment holds references to the source the templates were created from.
@@ -38,22 +46,23 @@
 /// * [`Environment::empty`] creates a completely blank environment.
 #[derive(Clone)]
 pub struct Environment<'source> {
     templates: TemplateStore<'source>,
     filters: BTreeMap<Cow<'source, str>, filters::BoxedFilter>,
     tests: BTreeMap<Cow<'source, str>, tests::BoxedTest>,
     globals: BTreeMap<Cow<'source, str>, Value>,
-    default_auto_escape: Arc<AutoEscapeFunc>,
     path_join_callback: Option<Arc<PathJoinFunc>>,
+    pub(crate) unknown_method_callback: Option<Arc<UnknownMethodFunc>>,
     undefined_behavior: UndefinedBehavior,
     formatter: Arc<FormatterFunc>,
     #[cfg(feature = "debug")]
     debug: bool,
     #[cfg(feature = "fuel")]
     fuel: Option<u64>,
+    recursion_limit: usize,
 }
 
 impl<'source> Default for Environment<'source> {
     fn default() -> Self {
         Environment::empty()
     }
 }
@@ -74,47 +83,51 @@
     ///
     /// This environment does not yet contain any templates but it will have all
     /// the default filters, tests and globals loaded.  If you do not want any
     /// default configuration you can use the alternative
     /// [`empty`](Environment::empty) method.
     pub fn new() -> Environment<'source> {
         Environment {
-            templates: TemplateStore::default(),
+            templates: TemplateStore::new(TemplateConfig::new(Arc::new(
+                defaults::default_auto_escape_callback,
+            ))),
             filters: defaults::get_builtin_filters(),
             tests: defaults::get_builtin_tests(),
             globals: defaults::get_globals(),
-            default_auto_escape: Arc::new(defaults::default_auto_escape_callback),
             path_join_callback: None,
+            unknown_method_callback: None,
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
             debug: cfg!(debug_assertions),
             #[cfg(feature = "fuel")]
             fuel: None,
+            recursion_limit: MAX_RECURSION,
         }
     }
 
     /// Creates a completely empty environment.
     ///
     /// This environment has no filters, no templates, no globals and no default
     /// logic for auto escaping configured.
     pub fn empty() -> Environment<'source> {
         Environment {
-            templates: TemplateStore::default(),
+            templates: TemplateStore::new(TemplateConfig::new(Arc::new(defaults::no_auto_escape))),
             filters: Default::default(),
             tests: Default::default(),
             globals: Default::default(),
-            default_auto_escape: Arc::new(defaults::no_auto_escape),
             path_join_callback: None,
+            unknown_method_callback: None,
             undefined_behavior: UndefinedBehavior::default(),
             formatter: Arc::new(defaults::escape_formatter),
             #[cfg(feature = "debug")]
             debug: cfg!(debug_assertions),
             #[cfg(feature = "fuel")]
             fuel: None,
+            recursion_limit: MAX_RECURSION,
         }
     }
 
     /// Loads a template from a string into the environment.
     ///
     /// The `name` parameter defines the name of the template which identifies
     /// it.  To look up a loaded template use the [`get_template`](Self::get_template)
@@ -133,15 +146,15 @@
         feature = "loader",
         doc = "To address this restriction use [`add_template_owned`](Self::add_template_owned)."
     )]
     pub fn add_template(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
         self.templates.insert(name, source)
     }
 
-    /// Adds a template without without borrowing.
+    /// Adds a template without borrowing.
     ///
     /// This lets you place an owned [`String`] in the environment rather than the
     /// borrowed `&str` without having to worry about lifetimes.
     ///
     /// ```
     /// # use minijinja::Environment;
     /// let mut env = Environment::new();
@@ -197,21 +210,56 @@
         self.templates.set_loader(f);
     }
 
     /// Preserve the trailing newline when rendering templates.
     ///
     /// The default is `false`, which causes a single newline, if present, to be
     /// stripped from the end of the template.
+    ///
+    /// This setting is used whenever a template is loaded into the environment.
+    /// Changing it at a later point only affects future templates loaded.
     pub fn set_keep_trailing_newline(&mut self, yes: bool) {
-        self.templates.keep_trailing_newline = yes;
+        self.templates
+            .template_config
+            .ws_config
+            .keep_trailing_newline = yes;
     }
 
     /// Returns the value of the trailing newline preservation flag.
     pub fn keep_trailing_newline(&self) -> bool {
-        self.templates.keep_trailing_newline
+        self.templates
+            .template_config
+            .ws_config
+            .keep_trailing_newline
+    }
+
+    /// Remove the first newline after a block.
+    ///
+    /// If this is set to `true` then the first newline after a block is removed
+    /// (block, not variable tag!). Defaults to `false`.
+    pub fn set_trim_blocks(&mut self, yes: bool) {
+        self.templates.template_config.ws_config.trim_blocks = yes;
+    }
+
+    /// Returns the value of the trim blocks flag.
+    pub fn trim_blocks(&self) -> bool {
+        self.templates.template_config.ws_config.trim_blocks
+    }
+
+    /// Remove leading spaces and tabs from the start of a line to a block.
+    ///
+    /// If this is set to `true` then leading spaces and tabs from the start of a line
+    /// to the block tag are removed.
+    pub fn set_lstrip_blocks(&mut self, yes: bool) {
+        self.templates.template_config.ws_config.lstrip_blocks = yes;
+    }
+
+    /// Returns the value of the lstrip blocks flag.
+    pub fn lstrip_blocks(&self) -> bool {
+        self.templates.template_config.ws_config.lstrip_blocks
     }
 
     /// Removes a template by name.
     pub fn remove_template(&mut self, name: &str) {
         self.templates.remove(name);
     }
 
@@ -241,44 +289,95 @@
     pub fn set_path_join_callback<F>(&mut self, f: F)
     where
         F: for<'s> Fn(&'s str, &'s str) -> Cow<'s, str> + Send + Sync + 'static,
     {
         self.path_join_callback = Some(Arc::new(f));
     }
 
+    /// Sets a callback invoked for unknown methods on objects.
+    ///
+    /// This registers a function with the environment that is invoked when invoking a method
+    /// on a value results in a [`UnknownMethod`](crate::ErrorKind::UnknownMethod) error.
+    /// In that case the callback is invoked with [`State`], the [`Value`], the name of
+    /// the method as `&str` as well as all arguments in a slice.
+    ///
+    /// This for instance implements a `.items()` method that invokes the `|items` filter:
+    ///
+    /// ```rust
+    /// use minijinja::value::{ValueKind, from_args};
+    /// use minijinja::{Error, ErrorKind};
+    /// # let mut env = minijinja::Environment::new();
+    ///
+    /// env.set_unknown_method_callback(|state, value, method, args| {
+    ///     if value.kind() == ValueKind::Map && method == "items" {
+    ///         let _: () = from_args(args)?;
+    ///         state.apply_filter("items", &[value.clone()])
+    ///     } else {
+    ///         Err(Error::from(ErrorKind::UnknownMethod))
+    ///     }
+    /// });
+    /// ```
+    ///
+    /// This can be used to increase the compatibility with Jinja2 templates that might
+    /// call Python methods on objects which are not available in minijinja.
+    pub fn set_unknown_method_callback<F>(&mut self, f: F)
+    where
+        F: Fn(&State, &Value, &str, &[Value]) -> Result<Value, Error> + Sync + Send + 'static,
+    {
+        self.unknown_method_callback = Some(Arc::new(f));
+    }
+
     /// Removes all stored templates.
     ///
     /// This method is mainly useful when combined with a loader as it causes
     /// the loader to "reload" templates.  By calling this method one can trigger
     /// a reload.
     pub fn clear_templates(&mut self) {
         self.templates.clear();
     }
 
+    /// Returns an iterator over the already loaded templates and their names.
+    ///
+    /// Only templates that are already loaded will be returned.
+    ///
+    /// ```
+    /// # use minijinja::{Environment, context};
+    /// let mut env = Environment::new();
+    /// env.add_template("hello.txt", "Hello {{ name }}!").unwrap();
+    /// env.add_template("goodbye.txt", "Goodbye {{ name }}!").unwrap();
+    ///
+    /// # assert_eq!(env.templates().count(), 2);
+    /// for (name, tmpl) in env.templates() {
+    ///     println!("{}", tmpl.render(context!{ name => "World" }).unwrap());
+    /// }
+    /// ```
+    pub fn templates(&self) -> impl Iterator<Item = (&str, Template<'_, '_>)> {
+        self.templates.iter().map(|(name, template)| {
+            let template = Template::new(self, CompiledTemplateRef::Borrowed(template));
+            (name, template)
+        })
+    }
+
     /// Fetches a template by name.
     ///
     /// This requires that the template has been loaded with
     /// [`add_template`](Environment::add_template) beforehand.  If the template was
-    /// not loaded an error of kind `TemplateNotFound` is returned.  If a loaded was
+    /// not loaded an error of kind `TemplateNotFound` is returned.  If a loader was
     /// added to the engine this can also dynamically load templates.
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// let mut env = Environment::new();
     /// env.add_template("hello.txt", "Hello {{ name }}!").unwrap();
     /// let tmpl = env.get_template("hello.txt").unwrap();
     /// println!("{}", tmpl.render(context!{ name => "World" }).unwrap());
     /// ```
     pub fn get_template(&self, name: &str) -> Result<Template<'_, '_>, Error> {
         let compiled = ok!(self.templates.get(name));
-        Ok(Template::new(
-            self,
-            CompiledTemplateRef::Borrowed(compiled),
-            self.initial_auto_escape(name),
-        ))
+        Ok(Template::new(self, CompiledTemplateRef::Borrowed(compiled)))
     }
 
     /// Loads a template from a string.
     ///
     /// In some cases you really only need to work with (eg: render) a template to be
     /// rendered once only.
     ///
@@ -295,18 +394,16 @@
         source: &'source str,
     ) -> Result<Template<'_, 'source>, Error> {
         Ok(Template::new(
             self,
             CompiledTemplateRef::Owned(Arc::new(ok!(CompiledTemplate::new(
                 name,
                 source,
-                self._syntax_config().clone(),
-                self.keep_trailing_newline(),
+                &self.templates.template_config,
             )))),
-            self.initial_auto_escape(name),
         ))
     }
 
     /// Loads a template from a string, with name `<string>`.
     ///
     /// This is a shortcut to [`template_from_named_str`](Self::template_from_named_str)
     /// with name set to `<string>`.
@@ -350,22 +447,22 @@
     ///
     /// This is an alias for [`template_from_str`](Self::template_from_str) paired with
     /// [`render`](Template::render).
     ///
     /// **Note on values:** The [`Value`] type implements `Serialize` and can be
     /// efficiently passed to render.  It does not undergo actual serialization.
     pub fn render_str<S: Serialize>(&self, source: &str, ctx: S) -> Result<String, Error> {
-        // reduce total amount of code faling under mono morphization into
+        // reduce total amount of code falling under mono morphization into
         // this function, and share the rest in _eval.
         ok!(self.template_from_str(source)).render(ctx)
     }
 
     /// Sets a new function to select the default auto escaping.
     ///
-    /// This function is invoked when templates are loaded from the environment
+    /// This function is invoked when templates are loaded into the environment
     /// to determine the default auto escaping behavior.  The function is
     /// invoked with the name of the template and can make an initial auto
     /// escaping decision based on that.  The default implementation
     /// ([`default_auto_escape_callback`](defaults::default_auto_escape_callback))
     /// turn on escaping depending on the file extension.
     ///
     /// ```
@@ -379,15 +476,15 @@
     ///     }
     /// });
     /// ```
     pub fn set_auto_escape_callback<F>(&mut self, f: F)
     where
         F: Fn(&str) -> AutoEscape + 'static + Sync + Send,
     {
-        self.default_auto_escape = Arc::new(f);
+        self.templates.template_config.default_auto_escape = Arc::new(f);
     }
 
     /// Changes the undefined behavior.
     ///
     /// This changes the runtime behavior of [`undefined`](Value::UNDEFINED) values in
     /// the template engine.  For more information see [`UndefinedBehavior`].  The
     /// default is [`UndefinedBehavior::Lenient`].
@@ -492,52 +589,100 @@
     #[cfg_attr(docsrs, doc(cfg(feature = "fuel")))]
     pub fn fuel(&self) -> Option<u64> {
         self.fuel
     }
 
     /// Sets the syntax for the environment.
     ///
-    /// Note that when `source` is used, the syntax is held on the underlying source
-    /// which means that the actual source needs to have it's syntax changed.
+    /// This setting is used whenever a template is loaded into the environment.
+    /// Changing it at a later point only affects future templates loaded.
     ///
-    /// See [`Syntax`](crate::Syntax) for more information.
+    /// See [`SyntaxConfig`](crate::syntax::SyntaxConfig) for more information.
     #[cfg(feature = "custom_syntax")]
     #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
-    pub fn set_syntax(&mut self, syntax: crate::custom_syntax::Syntax) -> Result<(), Error> {
-        self.templates.syntax_config = ok!(syntax.compile());
-        Ok(())
+    pub fn set_syntax(&mut self, syntax: crate::syntax::SyntaxConfig) {
+        self.templates.template_config.syntax_config = syntax;
     }
 
-    /// Returns the current syntax.
+    /// Returns the current syntax config.
     #[cfg(feature = "custom_syntax")]
     #[cfg_attr(docsrs, doc(cfg(feature = "custom_syntax")))]
-    pub fn syntax(&self) -> &crate::custom_syntax::Syntax {
-        &self._syntax_config().syntax
+    pub fn syntax(&self) -> &crate::syntax::SyntaxConfig {
+        &self.templates.template_config.syntax_config
+    }
+
+    /// Reconfigures the runtime recursion limit.
+    ///
+    /// This defaults to `500`.  Raising it above that level requires the `stacker`
+    /// feature to be enabled.  Otherwise the limit is silently capped at that safe
+    /// maximum.  Note that the maximum is not necessarily safe if the thread uses
+    /// a lot of stack space already, it's just a value that was validated once to
+    /// provide basic protection.
+    ///
+    /// Every operation that requires recursion in MiniJinja increments an internal
+    /// recursion counter.  The actual cost attributed to that recursion depends on
+    /// the cost of the operation.  If statements and for loops for instance only
+    /// increase the counter by 1, whereas template includes and macros might increase
+    /// it to 10 or more.
+    ///
+    /// **Note on stack growth:** even if the stacker feature is enabled it does not
+    /// mean that in all cases stack can grow to the limits desired.  For instance in
+    /// WASM the maximum limits are additionally enforced by the runtime.
+    pub fn set_recursion_limit(&mut self, level: usize) {
+        #[cfg(not(feature = "stacker"))]
+        {
+            self.recursion_limit = level.min(MAX_RECURSION);
+        }
+        #[cfg(feature = "stacker")]
+        {
+            self.recursion_limit = level;
+        }
     }
 
-    fn _syntax_config(&self) -> &SyntaxConfig {
-        &self.templates.syntax_config
+    /// Returns the current max recursion limit.
+    pub fn recursion_limit(&self) -> usize {
+        self.recursion_limit
     }
 
     /// Compiles an expression.
     ///
     /// This lets one compile an expression in the template language and
     /// receive the output.  This lets one use the expressions of the language
     /// be used as a minimal scripting language.  For more information and an
     /// example see [`Expression`].
     pub fn compile_expression(&self, expr: &'source str) -> Result<Expression<'_, 'source>, Error> {
-        attach_basic_debug_info(self._compile_expression(expr), expr)
+        self._compile_expression(expr)
+            .map(|instr| Expression::new(self, instr))
+    }
+
+    /// Compiles an expression without capturing the lifetime.
+    ///
+    /// This works exactly like [`compile_expression`](Self::compile_expression) but
+    /// lets you pass an owned string without capturing the lifetime.
+    #[cfg(feature = "loader")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "loader")))]
+    pub fn compile_expression_owned<E>(&self, expr: E) -> Result<Expression<'_, 'source>, Error>
+    where
+        E: Into<Cow<'source, str>>,
+    {
+        crate::loader::OwnedInstructions::try_new(Box::from(expr.into()), |expr| {
+            self._compile_expression(expr)
+        })
+        .map(|instr| Expression::new_owned(self, instr))
     }
 
-    fn _compile_expression(&self, expr: &'source str) -> Result<Expression<'_, 'source>, Error> {
-        let ast = ok!(parse_expr(expr, self._syntax_config().clone()));
-        let mut gen = CodeGenerator::new("<expression>", expr);
-        gen.compile_expr(&ast);
-        let (instructions, _) = gen.finish();
-        Ok(Expression::new(self, instructions))
+    fn _compile_expression<'expr>(&self, expr: &'expr str) -> Result<Instructions<'expr>, Error> {
+        attach_basic_debug_info(
+            parse_expr(expr).map(|ast| {
+                let mut gen = CodeGenerator::new("<expression>", expr);
+                gen.compile_expr(&ast);
+                gen.finish().0
+            }),
+            expr,
+        )
     }
 
     /// Adds a new filter function.
     ///
     /// Filter functions are functions that can be applied to values in
     /// templates.  For details about filters have a look at
     /// [`Filter`](crate::filters::Filter).
@@ -629,15 +774,15 @@
 
     /// Looks up a test function.
     pub(crate) fn get_test(&self, name: &str) -> Option<&tests::BoxedTest> {
         self.tests.get(name)
     }
 
     pub(crate) fn initial_auto_escape(&self, name: &str) -> AutoEscape {
-        (self.default_auto_escape)(name)
+        (self.templates.template_config.default_auto_escape)(name)
     }
 
     /// Formats a value into the final format.
     ///
     /// This step is called finalization in Jinja2 but since we are writing into
     /// the output stream rather than converting values, it's renamed to format
     /// here.
@@ -663,36 +808,41 @@
     }
 }
 
 #[cfg(not(feature = "loader"))]
 mod basic_store {
     use super::*;
 
-    #[derive(Clone, Default)]
-    pub struct BasicStore<'source> {
-        pub syntax_config: SyntaxConfig,
-        pub keep_trailing_newline: bool,
+    #[derive(Clone)]
+    pub(crate) struct BasicStore<'source> {
+        pub template_config: TemplateConfig,
         map: BTreeMap<&'source str, Arc<CompiledTemplate<'source>>>,
     }
 
     impl<'source> fmt::Debug for BasicStore<'source> {
         fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
             BTreeMapKeysDebug(&self.map).fmt(f)
         }
     }
 
     impl<'source> BasicStore<'source> {
+        pub fn new(template_config: TemplateConfig) -> BasicStore<'source> {
+            BasicStore {
+                template_config,
+                map: BTreeMap::default(),
+            }
+        }
+
         pub fn insert(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
             self.map.insert(
                 name,
                 Arc::new(ok!(CompiledTemplate::new(
                     name,
                     source,
-                    self.syntax_config.clone(),
-                    self.keep_trailing_newline
+                    &self.template_config
                 ))),
             );
             Ok(())
         }
 
         pub fn remove(&mut self, name: &str) {
             self.map.remove(name);
@@ -704,14 +854,18 @@
 
         pub fn get(&self, name: &str) -> Result<&CompiledTemplate<'source>, Error> {
             self.map
                 .get(name)
                 .map(|x| &**x)
                 .ok_or_else(|| Error::new_not_found(name))
         }
+
+        pub fn iter(&self) -> impl Iterator<Item = (&str, &CompiledTemplate<'source>)> {
+            self.map.iter().map(|(name, template)| (*name, &**template))
+        }
     }
 }
 
 #[cfg(not(feature = "loader"))]
 use self::basic_store::BasicStore as TemplateStore;
 
 #[cfg(feature = "loader")]
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/error.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use std::borrow::Cow;
 use std::fmt;
+use std::sync::Arc;
 
 use crate::compiler::tokens::Span;
 
 /// Represents template errors.
 ///
 /// If debug mode is enabled a template error contains additional debug
 /// information that can be displayed by formatting an error with the
@@ -12,15 +13,15 @@
 /// is hidden when the alternative formatting is used.
 ///
 /// Since MiniJinja takes advantage of chained errors it's recommended
 /// to render the entire chain to better understand the causes.
 ///
 /// # Example
 ///
-/// Here is an example of you might want to render errors:
+/// Here is an example of how you might want to render errors:
 ///
 /// ```rust
 /// # let mut env = minijinja::Environment::new();
 /// # env.add_template("", "");
 /// # let template = env.get_template("").unwrap(); let ctx = ();
 /// match template.render(ctx) {
 ///     Ok(result) => println!("{}", result),
@@ -37,23 +38,24 @@
 /// }
 /// ```
 pub struct Error {
     repr: Box<ErrorRepr>,
 }
 
 /// The internal error data
+#[derive(Clone)]
 struct ErrorRepr {
     kind: ErrorKind,
     detail: Option<Cow<'static, str>>,
     name: Option<String>,
     lineno: usize,
     span: Option<Span>,
-    source: Option<Box<dyn std::error::Error + Send + Sync>>,
+    source: Option<Arc<dyn std::error::Error + Send + Sync>>,
     #[cfg(feature = "debug")]
-    debug_info: Option<crate::debug::DebugInfo>,
+    debug_info: Option<Arc<crate::debug::DebugInfo>>,
 }
 
 impl fmt::Debug for Error {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut err = f.debug_struct("Error");
         err.field("kind", &self.kind());
         if let Some(ref detail) = self.repr.detail {
@@ -66,41 +68,31 @@
             err.field("line", &line);
         }
         if let Some(ref source) = std::error::Error::source(self) {
             err.field("source", source);
         }
         ok!(err.finish());
 
-        // so this is a bit questionablem, but because of how commonly errors are just
+        // so this is a bit questionable, but because of how commonly errors are just
         // unwrapped i think it's sensible to spit out the debug info following the
         // error struct dump.
         #[cfg(feature = "debug")]
         {
-            if !f.alternate() {
-                if let Some(info) = self.debug_info() {
-                    ok!(writeln!(f));
-                    ok!(crate::debug::render_debug_info(
-                        f,
-                        self.name(),
-                        self.kind(),
-                        self.line(),
-                        self.span(),
-                        info,
-                    ));
-                    ok!(writeln!(f));
-                }
+            if !f.alternate() && self.debug_info().is_some() {
+                ok!(writeln!(f));
+                ok!(writeln!(f, "{}", self.display_debug_info()));
             }
         }
 
         Ok(())
     }
 }
 
 /// An enum describing the error kind.
-#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+#[derive(Debug, Copy, Clone, PartialEq, Eq, Hash)]
 #[non_exhaustive]
 pub enum ErrorKind {
     /// A non primitive value was encountered where one was expected.
     NonPrimitive,
     /// A value is not valid for a key in a map.
     NonKey,
     /// An invalid operation was attempted.
@@ -196,25 +188,16 @@
             ok!(write!(f, "{}", self.kind()));
         }
         if let Some(ref filename) = self.name() {
             ok!(write!(f, " (in {}:{})", filename, self.line().unwrap_or(0)))
         }
         #[cfg(feature = "debug")]
         {
-            if f.alternate() {
-                if let Some(info) = self.debug_info() {
-                    ok!(crate::debug::render_debug_info(
-                        f,
-                        self.name(),
-                        self.kind(),
-                        self.line(),
-                        self.span(),
-                        info,
-                    ));
-                }
+            if f.alternate() && self.debug_info().is_some() {
+                ok!(write!(f, "{}", self.display_debug_info()));
             }
         }
         Ok(())
     }
 }
 
 impl Error {
@@ -230,14 +213,20 @@
                 source: None,
                 #[cfg(feature = "debug")]
                 debug_info: None,
             }),
         }
     }
 
+    pub(crate) fn internal_clone(&self) -> Error {
+        Error {
+            repr: self.repr.clone(),
+        }
+    }
+
     pub(crate) fn set_filename_and_line(&mut self, filename: &str, lineno: usize) {
         self.repr.name = Some(filename.into());
         self.repr.lineno = lineno;
     }
 
     pub(crate) fn set_filename_and_span(&mut self, filename: &str, span: Span) {
         self.repr.name = Some(filename.into());
@@ -249,17 +238,16 @@
         Error::new(
             ErrorKind::TemplateNotFound,
             format!("template {name:?} does not exist"),
         )
     }
 
     /// Attaches another error as source to this error.
-    #[allow(unused)]
     pub fn with_source<E: std::error::Error + Send + Sync + 'static>(mut self, source: E) -> Self {
-        self.repr.source = Some(Box::new(source));
+        self.repr.source = Some(Arc::new(source));
         self
     }
 
     /// Returns the error kind
     pub fn kind(&self) -> ErrorKind {
         self.repr.kind
     }
@@ -315,14 +303,45 @@
     #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
     pub fn range(&self) -> Option<std::ops::Range<usize>> {
         self.repr
             .span
             .map(|x| x.start_offset as usize..x.end_offset as usize)
     }
 
+    /// Helper function that renders all known debug info on format.
+    ///
+    /// This method returns an object that when formatted prints out the debug information
+    /// that is contained on that error.  Normally this is automatically rendered when the
+    /// error is displayed but in some cases you might want to decide for yourself when and
+    /// how to display that information.
+    #[cfg(feature = "debug")]
+    #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
+    pub fn display_debug_info(&self) -> impl fmt::Display + '_ {
+        struct Proxy<'a>(&'a Error);
+
+        impl<'a> fmt::Display for Proxy<'a> {
+            fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+                if let Some(info) = self.0.debug_info() {
+                    crate::debug::render_debug_info(
+                        f,
+                        self.0.name(),
+                        self.0.kind(),
+                        self.0.line(),
+                        self.0.span(),
+                        info,
+                    )
+                } else {
+                    Ok(())
+                }
+            }
+        }
+
+        Proxy(self)
+    }
+
     /// Returns the template source if available.
     #[cfg(feature = "debug")]
     #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
     pub fn template_source(&self) -> Option<&str> {
         self.debug_info().and_then(|x| x.source())
     }
 
@@ -335,21 +354,21 @@
     /// Returns the template debug information is available.
     ///
     /// The debug info snapshot is only embedded into the error if the debug
     /// mode is enabled on the environment
     /// ([`Environment::set_debug`](crate::Environment::set_debug)).
     #[cfg(feature = "debug")]
     pub(crate) fn debug_info(&self) -> Option<&crate::debug::DebugInfo> {
-        self.repr.debug_info.as_ref()
+        self.repr.debug_info.as_deref()
     }
 
     #[cfg(feature = "debug")]
     #[cfg_attr(docsrs, doc(cfg(feature = "debug")))]
     pub(crate) fn attach_debug_info(&mut self, value: crate::debug::DebugInfo) {
-        self.repr.debug_info = Some(value);
+        self.repr.debug_info = Some(Arc::new(value));
     }
 }
 
 impl std::error::Error for Error {
     fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
         self.repr.source.as_ref().map(|err| err.as_ref() as _)
     }
@@ -380,18 +399,18 @@
 
 pub fn attach_basic_debug_info<T>(rv: Result<T, Error>, source: &str) -> Result<T, Error> {
     #[cfg(feature = "debug")]
     {
         match rv {
             Ok(rv) => Ok(rv),
             Err(mut err) => {
-                err.repr.debug_info = Some(crate::debug::DebugInfo {
+                err.repr.debug_info = Some(Arc::new(crate::debug::DebugInfo {
                     template_source: Some(source.to_string()),
                     ..Default::default()
-                });
+                }));
                 Err(err)
             }
         }
     }
     #[cfg(not(feature = "debug"))]
     {
         let _source = source;
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/filters.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/filters.rs`

 * *Files 3% similar despite different names*

```diff
@@ -44,29 +44,66 @@
 //!
 //! MiniJinja will perform the necessary conversions automatically.  For more
 //! information see the [`Filter`] trait.
 //!
 //! # Accessing State
 //!
 //! In some cases it can be necessary to access the execution [`State`].  Since a borrowed
-//! state implements [`ArgType`](crate::value::ArgType) it's possible to add a
-//! parameter that holds the state.  For instance the following filter appends
-//! the current template name to the string:
+//! state implements [`ArgType`] it's possible to add a parameter that holds the state.
+//! For instance the following filter appends the current template name to the string:
 //!
 //! ```
 //! # use minijinja::Environment;
 //! # let mut env = Environment::new();
-//! use minijinja::value::Value;
-//! use minijinja::State;
+//! use minijinja::{Value, State};
 //!
 //! fn append_template(state: &State, value: &Value) -> String {
 //!     format!("{}-{}", value, state.name())
 //! }
 //!
-//! env.add_filter("appendTemplate", append_template);
+//! env.add_filter("append_template", append_template);
+//! ```
+//!
+//! # Filter configuration
+//!
+//! The recommended pattern for filters to change their behavior is to leverage global
+//! variables in the template.  For instance take a filter that performs date formatting.
+//! You might want to change the default time format format on a per-template basis
+//! without having to update every filter invocation.  In this case the recommended
+//! pattern is to reserve upper case variables and look them up in the filter:
+//!
+//! ```
+//! # use minijinja::Environment;
+//! # let mut env = Environment::new();
+//! # fn format_unix_timestamp(_: f64, _: &str) -> String { "".into() }
+//! use minijinja::State;
+//!
+//! fn timeformat(state: &State, ts: f64) -> String {
+//!     let configured_format = state.lookup("TIME_FORMAT");
+//!     let format = configured_format
+//!         .as_ref()
+//!         .and_then(|x| x.as_str())
+//!         .unwrap_or("HH:MM:SS");
+//!     format_unix_timestamp(ts, format)
+//! }
+//!
+//! env.add_filter("timeformat", timeformat);
+//! ```
+//!
+//! This then later lets a user override the default either by using
+//! [`add_global`](crate::Environment::add_global) or by passing it with the
+//! [`context!`] macro or similar.
+//!
+//! ```
+//! # use minijinja::context;
+//! # let other_variables = context!{};
+//! let ctx = context! {
+//!     TIME_FORMAT => "HH:MM",
+//!     ..other_variables
+//! };
 //! ```
 //!
 //! # Built-in Filters
 //!
 //! When the `builtins` feature is enabled a range of built-in filters are
 //! automatically added to the environment.  These are also all provided in
 //! this module.  Note though that these functions are not to be
@@ -101,15 +138,15 @@
 /// * `Rv` where `Rv` implements `Into<Value>`
 /// * `Result<Rv, Error>` where `Rv` implements `Into<Value>`
 ///
 /// Filters accept one mandatory parameter which is the value the filter is
 /// applied to and up to 4 extra parameters.  The extra parameters can be
 /// marked optional by using `Option<T>`.  The last argument can also use
 /// [`Rest<T>`](crate::value::Rest) to capture the remaining arguments.  All
-/// types are supported for which [`ArgType`](crate::value::ArgType) is implemented.
+/// types are supported for which [`ArgType`] is implemented.
 ///
 /// For a list of built-in filters see [`filters`](crate::filters).
 ///
 /// # Basic Example
 ///
 /// ```
 /// # use minijinja::Environment;
@@ -252,14 +289,15 @@
 }
 
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
     use crate::error::ErrorKind;
+    use crate::value::ops::as_f64;
     use crate::value::{Kwargs, ValueKind, ValueRepr};
     use std::borrow::Cow;
     use std::cmp::Ordering;
     use std::fmt::Write;
     use std::mem;
 
     /// Converts a value to uppercase.
@@ -452,33 +490,24 @@
             Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "cannot convert value into pair list",
             ))
         }
     }
 
-    /// Reverses a list or string
+    /// Reverses an iterable or string
     ///
     /// ```jinja
     /// {% for user in users|reverse %}
     ///   <li>{{ user.name }}
     /// {% endfor %}
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn reverse(v: Value) -> Result<Value, Error> {
-        if let Some(s) = v.as_str() {
-            Ok(Value::from(s.chars().rev().collect::<String>()))
-        } else if let Some(seq) = v.as_seq() {
-            Ok(Value::from(seq.iter().rev().collect::<Vec<_>>()))
-        } else {
-            Err(Error::new(
-                ErrorKind::InvalidOperation,
-                format!("cannot reverse value of type {}", v.kind()),
-            ))
-        }
+        v.reverse()
     }
 
     /// Trims a value
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn trim(s: Cow<'_, str>, chars: Option<Cow<'_, str>>) -> String {
         match chars {
             Some(chars) => {
@@ -503,17 +532,17 @@
             for c in s.chars() {
                 if !rv.is_empty() {
                     rv.push_str(joiner);
                 }
                 rv.push(c);
             }
             Ok(rv)
-        } else if let Some(seq) = val.as_seq() {
+        } else if let Some(iter) = val.as_object().and_then(|x| x.try_iter()) {
             let mut rv = String::new();
-            for item in seq.iter() {
+            for item in iter {
                 if !rv.is_empty() {
                     rv.push_str(joiner);
                 }
                 if let Some(s) = item.as_str() {
                     rv.push_str(s);
                 } else {
                     write!(rv, "{item}").ok();
@@ -566,14 +595,78 @@
             _ => Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "cannot get absolute value",
             )),
         }
     }
 
+    /// Converts a value into an integer.
+    ///
+    /// ```jinja
+    /// {{ "42"|int == 42 }} -> true
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn int(value: Value) -> Result<Value, Error> {
+        match &value.0 {
+            ValueRepr::Undefined | ValueRepr::None => Ok(Value::from(0)),
+            ValueRepr::Bool(x) => Ok(Value::from(*x as u64)),
+            ValueRepr::U64(_) | ValueRepr::I64(_) | ValueRepr::U128(_) | ValueRepr::I128(_) => {
+                Ok(value)
+            }
+            ValueRepr::F64(v) => {
+                let x = *v as i128;
+                if x as f64 == *v {
+                    Ok(Value::from(x))
+                } else {
+                    Err(Error::new(
+                        ErrorKind::InvalidOperation,
+                        format!("cannot convert float {} to integer", v),
+                    ))
+                }
+            }
+            ValueRepr::String(..) | ValueRepr::SmallStr(_) => value
+                .as_str()
+                .unwrap()
+                .parse::<i128>()
+                .map(Value::from)
+                .map_err(|err| Error::new(ErrorKind::InvalidOperation, err.to_string())),
+            ValueRepr::Bytes(_) | ValueRepr::Object(_) => Err(Error::new(
+                ErrorKind::InvalidOperation,
+                format!("cannot convert {} to integer", value.kind()),
+            )),
+            ValueRepr::Invalid(_) => value.validate(),
+        }
+    }
+
+    /// Converts a value into a float.
+    ///
+    /// ```jinja
+    /// {{ "42.5"|float == 42.5 }} -> true
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn float(value: Value) -> Result<Value, Error> {
+        match &value.0 {
+            ValueRepr::Undefined | ValueRepr::None => Ok(Value::from(0.0)),
+            ValueRepr::Bool(x) => Ok(Value::from(*x as u64 as f64)),
+            ValueRepr::String(..) | ValueRepr::SmallStr(_) => value
+                .as_str()
+                .unwrap()
+                .parse::<f64>()
+                .map(Value::from)
+                .map_err(|err| Error::new(ErrorKind::InvalidOperation, err.to_string())),
+            ValueRepr::Invalid(_) => value.validate(),
+            _ => as_f64(&value).map(Value::from).ok_or_else(|| {
+                Error::new(
+                    ErrorKind::InvalidOperation,
+                    format!("cannot convert {} to float", value.kind()),
+                )
+            }),
+        }
+    }
+
     /// Looks up an attribute.
     ///
     /// In MiniJinja this is the same as the `[]` operator.  In Jinja2 there is a
     /// small difference which is why this filter is sometimes used in Jinja2
     /// templates.  For compatibility it's provided here as well.
     ///
     /// ```jinja
@@ -606,39 +699,39 @@
             _ => Err(Error::new(
                 ErrorKind::InvalidOperation,
                 format!("cannot round value ({})", value.kind()),
             )),
         }
     }
 
-    /// Returns the first item from a list.
+    /// Returns the first item from an iterable.
     ///
     /// If the list is empty `undefined` is returned.
     ///
     /// ```jinja
     /// <dl>
     ///   <dt>primary email
     ///   <dd>{{ user.email_addresses|first|default('no user') }}
     /// </dl>
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn first(value: Value) -> Result<Value, Error> {
         if let Some(s) = value.as_str() {
             Ok(s.chars().next().map_or(Value::UNDEFINED, Value::from))
-        } else if let Some(s) = value.as_seq() {
-            Ok(s.get_item(0).unwrap_or(Value::UNDEFINED))
+        } else if let Some(mut iter) = value.as_object().and_then(|x| x.try_iter()) {
+            Ok(iter.next().unwrap_or(Value::UNDEFINED))
         } else {
             Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "cannot get first item from value",
             ))
         }
     }
 
-    /// Returns the last item from a list.
+    /// Returns the last item from an iterable.
     ///
     /// If the list is empty `undefined` is returned.
     ///
     /// ```jinja
     /// <h2>Most Recent Update</h2>
     /// {% with update = updates|last %}
     ///   <dl>
@@ -649,34 +742,44 @@
     ///   </dl>
     /// {% endwith %}
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn last(value: Value) -> Result<Value, Error> {
         if let Some(s) = value.as_str() {
             Ok(s.chars().next_back().map_or(Value::UNDEFINED, Value::from))
-        } else if let Some(seq) = value.as_seq() {
-            Ok(seq.iter().last().unwrap_or(Value::UNDEFINED))
+        } else if matches!(value.kind(), ValueKind::Seq | ValueKind::Iterable) {
+            let rev = ok!(value.reverse());
+            let mut iter = ok!(rev.try_iter());
+            Ok(iter.next().unwrap_or_default())
         } else {
             Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "cannot get last item from value",
             ))
         }
     }
 
-    /// Returns the smallest item from the list.
+    /// Returns the smallest item from an iterable.
+    ///
+    /// ```jinja
+    /// {{ [1, 2, 3, 4]|min }} -> 1
+    /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn min(state: &State, value: Value) -> Result<Value, Error> {
         let iter = ok!(state.undefined_behavior().try_iter(value).map_err(|err| {
             Error::new(ErrorKind::InvalidOperation, "cannot convert value to list").with_source(err)
         }));
         Ok(iter.min().unwrap_or(Value::UNDEFINED))
     }
 
-    /// Returns the largest item from the list.
+    /// Returns the largest item from an iterable.
+    ///
+    /// ```jinja
+    /// {{ [1, 2, 3, 4]|max }} -> 4
+    /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn max(state: &State, value: Value) -> Result<Value, Error> {
         let iter = ok!(state.undefined_behavior().try_iter(value).map_err(|err| {
             Error::new(ErrorKind::InvalidOperation, "cannot convert value to list").with_source(err)
         }));
         Ok(iter.max().unwrap_or(Value::UNDEFINED))
     }
@@ -733,14 +836,18 @@
         Ok(Value::from(iter.collect::<Vec<_>>()))
     }
 
     /// Converts the value into a boolean value.
     ///
     /// This behaves the same as the if statement does with regards to
     /// handling of boolean values.
+    ///
+    /// ```jinja
+    /// {{ 42|bool }} -> true
+    /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn bool(value: Value) -> bool {
         value.is_true()
     }
 
     /// Slice an iterable and return a list of lists containing
     /// those items.
@@ -892,15 +999,15 @@
                     _ => rv.push(c),
                 }
             }
             Value::from_safe_string(rv)
         })
     }
 
-    /// indents Value with spaces
+    /// Indents Value with spaces
     ///
     /// The first optional parameter to the filter can be set to `true` to
     /// indent the first line. The parameter defaults to false.
     /// the second optional parameter to the filter can be set to `true`
     /// to indent blank lines. The parameter defaults to false.
     /// This filter is useful, if you want to template yaml-files
     ///
@@ -967,35 +1074,38 @@
             .remove(b'.')
             .remove(b'-')
             .remove(b'_')
             .add(b' ');
 
         if value.kind() == ValueKind::Map {
             let mut rv = String::new();
-            for (idx, k) in ok!(value.try_iter()).enumerate() {
-                if idx > 0 {
+            for k in ok!(value.try_iter()) {
+                let v = ok!(value.get_item(&k));
+                if v.is_none() || v.is_undefined() {
+                    continue;
+                }
+                if !rv.is_empty() {
                     rv.push('&');
                 }
-                let v = ok!(value.get_item(&k));
                 write!(
                     rv,
                     "{}={}",
                     percent_encoding::utf8_percent_encode(&k.to_string(), SET),
                     percent_encoding::utf8_percent_encode(&v.to_string(), SET)
                 )
                 .unwrap();
             }
             Ok(rv)
         } else {
             match &value.0 {
                 ValueRepr::None | ValueRepr::Undefined => Ok("".into()),
                 ValueRepr::Bytes(b) => Ok(percent_encoding::percent_encode(b, SET).to_string()),
-                ValueRepr::String(s, _) => {
-                    Ok(percent_encoding::utf8_percent_encode(s, SET).to_string())
-                }
+                ValueRepr::String(..) | ValueRepr::SmallStr(_) => Ok(
+                    percent_encoding::utf8_percent_encode(value.as_str().unwrap(), SET).to_string(),
+                ),
                 _ => Ok(percent_encoding::utf8_percent_encode(&value.to_string(), SET).to_string()),
             }
         }
     }
 
     #[cfg(feature = "builtins")]
     fn select_or_reject(
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/functions.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/functions.rs`

 * *Files 21% similar despite different names*

```diff
@@ -36,28 +36,60 @@
 //!             "cannot load file"
 //!         ).with_source(e))
 //! }
 //!
 //! env.add_function("include_file", include_file);
 //! ```
 //!
+#![cfg_attr(
+    feature = "deserialization",
+    doc = r#"
+# Arguments in Custom Functions
+
+All arguments in custom functions must implement the [`ArgType`] trait.
+Standard types, such as `String`, `i32`, `bool`, `f64`, etc, already implement this trait.
+There are also helper types that will make it easier to extract an arguments with custom types.
+The [`ViaDeserialize<T>`](crate::value::ViaDeserialize) type, for instance, can accept any
+type `T` that implements the `Deserialize` trait from `serde`.
+
+```rust
+# use minijinja::Environment;
+# use serde::Deserialize;
+# let mut env = Environment::new();
+use minijinja::value::ViaDeserialize;
+
+#[derive(Deserialize)]
+struct Person {
+    name: String,
+    age: i32,
+}
+
+fn is_adult(person: ViaDeserialize<Person>) -> bool {
+    person.age >= 18
+}
+
+env.add_function("is_adult", is_adult);
+```
+"#
+)]
+//!
 //! # Note on Keyword Arguments
 //!
 //! MiniJinja inherits a lot of the runtime model from Jinja2.  That includes support for
 //! keyword arguments.  These however are a concept not native to Rust which makes them
-//! somewhat unconfortable to work with.  In MiniJinja keyword arguments are implemented by
+//! somewhat uncomfortable to work with.  In MiniJinja keyword arguments are implemented by
 //! converting them into an extra parameter represented by a map.  That means if you call
 //! a function as `foo(1, 2, three=3, four=4)` the function gets three arguments:
 //!
 //! ```json
 //! [1, 2, {"three": 3, "four": 4}]
 //! ```
 //!
-//! If a function wants to disambiugate between a value passed as keyword argument or not,
-//! the the [`Value::is_kwargs`] can be used which returns `true` if a value represents
+//! If a function wants to disambiguate between a value passed as keyword argument or not,
+//! the [`Value::is_kwargs`] can be used which returns `true` if a value represents
 //! keyword arguments as opposed to just a map.  A more convenient way to work with keyword
 //! arguments is the [`Kwargs`](crate::value::Kwargs) type.
 //!
 //! # Built-in Functions
 //!
 //! When the `builtins` feature is enabled a range of built-in functions are
 //! automatically added to the environment.  These are also all provided in
@@ -65,15 +97,15 @@
 //! called from Rust code as their exact interface (arguments and return types)
 //! might change from one MiniJinja version to another.
 use std::fmt;
 use std::sync::Arc;
 
 use crate::error::Error;
 use crate::utils::SealedMarker;
-use crate::value::{ArgType, FunctionArgs, FunctionResult, Object, Value};
+use crate::value::{ArgType, FunctionArgs, FunctionResult, Object, ObjectRepr, Value};
 use crate::vm::State;
 
 type FuncFunc = dyn Fn(&State, &[Value]) -> Result<Value, Error> + Sync + Send + 'static;
 
 /// A boxed function.
 #[derive(Clone)]
 pub(crate) struct BoxedFunction(Arc<FuncFunc>, #[cfg(feature = "debug")] &'static str);
@@ -91,18 +123,24 @@
 ///
 /// * `Rv` where `Rv` implements `Into<Value>`
 /// * `Result<Rv, Error>` where `Rv` implements `Into<Value>`
 ///
 /// The parameters can be marked optional by using `Option<T>`.  The last
 /// argument can also use [`Rest<T>`](crate::value::Rest) to capture the
 /// remaining arguments.  All types are supported for which
-/// [`ArgType`](crate::value::ArgType) is implemented.
+/// [`ArgType`] is implemented.
 ///
 /// For a list of built-in functions see [`functions`](crate::functions).
 ///
+/// **Note:** this trait cannot be implemented and only exists drive the
+/// functionality of [`add_function`](crate::Environment::add_function)
+/// and [`from_function`](crate::value::Value::from_function).  If you want
+/// to implement a custom callable, you can directly implement
+/// [`Object::call`] which is what the engine actually uses internally.
+///
 /// # Basic Example
 ///
 /// ```rust
 /// # use minijinja::Environment;
 /// # let mut env = Environment::new();
 /// use minijinja::{Error, ErrorKind};
 ///
@@ -205,34 +243,30 @@
                 return f.write_str(self.1);
             }
         }
         f.write_str("function")
     }
 }
 
-impl fmt::Display for BoxedFunction {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "{self:?}")
+impl Object for BoxedFunction {
+    fn repr(self: &Arc<Self>) -> ObjectRepr {
+        ObjectRepr::Plain
     }
-}
 
-impl Object for BoxedFunction {
-    fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
+    fn call(self: &Arc<Self>, state: &State, args: &[Value]) -> Result<Value, Error> {
         self.invoke(state, args)
     }
 }
 
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
-    use std::collections::BTreeMap;
-
     use crate::error::ErrorKind;
-    use crate::value::{MapType, ValueRepr};
+    use crate::value::{Rest, ValueMap, ValueRepr};
 
     /// Returns a range.
     ///
     /// Return a list containing an arithmetic progression of integers. `range(i,
     /// j)` returns `[i, i+1, i+2, ..., j-1]`. `lower` defaults to 0. When `step` is
     /// given, it specifies the increment (or decrement). For example, `range(4)`
     /// and `range(0, 4, 1)` return `[0, 1, 2, 3]`. The end point is omitted.
@@ -243,23 +277,25 @@
     ///   <li>{{ num }}
     /// {% endfor %}
     /// </ul>
     /// ```
     ///
     /// This function will refuse to create ranges over 10.000 items.
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
-    pub fn range(lower: u32, upper: Option<u32>, step: Option<u32>) -> Result<Vec<u32>, Error> {
-        fn to_result<I: ExactSizeIterator<Item = u32>>(i: I) -> Result<Vec<u32>, Error> {
-            if i.len() > 10000 {
+    pub fn range(lower: u32, upper: Option<u32>, step: Option<u32>) -> Result<Value, Error> {
+        fn to_result<I: ExactSizeIterator<Item = u32> + Send + Sync + Clone + 'static>(
+            i: I,
+        ) -> Result<Value, Error> {
+            if i.len() > 100000 {
                 Err(Error::new(
                     ErrorKind::InvalidOperation,
                     "range has too many elements",
                 ))
             } else {
-                Ok(i.collect())
+                Ok(Value::make_iterable(move || i.clone()))
             }
         }
 
         let rng = match upper {
             Some(upper) => lower..upper,
             None => 0..lower,
         };
@@ -284,34 +320,102 @@
     ///
     /// ```jinja
     /// <script>const CONFIG = {{ dict(
     ///   DEBUG=true,
     ///   API_URL_PREFIX="/api"
     /// )|tojson }};</script>
     /// ```
+    ///
+    /// Additionally this can be used to merge objects by passing extra keyword
+    /// arguments:
+    ///
+    /// ```jinja
+    /// {% set new_dict = dict(old_dict, extra_value=2) %}
+    /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
-    pub fn dict(value: Value) -> Result<Value, Error> {
-        match value.0 {
-            ValueRepr::Undefined => Ok(Value::from(BTreeMap::<bool, Value>::new())),
-            ValueRepr::Map(map, _) => Ok(Value(ValueRepr::Map(map, MapType::Normal))),
-            _ => Err(Error::from(ErrorKind::InvalidOperation)),
+    pub fn dict(value: Option<Value>, update_with: crate::value::Kwargs) -> Result<Value, Error> {
+        let mut rv = match value {
+            None => ValueMap::default(),
+            Some(value) => match value.0 {
+                ValueRepr::Undefined => ValueMap::default(),
+                ValueRepr::Object(obj) if obj.repr() == ObjectRepr::Map => {
+                    obj.try_iter_pairs().into_iter().flatten().collect()
+                }
+                _ => return Err(Error::from(ErrorKind::InvalidOperation)),
+            },
+        };
+
+        if update_with.values.is_true() {
+            rv.extend(
+                update_with
+                    .values
+                    .iter()
+                    .map(|(k, v)| (k.clone(), v.clone())),
+            );
         }
+
+        Ok(Value::from_object(rv))
     }
 
-    /// Outputs the current context stringified.
+    /// Outputs the current context or the arguments stringified.
     ///
     /// This is a useful function to quickly figure out the state of affairs
     /// in a template.  It emits a stringified debug dump of the current
     /// engine state including the layers of the context, the current block
-    /// and auto escaping setting.
+    /// and auto escaping setting.  The exact output is not defined and might
+    /// change from one version of Jinja2 to the next.
     ///
     /// ```jinja
     /// <pre>{{ debug() }}</pre>
+    /// <pre>{{ debug(variable1, variable2) }}</pre>
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
-    pub fn debug(state: &State) -> String {
-        format!("{state:#?}")
+    pub fn debug(state: &State, args: Rest<Value>) -> String {
+        if args.is_empty() {
+            format!("{state:#?}")
+        } else if args.len() == 1 {
+            format!("{:#?}", args.0[0])
+        } else {
+            format!("{:#?}", &args.0[..])
+        }
+    }
+
+    /// Creates a new container that allows attribute assignment using the `{% set %}` tag.
+    ///
+    /// ```jinja
+    /// {% set ns = namespace() %}
+    /// {% set ns.foo = 'bar' %}
+    /// ```
+    ///
+    /// The main purpose of this is to allow carrying a value from within a loop body
+    /// to an outer scope. Initial values can be provided as a dict, as keyword arguments,
+    /// or both (same behavior as [`dict`]).
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn namespace(defaults: Option<Value>) -> Result<Value, Error> {
+        let ns = crate::value::namespace_object::Namespace::default();
+        if let Some(defaults) = defaults {
+            if let Some(pairs) = defaults
+                .as_object()
+                .filter(|x| matches!(x.repr(), ObjectRepr::Map))
+                .and_then(|x| x.try_iter_pairs())
+            {
+                for (key, value) in pairs {
+                    if let Some(key) = key.as_str() {
+                        ns.set_value(key, value);
+                    }
+                }
+            } else {
+                return Err(Error::new(
+                    ErrorKind::InvalidOperation,
+                    format!(
+                        "expected object or keyword arguments, got {}",
+                        defaults.kind()
+                    ),
+                ));
+            }
+        }
+        Ok(Value::from_object(ns))
     }
 }
 
 #[cfg(feature = "builtins")]
 pub use self::builtins::*;
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/lib.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 //! - [`Environment`]: the main API entry point.  Teaches you how to configure the environment.
 //! - [`Template`]: the template object API.  Shows you how templates can be rendered.
 //! - [`syntax`]: provides documentation of the template engine syntax.
 //! - [`filters`]: teaches you how to write custom filters and to see the list of built-in filters.
 //! - [`tests`]: teaches you how to write custom test functions and to see the list of built-in tests.
 //! - [`functions`]: teaches how to write custom functions and to see the list of built-in functions.
 //! - For auto reloading use the [`minijinja-autoreload`](https://docs.rs/minijinja-autoreload) crate.
+//! - For simpler embedding of templates use the [`minijinja-embed`](https://docs.rs/minijinja-embed) crate.
 //!
 //! Additionally there is an [list of examples](https://github.com/mitsuhiko/minijinja/tree/main/examples)
 //! with many different small example programs on GitHub to explore.
 //!
 //! # Error Handling
 //!
 //! MiniJinja tries to give you good errors out of the box.  However if you use includes or
@@ -142,25 +143,28 @@
 //!   - `multi_template`: when removed the templates related to imports and extends
 //!     are removed (`{% from %}`, `{% import %}`, `{% include %}`, and `{% extends %}`
 //!     as well as `{% block %}`).
 //!   - `adjacent_loop_items`: when removed the `previtem` and `nextitem` attributes of
 //!     the `loop` object no longer exist.  Removing this feature can provide faster
 //!     template execution when a lot of loops are involved.
 //!   - `unicode`: when added unicode identifiers are supported and the `sort`
-//!     filter's case insensitive comparising changes to using unicode and not
+//!     filter's case insensitive comparison changes to using unicode and not
 //!     ASCII rules.  Without this features only ASCII identifiers can be used
 //!     for variable names and attributes.
 //!
 //! - **Rust Functionality:**
 //!
 //!   - `debug`: if this feature is removed some debug functionality of the engine is
 //!     removed as well.  This mainly affects the quality of error reporting.
 //!   - `deserialization`: when removed this disables deserialization support for
-//!     the [`Value`](crate::value::Value) type, removes the `ViaDeserialize`
-//!     type and the error type no longer implements `serde::de::Error`.
+//!     the [`Value`] type, removes the `ViaDeserialize` type and the error type
+//!     no longer implements `serde::de::Error`.
+//!   - `std_collections`: if this feature is removed some [`Object`](crate::value::Object)
+//!     implementations for standard library collections are removed.  Only the
+//!     ones needed for the engine to function itself are retained.
 //!
 //! There are some additional features that provide extra functionality:
 //!
 //! - `fuel`: enables the `fuel` feature which makes the engine track fuel consumption which
 //!   can be used to better protect against expensive templates.
 //! - `loader`: enables owned and dynamic template loading of templates.
 //! - `custom_syntax`: when this feature is enabled, custom delimiters are supported by
@@ -169,27 +173,37 @@
 //!   which preserves the original order of maps and structs.
 //! - `json`: When enabled the `tojson` filter is added as builtin filter as well as
 //!   the ability to auto escape via `AutoEscape::Json`.
 //! - `urlencode`: When enabled the `urlencode` filter is added as builtin filter.
 //!
 //! Performance and memory related features:
 //!
+//! - `stacker`: enables automatic stack growth which permits much larger levels of recursion
+//!   at runtime.  This does not affect the maximum recursion at parsing time which is always
+//!   limited.
 //! - `speedups`: enables all speedups, in particular it turns on the `v_htmlescape` dependency
-//!   for faster HTML escapling.
+//!   for faster HTML escaping.
 //! - `key_interning`: if this feature is enabled the automatic string interning in
 //!   the value type is enabled.  This feature used to be turned on by default but
 //!   has negative performance effects in newer versions of MiniJinja since a lot of
 //!   the previous uses of key interning are no longer needed.  Enabling it however
 //!   cuts down on memory usage slightly in certain scenarios by interning all string
 //!   keys used in dynamic map values.
 //!
+//! Internals:
+//!
+//! - `unstable_machinery`: exposes an unstable internal API (no semver guarantees) to parse
+//!   templates and interact with the engine internals.  If you need this functionality, please
+//!   leave some feedback on GitHub.
+//!
 //! </details>
 #![allow(clippy::cognitive_complexity)]
 #![allow(clippy::get_first)]
 #![allow(clippy::default_constructed_unit_structs)]
+#![allow(where_clauses_object_safety)]
 #![cfg_attr(docsrs, feature(doc_cfg))]
 #![deny(missing_docs)]
 #![doc(html_logo_url = "https://github.com/mitsuhiko/minijinja/raw/main/artwork/logo-square.png")]
 
 #[macro_use]
 mod macros;
 
@@ -211,34 +225,28 @@
 
 #[cfg(feature = "loader")]
 mod loader;
 
 #[cfg(feature = "loader")]
 pub use loader::path_loader;
 
-#[cfg(feature = "custom_syntax")]
-mod custom_syntax;
-
 #[cfg(feature = "debug")]
 mod debug;
 
 pub use self::defaults::{default_auto_escape_callback, escape_formatter};
 pub use self::environment::Environment;
 pub use self::error::{Error, ErrorKind};
 pub use self::expression::Expression;
 pub use self::output::Output;
 pub use self::template::Template;
 pub use self::utils::{AutoEscape, HtmlEscape, UndefinedBehavior};
 
 /// Re-export for convenience.
 pub use self::value::Value;
 
-#[cfg(feature = "custom_syntax")]
-pub use self::custom_syntax::Syntax;
-
 pub use self::macros::__context;
 pub use self::vm::State;
 
 /// This module gives access to the low level machinery.
 ///
 /// This module is only provided by the `unstable_machinery` feature and does not
 /// have a stable interface.  It mostly exists for internal testing purposes and
@@ -246,23 +254,23 @@
 #[cfg(feature = "unstable_machinery")]
 #[cfg_attr(docsrs, doc(cfg(feature = "unstable_machinery")))]
 pub mod machinery {
     #![allow(missing_docs)]
     pub use crate::compiler::ast;
     pub use crate::compiler::codegen::CodeGenerator;
     pub use crate::compiler::instructions::{Instruction, Instructions};
-    pub use crate::compiler::lexer::{tokenize, SyntaxConfig};
-    pub use crate::compiler::parser::{parse, parse_with_syntax};
+    pub use crate::compiler::lexer::{tokenize, Tokenizer, WhitespaceConfig};
+    pub use crate::compiler::parser::{parse, parse_expr};
     pub use crate::compiler::tokens::{Span, Token};
-    pub use crate::template::CompiledTemplate;
+    pub use crate::template::{CompiledTemplate, TemplateConfig};
     pub use crate::vm::Vm;
 
     use crate::Output;
 
-    /// Returns a reference to a [`CompiledTemplate`] from a [`Template`].
+    /// Returns a reference to a [`CompiledTemplate`] from a [`Template`](crate::Template).
     pub fn get_compiled_template<'x, 'env>(
         tmpl: &'x crate::Template<'env, 'env>,
     ) -> &'x CompiledTemplate<'env> {
         &tmpl.compiled
     }
 
     /// Creates an [`Output`] that writes into a string.
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/loader.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/loader.rs`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 use std::path::Path;
 use std::path::PathBuf;
 use std::sync::Arc;
 
 use memo_map::MemoMap;
 use self_cell::self_cell;
 
-use crate::compiler::lexer::SyntaxConfig;
+use crate::compiler::instructions::Instructions;
 use crate::error::{Error, ErrorKind};
 use crate::template::CompiledTemplate;
+use crate::template::TemplateConfig;
 
 type LoadFunc = dyn for<'a> Fn(&'a str) -> Result<Option<String>, Error> + Send + Sync;
 
 /// Internal utility for dynamic template loading.
 ///
 /// Because an [`Environment`](crate::Environment) holds a reference to the
 /// source lifetime it borrows templates from, it becomes very inconvenient when
 /// it is shared. This object provides a solution for such cases. First templates
 /// are loaded into the source to decouple the lifetimes from the environment.
-#[derive(Clone, Default)]
+#[derive(Clone)]
 pub(crate) struct LoaderStore<'source> {
-    pub syntax_config: SyntaxConfig,
-    pub keep_trailing_newline: bool,
+    pub template_config: TemplateConfig,
     loader: Option<Arc<LoadFunc>>,
     owned_templates: MemoMap<Arc<str>, Arc<LoadedTemplate>>,
     borrowed_templates: BTreeMap<&'source str, Arc<CompiledTemplate<'source>>>,
 }
 
 impl<'source> fmt::Debug for LoaderStore<'source> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
@@ -50,21 +50,38 @@
     struct LoadedTemplate {
         owner: (Arc<str>, Box<str>),
         #[covariant]
         dependent: CompiledTemplate,
     }
 }
 
+self_cell! {
+    pub(crate) struct OwnedInstructions {
+        owner: Box<str>,
+        #[covariant]
+        dependent: Instructions,
+    }
+}
+
 impl fmt::Debug for LoadedTemplate {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         fmt::Debug::fmt(&self.borrow_dependent(), f)
     }
 }
 
 impl<'source> LoaderStore<'source> {
+    pub fn new(template_config: TemplateConfig) -> LoaderStore<'source> {
+        LoaderStore {
+            template_config,
+            loader: None,
+            owned_templates: MemoMap::default(),
+            borrowed_templates: BTreeMap::default(),
+        }
+    }
+
     pub fn insert(&mut self, name: &'source str, source: &'source str) -> Result<(), Error> {
         self.insert_cow(Cow::Borrowed(name), Cow::Borrowed(source))
     }
 
     pub fn insert_cow(
         &mut self,
         name: Cow<'source, str>,
@@ -74,16 +91,15 @@
             (Cow::Borrowed(source), Cow::Borrowed(name)) => {
                 self.owned_templates.remove(name);
                 self.borrowed_templates.insert(
                     name,
                     Arc::new(ok!(CompiledTemplate::new(
                         name,
                         source,
-                        self.syntax_config.clone(),
-                        self.keep_trailing_newline
+                        &self.template_config
                     ))),
                 );
             }
             (source, name) => {
                 self.borrowed_templates.remove(&name as &str);
                 let name: Arc<str> = name.into();
                 self.owned_templates.replace(
@@ -135,24 +151,33 @@
         &self,
         name: Arc<str>,
         source: String,
     ) -> Result<Arc<LoadedTemplate>, Error> {
         LoadedTemplate::try_new(
             (name, source.into_boxed_str()),
             |(name, source)| -> Result<_, Error> {
-                CompiledTemplate::new(
-                    name,
-                    source,
-                    self.syntax_config.clone(),
-                    self.keep_trailing_newline,
-                )
+                CompiledTemplate::new(name, source, &self.template_config)
             },
         )
         .map(Arc::new)
     }
+
+    pub fn iter(&self) -> impl Iterator<Item = (&str, &CompiledTemplate<'_>)> {
+        let borrowed = self
+            .borrowed_templates
+            .iter()
+            .map(|(name, template)| (*name, &**template));
+
+        let owned = self
+            .owned_templates
+            .iter()
+            .map(|(name, template)| (&**name, template.borrow_dependent()));
+
+        borrowed.chain(owned)
+    }
 }
 
 /// Safely joins two paths.
 pub fn safe_join(base: &Path, template: &str) -> Option<PathBuf> {
     let mut rv = base.to_path_buf();
     for segment in template.split('/') {
         if segment.starts_with('.') || segment.contains('\\') {
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/macros.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/macros.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,37 +20,36 @@
     };
 }
 
 /// Hidden utility module for the [`context!`](crate::context!) macro.
 #[doc(hidden)]
 pub mod __context {
     pub use crate::value::merge_object::MergeObject;
-    use crate::value::{KeyRef, MapType, Value, ValueMap, ValueRepr};
+    use crate::value::{Value, ValueMap};
     use crate::Environment;
     use std::rc::Rc;
-    use std::sync::Arc;
 
     #[inline(always)]
     pub fn value_optimization() -> impl Drop {
         crate::value::value_optimization()
     }
 
     #[inline(always)]
     pub fn make() -> ValueMap {
         ValueMap::default()
     }
 
     #[inline(always)]
     pub fn add(ctx: &mut ValueMap, key: &'static str, value: Value) {
-        ctx.insert(KeyRef::Str(key), value);
+        ctx.insert(key.into(), value);
     }
 
     #[inline(always)]
     pub fn build(ctx: ValueMap) -> Value {
-        ValueRepr::Map(Arc::new(ctx), MapType::Normal).into()
+        Value::from_object(ctx)
     }
 
     pub fn thread_local_env() -> Rc<Environment<'static>> {
         thread_local! {
             static ENV: Rc<Environment<'static>> = Rc::new(Environment::new());
         }
         ENV.with(|x| x.clone())
@@ -113,15 +112,15 @@
 ///         b => "B"
 ///     }
 /// };
 /// ```
 ///
 /// The merge works with an value, not just values created by the `context!`
 /// macro and is performed lazy.  This means it also works with dynamic
-/// [`StructObject`](crate::value::StructObject)s.
+/// [`Object`](crate::value::Object)s.
 #[macro_export]
 macro_rules! context {
     () => {
         $crate::__context::build($crate::__context::make())
     };
     (
         $($key:ident $(=> $value:expr)?),*
@@ -137,40 +136,40 @@
         $(
             merged_ctx.push($crate::value::Value::from($ctx));
         )*;
         if merged_ctx.is_empty() {
             ctx
         } else {
             merged_ctx.insert(0, ctx);
-            $crate::value::Value::from_struct_object($crate::__context::MergeObject(merged_ctx))
+            $crate::value::Value::from_object($crate::__context::MergeObject(merged_ctx))
         }
     }};
     (
         $(.. $ctx:expr),* $(,)?
     ) => {{
         let _guard = $crate::__context::value_optimization();
         let mut ctx = ::std::vec::Vec::new();
         $(
             ctx.push($crate::value::Value::from($ctx));
         )*;
-        $crate::value::Value::from_struct_object($crate::__context::MergeObject(ctx))
+        $crate::value::Value::from_object($crate::__context::MergeObject(ctx))
     }};
 }
 
 #[macro_export]
 #[doc(hidden)]
 macro_rules! __context_pair {
     ($ctx:ident, $key:ident) => {{
         $crate::__context_pair!($ctx, $key => $key);
     }};
     ($ctx:ident, $key:ident => $value:expr) => {
         $crate::__context::add(
             &mut $ctx,
             stringify!($key),
-            $crate::value::Value::from_serializable(&$value),
+            $crate::value::Value::from_serialize(&$value),
         );
     };
 }
 
 /// An utility macro to create arguments for function calls.
 ///
 /// This creates a slice of values on the stack which can be
@@ -189,15 +188,15 @@
 /// # let env = Environment::default();
 /// # let state = &env.empty_state();
 /// # let value = Value::from(());
 /// value.call(state, args!(1, 2, foo => "bar"));
 /// ```
 ///
 /// Note that this like [`context!`](crate::context) goes through
-/// [`Value::from_serializable`](crate::value::Value::from_serializable).
+/// [`Value::from_serialize`](crate::value::Value::from_serialize).
 #[macro_export]
 macro_rules! args {
     () => { &[][..] as &[$crate::value::Value] };
     ($($arg:tt)*) => { $crate::__args_helper!(branch [[$($arg)*]], [$($arg)*]) };
 }
 
 /// Utility macro for `args!`
@@ -231,25 +230,25 @@
         &(&{args})[..]
     }};
 
     // Peels a single argument from the arguments and stuffs them into
     // `$args` or `$kwargs` depending on type.
     (peel $args:ident, $kwargs:ident, $has_kwargs:ident, []) => {};
     (peel $args:ident, $kwargs:ident, $has_kwargs:ident, [$name:ident => $expr:expr]) => {
-        $kwargs.push((stringify!($name), $crate::value::Value::from_serializable(&$expr)));
+        $kwargs.push((stringify!($name), $crate::value::Value::from_serialize(&$expr)));
     };
     (peel $args:ident, $kwargs:ident, $has_kwargs:ident, [$name:ident => $expr:expr, $($rest:tt)*]) => {
-        $kwargs.push((stringify!($name), $crate::value::Value::from_serializable(&$expr)));
+        $kwargs.push((stringify!($name), $crate::value::Value::from_serialize(&$expr)));
         $crate::__args_helper!(peel $args, $kwargs, true, [$($rest)*]);
     };
     (peel $args:ident, $kwargs:ident, false, [$expr:expr]) => {
-        $args.push($crate::value::Value::from_serializable(&$expr));
+        $args.push($crate::value::Value::from_serialize(&$expr));
     };
     (peel $args:ident, $kwargs:ident, false, [$expr:expr, $($rest:tt)*]) => {
-        $args.push($crate::value::Value::from_serializable(&$expr));
+        $args.push($crate::value::Value::from_serialize(&$expr));
         $crate::__args_helper!(peel $args, $kwargs, false, [$($rest)*]);
     };
 }
 
 /// A macro similar to [`format!`] but that uses MiniJinja for rendering.
 ///
 /// This can be used to quickly render a MiniJinja template into a string
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/output.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/output.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::ptr::addr_of_mut;
 use std::{fmt, io};
 
 use crate::error::{Error, ErrorKind};
 use crate::utils::AutoEscape;
 use crate::value::Value;
 
 /// How should output be captured?
@@ -120,15 +121,15 @@
 pub struct NullWriter;
 
 impl NullWriter {
     /// Returns a reference to the null writer.
     pub fn get_mut() -> &'static mut NullWriter {
         static mut NULL_WRITER: NullWriter = NullWriter;
         // SAFETY: this is safe as the null writer is a ZST
-        unsafe { &mut NULL_WRITER }
+        unsafe { &mut *addr_of_mut!(NULL_WRITER) }
     }
 }
 
 impl fmt::Write for NullWriter {
     #[inline]
     fn write_str(&mut self, _s: &str) -> fmt::Result {
         Ok(())
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/template.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/template.rs`

 * *Files 16% similar despite different names*

```diff
@@ -3,63 +3,82 @@
 use std::sync::Arc;
 use std::{fmt, io};
 
 use serde::Serialize;
 
 use crate::compiler::codegen::CodeGenerator;
 use crate::compiler::instructions::Instructions;
-use crate::compiler::lexer::SyntaxConfig;
+use crate::compiler::lexer::WhitespaceConfig;
 use crate::compiler::meta::find_undeclared;
-use crate::compiler::parser::parse_with_syntax;
+use crate::compiler::parser::parse;
 use crate::environment::Environment;
 use crate::error::{attach_basic_debug_info, Error};
 use crate::output::{Output, WriteWrapper};
+use crate::syntax::SyntaxConfig;
 use crate::utils::AutoEscape;
 use crate::value::{self, Value};
-use crate::vm::{prepare_blocks, State, Vm};
+use crate::vm::{prepare_blocks, Context, State, Vm};
+
+/// Callback for auto escape determination
+pub type AutoEscapeFunc = dyn Fn(&str) -> AutoEscape + Sync + Send;
+
+/// Internal struct that holds template loading level config values.
+#[derive(Clone)]
+pub struct TemplateConfig {
+    /// The syntax used for the template.
+    pub syntax_config: SyntaxConfig,
+    /// Controls whitespace behavior.
+    pub ws_config: WhitespaceConfig,
+    /// The callback that determines the initial auto escaping for templates.
+    pub default_auto_escape: Arc<AutoEscapeFunc>,
+}
+
+impl TemplateConfig {
+    pub(crate) fn new(default_auto_escape: Arc<AutoEscapeFunc>) -> TemplateConfig {
+        TemplateConfig {
+            syntax_config: SyntaxConfig::default(),
+            ws_config: WhitespaceConfig::default(),
+            default_auto_escape,
+        }
+    }
+}
 
 /// Represents a handle to a template.
 ///
 /// Templates are stored in the [`Environment`] as bytecode instructions.  With the
 /// [`Environment::get_template`] method that is looked up and returned in form of
 /// this handle.  Such a template can be cheaply copied as it only holds references.
 ///
 /// To render the [`render`](Template::render) method can be used.
 #[derive(Clone)]
 pub struct Template<'env: 'source, 'source> {
     env: &'env Environment<'env>,
     pub(crate) compiled: CompiledTemplateRef<'env, 'source>,
-    initial_auto_escape: AutoEscape,
 }
 
 impl<'env, 'source> fmt::Debug for Template<'env, 'source> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut ds = f.debug_struct("Template");
         ds.field("name", &self.name());
         #[cfg(feature = "internal_debug")]
         {
             ds.field("instructions", &self.compiled.instructions);
             ds.field("blocks", &self.compiled.blocks);
         }
-        ds.field("initial_auto_escape", &self.initial_auto_escape);
+        ds.field("initial_auto_escape", &self.compiled.initial_auto_escape);
         ds.finish()
     }
 }
 
 impl<'env, 'source> Template<'env, 'source> {
     pub(crate) fn new(
         env: &'env Environment<'env>,
         compiled: CompiledTemplateRef<'env, 'source>,
-        initial_auto_escape: AutoEscape,
     ) -> Template<'env, 'source> {
-        Template {
-            env,
-            compiled,
-            initial_auto_escape,
-        }
+        Template { env, compiled }
     }
 
     /// Returns the name of the template.
     pub fn name(&self) -> &str {
         self.compiled.instructions.name()
     }
 
@@ -73,16 +92,16 @@
     /// The provided value is used as the initial context for the template.  It
     /// can be any object that implements [`Serialize`](serde::Serialize).  You
     /// can either create your own struct and derive `Serialize` for it or the
     /// [`context!`](crate::context) macro can be used to create an ad-hoc context.
     ///
     /// For very large contexts and to avoid the overhead of serialization of
     /// potentially unused values, you might consider using a dynamic
-    /// [`StructObject`](crate::value::StructObject) as value.  For more
-    /// information see [Struct as Context](crate::value::StructObject#struct-as-context).
+    /// [`Object`](crate::value::Object) as value.  For more
+    /// information see [Map as Context](crate::value::Object#map-as-context).
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// # let mut env = Environment::new();
     /// # env.add_template("hello", "Hello {{ name }}!").unwrap();
     /// let tmpl = env.get_template("hello").unwrap();
     /// println!("{}", tmpl.render(context!(name => "John")).unwrap());
@@ -92,15 +111,15 @@
     /// combination with [`State::render_block`].
     ///
     /// **Note on values:** The [`Value`] type implements `Serialize` and can be
     /// efficiently passed to render.  It does not undergo actual serialization.
     pub fn render<S: Serialize>(&self, ctx: S) -> Result<String, Error> {
         // reduce total amount of code faling under mono morphization into
         // this function, and share the rest in _render.
-        self._render(Value::from_serializable(&ctx)).map(|x| x.0)
+        self._render(Value::from_serialize(&ctx)).map(|x| x.0)
     }
 
     /// Like [`render`](Self::render) but also return the evaluated [`State`].
     ///
     /// This can be used to inspect the [`State`] of the template post evaluation
     /// for instance to get fuel consumption numbers or to access globally set
     /// variables.
@@ -118,15 +137,15 @@
     /// efficiently passed to render.  It does not undergo actual serialization.
     pub fn render_and_return_state<S: Serialize>(
         &self,
         ctx: S,
     ) -> Result<(String, State<'_, 'env>), Error> {
         // reduce total amount of code faling under mono morphization into
         // this function, and share the rest in _render.
-        self._render(Value::from_serializable(&ctx))
+        self._render(Value::from_serialize(&ctx))
     }
 
     fn _render(&self, root: Value) -> Result<(String, State<'_, 'env>), Error> {
         let mut rv = String::with_capacity(self.compiled.buffer_size_hint);
         self._eval(root, &mut Output::with_string(&mut rv))
             .map(|(_, state)| (rv, state))
     }
@@ -152,54 +171,52 @@
     pub fn render_to_write<S: Serialize, W: io::Write>(
         &self,
         ctx: S,
         w: W,
     ) -> Result<State<'_, 'env>, Error> {
         let mut wrapper = WriteWrapper { w, err: None };
         self._eval(
-            Value::from_serializable(&ctx),
+            Value::from_serialize(&ctx),
             &mut Output::with_write(&mut wrapper),
         )
         .map(|(_, state)| state)
         .map_err(|err| wrapper.take_err(err))
     }
 
     /// Evaluates the template into a [`State`].
     ///
     /// This evaluates the template, discards the output and returns the final
     /// `State` for introspection.  From there global variables or blocks
     /// can be accessed.  What this does is quite similar to how the engine
-    /// interally works with tempaltes that are extended or imported from.
+    /// internally works with templates that are extended or imported from.
     ///
     /// ```
     /// # use minijinja::{Environment, context};
     /// # fn test() -> Result<(), minijinja::Error> {
     /// # let mut env = Environment::new();
-    /// # env.add_template("hello", "{% block hi %}Hello {{ name }}!{% endblock %}")?;
+    /// # env.add_template("hello", "")?;
     /// let tmpl = env.get_template("hello")?;
-    /// let rv = tmpl
-    ///     .eval_to_state(context!(name => "John"))?
-    ///     .render_block("hi")?;
-    /// println!("{}", rv);
+    /// let state = tmpl.eval_to_state(context!(name => "John"))?;
+    /// println!("{:?}", state.exports());
     /// # Ok(()) }
     /// ```
     ///
     /// If you also want to render, use [`render_and_return_state`](Self::render_and_return_state).
     ///
     /// For more information see [`State`].
     pub fn eval_to_state<S: Serialize>(&self, ctx: S) -> Result<State<'_, 'env>, Error> {
-        let root = Value::from_serializable(&ctx);
+        let root = Value::from_serialize(&ctx);
         let mut out = Output::null();
         let vm = Vm::new(self.env);
         let state = ok!(vm.eval(
             &self.compiled.instructions,
             root,
             &self.compiled.blocks,
             &mut out,
-            self.initial_auto_escape,
+            self.compiled.initial_auto_escape,
         ))
         .1;
         Ok(state)
     }
 
     fn _eval(
         &self,
@@ -207,15 +224,15 @@
         out: &mut Output,
     ) -> Result<(Option<Value>, State<'_, 'env>), Error> {
         Vm::new(self.env).eval(
             &self.compiled.instructions,
             root,
             &self.compiled.blocks,
             out,
-            self.initial_auto_escape,
+            self.compiled.initial_auto_escape,
         )
     }
 
     /// Returns a set of all undeclared variables in the template.
     ///
     /// This returns a set of all variables that might be looked up
     /// at runtime by the template.  Since this is runs a static
@@ -231,46 +248,47 @@
     /// let tmpl = env.get_template("x").unwrap();
     /// let undeclared = tmpl.undeclared_variables(false);
     /// // returns ["foo", "bar"]
     /// let undeclared = tmpl.undeclared_variables(true);
     /// // returns ["foo", "bar.baz"]
     /// ```
     pub fn undeclared_variables(&self, nested: bool) -> HashSet<String> {
-        match parse_with_syntax(
+        match parse(
             self.compiled.instructions.source(),
             self.name(),
-            self.compiled.syntax.clone(),
-            true,
+            self.compiled.syntax_config.clone(),
+            // TODO: this is not entirely great, but good enough for this use case.
+            Default::default(),
         ) {
             Ok(ast) => find_undeclared(&ast, nested),
             Err(_) => HashSet::new(),
         }
     }
 
     /// Creates an empty [`State`] for this template.
     ///
     /// It's very rare that you need to actually do this but it can be useful when
     /// testing values or working with macros or other callable objects from outside
     /// the template environment.
     pub fn new_state(&self) -> State<'_, 'env> {
         State::new(
             self.env,
-            Default::default(),
-            self.initial_auto_escape,
+            Context::new(self.env.recursion_limit()),
+            self.compiled.initial_auto_escape,
             &self.compiled.instructions,
             prepare_blocks(&self.compiled.blocks),
         )
     }
 
     /// Returns the instructions and blocks if the template is loaded from the
     /// environment.
     ///
     /// For templates loaded as string on the environment this API contract
     /// cannot be upheld because the template might not live long enough.  Under
-    /// normal cirumstances however such a template object would never make it
+    /// normal circumstances however such a template object would never make it
     /// to the callers of this API as this API is used for including or extending,
     /// both of which should only ever get access to a template from the environment
     /// which holds a borrowed ref.
     #[cfg(feature = "multi_template")]
     pub(crate) fn instructions_and_blocks(
         &self,
     ) -> Result<
@@ -288,15 +306,15 @@
             )),
         }
     }
 
     /// Returns the initial auto escape setting.
     #[cfg(feature = "multi_template")]
     pub(crate) fn initial_auto_escape(&self) -> AutoEscape {
-        self.initial_auto_escape
+        self.compiled.initial_auto_escape
     }
 }
 
 #[derive(Clone)]
 pub(crate) enum CompiledTemplateRef<'env: 'source, 'source> {
     Owned(Arc<CompiledTemplate<'source>>),
     Borrowed(&'env CompiledTemplate<'source>),
@@ -318,15 +336,17 @@
     /// The root instructions.
     pub instructions: Instructions<'source>,
     /// Block local instructions.
     pub blocks: BTreeMap<&'source str, Instructions<'source>>,
     /// Optional size hint for string rendering.
     pub buffer_size_hint: usize,
     /// The syntax config that created it.
-    pub syntax: SyntaxConfig,
+    pub syntax_config: SyntaxConfig,
+    /// The initial setting of auto escaping.
+    pub initial_auto_escape: AutoEscape,
 }
 
 impl<'env> fmt::Debug for CompiledTemplate<'env> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut ds = f.debug_struct("CompiledTemplate");
         #[cfg(feature = "internal_debug")]
         {
@@ -338,43 +358,39 @@
 }
 
 impl<'source> CompiledTemplate<'source> {
     /// Creates a compiled template from name and source using the given settings.
     pub fn new(
         name: &'source str,
         source: &'source str,
-        syntax: SyntaxConfig,
-        keep_trailing_newline: bool,
+        config: &TemplateConfig,
     ) -> Result<CompiledTemplate<'source>, Error> {
-        attach_basic_debug_info(
-            Self::_new_impl(name, source, syntax, keep_trailing_newline),
-            source,
-        )
+        attach_basic_debug_info(Self::_new_impl(name, source, config), source)
     }
 
     fn _new_impl(
         name: &'source str,
         source: &'source str,
-        syntax: SyntaxConfig,
-        keep_trailing_newline: bool,
+        config: &TemplateConfig,
     ) -> Result<CompiledTemplate<'source>, Error> {
         // the parser/compiler combination can create constants in which case
         // we can probably benefit from the value optimization a bit.
         let _guard = value::value_optimization();
-        let ast = ok!(parse_with_syntax(
+        let ast = ok!(parse(
             source,
             name,
-            syntax.clone(),
-            keep_trailing_newline
+            config.syntax_config.clone(),
+            config.ws_config
         ));
         let mut gen = CodeGenerator::new(name, source);
         gen.compile_stmt(&ast);
         let buffer_size_hint = gen.buffer_size_hint();
         let (instructions, blocks) = gen.finish();
         Ok(CompiledTemplate {
             instructions,
             blocks,
             buffer_size_hint,
-            syntax,
+            syntax_config: config.syntax_config.clone(),
+            initial_auto_escape: (config.default_auto_escape)(name),
         })
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/tests.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/tests.rs`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,14 @@
 }
 
 #[cfg(feature = "builtins")]
 mod builtins {
     use super::*;
 
     use std::borrow::Cow;
-    use std::convert::TryFrom;
 
     use crate::value::ValueKind;
 
     /// Checks if a value is odd.
     ///
     /// ```jinja
     /// {{ 41 is odd }} -> true
@@ -271,14 +270,42 @@
     /// {{ "42" is number }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn is_number(v: Value) -> bool {
         matches!(v.kind(), ValueKind::Number)
     }
 
+    /// Checks if this value is an integer.
+    ///
+    /// ```jinja
+    /// {{ 42 is integer }} -> true
+    /// {{ 42.0 is integer }} -> false
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn is_integer(v: Value) -> bool {
+        matches!(
+            v.0,
+            crate::value::ValueRepr::U64(_)
+                | crate::value::ValueRepr::I64(_)
+                | crate::value::ValueRepr::U128(_)
+                | crate::value::ValueRepr::I128(_)
+        )
+    }
+
+    /// Checks if this value is a float
+    ///
+    /// ```jinja
+    /// {{ 42 is float }} -> false
+    /// {{ 42.0 is float }} -> true
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn is_float(v: Value) -> bool {
+        matches!(v.0, crate::value::ValueRepr::F64(_))
+    }
+
     /// Checks if this value is a string.
     ///
     /// ```jinja
     /// {{ "42" is string }} -> true
     /// {{ 42 is string }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
@@ -293,14 +320,25 @@
     /// {{ 42 is sequence }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     pub fn is_sequence(v: Value) -> bool {
         matches!(v.kind(), ValueKind::Seq)
     }
 
+    /// Checks if this value can be iterated over.
+    ///
+    /// ```jinja
+    /// {{ [1, 2, 3] is iterable }} -> true
+    /// {{ 42 is iterable }} -> false
+    /// ```
+    #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
+    pub fn is_iterable(v: Value) -> bool {
+        v.try_iter().is_ok()
+    }
+
     /// Checks if this value is a mapping
     ///
     /// ```jinja
     /// {{ {"foo": "bar"} is mapping }} -> true
     /// {{ [1, 2, 3] is mapping }} -> false
     /// ```
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
@@ -432,18 +470,19 @@
     /// {{ 1 is in [1, 2, 3] }} -> true
     /// {{ [1, 2, 3]|select("in", [1, 2]) }} => [1, 2]
     /// ```
     ///
     /// This is useful when combined with [`select`](crate::filters::select).
     #[cfg_attr(docsrs, doc(cfg(feature = "builtins")))]
     #[cfg(feature = "builtins")]
-    pub fn is_in(value: &Value, other: &Value) -> bool {
-        crate::value::ops::contains(other, value)
+    pub fn is_in(state: &State, value: &Value, other: &Value) -> Result<bool, Error> {
+        ok!(state.undefined_behavior().assert_iterable(value));
+        Ok(crate::value::ops::contains(other, value)
             .map(|value| value.is_true())
-            .unwrap_or(false)
+            .unwrap_or(false))
     }
 
     /// Checks if a value is `true`.
     ///
     /// ```jinja
     /// {% if value is true %}...{% endif %}
     /// ```
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/utils.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::char::decode_utf16;
 use std::collections::BTreeMap;
 use std::fmt;
 use std::iter::{once, repeat};
 use std::str::Chars;
 
 use crate::error::{Error, ErrorKind};
-use crate::value::{OwnedValueIterator, StringType, Value, ValueKind, ValueRepr};
+use crate::value::{StringType, Value, ValueIter, ValueKind, ValueRepr};
 use crate::Output;
 
 /// internal marker to seal up some trait methods
 pub struct SealedMarker;
 
 pub fn memchr(haystack: &[u8], needle: u8) -> Option<usize> {
     haystack.iter().position(|&x| x == needle)
@@ -140,34 +140,45 @@
 impl UndefinedBehavior {
     /// Utility method used in the engine to determine what to do when an undefined is
     /// encountered.
     ///
     /// The flag indicates if this is the first or second level of undefined value.  If
     /// `parent_was_undefined` is set to `true`, the undefined was created by looking up
     /// a missing attribute on an undefined value.  If `false` the undefined was created by
-    /// looing up a missing attribute on a defined value.
+    /// looking up a missing attribute on a defined value.
     pub(crate) fn handle_undefined(self, parent_was_undefined: bool) -> Result<Value, Error> {
         match (self, parent_was_undefined) {
-            (UndefinedBehavior::Lenient, false) | (UndefinedBehavior::Chainable, _) => {
-                Ok(Value::UNDEFINED)
-            }
-            (UndefinedBehavior::Lenient, true) | (UndefinedBehavior::Strict, _) => {
+            (UndefinedBehavior::Lenient, false)
+            | (UndefinedBehavior::Strict, false)
+            | (UndefinedBehavior::Chainable, _) => Ok(Value::UNDEFINED),
+            (UndefinedBehavior::Lenient, true) | (UndefinedBehavior::Strict, true) => {
                 Err(Error::from(ErrorKind::UndefinedError))
             }
         }
     }
 
+    /// Utility method to check if something is true.
+    ///
+    /// This fails only for strict undefined values.
+    #[inline]
+    pub(crate) fn is_true(self, value: &Value) -> Result<bool, Error> {
+        if matches!(self, UndefinedBehavior::Strict) && value.is_undefined() {
+            Err(Error::from(ErrorKind::UndefinedError))
+        } else {
+            Ok(value.is_true())
+        }
+    }
+
     /// Tries to iterate over a value while handling the undefined value.
     ///
     /// If the value is undefined, then iteration fails if the behavior is set to strict,
     /// otherwise it succeeds with an empty iteration.  This is also internally used in the
     /// engine to convert values to lists.
-    pub(crate) fn try_iter(self, value: Value) -> Result<OwnedValueIterator, Error> {
-        self.assert_iterable(&value)
-            .and_then(|_| value.try_iter_owned())
+    pub(crate) fn try_iter(self, value: Value) -> Result<ValueIter, Error> {
+        self.assert_iterable(&value).and_then(|_| value.try_iter())
     }
 
     /// Are we strict on iteration?
     pub(crate) fn assert_iterable(self, value: &Value) -> Result<(), Error> {
         if matches!(self, UndefinedBehavior::Strict) && value.is_undefined() {
             Err(Error::from(ErrorKind::UndefinedError))
         } else {
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/argtypes.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/argtypes.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 use std::borrow::Cow;
 use std::cell::RefCell;
-use std::collections::{BTreeMap, HashMap, HashSet};
-use std::convert::TryFrom;
+use std::collections::HashSet;
 use std::ops::{Deref, DerefMut};
+use std::sync::Arc;
 
 use crate::error::{Error, ErrorKind};
 use crate::utils::UndefinedBehavior;
 use crate::value::{
-    Arc, KeyRef, MapType, Object, Packed, SeqObject, StringType, Value, ValueKind, ValueMap,
-    ValueRepr,
+    DynObject, ObjectRepr, Packed, SmallStr, StringType, Value, ValueKind, ValueMap, ValueRepr,
 };
 use crate::vm::State;
 
+use super::{Enumerator, Object};
+
 /// A utility trait that represents the return value of functions and filters.
 ///
 /// It's implemented for the following types:
 ///
-/// * `Rv` where `Rv` implements `Into<Value>`
+/// * `Rv` where `Rv` implements `Into<AnyMapObject>`
 /// * `Result<Rv, Error>` where `Rv` implements `Into<Value>`
 ///
 /// The equivalent for test functions is [`TestResult`](crate::tests::TestResult).
 pub trait FunctionResult {
     #[doc(hidden)]
     fn into_result(self) -> Result<Value, Error>;
 }
@@ -106,15 +107,15 @@
 /// * signed integers: [`i8`], [`i16`], [`i32`], [`i64`], [`i128`]
 /// * floats: [`f32`], [`f64`]
 /// * bool: [`bool`]
 /// * string: [`String`], [`&str`], `Cow<'_, str>`, [`char`]
 /// * bytes: [`&[u8]`][`slice`]
 /// * values: [`Value`], `&Value`
 /// * vectors: [`Vec<T>`]
-/// * sequences: [`&dyn SeqObject`](crate::value::SeqObject)
+/// * objects: [`DynObject`]
 /// * serde deserializable: [`ViaDeserialize<T>`](crate::value::deserialize::ViaDeserialize)
 /// * keyword arguments: [`Kwargs`]
 /// * leftover arguments: [`Rest<T>`]
 ///
 /// The type is also implemented for optional values (`Option<T>`) which is used
 /// to encode optional parameters to filters, functions or tests.  Additionally
 /// it's implemented for [`Rest<T>`] which is used to encode the remaining arguments
@@ -266,15 +267,24 @@
         ValueRepr::Bytes(Arc::new(val.into())).into()
     }
 }
 
 impl<'a> From<&'a str> for Value {
     #[inline(always)]
     fn from(val: &'a str) -> Self {
-        ValueRepr::String(Arc::from(val.to_string()), StringType::Normal).into()
+        SmallStr::try_new(val)
+            .map(|small_str| Value(ValueRepr::SmallStr(small_str)))
+            .unwrap_or_else(|| Value::from(val.to_string()))
+    }
+}
+
+impl<'a> From<&'a String> for Value {
+    #[inline(always)]
+    fn from(val: &'a String) -> Self {
+        Value::from(val.as_str())
     }
 }
 
 impl From<String> for Value {
     #[inline(always)]
     fn from(val: String) -> Self {
         ValueRepr::String(Arc::from(val), StringType::Normal).into()
@@ -287,64 +297,40 @@
         match val {
             Cow::Borrowed(x) => x.into(),
             Cow::Owned(x) => x.into(),
         }
     }
 }
 
+impl From<Arc<str>> for Value {
+    fn from(value: Arc<str>) -> Self {
+        Value(ValueRepr::String(value, StringType::Normal))
+    }
+}
+
 impl From<()> for Value {
     #[inline(always)]
     fn from(_: ()) -> Self {
         ValueRepr::None.into()
     }
 }
 
 impl<V: Into<Value>> FromIterator<V> for Value {
     fn from_iter<T: IntoIterator<Item = V>>(iter: T) -> Self {
-        ValueRepr::Seq(Arc::new(iter.into_iter().map(Into::into).collect())).into()
+        Value::from_object(iter.into_iter().map(Into::into).collect::<Vec<Value>>())
     }
 }
 
 impl<K: Into<Value>, V: Into<Value>> FromIterator<(K, V)> for Value {
     fn from_iter<T: IntoIterator<Item = (K, V)>>(iter: T) -> Self {
-        let map = iter
-            .into_iter()
-            .map(|(k, v)| (KeyRef::Value(k.into()), v.into()))
-            .collect();
-        ValueRepr::Map(Arc::new(map), MapType::Normal).into()
-    }
-}
-
-impl<K: Into<Value>, V: Into<Value>> From<BTreeMap<K, V>> for Value {
-    fn from(val: BTreeMap<K, V>) -> Self {
-        val.into_iter().map(|(k, v)| (k.into(), v.into())).collect()
-    }
-}
-
-impl<K: Into<Value>, V: Into<Value>> From<HashMap<K, V>> for Value {
-    fn from(val: HashMap<K, V>) -> Self {
-        val.into_iter().map(|(k, v)| (k.into(), v.into())).collect()
-    }
-}
-
-impl<T: Into<Value>> From<Vec<T>> for Value {
-    fn from(val: Vec<T>) -> Self {
-        val.into_iter().map(|v| v.into()).collect()
-    }
-}
-
-impl<T: Object> From<Arc<T>> for Value {
-    fn from(object: Arc<T>) -> Self {
-        Value::from(object as Arc<dyn Object>)
-    }
-}
-
-impl From<Arc<str>> for Value {
-    fn from(value: Arc<str>) -> Self {
-        Value(ValueRepr::String(value, StringType::Normal))
+        Value::from_object(
+            iter.into_iter()
+                .map(|(k, v)| (k.into(), v.into()))
+                .collect::<ValueMap>(),
+        )
     }
 }
 
 macro_rules! value_from {
     ($src:ty, $dst:ident) => {
         impl From<$src> for Value {
             #[inline(always)]
@@ -368,15 +354,16 @@
         ValueRepr::U128(Packed(val)).into()
     }
 }
 
 impl From<char> for Value {
     #[inline(always)]
     fn from(val: char) -> Self {
-        ValueRepr::String(Arc::from(val.to_string()), StringType::Normal).into()
+        let mut buf = [0u8; 4];
+        ValueRepr::SmallStr(SmallStr::try_new(val.encode_utf8(&mut buf)).unwrap()).into()
     }
 }
 
 value_from!(bool, Bool);
 value_from!(u8, U64);
 value_from!(u16, U64);
 value_from!(u32, U64);
@@ -384,16 +371,15 @@
 value_from!(i8, I64);
 value_from!(i16, I64);
 value_from!(i32, I64);
 value_from!(i64, I64);
 value_from!(f32, F64);
 value_from!(f64, F64);
 value_from!(Arc<Vec<u8>>, Bytes);
-value_from!(Arc<Vec<Value>>, Seq);
-value_from!(Arc<dyn Object>, Dynamic);
+value_from!(DynObject, Object);
 
 fn unsupported_conversion(kind: ValueKind, target: &str) -> Error {
     Error::new(
         ErrorKind::InvalidOperation,
         format!("cannot convert {kind} to {target}"),
     )
 }
@@ -461,14 +447,20 @@
 primitive_try_from!(char, {
     ValueRepr::String(ref val, _) => {
         let mut char_iter = val.chars();
         ok!(char_iter.next().filter(|_| char_iter.next().is_none()).ok_or_else(|| {
             unsupported_conversion(ValueKind::String, "non single character string")
         }))
     },
+    ValueRepr::SmallStr(ref val) => {
+        let mut char_iter = val.as_str().chars();
+        ok!(char_iter.next().filter(|_| char_iter.next().is_none()).ok_or_else(|| {
+            unsupported_conversion(ValueKind::String, "non single character string")
+        }))
+    },
 });
 primitive_try_from!(f32, {
     ValueRepr::U64(val) => val as f32,
     ValueRepr::I64(val) => val as f32,
     ValueRepr::U128(val) => val.0 as f32,
     ValueRepr::I128(val) => val.0 as f32,
     ValueRepr::F64(val) => val as f32,
@@ -496,14 +488,15 @@
 
 impl TryFrom<Value> for Arc<str> {
     type Error = Error;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value.0 {
             ValueRepr::String(x, _) => Ok(x),
+            ValueRepr::SmallStr(x) => Ok(Arc::from(x.as_str())),
             _ => Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "value is not a string",
             )),
         }
     }
 }
@@ -528,27 +521,14 @@
                 .as_bytes()
                 .ok_or_else(|| Error::new(ErrorKind::InvalidOperation, "value is not in bytes")),
             None => Err(Error::from(ErrorKind::MissingArgument)),
         }
     }
 }
 
-impl<'a> ArgType<'a> for &dyn SeqObject {
-    type Output = &'a dyn SeqObject;
-
-    fn from_value(value: Option<&'a Value>) -> Result<Self::Output, Error> {
-        match value {
-            Some(value) => value
-                .as_seq()
-                .ok_or_else(|| Error::new(ErrorKind::InvalidOperation, "value is not a sequence")),
-            None => Err(Error::from(ErrorKind::MissingArgument)),
-        }
-    }
-}
-
 impl<'a, T: ArgType<'a>> ArgType<'a> for Option<T> {
     type Output = Option<T::Output>;
 
     fn from_value(value: Option<&'a Value>) -> Result<Self::Output, Error> {
         match value {
             Some(value) => {
                 if value.is_undefined() || value.is_none() {
@@ -574,14 +554,15 @@
     type Output = Cow<'a, str>;
 
     #[inline(always)]
     fn from_value(value: Option<&'a Value>) -> Result<Cow<'a, str>, Error> {
         match value {
             Some(value) => Ok(match value.0 {
                 ValueRepr::String(ref s, _) => Cow::Borrowed(s as &str),
+                ValueRepr::SmallStr(ref s) => Cow::Borrowed(s.as_str()),
                 _ => Cow::Owned(value.to_string()),
             }),
             None => Err(Error::from(ErrorKind::MissingArgument)),
         }
     }
 }
 
@@ -733,66 +714,105 @@
 ///     let (args, kwargs) = from_args::<(&[Value], Kwargs)>(&args)?;
 ///     // do something with args and kwargs
 /// # todo!()
 /// }
 /// ```
 #[derive(Debug, Clone)]
 pub struct Kwargs {
-    values: Arc<ValueMap>,
+    pub(crate) values: Arc<KwargsValues>,
     used: RefCell<HashSet<String>>,
 }
 
+#[repr(transparent)]
+#[derive(Default, Debug)]
+pub(crate) struct KwargsValues(ValueMap);
+
+impl Deref for KwargsValues {
+    type Target = ValueMap;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0
+    }
+}
+
+impl KwargsValues {
+    fn as_value_map<'a>(self: &'a Arc<Self>) -> &'a Arc<ValueMap> {
+        // SAFETY: this is safe because of repr(transparent)
+        unsafe { std::mem::transmute(self) }
+    }
+}
+
+impl Object for KwargsValues {
+    fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+        self.as_value_map().get_value(key)
+    }
+
+    fn enumerate(self: &Arc<Self>) -> Enumerator {
+        self.as_value_map().enumerate()
+    }
+}
+
 impl<'a> ArgType<'a> for Kwargs {
     type Output = Self;
 
     fn from_value(value: Option<&'a Value>) -> Result<Self, Error> {
         match value {
             Some(value) => {
-                if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
-                    Ok(Kwargs::new(map.clone()))
-                } else {
-                    Err(Error::from(ErrorKind::MissingArgument))
-                }
+                Kwargs::extract(value).ok_or_else(|| Error::from(ErrorKind::MissingArgument))
             }
             None => Ok(Kwargs::new(Default::default())),
         }
     }
 
     fn from_state_and_values(
         _state: Option<&'a State>,
         values: &'a [Value],
         offset: usize,
     ) -> Result<(Self, usize), Error> {
-        if let Some(value) = values.get(offset) {
-            if let ValueRepr::Map(ref map, MapType::Kwargs) = value.0 {
-                return Ok((Kwargs::new(map.clone()), 1));
-            }
-        }
-        Ok((Kwargs::new(Default::default()), 0))
+        let args = values
+            .get(offset)
+            .and_then(Kwargs::extract)
+            .map(|kwargs| (kwargs, 1))
+            .unwrap_or_else(|| (Kwargs::new(Default::default()), 0));
+
+        Ok(args)
     }
 
     fn is_trailing() -> bool {
         true
     }
 }
 
 impl Kwargs {
-    fn new(map: Arc<ValueMap>) -> Kwargs {
+    fn new(map: Arc<KwargsValues>) -> Kwargs {
         Kwargs {
             values: map,
             used: RefCell::new(HashSet::new()),
         }
     }
 
+    /// Given a value, extracts the kwargs if there are any.
+    pub(crate) fn extract(value: &Value) -> Option<Kwargs> {
+        value
+            .as_object()
+            .and_then(|x| x.downcast::<KwargsValues>())
+            .map(Kwargs::new)
+    }
+
+    /// Wraps a value map into kwargs.
+    pub(crate) fn wrap(map: ValueMap) -> Value {
+        Value::from_object(KwargsValues(map))
+    }
+
     /// Get a single argument from the kwargs but don't mark it as used.
     pub fn peek<'a, T>(&'a self, key: &'a str) -> Result<T, Error>
     where
         T: ArgType<'a, Output = T>,
     {
-        T::from_value(self.values.get(&KeyRef::Str(key))).map_err(|mut err| {
+        T::from_value(self.values.get(&Value::from(key))).map_err(|mut err| {
             if err.kind() == ErrorKind::MissingArgument && err.detail().is_none() {
                 err.set_detail(format!("missing keyword argument '{}'", key));
             }
             err
         })
     }
 
@@ -824,15 +844,15 @@
         let rv = ok!(self.peek::<T>(key));
         self.used.borrow_mut().insert(key.to_string());
         Ok(rv)
     }
 
     /// Checks if a keyword argument exists.
     pub fn has(&self, key: &str) -> bool {
-        self.values.contains_key(&KeyRef::Str(key))
+        self.values.contains_key(&Value::from(key))
     }
 
     /// Iterates over all passed keyword arguments.
     pub fn args(&self) -> impl Iterator<Item = &str> {
         self.values.iter().filter_map(|x| x.0.as_str())
     }
 
@@ -859,48 +879,46 @@
 }
 
 impl FromIterator<(String, Value)> for Kwargs {
     fn from_iter<T>(iter: T) -> Self
     where
         T: IntoIterator<Item = (String, Value)>,
     {
-        Kwargs::new(Arc::new(
-            iter.into_iter()
-                .map(|(k, v)| (KeyRef::Value(Value::from(k)), v))
-                .collect(),
-        ))
+        Kwargs::new(Arc::new(KwargsValues(
+            iter.into_iter().map(|(k, v)| (Value::from(k), v)).collect(),
+        )))
     }
 }
 
 impl<'a> FromIterator<(&'a str, Value)> for Kwargs {
     fn from_iter<T>(iter: T) -> Self
     where
         T: IntoIterator<Item = (&'a str, Value)>,
     {
-        Kwargs::new(Arc::new(
-            iter.into_iter()
-                .map(|(k, v)| (KeyRef::Value(Value::from(k)), v))
-                .collect(),
-        ))
+        Kwargs::new(Arc::new(KwargsValues(
+            iter.into_iter().map(|(k, v)| (Value::from(k), v)).collect(),
+        )))
     }
 }
 
 impl From<Kwargs> for Value {
     fn from(value: Kwargs) -> Self {
-        Value(ValueRepr::Map(value.values, MapType::Kwargs))
+        Value::from_dyn_object(value.values)
     }
 }
 
 impl TryFrom<Value> for Kwargs {
     type Error = Error;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value.0 {
             ValueRepr::Undefined => Ok(Kwargs::new(Default::default())),
-            ValueRepr::Map(ref val, MapType::Kwargs) => Ok(Kwargs::new(val.clone())),
+            ValueRepr::Object(_) => {
+                Kwargs::extract(&value).ok_or_else(|| Error::from(ErrorKind::InvalidOperation))
+            }
             _ => Err(Error::from(ErrorKind::InvalidOperation)),
         }
     }
 }
 
 impl<'a> ArgType<'a> for Value {
     type Output = Self;
@@ -942,50 +960,86 @@
 impl<'a, T: ArgType<'a, Output = T>> ArgType<'a> for Vec<T> {
     type Output = Vec<T>;
 
     fn from_value(value: Option<&'a Value>) -> Result<Self, Error> {
         match value {
             None => Ok(Vec::new()),
             Some(value) => {
-                let seq = ok!(value
-                    .as_seq()
-                    .ok_or_else(|| { Error::new(ErrorKind::InvalidOperation, "not a sequence") }));
+                let iter = ok!(value
+                    .as_object()
+                    .filter(|x| matches!(x.repr(), ObjectRepr::Seq | ObjectRepr::Iterable))
+                    .and_then(|x| x.try_iter())
+                    .ok_or_else(|| { Error::new(ErrorKind::InvalidOperation, "not iterable") }));
                 let mut rv = Vec::new();
-                for value in seq.iter() {
+                for value in iter {
                     rv.push(ok!(T::from_value_owned(value)));
                 }
                 Ok(rv)
             }
         }
     }
 
     fn from_value_owned(value: Value) -> Result<Self, Error> {
-        let seq = ok!(value
-            .as_seq()
-            .ok_or_else(|| { Error::new(ErrorKind::InvalidOperation, "not a sequence") }));
+        let iter = ok!(value
+            .as_object()
+            .filter(|x| matches!(x.repr(), ObjectRepr::Seq | ObjectRepr::Iterable))
+            .and_then(|x| x.try_iter())
+            .ok_or_else(|| { Error::new(ErrorKind::InvalidOperation, "not iterable") }));
         let mut rv = Vec::new();
-        for value in seq.iter() {
+        for value in iter {
             rv.push(ok!(T::from_value_owned(value)));
         }
         Ok(rv)
     }
 }
 
+impl<'a> ArgType<'a> for DynObject {
+    type Output = Self;
+
+    fn from_value(value: Option<&'a Value>) -> Result<Self, Error> {
+        value
+            .ok_or_else(|| Error::from(ErrorKind::MissingArgument))
+            .and_then(|v| Self::from_value_owned(v.clone()))
+    }
+
+    fn from_value_owned(value: Value) -> Result<Self, Error> {
+        value
+            .as_object()
+            .cloned()
+            .ok_or_else(|| Error::new(ErrorKind::InvalidOperation, "not an object"))
+    }
+}
+
 impl From<Value> for String {
     fn from(val: Value) -> Self {
         val.to_string()
     }
 }
 
 impl From<usize> for Value {
     fn from(val: usize) -> Self {
         Value::from(val as u64)
     }
 }
 
+impl From<isize> for Value {
+    fn from(val: isize) -> Self {
+        Value::from(val as i64)
+    }
+}
+
+impl<I: Into<Value>> From<Option<I>> for Value {
+    fn from(value: Option<I>) -> Self {
+        match value {
+            Some(value) => value.into(),
+            None => Value::from(()),
+        }
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_as_f64() {
         let v = Value::from(42u32);
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/deserialize.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/deserialize.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::ops::{Deref, DerefMut};
 
 use serde::de::{self, MapAccess, SeqAccess, Visitor};
 use serde::{forward_to_deserialize_any, Deserialize};
 
-use crate::value::{ArgType, KeyRef, MapType, Value, ValueKind, ValueMap, ValueRepr};
+use crate::value::{ArgType, ObjectRepr, Value, ValueKind, ValueMap, ValueRepr};
 use crate::{Error, ErrorKind};
 
 impl<'de> Deserialize<'de> for Value {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
     where
         D: serde::Deserializer<'de>,
     {
@@ -95,17 +95,17 @@
 
     fn visit_map<A>(self, mut map: A) -> Result<Value, A::Error>
     where
         A: MapAccess<'de>,
     {
         let mut rv = ValueMap::default();
         while let Some((k, v)) = ok!(map.next_entry()) {
-            rv.insert(KeyRef::Value(k), v);
+            rv.insert(k, v);
         }
-        Ok(Value(ValueRepr::Map(rv.into(), MapType::Normal)))
+        Ok(Value::from_object(rv))
     }
 }
 
 /// Utility type to deserialize an argument.
 ///
 /// This allows you to directly accept a type that implements [`Deserialize`] as an
 /// argument to a filter or test.  The type dereferences into the inner type and
@@ -173,37 +173,34 @@
             ValueRepr::Bool(v) => visitor.visit_bool(v),
             ValueRepr::U64(v) => visitor.visit_u64(v),
             ValueRepr::I64(v) => visitor.visit_i64(v),
             ValueRepr::I128(v) => visitor.visit_i128(v.0),
             ValueRepr::U128(v) => visitor.visit_u128(v.0),
             ValueRepr::F64(v) => visitor.visit_f64(v),
             ValueRepr::String(ref v, _) => visitor.visit_str(v),
+            ValueRepr::SmallStr(v) => visitor.visit_str(v.as_str()),
             ValueRepr::Undefined | ValueRepr::None => visitor.visit_unit(),
             ValueRepr::Bytes(ref v) => visitor.visit_bytes(v),
-            ValueRepr::Seq(_) | ValueRepr::Map(..) | ValueRepr::Dynamic(_) => {
-                if let Some(s) = self.value.as_seq() {
+            ValueRepr::Object(o) => match o.repr() {
+                ObjectRepr::Plain => Err(de::Error::custom("cannot deserialize plain objects")),
+                ObjectRepr::Seq | ObjectRepr::Iterable => {
                     visitor.visit_seq(de::value::SeqDeserializer::new(
-                        s.iter().map(ValueDeserializer::new),
-                    ))
-                } else if self.value.kind() == ValueKind::Map {
-                    visitor.visit_map(de::value::MapDeserializer::new(
-                        ok!(self.value.try_iter()).map(|k| {
-                            (
-                                ValueDeserializer::new(k.clone()),
-                                ValueDeserializer::new(self.value.get_item(&k).unwrap_or_default()),
-                            )
-                        }),
-                    ))
-                } else {
-                    Err(de::Error::invalid_type(
-                        value_to_unexpected(&self.value),
-                        &"supported value",
+                        o.try_iter()
+                            .into_iter()
+                            .flatten()
+                            .map(ValueDeserializer::new),
                     ))
                 }
-            }
+                ObjectRepr::Map => visitor.visit_map(de::value::MapDeserializer::new(
+                    o.try_iter_pairs()
+                        .into_iter()
+                        .flatten()
+                        .map(|(k, v)| (ValueDeserializer::new(k), ValueDeserializer::new(v))),
+                )),
+            },
         }
     }
 
     fn deserialize_option<V: de::Visitor<'de>>(self, visitor: V) -> Result<V::Value, Error> {
         match self.value.0 {
             ValueRepr::None | ValueRepr::Undefined => visitor.visit_unit(),
             _ => visitor.visit_some(self),
@@ -309,20 +306,27 @@
         }
     }
 
     fn tuple_variant<V>(self, _len: usize, visitor: V) -> Result<V::Value, Error>
     where
         V: de::Visitor<'de>,
     {
-        match self.value.as_ref().and_then(|x| x.as_seq()) {
-            Some(seq) => de::Deserializer::deserialize_any(
-                de::value::SeqDeserializer::new(seq.iter().map(ValueDeserializer::new)),
-                visitor,
-            ),
-            None => Err(de::Error::invalid_type(
+        match self.value.as_ref().and_then(|x| x.as_object()) {
+            Some(obj) if matches!(obj.repr(), ObjectRepr::Seq) => {
+                de::Deserializer::deserialize_any(
+                    de::value::SeqDeserializer::new(
+                        obj.try_iter()
+                            .into_iter()
+                            .flatten()
+                            .map(ValueDeserializer::new),
+                    ),
+                    visitor,
+                )
+            }
+            _ => Err(de::Error::invalid_type(
                 self.value
                     .as_ref()
                     .map_or(de::Unexpected::Unit, value_to_unexpected),
                 &"tuple variant",
             )),
         }
     }
@@ -438,17 +442,12 @@
             if signed as i128 == val.0 {
                 de::Unexpected::Signed(signed)
             } else {
                 de::Unexpected::Other("u128")
             }
         }
         ValueRepr::String(ref s, _) => de::Unexpected::Str(s),
+        ValueRepr::SmallStr(ref s) => de::Unexpected::Str(s.as_str()),
         ValueRepr::Bytes(ref b) => de::Unexpected::Bytes(b),
-        ValueRepr::Seq(_) => de::Unexpected::Seq,
-        ValueRepr::Map(_, _) => de::Unexpected::Map,
-        ValueRepr::Dynamic(ref d) => match d.kind() {
-            super::ObjectKind::Plain => de::Unexpected::Other("plain object"),
-            super::ObjectKind::Seq(_) => de::Unexpected::Seq,
-            super::ObjectKind::Struct(_) => de::Unexpected::Map,
-        },
+        ValueRepr::Object(..) => de::Unexpected::Other("<dynamic value>"),
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/merge_object.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/merge_object.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 use std::collections::BTreeSet;
 use std::sync::Arc;
 
-use crate::value::object::StructObject;
-use crate::value::Value;
+use crate::value::{Enumerator, Object, ObjectExt, Value};
 
 /// Utility struct used by [`context!`](crate::context) to merge
 /// multiple values.
+#[derive(Clone, Debug)]
 pub struct MergeObject(pub Vec<Value>);
 
-impl StructObject for MergeObject {
-    fn get_field(&self, field: &str) -> Option<Value> {
-        for val in &self.0 {
-            match val.get_attr(field) {
-                Ok(val) if !val.is_undefined() => return Some(val),
-                _ => {}
-            }
-        }
-        None
+impl Object for MergeObject {
+    fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+        self.0
+            .iter()
+            .filter_map(|x| x.get_item_opt(key))
+            .find(|x| !x.is_undefined())
     }
 
-    fn fields(&self) -> Vec<Arc<str>> {
-        let mut seen = BTreeSet::new();
-        let mut rv = Vec::new();
-        for val in &self.0 {
-            if let Ok(iter) = val.try_iter() {
-                for item in iter {
-                    let s: Result<Arc<str>, _> = item.try_into();
-                    if let Ok(s) = s {
-                        if !seen.contains(&s) {
-                            seen.insert(s.clone());
-                            rv.push(s);
+    fn enumerate(self: &Arc<Self>) -> Enumerator {
+        self.mapped_enumerator(|this| {
+            let mut seen = BTreeSet::new();
+            Box::new(
+                this.0
+                    .iter()
+                    .flat_map(|v| v.try_iter().ok())
+                    .flatten()
+                    .filter_map(move |v| {
+                        if seen.contains(&v) {
+                            None
+                        } else {
+                            seen.insert(v.clone());
+                            Some(v)
                         }
-                    }
-                }
-            }
-        }
-        rv
+                    }),
+            )
+        })
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/mod.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -10,53 +10,91 @@
 //! advanced use cases it's useful to know that this type exists.
 //!
 //! # Basic Value Conversions
 //!
 //! Values are typically created via the [`From`] trait:
 //!
 //! ```
+//! use std::collections::BTreeMap;
 //! # use minijinja::value::Value;
 //! let int_value = Value::from(42);
 //! let none_value = Value::from(());
 //! let true_value = Value::from(true);
+//! let map = Value::from({
+//!     let mut m = BTreeMap::new();
+//!     m.insert("foo", 1);
+//!     m.insert("bar", 2);
+//!     m
+//! });
 //! ```
 //!
-//! Or via the [`FromIterator`] trait:
+//! Or via the [`FromIterator`] trait which can create sequences or maps.  When
+//! given a tuple it creates maps, otherwise it makes a sequence.
 //!
 //! ```
 //! # use minijinja::value::Value;
 //! // collection into a sequence
 //! let value: Value = (1..10).into_iter().collect();
 //!
 //! // collection into a map
 //! let value: Value = [("key", "value")].into_iter().collect();
 //! ```
 //!
+//! For certain types of iterators (`Send` + `Sync` + `'static`) it's also
+//! possible to make the value lazily iterate over the value by using the
+//! [`Value::make_iterable`] function instead.  Whenever the value requires
+//! iteration, the function is called to create that iterator.
+//!
+//! ```
+//! # use minijinja::value::Value;
+//! let value: Value = Value::make_iterable(|| 1..10);
+//! ```
+//!
 //! To to into the inverse directly the various [`TryFrom`](std::convert::TryFrom)
 //! implementations can be used:
 //!
 //! ```
 //! # use minijinja::value::Value;
 //! use std::convert::TryFrom;
 //! let v = u64::try_from(Value::from(42)).unwrap();
 //! ```
 //!
 //! The special [`Undefined`](Value::UNDEFINED) value also exists but does not
 //! have a rust equivalent.  It can be created via the [`UNDEFINED`](Value::UNDEFINED)
 //! constant.
 //!
+//! # Collections
+//!
+//! The standard library's collection types such as
+//! [`HashMap`](std::collections::HashMap), [`Vec`] and various others from the
+//! collections module are implemented are objects.  There is a cavet here which is
+//! that maps can only have string or [`Value`] as key.  The values in the collections
+//! are lazily converted into value when accessed or iterated over.   These types can
+//! be constructed either from [`Value::from`] or [`Value::from_object`].  Because the
+//! types are boxed unchanged, you can also downcast them.
+//!
+//! ```rust
+//! # use minijinja::Value;
+//! let vec = Value::from(vec![1i32, 2, 3, 4]);
+//! let vec_ref = vec.downcast_object_ref::<Vec<i32>>().unwrap();
+//! assert_eq!(vec_ref, &vec![1, 2, 3, 4]);
+//! ```
+//!
+//! **Caveat:** for convenience reasons maps with `&str` keys can be stored.  The keys
+//! however are converted into `Arc<str>`.
+//!
 //! # Serde Conversions
 //!
 //! MiniJinja will usually however create values via an indirection via [`serde`] when
 //! a template is rendered or an expression is evaluated.  This can also be
-//! triggered manually by using the [`Value::from_serializable`] method:
+//! triggered manually by using the [`Value::from_serialize`] method:
 //!
 //! ```
 //! # use minijinja::value::Value;
-//! let value = Value::from_serializable(&[1, 2, 3]);
+//! let value = Value::from_serialize(&[1, 2, 3]);
 //! ```
 //!
 //! The inverse of that operation is to pass a value directly as serializer to
 //! a type that supports deserialization.  This requires the `deserialization`
 //! feature.
 //!
 #![cfg_attr(
@@ -82,98 +120,116 @@
 //! Values are immutable objects which are internally reference counted which
 //! means they can be copied relatively cheaply.  Special care must be taken
 //! so that cycles are not created to avoid causing memory leaks.
 //!
 //! # HTML Escaping
 //!
 //! MiniJinja inherits the general desire to be clever about escaping.  For this
-//! prupose a value will (when auto escaping is enabled) always be escaped.  To
+//! purpose a value will (when auto escaping is enabled) always be escaped.  To
 //! prevent this behavior the [`safe`](crate::filters::safe) filter can be used
 //! in the template.  Outside of templates the [`Value::from_safe_string`] method
 //! can be used to achieve the same result.
 //!
 //! # Dynamic Objects
 //!
 //! Values can also hold "dynamic" objects.  These are objects which implement the
-//! [`Object`] trait and optionally [`SeqObject`] or [`StructObject`]  These can
-//! be used to implement dynamic functionality such as stateful values and more.
-//! Dynamic objects are internally also used to implement the special `loop`
-//! variable or macros.
-//!
-//! To create a dynamic `Value` object, use [`Value::from_object`],
-//! [`Value::from_seq_object`], [`Value::from_struct_object`] or the `From<Arc<T:
-//! Object>>` implementations for `Value`:
+//! [`Object`] trait.  These can be used to implement dynamic functionality such
+//! as stateful values and more.  Dynamic objects are internally also used to
+//! implement the special `loop` variable, macros and similar things.
+//!
+//! To create a [`Value`] from a dynamic object use [`Value::from_object`],
+//! [`Value::from_dyn_object`]:
 //!
 //! ```rust
 //! # use std::sync::Arc;
-//! # use minijinja::value::{Value, Object};
+//! # use minijinja::value::{Value, Object, DynObject};
 //! #[derive(Debug)]
 //! struct Foo;
 //!
-//! # impl std::fmt::Display for Foo {
-//! #     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result { Ok(()) }
-//! # }
-//! #
 //! impl Object for Foo {
 //!     /* implementation */
 //! }
 //!
 //! let value = Value::from_object(Foo);
-//! let value = Value::from(Arc::new(Foo));
-//! let value = Value::from(Arc::new(Foo) as Arc<dyn Object>);
+//! let value = Value::from_dyn_object(Arc::new(Foo));
 //! ```
+//!
+//! # Invalid Values
+//!
+//! MiniJinja knows the concept of an "invalid value".  These are rare in practice
+//! and should not be used, but they are needed in some situations.  An invalid value
+//! looks like a value but working with that value in the context of the engine will
+//! fail in most situations.  In principle an invalid value is a value that holds an
+//! error internally.  It's created with [`From`]:
+//!
+//! ```
+//! use minijinja::{Value, Error, ErrorKind};
+//! let error = Error::new(ErrorKind::InvalidOperation, "failed to generate an item");
+//! let invalid_value = Value::from(error);
+//! ```
+//!
+//! Invalid values are typically encountered in the following situations:
+//!
+//! - serialization fails with an error: this is the case when a value is crated
+//!   via [`Value::from_serialize`] and the underlying [`Serialize`] implementation
+//!   fails with an error.
+//! - fallible iteration: there might be situations where an iterator cannot indicate
+//!   failure ahead of iteration and must abort.  In that case the only option an
+//!   iterator in MiniJinja has is to create an invalid value.
+//!
+//! It's generally recommende to ignore the existence of invalid objects and let them
+//! fail naturally as they are encountered.
 
 // this module is based on the content module in insta which in turn is based
 // on the content module in serde::private::ser.
 
 use std::cell::{Cell, RefCell};
 use std::cmp::Ordering;
 use std::collections::BTreeMap;
-use std::convert::TryFrom;
 use std::fmt;
 use std::hash::{Hash, Hasher};
-use std::marker::PhantomData;
-use std::sync::Arc;
+use std::sync::{Arc, Mutex};
 
 use serde::ser::{Serialize, Serializer};
 
 use crate::error::{Error, ErrorKind};
 use crate::functions;
 use crate::utils::OnDrop;
-use crate::value::object::{SimpleSeqObject, SimpleStructObject};
 use crate::value::ops::as_f64;
 use crate::value::serialize::transform;
 use crate::vm::State;
 
 pub use crate::value::argtypes::{from_args, ArgType, FunctionArgs, FunctionResult, Kwargs, Rest};
-pub use crate::value::object::{Object, ObjectKind, SeqObject, SeqObjectIter, StructObject};
+pub use crate::value::object::{DynObject, Enumerator, Object, ObjectExt, ObjectRepr};
 
+#[macro_use]
+mod type_erase;
 mod argtypes;
 #[cfg(feature = "deserialization")]
 mod deserialize;
-mod keyref;
 pub(crate) mod merge_object;
+pub(crate) mod namespace_object;
 mod object;
 pub(crate) mod ops;
 mod serialize;
+#[cfg(feature = "key_interning")]
+mod string_interning;
 
 #[cfg(feature = "deserialization")]
 pub use self::deserialize::ViaDeserialize;
 
-pub(crate) use crate::value::keyref::KeyRef;
-
 // We use in-band signalling to roundtrip some internal values.  This is
 // not ideal but unfortunately there is no better system in serde today.
 const VALUE_HANDLE_MARKER: &str = "\x01__minijinja_ValueHandle";
 
 #[cfg(feature = "preserve_order")]
-pub(crate) type ValueMap = indexmap::IndexMap<KeyRef<'static>, Value>;
+pub(crate) type ValueMap = indexmap::IndexMap<Value, Value>;
 
 #[cfg(not(feature = "preserve_order"))]
-pub(crate) type ValueMap = std::collections::BTreeMap<KeyRef<'static>, Value>;
+pub(crate) type ValueMap = std::collections::BTreeMap<Value, Value>;
 
 #[inline(always)]
 pub(crate) fn value_map_with_capacity(capacity: usize) -> ValueMap {
     #[cfg(not(feature = "preserve_order"))]
     {
         let _ = capacity;
         ValueMap::new()
@@ -181,19 +237,19 @@
     #[cfg(feature = "preserve_order")]
     {
         ValueMap::with_capacity(crate::utils::untrusted_size_hint(capacity))
     }
 }
 
 thread_local! {
-    static INTERNAL_SERIALIZATION: Cell<bool> = Cell::new(false);
+    static INTERNAL_SERIALIZATION: Cell<bool> = const { Cell::new(false) };
 
     // This should be an AtomicU64 but sadly 32bit targets do not necessarily have
     // AtomicU64 available.
-    static LAST_VALUE_HANDLE: Cell<u32> = Cell::new(0);
+    static LAST_VALUE_HANDLE: Cell<u32> = const { Cell::new(0) };
     static VALUE_HANDLES: RefCell<BTreeMap<u32, Value>> = RefCell::new(BTreeMap::new());
 }
 
 /// Function that returns true when serialization for [`Value`] is taking place.
 ///
 /// MiniJinja internally creates [`Value`] objects from all values passed to the
 /// engine.  It does this by going through the regular serde serialization trait.
@@ -217,15 +273,15 @@
 ///
 /// If `key_interning` is enabled, this turns on that feature, otherwise
 /// it becomes a noop.
 #[inline(always)]
 pub(crate) fn value_optimization() -> impl Drop {
     #[cfg(feature = "key_interning")]
     {
-        crate::value::keyref::key_interning::use_string_cache()
+        crate::value::string_interning::use_string_cache()
     }
     #[cfg(not(feature = "key_interning"))]
     {
         OnDrop::new(|| {})
     }
 }
 
@@ -240,57 +296,63 @@
             INTERNAL_SERIALIZATION.with(|flag| flag.set(false));
         }
     })
 }
 
 /// Describes the kind of value.
 #[derive(Copy, Clone, Debug, Eq, PartialEq, Ord, PartialOrd)]
+#[non_exhaustive]
 pub enum ValueKind {
     /// The value is undefined
     Undefined,
-    /// The value is the none singleton ([`()`])
+    /// The value is the none singleton (`()`)
     None,
     /// The value is a [`bool`]
     Bool,
     /// The value is a number of a supported type.
     Number,
     /// The value is a string.
     String,
     /// The value is a byte array.
     Bytes,
     /// The value is an array of other values.
     Seq,
     /// The value is a key/value mapping.
     Map,
+    /// An iterable
+    Iterable,
+    /// A plain object without specific behavior.
+    Plain,
+    /// This value is invalid (holds an error).
+    ///
+    /// This can happen when a serialization error occurred or the engine
+    /// encountered a failure in a place where an error can otherwise not
+    /// be produced.  Interacting with such values in the context of the
+    /// template evaluation process will attempt to propagate the error.
+    Invalid,
 }
 
 impl fmt::Display for ValueKind {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         f.write_str(match *self {
             ValueKind::Undefined => "undefined",
             ValueKind::None => "none",
             ValueKind::Bool => "bool",
             ValueKind::Number => "number",
             ValueKind::String => "string",
             ValueKind::Bytes => "bytes",
             ValueKind::Seq => "sequence",
             ValueKind::Map => "map",
+            ValueKind::Iterable => "iterator",
+            ValueKind::Plain => "plain object",
+            ValueKind::Invalid => "invalid value",
         })
     }
 }
 
-/// The type of map
-#[derive(Copy, Clone, Debug)]
-pub(crate) enum MapType {
-    /// A regular map
-    Normal,
-    /// A map representing keyword arguments
-    Kwargs,
-}
-
 /// Type type of string
 #[derive(Copy, Clone, Debug)]
 pub(crate) enum StringType {
     Normal,
     Safe,
 }
 
@@ -304,30 +366,67 @@
 
 impl<T: Copy> Clone for Packed<T> {
     fn clone(&self) -> Self {
         *self
     }
 }
 
+/// Max size of a small str.
+///
+/// Logic: Value is 24 bytes. 1 byte is for the disciminant. One byte is
+/// needed for the small str length.
+const SMALL_STR_CAP: usize = 22;
+
+/// Helper to store string data inline.
+#[derive(Clone)]
+pub(crate) struct SmallStr {
+    len: u8,
+    buf: [u8; SMALL_STR_CAP],
+}
+
+impl SmallStr {
+    pub fn try_new(s: &str) -> Option<SmallStr> {
+        let len = s.len();
+        if len <= SMALL_STR_CAP {
+            let mut buf = [0u8; SMALL_STR_CAP];
+            buf[..len].copy_from_slice(s.as_bytes());
+            Some(SmallStr {
+                len: len as u8,
+                buf,
+            })
+        } else {
+            None
+        }
+    }
+
+    pub fn as_str(&self) -> &str {
+        // SAFETY: This is safe because we only place well-formed utf-8 strings
+        unsafe { std::str::from_utf8_unchecked(&self.buf[..self.len as usize]) }
+    }
+
+    pub fn is_empty(&self) -> bool {
+        self.len == 0
+    }
+}
+
 #[derive(Clone)]
 pub(crate) enum ValueRepr {
     Undefined,
     Bool(bool),
     U64(u64),
     I64(i64),
     F64(f64),
     None,
-    Invalid(Arc<str>),
+    Invalid(Arc<Error>),
     U128(Packed<u128>),
     I128(Packed<i128>),
     String(Arc<str>, StringType),
+    SmallStr(SmallStr),
     Bytes(Arc<Vec<u8>>),
-    Seq(Arc<Vec<Value>>),
-    Map(Arc<ValueMap>, MapType),
-    Dynamic(Arc<dyn Object>),
+    Object(DynObject),
 }
 
 impl fmt::Debug for ValueRepr {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
             ValueRepr::Undefined => f.write_str("undefined"),
             ValueRepr::Bool(val) => fmt::Debug::fmt(val, f),
@@ -335,52 +434,31 @@
             ValueRepr::I64(val) => fmt::Debug::fmt(val, f),
             ValueRepr::F64(val) => fmt::Debug::fmt(val, f),
             ValueRepr::None => f.write_str("none"),
             ValueRepr::Invalid(ref val) => write!(f, "<invalid value: {}>", val),
             ValueRepr::U128(val) => fmt::Debug::fmt(&{ val.0 }, f),
             ValueRepr::I128(val) => fmt::Debug::fmt(&{ val.0 }, f),
             ValueRepr::String(val, _) => fmt::Debug::fmt(val, f),
+            ValueRepr::SmallStr(val) => fmt::Debug::fmt(val.as_str(), f),
             ValueRepr::Bytes(val) => fmt::Debug::fmt(val, f),
-            ValueRepr::Seq(val) => fmt::Debug::fmt(val, f),
-            ValueRepr::Map(val, _) => fmt::Debug::fmt(val, f),
-            ValueRepr::Dynamic(val) => fmt::Debug::fmt(val, f),
+            ValueRepr::Object(val) => val.render(f),
         }
     }
 }
 
 impl Hash for Value {
     fn hash<H: Hasher>(&self, state: &mut H) {
         match &self.0 {
             ValueRepr::None | ValueRepr::Undefined => 0u8.hash(state),
             ValueRepr::String(ref s, _) => s.hash(state),
+            ValueRepr::SmallStr(s) => s.as_str().hash(state),
             ValueRepr::Bool(b) => b.hash(state),
-            ValueRepr::Invalid(s) => s.hash(state),
+            ValueRepr::Invalid(ref e) => (e.kind(), e.detail()).hash(state),
             ValueRepr::Bytes(b) => b.hash(state),
-            ValueRepr::Seq(b) => b.hash(state),
-            ValueRepr::Map(m, _) => m.iter().for_each(|(k, v)| {
-                k.hash(state);
-                v.hash(state);
-            }),
-            ValueRepr::Dynamic(d) => match d.kind() {
-                ObjectKind::Plain => 0u8.hash(state),
-                ObjectKind::Seq(s) => s.iter().for_each(|x| x.hash(state)),
-                ObjectKind::Struct(s) => {
-                    if let Some(fields) = s.static_fields() {
-                        fields.iter().for_each(|k| {
-                            k.hash(state);
-                            s.get_field(k).hash(state);
-                        });
-                    } else {
-                        s.fields().iter().for_each(|k| {
-                            k.hash(state);
-                            s.get_field(k).hash(state);
-                        });
-                    }
-                }
-            },
+            ValueRepr::Object(d) => d.hash(state),
             ValueRepr::U64(_)
             | ValueRepr::I64(_)
             | ValueRepr::F64(_)
             | ValueRepr::U128(_)
             | ValueRepr::I128(_) => {
                 if let Ok(val) = i64::try_from(self.clone()) {
                     val.hash(state)
@@ -398,28 +476,28 @@
 
 impl PartialEq for Value {
     fn eq(&self, other: &Self) -> bool {
         match (&self.0, &other.0) {
             (ValueRepr::None, ValueRepr::None) => true,
             (ValueRepr::Undefined, ValueRepr::Undefined) => true,
             (ValueRepr::String(ref a, _), ValueRepr::String(ref b, _)) => a == b,
+            (ValueRepr::SmallStr(a), ValueRepr::SmallStr(b)) => a.as_str() == b.as_str(),
             (ValueRepr::Bytes(a), ValueRepr::Bytes(b)) => a == b,
             _ => match ops::coerce(self, other) {
                 Some(ops::CoerceResult::F64(a, b)) => a == b,
                 Some(ops::CoerceResult::I128(a, b)) => a == b,
                 Some(ops::CoerceResult::Str(a, b)) => a == b,
                 None => {
-                    if let (Some(a), Some(b)) = (self.as_seq(), other.as_seq()) {
-                        a.iter().eq(b.iter())
-                    } else if self.kind() == ValueKind::Map && other.kind() == ValueKind::Map {
-                        if self.len() != other.len() {
-                            return false;
-                        }
-                        if let Ok(mut iter) = self.try_iter() {
-                            iter.all(|x| self.get_item_opt(&x) == other.get_item_opt(&x))
+                    if let (Some(a), Some(b)) = (self.as_object(), other.as_object()) {
+                        if a.repr() != b.repr() {
+                            false
+                        } else if let (Some(ak), Some(bk)) =
+                            (a.try_iter_pairs(), b.try_iter_pairs())
+                        {
+                            ak.eq(bk)
                         } else {
                             false
                         }
                     } else {
                         false
                     }
                 }
@@ -447,33 +525,34 @@
 
 impl Ord for Value {
     fn cmp(&self, other: &Self) -> Ordering {
         let value_ordering = match (&self.0, &other.0) {
             (ValueRepr::None, ValueRepr::None) => Ordering::Equal,
             (ValueRepr::Undefined, ValueRepr::Undefined) => Ordering::Equal,
             (ValueRepr::String(ref a, _), ValueRepr::String(ref b, _)) => a.cmp(b),
+            (ValueRepr::SmallStr(a), ValueRepr::SmallStr(b)) => a.as_str().cmp(b.as_str()),
             (ValueRepr::Bytes(a), ValueRepr::Bytes(b)) => a.cmp(b),
             _ => match ops::coerce(self, other) {
                 Some(ops::CoerceResult::F64(a, b)) => f64_total_cmp(a, b),
                 Some(ops::CoerceResult::I128(a, b)) => a.cmp(&b),
                 Some(ops::CoerceResult::Str(a, b)) => a.cmp(b),
-                None => {
-                    if let (Some(a), Some(b)) = (self.as_seq(), other.as_seq()) {
-                        a.iter().cmp(b.iter())
-                    } else if self.kind() == ValueKind::Map && other.kind() == ValueKind::Map {
-                        if let (Ok(a), Ok(b)) = (self.try_iter(), other.try_iter()) {
-                            a.map(|k| (k.clone(), self.get_item_opt(&k)))
-                                .cmp(b.map(|k| (k.clone(), other.get_item_opt(&k))))
-                        } else {
-                            Ordering::Equal
-                        }
-                    } else {
-                        Ordering::Equal
-                    }
-                }
+                None => match (self.kind(), other.kind()) {
+                    (ValueKind::Seq, ValueKind::Seq) => match (self.try_iter(), other.try_iter()) {
+                        (Ok(a), Ok(b)) => a.cmp(b),
+                        _ => self.len().cmp(&other.len()),
+                    },
+                    (ValueKind::Map, ValueKind::Map) => match (
+                        self.as_object().and_then(|x| x.try_iter_pairs()),
+                        other.as_object().and_then(|x| x.try_iter_pairs()),
+                    ) {
+                        (Some(a), Some(b)) => a.cmp(b),
+                        _ => self.len().cmp(&other.len()),
+                    },
+                    _ => Ordering::Equal,
+                },
             },
         };
         value_ordering.then((self.kind() as usize).cmp(&(other.kind() as usize)))
     }
 }
 
 impl fmt::Debug for Value {
@@ -502,37 +581,18 @@
                     write!(f, "{num}")
                 }
             }
             ValueRepr::None => f.write_str("none"),
             ValueRepr::Invalid(ref val) => write!(f, "<invalid value: {}>", val),
             ValueRepr::I128(val) => write!(f, "{}", { val.0 }),
             ValueRepr::String(val, _) => write!(f, "{val}"),
+            ValueRepr::SmallStr(val) => write!(f, "{}", val.as_str()),
             ValueRepr::Bytes(val) => write!(f, "{}", String::from_utf8_lossy(val)),
-            ValueRepr::Seq(values) => {
-                ok!(f.write_str("["));
-                for (idx, val) in values.iter().enumerate() {
-                    if idx > 0 {
-                        ok!(f.write_str(", "));
-                    }
-                    ok!(write!(f, "{val:?}"));
-                }
-                f.write_str("]")
-            }
-            ValueRepr::Map(m, _) => {
-                ok!(f.write_str("{"));
-                for (idx, (key, val)) in m.iter().enumerate() {
-                    if idx > 0 {
-                        ok!(f.write_str(", "));
-                    }
-                    ok!(write!(f, "{key:?}: {val:?}"));
-                }
-                f.write_str("}")
-            }
             ValueRepr::U128(val) => write!(f, "{}", { val.0 }),
-            ValueRepr::Dynamic(x) => write!(f, "{x}"),
+            ValueRepr::Object(x) => write!(f, "{x}"),
         }
     }
 }
 
 impl Default for Value {
     fn default() -> Value {
         ValueRepr::Undefined.into()
@@ -545,15 +605,15 @@
 /// reuse strings in certain cases.  This function can be used to utilize the
 /// same functionality.  There is no guarantee that a string will be interned
 /// as there are heuristics involved for it.  Additionally the string interning
 /// will only work during the template engine execution (eg: within filters etc.).
 pub fn intern(s: &str) -> Arc<str> {
     #[cfg(feature = "key_interning")]
     {
-        crate::value::keyref::key_interning::try_intern(s)
+        crate::value::string_interning::try_intern(s)
     }
     #[cfg(not(feature = "key_interning"))]
     {
         Arc::from(s.to_string())
     }
 }
 
@@ -574,35 +634,51 @@
     ///
     /// During serialization of the value, [`serializing_for_value`] will return
     /// `true` which makes it possible to customize serialization for MiniJinja.
     /// For more information see [`serializing_for_value`].
     ///
     /// ```
     /// # use minijinja::value::Value;
-    /// let val = Value::from_serializable(&vec![1, 2, 3]);
+    /// let val = Value::from_serialize(&vec![1, 2, 3]);
     /// ```
     ///
     /// This method does not fail but it might return a value that is not valid.  Such
     /// values will when operated on fail in the template engine in most situations.
     /// This for instance can happen if the underlying implementation of [`Serialize`]
     /// fails.  There are also cases where invalid objects are silently hidden in the
     /// engine today.  This is for instance the case for when keys are used in hash maps
     /// that the engine cannot deal with.  Invalid values are considered an implementation
     /// detail.  There is currently no API to validate a value.
     ///
     /// If the `deserialization` feature is enabled then the inverse of this method
     /// is to use the [`Value`] type as serializer.  You can pass a value into the
     /// [`deserialize`](serde::Deserialize::deserialize) method of a type that supports
     /// serde deserialization.
-    pub fn from_serializable<T: Serialize>(value: &T) -> Value {
+    pub fn from_serialize<T: Serialize>(value: T) -> Value {
         let _serialization_guard = mark_internal_serialization();
         let _optimization_guard = value_optimization();
         transform(value)
     }
 
+    /// Extracts a contained error.
+    ///
+    /// An invalid value carres an error internally and will reveal that error
+    /// at a later point when iteracted with.  This is used to carry
+    /// serialization errors or failures that happen when the engine otherwise
+    /// assumes an infallible operation such as iteration.
+    pub(crate) fn validate(self) -> Result<Value, Error> {
+        if let ValueRepr::Invalid(err) = self.0 {
+            // Today the API implies tghat errors are `Clone`, but we don't want to expose
+            // this as a functionality (yet?).
+            Err(Arc::try_unwrap(err).unwrap_or_else(|arc| (*arc).internal_clone()))
+        } else {
+            Ok(self)
+        }
+    }
+
     /// Creates a value from a safe string.
     ///
     /// A safe string is one that will bypass auto escaping.  For instance if you
     /// want to have the template engine render some HTML without the user having to
     /// supply the `|safe` filter, you can use a value of this type instead.
     ///
     /// ```
@@ -622,59 +698,195 @@
     /// use std::fmt;
     ///
     /// #[derive(Debug)]
     /// struct Thing {
     ///     id: usize,
     /// }
     ///
-    /// impl fmt::Display for Thing {
-    ///     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-    ///         fmt::Debug::fmt(self, f)
+    /// impl Object for Thing {}
+    ///
+    /// let val = Value::from_object(Thing { id: 42 });
+    /// ```
+    pub fn from_object<T: Object + Send + Sync + 'static>(value: T) -> Value {
+        Value::from(ValueRepr::Object(DynObject::new(Arc::new(value))))
+    }
+
+    /// Like [`from_object`](Self::from_object) but for type erased dynamic objects.
+    ///
+    /// This especially useful if you have an object that has an `Arc<T>` to another
+    /// child object that you want to return as a `Arc<T>` turns into a [`DynObject`]
+    /// automatically.
+    ///
+    /// ```rust
+    /// # use std::sync::Arc;
+    /// # use minijinja::value::{Value, Object, Enumerator};
+    /// #[derive(Debug)]
+    /// pub struct HttpConfig {
+    ///     port: usize,
+    /// }
+    ///
+    /// #[derive(Debug)]
+    /// struct Config {
+    ///     http: Arc<HttpConfig>,
+    /// }
+    ///
+    /// impl Object for HttpConfig {
+    ///     fn enumerate(self: &Arc<Self>) -> Enumerator {
+    ///         Enumerator::Str(&["port"])
+    ///     }
+    ///
+    ///     fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+    ///         match key.as_str()? {
+    ///             "port" => Some(Value::from(self.port)),
+    ///             _ => None,
+    ///         }
     ///     }
     /// }
     ///
-    /// impl Object for Thing {}
+    /// impl Object for Config {
+    ///     fn enumerate(self: &Arc<Self>) -> Enumerator {
+    ///         Enumerator::Str(&["http"])
+    ///     }
+    ///
+    ///     fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+    ///         match key.as_str()? {
+    ///             "http" => Some(Value::from_dyn_object(self.http.clone())),
+    ///             _ => None
+    ///         }
+    ///     }
+    /// }
+    /// ```
+    pub fn from_dyn_object<T: Into<DynObject>>(value: T) -> Value {
+        Value::from(ValueRepr::Object(value.into()))
+    }
+
+    /// Creates a value that is an iterable.
+    ///
+    /// The function is invoked to create a new iterator every time the value is
+    /// iterated over.
     ///
-    /// let val = Value::from_object(Thing { id: 42 });
+    /// ```
+    /// # use minijinja::value::Value;
+    /// let val = Value::make_iterable(|| 0..10);
     /// ```
     ///
-    /// Objects are internally reference counted.  If you want to hold on to the
-    /// `Arc` you can directly create the value from an arc'ed object:
+    /// Iterators that implement [`ExactSizeIterator`] or have a matching lower and upper
+    /// bound on the [`Iterator::size_hint`] report a known `loop.length`.  Iterators that
+    /// do not fulfill these requirements will not.  The same is true for `revindex` and
+    /// similar properties.
+    pub fn make_iterable<I, T, F>(maker: F) -> Value
+    where
+        I: Iterator<Item = T> + Send + Sync + 'static,
+        T: Into<Value> + Send + Sync + 'static,
+        F: Fn() -> I + Send + Sync + 'static,
+    {
+        Value::make_object_iterable((), move |_| Box::new(maker().map(Into::into)))
+    }
+
+    /// Creates an iterable that iterates over the given value.
+    ///
+    /// This is similar to [`make_iterable`](Self::make_iterable) but it takes an extra
+    /// reference to a value it can borrow out from.  It's a bit less generic in that it
+    /// needs to return a boxed iterator of values directly.
     ///
     /// ```rust
-    /// # use minijinja::value::{Value, Object};
-    /// # #[derive(Debug)]
-    /// # struct Thing { id: usize };
-    /// # impl std::fmt::Display for Thing {
-    /// #     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-    /// #         todo!();
-    /// #     }
-    /// # }
-    /// # impl Object for Thing {}
-    /// use std::sync::Arc;
-    /// let val = Value::from(Arc::new(Thing { id: 42 }));
-    /// ```
-    pub fn from_object<T: Object>(value: T) -> Value {
-        Value::from(Arc::new(value) as Arc<dyn Object>)
-    }
-
-    /// Creates a value from an owned [`SeqObject`].
-    ///
-    /// This is a simplified API for creating dynamic sequences
-    /// without having to implement the entire [`Object`] protocol.
-    pub fn from_seq_object<T: SeqObject + 'static>(value: T) -> Value {
-        Value::from_object(SimpleSeqObject(value))
-    }
-
-    /// Creates a value from an owned [`StructObject`].
-    ///
-    /// This is a simplified API for creating dynamic structs
-    /// without having to implement the entire [`Object`] protocol.
-    pub fn from_struct_object<T: StructObject + 'static>(value: T) -> Value {
-        Value::from_object(SimpleStructObject(value))
+    /// # use minijinja::value::Value;
+    /// let val = Value::make_object_iterable(vec![1, 2, 3], |vec| {
+    ///     Box::new(vec.iter().copied().map(Value::from))
+    /// });
+    /// assert_eq!(val.to_string(), "[1, 2, 3]");
+    /// ````
+    pub fn make_object_iterable<T, F>(object: T, maker: F) -> Value
+    where
+        T: Send + Sync + 'static,
+        F: for<'a> Fn(&'a T) -> Box<dyn Iterator<Item = Value> + Send + Sync + 'a>
+            + Send
+            + Sync
+            + 'static,
+    {
+        struct Iterable<T, F> {
+            maker: F,
+            object: T,
+        }
+
+        impl<T, F> fmt::Debug for Iterable<T, F> {
+            fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+                f.debug_struct("<iterator>").finish()
+            }
+        }
+
+        impl<T, F> Object for Iterable<T, F>
+        where
+            T: Send + Sync + 'static,
+            F: for<'a> Fn(&'a T) -> Box<dyn Iterator<Item = Value> + Send + Sync + 'a>
+                + Send
+                + Sync
+                + 'static,
+        {
+            fn repr(self: &Arc<Self>) -> ObjectRepr {
+                ObjectRepr::Iterable
+            }
+
+            fn enumerate(self: &Arc<Self>) -> Enumerator {
+                struct Iter {
+                    iter: Box<dyn Iterator<Item = Value> + Send + Sync + 'static>,
+                    _object: DynObject,
+                }
+
+                impl Iterator for Iter {
+                    type Item = Value;
+
+                    fn next(&mut self) -> Option<Self::Item> {
+                        self.iter.next()
+                    }
+
+                    fn size_hint(&self) -> (usize, Option<usize>) {
+                        self.iter.size_hint()
+                    }
+                }
+
+                // SAFETY: this is safe because the object is kept alive by the iter
+                let iter = unsafe { std::mem::transmute((self.maker)(&self.object)) };
+                let _object = DynObject::new(self.clone());
+                Enumerator::Iter(Box::new(Iter { iter, _object }))
+            }
+        }
+
+        Value::from_object(Iterable { maker, object })
+    }
+
+    /// Creates a value from a one-shot iterator.
+    ///
+    /// This takes an iterator (yielding values that can be turned into a [`Value`])
+    /// and wraps it in a way that it turns into an iterable value.  From the view of
+    /// the template this can be iterated over exactly once for the most part once
+    /// exhausted.
+    ///
+    /// Such iterators are strongly recommended against in the general sense due to
+    /// their surprising behavior, but they can be useful for more advanced use
+    /// cases where data should be streamed into the template as it becomes available.
+    ///
+    /// Such iterators never have any size hints.
+    ///
+    /// ```
+    /// # use minijinja::value::Value;
+    /// let val = Value::make_one_shot_iterator(0..10);
+    /// ```
+    ///
+    /// Attempting to iterate over it a second time will not yield any more items.
+    pub fn make_one_shot_iterator<I, T>(iter: I) -> Value
+    where
+        I: Iterator<Item = T> + Send + Sync + 'static,
+        T: Into<Value> + Send + Sync + 'static,
+    {
+        let iter = Arc::new(Mutex::new(iter.fuse()));
+        Value::make_iterable(move || {
+            let iter = iter.clone();
+            std::iter::from_fn(move || iter.lock().unwrap().next())
+        })
     }
 
     /// Creates a callable value from a function.
     ///
     /// ```
     /// # use minijinja::value::Value;
     /// let pow = Value::from_function(|a: u32| a * a);
@@ -697,26 +909,23 @@
     pub fn kind(&self) -> ValueKind {
         match self.0 {
             ValueRepr::Undefined => ValueKind::Undefined,
             ValueRepr::Bool(_) => ValueKind::Bool,
             ValueRepr::U64(_) | ValueRepr::I64(_) | ValueRepr::F64(_) => ValueKind::Number,
             ValueRepr::None => ValueKind::None,
             ValueRepr::I128(_) => ValueKind::Number,
-            ValueRepr::String(..) => ValueKind::String,
+            ValueRepr::String(..) | ValueRepr::SmallStr(_) => ValueKind::String,
             ValueRepr::Bytes(_) => ValueKind::Bytes,
             ValueRepr::U128(_) => ValueKind::Number,
-            ValueRepr::Seq(_) => ValueKind::Seq,
-            ValueRepr::Map(..) => ValueKind::Map,
-            // XXX: invalid values report themselves as maps which is a lie
-            ValueRepr::Invalid(_) => ValueKind::Map,
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                // XXX: basic objects should probably not report as map
-                ObjectKind::Plain => ValueKind::Map,
-                ObjectKind::Seq(_) => ValueKind::Seq,
-                ObjectKind::Struct(_) => ValueKind::Map,
+            ValueRepr::Invalid(_) => ValueKind::Invalid,
+            ValueRepr::Object(ref obj) => match obj.repr() {
+                ObjectRepr::Map => ValueKind::Map,
+                ObjectRepr::Seq => ValueKind::Seq,
+                ObjectRepr::Iterable => ValueKind::Iterable,
+                ObjectRepr::Plain => ValueKind::Plain,
             },
         }
     }
 
     /// Returns `true` if the value is a number.
     ///
     /// To convert a value into a primitive number, use [`TryFrom`] or [`TryInto`].
@@ -729,36 +938,35 @@
                 | ValueRepr::I128(_)
                 | ValueRepr::U128(_)
         )
     }
 
     /// Returns `true` if the map represents keyword arguments.
     pub fn is_kwargs(&self) -> bool {
-        matches!(self.0, ValueRepr::Map(_, MapType::Kwargs))
+        Kwargs::extract(self).is_some()
     }
 
-    /// Is this value true?
+    /// Is this value considered true?
+    ///
+    /// The engine inherits the same behavior as Jinja2 when it comes to
+    /// considering objects true.  Empty objects are generally not considered
+    /// true.  For custom objects this is customized by [`Object::is_true`].
     pub fn is_true(&self) -> bool {
         match self.0 {
             ValueRepr::Bool(val) => val,
             ValueRepr::U64(x) => x != 0,
             ValueRepr::U128(x) => x.0 != 0,
             ValueRepr::I64(x) => x != 0,
             ValueRepr::I128(x) => x.0 != 0,
             ValueRepr::F64(x) => x != 0.0,
             ValueRepr::String(ref x, _) => !x.is_empty(),
+            ValueRepr::SmallStr(ref x) => !x.is_empty(),
             ValueRepr::Bytes(ref x) => !x.is_empty(),
             ValueRepr::None | ValueRepr::Undefined | ValueRepr::Invalid(_) => false,
-            ValueRepr::Seq(ref x) => !x.is_empty(),
-            ValueRepr::Map(ref x, _) => !x.is_empty(),
-            ValueRepr::Dynamic(ref x) => match x.kind() {
-                ObjectKind::Plain => true,
-                ObjectKind::Seq(s) => s.item_count() != 0,
-                ObjectKind::Struct(s) => s.field_count() != 0,
-            },
+            ValueRepr::Object(ref x) => x.is_true(),
         }
     }
 
     /// Returns `true` if this value is safe.
     pub fn is_safe(&self) -> bool {
         matches!(&self.0, ValueRepr::String(_, StringType::Safe))
     }
@@ -770,127 +978,116 @@
 
     /// Returns `true` if this value is none.
     pub fn is_none(&self) -> bool {
         matches!(&self.0, ValueRepr::None)
     }
 
     /// If the value is a string, return it.
+    pub fn to_str(&self) -> Option<Arc<str>> {
+        match &self.0 {
+            ValueRepr::String(ref s, _) => Some(s.clone()),
+            ValueRepr::SmallStr(ref s) => Some(Arc::from(s.as_str())),
+            _ => None,
+        }
+    }
+
+    /// If the value is a string, return it.
     pub fn as_str(&self) -> Option<&str> {
         match &self.0 {
             ValueRepr::String(ref s, _) => Some(s as &str),
+            ValueRepr::SmallStr(ref s) => Some(s.as_str()),
             _ => None,
         }
     }
 
+    /// If this is an i64 return it
+    pub fn as_usize(&self) -> Option<usize> {
+        usize::try_from(self.clone()).ok()
+    }
+
+    /// If this is an i64 return it
+    pub fn as_i64(&self) -> Option<i64> {
+        i64::try_from(self.clone()).ok()
+    }
+
     /// Returns the bytes of this value if they exist.
     pub fn as_bytes(&self) -> Option<&[u8]> {
         match &self.0 {
             ValueRepr::String(ref s, _) => Some(s.as_bytes()),
+            ValueRepr::SmallStr(ref s) => Some(s.as_str().as_bytes()),
             ValueRepr::Bytes(ref b) => Some(&b[..]),
             _ => None,
         }
     }
 
-    /// If the value is an object, it's returned as [`Object`].
-    pub fn as_object(&self) -> Option<&dyn Object> {
+    /// If the value is an object a reference to it is returned.
+    ///
+    /// The returned value is a reference to a type erased [`DynObject`].
+    /// For a specific type use [`downcast_object`](Self::downcast_object)
+    /// instead.
+    pub fn as_object(&self) -> Option<&DynObject> {
         match self.0 {
-            ValueRepr::Dynamic(ref dy) => Some(&**dy as &dyn Object),
+            ValueRepr::Object(ref dy) => Some(dy),
             _ => None,
         }
     }
 
-    /// If the value is a sequence it's returned as [`SeqObject`].
-    pub fn as_seq(&self) -> Option<&dyn SeqObject> {
-        match self.0 {
-            ValueRepr::Seq(ref v) => return Some(&**v as &dyn SeqObject),
-            ValueRepr::Dynamic(ref dy) => {
-                if let ObjectKind::Seq(seq) = dy.kind() {
-                    return Some(seq);
-                }
-            }
-            _ => {}
-        }
-        None
-    }
-
-    /// If the value is a struct, return it as [`StructObject`].
-    pub fn as_struct(&self) -> Option<&dyn StructObject> {
-        if let ValueRepr::Dynamic(ref dy) = self.0 {
-            if let ObjectKind::Struct(s) = dy.kind() {
-                return Some(s);
-            }
-        }
-        None
-    }
-
     /// Returns the length of the contained value.
     ///
     /// Values without a length will return `None`.
     ///
     /// ```
     /// # use minijinja::value::Value;
     /// let seq = Value::from(vec![1, 2, 3, 4]);
     /// assert_eq!(seq.len(), Some(4));
     /// ```
     pub fn len(&self) -> Option<usize> {
         match self.0 {
             ValueRepr::String(ref s, _) => Some(s.chars().count()),
-            ValueRepr::Map(ref items, _) => Some(items.len()),
-            ValueRepr::Seq(ref items) => Some(items.len()),
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                ObjectKind::Plain => None,
-                ObjectKind::Seq(s) => Some(s.item_count()),
-                ObjectKind::Struct(s) => Some(s.field_count()),
-            },
+            ValueRepr::SmallStr(ref s) => Some(s.as_str().chars().count()),
+            ValueRepr::Object(ref dy) => dy.enumerator_len(),
             _ => None,
         }
     }
 
     /// Looks up an attribute by attribute name.
     ///
     /// This this returns [`UNDEFINED`](Self::UNDEFINED) when an invalid key is
-    /// resolved.  An error is returned when if the value does not contain an object
+    /// resolved.  An error is returned if the value does not contain an object
     /// that has attributes.
     ///
     /// ```
     /// # use minijinja::value::Value;
     /// # fn test() -> Result<(), minijinja::Error> {
     /// let ctx = minijinja::context! {
     ///     foo => "Foo"
     /// };
     /// let value = ctx.get_attr("foo")?;
     /// assert_eq!(value.to_string(), "Foo");
     /// # Ok(()) }
     /// ```
     pub fn get_attr(&self, key: &str) -> Result<Value, Error> {
-        Ok(match self.0 {
+        let value = match self.0 {
             ValueRepr::Undefined => return Err(Error::from(ErrorKind::UndefinedError)),
-            ValueRepr::Map(ref items, _) => items.get(&KeyRef::Str(key)).cloned(),
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                ObjectKind::Struct(s) => s.get_field(key),
-                ObjectKind::Plain | ObjectKind::Seq(_) => None,
-            },
+            ValueRepr::Object(ref dy) => dy.get_value(&Value::from(key)),
             _ => None,
-        }
-        .unwrap_or(Value::UNDEFINED))
+        };
+
+        Ok(value.unwrap_or(Value::UNDEFINED))
     }
 
     /// Alternative lookup strategy without error handling exclusively for context
     /// resolution.
     ///
     /// The main difference is that the return value will be `None` if the value is
     /// unable to look up the key rather than returning `Undefined` and errors will
     /// also not be created.
     pub(crate) fn get_attr_fast(&self, key: &str) -> Option<Value> {
         match self.0 {
-            ValueRepr::Map(ref items, _) => items.get(&KeyRef::Str(key)).cloned(),
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                ObjectKind::Struct(s) => s.get_field(key),
-                ObjectKind::Plain | ObjectKind::Seq(_) => None,
-            },
+            ValueRepr::Object(ref dy) => dy.get_value(&Value::from(key)),
             _ => None,
         }
     }
 
     /// Looks up an index of the value.
     ///
     /// This is a shortcut for [`get_item`](Self::get_item).
@@ -930,15 +1127,16 @@
 
     /// Iterates over the value.
     ///
     /// Depending on the [`kind`](Self::kind) of the value the iterator
     /// has a different behavior.
     ///
     /// * [`ValueKind::Map`]: the iterator yields the keys of the map.
-    /// * [`ValueKind::Seq`]: the iterator yields the items in the sequence.
+    /// * [`ValueKind::Seq`] / [`ValueKind::Iterable`]: the iterator yields the items in the sequence.
+    /// * [`ValueKind::String`]: the iterator yields characters in a string.
     /// * [`ValueKind::None`] / [`ValueKind::Undefined`]: the iterator is empty.
     ///
     /// ```
     /// # use minijinja::value::Value;
     /// # fn test() -> Result<(), minijinja::Error> {
     /// let value = Value::from({
     ///     let mut m = std::collections::BTreeMap::new();
@@ -948,133 +1146,188 @@
     /// });
     /// for key in value.try_iter()? {
     ///     let value = value.get_item(&key)?;
     ///     println!("{} = {}", key, value);
     /// }
     /// # Ok(()) }
     /// ```
-    pub fn try_iter(&self) -> Result<ValueIter<'_>, Error> {
-        self.try_iter_owned().map(|inner| ValueIter {
-            _marker: PhantomData,
-            inner,
+    pub fn try_iter(&self) -> Result<ValueIter, Error> {
+        match self.0 {
+            ValueRepr::None | ValueRepr::Undefined => Some(ValueIterImpl::Empty),
+            ValueRepr::String(ref s, _) => {
+                Some(ValueIterImpl::Chars(0, s.chars().count(), Arc::clone(s)))
+            }
+            ValueRepr::SmallStr(ref s) => Some(ValueIterImpl::Chars(
+                0,
+                s.as_str().chars().count(),
+                Arc::from(s.as_str()),
+            )),
+            ValueRepr::Object(ref obj) => obj.try_iter().map(ValueIterImpl::Dyn),
+            _ => None,
+        }
+        .map(|imp| ValueIter { imp })
+        .ok_or_else(|| {
+            Error::new(
+                ErrorKind::InvalidOperation,
+                format!("{} is not iterable", self.kind()),
+            )
+        })
+    }
+
+    /// Returns a reversed view of this value.
+    ///
+    /// This is implemented for the following types with the following behaviors:
+    ///
+    /// * undefined or none: value returned unchanged.
+    /// * string and bytes: returns a reversed version of that value
+    /// * iterables: returns a reversed version of the iterable.  If the iterable is not
+    ///   reversable itself, it consumes it and then reverses it.
+    pub fn reverse(&self) -> Result<Value, Error> {
+        match self.0 {
+            ValueRepr::Undefined | ValueRepr::None => Some(self.clone()),
+            ValueRepr::String(ref s, _) => Some(Value::from(s.chars().rev().collect::<String>())),
+            ValueRepr::SmallStr(ref s) => {
+                // TODO: add small str optimization here
+                Some(Value::from(s.as_str().chars().rev().collect::<String>()))
+            }
+            ValueRepr::Bytes(ref b) => {
+                Some(Value::from(b.iter().rev().copied().collect::<Vec<_>>()))
+            }
+            ValueRepr::Object(ref o) => match o.enumerate() {
+                Enumerator::NonEnumerable => None,
+                Enumerator::Empty => Some(Value::make_iterable(|| None::<Value>.into_iter())),
+                Enumerator::Seq(l) => {
+                    let self_clone = o.clone();
+                    Some(Value::make_iterable(move || {
+                        let self_clone = self_clone.clone();
+                        (0..l).rev().map(move |idx| {
+                            self_clone.get_value(&Value::from(idx)).unwrap_or_default()
+                        })
+                    }))
+                }
+                Enumerator::Iter(iter) => {
+                    let mut v = iter.collect::<Vec<_>>();
+                    v.reverse();
+                    Some(Value::make_object_iterable(v, move |v| {
+                        Box::new(v.iter().cloned())
+                    }))
+                }
+                Enumerator::RevIter(rev_iter) => {
+                    let for_restart = self.clone();
+                    let iter = Mutex::new(Some(rev_iter));
+                    Some(Value::make_iterable(move || {
+                        if let Some(iter) = iter.lock().unwrap().take() {
+                            Box::new(iter) as Box<dyn Iterator<Item = Value> + Send + Sync>
+                        } else {
+                            match for_restart.reverse().and_then(|x| x.try_iter()) {
+                                Ok(iterable) => Box::new(iterable)
+                                    as Box<dyn Iterator<Item = Value> + Send + Sync>,
+                                Err(err) => Box::new(Some(Value::from(err)).into_iter())
+                                    as Box<dyn Iterator<Item = Value> + Send + Sync>,
+                            }
+                        }
+                    }))
+                }
+                Enumerator::Str(s) => Some(Value::make_iterable(move || s.iter().rev().copied())),
+                Enumerator::Values(mut v) => {
+                    v.reverse();
+                    Some(Value::make_object_iterable(v, move |v| {
+                        Box::new(v.iter().cloned())
+                    }))
+                }
+            },
+            _ => None,
+        }
+        .ok_or_else(|| {
+            Error::new(
+                ErrorKind::InvalidOperation,
+                format!("cannot reverse values of type {}", self.kind()),
+            )
         })
     }
 
     /// Returns some reference to the boxed object if it is of type `T`, or None if it isn’t.
     ///
     /// This is basically the "reverse" of [`from_object`](Self::from_object),
-    /// [`from_seq_object`](Self::from_seq_object) and [`from_struct_object`](Self::from_struct_object).
-    /// It's also a shortcut for [`downcast_ref`](trait.Object.html#method.downcast_ref)
-    /// on the return value of [`as_object`](Self::as_object).
+    /// [`from_object`](Self::from_object) and
+    /// [`from_object`](Self::from_object). It's also a shortcut for
+    /// [`downcast_ref`](trait.Object.html#method.downcast_ref) on the return
+    /// value of [`as_object`](Self::as_object).
     ///
     /// # Example
     ///
     /// ```rust
     /// # use minijinja::value::{Value, Object};
     /// use std::fmt;
     ///
     /// #[derive(Debug)]
     /// struct Thing {
     ///     id: usize,
     /// }
     ///
-    /// impl fmt::Display for Thing {
-    ///     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-    ///         fmt::Debug::fmt(self, f)
-    ///     }
-    /// }
-    ///
     /// impl Object for Thing {}
     ///
     /// let x_value = Value::from_object(Thing { id: 42 });
     /// let thing = x_value.downcast_object_ref::<Thing>().unwrap();
     /// assert_eq!(thing.id, 42);
     /// ```
-    ///
-    /// It also works with [`SeqObject`] or [`StructObject`]:
-    ///
-    /// ```rust
-    /// # use minijinja::value::{Value, SeqObject};
-    ///
-    /// struct Thing {
-    ///     id: usize,
-    /// }
-    ///
-    /// impl SeqObject for Thing {
-    ///     fn get_item(&self, idx: usize) -> Option<Value> {
-    ///         (idx < 3).then(|| Value::from(idx))
-    ///     }
-    ///     fn item_count(&self) -> usize {
-    ///         3
-    ///     }
-    /// }
-    ///
-    /// let x_value = Value::from_seq_object(Thing { id: 42 });
-    /// let thing = x_value.downcast_object_ref::<Thing>().unwrap();
-    /// assert_eq!(thing.id, 42);
-    /// ```
     pub fn downcast_object_ref<T: 'static>(&self) -> Option<&T> {
-        self.as_object().and_then(|x| x.downcast_ref())
+        match self.0 {
+            ValueRepr::Object(ref o) => o.downcast_ref(),
+            _ => None,
+        }
+    }
+
+    /// Like [`downcast_object_ref`](Self::downcast_object_ref) but returns
+    /// the actual object.
+    pub fn downcast_object<T: 'static>(&self) -> Option<Arc<T>> {
+        match self.0 {
+            ValueRepr::Object(ref o) => o.downcast(),
+            _ => None,
+        }
     }
 
     pub(crate) fn get_item_opt(&self, key: &Value) -> Option<Value> {
-        let key = KeyRef::Value(key.clone());
+        fn index(value: &Value, len: impl Fn() -> Option<usize>) -> Option<usize> {
+            match value.as_i64().and_then(|v| isize::try_from(v).ok()) {
+                Some(i) if i < 0 => some!(len()).checked_sub(i.unsigned_abs()),
+                Some(i) => Some(i as usize),
+                None => None,
+            }
+        }
 
-        let seq = match self.0 {
-            ValueRepr::Map(ref items, _) => return items.get(&key).cloned(),
-            ValueRepr::Seq(ref items) => &**items as &dyn SeqObject,
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                ObjectKind::Plain => return None,
-                ObjectKind::Seq(s) => s,
-                ObjectKind::Struct(s) => {
-                    return if let Some(key) = key.as_str() {
-                        s.get_field(key)
-                    } else {
-                        None
-                    };
+        match self.0 {
+            ValueRepr::Object(ref dy) => match dy.repr() {
+                ObjectRepr::Map | ObjectRepr::Plain | ObjectRepr::Iterable => dy.get_value(key),
+                ObjectRepr::Seq => {
+                    let idx = index(key, || dy.enumerator_len()).map(Value::from);
+                    dy.get_value(idx.as_ref().unwrap_or(key))
                 }
             },
             ValueRepr::String(ref s, _) => {
-                if let Some(idx) = key.as_i64() {
-                    let idx = some!(isize::try_from(idx).ok());
-                    let idx = if idx < 0 {
-                        some!(s.chars().count().checked_sub(-idx as usize))
-                    } else {
-                        idx as usize
-                    };
-                    return s.chars().nth(idx).map(Value::from);
-                } else {
-                    return None;
-                }
+                let idx = some!(index(key, || Some(s.chars().count())));
+                s.chars().nth(idx).map(Value::from)
             }
-            _ => return None,
-        };
-
-        if let Some(idx) = key.as_i64() {
-            let idx = some!(isize::try_from(idx).ok());
-            let idx = if idx < 0 {
-                some!(seq.item_count().checked_sub(-idx as usize))
-            } else {
-                idx as usize
-            };
-            seq.get_item(idx)
-        } else {
-            None
+            ValueRepr::SmallStr(ref s) => {
+                let idx = some!(index(key, || Some(s.as_str().chars().count())));
+                s.as_str().chars().nth(idx).map(Value::from)
+            }
+            _ => None,
         }
     }
 
     /// Calls the value directly.
     ///
     /// If the value holds a function or macro, this invokes it.  Note that in
     /// MiniJinja there is a separate namespace for methods on objects and callable
     /// items.  To call methods (which should be a rather rare occurrence) you
     /// have to use [`call_method`](Self::call_method).
     ///
     /// The `args` slice is for the arguments of the function call.  To pass
-    /// keyword arguments use the [`Kwargs`](crate::value::Kwargs) type.
+    /// keyword arguments use the [`Kwargs`] type.
     ///
     /// Usually the state is already available when it's useful to call this method,
     /// but when it's not available you can get a fresh template state straight
     /// from the [`Template`](crate::Template) via [`new_state`](crate::Template::new_state).
     ///
     /// ```
     /// # use minijinja::{Environment, value::{Value, Kwargs}};
@@ -1107,94 +1360,50 @@
     /// let func = Value::from_function(|v: i64, kwargs: Kwargs| {
     ///     v * kwargs.get::<i64>("mult").unwrap_or(1)
     /// });
     /// let rv = func.call(state, args!(42, mult => 2)).unwrap();
     /// assert_eq!(rv, Value::from(84));
     /// ```
     pub fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
-        if let ValueRepr::Dynamic(ref dy) = self.0 {
+        if let ValueRepr::Object(ref dy) = self.0 {
             dy.call(state, args)
         } else {
             Err(Error::new(
                 ErrorKind::InvalidOperation,
                 format!("value of type {} is not callable", self.kind()),
             ))
         }
     }
 
     /// Calls a method on the value.
     ///
     /// The name of the method is `name`, the arguments passed are in the `args`
     /// slice.
     pub fn call_method(&self, state: &State, name: &str, args: &[Value]) -> Result<Value, Error> {
-        match self.0 {
-            ValueRepr::Dynamic(ref dy) => return dy.call_method(state, name, args),
-            ValueRepr::Map(ref map, _) => {
-                if let Some(value) = map.get(&KeyRef::Str(name)) {
-                    return value.call(state, args);
-                }
-            }
-            _ => {}
-        }
-        Err(Error::new(
-            ErrorKind::InvalidOperation,
-            format!("object has no method named {name}"),
-        ))
-    }
-
-    /// Iterates over the value without holding a reference.
-    pub(crate) fn try_iter_owned(&self) -> Result<OwnedValueIterator, Error> {
-        let (iter_state, len) = match self.0 {
-            ValueRepr::None | ValueRepr::Undefined => (ValueIteratorState::Empty, 0),
-            ValueRepr::String(ref s, _) => (
-                ValueIteratorState::Chars(0, Arc::clone(s)),
-                s.chars().count(),
-            ),
-            ValueRepr::Seq(ref seq) => (ValueIteratorState::Seq(0, Arc::clone(seq)), seq.len()),
-            #[cfg(feature = "preserve_order")]
-            ValueRepr::Map(ref items, _) => {
-                (ValueIteratorState::Map(0, Arc::clone(items)), items.len())
-            }
-            #[cfg(not(feature = "preserve_order"))]
-            ValueRepr::Map(ref items, _) => (
-                ValueIteratorState::Map(
-                    items.iter().next().map(|x| x.0.clone()),
-                    Arc::clone(items),
-                ),
-                items.len(),
-            ),
-            ValueRepr::Dynamic(ref obj) => {
-                match obj.kind() {
-                    ObjectKind::Plain => (ValueIteratorState::Empty, 0),
-                    ObjectKind::Seq(s) => (
-                        ValueIteratorState::DynSeq(0, Arc::clone(obj)),
-                        s.item_count(),
-                    ),
-                    ObjectKind::Struct(s) => {
-                        // the assumption is that structs don't have excessive field counts
-                        // and that most iterations go over all fields, so creating a
-                        // temporary vector here is acceptable.
-                        if let Some(fields) = s.static_fields() {
-                            (ValueIteratorState::StaticStr(0, fields), fields.len())
-                        } else {
-                            let attrs = s.fields();
-                            let attr_count = attrs.len();
-                            (ValueIteratorState::ArcStr(0, attrs), attr_count)
-                        }
+        match self._call_method(state, name, args) {
+            Ok(rv) => Ok(rv),
+            Err(mut err) => {
+                if err.kind() == ErrorKind::UnknownMethod {
+                    if let Some(ref callback) = state.env().unknown_method_callback {
+                        return callback(state, self, name, args);
+                    } else if err.detail().is_none() {
+                        err.set_detail(format!("{} has no method named {}", self.kind(), name));
                     }
                 }
+                Err(err)
             }
-            _ => {
-                return Err(Error::new(
-                    ErrorKind::InvalidOperation,
-                    format!("{} is not iterable", self.kind()),
-                ))
-            }
-        };
-        Ok(OwnedValueIterator { iter_state, len })
+        }
+    }
+
+    fn _call_method(&self, state: &State, name: &str, args: &[Value]) -> Result<Value, Error> {
+        if let Some(object) = self.as_object() {
+            object.call_method(state, name, args)
+        } else {
+            Err(Error::from(ErrorKind::UnknownMethod))
+        }
     }
 
     #[cfg(feature = "builtins")]
     pub(crate) fn get_path(&self, path: &str) -> Result<Value, Error> {
         let mut rv = self.clone();
         for part in path.split('.') {
             if let Ok(num) = part.parse::<usize>() {
@@ -1238,208 +1447,128 @@
             ValueRepr::F64(f) => serializer.serialize_f64(f),
             ValueRepr::None | ValueRepr::Undefined | ValueRepr::Invalid(_) => {
                 serializer.serialize_unit()
             }
             ValueRepr::U128(u) => serializer.serialize_u128(u.0),
             ValueRepr::I128(i) => serializer.serialize_i128(i.0),
             ValueRepr::String(ref s, _) => serializer.serialize_str(s),
+            ValueRepr::SmallStr(ref s) => serializer.serialize_str(s.as_str()),
             ValueRepr::Bytes(ref b) => serializer.serialize_bytes(b),
-            ValueRepr::Seq(ref elements) => elements.serialize(serializer),
-            ValueRepr::Map(ref entries, _) => {
-                use serde::ser::SerializeMap;
-                let mut map = ok!(serializer.serialize_map(Some(entries.len())));
-                for (ref k, ref v) in entries.iter() {
-                    ok!(map.serialize_entry(k, v));
-                }
-                map.end()
-            }
-            ValueRepr::Dynamic(ref dy) => match dy.kind() {
-                ObjectKind::Plain => serializer.serialize_str(&dy.to_string()),
-                ObjectKind::Seq(s) => {
+            ValueRepr::Object(ref o) => match o.repr() {
+                ObjectRepr::Plain => serializer.serialize_str(&o.to_string()),
+                ObjectRepr::Seq | ObjectRepr::Iterable => {
                     use serde::ser::SerializeSeq;
-                    let mut seq = ok!(serializer.serialize_seq(Some(s.item_count())));
-                    for item in s.iter() {
-                        ok!(seq.serialize_element(&item));
+                    let mut seq = ok!(serializer.serialize_seq(o.enumerator_len()));
+                    if let Some(iter) = o.try_iter() {
+                        for item in iter {
+                            ok!(seq.serialize_element(&item));
+                        }
                     }
+
                     seq.end()
                 }
-                ObjectKind::Struct(s) => {
+                ObjectRepr::Map => {
                     use serde::ser::SerializeMap;
                     let mut map = ok!(serializer.serialize_map(None));
-                    if let Some(fields) = s.static_fields() {
-                        for k in fields {
-                            let v = s.get_field(k).unwrap_or(Value::UNDEFINED);
-                            ok!(map.serialize_entry(k, &v));
-                        }
-                    } else {
-                        for k in s.fields() {
-                            let v = s.get_field(&k).unwrap_or(Value::UNDEFINED);
-                            ok!(map.serialize_entry(&*k as &str, &v));
+                    if let Some(iter) = o.try_iter_pairs() {
+                        for (key, value) in iter {
+                            ok!(map.serialize_entry(&key, &value));
                         }
                     }
+
                     map.end()
                 }
             },
         }
     }
 }
 
-/// Iterates over a value.
-pub struct ValueIter<'a> {
-    _marker: PhantomData<&'a Value>,
-    inner: OwnedValueIterator,
-}
-
-impl<'a> Iterator for ValueIter<'a> {
-    type Item = Value;
-
-    #[inline(always)]
-    fn next(&mut self) -> Option<Self::Item> {
-        self.inner.next()
-    }
-}
-
-pub(crate) struct OwnedValueIterator {
-    iter_state: ValueIteratorState,
-    len: usize,
+/// Utility to iterate over values.
+pub struct ValueIter {
+    imp: ValueIterImpl,
 }
 
-impl Iterator for OwnedValueIterator {
+impl Iterator for ValueIter {
     type Item = Value;
 
     fn next(&mut self) -> Option<Self::Item> {
-        self.iter_state.advance_state().map(|x| {
-            self.len -= 1;
-            x
-        })
+        match &mut self.imp {
+            ValueIterImpl::Empty => None,
+            ValueIterImpl::Chars(offset, len, ref s) => {
+                (s as &str)[*offset..].chars().next().map(|c| {
+                    *offset += c.len_utf8();
+                    *len -= 1;
+                    Value::from(c)
+                })
+            }
+            ValueIterImpl::Dyn(iter) => iter.next(),
+        }
     }
 
     fn size_hint(&self) -> (usize, Option<usize>) {
-        (self.len, Some(self.len))
+        match self.imp {
+            ValueIterImpl::Empty => (0, Some(0)),
+            ValueIterImpl::Chars(_, len, _) => (0, Some(len)),
+            ValueIterImpl::Dyn(ref iter) => iter.size_hint(),
+        }
     }
 }
 
-impl ExactSizeIterator for OwnedValueIterator {}
-
-impl fmt::Debug for OwnedValueIterator {
+impl fmt::Debug for ValueIter {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         f.debug_struct("ValueIterator").finish()
     }
 }
 
-enum ValueIteratorState {
+enum ValueIterImpl {
     Empty,
-    Chars(usize, Arc<str>),
-    Seq(usize, Arc<Vec<Value>>),
-    StaticStr(usize, &'static [&'static str]),
-    ArcStr(usize, Vec<Arc<str>>),
-    DynSeq(usize, Arc<dyn Object>),
-    #[cfg(not(feature = "preserve_order"))]
-    Map(Option<KeyRef<'static>>, Arc<ValueMap>),
-    #[cfg(feature = "preserve_order")]
-    Map(usize, Arc<ValueMap>),
+    Chars(usize, usize, Arc<str>),
+    Dyn(Box<dyn Iterator<Item = Value> + Send + Sync>),
 }
 
-impl ValueIteratorState {
-    fn advance_state(&mut self) -> Option<Value> {
-        match self {
-            ValueIteratorState::Empty => None,
-            ValueIteratorState::Chars(offset, ref s) => {
-                (s as &str)[*offset..].chars().next().map(|c| {
-                    *offset += c.len_utf8();
-                    Value::from(c)
-                })
-            }
-            ValueIteratorState::Seq(idx, items) => items
-                .get(*idx)
-                .map(|x| {
-                    *idx += 1;
-                    x
-                })
-                .cloned(),
-            ValueIteratorState::StaticStr(idx, items) => items.get(*idx).map(|x| {
-                *idx += 1;
-                Value::from(intern(x))
-            }),
-            ValueIteratorState::ArcStr(idx, items) => items.get(*idx).map(|x| {
-                *idx += 1;
-                Value::from(x.clone())
-            }),
-            ValueIteratorState::DynSeq(idx, obj) => {
-                if let ObjectKind::Seq(seq) = obj.kind() {
-                    seq.get_item(*idx).map(|x| {
-                        *idx += 1;
-                        x
-                    })
-                } else {
-                    unreachable!()
-                }
-            }
-            #[cfg(feature = "preserve_order")]
-            ValueIteratorState::Map(idx, map) => map.get_index(*idx).map(|x| {
-                *idx += 1;
-                x.0.as_value()
-            }),
-            #[cfg(not(feature = "preserve_order"))]
-            ValueIteratorState::Map(ptr, map) => {
-                if let Some(current) = ptr.take() {
-                    let next = map.range(&current..).nth(1).map(|x| x.0.clone());
-                    let rv = current.as_value();
-                    *ptr = next;
-                    Some(rv)
-                } else {
-                    None
-                }
-            }
-        }
+impl From<Error> for Value {
+    fn from(value: Error) -> Self {
+        Value(ValueRepr::Invalid(Arc::new(value)))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     use similar_asserts::assert_eq;
 
     #[test]
     fn test_dynamic_object_roundtrip() {
         use std::sync::atomic::{self, AtomicUsize};
 
-        #[derive(Debug)]
-        struct X(AtomicUsize);
-
-        impl fmt::Display for X {
-            fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-                write!(f, "{}", self.0.load(atomic::Ordering::Relaxed))
-            }
-        }
+        #[derive(Debug, Clone)]
+        struct X(Arc<AtomicUsize>);
 
         impl Object for X {
-            fn kind(&self) -> ObjectKind<'_> {
-                ObjectKind::Struct(self)
-            }
-        }
-
-        impl crate::value::object::StructObject for X {
-            fn get_field(&self, name: &str) -> Option<Value> {
-                match name {
+            fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+                match key.as_str()? {
                     "value" => Some(Value::from(self.0.load(atomic::Ordering::Relaxed))),
                     _ => None,
                 }
             }
 
-            fn static_fields(&self) -> Option<&'static [&'static str]> {
-                Some(&["value"][..])
+            fn enumerate(self: &Arc<Self>) -> Enumerator {
+                Enumerator::Str(&["value"])
+            }
+
+            fn render(self: &Arc<Self>, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+                write!(f, "{}", self.0.load(atomic::Ordering::Relaxed))
             }
         }
 
         let x = Arc::new(X(Default::default()));
-        let x_value = Value::from(x.clone());
+        let x_value = Value::from_dyn_object(x.clone());
         x.0.fetch_add(42, atomic::Ordering::Relaxed);
-        let x_clone = Value::from_serializable(&x_value);
+        let x_clone = Value::from_serialize(&x_value);
         x.0.fetch_add(23, atomic::Ordering::Relaxed);
 
         assert_eq!(x_value.to_string(), "65");
         assert_eq!(x_clone.to_string(), "65");
     }
 
     #[test]
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/ops.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/ops.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-use std::convert::{TryFrom, TryInto};
-
 use crate::error::{Error, ErrorKind};
-use crate::value::{KeyRef, ObjectKind, SeqObject, Value, ValueKind, ValueRepr};
+use crate::value::{ObjectRepr, Value, ValueKind, ValueRepr};
 
 const MIN_I128_AS_POS_U128: u128 = 170141183460469231731687303715884105728;
 
 pub enum CoerceResult<'a> {
     I128(i128, i128),
     F64(f64, f64),
     Str(&'a str, &'a str),
@@ -27,14 +25,19 @@
     match (&a.0, &b.0) {
         // equal mappings are trivial
         (ValueRepr::U64(a), ValueRepr::U64(b)) => Some(CoerceResult::I128(*a as i128, *b as i128)),
         (ValueRepr::U128(a), ValueRepr::U128(b)) => {
             Some(CoerceResult::I128(a.0 as i128, b.0 as i128))
         }
         (ValueRepr::String(a, _), ValueRepr::String(b, _)) => Some(CoerceResult::Str(a, b)),
+        (ValueRepr::SmallStr(a), ValueRepr::SmallStr(b)) => {
+            Some(CoerceResult::Str(a.as_str(), b.as_str()))
+        }
+        (ValueRepr::SmallStr(a), ValueRepr::String(b, _)) => Some(CoerceResult::Str(a.as_str(), b)),
+        (ValueRepr::String(a, _), ValueRepr::SmallStr(b)) => Some(CoerceResult::Str(a, b.as_str())),
         (ValueRepr::I64(a), ValueRepr::I64(b)) => Some(CoerceResult::I128(*a as i128, *b as i128)),
         (ValueRepr::I128(a), ValueRepr::I128(b)) => Some(CoerceResult::I128(a.0, b.0)),
         (ValueRepr::F64(a), ValueRepr::F64(b)) => Some(CoerceResult::F64(*a, *b)),
 
         // are floats involved?
         (ValueRepr::F64(a), _) => Some(CoerceResult::F64(*a, some!(as_f64(b)))),
         (_, ValueRepr::F64(b)) => Some(CoerceResult::F64(some!(as_f64(a)), *b)),
@@ -92,53 +95,46 @@
     if step == 0 {
         return Err(Error::new(
             ErrorKind::InvalidOperation,
             "cannot slice by step size of 0",
         ));
     }
 
-    let maybe_seq = match value.0 {
-        ValueRepr::String(..) => {
+    let kind = value.kind();
+    let error = Err(Error::new(
+        ErrorKind::InvalidOperation,
+        format!("value of type {} cannot be sliced", kind),
+    ));
+
+    match value.0 {
+        ValueRepr::String(..) | ValueRepr::SmallStr(_) => {
             let s = value.as_str().unwrap();
             let (start, len) = get_offset_and_len(start, stop, || s.chars().count());
-            return Ok(Value::from(
+            Ok(Value::from(
                 s.chars()
                     .skip(start)
                     .take(len)
                     .step_by(step)
                     .collect::<String>(),
-            ));
-        }
-        ValueRepr::Undefined | ValueRepr::None => return Ok(Value::from(Vec::<Value>::new())),
-        ValueRepr::Seq(ref s) => Some(&**s as &dyn SeqObject),
-        ValueRepr::Dynamic(ref dy) => {
-            if let ObjectKind::Seq(seq) = dy.kind() {
-                Some(seq)
-            } else {
-                None
-            }
-        }
-        _ => None,
-    };
-
-    match maybe_seq {
-        Some(seq) => {
-            let (start, len) = get_offset_and_len(start, stop, || seq.item_count());
-            Ok(Value::from(
-                seq.iter()
-                    .skip(start)
-                    .take(len)
-                    .step_by(step)
-                    .collect::<Vec<_>>(),
             ))
         }
-        None => Err(Error::new(
-            ErrorKind::InvalidOperation,
-            format!("value of type {} cannot be sliced", value.kind()),
-        )),
+        ValueRepr::Undefined | ValueRepr::None => Ok(Value::from(Vec::<Value>::new())),
+        ValueRepr::Object(obj) if matches!(obj.repr(), ObjectRepr::Seq | ObjectRepr::Iterable) => {
+            Ok(Value::make_object_iterable(obj, move |obj| {
+                let len = obj.enumerator_len().unwrap_or_default();
+                let (start, len) = get_offset_and_len(start, stop, || len);
+                // The manual match here is important that we do not mess up the size_hint
+                if let Some(iter) = obj.try_iter() {
+                    Box::new(iter.skip(start).take(len).step_by(step))
+                } else {
+                    Box::new(None.into_iter())
+                }
+            }))
+        }
+        _ => error,
     }
 }
 
 fn int_as_value(val: i128) -> Value {
     if val as i64 as i128 == val {
         (val as i64).into()
     } else {
@@ -177,14 +173,29 @@
                 _ => Err(impossible_op(stringify!($float), lhs, rhs))
             }
         }
     }
 }
 
 pub fn add(lhs: &Value, rhs: &Value) -> Result<Value, Error> {
+    if matches!(lhs.kind(), ValueKind::Seq | ValueKind::Iterable)
+        && matches!(rhs.kind(), ValueKind::Seq | ValueKind::Iterable)
+    {
+        let lhs = lhs.clone();
+        let rhs = rhs.clone();
+        return Ok(Value::make_iterable(move || {
+            if let Ok(lhs) = lhs.try_iter() {
+                if let Ok(rhs) = rhs.try_iter() {
+                    return Box::new(lhs.chain(rhs))
+                        as Box<dyn Iterator<Item = Value> + Send + Sync>;
+                }
+            }
+            Box::new(None.into_iter()) as Box<dyn Iterator<Item = Value> + Send + Sync>
+        }));
+    }
     match coerce(lhs, rhs) {
         Some(CoerceResult::I128(a, b)) => a
             .checked_add(b)
             .ok_or_else(|| failed_op("+", lhs, rhs))
             .map(int_as_value),
         Some(CoerceResult::F64(a, b)) => Ok((a + b).into()),
         Some(CoerceResult::Str(a, b)) => Ok(Value::from([a, b].concat())),
@@ -274,18 +285,22 @@
     }
     let rv = if let Some(s) = container.as_str() {
         if let Some(s2) = value.as_str() {
             s.contains(s2)
         } else {
             s.contains(&value.to_string())
         }
-    } else if let Some(seq) = container.as_seq() {
-        seq.iter().any(|item| &item == value)
-    } else if let ValueRepr::Map(ref map, _) = container.0 {
-        map.get(&KeyRef::Value(value.clone())).is_some()
+    } else if let ValueRepr::Object(ref obj) = container.0 {
+        match obj.repr() {
+            ObjectRepr::Plain => false,
+            ObjectRepr::Map => obj.get_value(value).is_some(),
+            ObjectRepr::Seq | ObjectRepr::Iterable => {
+                obj.try_iter().into_iter().flatten().any(|v| &v == value)
+            }
+        }
     } else {
         return Err(Error::new(
             ErrorKind::InvalidOperation,
             "cannot perform a containment check on this value",
         ));
     };
     Ok(Value::from(rv))
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/value/serialize.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/value/serialize.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 use std::collections::BTreeMap;
 use std::fmt;
 
 use serde::{ser, Serialize, Serializer};
 
+use crate::error::{Error, ErrorKind};
 use crate::utils::untrusted_size_hint;
 use crate::value::{
-    value_map_with_capacity, Arc, KeyRef, MapType, Packed, StringType, Value, ValueMap, ValueRepr,
-    VALUE_HANDLES, VALUE_HANDLE_MARKER,
+    value_map_with_capacity, Arc, Packed, Value, ValueMap, ValueRepr, VALUE_HANDLES,
+    VALUE_HANDLE_MARKER,
 };
 
 #[derive(Debug)]
-pub struct InvalidValue(Arc<str>);
+pub struct InvalidValue(String);
 
 impl std::error::Error for InvalidValue {}
 
 impl fmt::Display for InvalidValue {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         self.0.fmt(f)
     }
 }
 
 impl serde::ser::Error for InvalidValue {
     fn custom<T>(msg: T) -> Self
     where
         T: fmt::Display,
     {
-        InvalidValue(Arc::from(msg.to_string()))
+        InvalidValue(msg.to_string())
     }
 }
 
 /// Transforms a serializable value to a value object.
 ///
 /// This neither fails nor panics.  For objects that cannot be represented
 /// the value might be represented as a half broken error object.
 pub fn transform<T: Serialize>(value: T) -> Value {
     match value.serialize(ValueSerializer) {
         Ok(rv) => rv,
-        Err(invalid) => ValueRepr::Invalid(invalid.0).into(),
+        Err(invalid) => Value::from(Error::new(ErrorKind::BadSerialization, invalid.0)),
     }
 }
 
 pub struct ValueSerializer;
 
 impl Serializer for ValueSerializer {
     type Ok = Value;
@@ -103,19 +104,19 @@
     }
 
     fn serialize_f64(self, v: f64) -> Result<Value, InvalidValue> {
         Ok(ValueRepr::F64(v).into())
     }
 
     fn serialize_char(self, v: char) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::String(Arc::from(v.to_string()), StringType::Normal).into())
+        Ok(Value::from(v))
     }
 
     fn serialize_str(self, value: &str) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::String(Arc::from(value.to_owned()), StringType::Normal).into())
+        Ok(Value::from(value))
     }
 
     fn serialize_bytes(self, value: &[u8]) -> Result<Value, InvalidValue> {
         Ok(ValueRepr::Bytes(Arc::new(value.to_owned())).into())
     }
 
     fn serialize_none(self) -> Result<Value, InvalidValue> {
@@ -173,16 +174,16 @@
         variant: &'static str,
         value: &T,
     ) -> Result<Value, InvalidValue>
     where
         T: Serialize,
     {
         let mut map = value_map_with_capacity(1);
-        map.insert(KeyRef::Str(variant), transform(value));
-        Ok(ValueRepr::Map(Arc::new(map), MapType::Normal).into())
+        map.insert(variant.into(), transform(value));
+        Ok(Value::from_object(map))
     }
 
     fn serialize_seq(self, len: Option<usize>) -> Result<Self::SerializeSeq, InvalidValue> {
         Ok(SerializeSeq {
             elements: Vec::with_capacity(untrusted_size_hint(len.unwrap_or(0))),
         })
     }
@@ -260,15 +261,15 @@
         T: Serialize,
     {
         self.elements.push(transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::Seq(Arc::new(self.elements)).into())
+        Ok(Value::from_object(self.elements))
     }
 }
 
 pub struct SerializeTuple {
     elements: Vec<Value>,
 }
 
@@ -281,15 +282,15 @@
         T: Serialize,
     {
         self.elements.push(transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::Seq(Arc::new(self.elements)).into())
+        Ok(Value::from_object(self.elements))
     }
 }
 
 pub struct SerializeTupleStruct {
     fields: Vec<Value>,
 }
 
@@ -302,15 +303,15 @@
         T: Serialize,
     {
         self.fields.push(transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
-        Ok(Value(ValueRepr::Seq(Arc::new(self.fields))))
+        Ok(Value::from_object(self.fields))
     }
 }
 
 pub struct SerializeTupleVariant {
     name: &'static str,
     fields: Vec<Value>,
 }
@@ -325,19 +326,16 @@
     {
         self.fields.push(transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         let mut map = value_map_with_capacity(1);
-        map.insert(
-            KeyRef::Str(self.name),
-            Value(ValueRepr::Seq(self.fields.into())),
-        );
-        Ok(Value(ValueRepr::Map(map.into(), MapType::Normal)))
+        map.insert(self.name.into(), Value::from_object(self.fields));
+        Ok(Value::from_object(map))
     }
 }
 
 pub struct SerializeMap {
     entries: ValueMap,
     key: Option<Value>,
 }
@@ -358,37 +356,34 @@
     }
 
     fn serialize_value<T: ?Sized>(&mut self, value: &T) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
         if let Some(key) = self.key.take() {
-            self.entries.insert(KeyRef::Value(key), transform(value));
+            self.entries.insert(key, transform(value));
         }
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
-        Ok(Value(ValueRepr::Map(
-            Arc::new(self.entries),
-            MapType::Normal,
-        )))
+        Ok(Value::from_object(self.entries))
     }
 
     fn serialize_entry<K: ?Sized, V: ?Sized>(
         &mut self,
         key: &K,
         value: &V,
     ) -> Result<(), InvalidValue>
     where
         K: Serialize,
         V: Serialize,
     {
         if let Ok(key) = key.serialize(ValueSerializer) {
-            self.entries.insert(KeyRef::Value(key), transform(value));
+            self.entries.insert(key, transform(value));
         }
         Ok(())
     }
 }
 
 pub struct SerializeStruct {
     fields: ValueMap,
@@ -402,20 +397,20 @@
         &mut self,
         key: &'static str,
         value: &T,
     ) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
-        self.fields.insert(KeyRef::Str(key), transform(value));
+        self.fields.insert(key.into(), transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
-        Ok(ValueRepr::Map(Arc::new(self.fields), MapType::Normal).into())
+        Ok(Value::from_object(self.fields))
     }
 }
 
 pub struct SerializeStructVariant {
     variant: &'static str,
     map: ValueMap,
 }
@@ -428,20 +423,17 @@
         &mut self,
         key: &'static str,
         value: &T,
     ) -> Result<(), InvalidValue>
     where
         T: Serialize,
     {
-        self.map.insert(KeyRef::Str(key), transform(value));
+        self.map.insert(key.into(), transform(value));
         Ok(())
     }
 
     fn end(self) -> Result<Value, InvalidValue> {
         let mut rv = BTreeMap::new();
-        rv.insert(
-            self.variant,
-            Value::from(ValueRepr::Map(Arc::new(self.map), MapType::Normal)),
-        );
+        rv.insert(self.variant.to_string(), Value::from_object(self.map));
         Ok(rv.into())
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/context.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/context.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 use std::borrow::Cow;
 use std::collections::{BTreeMap, HashSet};
 use std::fmt;
 use std::sync::Arc;
 
 use crate::environment::Environment;
 use crate::error::{Error, ErrorKind};
-use crate::value::{OwnedValueIterator, Value, ValueRepr};
-use crate::vm::closure_object::Closure;
+use crate::value::{Value, ValueIter};
 use crate::vm::loop_object::Loop;
 
-type Locals<'env> = BTreeMap<&'env str, Value>;
+#[cfg(feature = "macros")]
+use crate::vm::closure_object::Closure;
 
-/// The maximum recursion in the VM.  Normally each stack frame
-/// adds one to this counter (eg: every time a frame is added).
-/// However in some situations more depth is pushed if the cost
-/// of the stack frame is higher.
-const MAX_RECURSION: usize = 500;
+type Locals<'env> = BTreeMap<&'env str, Value>;
 
 pub(crate) struct LoopState {
     pub(crate) with_loop_var: bool,
     pub(crate) recurse_jump_target: Option<usize>,
     // if we're popping the frame, do we want to jump somewhere?  The
     // first item is the target jump instruction, the second argument
     // tells us if we need to end capturing.
     pub(crate) current_recursion_jump: Option<(usize, bool)>,
-    pub(crate) iterator: OwnedValueIterator,
+    pub(crate) iterator: ValueIter,
     pub(crate) object: Arc<Loop>,
 }
 
 pub(crate) struct Frame<'env> {
     pub(crate) locals: Locals<'env>,
     pub(crate) ctx: Value,
     pub(crate) current_loop: Option<LoopState>,
 
     // normally a frame does not carry a closure, but it can when a macro is
     // declared.  Once that happens, all writes to the frames locals are also
     // duplicated into the closure.  Macros declared on that level, then share
     // the closure object to enclose the parent values.  This emulates the
     // behavior of closures in Jinja2.
+    #[cfg(feature = "macros")]
     pub(crate) closure: Option<Arc<Closure>>,
 }
 
 impl<'env> Default for Frame<'env> {
     fn default() -> Frame<'env> {
         Frame::new(Value::UNDEFINED)
     }
@@ -50,25 +47,22 @@
 impl<'env> Frame<'env> {
     /// Creates a new frame with the given context and no validation
     pub fn new(ctx: Value) -> Frame<'env> {
         Frame {
             locals: Locals::new(),
             ctx,
             current_loop: None,
+            #[cfg(feature = "macros")]
             closure: None,
         }
     }
 
-    /// Creates a new frame with the given context and validates the the value is not invalid
+    /// Creates a new frame with the given context and validates the value is not invalid
     pub fn new_checked(root: Value) -> Result<Frame<'env>, Error> {
-        if let ValueRepr::Invalid(ref err) = root.0 {
-            Err(Error::new(ErrorKind::BadSerialization, err.to_string()))
-        } else {
-            Ok(Frame::new(root))
-        }
+        Ok(Frame::new(ok!(root.validate())))
     }
 }
 
 #[cfg(feature = "internal_debug")]
 impl<'env> fmt::Debug for Frame<'env> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut m = f.debug_map();
@@ -106,14 +100,19 @@
     }
 
     #[track_caller]
     pub fn pop(&mut self) -> Value {
         self.values.pop().unwrap()
     }
 
+    pub fn reverse_top(&mut self, n: usize) {
+        let start = self.values.len() - n;
+        self.values[start..].reverse();
+    }
+
     pub fn slice_top(&mut self, n: usize) -> &[Value] {
         &self.values[self.values.len() - n..]
     }
 
     pub fn drop_top(&mut self, n: usize) {
         self.values.truncate(self.values.len() - n);
     }
@@ -133,14 +132,15 @@
         Stack { values }
     }
 }
 
 pub(crate) struct Context<'env> {
     stack: Vec<Frame<'env>>,
     outer_stack_depth: usize,
+    recursion_limit: usize,
 }
 
 impl<'env> fmt::Debug for Context<'env> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         fn dump<'a>(
             m: &mut std::fmt::DebugMap,
             seen: &mut HashSet<Cow<'a, str>>,
@@ -180,76 +180,82 @@
         let mut m = f.debug_map();
         let mut seen = HashSet::new();
         ok!(dump(&mut m, &mut seen, self));
         m.finish()
     }
 }
 
-impl<'env> Default for Context<'env> {
-    fn default() -> Context<'env> {
+impl<'env> Context<'env> {
+    /// Creates an empty context.
+    pub fn new(recursion_limit: usize) -> Context<'env> {
         Context {
             stack: Vec::with_capacity(32),
             outer_stack_depth: 0,
+            recursion_limit,
         }
     }
-}
 
-impl<'env> Context<'env> {
     /// Creates a context
-    pub fn new(frame: Frame<'env>) -> Context<'env> {
-        let mut rv = Context::default();
+    pub fn new_with_frame(frame: Frame<'env>, recursion_limit: usize) -> Context<'env> {
+        let mut rv = Context::new(recursion_limit);
         rv.stack.push(frame);
         rv
     }
 
     /// Stores a variable in the context.
     pub fn store(&mut self, key: &'env str, value: Value) {
         let top = self.stack.last_mut().unwrap();
-        if let Some(ref closure) = top.closure {
-            closure.store(key, value.clone());
+        #[cfg(feature = "macros")]
+        {
+            if let Some(ref closure) = top.closure {
+                closure.store(key, value.clone());
+            }
         }
         top.locals.insert(key, value);
     }
 
     /// Adds a value to a closure if missing.
     ///
     /// All macros declare on a certain level reuse the same closure.  This is done
     /// to emulate the behavior of how scopes work in Jinja2 in Python.  The
     /// unfortunate downside is that this has to be done with a `Mutex`.
     #[cfg(feature = "macros")]
     pub fn enclose(&mut self, env: &Environment, key: &str) {
-        self.closure()
+        self.stack
+            .last_mut()
+            .unwrap()
+            .closure
+            .as_mut()
+            .unwrap()
+            .clone()
             .store_if_missing(key, || self.load(env, key).unwrap_or(Value::UNDEFINED));
     }
 
     /// Loads the closure and returns it.
     #[cfg(feature = "macros")]
-    pub fn closure(&mut self) -> Arc<Closure> {
-        let top = self.stack.last_mut().unwrap();
-        top.closure
-            .get_or_insert_with(|| Arc::new(Closure::default()))
-            .clone()
+    pub fn closure(&mut self) -> Option<&Arc<Closure>> {
+        self.stack.last_mut().unwrap().closure.as_ref()
     }
 
     /// Temporarily takes the closure.
     ///
     /// This is done because includes are in the same scope as the module that
     /// triggers the import, but we do not want to allow closures to be modified
     /// from another file as this would be very confusing.
     ///
     /// This means that if you override a variable referenced by a macro after
     /// including in the parent template, it will not override the value seen by
     /// the macro.
-    #[cfg(feature = "multi_template")]
+    #[cfg(all(feature = "multi_template", feature = "macros"))]
     pub fn take_closure(&mut self) -> Option<Arc<Closure>> {
         self.stack.last_mut().unwrap().closure.take()
     }
 
     /// Puts the closure back.
-    #[cfg(feature = "multi_template")]
+    #[cfg(feature = "macros")]
     pub fn reset_closure(&mut self, closure: Option<Arc<Closure>>) {
         self.stack.last_mut().unwrap().closure = closure;
     }
 
     /// Looks up a variable in the context.
     pub fn load(&self, env: &Environment, key: &str) -> Option<Value> {
         for frame in self.stack.iter().rev() {
@@ -257,15 +263,15 @@
             if let Some(value) = frame.locals.get(key) {
                 return Some(value.clone());
             }
 
             // if we are a loop, check if we are looking up the special loop var.
             if let Some(ref l) = frame.current_loop {
                 if l.with_loop_var && key == "loop" {
-                    return Some(Value::from(l.object.clone()));
+                    return Some(Value::from_dyn_object(l.object.clone()));
                 }
             }
 
             // perform a fast lookup.  This one will not produce errors if the
             // context is undefined or of the wrong type.
             if let Some(rv) = frame.ctx.get_attr_fast(key) {
                 return Some(rv);
@@ -326,15 +332,15 @@
     /// Decrease the stack depth.
     #[allow(unused)]
     pub fn decr_depth(&mut self, delta: usize) {
         self.outer_stack_depth -= delta;
     }
 
     fn check_depth(&self) -> Result<(), Error> {
-        if self.depth() > MAX_RECURSION {
+        if self.depth() > self.recursion_limit {
             return Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "recursion limit exceeded",
             ));
         }
         Ok(())
     }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/fuel.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/fuel.rs`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/loop_object.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/loop_object.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 use std::fmt;
 use std::sync::atomic::{AtomicUsize, Ordering};
-use std::sync::Mutex;
+use std::sync::{Arc, Mutex};
 
 use crate::error::{Error, ErrorKind};
-use crate::value::{Object, ObjectKind, StructObject, Value};
+use crate::value::{Enumerator, Object, Value};
 use crate::vm::state::State;
 
 pub(crate) struct Loop {
-    pub len: usize,
+    pub len: Option<usize>,
     pub idx: AtomicUsize,
     pub depth: usize,
     #[cfg(feature = "adjacent_loop_items")]
     pub value_triple: Mutex<(Option<Value>, Option<Value>, Option<Value>)>,
     pub last_changed_value: Mutex<Option<Vec<Value>>>,
 }
 
 impl fmt::Debug for Loop {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        let mut s = f.debug_struct("Loop");
-        for attr in self.static_fields().unwrap() {
-            s.field(attr, &self.get_field(attr).unwrap());
-        }
-        s.finish()
+        f.debug_struct("Loop")
+            .field("len", &self.len)
+            .field("idx", &self.idx)
+            .field("depth", &self.depth)
+            .finish()
     }
 }
 
 impl Object for Loop {
-    fn kind(&self) -> ObjectKind<'_> {
-        ObjectKind::Struct(self)
-    }
-
-    fn call(&self, _state: &State, _args: &[Value]) -> Result<Value, Error> {
+    fn call(self: &Arc<Self>, _state: &State, _args: &[Value]) -> Result<Value, Error> {
         Err(Error::new(
             ErrorKind::InvalidOperation,
             "loop cannot be called if reassigned to different variable",
         ))
     }
 
-    fn call_method(&self, _state: &State, name: &str, args: &[Value]) -> Result<Value, Error> {
+    fn call_method(
+        self: &Arc<Self>,
+        _state: &State,
+        name: &str,
+        args: &[Value],
+    ) -> Result<Value, Error> {
         if name == "changed" {
             let mut last_changed_value = self.last_changed_value.lock().unwrap();
             let value = args.to_owned();
             let changed = last_changed_value.as_ref() != Some(&value);
             if changed {
                 *last_changed_value = Some(value);
                 Ok(Value::from(true))
@@ -51,60 +52,62 @@
         } else if name == "cycle" {
             let idx = self.idx.load(Ordering::Relaxed);
             match args.get(idx % args.len()) {
                 Some(arg) => Ok(arg.clone()),
                 None => Ok(Value::UNDEFINED),
             }
         } else {
-            Err(Error::new(
-                ErrorKind::UnknownMethod,
-                format!("loop object has no method named {name}"),
-            ))
+            Err(Error::from(ErrorKind::UnknownMethod))
         }
     }
-}
 
-impl StructObject for Loop {
-    fn static_fields(&self) -> Option<&'static [&'static str]> {
-        Some(
-            &[
-                "index0",
-                "index",
-                "length",
-                "revindex",
-                "revindex0",
-                "first",
-                "last",
-                "depth",
-                "depth0",
-                #[cfg(feature = "adjacent_loop_items")]
-                "previtem",
-                #[cfg(feature = "adjacent_loop_items")]
-                "nextitem",
-            ][..],
-        )
+    fn enumerate(self: &Arc<Self>) -> Enumerator {
+        Enumerator::Str(&[
+            "index0",
+            "index",
+            "length",
+            "revindex",
+            "revindex0",
+            "first",
+            "last",
+            "depth",
+            "depth0",
+            #[cfg(feature = "adjacent_loop_items")]
+            "previtem",
+            #[cfg(feature = "adjacent_loop_items")]
+            "nextitem",
+        ])
     }
 
-    fn get_field(&self, name: &str) -> Option<Value> {
+    fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+        let key = some!(key.as_str());
         let idx = self.idx.load(Ordering::Relaxed) as u64;
         // if we never iterated, then all attributes are undefined.
         // this can happen in some rare circumstances where the engine
         // did not manage to iterate
         if idx == !0 {
             return Some(Value::UNDEFINED);
         }
-        let len = self.len as u64;
-        match name {
+        let len = self.len.map(|x| x as u64);
+        match key {
             "index0" => Some(Value::from(idx)),
             "index" => Some(Value::from(idx + 1)),
-            "length" => Some(Value::from(len)),
-            "revindex" => Some(Value::from(len.saturating_sub(idx))),
-            "revindex0" => Some(Value::from(len.saturating_sub(idx).saturating_sub(1))),
+            "length" => Some(len.map(Value::from).unwrap_or(Value::UNDEFINED)),
+            "revindex" => Some(
+                len.map(|len| Value::from(len.saturating_sub(idx)))
+                    .unwrap_or(Value::UNDEFINED),
+            ),
+            "revindex0" => Some(
+                len.map(|len| Value::from(len.saturating_sub(idx).saturating_sub(1)))
+                    .unwrap_or(Value::UNDEFINED),
+            ),
             "first" => Some(Value::from(idx == 0)),
-            "last" => Some(Value::from(len == 0 || idx == len - 1)),
+            "last" => Some(len.map_or(Value::from(false), |len| {
+                Value::from(len == 0 || idx == len - 1)
+            })),
             "depth" => Some(Value::from(self.depth + 1)),
             "depth0" => Some(Value::from(self.depth)),
             #[cfg(feature = "adjacent_loop_items")]
             "previtem" => Some(
                 self.value_triple
                     .lock()
                     .unwrap()
@@ -120,19 +123,20 @@
                     .2
                     .clone()
                     .unwrap_or(Value::UNDEFINED),
             ),
             _ => None,
         }
     }
-}
 
-impl fmt::Display for Loop {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+    fn render(self: &Arc<Self>, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(
             f,
             "<loop {}/{}>",
             self.idx.load(Ordering::Relaxed),
-            self.len
+            match self.len {
+                Some(ref len) => len as &dyn fmt::Display,
+                None => &"?" as &dyn fmt::Display,
+            },
         )
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/macro_object.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/macro_object.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 use std::collections::BTreeSet;
 use std::fmt;
 use std::sync::Arc;
 
 use crate::error::{Error, ErrorKind};
 use crate::output::Output;
 use crate::utils::AutoEscape;
-use crate::value::{
-    KeyRef, MapType, Object, ObjectKind, StringType, StructObject, Value, ValueRepr,
-};
+use crate::value::{Enumerator, Kwargs, Object, Value};
 use crate::vm::state::State;
 use crate::vm::Vm;
 
-pub(crate) struct MacroData {
-    pub name: Arc<str>,
-    pub arg_spec: Vec<Arc<str>>,
+pub(crate) struct Macro {
+    pub name: Value,
+    pub arg_spec: Vec<Value>,
     // because values need to be 'static, we can't hold a reference to the
     // instructions that declared the macro.  Instead of that we place the
     // reference to the macro instruction (and the jump offset) in the
     // state under `state.macros`.
     pub macro_ref_id: usize,
     pub state_id: isize,
     pub closure: Value,
     pub caller_reference: bool,
 }
 
-pub(crate) struct Macro {
-    // the extra level of Arc here is necessary for recursive calls only.
-    // For more information have a look at the call() method.
-    pub data: Arc<MacroData>,
-}
-
 impl fmt::Debug for Macro {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "{self}")
+        write!(f, "<macro {}>", self.name)
     }
 }
 
-impl fmt::Display for Macro {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "<macro {}>", self.data.name)
+impl Object for Macro {
+    fn enumerate(self: &Arc<Self>) -> Enumerator {
+        Enumerator::Str(&["name", "arguments", "caller"])
     }
-}
 
-impl Object for Macro {
-    fn kind(&self) -> ObjectKind<'_> {
-        ObjectKind::Struct(self)
+    fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
+        Some(match some!(key.as_str()) {
+            "name" => self.name.clone(),
+            "arguments" => Value::from_iter(self.arg_spec.iter().cloned()),
+            "caller" => Value::from(self.caller_reference),
+            _ => return None,
+        })
     }
 
-    fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
+    fn call(self: &Arc<Self>, state: &State<'_, '_>, args: &[Value]) -> Result<Value, Error> {
         // we can only call macros that point to loaded template state.
-        if state.id != self.data.state_id {
+        if state.id != self.state_id {
             return Err(Error::new(
                 ErrorKind::InvalidOperation,
                 "cannot call this macro. template state went away.",
             ));
         }
 
         let (args, kwargs) = match args.last() {
-            Some(Value(ValueRepr::Map(kwargs, MapType::Kwargs))) => {
-                (&args[..args.len() - 1], Some(kwargs))
-            }
+            Some(last) => match Kwargs::extract(last) {
+                Some(kwargs) => (&args[..args.len() - 1], Some(kwargs)),
+                None => (args, None),
+            },
             _ => (args, None),
         };
 
-        if args.len() > self.data.arg_spec.len() {
+        if args.len() > self.arg_spec.len() {
             return Err(Error::from(ErrorKind::TooManyArguments));
         }
 
         let mut kwargs_used = BTreeSet::new();
-        let mut arg_values = Vec::with_capacity(self.data.arg_spec.len());
-        for (idx, name) in self.data.arg_spec.iter().enumerate() {
-            let kwarg = match kwargs {
-                Some(kwargs) => kwargs.get(&KeyRef::Str(name)),
+        let mut arg_values = Vec::with_capacity(self.arg_spec.len());
+        for (idx, name) in self.arg_spec.iter().enumerate() {
+            let name = match name.as_str() {
+                Some(name) => name,
+                None => {
+                    arg_values.push(Value::UNDEFINED);
+                    continue;
+                }
+            };
+            let kwarg: Option<&Value> = match kwargs {
+                Some(ref kwargs) => kwargs.get(name).ok(),
                 _ => None,
             };
             arg_values.push(match (args.get(idx), kwarg) {
                 (Some(_), Some(_)) => {
                     return Err(Error::new(
                         ErrorKind::TooManyArguments,
                         format!("duplicate argument `{name}`"),
@@ -86,46 +89,47 @@
                     kwargs_used.insert(name as &str);
                     kwarg.clone()
                 }
                 (None, None) => Value::UNDEFINED,
             });
         }
 
-        let caller = if self.data.caller_reference {
+        let caller = if self.caller_reference {
             kwargs_used.insert("caller");
             Some(
                 kwargs
-                    .and_then(|x| x.get(&KeyRef::Str("caller")).cloned())
+                    .as_ref()
+                    .and_then(|x| x.get("caller").ok())
                     .unwrap_or(Value::UNDEFINED),
             )
         } else {
             None
         };
 
         if let Some(kwargs) = kwargs {
-            for key in kwargs.keys().filter_map(|x| x.as_str()) {
+            for key in kwargs.values.keys().filter_map(|x| x.as_str()) {
                 if !kwargs_used.contains(key) {
                     return Err(Error::new(
                         ErrorKind::TooManyArguments,
                         format!("unknown keyword argument `{key}`"),
                     ));
                 }
             }
         }
 
-        let (instructions, offset) = &state.macros[self.data.macro_ref_id];
+        let (instructions, offset) = &state.macros[self.macro_ref_id];
         let vm = Vm::new(state.env());
         let mut rv = String::new();
         let mut out = Output::with_string(&mut rv);
 
         // If a macro is self referential we need to put a reference to ourselves
         // there.  Unfortunately because we only have a &self reference here, we
         // cannot bump our own refcount.  Instead we need to wrap the macro data
         // into an extra level of Arc to avoid unnecessary clones.
-        let closure = self.data.closure.clone();
+        let closure = self.closure.clone();
 
         // This requires some explanation here.  Because we get the state as &State and
         // not &mut State we are required to create a new state here.  This is unfortunate
         // but makes the calling interface more convenient for the rest of the system.
         // Because macros cannot return anything other than strings (most importantly they)
         // can't return other macros this is however not an issue, as modifications in the
         // macro cannot leak out.
@@ -141,32 +145,12 @@
 
         Ok(if !matches!(state.auto_escape(), AutoEscape::None) {
             Value::from_safe_string(rv)
         } else {
             Value::from(rv)
         })
     }
-}
-
-impl StructObject for Macro {
-    fn static_fields(&self) -> Option<&'static [&'static str]> {
-        Some(&["name", "arguments", "caller"][..])
-    }
 
-    fn get_field(&self, name: &str) -> Option<Value> {
-        match name {
-            "name" => Some(Value(ValueRepr::String(
-                self.data.name.clone(),
-                StringType::Normal,
-            ))),
-            "arguments" => Some(Value::from(
-                self.data
-                    .arg_spec
-                    .iter()
-                    .map(|x| Value(ValueRepr::String(x.clone(), StringType::Normal)))
-                    .collect::<Vec<_>>(),
-            )),
-            "caller" => Some(Value::from(self.data.caller_reference)),
-            _ => None,
-        }
+    fn render(self: &Arc<Self>, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        write!(f, "<macro {}>", self.name)
     }
 }
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/mod.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 use crate::compiler::instructions::{
     Instruction, Instructions, LOOP_FLAG_RECURSIVE, LOOP_FLAG_WITH_LOOP_VAR, MAX_LOCALS,
 };
 use crate::environment::Environment;
 use crate::error::{Error, ErrorKind};
 use crate::output::{CaptureMode, Output};
 use crate::utils::{untrusted_size_hint, AutoEscape, UndefinedBehavior};
-use crate::value::{
-    ops, value_map_with_capacity, value_optimization, KeyRef, MapType, Value, ValueRepr,
-};
-use crate::vm::context::{Context, Frame, LoopState, Stack};
+use crate::value::namespace_object::Namespace;
+use crate::value::{ops, value_map_with_capacity, value_optimization, Kwargs, Value};
+use crate::vm::context::{Frame, LoopState, Stack};
 use crate::vm::loop_object::Loop;
 use crate::vm::state::BlockStack;
 
 #[cfg(feature = "macros")]
-use crate::vm::macro_object::{Macro, MacroData};
+use crate::vm::closure_object::Closure;
 
+pub(crate) use crate::vm::context::Context;
 pub use crate::vm::state::State;
 
+#[cfg(feature = "macros")]
 mod closure_object;
 mod context;
 #[cfg(feature = "fuel")]
 mod fuel;
 mod loop_object;
 #[cfg(feature = "macros")]
 mod macro_object;
@@ -87,15 +88,15 @@
         blocks: &'template BTreeMap<&'env str, Instructions<'env>>,
         out: &mut Output,
         auto_escape: AutoEscape,
     ) -> Result<(Option<Value>, State<'template, 'env>), Error> {
         let _guard = value_optimization();
         let mut state = State::new(
             self.env,
-            Context::new(ok!(Frame::new_checked(root))),
+            Context::new_with_frame(ok!(Frame::new_checked(root)), self.env.recursion_limit()),
             auto_escape,
             instructions,
             prepare_blocks(blocks),
         );
         self.eval_state(&mut state, out).map(|x| (x, state))
     }
 
@@ -108,32 +109,34 @@
         pc: usize,
         closure: Value,
         caller: Option<Value>,
         out: &mut Output,
         state: &State,
         args: Vec<Value>,
     ) -> Result<Option<Value>, Error> {
-        let mut ctx = Context::new(Frame::new(closure));
+        let mut ctx = Context::new_with_frame(Frame::new(closure), self.env.recursion_limit());
         if let Some(caller) = caller {
             ctx.store("caller", caller);
         }
         ok!(ctx.incr_depth(state.ctx.depth() + MACRO_RECURSION_COST));
-        self.eval_impl(
+        self.do_eval(
             &mut State {
                 env: self.env,
                 ctx,
                 current_block: None,
                 auto_escape: state.auto_escape(),
                 instructions,
                 blocks: BTreeMap::default(),
                 loaded_templates: Default::default(),
                 #[cfg(feature = "macros")]
                 id: state.id,
                 #[cfg(feature = "macros")]
                 macros: state.macros.clone(),
+                #[cfg(feature = "macros")]
+                closure_tracker: state.closure_tracker.clone(),
                 #[cfg(feature = "fuel")]
                 fuel_tracker: state.fuel_tracker.clone(),
             },
             out,
             Stack::from(args),
             pc,
         )
@@ -142,17 +145,38 @@
     /// This is the actual evaluation loop that works with a specific context.
     #[inline(always)]
     fn eval_state(
         &self,
         state: &mut State<'_, 'env>,
         out: &mut Output,
     ) -> Result<Option<Value>, Error> {
-        self.eval_impl(state, out, Stack::default(), 0)
+        self.do_eval(state, out, Stack::default(), 0)
     }
 
+    /// Performs the actual evaluation, optionally with stack growth functionality.
+    fn do_eval(
+        &self,
+        state: &mut State<'_, 'env>,
+        out: &mut Output,
+        stack: Stack,
+        pc: usize,
+    ) -> Result<Option<Value>, Error> {
+        #[cfg(feature = "stacker")]
+        {
+            stacker::maybe_grow(32 * 1024, 1024 * 1024, || {
+                self.eval_impl(state, out, stack, pc)
+            })
+        }
+        #[cfg(not(feature = "stacker"))]
+        {
+            self.eval_impl(state, out, stack, pc)
+        }
+    }
+
+    #[inline]
     fn eval_impl(
         &self,
         state: &mut State<'_, 'env>,
         out: &mut Output,
         mut stack: Stack,
         mut pc: usize,
     ) -> Result<Option<Value>, Error> {
@@ -207,16 +231,15 @@
                     pc = 0;
                     continue;
                 }
             };
 
             // if we only have two arguments that we pull from the stack, we
             // can assign them to a and b.  This slightly reduces the amount of
-            // code bloat generated here.  Do the same for a potential error
-            // that needs processing.
+            // code bloat generated here.
             let a;
             let b;
             let mut err;
 
             macro_rules! func_binop {
                 ($method:ident) => {{
                     b = stack.pop();
@@ -249,29 +272,35 @@
                     }
                 };
             }
 
             macro_rules! assert_valid {
                 ($expr:expr) => {{
                     let val = $expr;
-                    if let ValueRepr::Invalid(ref err) = val.0 {
-                        bail!(Error::new(ErrorKind::BadSerialization, err.to_string()));
+                    match val.validate() {
+                        Ok(val) => val,
+                        Err(err) => bail!(err),
                     }
-                    val
                 }};
             }
 
             // if the fuel consumption feature is enabled, track the fuel
             // consumption here.
             #[cfg(feature = "fuel")]
             if let Some(ref tracker) = state.fuel_tracker {
                 ctx_ok!(tracker.track(instr));
             }
 
             match instr {
+                Instruction::Swap => {
+                    let a = stack.pop();
+                    let b = stack.pop();
+                    stack.push(a);
+                    stack.push(b);
+                }
                 Instruction::EmitRaw(val) => {
                     // this only produces a format error, no need to attach
                     // location information.
                     ok!(out.write_str(val).map_err(Error::from));
                 }
                 Instruction::Emit => {
                     ctx_ok!(self.env.format(&stack.pop(), state, out));
@@ -292,14 +321,26 @@
                     // Only when we cannot look up something, we start to consider the undefined
                     // special case.
                     stack.push(match a.get_attr_fast(name) {
                         Some(value) => assert_valid!(value),
                         None => ctx_ok!(undefined_behavior.handle_undefined(a.is_undefined())),
                     });
                 }
+                Instruction::SetAttr(name) => {
+                    b = stack.pop();
+                    a = stack.pop();
+                    if let Some(ns) = b.downcast_object_ref::<Namespace>() {
+                        ns.set_value(name, a);
+                    } else {
+                        bail!(Error::new(
+                            ErrorKind::InvalidOperation,
+                            format!("can only assign to namespaces, not {}", b.kind())
+                        ));
+                    }
+                }
                 Instruction::GetItem => {
                     a = stack.pop();
                     b = stack.pop();
                     stack.push(match b.get_item_opt(&a) {
                         Some(value) => assert_valid!(value),
                         None => ctx_ok!(undefined_behavior.handle_undefined(b.is_undefined())),
                     });
@@ -318,50 +359,38 @@
                     stack.push(value.clone());
                 }
                 Instruction::BuildMap(pair_count) => {
                     let mut map = value_map_with_capacity(*pair_count);
                     for _ in 0..*pair_count {
                         let value = stack.pop();
                         let key = stack.pop();
-                        map.insert(KeyRef::Value(key), value);
+                        map.insert(key, value);
                     }
-                    stack.push(Value(ValueRepr::Map(map.into(), MapType::Normal)))
+                    stack.push(Value::from_object(map))
                 }
                 Instruction::BuildKwargs(pair_count) => {
                     let mut map = value_map_with_capacity(*pair_count);
                     for _ in 0..*pair_count {
                         let value = stack.pop();
                         let key = stack.pop();
-                        map.insert(KeyRef::Value(key), value);
+                        map.insert(key, value);
                     }
-                    stack.push(Value(ValueRepr::Map(map.into(), MapType::Kwargs)))
+                    stack.push(Kwargs::wrap(map))
                 }
-                Instruction::BuildList(count) => {
-                    let mut v = Vec::with_capacity(untrusted_size_hint(*count));
-                    for _ in 0..*count {
+                Instruction::BuildList(n) => {
+                    let count = n.unwrap_or_else(|| stack.pop().try_into().unwrap());
+                    let mut v = Vec::with_capacity(untrusted_size_hint(count));
+                    for _ in 0..count {
                         v.push(stack.pop());
                     }
                     v.reverse();
-                    stack.push(Value(ValueRepr::Seq(Arc::new(v))));
+                    stack.push(Value::from_object(v))
                 }
                 Instruction::UnpackList(count) => {
-                    ctx_ok!(self.unpack_list(&mut stack, count));
-                }
-                Instruction::ListAppend => {
-                    a = stack.pop();
-                    // this intentionally only works with actual sequences
-                    if let ValueRepr::Seq(mut v) = stack.pop().0 {
-                        Arc::make_mut(&mut v).push(a);
-                        stack.push(Value(ValueRepr::Seq(v)))
-                    } else {
-                        bail!(Error::new(
-                            ErrorKind::InvalidOperation,
-                            "cannot append to non-list"
-                        ));
-                    }
+                    ctx_ok!(self.unpack_list(&mut stack, *count));
                 }
                 Instruction::Add => func_binop!(add),
                 Instruction::Sub => func_binop!(sub),
                 Instruction::Mul => func_binop!(mul),
                 Instruction::Div => func_binop!(div),
                 Instruction::IntDiv => func_binop!(int_div),
                 Instruction::Rem => func_binop!(rem),
@@ -449,29 +478,29 @@
                 }
                 Instruction::Jump(jump_target) => {
                     pc = *jump_target;
                     continue;
                 }
                 Instruction::JumpIfFalse(jump_target) => {
                     a = stack.pop();
-                    if !a.is_true() {
+                    if !ok!(undefined_behavior.is_true(&a)) {
                         pc = *jump_target;
                         continue;
                     }
                 }
                 Instruction::JumpIfFalseOrPop(jump_target) => {
-                    if !stack.peek().is_true() {
+                    if !ok!(undefined_behavior.is_true(stack.peek())) {
                         pc = *jump_target;
                         continue;
                     } else {
                         stack.pop();
                     }
                 }
                 Instruction::JumpIfTrueOrPop(jump_target) => {
-                    if stack.peek().is_true() {
+                    if ok!(undefined_behavior.is_true(stack.peek())) {
                         pc = *jump_target;
                         continue;
                     } else {
                         stack.pop();
                     }
                 }
                 #[cfg(feature = "multi_template")]
@@ -619,31 +648,44 @@
                     ctx_ok!(self.perform_include(a, state, out, *ignore_missing));
                 }
                 #[cfg(feature = "multi_template")]
                 Instruction::ExportLocals => {
                     let locals = state.ctx.current_locals_mut();
                     let mut module = value_map_with_capacity(locals.len());
                     for (key, value) in locals.iter() {
-                        module.insert(KeyRef::Value(Value::from(*key)), value.clone());
+                        module.insert(Value::from(*key), value.clone());
                     }
-                    stack.push(Value(ValueRepr::Map(module.into(), MapType::Normal)));
+                    stack.push(Value::from_object(module));
                 }
                 #[cfg(feature = "macros")]
                 Instruction::BuildMacro(name, offset, flags) => {
                     self.build_macro(&mut stack, state, *offset, name, *flags);
                 }
                 #[cfg(feature = "macros")]
                 Instruction::Return => break,
                 #[cfg(feature = "macros")]
                 Instruction::Enclose(name) => {
+                    // the first time we enclose a value, we need to create a closure
+                    // and store it on the context, and add it to the closure tracker
+                    // for cycle breaking.
+                    if state.ctx.closure().is_none() {
+                        let closure = Arc::new(Closure::default());
+                        state.closure_tracker.track_closure(closure.clone());
+                        state.ctx.reset_closure(Some(closure));
+                    }
                     state.ctx.enclose(state.env, name);
                 }
                 #[cfg(feature = "macros")]
                 Instruction::GetClosure => {
-                    stack.push(Value::from(state.ctx.closure()));
+                    stack.push(
+                        state
+                            .ctx
+                            .closure()
+                            .map_or(Value::UNDEFINED, |x| Value::from_dyn_object(x.clone())),
+                    );
                 }
             }
             pc += 1;
         }
 
         Ok(stack.try_pop())
     }
@@ -652,23 +694,24 @@
     fn perform_include(
         &self,
         name: Value,
         state: &mut State<'_, 'env>,
         out: &mut Output,
         ignore_missing: bool,
     ) -> Result<(), Error> {
-        use crate::value::SeqObject;
-
-        let single_name_slice = std::slice::from_ref(&name);
-        let choices = name
-            .as_seq()
-            .unwrap_or(&single_name_slice as &dyn SeqObject);
+        let obj = name.as_object();
+        let choices = obj
+            .as_ref()
+            .and_then(|d| d.try_iter())
+            .into_iter()
+            .flatten()
+            .chain(obj.is_none().then(|| name.clone()));
 
         let mut templates_tried = vec![];
-        for choice in choices.iter() {
+        for choice in choices {
             let name = ok!(choice.as_str().ok_or_else(|| {
                 Error::new(
                     ErrorKind::InvalidOperation,
                     "template name was not a string",
                 )
             }));
             let tmpl = match state.get_template(name) {
@@ -683,18 +726,26 @@
                 }
             };
 
             let (new_instructions, new_blocks) = ok!(tmpl.instructions_and_blocks());
             let old_escape = mem::replace(&mut state.auto_escape, tmpl.initial_auto_escape());
             let old_instructions = mem::replace(&mut state.instructions, new_instructions);
             let old_blocks = mem::replace(&mut state.blocks, prepare_blocks(new_blocks));
-            let old_closure = state.ctx.take_closure();
             ok!(state.ctx.incr_depth(INCLUDE_RECURSION_COST));
-            let rv = self.eval_state(state, out);
-            state.ctx.reset_closure(old_closure);
+            let rv;
+            #[cfg(feature = "macros")]
+            {
+                let old_closure = state.ctx.take_closure();
+                rv = self.eval_state(state, out);
+                state.ctx.reset_closure(old_closure);
+            }
+            #[cfg(not(feature = "macros"))]
+            {
+                rv = self.eval_state(state, out);
+            }
             state.ctx.decr_depth(INCLUDE_RECURSION_COST);
             state.auto_escape = old_escape;
             state.instructions = old_instructions;
             state.blocks = old_blocks;
             ok!(rv.map_err(|err| {
                 Error::new(
                     ErrorKind::BadInclude,
@@ -805,15 +856,15 @@
         let tmpl = ok!(state.get_template(name));
         let (new_instructions, new_blocks) = ok!(tmpl.instructions_and_blocks());
         state.loaded_templates.insert(new_instructions.name());
         for (name, instr) in new_blocks.iter() {
             state
                 .blocks
                 .entry(name)
-                .or_insert_with(BlockStack::default)
+                .or_default()
                 .append_instructions(instr);
         }
         Ok(new_instructions)
     }
 
     #[cfg(feature = "multi_template")]
     pub(crate) fn call_block(
@@ -868,15 +919,22 @@
         iterable: Value,
         flags: u8,
         pc: usize,
         current_recursion_jump: Option<(usize, bool)>,
     ) -> Result<(), Error> {
         #[allow(unused_mut)]
         let mut iterator = ok!(state.undefined_behavior().try_iter(iterable));
-        let len = iterator.len();
+        // for an iterator where the lower and upper bound are matching we can
+        // consider them to have ExactSizeIterator semantics.  We do however not
+        // expect ExactSizeIterator bounds themselves to support iteration by
+        // other means.
+        let len = match iterator.size_hint() {
+            (lower, Some(upper)) if lower == upper => Some(lower),
+            _ => None,
+        };
         let depth = state
             .ctx
             .current_loop()
             .filter(|x| x.recurse_jump_target.is_some())
             .map_or(0, |x| x.object.depth + 1);
         let recursive = flags & LOOP_FLAG_RECURSIVE != 0;
         let with_loop_var = flags & LOOP_FLAG_WITH_LOOP_VAR != 0;
@@ -896,68 +954,60 @@
                 iterator,
             }),
             ..Frame::default()
         }));
         Ok(())
     }
 
-    fn unpack_list(&self, stack: &mut Stack, count: &usize) -> Result<(), Error> {
+    fn unpack_list(&self, stack: &mut Stack, count: usize) -> Result<(), Error> {
         let top = stack.pop();
-        let seq = ok!(top
-            .as_seq()
-            .ok_or_else(|| Error::new(ErrorKind::CannotUnpack, "not a sequence")));
-        if seq.item_count() != *count {
-            return Err(Error::new(
-                ErrorKind::CannotUnpack,
-                format!(
-                    "sequence of wrong length (expected {}, got {})",
-                    *count,
-                    seq.item_count()
-                ),
-            ));
-        }
-        for item in seq.iter().rev() {
+        let iter = ok!(top
+            .as_object()
+            .and_then(|x| x.try_iter())
+            .ok_or_else(|| Error::new(ErrorKind::CannotUnpack, "value is not iterable")));
+
+        let mut n = 0;
+        for item in iter {
             stack.push(item);
+            n += 1;
+        }
+
+        if n == count {
+            stack.reverse_top(n);
+            Ok(())
+        } else {
+            Err(Error::new(
+                ErrorKind::CannotUnpack,
+                format!("sequence of wrong length (expected {}, got {})", count, n,),
+            ))
         }
-        Ok(())
     }
 
     #[cfg(feature = "macros")]
     fn build_macro(
         &self,
         stack: &mut Stack,
         state: &mut State,
         offset: usize,
         name: &str,
         flags: u8,
     ) {
-        use crate::compiler::instructions::MACRO_CALLER;
+        use crate::{compiler::instructions::MACRO_CALLER, vm::macro_object::Macro};
 
-        let arg_spec = match stack.pop().0 {
-            ValueRepr::Seq(args) => args
-                .iter()
-                .map(|value| match &value.0 {
-                    ValueRepr::String(arg, _) => arg.clone(),
-                    _ => unreachable!(),
-                })
-                .collect(),
-            _ => unreachable!(),
-        };
+        let arg_spec = stack.pop().try_iter().unwrap().collect();
         let closure = stack.pop();
         let macro_ref_id = state.macros.len();
         Arc::make_mut(&mut state.macros).push((state.instructions, offset));
         stack.push(Value::from_object(Macro {
-            data: Arc::new(MacroData {
-                name: Arc::from(name.to_string()),
-                arg_spec,
-                macro_ref_id,
-                state_id: state.id,
-                closure,
-                caller_reference: (flags & MACRO_CALLER) != 0,
-            }),
+            name: Value::from(name),
+            arg_spec,
+            macro_ref_id,
+            state_id: state.id,
+            closure,
+            caller_reference: (flags & MACRO_CALLER) != 0,
         }));
     }
 }
 
 #[inline(never)]
 #[cold]
 fn process_err(err: &mut Error, pc: usize, state: &State) {
```

### Comparing `minijinja-1.0.8/local_dependencies/minijinja/src/vm/state.rs` & `minijinja-2.0.1/local_dependencies/minijinja/src/vm/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     pub(crate) blocks: BTreeMap<&'env str, BlockStack<'template, 'env>>,
     #[allow(unused)]
     pub(crate) loaded_templates: BTreeSet<&'env str>,
     #[cfg(feature = "macros")]
     pub(crate) id: isize,
     #[cfg(feature = "macros")]
     pub(crate) macros: std::sync::Arc<Vec<(&'template Instructions<'env>, usize)>>,
+    #[cfg(feature = "macros")]
+    pub(crate) closure_tracker: std::sync::Arc<crate::vm::closure_object::ClosureTracker>,
     #[cfg(feature = "fuel")]
     pub(crate) fuel_tracker: Option<std::sync::Arc<FuelTracker>>,
 }
 
 impl<'template, 'env> fmt::Debug for State<'template, 'env> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let mut ds = f.debug_struct("State");
@@ -84,24 +86,26 @@
             current_block: None,
             auto_escape,
             instructions,
             blocks,
             loaded_templates: BTreeSet::new(),
             #[cfg(feature = "macros")]
             macros: Default::default(),
+            #[cfg(feature = "macros")]
+            closure_tracker: Default::default(),
             #[cfg(feature = "fuel")]
             fuel_tracker: env.fuel().map(FuelTracker::new),
         }
     }
 
     /// Creates an empty state for an environment.
     pub(crate) fn new_for_env(env: &'env Environment) -> State<'env, 'env> {
         State::new(
             env,
-            Context::default(),
+            Context::new(env.recursion_limit()),
             AutoEscape::None,
             &crate::compiler::instructions::EMPTY_INSTRUCTIONS,
             BTreeMap::new(),
         )
     }
 
     /// Returns a reference to the current environment.
@@ -222,14 +226,15 @@
     }
 
     /// Invokes a filter with some arguments.
     ///
     /// ```
     /// # use minijinja::Environment;
     /// # let mut env = Environment::new();
+    /// # env.add_filter("upper", |x: &str| x.to_uppercase());
     /// # let tmpl = env.template_from_str("").unwrap();
     /// # let state = tmpl.new_state();
     /// let rv = state.apply_filter("upper", &["hello world".into()]).unwrap();
     /// assert_eq!(rv.as_str(), Some("HELLO WORLD"));
     /// ```
     pub fn apply_filter(&self, filter: &str, args: &[Value]) -> Result<Value, Error> {
         match self.env.get_filter(filter) {
@@ -239,14 +244,15 @@
     }
 
     /// Invokes a test function on a value.
     ///
     /// ```
     /// # use minijinja::Environment;
     /// # let mut env = Environment::new();
+    /// # env.add_test("even", |x: i32| x % 2 == 0);
     /// # let tmpl = env.template_from_str("").unwrap();
     /// # let state = tmpl.new_state();
     /// let rv = state.perform_test("even", &[42i32.into()]).unwrap();
     /// assert!(rv);
     /// ```
     pub fn perform_test(&self, test: &str, args: &[Value]) -> Result<bool, Error> {
         match self.env.get_test(test) {
```

### Comparing `minijinja-1.0.8/Cargo.toml` & `minijinja-2.0.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "minijinja-py"
-version = "1.0.8"
+version = "2.0.1"
 edition = "2021"
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "minijinja_py"
 crate-type = ["cdylib"]
 
 [dependencies]
-minijinja = { version = "1.0.8", path = "local_dependencies/minijinja", features = ["loader", "json", "urlencode", "fuel", "preserve_order", "speedups", "custom_syntax"] }
+minijinja = { version = "2.0.1", path = "local_dependencies/minijinja", features = ["loader", "json", "urlencode", "fuel", "preserve_order", "speedups", "custom_syntax"] }
 once_cell = "1.17.0"
-pyo3 = { version = "0.18.0", features = ["extension-module", "serde", "abi3-py38"] }
+pyo3 = { version = "0.21.1", features = ["extension-module", "serde", "abi3-py38"] }
```

### Comparing `minijinja-1.0.8/LICENSE` & `minijinja-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/README.md` & `minijinja-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 ```python
 result = env.render_template('template_name', var1="value 1", var2="value 2")
 print(result)
 ```
 
 ## Purpose
 
-MiniJinja attempts a certain level of compatibility with Jinja2, but it does not
-try to achieve this at all costs.  As a result you will notice that quite a few
-templates will refuse to render with MiniJinja despite the fact that they probably
-look quite innocent.  It is however possible to write templates that render to the
-same results for both Jinja2 and MiniJinja.  This raises the question why you might
-want to use MiniJinja.
+MiniJinja attempts a reasonably high level of compatibility with Jinja2, but it
+does not try to achieve this at all costs.  As a result you will notice that
+quite a few templates will refuse to render with MiniJinja despite the fact that
+they probably look quite innocent.  It is however possible to write templates
+that render to the same results for both Jinja2 and MiniJinja.  This raises the
+question why you might want to use MiniJinja.
 
 The main benefit would be to achieve the exact same results in both Rust and Python.
 Additionally MiniJinja has a stronger sandbox than Jinja2 and might perform ever so
 slightly better in some situations.  However you should be aware that due to the
 marshalling that needs to happen in either direction there is a certain amount of
 loss of information.
 
@@ -142,37 +142,41 @@
     return state.lookup("a_variable") + value
 
 env.add_filter("add_a_variable", my_filter)
 ```
 
 ## Runtime Behavior
 
-MiniJinja uses it's own runtime model which is not matching the Python
-runtime model.  As a result there are clear gaps in beahvior between the
-two and only limited effort is made to bridge them.  For instance you will
-be able to call some methods of types, but for instance builtins such as
-dicts and lists do not expose their methods on the MiniJinja side.  This
-means that it's very intentional that if you pass a dictionary to MiniJinja,
-the Python `.items()` method is unavailable.
+MiniJinja uses it's own runtime model which is not matching the Python runtime
+model.  As a result there are gaps in behavior between the two but some
+limited effort is made to bridge them.  For instance you will be able to call
+some methods of types, but for instance builtins such as dicts and lists do not
+expose their methods on the MiniJinja side in all cases.  A natively generated
+MiniJinja map (such as with the `dict` global function) will not have an `.items()`
+method, whereas a Python dict passed to MiniJinja will.
 
 Here is what this means for some basic types:
 
 * Python dictionaries and lists (as well as other objects that behave as sequences)
-  appear in the MiniJinja side as native lists.  They do not expose any specific
-  other behavior and when they move back to the Python side they will appear as basic
-  lists.  Specifically this means that a tuple (which does not exist in MiniJinja)
-  when moving from Python to MiniJinja turns into a list and will remain a list when
-  it moves back.
+  appear in the MiniJinja side very similar to how they do in Python.
+* Tuples on the MiniJinja side are represented as lists, but will appear again as
+  tuples if passed back to Python.
 * Python objects are represented in MiniJinja similarly to dicts, but they retain all
   their meaningful Python APIs.  This means they stringify via `__str__` and they
   allow the MiniJinja code to call their non-underscored methods.  Note that there is
   no extra security layer in use at the moment so take care of what you pass there.
 * MiniJinja's python binding understand what `__html__` is when it exists on a string
   subclass.  This means that a `markupsafe.Markup` object will appear as safe string in
   MiniJinja.  This information can also flow back to Python again.
+* Stringification of objects uses `__str__` which is why mixed Python and MiniJinja
+  objects can be a bit confusing at times.
+* Where in Jinja2 there is a difference between `foo["bar"]` and `foo.bar` which can
+  be used to disambiugate properties and keys, in MiniJinja there is no such difference.
+  However methods are disambiugated so `foo.items()` works and will correctly call
+  the method in all cases.
 
 ## Sponsor
 
 If you like the project and find it useful you can [become a
 sponsor](https://github.com/sponsors/mitsuhiko).
 
 ## License and Links
```

### Comparing `minijinja-1.0.8/hello.py` & `minijinja-2.0.1/hello.py`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/pyproject.toml` & `minijinja-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.15,<0.16"]
 build-backend = "maturin"
 
 [project]
 name = "minijinja"
-version = "1.0.8"
+version = "2.0.1"
 description = "An experimental Python binding of the Rust MiniJinja template engine."
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Armin Ronacher", email = "armin.ronacher@active-4.com" }
 ]
 maintainers = [
```

### Comparing `minijinja-1.0.8/python/minijinja/__init__.py` & `minijinja-2.0.1/python/minijinja/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,26 @@
         globals=None,
         debug=True,
         fuel=None,
         undefined_behavior=None,
         auto_escape_callback=None,
         path_join_callback=None,
         keep_trailing_newline=False,
+        trim_blocks=False,
+        lstrip_blocks=False,
         finalizer=None,
         reload_before_render=False,
         block_start_string="{%",
         block_end_string="%}",
         variable_start_string="{{",
         variable_end_string="}}",
         comment_start_string="{#",
         comment_end_string="#}",
+        line_statement_prefix=None,
+        line_comment_prefix=None,
     ):
         super().__init__()
         if loader is not None:
             if templates:
                 raise TypeError("Cannot set loader and templates at the same time")
             self.loader = loader
         elif templates is not None:
@@ -61,28 +65,34 @@
         self.debug = debug
         if auto_escape_callback is not None:
             self.auto_escape_callback = auto_escape_callback
         if path_join_callback is not None:
             self.path_join_callback = path_join_callback
         if keep_trailing_newline:
             self.keep_trailing_newline = True
+        if trim_blocks:
+            self.trim_blocks = True
+        if lstrip_blocks:
+            self.lstrip_blocks = True
         if finalizer is not None:
             self.finalizer = finalizer
         if undefined_behavior is not None:
             self.undefined_behavior = undefined_behavior
         self.reload_before_render = reload_before_render
 
         # XXX: because this is not an atomic reconfigure if you set one of
         # the values to a conflicting set, it will immediately error out :(
         self.block_start_string = block_start_string
         self.block_end_string = block_end_string
         self.variable_start_string = variable_start_string
         self.variable_end_string = variable_end_string
         self.comment_start_string = comment_start_string
         self.comment_end_string = comment_end_string
+        self.line_statement_prefix = line_statement_prefix
+        self.line_comment_prefix = line_comment_prefix
 
 
 DEFAULT_ENVIRONMENT = Environment()
 
 
 def render_str(*args, **context):
     """Shortcut to render a string with the default environment."""
```

### Comparing `minijinja-1.0.8/python/minijinja/_internal.py` & `minijinja-2.0.1/python/minijinja/_internal.py`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/src/environment.rs` & `minijinja-2.0.1/src/environment.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,65 @@
 use std::borrow::Cow;
 use std::ffi::c_void;
 use std::sync::atomic::{AtomicBool, AtomicPtr, Ordering};
 use std::sync::Mutex;
 
+use minijinja::syntax::SyntaxConfig;
 use minijinja::value::{Rest, Value};
-use minijinja::{context, escape_formatter, AutoEscape, Error, State, Syntax, UndefinedBehavior};
-use pyo3::conversion::AsPyPointer;
+use minijinja::{context, escape_formatter, AutoEscape, Error, State, UndefinedBehavior};
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
+use pyo3::pybacked::PyBackedStr;
 use pyo3::types::{PyDict, PyTuple};
 
 use crate::error_support::{report_unraisable, to_minijinja_error, to_py_error};
 use crate::state::bind_state;
 use crate::typeconv::{
-    get_custom_autoescape, to_minijinja_value, to_python_args, to_python_value, DictLikeObject,
+    get_custom_autoescape, to_minijinja_value, to_python_args, to_python_value, DynamicObject,
 };
 
 thread_local! {
-    static CURRENT_ENV: AtomicPtr<c_void> = AtomicPtr::new(std::ptr::null_mut());
+    static CURRENT_ENV: AtomicPtr<c_void> = const { AtomicPtr::new(std::ptr::null_mut()) };
+}
+
+struct Syntax {
+    block_start: String,
+    block_end: String,
+    variable_start: String,
+    variable_end: String,
+    comment_start: String,
+    comment_end: String,
+    line_statement_prefix: String,
+    line_comment_prefix: String,
+}
+
+impl Default for Syntax {
+    fn default() -> Self {
+        Self {
+            block_start: "{%".into(),
+            block_end: "%}".into(),
+            variable_start: "{{".into(),
+            variable_end: "}}".into(),
+            comment_start: "{#".into(),
+            comment_end: "#}".into(),
+            line_statement_prefix: "".into(),
+            line_comment_prefix: "".into(),
+        }
+    }
+}
+impl Syntax {
+    fn compile(&self) -> Result<SyntaxConfig, Error> {
+        SyntaxConfig::builder()
+            .block_delimiters(self.block_start.clone(), self.block_end.clone())
+            .variable_delimiters(self.variable_start.clone(), self.variable_end.clone())
+            .comment_delimiters(self.comment_start.clone(), self.comment_end.clone())
+            .line_statement_prefix(self.line_statement_prefix.clone())
+            .line_comment_prefix(self.line_comment_prefix.clone())
+            .build()
+    }
 }
 
 macro_rules! syntax_setter {
     ($slf:expr, $value:expr, $field:ident, $default:expr) => {{
         let value = $value;
         let mut inner = $slf.inner.lock().unwrap();
         if inner.syntax.is_none() {
@@ -29,16 +67,16 @@
                 return Ok(());
             }
             inner.syntax = Some(Syntax::default());
         }
         if let Some(ref mut syntax) = inner.syntax {
             if syntax.$field != value {
                 syntax.$field = value.into();
-                let new_syntax = syntax.clone();
-                inner.env.set_syntax(new_syntax).map_err(to_py_error)?;
+                let syntax_config = syntax.compile().map_err(to_py_error)?;
+                inner.env.set_syntax(syntax_config);
             }
         }
         Ok(())
     }};
 }
 
 macro_rules! syntax_getter {
@@ -147,30 +185,30 @@
     pub fn get_fuel(&self) -> PyResult<Option<u64>> {
         let inner = self.inner.lock().unwrap();
         Ok(inner.env.fuel())
     }
 
     /// Registers a filter function.
     #[pyo3(text_signature = "(self, name, callback)")]
-    pub fn add_filter(&self, name: &str, callback: &PyAny) -> PyResult<()> {
+    pub fn add_filter(&self, name: &str, callback: &Bound<'_, PyAny>) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
-        let callback: Py<PyAny> = callback.into();
+        let callback: Py<PyAny> = callback.clone().unbind();
         self.inner.lock().unwrap().env.add_filter(
             name.to_string(),
             move |state: &State, args: Rest<Value>| -> Result<Value, Error> {
                 Python::with_gil(|py| {
                     bind_state(state, || {
-                        let (py_args, py_kwargs) = to_python_args(py, callback.as_ref(py), &args)
+                        let (py_args, py_kwargs) = to_python_args(py, callback.bind(py), &args)
                             .map_err(to_minijinja_error)?;
                         let rv = callback
-                            .call(py, py_args, py_kwargs)
+                            .call_bound(py, py_args, py_kwargs.as_ref())
                             .map_err(to_minijinja_error)?;
-                        Ok(to_minijinja_value(rv.as_ref(py)))
+                        Ok(to_minijinja_value(rv.bind(py)))
                     })
                 })
             },
         );
         Ok(())
     }
 
@@ -179,67 +217,67 @@
     pub fn remove_filter(&self, name: &str) -> PyResult<()> {
         self.inner.lock().unwrap().env.remove_filter(name);
         Ok(())
     }
 
     /// Registers a test function.
     #[pyo3(text_signature = "(self, name, callback)")]
-    pub fn add_test(&self, name: &str, callback: &PyAny) -> PyResult<()> {
+    pub fn add_test(&self, name: &str, callback: &Bound<'_, PyAny>) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
-        let callback: Py<PyAny> = callback.into();
+        let callback: Py<PyAny> = callback.clone().unbind();
         self.inner.lock().unwrap().env.add_test(
             name.to_string(),
             move |state: &State, args: Rest<Value>| -> Result<bool, Error> {
                 Python::with_gil(|py| {
                     bind_state(state, || {
-                        let (py_args, py_kwargs) = to_python_args(py, callback.as_ref(py), &args)
+                        let (py_args, py_kwargs) = to_python_args(py, callback.bind(py), &args)
                             .map_err(to_minijinja_error)?;
                         let rv = callback
-                            .call(py, py_args, py_kwargs)
+                            .call_bound(py, py_args, py_kwargs.as_ref())
                             .map_err(to_minijinja_error)?;
-                        Ok(to_minijinja_value(rv.as_ref(py)).is_true())
+                        Ok(to_minijinja_value(rv.bind(py)).is_true())
                     })
                 })
             },
         );
         Ok(())
     }
 
     /// Removes a test function.
     #[pyo3(text_signature = "(self, name)")]
     pub fn remove_test(&self, name: &str) -> PyResult<()> {
         self.inner.lock().unwrap().env.remove_test(name);
         Ok(())
     }
 
-    fn add_function(&self, name: &str, callback: &PyAny) -> PyResult<()> {
-        let callback: Py<PyAny> = callback.into();
+    fn add_function(&self, name: &str, callback: &Bound<'_, PyAny>) -> PyResult<()> {
+        let callback: Py<PyAny> = callback.clone().unbind();
         self.inner.lock().unwrap().env.add_function(
             name.to_string(),
             move |state: &State, args: Rest<Value>| -> Result<Value, Error> {
                 Python::with_gil(|py| {
                     bind_state(state, || {
-                        let (py_args, py_kwargs) = to_python_args(py, callback.as_ref(py), &args)
+                        let (py_args, py_kwargs) = to_python_args(py, callback.bind(py), &args)
                             .map_err(to_minijinja_error)?;
                         let rv = callback
-                            .call(py, py_args, py_kwargs)
+                            .call_bound(py, py_args, py_kwargs.as_ref())
                             .map_err(to_minijinja_error)?;
-                        Ok(to_minijinja_value(rv.as_ref(py)))
+                        Ok(to_minijinja_value(rv.bind(py)))
                     })
                 })
             },
         );
         Ok(())
     }
 
     /// Registers a global
     #[pyo3(text_signature = "(self, name, value)")]
-    pub fn add_global(&self, name: &str, value: &PyAny) -> PyResult<()> {
+    pub fn add_global(&self, name: &str, value: &Bound<'_, PyAny>) -> PyResult<()> {
         if value.is_callable() {
             self.add_function(name, value)
         } else {
             self.inner
                 .lock()
                 .unwrap()
                 .env
@@ -256,39 +294,39 @@
     }
 
     /// Sets an auto escape callback.
     ///
     /// Note that because this interface in MiniJinja is infallible, the callback is
     /// not able to raise an error.
     #[setter]
-    pub fn set_auto_escape_callback(&self, callback: &PyAny) -> PyResult<()> {
+    pub fn set_auto_escape_callback(&self, callback: &Bound<'_, PyAny>) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
-        let callback: Py<PyAny> = callback.into();
+        let callback: Py<PyAny> = callback.clone().unbind();
         let mut inner = self.inner.lock().unwrap();
         inner.auto_escape_callback = Some(callback.clone());
         inner
             .env
             .set_auto_escape_callback(move |name: &str| -> AutoEscape {
                 Python::with_gil(|py| {
-                    let py_args = PyTuple::new(py, [name]);
-                    let rv = match callback.call(py, py_args, None) {
+                    let py_args = PyTuple::new_bound(py, [name]);
+                    let rv = match callback.call_bound(py, py_args, None) {
                         Ok(value) => value,
                         Err(err) => {
                             report_unraisable(py, err);
                             return AutoEscape::None;
                         }
                     };
-                    let rv = rv.as_ref(py);
+                    let rv = rv.bind(py);
                     if rv.is_none() {
                         return AutoEscape::None;
                     }
-                    if let Ok(value) = rv.extract::<&str>() {
-                        match value {
+                    if let Ok(value) = rv.extract::<PyBackedStr>() {
+                        match &value as &str {
                             "html" => AutoEscape::Html,
                             "json" => AutoEscape::Json,
                             other => get_custom_autoescape(other),
                         }
                     } else if let Ok(value) = rv.extract::<bool>() {
                         match value {
                             true => AutoEscape::Html,
@@ -307,34 +345,34 @@
         Ok(self.inner.lock().unwrap().auto_escape_callback.clone())
     }
 
     /// Sets a finalizer.
     ///
     /// A finalizer is called before a value is rendered to customize it.
     #[setter]
-    pub fn set_finalizer(&self, callback: &PyAny) -> PyResult<()> {
+    pub fn set_finalizer(&self, callback: &Bound<'_, PyAny>) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
-        let callback: Py<PyAny> = callback.into();
+        let callback: Py<PyAny> = callback.clone().unbind();
         let mut inner = self.inner.lock().unwrap();
         inner.finalizer_callback = Some(callback.clone());
         inner.env.set_formatter(move |output, state, value| {
             Python::with_gil(|py| -> Result<(), Error> {
                 let maybe_new_value = bind_state(state, || -> Result<_, Error> {
                     let args = std::slice::from_ref(value);
-                    let (py_args, py_kwargs) = to_python_args(py, callback.as_ref(py), args)
-                        .map_err(to_minijinja_error)?;
+                    let (py_args, py_kwargs) =
+                        to_python_args(py, callback.bind(py), args).map_err(to_minijinja_error)?;
                     let rv = callback
-                        .call(py, py_args, py_kwargs)
+                        .call_bound(py, py_args, py_kwargs.as_ref())
                         .map_err(to_minijinja_error)?;
                     if rv.is(&py.NotImplemented()) {
                         Ok(None)
                     } else {
-                        Ok(Some(to_minijinja_value(rv.as_ref(py))))
+                        Ok(Some(to_minijinja_value(rv.bind(py))))
                     }
                 })?;
                 let value = match maybe_new_value {
                     Some(ref new_value) => new_value,
                     None => value,
                 };
                 escape_formatter(output, state, value)
@@ -350,33 +388,33 @@
 
     /// Sets a loader function for the environment.
     ///
     /// The loader function is invoked with the name of the template to load.  If the
     /// template exists the source code of the template should be returned a string,
     /// otherwise `None` can be used to indicate that the template does not exist.
     #[setter]
-    pub fn set_loader(&self, callback: Option<&PyAny>) -> PyResult<()> {
+    pub fn set_loader(&self, callback: Option<&Bound<'_, PyAny>>) -> PyResult<()> {
         let callback = match callback {
             None => None,
             Some(callback) => {
                 if !callback.is_callable() {
                     return Err(PyRuntimeError::new_err("expected callback"));
                 }
-                Some(callback.into())
+                Some(callback.clone().unbind())
             }
         };
         let mut inner = self.inner.lock().unwrap();
         inner.loader = callback.clone();
 
         if let Some(callback) = callback {
             inner.env.set_loader(move |name| {
                 Python::with_gil(|py| {
-                    let callback = callback.as_ref(py);
+                    let callback = callback.bind(py);
                     let rv = callback
-                        .call1(PyTuple::new(py, [name]))
+                        .call1(PyTuple::new_bound(py, [name]))
                         .map_err(to_minijinja_error)?;
                     if rv.is_none() {
                         Ok(None)
                     } else {
                         Ok(Some(rv.to_string()))
                     }
                 })
@@ -390,25 +428,25 @@
     #[getter]
     pub fn get_loader(&self) -> Option<Py<PyAny>> {
         self.inner.lock().unwrap().loader.clone()
     }
 
     /// Sets a new path join callback.
     #[setter]
-    pub fn set_path_join_callback(&self, callback: &PyAny) -> PyResult<()> {
+    pub fn set_path_join_callback(&self, callback: &Bound<'_, PyAny>) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
-        let callback: Py<PyAny> = callback.into();
+        let callback: Py<PyAny> = callback.clone().unbind();
         let mut inner = self.inner.lock().unwrap();
         inner.path_join_callback = Some(callback.clone());
         inner.env.set_path_join_callback(move |name, parent| {
             Python::with_gil(|py| {
-                let callback = callback.as_ref(py);
-                match callback.call1(PyTuple::new(py, [name, parent])) {
+                let callback = callback.bind(py);
+                match callback.call1(PyTuple::new_bound(py, [name, parent])) {
                     Ok(rv) => Cow::Owned(rv.to_string()),
                     Err(err) => {
                         report_unraisable(py, err);
                         Cow::Borrowed(name)
                     }
                 }
             })
@@ -500,14 +538,36 @@
     }
 
     #[getter]
     pub fn get_comment_end_string(&self) -> String {
         syntax_getter!(self, comment_end, "#}")
     }
 
+    #[setter]
+    pub fn set_line_statement_prefix(&self, value: Option<String>) -> PyResult<()> {
+        syntax_setter!(self, value.unwrap_or_default(), line_statement_prefix, "")
+    }
+
+    #[getter]
+    pub fn get_line_statement_prefix(&self) -> Option<String> {
+        let rv: String = syntax_getter!(self, line_statement_prefix, "");
+        (!rv.is_empty()).then_some(rv)
+    }
+
+    #[setter]
+    pub fn set_line_comment_prefix(&self, value: Option<String>) -> PyResult<()> {
+        syntax_setter!(self, value.unwrap_or_default(), line_comment_prefix, "")
+    }
+
+    #[getter]
+    pub fn get_line_comment_prefix(&self) -> Option<String> {
+        let rv: String = syntax_getter!(self, line_comment_prefix, "");
+        (!rv.is_empty()).then_some(rv)
+    }
+
     /// Configures the trailing newline trimming feature.
     #[setter]
     pub fn set_keep_trailing_newline(&self, yes: bool) -> PyResult<()> {
         self.inner
             .lock()
             .unwrap()
             .env
@@ -517,14 +577,40 @@
 
     /// Returns the current value of the trailing newline trimming flag.
     #[getter]
     pub fn get_keep_trailing_newline(&self) -> PyResult<bool> {
         Ok(self.inner.lock().unwrap().env.keep_trailing_newline())
     }
 
+    /// Configures the trim blocks feature.
+    #[setter]
+    pub fn set_trim_blocks(&self, yes: bool) -> PyResult<()> {
+        self.inner.lock().unwrap().env.set_trim_blocks(yes);
+        Ok(())
+    }
+
+    /// Returns the current value of the trim blocks flag.
+    #[getter]
+    pub fn get_trim_blocks(&self) -> PyResult<bool> {
+        Ok(self.inner.lock().unwrap().env.trim_blocks())
+    }
+
+    /// Configures the lstrip blocks feature.
+    #[setter]
+    pub fn set_lstrip_blocks(&self, yes: bool) -> PyResult<()> {
+        self.inner.lock().unwrap().env.set_lstrip_blocks(yes);
+        Ok(())
+    }
+
+    /// Returns the current value of the lstrip blocks flag.
+    #[getter]
+    pub fn get_lstrip_blocks(&self) -> PyResult<bool> {
+        Ok(self.inner.lock().unwrap().env.lstrip_blocks())
+    }
+
     /// Manually adds a template to the environment.
     pub fn add_template(&self, name: String, source: String) -> PyResult<()> {
         let mut inner = self.inner.lock().unwrap();
         inner
             .env
             .add_template_owned(name, source)
             .map_err(to_py_error)
@@ -544,43 +630,43 @@
     ///
     /// The first argument is the name of the template, all other arguments must be passed
     /// as keyword arguments and are pass as render context of the template.
     #[pyo3(signature = (template_name, /, **ctx))]
     pub fn render_template(
         slf: PyRef<'_, Self>,
         template_name: &str,
-        ctx: Option<&PyDict>,
+        ctx: Option<&Bound<'_, PyDict>>,
     ) -> PyResult<String> {
         if slf.reload_before_render.load(Ordering::Relaxed) {
             slf.reload()?;
         }
         bind_environment(slf.as_ptr(), || {
             let inner = slf.inner.lock().unwrap();
             let tmpl = inner.env.get_template(template_name).map_err(to_py_error)?;
             let ctx = ctx
-                .map(|ctx| Value::from_struct_object(DictLikeObject { inner: ctx.into() }))
+                .map(|ctx| Value::from_object(DynamicObject::new(ctx.as_any().clone().unbind())))
                 .unwrap_or_else(|| context!());
             tmpl.render(ctx).map_err(to_py_error)
         })
     }
 
     /// Renders a template from a string
     ///
     /// The first argument is the source of the template, all other arguments must be passed
     /// as keyword arguments and are pass as render context of the template.
     #[pyo3(signature = (source, name=None, /, **ctx))]
     pub fn render_str(
         slf: PyRef<'_, Self>,
         source: &str,
         name: Option<&str>,
-        ctx: Option<&PyDict>,
+        ctx: Option<&Bound<'_, PyDict>>,
     ) -> PyResult<String> {
         bind_environment(slf.as_ptr(), || {
             let ctx = ctx
-                .map(|ctx| Value::from_struct_object(DictLikeObject { inner: ctx.into() }))
+                .map(|ctx| Value::from_object(DynamicObject::new(ctx.as_any().clone().unbind())))
                 .unwrap_or_else(|| context!());
             slf.inner
                 .lock()
                 .unwrap()
                 .env
                 .render_named_str(name.unwrap_or("<string>"), source, ctx)
                 .map_err(to_py_error)
@@ -588,24 +674,24 @@
     }
 
     /// Evaluates an expression with a given context.
     #[pyo3(signature = (expression, /, **ctx))]
     pub fn eval_expr(
         slf: PyRef<'_, Self>,
         expression: &str,
-        ctx: Option<&PyDict>,
+        ctx: Option<&Bound<'_, PyDict>>,
     ) -> PyResult<Py<PyAny>> {
         bind_environment(slf.as_ptr(), || {
             let inner = slf.inner.lock().unwrap();
             let expr = inner
                 .env
                 .compile_expression(expression)
                 .map_err(to_py_error)?;
             let ctx = ctx
-                .map(|ctx| Value::from_struct_object(DictLikeObject { inner: ctx.into() }))
+                .map(|ctx| Value::from_object(DynamicObject::new(ctx.as_any().clone().unbind())))
                 .unwrap_or_else(|| context!());
             to_python_value(expr.eval(ctx).map_err(to_py_error)?)
         })
     }
 }
 
 pub fn with_environment<R, F: FnOnce(Py<Environment>) -> PyResult<R>>(f: F) -> PyResult<R> {
```

### Comparing `minijinja-1.0.8/src/error_support.rs` & `minijinja-2.0.1/src/error_support.rs`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use pyo3::ffi::PyErr_WriteUnraisable;
 use pyo3::prelude::*;
 use pyo3::types::PyTuple;
 
 static TEMPLATE_ERROR: OnceCell<Py<PyAny>> = OnceCell::new();
 
 thread_local! {
-    static STASHED_ERROR: RefCell<Option<PyErr>> = RefCell::new(None);
+    static STASHED_ERROR: RefCell<Option<PyErr>> = const { RefCell::new(None) };
 }
 
 /// Provides information about a template error from the runtime.
 #[pyclass(subclass, module = "minijinja._lowlevel", name = "ErrorInfo")]
 pub struct ErrorInfo {
     err: minijinja::Error,
 }
@@ -92,15 +92,15 @@
         PyErr_WriteUnraisable(std::ptr::null_mut());
     }
 }
 
 fn make_error(err: Error) -> PyErr {
     Python::with_gil(|py| {
         let template_error: &Py<PyAny> = TEMPLATE_ERROR.get_or_init(|| {
-            let module = py.import("minijinja._internal").unwrap();
+            let module = py.import_bound("minijinja._internal").unwrap();
             let err = module.getattr("make_error").unwrap();
             err.into()
         });
-        let args = PyTuple::new(py, [PyCell::new(py, ErrorInfo { err }).unwrap()]);
-        PyErr::from_value(template_error.call1(py, args).unwrap().as_ref(py))
+        let args = PyTuple::new_bound(py, [Bound::new(py, ErrorInfo { err }).unwrap()]);
+        PyErr::from_value_bound(template_error.call1(py, args).unwrap().bind(py).clone())
     })
 }
```

### Comparing `minijinja-1.0.8/src/state.rs` & `minijinja-2.0.1/src/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use std::ffi::c_void;
 use std::sync::atomic::{AtomicPtr, Ordering};
 
 use crate::environment::{with_environment, Environment};
 use crate::typeconv::to_python_value;
 
 thread_local! {
-    static CURRENT_STATE: AtomicPtr<c_void> = AtomicPtr::new(std::ptr::null_mut());
+    static CURRENT_STATE: AtomicPtr<c_void> = const { AtomicPtr::new(std::ptr::null_mut()) };
 }
 
 /// A reference to the current state.
 #[pyclass(subclass, module = "minijinja._lowlevel", name = "State")]
 pub struct StateRef;
 
 #[pymethods]
```

### Comparing `minijinja-1.0.8/src/typeconv.rs` & `minijinja-2.0.1/src/typeconv.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,328 +1,287 @@
 use std::collections::BTreeMap;
 use std::fmt;
 use std::sync::{Arc, Mutex};
 
-use minijinja::value::{Object, ObjectKind, SeqObject, StructObject, Value, ValueKind};
+use minijinja::value::{Enumerator, Object, ObjectRepr, Value, ValueKind};
 use minijinja::{AutoEscape, Error, State};
 
 use once_cell::sync::OnceCell;
 use pyo3::prelude::*;
+use pyo3::pybacked::PyBackedStr;
 use pyo3::types::{PyDict, PyList, PySequence, PyTuple};
 
-use crate::error_support::to_minijinja_error;
+use crate::error_support::{to_minijinja_error, to_py_error};
 use crate::state::{bind_state, StateRef};
 
 static AUTO_ESCAPE_CACHE: Mutex<BTreeMap<String, AutoEscape>> = Mutex::new(BTreeMap::new());
 static MARK_SAFE: OnceCell<Py<PyAny>> = OnceCell::new();
 
 fn is_safe_attr(name: &str) -> bool {
     !name.starts_with('_')
 }
 
-pub struct DictLikeObject {
-    pub inner: Py<PyDict>,
+fn is_dictish(val: &Bound<'_, PyAny>) -> bool {
+    val.hasattr("__getitem__").unwrap_or(false) && val.hasattr("items").unwrap_or(false)
 }
 
-impl StructObject for DictLikeObject {
-    fn get_field(&self, name: &str) -> Option<Value> {
-        Python::with_gil(|py| {
-            let inner = self.inner.as_ref(py);
-            inner.get_item(name).map(to_minijinja_value)
-        })
-    }
-
-    fn fields(&self) -> Vec<Arc<str>> {
-        Python::with_gil(|py| {
-            let inner = self.inner.as_ref(py);
-            inner.keys().iter().map(|x| x.to_string().into()).collect()
-        })
-    }
+pub struct DynamicObject {
+    pub inner: Py<PyAny>,
 }
 
-struct ListLikeObject {
-    inner: Py<PySequence>,
-}
-
-impl SeqObject for ListLikeObject {
-    fn get_item(&self, idx: usize) -> Option<Value> {
-        Python::with_gil(|py| {
-            let inner = self.inner.as_ref(py);
-            inner.get_item(idx).ok().map(to_minijinja_value)
-        })
+impl DynamicObject {
+    pub fn new(inner: Py<PyAny>) -> DynamicObject {
+        DynamicObject { inner }
     }
-
-    fn item_count(&self) -> usize {
-        Python::with_gil(|py| self.inner.as_ref(py).len().unwrap_or(0))
-    }
-}
-
-struct DynamicObject {
-    inner: Py<PyAny>,
-    sequencified: Option<Vec<Py<PyAny>>>,
 }
 
 impl fmt::Debug for DynamicObject {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        fmt::Display::fmt(&self, f)
-    }
-}
-
-impl fmt::Display for DynamicObject {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        Python::with_gil(|py| write!(f, "{}", self.inner.as_ref(py)))
+        Python::with_gil(|py| write!(f, "{}", self.inner.bind(py)))
     }
 }
 
 impl Object for DynamicObject {
-    fn kind(&self) -> ObjectKind<'_> {
+    fn repr(self: &Arc<Self>) -> ObjectRepr {
         Python::with_gil(|py| {
-            let inner = self.inner.as_ref(py);
-            if inner.downcast::<PySequence>().is_ok() || self.sequencified.is_some() {
-                ObjectKind::Seq(self)
+            let inner = self.inner.bind(py);
+            if inner.downcast::<PySequence>().is_ok() {
+                ObjectRepr::Seq
+            } else if is_dictish(inner) {
+                ObjectRepr::Map
+            } else if inner.iter().is_ok() {
+                ObjectRepr::Iterable
             } else {
-                ObjectKind::Struct(self)
+                ObjectRepr::Plain
             }
         })
     }
 
-    fn call(&self, state: &State, args: &[Value]) -> Result<Value, Error> {
+    fn render(self: &Arc<Self>, f: &mut fmt::Formatter<'_>) -> fmt::Result
+    where
+        Self: Sized + 'static,
+    {
+        Python::with_gil(|py| write!(f, "{}", self.inner.bind(py)))
+    }
+
+    fn call(self: &Arc<Self>, state: &State, args: &[Value]) -> Result<Value, Error> {
         Python::with_gil(|py| -> Result<Value, Error> {
             bind_state(state, || {
-                let inner = self.inner.as_ref(py);
+                let inner = self.inner.bind(py);
                 let (py_args, py_kwargs) =
                     to_python_args(py, inner, args).map_err(to_minijinja_error)?;
                 Ok(to_minijinja_value(
-                    inner.call(py_args, py_kwargs).map_err(to_minijinja_error)?,
+                    &inner
+                        .call(py_args, py_kwargs.as_ref())
+                        .map_err(to_minijinja_error)?,
                 ))
             })
         })
     }
 
-    fn call_method(&self, state: &State, name: &str, args: &[Value]) -> Result<Value, Error> {
+    fn call_method(
+        self: &Arc<Self>,
+        state: &State,
+        name: &str,
+        args: &[Value],
+    ) -> Result<Value, Error> {
         if !is_safe_attr(name) {
             return Err(Error::new(
                 minijinja::ErrorKind::InvalidOperation,
                 "insecure method call",
             ));
         }
         Python::with_gil(|py| -> Result<Value, Error> {
             bind_state(state, || {
-                let inner = self.inner.as_ref(py);
+                let inner = self.inner.bind(py);
                 let (py_args, py_kwargs) =
                     to_python_args(py, inner, args).map_err(to_minijinja_error)?;
                 Ok(to_minijinja_value(
-                    inner
-                        .call_method(name, py_args, py_kwargs)
+                    &inner
+                        .call_method(name, py_args, py_kwargs.as_ref())
                         .map_err(to_minijinja_error)?,
                 ))
             })
         })
     }
-}
 
-impl SeqObject for DynamicObject {
-    fn get_item(&self, idx: usize) -> Option<Value> {
+    fn get_value(self: &Arc<Self>, key: &Value) -> Option<Value> {
         Python::with_gil(|py| {
-            if let Some(ref seq) = self.sequencified {
-                return seq.get(idx).map(|x| to_minijinja_value(x.as_ref(py)));
-            }
-            let inner = self.inner.as_ref(py);
-            if let Ok(seq) = inner.downcast::<PySequence>() {
-                seq.get_item(idx).ok().map(to_minijinja_value)
-            } else {
-                None
+            let inner = self.inner.bind(py);
+            match inner.get_item(to_python_value_impl(py, key.clone()).ok()?) {
+                Ok(value) => Some(to_minijinja_value(&value)),
+                Err(_) => {
+                    if let Some(attr) = key.as_str() {
+                        if is_safe_attr(attr) {
+                            if let Ok(rv) = inner.getattr(attr) {
+                                return Some(to_minijinja_value(&rv));
+                            }
+                        }
+                    }
+                    None
+                }
             }
         })
     }
 
-    fn item_count(&self) -> usize {
+    fn enumerate(self: &Arc<Self>) -> Enumerator {
         Python::with_gil(|py| {
-            if let Some(ref seq) = self.sequencified {
-                seq.len()
+            let inner = self.inner.bind(py);
+            if inner.downcast::<PySequence>().is_ok() {
+                Enumerator::Seq(inner.len().unwrap_or(0))
+            } else if let Ok(iter) = inner.iter() {
+                Enumerator::Values(
+                    iter.filter_map(|x| match x {
+                        Ok(x) => Some(to_minijinja_value(&x)),
+                        Err(_) => None,
+                    })
+                    .collect(),
+                )
             } else {
-                let inner = self.inner.as_ref(py);
-                inner.len().unwrap_or(0)
+                Enumerator::NonEnumerable
             }
         })
     }
 }
 
-impl StructObject for DynamicObject {
-    fn get_field(&self, name: &str) -> Option<Value> {
-        if !is_safe_attr(name) {
-            return None;
-        }
-        Python::with_gil(|py| {
-            let inner = self.inner.as_ref(py);
-            inner.getattr(name).map(to_minijinja_value).ok()
-        })
-    }
-}
-
-pub fn to_minijinja_value(value: &PyAny) -> Value {
-    if let Ok(dict) = value.downcast::<PyDict>() {
-        Value::from_struct_object(DictLikeObject { inner: dict.into() })
-    } else if let Ok(tup) = value.downcast::<PyTuple>() {
-        Value::from_seq_object(ListLikeObject {
-            inner: tup.as_sequence().into(),
-        })
-    } else if let Ok(list) = value.downcast::<PyList>() {
-        Value::from_seq_object(ListLikeObject {
-            inner: list.as_sequence().into(),
-        })
-    } else if value.is_none() {
+pub fn to_minijinja_value(value: &Bound<'_, PyAny>) -> Value {
+    if value.is_none() {
         Value::from(())
     } else if let Ok(val) = value.extract::<bool>() {
         Value::from(val)
     } else if let Ok(val) = value.extract::<i64>() {
         Value::from(val)
     } else if let Ok(val) = value.extract::<f64>() {
         Value::from(val)
-    } else if let Ok(val) = value.extract::<&str>() {
+    } else if let Ok(val) = value.extract::<PyBackedStr>() {
         if let Ok(to_html) = value.getattr("__html__") {
             if to_html.is_callable() {
                 // TODO: if to_minijinja_value returns results we could
                 // report the swallowed error of __html__.
                 if let Ok(html) = to_html.call0() {
-                    if let Ok(val) = html.extract::<&str>() {
-                        return Value::from_safe_string(val.into());
+                    if let Ok(val) = html.extract::<PyBackedStr>() {
+                        return Value::from_safe_string(val.to_string());
                     }
                 }
             }
         }
-        Value::from(val)
+        Value::from(val.to_string())
     } else {
-        let mut sequencified = None;
-        if let Ok(iter) = value.iter() {
-            let mut seq = Vec::new();
-            for value in iter.flatten() {
-                seq.push(value.into());
-            }
-            sequencified = Some(seq);
-        }
-        Value::from_object(DynamicObject {
-            inner: value.into(),
-            sequencified,
-        })
+        Value::from_object(DynamicObject::new(value.clone().unbind()))
     }
 }
 
 pub fn to_python_value(value: Value) -> PyResult<Py<PyAny>> {
     Python::with_gil(|py| to_python_value_impl(py, value))
 }
 
 fn mark_string_safe(py: Python<'_>, value: &str) -> PyResult<Py<PyAny>> {
     let mark_safe: &Py<PyAny> = MARK_SAFE.get_or_try_init::<_, PyErr>(|| {
-        let module = py.import("minijinja._internal")?;
+        let module = py.import_bound("minijinja._internal")?;
         Ok(module.getattr("mark_safe")?.into())
     })?;
-    mark_safe.call1(py, PyTuple::new(py, [value]))
+    mark_safe.call1(py, PyTuple::new_bound(py, [value]))
 }
 
 fn to_python_value_impl(py: Python<'_>, value: Value) -> PyResult<Py<PyAny>> {
     // if we are holding a true dynamic object, we want to allow bidirectional
     // conversion.  That means that when passing the object back to Python we
     // extract the retained raw Python reference.
     if let Some(pyobj) = value.downcast_object_ref::<DynamicObject>() {
         return Ok(pyobj.inner.clone());
     }
 
-    if let Some(seq) = value.as_seq() {
-        let rv = PyList::empty(py);
-        for idx in 0..seq.item_count() {
-            if let Some(item) = seq.get_item(idx) {
-                rv.append(to_python_value_impl(py, item)?)?;
-            } else {
-                rv.append(py.None())?;
-            }
-        }
-        Ok(rv.into())
-    } else if let Some(s) = value.as_struct() {
-        let rv = PyDict::new(py);
-        for field in s.fields().into_iter() {
-            if let Some(value) = s.get_field(&field) {
-                rv.set_item(&field as &str, to_python_value_impl(py, value)?)?;
-            }
-        }
-        Ok(rv.into())
-    } else {
-        match value.kind() {
-            ValueKind::Undefined | ValueKind::None => Ok(().into_py(py)),
-            ValueKind::Bool => Ok(value.is_true().into_py(py)),
-            ValueKind::Number => {
-                if let Ok(rv) = TryInto::<i64>::try_into(value.clone()) {
-                    Ok(rv.into_py(py))
-                } else if let Ok(rv) = TryInto::<u64>::try_into(value.clone()) {
-                    Ok(rv.into_py(py))
-                } else if let Ok(rv) = TryInto::<f64>::try_into(value) {
-                    Ok(rv.into_py(py))
-                } else {
-                    unreachable!()
-                }
-            }
-            ValueKind::String => {
-                if value.is_safe() {
-                    Ok(mark_string_safe(py, value.as_str().unwrap())?)
-                } else {
-                    Ok(value.as_str().unwrap().into_py(py))
+    if let Some(obj) = value.as_object() {
+        match obj.repr() {
+            ObjectRepr::Plain => return Ok(obj.to_string().into_py(py)),
+            ObjectRepr::Map => {
+                let rv = PyDict::new_bound(py);
+                if let Some(pair_iter) = obj.try_iter_pairs() {
+                    for (key, value) in pair_iter {
+                        rv.set_item(
+                            to_python_value_impl(py, key)?,
+                            to_python_value_impl(py, value)?,
+                        )?;
+                    }
                 }
+                return Ok(rv.into());
             }
-            ValueKind::Bytes => Ok(value.as_bytes().unwrap().into_py(py)),
-            // this should be covered above
-            ValueKind::Seq => unreachable!(),
-            ValueKind::Map => {
-                let rv = PyDict::new(py);
-                if let Ok(iter) = value.try_iter() {
-                    for k in iter {
-                        if let Ok(v) = value.get_item(&k) {
-                            rv.set_item(
-                                to_python_value_impl(py, k)?,
-                                to_python_value_impl(py, v)?,
-                            )?;
-                        }
+            ObjectRepr::Seq | ObjectRepr::Iterable => {
+                let rv = PyList::empty_bound(py);
+                if let Some(iter) = obj.try_iter() {
+                    for value in iter {
+                        rv.append(to_python_value_impl(py, value)?)?;
                     }
                 }
-                Ok(rv.into())
+                return Ok(rv.into());
+            }
+            _ => {}
+        }
+    }
+
+    match value.kind() {
+        ValueKind::Undefined | ValueKind::None => Ok(().into_py(py)),
+        ValueKind::Bool => Ok(value.is_true().into_py(py)),
+        ValueKind::Number => {
+            if let Ok(rv) = TryInto::<i64>::try_into(value.clone()) {
+                Ok(rv.into_py(py))
+            } else if let Ok(rv) = TryInto::<u64>::try_into(value.clone()) {
+                Ok(rv.into_py(py))
+            } else if let Ok(rv) = TryInto::<f64>::try_into(value) {
+                Ok(rv.into_py(py))
+            } else {
+                unreachable!()
+            }
+        }
+        ValueKind::String => {
+            if value.is_safe() {
+                Ok(mark_string_safe(py, value.as_str().unwrap())?)
+            } else {
+                Ok(value.as_str().unwrap().into_py(py))
             }
         }
+        ValueKind::Bytes => Ok(value.as_bytes().unwrap().into_py(py)),
+        kind => Err(to_py_error(minijinja::Error::new(
+            minijinja::ErrorKind::InvalidOperation,
+            format!("object {} cannot roundtrip", kind),
+        ))),
     }
 }
 
 pub fn to_python_args<'py>(
     py: Python<'py>,
-    callback: &PyAny,
+    callback: &Bound<'_, PyAny>,
     args: &[Value],
-) -> PyResult<(&'py PyTuple, Option<&'py PyDict>)> {
+) -> PyResult<(Bound<'py, PyTuple>, Option<Bound<'py, PyDict>>)> {
     let mut py_args = Vec::new();
     let mut py_kwargs = None;
 
     if callback
         .getattr("__minijinja_pass_state__")
-        .map_or(false, |x| x.is_true().unwrap_or(false))
+        .map_or(false, |x| x.is_truthy().unwrap_or(false))
     {
-        py_args.push(Py::new(py, StateRef)?.to_object(py));
+        py_args.push(Bound::new(py, StateRef)?.to_object(py));
     }
 
     for arg in args {
         if arg.is_kwargs() {
-            let kwargs = py_kwargs.get_or_insert_with(|| PyDict::new(py));
+            let kwargs = py_kwargs.get_or_insert_with(|| PyDict::new_bound(py));
             if let Ok(iter) = arg.try_iter() {
                 for k in iter {
                     if let Ok(v) = arg.get_item(&k) {
                         kwargs
                             .set_item(to_python_value_impl(py, k)?, to_python_value_impl(py, v)?)?;
                     }
                 }
             }
         } else {
             py_args.push(to_python_value_impl(py, arg.clone())?);
         }
     }
-    let py_args = PyTuple::new(py, py_args);
+    let py_args = PyTuple::new_bound(py, py_args);
     Ok((py_args, py_kwargs))
 }
 
 pub fn get_custom_autoescape(value: &str) -> AutoEscape {
     let mut cache = AUTO_ESCAPE_CACHE.lock().unwrap();
     if let Some(rv) = cache.get(value).copied() {
         return rv;
```

### Comparing `minijinja-1.0.8/tests/test_basic.py` & `minijinja-2.0.1/tests/test_basic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import binascii
 import pytest
 import posixpath
+import types
 
 from _pytest.unraisableexception import catch_unraisable_exception
-from minijinja import Environment, TemplateError, safe, pass_state
+from minijinja import Environment, TemplateError, safe, pass_state, eval_expr, render_str
 
 
 def test_expression():
     env = Environment()
     rv = env.eval_expr("1 + b", b=42)
     assert rv == 43
     rv = env.eval_expr("range(n)", n=10)
@@ -31,21 +32,23 @@
     env = Environment()
     rv = env.eval_expr("[hmm.public_attr, hmm.__module__]", hmm=hmm)
     assert rv == [42, None]
 
 
 def test_generator():
     def hmm():
-        # This implicitly gets converted into a list. It's not a real iterator.
         yield 1
         yield 2
         yield 3
 
     hmm.public_attr = 42
     env = Environment()
+    rv = env.eval_expr("values", values=hmm())
+    assert isinstance(rv, types.GeneratorType)
+
     rv = env.eval_expr("values|list", values=hmm())
     assert rv == [1, 2, 3]
 
 
 def test_method_calling():
     class MyClass(object):
         def my_method(self):
@@ -53,14 +56,25 @@
 
         def __repr__(self):
             return "This is X"
 
     env = Environment()
     rv = env.eval_expr("[x ~ '', x.my_method()]", x=MyClass())
     assert rv == ["This is X", 23]
+    rv = env.eval_expr("x.items()|list", x={"a": "b"})
+    assert rv == [("a", "b")]
+
+
+def test_types_passthrough():
+    tup = (1, 2, 3)
+    assert eval_expr("x", x=tup) == tup
+    assert render_str("{{ x }}", x=tup) == "(1, 2, 3)"
+    assert eval_expr("x is sequence", x=tup) == True
+    assert render_str("{{ x }}", x=(1, True)) == "(1, True)"
+    assert eval_expr("x[0] == 42", x=[42]) == True
 
 
 def test_custom_filter():
     def my_filter(value):
         return "<%s>" % value.upper()
 
     env = Environment()
@@ -275,8 +289,55 @@
         assert cm.unraisable is None
 
 
 def test_keep_trailing_newline():
     env = Environment(keep_trailing_newline=False)
     assert env.render_str("foo\n") == "foo"
     env = Environment(keep_trailing_newline=True)
-    assert env.render_str("foo\n") == "foo\n"
+    assert env.render_str("foo\n") == "foo\n"
+
+
+def test_trim_blocks():
+    env = Environment(trim_blocks=False)
+    assert env.render_str("{% if true %}\nfoo{% endif %}") == "\nfoo"
+    env = Environment(trim_blocks=True)
+    assert env.render_str("{% if true %}\nfoo{% endif %}") == "foo"
+
+
+def test_lstrip_blocks():
+    env = Environment(lstrip_blocks=False)
+    assert env.render_str("  {% if true %}\nfoo{% endif %}") == "  \nfoo"
+    env = Environment(lstrip_blocks=True)
+    assert env.render_str("  {% if true %}\nfoo{% endif %}") == "\nfoo"
+
+
+def test_trim_and_lstrip_blocks():
+    env = Environment(lstrip_blocks=False, trim_blocks=False)
+    assert env.render_str("  {% if true %}\nfoo{% endif %}") == "  \nfoo"
+    env = Environment(lstrip_blocks=True, trim_blocks=True)
+    assert env.render_str("  {% if true %}\nfoo{% endif %}") == "foo"
+
+
+def test_line_statements():
+    env = Environment()
+    assert env.line_statement_prefix is None
+    assert env.line_comment_prefix is None
+
+    env = Environment(line_statement_prefix="#", line_comment_prefix="##")
+    assert env.line_statement_prefix == "#"
+    assert env.line_comment_prefix == "##"
+
+    rv = env.render_str("# for x in range(3)\n{{ x }}\n# endfor")
+    assert rv == "0\n1\n2\n"
+
+
+def test_custom_delimiters():
+    env = Environment(
+        variable_start_string="${",
+        variable_end_string="}",
+        block_start_string="<%",
+        block_end_string="%>",
+        comment_start_string="<!--",
+        comment_end_string="-->",
+    )
+    rv = env.render_str('<% if true %>${ value }<% endif %><!-- nothing -->', value=42)
+    assert rv == '42'
```

### Comparing `minijinja-1.0.8/tests/test_security.py` & `minijinja-2.0.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/tests/test_state.py` & `minijinja-2.0.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `minijinja-1.0.8/Cargo.lock` & `minijinja-2.0.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "actix-codec"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "617a8268e3537fe1d8c9ead925fca49ef6400927ee7bc26750e90ecee14ce4b8"
+checksum = "5f7b0a21988c1bf877cf4759ef5ddaac04c1c9fe808c9142ecb78ba97d97a28a"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "bytes",
  "futures-core",
  "futures-sink",
  "memchr",
  "pin-project-lite",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "actix-http"
-version = "3.4.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a92ef85799cba03f76e4f7c10f533e66d87c9a7e7055f3391f09000ad8351bc9"
+checksum = "d223b13fd481fc0d1f83bb12659ae774d9e3601814c68a0bc539731698cca743"
 dependencies = [
  "actix-codec",
  "actix-rt",
  "actix-service",
  "actix-utils",
  "ahash",
  "base64",
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "brotli",
  "bytes",
  "bytestring",
  "derive_more",
  "encoding_rs",
  "flate2",
  "futures-core",
@@ -61,22 +61,22 @@
 [[package]]
 name = "actix-macros"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e01ed3140b2f8d422c68afa1ed2e85d996ea619c988ac834d255db32138655cb"
 dependencies = [
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "actix-router"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d66ff4d247d2b160861fa2866457e85706833527840e4133f8f49aa423a38799"
+checksum = "d22475596539443685426b6bdadb926ad0ecaefdfc5fb05e5e3441f15463c511"
 dependencies = [
  "bytestring",
  "http",
  "regex",
  "serde",
  "tracing",
 ]
@@ -127,17 +127,17 @@
 dependencies = [
  "local-waker",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "actix-web"
-version = "4.4.0"
+version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e4a5b5e29603ca8c94a77c65cf874718ceb60292c5a5c3e5f4ace041af462b9"
+checksum = "43a6556ddebb638c2358714d853257ed226ece6023ef9364f23f0c70737ea984"
 dependencies = [
  "actix-codec",
  "actix-http",
  "actix-macros",
  "actix-router",
  "actix-rt",
  "actix-server",
@@ -174,15 +174,15 @@
 version = "4.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb1f50ebbb30eca122b188319a4398b3f7bb4a8cdf50ecfb73bfc6a3c3ce54f5"
 dependencies = [
  "actix-router",
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "actix-web-demo"
 version = "0.1.0"
 dependencies = [
  "actix-web",
@@ -202,29 +202,30 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.3"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
+ "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.5"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c378d78423fdad8089616f827526ee33c19f2fddbd5de1629152c9593ba4783"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -259,23 +260,23 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.3"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b84bf0a05bbb2a83e5eb6fa36bb6e87baa08193c35ff52bbf6b38d8af2890e46"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "anymap2"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d301b3b94cb4b2f23d7917810addbbaff90738e0ca2be692bd027e70d7e0330c"
 
@@ -294,83 +295,68 @@
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56df0aeedf6b7a2fc67d06db35b09684c3e8da0c95f8f27685cb17e08413d87a"
 dependencies = [
  "argh_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "argh_shared"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5693f39141bda5760ecc4111ab08da40565d1771038c4a0250f03457ec707531"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "askama"
-version = "0.11.1"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb98f10f371286b177db5eeb9a6e5396609555686a35e1d4f7b9a9c6d8af0139"
+checksum = "b79091df18a97caea757e28cd2d5fda49c6cd4bd01ddffd7ff01ace0c0ad2c28"
 dependencies = [
  "askama_derive",
  "askama_escape",
- "askama_shared",
+ "humansize",
+ "num-traits",
+ "percent-encoding",
 ]
 
 [[package]]
 name = "askama_derive"
-version = "0.11.2"
+version = "0.12.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87bf87e6e8b47264efa9bde63d6225c6276a52e05e91bf37eaa8afd0032d6b71"
+checksum = "19fe8d6cb13c4714962c072ea496f3392015f0989b1a2847bb4b2d9effd71d83"
 dependencies = [
- "askama_shared",
+ "askama_parser",
+ "basic-toml",
+ "mime",
+ "mime_guess",
  "proc-macro2",
- "syn 1.0.109",
+ "quote",
+ "serde",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "askama_escape"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "619743e34b5ba4e9703bba34deac3427c72507c7159f5fd030aea8cac0cfe341"
 
 [[package]]
-name = "askama_shared"
-version = "0.12.2"
+name = "askama_parser"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf722b94118a07fcbc6640190f247334027685d4e218b794dbfe17c32bf38ed0"
+checksum = "acb1161c6b64d1c3d83108213c2a2533a342ac225aabd0bda218278c2ddb00c0"
 dependencies = [
- "askama_escape",
- "humansize 1.1.1",
- "mime",
- "mime_guess",
  "nom",
- "num-traits",
- "percent-encoding",
- "proc-macro2",
- "quote",
- "serde",
- "syn 1.0.109",
- "toml 0.5.11",
-]
-
-[[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -381,32 +367,41 @@
 dependencies = [
  "minijinja",
  "minijinja-autoreload",
 ]
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "95d8e92cac0961e91dbd517496b00f7e9b92363dbe6d42c3198268323798860c"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.4"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ba43ea6f343b788c8764558649e08df62f86c6ef251fdaeb1ffd010a9ae50a2"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+
+[[package]]
+name = "basic-toml"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "823388e228f614e9558c6804262db37960ec8821856535f5c3f59913140558f8"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "benchmarks"
 version = "0.1.0"
 dependencies = [
  "askama",
  "criterion",
@@ -431,17 +426,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
@@ -452,28 +447,28 @@
 name = "boolinator"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfa8873f51c92e232f9bac4065cddef41b714152812bfc5f7672ba16d6ef8cd9"
 
 [[package]]
 name = "brotli"
-version = "3.3.4"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1a0b1dbcc8ae29329621f8d4f0d835787c1c38bb1401979b49d13b0b305ff68"
+checksum = "d640d25bc63c50fb1f0b545ffd80207d2e10a4c965530809b40ba3386825c391"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "2.3.4"
+version = "2.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b6561fd3f895a11e8f72af2cb7d22e08366bebc2b6b57f7744c4bda27034744"
+checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bstr"
@@ -484,46 +479,46 @@
  "lazy_static",
  "memchr",
  "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "bstr"
-version = "1.6.2"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c2f7349907b712260e64b0afe2f84692af14a454be26187d9df565c7f69266a"
+checksum = "05efc5cfd9110c8416e471df0e96702d58690178e206e61b7173706673c93706"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "build-script"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "bytestring"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "238e4886760d98c4f899360c834fa93e62cf7f721ac3c2da375cbdf4b8679aae"
+checksum = "74d80203ea6b29df88012294f62733de21cfeab47f17b41af3a38bc30a03ee72"
 dependencies = [
  "bytes",
 ]
 
 [[package]]
 name = "call-block-function"
 version = "0.1.0"
@@ -535,159 +530,177 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.3"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1369bc6b9e9a7dfdae2055f6ec151fe9c554a9d23d357c0237cee2e25eaabb7"
+checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
 name = "chrono-tz-build"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2f5ebdc942f57ed96d560a6d1a459bae5851102a25d5bf89dc04ae453e31ecf"
+checksum = "433e39f13c9a060046954e0592a8d0a4bcb1040125cbf91cb8ee58964cfb350f"
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.25"
+version = "4.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
+checksum = "949626d00e063efc93b6dca932419ceb5432f99769911c0b995f7e884c778813"
 dependencies = [
- "bitflags 1.3.2",
- "clap_lex 0.2.4",
- "indexmap 1.9.3",
- "textwrap",
+ "clap_builder",
 ]
 
 [[package]]
-name = "clap"
-version = "4.4.3"
+name = "clap_builder"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84ed82781cea27b43c9b106a979fe450a13a31aab0500595fb3fc06616de08e6"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
- "clap_builder",
+ "anstyle",
+ "clap_lex",
 ]
 
 [[package]]
-name = "clap_builder"
-version = "4.4.2"
+name = "clap_complete"
+version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bb9faaa7c2ef94b2743a21f5a29e6f0010dff4caa69ac8e9d6cf8b6fa74da08"
+checksum = "885e4d7d5af40bfb99ae6f9433e292feac98d452dcb3ec3d25dfe7552b77da8c"
 dependencies = [
- "anstyle",
- "clap_lex 0.5.1",
+ "clap",
 ]
 
 [[package]]
-name = "clap_lex"
-version = "0.2.4"
+name = "clap_complete_fig"
+version = "4.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+checksum = "54b3e65f91fabdd23cac3d57d39d5d938b4daabd070c335c006dccb866a61110"
 dependencies = [
- "os_str_bytes",
+ "clap",
+ "clap_complete",
+]
+
+[[package]]
+name = "clap_complete_nushell"
+version = "4.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0e48e026ce7df2040239117d25e4e79714907420c70294a5ce4b6bbe6a7b6"
+dependencies = [
+ "clap",
+ "clap_complete",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.5.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
+
+[[package]]
+name = "clap_mangen"
+version = "0.2.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1dd95b5ebb5c1c54581dd6346f3ed6a79a3eef95dd372fc2ac13d535535300e"
+dependencies = [
+ "clap",
+ "roff",
+]
 
 [[package]]
 name = "clipboard-win"
 version = "4.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7191c27c2357d9b7ef96baac1773290d4ca63b24205b82a3fd8a0637afcf0362"
 dependencies = [
  "error-code",
  "str-buf",
  "winapi",
 ]
 
 [[package]]
 name = "console"
-version = "0.15.7"
+version = "0.15.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
+checksum = "0e1f83fc076bd6dd27517eacdf25fef6c4dfe5f1d7448bafaaf3a26f13b5e4eb"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
@@ -711,51 +724,51 @@
  "percent-encoding",
  "time",
  "version_check",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
- "clap 3.2.25",
+ "clap",
  "criterion-plot",
+ "is-terminal",
  "itertools",
- "lazy_static",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -770,55 +783,43 @@
 checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
-name = "crossbeam-channel"
-version = "0.5.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
-dependencies = [
- "cfg-if",
- "crossbeam-utils",
-]
-
-[[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset 0.9.0",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
@@ -838,18 +839,19 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "deranged"
-version = "0.3.8"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2696e8a945f658fd14dc3b87242e6b80cd0f36ff04ea560fa39082368847946"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
+ "powerfmt",
  "serde",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -868,17 +870,17 @@
 dependencies = [
  "minijinja",
  "serde",
 ]
 
 [[package]]
 name = "deunicode"
-version = "0.4.4"
+version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d95203a6a50906215a502507c0f879a0ce7ff205a6111e2db2a5ef8e4bb92e43"
+checksum = "b6e854126756c496b8c81dec88f9a706b15b875c5849d4097a3854476b9fdf94"
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
@@ -917,17 +919,25 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+
+[[package]]
+name = "embedding"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+ "minijinja-embed",
+]
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -950,31 +960,20 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "136526188508e25c6fef639d7927dfb3e0e3084488bf202267829cf7fc23dbdd"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys 0.48.0",
-]
-
-[[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "error"
 version = "0.1.0"
 dependencies = [
  "minijinja",
@@ -1002,64 +1001,70 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde_json",
 ]
 
 [[package]]
+name = "fastrand"
+version = "2.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+
+[[package]]
 name = "fd-lock"
 version = "3.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef033ed5e9bad94e55838ca0ca906db0e043f517adda0c8b79c7a8c66c93c1b5"
 dependencies = [
  "cfg-if",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.22"
+version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4029edd3e734da6fe05b6cd7bd2960760a616bd2ddd0d59a0124746d6272af0"
+checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "filters"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6c98ee8095e9d1dcbf2fcc6d95acccb90d1c81db1e44725c6a984b1dbdfb010"
+checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fsevent-sys"
 version = "4.1.0"
@@ -1067,76 +1072,76 @@
 checksum = "76ee7a02da4d231650c7cea31349b889be2f45ddb3ef3032d2ec8185f6313fd2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-io"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1161,40 +1166,40 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "globset"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "759c97c1e17c55525b57192c06a267cda0ac5210b222d6b82189a2338fa1c13d"
+checksum = "57da3b9b5b85bd66f31093f8c408b90a74431672542466497dcbdfdc02034be1"
 dependencies = [
  "aho-corasick",
- "bstr 1.6.2",
- "fnv",
+ "bstr 1.9.1",
  "log",
- "regex",
+ "regex-automata 0.4.6",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "globwalk"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93e3af942408868f6934a7b85134a3230832b9977cf66125df2f9edcfce4ddcc"
@@ -1368,42 +1373,46 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.21"
+version = "0.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91fc23aa11be92976ef4729127f1a74adf36d8436f7816b185d18df956790833"
+checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 1.9.3",
+ "indexmap 2.2.5",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+dependencies = [
+ "cfg-if",
+ "crunchy",
+]
 
 [[package]]
 name = "handlebars"
-version = "4.4.0"
+version = "5.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c39b3bc2a8f715298032cf5087e58573809374b08160aa7d750582bdb82d2683"
+checksum = "d08485b96a0e6393e9e4d1b8d48cf74ad6c063cd905eb33f42c1ce3f0377539b"
 dependencies = [
  "log",
  "pest",
  "pest_derive",
  "serde",
  "serde_json",
  "thiserror",
@@ -1413,54 +1422,51 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.0"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hello"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.2"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "home"
-version = "0.5.5"
+version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -1473,82 +1479,75 @@
 name = "httpdate"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
 
 [[package]]
 name = "humansize"
-version = "1.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02296996cb8796d7c6e3bc2d9211b7802812d36999a51bb754123ead7d37d026"
-
-[[package]]
-name = "humansize"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6cb51c9a029ddc91b07a787f1d86b53ccfa49b0e86688c946ebe8d3555685dd7"
 dependencies = [
  "libm",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.57"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "ignore"
-version = "0.4.20"
+version = "0.4.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbe7873dab538a9a44ad79ede1faf5f30d49f9a5c883ddbab48bce81b64b7492"
+checksum = "b46810df39e66e925525d6e38ce1e7f6e1d208f72dc39757880fcb66e2c58af1"
 dependencies = [
+ "crossbeam-deque",
  "globset",
- "lazy_static",
  "log",
  "memchr",
- "regex",
+ "regex-automata 0.4.6",
  "same-file",
- "thread_local",
  "walkdir",
  "winapi-util",
 ]
 
 [[package]]
 name = "implicit-clone"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c6ecbd987bb94f1f3c76c6787879756cf4b6f73bfff48d79308e8c56b46f65f"
+checksum = "cfd6201e7c30ccb24773cac7efa6fec1e06189d414b7439ce756a481c8bfbf53"
 dependencies = [
  "indexmap 1.9.3",
 ]
 
 [[package]]
 name = "indexmap"
 version = "1.9.3"
@@ -1557,27 +1556,27 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.0.0"
+version = "2.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.0",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inheritance"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde",
@@ -1602,65 +1601,87 @@
 checksum = "e05c02b5e89bff3b946cedeca278abc628fe811e604f027c45a8aa3cf793d0eb"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "insta"
-version = "1.31.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0770b0a3d4c70567f0d58331f3088b0e4c4f56c9b8d764efe654b4a5d46de3a"
+checksum = "3eab73f58e59ca6526037208f0e98851159ec1633cf17b6cd2e1f2c3fd5d53cc"
 dependencies = [
  "console",
  "globset",
  "lazy_static",
  "linked-hash-map",
+ "regex",
  "serde",
  "similar",
  "walkdir",
- "yaml-rust",
+]
+
+[[package]]
+name = "insta-cmd"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffeeefa927925cced49ccb01bf3e57c9d4cd132df21e576eb9415baeab2d3de6"
+dependencies = [
+ "insta",
+ "serde",
+ "serde_json",
 ]
 
 [[package]]
 name = "invalid-value"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde",
 ]
 
 [[package]]
+name = "is-terminal"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "jobserver"
-version = "0.1.26"
+version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kqueue"
 version = "1.0.8"
@@ -1701,35 +1722,42 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.148"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cdc71e17332e86d2e1d38c1f99edcb6288ee11b815fb1a4b049eaa2114d369b"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
+
+[[package]]
+name = "line-statements"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.7"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a9bad9f94746442c783ca431b22403b519cd7fbeed0533fdd6328b2f2212128"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "liquid"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69f68ae1011499ae2ef879f631891f21c78e309755f4a5e483c4a8f12e10b609"
 dependencies = [
@@ -1762,15 +1790,15 @@
 name = "liquid-derive"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc2fb41a9bb4257a3803154bdf7e2df7d45197d1941c9b1a90ad815231630721"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "liquid-lib"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2a17e273a6fb1fb6268f7a5867ddfd0bd4683c7e19b51084f3d567fad4348c0"
@@ -1798,79 +1826,69 @@
 dependencies = [
  "minijinja",
  "serde_json",
 ]
 
 [[package]]
 name = "local-channel"
-version = "0.1.3"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f303ec0e94c6c54447f84f3b0ef7af769858a9c4ef56ef2a986d3dcd4c3fc9c"
+checksum = "b6cbc85e69b8df4b8bb8b89ec634e7189099cea8927a276b7384ce5488e53ec8"
 dependencies = [
  "futures-core",
  "futures-sink",
- "futures-util",
  "local-waker",
 ]
 
 [[package]]
 name = "local-waker"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e34f76eb3611940e0e7d53a9aaa4e6a3151f69541a282fd0dad5571420c53ff1"
+checksum = "4d873d7c67ce09b42110d801813efbc9364414e356be9935700d368351657487"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "macros"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memo-map"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "374c335b2df19e62d4cb323103473cbc6510980253119180de862d89184f6a83"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "merge-context"
 version = "0.1.0"
@@ -1893,112 +1911,117 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "1.0.8"
+version = "2.0.1"
 dependencies = [
  "aho-corasick",
  "indexmap 1.9.3",
  "insta",
  "memo-map",
  "percent-encoding",
  "self_cell",
  "serde",
  "serde_json",
  "similar-asserts",
+ "stacker",
  "unicase",
  "unicode-ident",
  "v_htmlescape",
 ]
 
 [[package]]
 name = "minijinja-autoreload"
-version = "1.0.8"
+version = "2.0.1"
 dependencies = [
  "minijinja",
  "notify",
 ]
 
 [[package]]
 name = "minijinja-cli"
-version = "1.0.8"
+version = "2.0.1"
 dependencies = [
  "anyhow",
  "ciborium",
- "clap 4.4.3",
+ "clap",
+ "clap_complete",
+ "clap_complete_fig",
+ "clap_complete_nushell",
+ "clap_mangen",
  "dunce",
+ "insta",
+ "insta-cmd",
  "minijinja",
  "minijinja-contrib",
  "rustyline",
  "serde",
  "serde_json",
  "serde_json5",
  "serde_qs",
  "serde_yaml",
- "toml 0.7.8",
+ "tempfile",
+ "toml",
 ]
 
 [[package]]
 name = "minijinja-contrib"
-version = "1.0.8"
+version = "2.0.1"
 dependencies = [
  "chrono",
  "minijinja",
  "serde",
  "similar-asserts",
  "time",
  "time-tz",
 ]
 
 [[package]]
+name = "minijinja-embed"
+version = "2.0.1"
+
+[[package]]
 name = "minijinja-py"
-version = "1.0.8"
+version = "2.0.1"
 dependencies = [
  "minijinja",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
-name = "minijinja-stack-ref"
-version = "1.0.8"
-dependencies = [
- "minijinja",
-]
-
-[[package]]
 name = "minimal"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
@@ -2029,14 +2052,22 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "none-as-undefined"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+ "serde",
+]
+
+[[package]]
 name = "notify"
 version = "5.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "729f63e1ca555a43fe3efa4f3efdf4801c479da85b432242a7b726f353c88486"
 dependencies = [
  "bitflags 1.3.2",
  "filetime",
@@ -2046,74 +2077,81 @@
  "libc",
  "mio",
  "walkdir",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.3.2",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "object-ref"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
@@ -2139,57 +2177,57 @@
 dependencies = [
  "minijinja",
  "once_cell",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.3.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.3"
+version = "2.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7a4d085fd991ac8d5b05a147b437791b4260b76326baf0fc60cf7c9c27ecd33"
+checksum = "56f8023d0fb78c8e03784ea1c7f3fa36e68a723138990b8d5a47d916b651e7a8"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.7.3"
+version = "2.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bee7be22ce7918f641a33f08e3f43388c7656772244e2bbb2477f44cc9021a"
+checksum = "b0d24f72393fd16ab6ac5738bc33cdb6a9aa73f8b902e8fe29cf4e67d7dd1026"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.7.3"
+version = "2.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1511785c5e98d79a05e8a6bc34b4ac2168a0e3e92161862030ad84daa223141"
+checksum = "fdc17e2a6c7d0a492f0158d7a4bd66cc17280308bbaff78d5bef566dca35ab80"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.7.3"
+version = "2.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b42f0394d3123e33353ca5e1e89092e533d2cc490389f2bd6131c43c634ebc5f"
+checksum = "934cd7631c050f4674352a6e835d5f6711ffbfb9345c2fc0107155ac495ae293"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -2228,30 +2266,30 @@
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.1.3"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fda4ed1c6c173e3fc7a83629421152e01d7b1f9b7f65fb301e490e8cfc656422"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.3"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4359fd9c9171ec6e8c62926d6faaf553a8dc3f64e1507e76da7911b4f6a04405"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
@@ -2271,17 +2309,17 @@
  "futures",
  "rustversion",
  "thiserror",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
@@ -2304,14 +2342,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
@@ -2345,17 +2395,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.67"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prokio"
 version = "0.1.0"
@@ -2370,79 +2420,91 @@
  "pinned",
  "tokio",
  "tokio-stream",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.8.0",
+ "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radix_trie"
 version = "0.2.1"
@@ -2481,85 +2543,83 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.7.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
+checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.11.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
- "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
- "num_cpus",
 ]
 
 [[package]]
 name = "recursive-for"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.5"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697061221ea1b4a94a624f67d0ae2bfe4e22b8a17b6a192afb11046542cc8c47"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.3.8",
+ "regex-automata 0.4.6",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-automata"
-version = "0.3.8"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2f401f4955220693b56f8ec66ee9c78abffd8d1c4f23dc41a23839eb88f0795"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "render-macro"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
@@ -2577,14 +2637,20 @@
 name = "render-value"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
+name = "roff"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b833d8d034ea094b1ea68aa6d5c740e0d04bad9d16568d08ba6f76823a114316"
+
+[[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc_version"
@@ -2593,38 +2659,38 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.13"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7db8590df6dfcd144d22afd1b83b36c21a18d7cbc1dc4bb5295a8712e9eb662"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "rustyline"
 version = "12.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "994eca4bca05c87e86e15d90fc7a91d1be64b4482b38cb2d27474568fe7c9db9"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "cfg-if",
  "clipboard-win",
  "fd-lock",
  "home",
  "libc",
  "log",
  "memchr",
@@ -2635,17 +2701,17 @@
  "unicode-width",
  "utf8parse",
  "winapi",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -2663,29 +2729,29 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "self_cell"
-version = "1.0.1"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c309e515543e67811222dbc9e3dd7e1056279b782e1dacffe4242b718734fb6"
+checksum = "58bf37232d3bb9a2c4e641ca2a11d83b5062066f88df7fed36c28772046d65ba"
 
 [[package]]
 name = "semver"
-version = "1.0.18"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.5.0"
@@ -2707,28 +2773,28 @@
  "serde",
  "thiserror",
  "xml-rs",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2751,17 +2817,17 @@
  "percent-encoding",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.3"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
+checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -2772,41 +2838,41 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.25"
+version = "0.9.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a49e178e4452f45cb61d0cd8cebc1b0fafd3e41929e996cef79aa3aca91f574"
+checksum = "a0623d197252096520c6f2a5e1171ee436e5af99a5d7caa2891e55e61950e6d9"
 dependencies = [
- "indexmap 2.0.0",
+ "indexmap 2.2.5",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "sha1"
-version = "0.10.5"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
+checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.7"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -2816,17 +2882,17 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "similar"
-version = "2.2.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "420acb44afdae038210c99e69aae24109f32f15500aa708e81d46c9f29d55fcf"
+checksum = "32fea41aca09ee824cc9724996433064c89f7777e60762749a4170a14abbfa21"
 dependencies = [
  "bstr 0.2.17",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "similar-asserts"
@@ -2851,43 +2917,49 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "slug"
-version = "0.1.4"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3bc762e6a4b6c6fcaade73e77f9ebc6991b676f88bb2358bddb56560f073373"
+checksum = "3bd94acec9c8da640005f8e135a39fc0372e74535e6b368b7a04b875f784c8c4"
 dependencies = [
  "deunicode",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.4"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4031e820eb552adee9295814c0ced9e5cf38ddf1e8b7d566d6de8e2538ea989e"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "stack-ref"
-version = "0.1.0"
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
 dependencies = [
- "minijinja",
- "minijinja-stack-ref",
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -2895,124 +2967,130 @@
 [[package]]
 name = "str-buf"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e08d8363704e6c71fc928674353e6b7c23dcea9d82d7012c8faf2a3a025f8d0"
 
 [[package]]
+name = "streaming"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.36"
+version = "2.0.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91e02e55d62894af2a08aca894c6577281f76769ba47c94d5756bec8ac6e7373"
+checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+
+[[package]]
+name = "tempfile"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
+dependencies = [
+ "cfg-if",
+ "fastrand",
+ "rustix",
+ "windows-sys 0.52.0",
+]
 
 [[package]]
 name = "tera"
 version = "1.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "970dff17c11e884a4a09bc76e3a17ef71e01bb13447a11e85226e254fe6d10b8"
 dependencies = [
  "chrono",
  "chrono-tz",
  "globwalk",
- "humansize 2.1.3",
+ "humansize",
  "lazy_static",
  "percent-encoding",
  "pest",
  "pest_derive",
  "rand",
  "regex",
  "serde",
  "serde_json",
  "slug",
  "unic-segment",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
-
-[[package]]
 name = "thiserror"
-version = "1.0.48"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d6d7a740b8a666a7e828dd00da9c0dc290dff53154ea77ac109281de90589b7"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.48"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49922ecae66cc8a249b77e68d1d0623c1b2c514f0060c27cdc68bd62a1219d35"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
-]
-
-[[package]]
-name = "thread_local"
-version = "1.1.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
-dependencies = [
- "cfg-if",
- "once_cell",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.28"
+version = "0.3.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6bb557fd245c28e6411aa56b6403c689ad95061f50e4be16c274e70a17e48"
+checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
 dependencies = [
  "deranged",
  "itoa",
+ "num-conv",
+ "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.14"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a942f44339478ef67935ab2bbaec2fb0322496cf3cbe84b261e06ac3814c572"
+checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "time-tz"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3050,126 +3128,116 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.32.0"
+version = "1.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ed6077ed6cd6c74735e21f37eb16dc3935f96878b1fe961074089cc80893f9"
+checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.14"
+version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
+checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.8"
+version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
+checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.5.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
-dependencies = [
- "serde",
-]
-
-[[package]]
-name = "toml"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd79e69d3b627db300ff956027cc6c3798cef26d22526befdfcd12feeb6d2257"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.3"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
- "indexmap 2.0.0",
+ "indexmap 2.2.5",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
@@ -3179,14 +3247,21 @@
 [[package]]
 name = "ucd-trie"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
 
 [[package]]
+name = "undefined-tracking"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+]
+
+[[package]]
 name = "unic-char-property"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8c57a407d9b6fa02b4795eb81c5b6652060a15a7903ea981f3d723e6c0be221"
 dependencies = [
  "unic-char-range",
 ]
@@ -3239,62 +3314,62 @@
 checksum = "f7d2d4dafb69621809a81864c9c1b864479e1235c0dd4e199924b9742439ed89"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.9"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f28467d3e1d3c6586d8f25fa243f544f5800fec42d97032474e17222c2b75cfa"
+checksum = "673aac59facbab8a9007c7f6108d11f63b603f7cabff99fabf650fea5c32b861"
 
 [[package]]
 name = "url"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "143b538f18257fac9cad154828a57c6bf5157e1aa604d4816b5995bf6de87ae5"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -3320,109 +3395,109 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.37"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.36",
+ "syn 2.0.53",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-yew"
 version = "0.1.0"
 dependencies = [
  "minijinja",
  "serde_json",
  "web-sys",
  "yew",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -3438,34 +3513,34 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows"
-version = "0.48.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.48.5",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
@@ -3479,14 +3554,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -3509,120 +3593,168 @@
  "windows_i686_msvc 0.48.5",
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
+]
+
+[[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
 name = "winnow"
-version = "0.5.15"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c2e3184b9c4e92ad5167ca73039d0c42476302ab603e2fec4487511f38ccefc"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xml-rs"
-version = "0.8.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab77e97b50aee93da431f2cee7cd0f43b4d1da3c408042f2d7d164187774f0a"
-
-[[package]]
-name = "yaml-rust"
-version = "0.4.5"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
-dependencies = [
- "linked-hash-map",
-]
+checksum = "0fcb9cbac069e033553e8bb871be2fbdffcab578eb25bd0f7c508cedc6dcd75a"
 
 [[package]]
 name = "yew"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dbecfe44343b70cc2932c3eb445425969ae21754a8ab3a0966981c1cf7af1cc"
 dependencies = [
@@ -3657,35 +3789,53 @@
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "zerocopy"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.53",
+]
+
+[[package]]
 name = "zstd"
-version = "0.12.4"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
+checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.6"
+version = "7.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
+checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
 dependencies = [
- "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.8+zstd.1.5.5"
+version = "2.0.9+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
+checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
 dependencies = [
  "cc",
- "libc",
  "pkg-config",
 ]
```

### Comparing `minijinja-1.0.8/PKG-INFO` & `minijinja-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijinja
-Version: 1.0.8
+Version: 2.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -71,20 +71,20 @@
 ```python
 result = env.render_template('template_name', var1="value 1", var2="value 2")
 print(result)
 ```
 
 ## Purpose
 
-MiniJinja attempts a certain level of compatibility with Jinja2, but it does not
-try to achieve this at all costs.  As a result you will notice that quite a few
-templates will refuse to render with MiniJinja despite the fact that they probably
-look quite innocent.  It is however possible to write templates that render to the
-same results for both Jinja2 and MiniJinja.  This raises the question why you might
-want to use MiniJinja.
+MiniJinja attempts a reasonably high level of compatibility with Jinja2, but it
+does not try to achieve this at all costs.  As a result you will notice that
+quite a few templates will refuse to render with MiniJinja despite the fact that
+they probably look quite innocent.  It is however possible to write templates
+that render to the same results for both Jinja2 and MiniJinja.  This raises the
+question why you might want to use MiniJinja.
 
 The main benefit would be to achieve the exact same results in both Rust and Python.
 Additionally MiniJinja has a stronger sandbox than Jinja2 and might perform ever so
 slightly better in some situations.  However you should be aware that due to the
 marshalling that needs to happen in either direction there is a certain amount of
 loss of information.
 
@@ -163,37 +163,41 @@
     return state.lookup("a_variable") + value
 
 env.add_filter("add_a_variable", my_filter)
 ```
 
 ## Runtime Behavior
 
-MiniJinja uses it's own runtime model which is not matching the Python
-runtime model.  As a result there are clear gaps in beahvior between the
-two and only limited effort is made to bridge them.  For instance you will
-be able to call some methods of types, but for instance builtins such as
-dicts and lists do not expose their methods on the MiniJinja side.  This
-means that it's very intentional that if you pass a dictionary to MiniJinja,
-the Python `.items()` method is unavailable.
+MiniJinja uses it's own runtime model which is not matching the Python runtime
+model.  As a result there are gaps in behavior between the two but some
+limited effort is made to bridge them.  For instance you will be able to call
+some methods of types, but for instance builtins such as dicts and lists do not
+expose their methods on the MiniJinja side in all cases.  A natively generated
+MiniJinja map (such as with the `dict` global function) will not have an `.items()`
+method, whereas a Python dict passed to MiniJinja will.
 
 Here is what this means for some basic types:
 
 * Python dictionaries and lists (as well as other objects that behave as sequences)
-  appear in the MiniJinja side as native lists.  They do not expose any specific
-  other behavior and when they move back to the Python side they will appear as basic
-  lists.  Specifically this means that a tuple (which does not exist in MiniJinja)
-  when moving from Python to MiniJinja turns into a list and will remain a list when
-  it moves back.
+  appear in the MiniJinja side very similar to how they do in Python.
+* Tuples on the MiniJinja side are represented as lists, but will appear again as
+  tuples if passed back to Python.
 * Python objects are represented in MiniJinja similarly to dicts, but they retain all
   their meaningful Python APIs.  This means they stringify via `__str__` and they
   allow the MiniJinja code to call their non-underscored methods.  Note that there is
   no extra security layer in use at the moment so take care of what you pass there.
 * MiniJinja's python binding understand what `__html__` is when it exists on a string
   subclass.  This means that a `markupsafe.Markup` object will appear as safe string in
   MiniJinja.  This information can also flow back to Python again.
+* Stringification of objects uses `__str__` which is why mixed Python and MiniJinja
+  objects can be a bit confusing at times.
+* Where in Jinja2 there is a difference between `foo["bar"]` and `foo.bar` which can
+  be used to disambiugate properties and keys, in MiniJinja there is no such difference.
+  However methods are disambiugated so `foo.items()` works and will correctly call
+  the method in all cases.
 
 ## Sponsor
 
 If you like the project and find it useful you can [become a
 sponsor](https://github.com/sponsors/mitsuhiko).
 
 ## License and Links
```

