# Comparing `tmp/bihyung-0.1.3.tar.gz` & `tmp/bihyung-0.2.0.tar.gz`

## Comparing `bihyung-0.1.3.tar` & `bihyung-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,7 @@
--rw-r--r--   0     1001      127      966 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/Cargo.toml
--rw-r--r--   0     1001      127      220 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/README.md
--rw-r--r--   0     1001      127     2984 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/benches/port_open.rs
--rw-r--r--   0     1001      127      352 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/examples/langchain_llama.rs
--rw-r--r--   0     1001      127     1023 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/daemon_trait.rs
--rw-r--r--   0     1001      127      429 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/lib.rs
--rw-r--r--   0     1001      127     7532 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/llama_daemon/daemon2.rs
--rw-r--r--   0     1001      127     1102 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/llama_daemon/mod.rs
--rw-r--r--   0     1001      127      950 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/mlc_daemon/bootstrap.rs
--rw-r--r--   0     1001      127    10694 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/mlc_daemon/daemon2.rs
--rw-r--r--   0     1001      127       96 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/mlc_daemon/mod.rs
--rw-r--r--   0     1001      127     8476 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/proxy.rs
--rw-r--r--   0     1001      127     3934 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/src/test_client.rs
--rw-r--r--   0     1001      127       62 2024-04-27 18:28:12.000000 bihyung-0.1.3/llm-daemon/tests/simple_test.rs
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 bihyung-0.1.3/bihyung/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-04-27 18:28:12.000000 bihyung-0.1.3/bihyung/.gitignore
--rw-r--r--   0     1001      127     4056 2024-04-27 18:28:12.000000 bihyung-0.1.3/bihyung/src/lib.rs
--rw-r--r--   0     1001      127   101767 2024-04-27 18:28:12.000000 bihyung-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 bihyung-0.1.3/Cargo.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.0/bihyung/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-04-28 01:47:01.000000 bihyung-0.2.0/bihyung/.gitignore
+-rw-r--r--   0     1001      127     4056 2024-04-28 01:47:01.000000 bihyung-0.2.0/bihyung/src/lib.rs
+-rw-r--r--   0     1001      127   102229 2024-04-28 01:47:12.000000 bihyung-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.0/Cargo.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.0/PKG-INFO
```

### Comparing `bihyung-0.1.3/bihyung/.gitignore` & `bihyung-0.2.0/bihyung/.gitignore`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.3/bihyung/src/lib.rs` & `bihyung-0.2.0/bihyung/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.1.3/Cargo.lock` & `bihyung-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -278,18 +278,18 @@
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bihyung"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "enum_dispatch",
- "llm-daemon",
+ "llm-daemon 0.2.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "url",
 ]
@@ -1661,15 +1661,15 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "llm-daemon"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "axum",
  "criterion",
  "daemonize",
  "futures",
@@ -1684,14 +1684,36 @@
  "tracing",
  "tracing-subscriber",
  "tracing-test",
  "url",
 ]
 
 [[package]]
+name = "llm-daemon"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "929c88315de03d76a11f848ef6a5794fcd72f305e5c14015c0551ac35ce0a190"
+dependencies = [
+ "anyhow",
+ "axum",
+ "daemonize",
+ "futures",
+ "hyper 1.3.1",
+ "hyper-util",
+ "reqwest 0.12.4",
+ "serde",
+ "serde_json",
+ "tempfile",
+ "tokio",
+ "tracing",
+ "tracing-subscriber",
+ "url",
+]
+
+[[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
```

