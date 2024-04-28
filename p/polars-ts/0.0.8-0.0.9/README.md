# Comparing `tmp/polars_ts-0.0.8.tar.gz` & `tmp/polars_ts-0.0.9.tar.gz`

## Comparing `polars_ts-0.0.8.tar` & `polars_ts-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,74 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.8/Cargo.toml
--rw-r--r--   0     1001      127     3402 2024-04-19 09:23:23.000000 polars_ts-0.0.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127     3107 2024-04-19 09:23:23.000000 polars_ts-0.0.8/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-19 09:23:23.000000 polars_ts-0.0.8/.python-version
--rw-r--r--   0     1001      127      147 2024-04-19 09:23:23.000000 polars_ts-0.0.8/.vscode/settings.json
--rw-r--r--   0     1001      127    11357 2024-04-19 09:23:23.000000 polars_ts-0.0.8/LICENSE
--rw-r--r--   0     1001      127      704 2024-04-19 09:23:23.000000 polars_ts-0.0.8/Makefile
--rw-r--r--   0     1001      127     1002 2024-04-19 09:23:23.000000 polars_ts-0.0.8/README.md
--rw-r--r--   0     1001      127      950 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/__init__.py
--rw-r--r--   0     1001      127     1637 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/calendar.py
--rw-r--r--   0     1001      127     2537 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/calendar_helper/__init__.py
--rw-r--r--   0     1001      127      673 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/display.py
--rw-r--r--   0     1001      127     2567 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/dummy.py
--rw-r--r--   0     1001      127     2851 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/dummy_helper/__init__.py
--rw-r--r--   0     1001      127     1178 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/dummymkt.py
--rw-r--r--   0     1001      127     1642 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/dummymkt_helper/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/expr/__init__.py
--rw-r--r--   0     1001      127     1580 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/expr/random.py
--rw-r--r--   0     1001      127     1213 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures.py
--rw-r--r--   0     1001      127     2307 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures_helper/__init__.py
--rw-r--r--   0     1001      127      850 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures_helper/bbg_symbols.py
--rw-r--r--   0     1001      127     1135 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures_helper/generic_symbols.py
--rw-r--r--   0     1001      127     7751 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures_helper/roll_calendar.py
--rw-r--r--   0     1001      127      890 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/futures_helper/util.py
--rw-r--r--   0     1001      127     5703 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/grouper.py
--rw-r--r--   0     1001      127      507 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/io.py
--rw-r--r--   0     1001      127     1084 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/io_helper/__init__.py
--rw-r--r--   0     1001      127     1669 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/mathx.py
--rw-r--r--   0     1001      127     1876 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/mathx_helper/__init__.py
--rw-r--r--   0     1001      127     2446 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/resample.py
--rw-r--r--   0     1001      127     2975 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/resample_helper/__init__.py
--rw-r--r--   0     1001      127      947 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/sf.py
--rw-r--r--   0     1001      127     2018 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/sf_helper/__init__.py
--rw-r--r--   0     1001      127      684 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/time.py
--rw-r--r--   0     1001      127      937 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/time_helper/__init__.py
--rw-r--r--   0     1001      127      397 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/tsf.py
--rw-r--r--   0     1001      127      536 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/types.py
--rw-r--r--   0     1001      127     1289 2024-04-19 09:23:23.000000 polars_ts-0.0.8/polars_ts/utils.py
--rw-r--r--   0     1001      127       32 2024-04-19 09:23:23.000000 polars_ts-0.0.8/requirements.txt
--rw-r--r--   0     1001      127      445 2024-04-19 09:23:23.000000 polars_ts-0.0.8/ruff.toml
--rw-r--r--   0     1001      127      212 2024-04-19 09:23:23.000000 polars_ts-0.0.8/run.py
--rw-r--r--   0     1001      127     2617 2024-04-19 09:23:23.000000 polars_ts-0.0.8/src/expressions.rs
--rw-r--r--   0     1001      127      382 2024-04-19 09:23:23.000000 polars_ts-0.0.8/src/lib.rs
--rw-r--r--   0     1001      127     1839 2024-04-19 09:23:23.000000 polars_ts-0.0.8/src/math/mod.rs
--rw-r--r--   0     1001      127     2712 2024-04-19 09:23:23.000000 polars_ts-0.0.8/src/utils.rs
--rw-r--r--   0     1001      127      212 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/00_config/roll_config.csv
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/__init__.py
--rw-r--r--   0     1001      127      146 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/config.py
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/futures/__init__.py
--rw-r--r--   0     1001      127     2148 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/futures/test_continuous_contract.py
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/grouper/__init__.py
--rw-r--r--   0     1001      127     2779 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/grouper/test_grouper.py
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/mathx/__init__.py
--rw-r--r--   0     1001      127    11052 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/mathx/test_cum_sum.py
--rw-r--r--   0     1001      127    13921 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/mathx/test_diff.py
--rw-r--r--   0     1001      127     3234 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/mathx/test_ewm_mean.py
--rw-r--r--   0     1001      127    11395 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/mathx/test_shift.py
--rw-r--r--   0     1001      127        0 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/resample/__init__.py
--rw-r--r--   0     1001      127    29539 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/resample/test_resample.py
--rw-r--r--   0     1001      127     1248 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/sf/test_join.py
--rw-r--r--   0     1001      127     1080 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/sf/test_sf.py
--rw-r--r--   0     1001      127      846 2024-04-19 09:23:23.000000 polars_ts-0.0.8/tests/test_rust_templates.py
--rw-r--r--   0     1001      127    36490 2024-04-19 09:23:23.000000 polars_ts-0.0.8/Cargo.lock
--rw-r--r--   0     1001      127      478 2024-04-19 09:23:23.000000 polars_ts-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 polars_ts-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      127     3402 2024-04-22 19:42:39.000000 polars_ts-0.0.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127     3107 2024-04-22 19:42:39.000000 polars_ts-0.0.9/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-22 19:42:39.000000 polars_ts-0.0.9/.python-version
+-rw-r--r--   0     1001      127      915 2024-04-22 19:42:39.000000 polars_ts-0.0.9/.vscode/launch.json
+-rw-r--r--   0     1001      127      147 2024-04-22 19:42:39.000000 polars_ts-0.0.9/.vscode/settings.json
+-rw-r--r--   0     1001      127    11357 2024-04-22 19:42:39.000000 polars_ts-0.0.9/LICENSE
+-rw-r--r--   0     1001      127      704 2024-04-22 19:42:39.000000 polars_ts-0.0.9/Makefile
+-rw-r--r--   0     1001      127     1002 2024-04-22 19:42:39.000000 polars_ts-0.0.9/README.md
+-rw-r--r--   0     1001      127      988 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/__init__.py
+-rw-r--r--   0     1001      127     1637 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/calendar.py
+-rw-r--r--   0     1001      127     2537 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/calendar_helper/__init__.py
+-rw-r--r--   0     1001      127      673 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/display.py
+-rw-r--r--   0     1001      127     2567 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/dummy.py
+-rw-r--r--   0     1001      127     2851 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/dummy_helper/__init__.py
+-rw-r--r--   0     1001      127     1178 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/dummymkt.py
+-rw-r--r--   0     1001      127     1642 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/dummymkt_helper/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/expr/__init__.py
+-rw-r--r--   0     1001      127     1580 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/expr/random.py
+-rw-r--r--   0     1001      127      793 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/expr/time.py
+-rw-r--r--   0     1001      127     1213 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures.py
+-rw-r--r--   0     1001      127     2307 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures_helper/__init__.py
+-rw-r--r--   0     1001      127      850 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures_helper/bbg_symbols.py
+-rw-r--r--   0     1001      127     1135 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures_helper/generic_symbols.py
+-rw-r--r--   0     1001      127     7751 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures_helper/roll_calendar.py
+-rw-r--r--   0     1001      127      890 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/futures_helper/util.py
+-rw-r--r--   0     1001      127     5703 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/grouper.py
+-rw-r--r--   0     1001      127      507 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/io.py
+-rw-r--r--   0     1001      127     1084 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/io_helper/__init__.py
+-rw-r--r--   0     1001      127     1615 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/mathx.py
+-rw-r--r--   0     1001      127     1786 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/mathx_helper/__init__.py
+-rw-r--r--   0     1001      127     2403 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/resample.py
+-rw-r--r--   0     1001      127     2901 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/resample_helper/__init__.py
+-rw-r--r--   0     1001      127     2033 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/sf.py
+-rw-r--r--   0     1001      127     3793 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/sf_helper/__init__.py
+-rw-r--r--   0     1001      127     1387 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/time.py
+-rw-r--r--   0     1001      127     1328 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/time_helper/__init__.py
+-rw-r--r--   0     1001      127      397 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/tsf.py
+-rw-r--r--   0     1001      127      528 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/types.py
+-rw-r--r--   0     1001      127     1289 2024-04-22 19:42:39.000000 polars_ts-0.0.9/polars_ts/utils.py
+-rw-r--r--   0     1001      127       32 2024-04-22 19:42:39.000000 polars_ts-0.0.9/requirements.txt
+-rw-r--r--   0     1001      127      445 2024-04-22 19:42:39.000000 polars_ts-0.0.9/ruff.toml
+-rw-r--r--   0     1001      127      212 2024-04-22 19:42:39.000000 polars_ts-0.0.9/run.py
+-rw-r--r--   0     1001      127     6779 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/expressions.rs
+-rw-r--r--   0     1001      127      392 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      127     1839 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/math/mod.rs
+-rw-r--r--   0     1001      127     1176 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/time/mod.rs
+-rw-r--r--   0     1001      127     4555 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/time/utils.rs
+-rw-r--r--   0     1001      127     2712 2024-04-22 19:42:39.000000 polars_ts-0.0.9/src/utils.rs
+-rw-r--r--   0     1001      127      212 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/00_config/roll_config.csv
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/__init__.py
+-rw-r--r--   0     1001      127      146 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/config.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/futures/__init__.py
+-rw-r--r--   0     1001      127     2109 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/futures/test_continuous_contract.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/grouper/__init__.py
+-rw-r--r--   0     1001      127     2779 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/grouper/test_grouper.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/mathx/__init__.py
+-rw-r--r--   0     1001      127    11052 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/mathx/test_cum_sum.py
+-rw-r--r--   0     1001      127    13921 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/mathx/test_diff.py
+-rw-r--r--   0     1001      127     3234 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/mathx/test_ewm_mean.py
+-rw-r--r--   0     1001      127    11395 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/mathx/test_shift.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/resample/__init__.py
+-rw-r--r--   0     1001      127    29539 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/resample/test_resample.py
+-rw-r--r--   0     1001      127     1248 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/sf/test_join.py
+-rw-r--r--   0     1001      127     7855 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/sf/test_join_on_list_items.py
+-rw-r--r--   0     1001      127     1080 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/sf/test_sf.py
+-rw-r--r--   0     1001      127      846 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/test_rust_templates.py
+-rw-r--r--   0     1001      127        0 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/time/__init__.py
+-rw-r--r--   0     1001      127     7779 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tests/time/test_basic.py
+-rw-r--r--   0     1001      127     3163 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tools/launch.py
+-rw-r--r--   0     1001      127     2283 2024-04-22 19:42:39.000000 polars_ts-0.0.9/tools/scripts/debug_holidays.py
+-rw-r--r--   0     1001      127    43764 2024-04-22 19:42:39.000000 polars_ts-0.0.9/Cargo.lock
+-rw-r--r--   0     1001      127      478 2024-04-22 19:42:39.000000 polars_ts-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.9/PKG-INFO
```

### Comparing `polars_ts-0.0.8/Cargo.toml` & `polars_ts-0.0.9/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [package]
 name = "polars-ts"
