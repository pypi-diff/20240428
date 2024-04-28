# Comparing `tmp/traderusty-0.1.2.tar.gz` & `tmp/traderusty-0.1.3.tar.gz`

## Comparing `traderusty-0.1.2.tar` & `traderusty-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 traderusty-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127     3000 2024-04-25 03:23:55.000000 traderusty-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-25 03:23:55.000000 traderusty-0.1.2/.gitignore
--rw-r--r--   0     1001      127      171 2024-04-25 03:23:55.000000 traderusty-0.1.2/CHANGELOG.md
--rw-r--r--   0     1001      127     2282 2024-04-25 03:23:55.000000 traderusty-0.1.2/Dockerfile
--rw-r--r--   0     1001      127     1065 2024-04-25 03:23:55.000000 traderusty-0.1.2/LICENSE.txt
--rw-r--r--   0     1001      127      174 2024-04-25 03:23:55.000000 traderusty-0.1.2/README.md
--rw-r--r--   0     1001      127      109 2024-04-25 03:23:55.000000 traderusty-0.1.2/python/tests/test_all.py
--rw-r--r--   0     1001      127      125 2024-04-25 03:23:55.000000 traderusty-0.1.2/python/traderusty/__init__.py
--rw-r--r--   0     1001      127       64 2024-04-25 03:23:55.000000 traderusty-0.1.2/python/traderusty/traderusty.pyi
--rw-r--r--   0     1001      127      505 2024-04-25 03:23:55.000000 traderusty-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     2659 2024-04-25 03:23:55.000000 traderusty-0.1.2/src/rusty.rs
--rw-r--r--   0     1001      127    65336 2024-04-25 03:23:58.000000 traderusty-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127     1438 2024-04-25 03:23:55.000000 traderusty-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 traderusty-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 traderusty-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     2935 2024-04-27 02:26:31.000000 traderusty-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-27 02:26:31.000000 traderusty-0.1.3/.gitignore
+-rw-r--r--   0     1001      127      264 2024-04-27 02:26:31.000000 traderusty-0.1.3/CHANGELOG.md
+-rw-r--r--   0     1001      127     2282 2024-04-27 02:26:31.000000 traderusty-0.1.3/Dockerfile
+-rw-r--r--   0     1001      127     1065 2024-04-27 02:26:31.000000 traderusty-0.1.3/LICENSE.txt
+-rw-r--r--   0     1001      127      174 2024-04-27 02:26:31.000000 traderusty-0.1.3/README.md
+-rw-r--r--   0     1001      127      109 2024-04-27 02:26:31.000000 traderusty-0.1.3/python/tests/test_all.py
+-rw-r--r--   0     1001      127      125 2024-04-27 02:26:31.000000 traderusty-0.1.3/python/traderusty/__init__.py
+-rw-r--r--   0     1001      127       64 2024-04-27 02:26:31.000000 traderusty-0.1.3/python/traderusty/traderusty.pyi
+-rw-r--r--   0     1001      127      838 2024-04-27 02:26:31.000000 traderusty-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     6725 2024-04-27 02:26:31.000000 traderusty-0.1.3/src/rusty.rs
+-rw-r--r--   0     1001      127    65584 2024-04-27 02:26:31.000000 traderusty-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127     1438 2024-04-27 02:26:31.000000 traderusty-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 traderusty-0.1.3/PKG-INFO
```

### Comparing `traderusty-0.1.2/Cargo.toml` & `traderusty-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "traderusty"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 
 [features]
 default = ["runtime-dispatch-simd"]
 runtime-dispatch-simd = ["bytecount/runtime-dispatch-simd"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `traderusty-0.1.2/.github/workflows/CI.yml` & `traderusty-0.1.3/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -66,32 +66,31 @@
           name: wheels-windows-${{ matrix.target }}
           path: dist
 
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
-        target: [x64]
         pyver:  ['3.9']
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.pyver }}
-          architecture: ${{ matrix.target }}
+          architecture: arm64
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
-          target: ${{ matrix.target }}
+          target: aarch64
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
-          name: wheels-macos-${{ matrix.target }}
+          name: wheels-macos-arm64
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
```

### Comparing `traderusty-0.1.2/.gitignore` & `traderusty-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.2/Dockerfile` & `traderusty-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.2/LICENSE.txt` & `traderusty-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.2/Cargo.lock` & `traderusty-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -660,23 +660,23 @@
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -927,17 +927,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1184,33 +1184,33 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
@@ -1490,14 +1490,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
@@ -2082,15 +2091,15 @@
  "tracing-core",
  "tracing-log",
  "tracing-serde",
 ]
 
 [[package]]
 name = "traderusty"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "bytecount",
  "maturin",
  "pyo3",
  "tempfile",
 ]
 
@@ -2145,17 +2154,17 @@
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
@@ -2175,19 +2184,19 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.21.7",
+ "base64 0.22.0",
  "flate2",
  "log",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
  "serde",
@@ -2322,17 +2331,17 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.7"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "134306a13c5647ad6453e8deaec55d3a44d6021970129e6188735e74bf546697"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
@@ -2476,17 +2485,17 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.6"
+version = "0.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winsafe"
 version = "0.0.19"
@@ -2557,17 +2566,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.8.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63381fa6624bf92130a6b87c0d07380116f80b565c42cf0d754136f0238359ef"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 
 [[package]]
 name = "zip"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
```

### Comparing `traderusty-0.1.2/pyproject.toml` & `traderusty-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `traderusty-0.1.2/PKG-INFO` & `traderusty-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: traderusty
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

