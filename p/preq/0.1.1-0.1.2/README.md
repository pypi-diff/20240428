# Comparing `tmp/preq-0.1.1.tar.gz` & `tmp/preq-0.1.2.tar.gz`

## Comparing `preq-0.1.1.tar` & `preq-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 preq-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000     3106 2024-04-14 18:23:40.000000 preq-0.1.1/.gitignore
--rw-r--r--   0     1000     1000    20262 2024-04-22 01:07:12.000000 preq-0.1.1/Cargo.lock
--rw-r--r--   0     1000     1000        0 2024-04-20 22:49:41.000000 preq-0.1.1/Config.toml
--rw-r--r--   0     1000     1000      101 2024-04-14 18:02:15.000000 preq-0.1.1/README.md
--rw-r--r--   0     1000     1000     2505 2024-04-14 19:55:31.000000 preq-0.1.1/assets/stdlib
--rw-r--r--   0     1000     1000     1688 2024-04-22 01:07:51.000000 preq-0.1.1/src/cli.rs
--rw-r--r--   0     1000     1000      681 2024-04-20 22:54:39.000000 preq-0.1.1/src/config.rs
--rw-r--r--   0     1000     1000      964 2024-04-22 00:47:58.000000 preq-0.1.1/src/input.rs
--rw-r--r--   0     1000     1000      534 2024-04-22 01:07:49.000000 preq-0.1.1/src/main.rs
--rw-r--r--   0     1000     1000      973 2024-04-21 23:41:48.000000 preq-0.1.1/src/map.rs
--rw-r--r--   0     1000     1000     1397 2024-04-22 00:42:01.000000 preq-0.1.1/src/parse.rs
--rw-r--r--   0     1000     1000      564 2024-04-21 23:08:11.000000 preq-0.1.1/src/utils/fallback.rs
--rw-r--r--   0     1000     1000       31 2024-04-21 23:09:02.000000 preq-0.1.1/src/utils/mod.rs
--rw-r--r--   0     1000     1000     3078 2024-04-21 23:26:20.000000 preq-0.1.1/src/utils/pyfuncs.rs
--rw-r--r--   0     1000     1000      458 2024-04-21 23:49:17.000000 preq-0.1.1/src/write.rs
--rw-r--r--   0     1000     1000    20572 2024-04-14 18:43:49.000000 preq-0.1.1/tests/pipreqs
--rw-r--r--   0     1000     1000      444 2024-04-22 01:09:57.000000 preq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 preq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 preq-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000     3106 2024-04-14 18:23:40.000000 preq-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000    20271 2024-04-28 21:13:26.000000 preq-0.1.2/Cargo.lock
+-rw-r--r--   0     1000     1000        0 2024-04-20 22:49:41.000000 preq-0.1.2/Config.toml
+-rw-r--r--   0     1000     1000      101 2024-04-14 18:02:15.000000 preq-0.1.2/README.md
+-rw-r--r--   0     1000     1000     2505 2024-04-14 19:55:31.000000 preq-0.1.2/assets/stdlib
+-rw-r--r--   0     1000     1000     2122 2024-04-28 19:28:13.000000 preq-0.1.2/src/cli.rs
+-rw-r--r--   0     1000     1000      681 2024-04-20 22:54:39.000000 preq-0.1.2/src/config.rs
+-rw-r--r--   0     1000     1000      973 2024-04-21 23:41:48.000000 preq-0.1.2/src/imports/mapper.rs
+-rw-r--r--   0     1000     1000       44 2024-04-28 19:17:14.000000 preq-0.1.2/src/imports/mod.rs
+-rw-r--r--   0     1000     1000     1397 2024-04-22 00:42:01.000000 preq-0.1.2/src/imports/parser.rs
+-rw-r--r--   0     1000     1000     2669 2024-04-28 21:08:34.000000 preq-0.1.2/src/imports/reader.rs
+-rw-r--r--   0     1000     1000        0 2024-04-28 19:19:49.000000 preq-0.1.2/src/imports/tests.rs
+-rw-r--r--   0     1000     1000      561 2024-04-28 21:11:28.000000 preq-0.1.2/src/main.rs
+-rw-r--r--   0     1000     1000        0 2024-04-28 18:39:15.000000 preq-0.1.2/src/pypi.rs
+-rw-r--r--   0     1000     1000      564 2024-04-21 23:08:11.000000 preq-0.1.2/src/utils/fallback.rs
+-rw-r--r--   0     1000     1000       31 2024-04-21 23:09:02.000000 preq-0.1.2/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     3078 2024-04-21 23:26:20.000000 preq-0.1.2/src/utils/pyfuncs.rs
+-rw-r--r--   0     1000     1000     1963 2024-04-28 21:00:55.000000 preq-0.1.2/src/writer.rs
+-rw-r--r--   0     1000     1000    20572 2024-04-14 18:43:49.000000 preq-0.1.2/tests/pipreqs
+-rw-r--r--   0     1000     1000      454 2024-04-28 21:13:42.000000 preq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 preq-0.1.2/PKG-INFO
```

### Comparing `preq-0.1.1/.gitignore` & `preq-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/Cargo.lock` & `preq-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -416,22 +416,23 @@
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
 name = "preq"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "clap",
  "config",
  "lazy_static",
  "regex",
  "serde",
  "serde_json",