-version = "0.0.8"
+version = "0.0.9"
 edition = "2021"
 
 [lib]
 name = "polars_ts"
 crate-type= ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21.2", features = ["extension-module", "abi3-py38"] }
 pyo3-polars = { version = "0.13.0", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
-polars = { version = "0.39.2", default-features = false }
+polars = { version = "0.39.2", features = ["dtype-date"], default-features = false }
+polars-core = { version = "0.39.2", features=["serde"], default-features = false }
+polars-time = { version = "0.39.2", features = ["dtype-date"], default-features = false }
+polars-arrow = { version = "0.39.2", default-features = false }
+
 rand = "0.8.5"
 rand_distr = "0.4.3"
 wyhash = "0.5.0"
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"] }
```

### Comparing `polars_ts-0.0.8/.github/workflows/publish_to_pypi.yml` & `polars_ts-0.0.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/.gitignore` & `polars_ts-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/LICENSE` & `polars_ts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/Makefile` & `polars_ts-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/README.md` & `polars_ts-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/__init__.py` & `polars_ts-0.0.9/polars_ts/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from .mathx import *
 from .resample import *
 
 from .calendar import *
 from .futures import *
 from .dummymkt import *
 
+from .grouper import Grouper  # noqa
+
 pl.enable_string_cache()
 
 
 if TYPE_CHECKING:
     from polars.type_aliases import IntoExpr
```

### Comparing `polars_ts-0.0.8/polars_ts/calendar.py` & `polars_ts-0.0.9/polars_ts/calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/calendar_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/calendar_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
 def impl_month_to_imm_dict(
     invert: bool = False,
 ) -> Dict[Union[str, int], Union[str, int]]:
     result_cols = ["month_idx", "imm_code"]
     df = (
-        pl.DataFrame({"imm_code": "FGHJKMNQUVXZ"})
+        pl.from_dict({"imm_code": "FGHJKMNQUVXZ"})
         .select(
             pl.col("imm_code").str.extract_all("[F-Z]").explode().cast(pl.Categorical)
         )
         .with_row_index("month_idx", offset=1)
         .select(reversed(result_cols) if invert else result_cols)
     )
```

### Comparing `polars_ts-0.0.8/polars_ts/display.py` & `polars_ts-0.0.9/polars_ts/display.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/dummy.py` & `polars_ts-0.0.9/polars_ts/dummy.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/dummy_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/dummy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/dummymkt.py` & `polars_ts-0.0.9/polars_ts/dummymkt.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/dummymkt_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/dummymkt_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/expr/random.py` & `polars_ts-0.0.9/polars_ts/expr/random.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures.py` & `polars_ts-0.0.9/polars_ts/futures.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/futures_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures_helper/bbg_symbols.py` & `polars_ts-0.0.9/polars_ts/futures_helper/bbg_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures_helper/generic_symbols.py` & `polars_ts-0.0.9/polars_ts/futures_helper/generic_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures_helper/roll_calendar.py` & `polars_ts-0.0.9/polars_ts/futures_helper/roll_calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/futures_helper/util.py` & `polars_ts-0.0.9/polars_ts/futures_helper/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..utils import parse_into_expr
 
 
 def month_to_imm_dict(invert: bool = False) -> Dict[Union[str, int], Union[str, int]]:
     result_cols = ["month_idx", "imm_code"]
     df = (
-        pl.DataFrame({"imm_code": "FGHJKMNQUVXZ"})
+        pl.from_dict({"imm_code": "FGHJKMNQUVXZ"})
         .select(
             pl.col("imm_code").str.extract_all("[F-Z]").explode().cast(pl.Categorical)
         )
         .with_row_index("month_idx", offset=1)
         .select(reversed(result_cols) if invert else result_cols)
     )
```

### Comparing `polars_ts-0.0.8/polars_ts/grouper.py` & `polars_ts-0.0.9/polars_ts/grouper.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/io_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/io_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/polars_ts/mathx.py` & `polars_ts-0.0.9/polars_ts/mathx.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,32 @@
 
     def diff(
         self,
         k: int = 1,
         method: Literal["arithmetic", "fractional", "geometric"] = "arithmetic",
         partition: Grouper = Grouper().by_all(),
         null_strategy: NullStrategyType = "drop",
-        null_sentinel_numeric: SentinelNumeric = 0.0,
+        null_sentinel: SentinelNumeric = 0.0,
     ) -> FrameType:
-        df = impl_diff(
-            self._df, k, method, partition, null_strategy, null_sentinel_numeric
-        )
+        df = impl_diff(self._df, k, method, partition, null_strategy, null_sentinel)
         return prepare_result(df)
 
     def cum_sum(self, partition: Grouper = Grouper().by_all()) -> FrameType:
         df = impl_cum_sum(self._df, partition)
 
         return prepare_result(df)
 
     def shift(
         self,
         k: int = 1,
         null_strategy: NullStrategyType = "ignore",
-        null_sentinel_numeric: SentinelNumeric = 0.0,
+        null_sentinel: SentinelNumeric = 0.0,
         partition: Grouper = Grouper().by_all(),
     ) -> FrameType:
-        df = impl_shift(self._df, k, null_strategy, null_sentinel_numeric, partition)
+        df = impl_shift(self._df, k, null_strategy, null_sentinel, partition)
         return prepare_result(df)
 
     def ewm_mean(
         self,
         half_life: float,
         partition: Grouper = Grouper().by_all(),
     ) -> FrameType:
```

### Comparing `polars_ts-0.0.8/polars_ts/mathx_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/mathx_helper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import math
 from typing import Literal
 
 import polars as pl
 
-from ..sf_helper import impl_apply_null_strategy
+from ..sf_helper import impl_fill_null
 from ..grouper import Grouper
 
 from ..types import FrameType, NullStrategyType, SentinelNumeric
 
 
 def impl_diff(
     df: FrameType,
     k: int,
     method: Literal["arithmetic", "fractional", "geometric"],
     partition: Grouper,
     null_strategy: NullStrategyType,
-    null_sentinel_numeric: SentinelNumeric,
+    null_sentinel: SentinelNumeric,
 ) -> FrameType:
     grouper_cols = partition.apply(df)
     numeric_cols = partition.numerics(df)
 
     result = df.with_columns(pl.col(numeric_cols).diff(k).over(grouper_cols))
-    result = impl_apply_null_strategy(
-        result, null_strategy, null_sentinel_numeric, partition
-    )
+    result = impl_fill_null(result, null_strategy, null_sentinel, partition)
 
     return result
 
 
 def impl_cum_sum(df: FrameType, partition: Grouper) -> FrameType:
     grouper_cols = partition.apply(df)
     numeric_cols = partition.numerics(df)
@@ -37,24 +35,22 @@
     return result
 
 
 def impl_shift(
     df: FrameType,
     k: int,
     null_strategy: NullStrategyType,
-    null_sentinel_numeric: SentinelNumeric,
+    null_sentinel: SentinelNumeric,
     partition: Grouper,
 ) -> FrameType:
     grouper_cols = partition.apply(df)
     numeric_cols = partition.numerics(df)
 
     result = df.with_columns(pl.col(numeric_cols).shift(k).over(grouper_cols))
-    result = impl_apply_null_strategy(
-        result, null_strategy, null_sentinel_numeric, partition
-    )
+    result = impl_fill_null(result, null_strategy, null_sentinel, partition)
 
     return result
 
 
 def impl_ewm_mean(
     df: FrameType,
     half_life: float,
```

### Comparing `polars_ts-0.0.8/polars_ts/resample.py` & `polars_ts-0.0.9/polars_ts/resample.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from typing import Literal, Union, Generic
+from typing import Literal, Generic
 
 import polars as pl
 
 from .sf_helper import prepare_result
 
 from .resample_helper import (
     impl_align_to_time,
     impl_align_values,
     impl_resample_categories,
 )
 
 from .grouper import Grouper
 from .tsf import TimeSeriesFrame
-from .types import (
-    IntervalType,
-    NullStrategyType,
-    FrameType,
-)
+from .types import IntervalType, NullStrategyType, FrameType, SentinelNumeric
 
 __NAMESPACE = "rs"
 
 
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
 class ResampleFrame(TimeSeriesFrame, Generic[FrameType]):
     def __init__(self, df: FrameType):
@@ -50,18 +46,18 @@
 
     def align_to_time(
         self,
         time_axis: pl.Series,
         partition: Grouper = Grouper().by_all(),
         closed: IntervalType = "left",
         null_strategy: NullStrategyType = "forward",
-        null_sentinel_numeric: Union[float, int] = 0.0,
+        null_sentinel: SentinelNumeric = 0.0,
     ) -> FrameType:
         df = impl_align_to_time(
-            self._df, time_axis, partition, closed, null_strategy, null_sentinel_numeric
+            self._df, time_axis, partition, closed, null_strategy, null_sentinel
         )
 
         return prepare_result(df)
 
     def resample_categories(
         self,
         time_axis: pl.Series,
@@ -74,19 +70,19 @@
 
     def align_values(
         self,
         rhs: FrameType,
         partition: Grouper = Grouper().by_all(),
         retain_values: Literal["lhs", "rhs", "both"] = "lhs",
         null_strategy: NullStrategyType = "forward",
-        null_sentinel_numeric: Union[float, int] = 0.0,
+        null_sentinel: SentinelNumeric = 0.0,
     ) -> FrameType:
         df = impl_align_values(
             self._df,
             rhs,
             partition,
             retain_values,
             null_strategy,
-            null_sentinel_numeric,
+            null_sentinel,
         )
 
         return prepare_result(df)
```

### Comparing `polars_ts-0.0.8/polars_ts/resample_helper/__init__.py` & `polars_ts-0.0.9/polars_ts/resample_helper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import polars as pl
 
-from ..sf_helper import impl_apply_null_strategy
+from ..sf_helper import impl_fill_null
 from ..grouper import Grouper
 
 from ..types import (
     IntervalType,
     NullStrategyType,
     RetainValuesType,
     FrameType,
@@ -14,24 +14,24 @@
 
 def impl_align_to_time(
     df: FrameType,
     time_axis: pl.Series,
     partition: Grouper,
     closed: IntervalType,
     null_strategy: NullStrategyType,
-    null_sentinel_numeric: SentinelNumeric,
+    null_sentinel: SentinelNumeric,
 ) -> FrameType:
     resampled = impl_resample_categories(df, time_axis, partition, closed)
     realigned = impl_align_values(
         df,
         resampled,
         partition,
         retain_values="lhs",
         null_strategy=null_strategy,
-        null_sentinel_numeric=null_sentinel_numeric,
+        null_sentinel=null_sentinel,
     )
 
     return realigned
 
 
 def impl_resample_categories(
     df: FrameType,
@@ -71,15 +71,15 @@
 
 def impl_align_values(
     lhs: FrameType,
     rhs: FrameType,
     partition: Grouper,
     retain_values: RetainValuesType,
     null_strategy: NullStrategyType,
-    null_sentinel_numeric: SentinelNumeric,
+    null_sentinel: SentinelNumeric,
 ) -> FrameType:
     rhs_cat_cols = Grouper.categories(rhs, include_time=True)
     rhs_grid = rhs.select(rhs_cat_cols)
 
     if retain_values == "lhs":
         # strip away rhs values
         rhs = rhs_grid
@@ -94,14 +94,12 @@
     result = (
         lhs.join(rhs, on=common_cols, how="outer_coalesce")
         .filter(pl.col("time").is_not_null())
         .sort(*common_cols)
         .unique(keep="first", maintain_order=True)
     )
 
-    result = impl_apply_null_strategy(
-        result, null_strategy, null_sentinel_numeric, partition
-    )
+    result = impl_fill_null(result, null_strategy, null_sentinel, partition)
 
     result = result.join(rhs_grid, on=rhs_cat_cols, how="inner")
 
     return result
```

### Comparing `polars_ts-0.0.8/polars_ts/types.py` & `polars_ts-0.0.9/polars_ts/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CorrelationType = Literal[
     "additive", "multiplicative", "shift", "exponent", "average", "none"
 ]
 
 NullStrategyType = Literal[
     "drop",
     "ignore",
-    "sentinel_numeric",
+    "sentinel",
     "forward",
     "backward",
     "interpolate_linear",
     "interpolate_nearest",
 ]
 
 SentinelNumeric = Union[float, int]
```

### Comparing `polars_ts-0.0.8/polars_ts/utils.py` & `polars_ts-0.0.9/polars_ts/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/src/math/mod.rs` & `polars_ts-0.0.9/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/src/utils.rs` & `polars_ts-0.0.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/futures/test_continuous_contract.py` & `polars_ts-0.0.9/tests/futures/test_continuous_contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     )
 
     roll_calendar = pl.LazyFrame().future.create_roll_calendar(
         roll_config, security_dates
     )
 
     instrument_prices = security_dates.dummymkt.fetch_instrument_prices(
-        "fut_first_trade_dt",
-        pl.min_horizontal("expiry_date", pl.lit(market_end_date.date())),
-        remove_weekends=False,
+        market_start_date.date(),
+        market_end_date.date(),
+        remove_weekends=True,
     )
 
     adjusted_prices = (
         pl.LazyFrame()
         .future.prepare_unadjusted_for_stitching(roll_calendar, instrument_prices)
         .future.stitch_panama_backwards()
     )
@@ -60,11 +60,11 @@
         ("panama_backwards", pl.Float64),
     ]
 
     assert adjusted_prices_schema == expected_schema
 
     result = adjusted_prices.collect()
 
-    assert result.shape == (10030, 5)
+    assert result.shape == (7830, 5)
 
     # replace that with a stable hash
-    assert result.hash_rows().sum() == 4148443207706655575
+    assert result.hash_rows().sum() == 11359005816526693312
```

### Comparing `polars_ts-0.0.8/tests/grouper/test_grouper.py` & `polars_ts-0.0.9/tests/grouper/test_grouper.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/mathx/test_cum_sum.py` & `polars_ts-0.0.9/tests/mathx/test_cum_sum.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/mathx/test_diff.py` & `polars_ts-0.0.9/tests/mathx/test_diff.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/mathx/test_ewm_mean.py` & `polars_ts-0.0.9/tests/mathx/test_ewm_mean.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/mathx/test_shift.py` & `polars_ts-0.0.9/tests/mathx/test_shift.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/resample/test_resample.py` & `polars_ts-0.0.9/tests/resample/test_resample.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/sf/test_join.py` & `polars_ts-0.0.9/tests/sf/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/sf/test_sf.py` & `polars_ts-0.0.9/tests/sf/test_sf.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.8/tests/test_rust_templates.py` & `polars_ts-0.0.9/tests/test_rust_templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import polars as pl
 from polars_ts import pig_latinnify, template_1
 
 
 def test_piglatinnify():
-    df = pl.DataFrame(
+    df = pl.from_dict(
         {
             "english": ["this", "is", "not", "pig", "latin"],
         }
     )
     result = df.with_columns(pig_latin=pig_latinnify("english"))
 
-    expected_df = pl.DataFrame(
+    expected_df = pl.from_dict(
         {
             "english": ["this", "is", "not", "pig", "latin"],
             "pig_latin": ["histay", "siay", "otnay", "igpay", "atinlay"],
         }
     )
 
     assert result.equals(expected_df)
 
 
 def test_template_1():
-    df = pl.DataFrame({"x": [0, 1, 2, 3, 4]})
+    df = pl.from_dict({"x": [0, 1, 2, 3, 4]})
 
     result = df.lazy().with_columns(result=template_1(pl.col("x"), seed=100)).collect()
 
-    expected_df = pl.DataFrame(
+    expected_df = pl.from_dict(
         {
             "x": [0, 1, 2, 3, 4],
             "result": [100, 201, 303, 406, 510],
         }
     )
 
     assert result.equals(expected_df)
```

### Comparing `polars_ts-0.0.8/Cargo.lock` & `polars_ts-0.0.9/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,41 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
+
+[[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "argminmax"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
@@ -42,24 +57,33 @@
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
 [[package]]
+name = "atoi"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -70,20 +94,23 @@
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
@@ -94,48 +121,71 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+dependencies = [
+ "jobserver",
+ "libc",
+ "once_cell",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
  "num-traits",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "core-foundation-sys"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
+name = "crossbeam-channel"
+version = "0.5.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+dependencies = [
+ "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
@@ -150,30 +200,51 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "crossbeam-queue"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+
+[[package]]
+name = "enum_dispatch"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
+dependencies = [
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -199,26 +270,32 @@
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
  "allocator-api2",
@@ -237,40 +314,63 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows-core",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jemalloc-sys"
 version = "0.5.4+5.3.0-patched"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac6c1946e1cea1788cbfde01c993b52a10e2da07f4bac608228d1bed20bfebf2"
 dependencies = [
@@ -285,14 +385,23 @@
 checksum = "a0de374a9f8e63150e6f5e8a60cc14c668226d7a347d8aee1a45766e3c4dd3bc"
 dependencies = [
  "jemalloc-sys",
  "libc",
 ]
 
 [[package]]
+name = "jobserver"
+version = "0.1.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -322,33 +431,53 @@
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "lz4"
+version = "1.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
+dependencies = [
+ "libc",
+ "lz4-sys",
+]
+
+[[package]]
+name = "lz4-sys"
+version = "1.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.4"
@@ -368,14 +497,32 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
 [[package]]
+name = "now"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
+dependencies = [
+ "chrono",
+]
+
+[[package]]
+name = "ntapi"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -439,14 +586,20 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pkg-config"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
@@ -457,15 +610,19 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
+ "polars-io",
+ "polars-lazy",
+ "polars-ops",
  "polars-parquet",
+ "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
 version = "0.39.2"
@@ -480,24 +637,26 @@
  "either",
  "ethnum",
  "fast-float",
  "foreign_vec",
  "getrandom",
  "hashbrown",
  "itoa",
+ "lz4",
  "multiversion",
  "num-traits",
  "polars-arrow-format",
  "polars-error",
  "polars-utils",
  "ryu",
  "simdutf8",
  "streaming-iterator",
  "strength_reduce",
  "version_check",
+ "zstd",
 ]
 
 [[package]]
 name = "polars-arrow-format"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b0ef2474af9396b19025b189d96e992311e6a47f90c53cd998b36c4c64b84c"
@@ -527,82 +686,110 @@
 version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "bytemuck",
+ "chrono",
  "either",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-arrow",
  "polars-compute",
  "polars-error",
  "polars-row",
  "polars-utils",
  "rand",
  "rand_distr",
  "rayon",
+ "regex",
+ "serde",
  "smartstring",
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
 version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
  "polars-arrow-format",
+ "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-ffi"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "199206173cb2dcdc6840d65c0395313ac55c5a1e82c5c9fbeaa44a4c340a88b0"
+checksum = "dcdd5a0b45dea8df72db9dfca694a1acc753bd868f3a751903b83cacdb896d2b"
 dependencies = [
  "polars-arrow",
  "polars-core",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d47f2cdd8e2a2bfc71b0d30444d4c378ddc0d6f80826746fc3c731c06251b42"
+checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
 dependencies = [
  "ahash",
  "bytes",
  "home",
  "memchr",
  "memmap2",
  "num-traits",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-error",
+ "polars-time",
  "polars-utils",
  "rayon",
  "regex",
  "smartstring",
 ]
 
 [[package]]
+name = "polars-lazy"
+version = "0.39.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89b2632b1af668e2058d5f8f916d8fbde3cac63d03ae29a705f598e41dcfeb7f"
+dependencies = [
+ "ahash",
+ "bitflags 2.5.0",
+ "glob",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-pipe",
+ "polars-plan",
+ "polars-time",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+ "version_check",
+]
+
+[[package]]
 name = "polars-ops"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f311543e0e110d385867df25f47c1c740ee0cc854feead54262a24b0246383bb"
+checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
 dependencies = [
  "ahash",
  "argminmax",
  "bytemuck",
  "either",
  "hashbrown",
  "indexmap",
@@ -635,28 +822,54 @@
  "polars-utils",
  "seq-macro",
  "simdutf8",
  "streaming-decompression",
 ]
 
 [[package]]
+name = "polars-pipe"
+version = "0.39.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48700f1d5bd56a15451e581f465c09541492750360f18637b196f995470a015c"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-queue",
+ "enum_dispatch",
+ "hashbrown",
+ "num-traits",
+ "polars-arrow",
+ "polars-compute",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-plan",
+ "polars-row",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+ "uuid",
+ "version_check",
+]
+
+[[package]]
 name = "polars-plan"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c509bc273c402a8b1fbfa63df2b2e90ca10d30decab698c7739003817de67e1"
+checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
+ "polars-time",
  "polars-utils",
  "rayon",
  "recursive",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
@@ -670,19 +883,41 @@
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
+name = "polars-time"
+version = "0.39.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "efc18e3ad92eec55db89d88f16c22d436559ba7030cf76f86f6ed7a754b673f1"
+dependencies = [
+ "atoi",
+ "chrono",
+ "now",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-error",
+ "polars-ops",
+ "polars-utils",
+ "regex",
+ "smartstring",
+]
+
+[[package]]
 name = "polars-ts"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "jemallocator",
  "polars",
+ "polars-arrow",
+ "polars-core",
+ "polars-time",
  "pyo3",
  "pyo3-polars",
  "rand",
  "rand_distr",
  "serde",
  "wyhash",
 ]
@@ -700,14 +935,15 @@
  "num-traits",
  "once_cell",
  "polars-error",
  "raw-cpuid",
  "rayon",
  "smartstring",
  "stacker",
+ "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -717,17 +953,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -780,28 +1016,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-polars"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
@@ -824,22 +1060,22 @@
 checksum = "3ba3d428667917efd2c233534db5779f55b398e123aea75243da8491856e1131"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -887,17 +1123,17 @@
 checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -922,31 +1158,31 @@
 [[package]]
 name = "recursive-proc-macro-impl"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
 dependencies = [
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -959,23 +1195,23 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -989,17 +1225,17 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-pickle"
 version = "1.1.1"
@@ -1011,42 +1247,43 @@
  "num-bigint",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
  "autocfg",
+ "serde",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "stacker"
 version = "0.1.15"
@@ -1093,15 +1330,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1109,53 +1346,67 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "sysinfo"
+version = "0.30.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87341a165d73787554941cd5ef55ad728011566fe714e987d1b976c15dbc3a83"
+dependencies = [
+ "cfg-if",
+ "core-foundation-sys",
+ "libc",
+ "ntapi",
+ "once_cell",
+ "windows",
+]
+
+[[package]]
 name = "target-features"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1bbb9f3c5c463a01705937a24fdabc5047929ac764b2d5b9cf681c1f5041ed5"
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -1163,14 +1414,23 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
@@ -1195,15 +1455,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1217,15 +1477,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1251,20 +1511,39 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1276,110 +1555,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "wyhash"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf6e163c25e3fac820b4b453185ea2dea3b6a3e0a721d4d23d75bd33734c295"
 dependencies = [
@@ -1405,9 +1691,37 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.60",
+]
+
+[[package]]
+name = "zstd"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "7.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
+dependencies = [
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.10+zstd.1.5.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
+dependencies = [
+ "cc",
+ "pkg-config",
 ]
```

### Comparing `polars_ts-0.0.8/PKG-INFO` & `polars_ts-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: polars-ts
-Version: 0.0.8
-Requires-Dist: polars >=0.20.21
+Version: 0.0.9
+Requires-Dist: polars >=0.20.22
 Requires-Dist: polars-xdt
 Requires-Dist: hvplot
 Requires-Dist: pyarrow
 Requires-Dist: hvplot ; extra == 'dev'
 Requires-Dist: pyarrow ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
```