+ "toml",
  "workdir",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `preq-0.1.1/assets/stdlib` & `preq-0.1.2/assets/stdlib`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/src/cli.rs` & `preq-0.1.2/src/cli.rs`

 * *Files 9% similar despite different names*

```diff
@@ -8,44 +8,56 @@
     author = "atbraz",
     about = "Generates requirements.txt for Python projects.",
     long_about = "Generates requirements.txt for Python projects by parsing imports from Python files and checking for their package names and versions in your venv."
 )]
 pub struct Args {
     #[clap(
         value_name = "PATH",
+        default_value = ".",
         help = "Input path, can be a file or a directory",
         long_help = "Input path, can be a file or a directory. If a directory is provided, all Python files in the directory will be parsed for imports.",
         required = true,
         value_parser = clap::value_parser!(PathBuf)
     )]
     pub path: PathBuf,
 
     #[clap(
         value_name = "OUTPUT",
-        default_value = "requirements.txt",
-        short,
-        long,
+        default_value = "./requirements.txt",
+        short = 'o',
+        long = "output",
         help = "Output file to use",
         long_help = "Output file to use. If not provided, will write to requirements.txt in the current directory. If set to 'pyproject.toml', will write to project.dependencies (must be in current directory).",
         value_parser = clap::value_parser!(PathBuf)
     )]
-    pub output: Option<PathBuf>,
+    pub output: PathBuf,
+
+    #[clap(
+        value_name = "TREE",
+        default_value = "false",
+        short = 't',
+        long = "tree",
+        help = "Output a tree of dependencies",
+        long_help = "Output a tree of dependencies. If set to 'true', will output a tree of dependencies to the output file.",
+        action = ArgAction::SetTrue,
+    )]
+    pub tree: bool,
 
     #[clap(
         value_name = "DRY_RUN",
-        short,
+        default_value = "false",
         long,
         help = "Dry run, do not write to file",
         long_help = "Simulates what would be written to the output file should in a regular call.",
         action = ArgAction::SetTrue,
     )]
     pub dry_run: bool,
 
     #[clap(
         value_name = "VERBOSE",
-        short,
-        long,
+        short = 'v',
+        long = "verbose",
         help = "Verbose mode",
         action = ArgAction::SetTrue,
     )]
     pub verbose: bool,
 }
```

### Comparing `preq-0.1.1/src/config.rs` & `preq-0.1.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/src/map.rs` & `preq-0.1.2/src/imports/mapper.rs`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/src/parse.rs` & `preq-0.1.2/src/imports/parser.rs`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/src/utils/fallback.rs` & `preq-0.1.2/src/utils/fallback.rs`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/src/utils/pyfuncs.rs` & `preq-0.1.2/src/utils/pyfuncs.rs`

 * *Files identical despite different names*

### Comparing `preq-0.1.1/tests/pipreqs` & `preq-0.1.2/tests/pipreqs`

 * *Files identical despite different names*

