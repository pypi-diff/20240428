# Comparing `tmp/chencrafts-1.1.tar.gz` & `tmp/chencrafts-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chencrafts-1.1.tar", last modified: Thu Apr 18 06:13:08 2024, max compression
+gzip compressed data, was "chencrafts-1.3.tar", last modified: Sun Apr 28 05:45:59 2024, max compression
```

## Comparing `chencrafts-1.1.tar` & `chencrafts-1.3.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.612922 chencrafts-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-18 06:12:52.000000 chencrafts-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 06:12:52.000000 chencrafts-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-18 06:13:08.612922 chencrafts-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 06:12:52.000000 chencrafts-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.600922 chencrafts-1.1/chencrafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.604922 chencrafts-1.1/chencrafts/bsqubits/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.604922 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30405 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/cat_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/QEC_graph/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/batched_custom_sweeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/cat_ideal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/cat_real.py
--rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/derive_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/error_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/pulse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/bsqubits/systems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/cqed/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/block_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/crit_photon_num.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/cqed/custom_sweeps/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/crit_photon_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/custom_sweeps/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/decoherence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/flexible_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/mode_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/pulses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/qt_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/scq_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/spec_poly_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/special_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/cqed/symbolic_bosons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/fluxonium_tunable_coupler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/protomon_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/projects/protomon_full_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/chencrafts/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/gadgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-18 06:12:52.000000 chencrafts-1.1/chencrafts/toolbox/useless.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.612922 chencrafts-1.1/chencrafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 06:13:08.000000 chencrafts-1.1/chencrafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 06:12:52.000000 chencrafts-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 06:12:52.000000 chencrafts-1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:13:08.612922 chencrafts-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 06:12:52.000000 chencrafts-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:08.608922 chencrafts-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-18 06:12:52.000000 chencrafts-1.1/tests/test_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.390078 chencrafts-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.378078 chencrafts-1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.382078 chencrafts-1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-28 05:45:55.000000 chencrafts-1.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-28 05:45:55.000000 chencrafts-1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-28 05:45:55.000000 chencrafts-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-28 05:45:55.000000 chencrafts-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-28 05:45:59.390078 chencrafts-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 05:45:55.000000 chencrafts-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.382078 chencrafts-1.3/chencrafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.382078 chencrafts-1.3/chencrafts/bsqubits/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.386078 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33150 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/cat_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/QEC_graph/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/batched_custom_sweeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/cat_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19291 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/cat_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/derive_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/error_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/pulse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26739 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/bsqubits/systems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.386078 chencrafts-1.3/chencrafts/cqed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/block_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/crit_photon_num.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.386078 chencrafts-1.3/chencrafts/cqed/custom_sweeps/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/custom_sweeps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/custom_sweeps/crit_photon_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/custom_sweeps/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/custom_sweeps/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/custom_sweeps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/decoherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/flexible_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/mode_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/pulses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/qt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/scq_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/spec_poly_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/special_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/cqed/symbolic_bosons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.386078 chencrafts-1.3/chencrafts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78060 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/projects/fluxonium_tunable_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/projects/protomon_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36649 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/projects/protomon_full_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.390078 chencrafts-1.3/chencrafts/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/gadgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41421 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-28 05:45:55.000000 chencrafts-1.3/chencrafts/toolbox/useless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.390078 chencrafts-1.3/chencrafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 05:45:59.000000 chencrafts-1.3/chencrafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-28 05:45:55.000000 chencrafts-1.3/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-28 05:45:55.000000 chencrafts-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:45:59.390078 chencrafts-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:45:59.390078 chencrafts-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-28 05:45:55.000000 chencrafts-1.3/tests/test_optimization.py
```

### Comparing `chencrafts-1.1/LICENSE` & `chencrafts-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/PKG-INFO` & `chencrafts-1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 1.1
-Summary: CHEN CRAFTS, my personal toolbox!
-Home-page: https://github.com/Harrinive/chencrafts
-Author: Danyang Chen
-Author-email: DanyangChen2026@u.northwestern.edu
-License: MIT
+Version: 1.3
+Summary: A personal toolbox for superconducting qubits and quantum mechanics.
+Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
+License: BSD
+Project-URL: Homepage, https://github.com/Harrinive/chencrafts
+Project-URL: Repository, https://github.com/Harrinive/chencrafts
 Keywords: personal toolbox,superconducting qubits,quantum mechanics
-Platform: Linux
-Platform: Mac OSX
-Platform: Unix
-Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: matplotlib
 Requires-Dist: scipy
-Requires-Dist: tqdm
 Requires-Dist: pandas
+Requires-Dist: tqdm
 Requires-Dist: dill
 Requires-Dist: pathos
 Requires-Dist: scqubits
 Requires-Dist: IPython
 Provides-Extra: cqed
-Requires-Dist: torch; extra == "cqed"
+Requires-Dist: torch>=1.7; extra == "cqed"
 Requires-Dist: multiprocess; extra == "cqed"
 Provides-Extra: bsqubits
-Requires-Dist: networkx; extra == "bsqubits"
+Requires-Dist: networkx>=2.4; extra == "bsqubits"
 
+CHENCRAFTS, Danyang's personal toolbox!
+=================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-1.1/README.md` & `chencrafts-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CHEN CRAFTS, my personal toolbox!
+CHENCRAFTS, Danyang's personal toolbox!
 =================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-1.1/chencrafts/__init__.py` & `chencrafts-1.3/chencrafts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 # import submodules
 # when changed, remember to change setup.py
 import chencrafts.bsqubits as bsq
 import chencrafts.cqed as cqed
 import chencrafts.projects as prj
 import chencrafts.toolbox as tb
 
-# set matplotlib 
-import matplotlib as _mpl
-import matplotlib.font_manager as _mpl_font
-from chencrafts.toolbox.plot import color_cyclers as _color_cyclers
-_mpl.rcParams = _mpl.rcParamsDefault.copy()
-# figure format
-
 # set figure format in jupyter notebook
 try:
     get_ipython()
     import matplotlib_inline.backend_inline as _backend_inline
     _backend_inline.set_matplotlib_formats("png")
 except NameError:
     pass
 
+# set matplotlib 
+import matplotlib as _mpl
+import matplotlib.font_manager as _mpl_font
+from chencrafts.toolbox.plot import color_cyclers as _color_cyclers
+_mpl.rcParams = _mpl.rcParamsDefault.copy()
+
 # color cycle
 _mpl.rcParams["axes.prop_cycle"] = _color_cyclers["PGL"]
 _mpl.rcParams['text.usetex'] = False
+
 # disable font warning message
 font_selected = None
 try:
     font_names = _mpl_font.get_font_names()
     for font in ["IBM Plex Sans", "Roboto", "Arial", "Helvetica"]:
         if font in font_names:
             font_selected = font
```

### Comparing `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/__init__.py` & `chencrafts-1.3/chencrafts/bsqubits/QEC_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/cat_tree.py` & `chencrafts-1.3/chencrafts/bsqubits/QEC_graph/cat_tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,333 @@
+from typing import List, Tuple, Any, TYPE_CHECKING, Dict, Callable, overload, Literal
+from warnings import warn
+from copy import deepcopy
+from tqdm.notebook import tqdm
+from abc import ABC, abstractmethod
+
 import numpy as np
 import qutip as qt
 import scqubits as scq
 
-
 from chencrafts.cqed import FlexibleSweep, superop_evolve
 
 from chencrafts.bsqubits.QEC_graph.node import StateNode, StateEnsemble, MeasurementRecord
 from chencrafts.bsqubits.QEC_graph.edge import (
     PropagatorEdge, MeasurementEdge, Edge, CheckPointEdge)
 from chencrafts.bsqubits.QEC_graph.graph import EvolutionGraph, EvolutionTree
 
 import chencrafts.bsqubits.cat_ideal as cat_ideal
 import chencrafts.bsqubits.cat_real as cat_real
 
-from tqdm.notebook import tqdm
-from typing import List, Tuple, Any, TYPE_CHECKING, Dict, Callable, overload, Literal
-from warnings import warn
 
 
-class GraphBuilder:
+class TreeBuilder(ABC):
 
     graph = EvolutionGraph()
 
+    # ideal_process_switches
+    idling_is_ideal: bool = False
+    gate_1_is_ideal: bool = True
+    parity_mapping_is_ideal: bool = False
+    gate_2_is_ideal: bool = True
+    qubit_measurement_is_ideal: bool = False
+    qubit_reset_is_ideal: bool = True
+
     def __init__(
         self,
         fsweep: FlexibleSweep,
         sim_para: Dict[str, Any],
     ):
         self.fsweep = fsweep
         self.sim_para = sim_para
 
+    # utils ############################################################
+    @staticmethod
+    def _current_parity(meas_record: MeasurementRecord):
+        # with adaptive qubit pulse, detecting "1" meaning a parity flip
+        return sum(meas_record) % 2
+
+    @staticmethod
+    @overload
+    def _kraus_to_super(
+        qobj_list: List[qt.Qobj]
+    ) -> qt.Qobj:
+        ...
+
+    @staticmethod
+    @overload
+    def _kraus_to_super(
+        qobj_list: Callable[[MeasurementRecord], List[qt.Qobj]]
+    ) -> Callable[[MeasurementRecord], qt.Qobj]:
+        ...
+        
+    @staticmethod
+    def _kraus_to_super(
+        qobj_list: List[qt.Qobj] | Callable[[MeasurementRecord], List[qt.Qobj]]
+    ) -> qt.Qobj | Callable[[MeasurementRecord], qt.Qobj]:
+        """
+        Convert a list of Kraus operators to a superoperator. It also works
+        for a function that returns a list of Kraus operators.
+        """
+        if isinstance(qobj_list, qt.Qobj):
+            # Qobj is callable and we should detect it before checking callable
+            raise TypeError("The input should be a list of Qobj or a function.")
+        
+        if isinstance(qobj_list, list):
+            return sum([qt.to_super(qobj) for qobj in qobj_list])
+        elif callable(qobj_list):
+            return lambda meas_record: sum([qt.to_super(qobj) for qobj in qobj_list(meas_record)])
+        else:
+            raise TypeError("The input should be a list of Qobj or a function.")
+        
+    @staticmethod
+    def _add_leaves(
+        graph: EvolutionTree,
+        nodes: StateEnsemble,
+        edge: Edge,
+    ) -> StateEnsemble:
+        final_nodes = StateEnsemble()
+
+        for node in nodes.active_nodes():
+            edge = deepcopy(edge)
+            f_node = StateNode()
+            final_nodes.append(f_node)
+            graph.add_node(f_node)
+            graph.add_edge_connect(
+                edge,
+                node,
+                f_node,
+            )
+
+        return final_nodes
+        
+    # idling ###########################################################
+    _idling_real: qt.Qobj
+    _idling_ideal: List[qt.Qobj]
+
+    def idle(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+        correctable_single_photon_loss: bool = True,
+    ) -> StateEnsemble:
+        """
+        Idling process.
+
+        Add one idling edge to every node in the initial ensemble.
+
+        Note that it doesn't support idling_is_ideal.
+
+        Parameters
+        ----------
+        correctable_single_photon_loss: bool
+            Denote single-photon loss as a correctable error, which enables 
+            the fidelity calculation when QEC is on. When QEC is off, we should 
+            set it to False.
+        """
+        if correctable_single_photon_loss:
+            accepted_states_num = 2
+        else:
+            accepted_states_num = 1
+
+        edge_idling = PropagatorEdge(
+            f"ID ({step})",
+            self._idling_real,  # when ideal, time=0, it's already the identity, no need to change
+            self._idling_ideal[:accepted_states_num],
+        )
+
+        return self._add_leaves(graph, init_nodes.active_nodes(), edge_idling)
+    
+    # qubit gate #######################################################
+    _qubit_gate_p_ideal: List[qt.Qobj]
+    _qubit_gate_m_ideal: List[qt.Qobj]
+    _qubit_gate_p_real: qt.Qobj
+    _qubit_gate_m_real: qt.Qobj
+
+    @abstractmethod
+    def _qubit_gate_2_map_real(
+        self,
+        meas_record: MeasurementRecord,
+    ) -> qt.Qobj:
+        pass
+        
+    @abstractmethod
+    def _qubit_gate_2_map_ideal(
+        self,
+        meas_record: MeasurementRecord,
+    ) -> List[qt.Qobj]:
+        pass
+
+    def qubit_gate_1(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        edge_qubit_gate = PropagatorEdge(
+            f"G1 ({step})",
+            (
+                self._qubit_gate_p_real 
+                if not self.gate_1_is_ideal 
+                else self._kraus_to_super(self._qubit_gate_p_ideal)
+            ),
+            self._qubit_gate_p_ideal,
+        )
+        return self._add_leaves(graph, init_nodes.active_nodes(), edge_qubit_gate)
+    
+    def qubit_gate_2(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        edge_qubit_gate = PropagatorEdge(
+            f"G2 ({step})",
+            (
+                self._qubit_gate_2_map_real 
+                if not self.gate_2_is_ideal 
+                else self._kraus_to_super(self._qubit_gate_2_map_ideal)
+            ),
+            self._qubit_gate_2_map_ideal,
+        )
+
+        return self._add_leaves(graph, init_nodes.active_nodes(), edge_qubit_gate)
+    
+    # parity mapping ###################################################
+    _parity_mapping_ideal: List[qt.Qobj]
+    _parity_mapping_real: qt.Qobj
+
+    def parity_mapping(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        edge_parity_mapping = PropagatorEdge(
+            name = f"PM ({step})",
+            real_map = (
+                self._parity_mapping_real
+                if not self.parity_mapping_is_ideal 
+                else self._kraus_to_super(self._parity_mapping_ideal)
+            ),
+            ideal_maps = self._parity_mapping_ideal
+        )
+
+        return self._add_leaves(graph, init_nodes.active_nodes(), edge_parity_mapping)
+    
+    # qubit measurement ################################################
+    _accepted_measurement_outcome_pool: List[int]
+    _measurement_outcome_pool: List[int]
+
+    _qubit_projs_ideal: List[qt.Qobj]
+    _qubit_projs_real: List[qt.Qobj]
+
+    def qubit_measurement(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        all_final_nodes = StateEnsemble()
+
+        for idx in range(len(self._qubit_projs_ideal)):
+            # final_node is trash if not accepted
+            trashed = idx >= len(self._accepted_measurement_outcome_pool)
+            edge = MeasurementEdge(
+                name = f"MS ({step})",
+                outcome = self._measurement_outcome_pool[idx],
+                real_map = (
+                    self._qubit_projs_real[idx] 
+                    if not self.qubit_measurement_is_ideal 
+                    else self._qubit_projs_ideal[idx]
+                ),
+                ideal_map = [self._qubit_projs_ideal[idx]],
+            )              
+
+            final_nodes = self._add_leaves(
+                graph, init_nodes.active_nodes(), edge
+            )
+
+            for node in final_nodes.active_nodes():
+                node.terminated = trashed
+
+            all_final_nodes.nodes += final_nodes.nodes
+
+        return all_final_nodes
+    
+    # qubit reset ######################################################
+    @abstractmethod
+    def _qubit_reset_map_real(
+        self,
+        meas_record: MeasurementRecord,
+    ) -> qt.Qobj:
+        pass
+            
+    @abstractmethod
+    def _qubit_reset_map_ideal(
+        self,
+        meas_record: MeasurementRecord,
+    ) -> List[qt.Qobj]:
+        pass
+
+    def qubit_reset(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        final_nodes = StateEnsemble()
+
+        for node in init_nodes.active_nodes():
+            edge_qubit_reset = PropagatorEdge(
+                f"RS ({step})",
+                (
+                    self._qubit_reset_map_real 
+                    if not self.qubit_reset_is_ideal 
+                    else self._kraus_to_super(self._qubit_reset_map_ideal)
+                ),
+                self._qubit_reset_map_ideal,
+            )
+            final_nodes.append(StateNode())
+
+            graph.add_node(final_nodes[-1])
+
+            graph.add_edge_connect(
+                edge_qubit_reset,
+                node,
+                final_nodes[-1],
+            )
+
+        return final_nodes
+    
+    # check point ######################################################
+    def check_point(
+        self,
+        step: int | str,
+        graph: EvolutionTree,
+        init_nodes: StateEnsemble,
+    ) -> StateEnsemble:
+        all_final_nodes = StateEnsemble()
+
+        for success in [True, False]:
+            edge_check_point = CheckPointEdge(
+                name = f"CP ({step})",
+                success = success,
+            )
+            final_nodes = self._add_leaves(
+                graph, init_nodes.active_nodes(), edge_check_point
+            )
+
+            all_final_nodes.nodes += final_nodes.nodes
+        
+        return all_final_nodes
+
 
-class CatGraphBuilder(GraphBuilder):
+class CatGraphBuilder(TreeBuilder):
     _res_mode_idx: int
     _qubit_mode_idx: int
     res_dim: int
     qubit_dim: int
 
     static_hamiltonian: qt.Qobj
     c_ops: List[qt.Qobj]
@@ -43,36 +335,29 @@
     frame_hamiltonian: qt.Qobj
 
     # the ideal process and the real process share the same outcomes,
     # as the actual action is based on the real outcomes.
     _accepted_measurement_outcome_pool = [0, 1]
     _measurement_outcome_pool: List
 
-    # processes:
-    _identity: qt.Qobj
-    _idling_real: qt.Qobj
-    _idling_ideal: List[qt.Qobj]
-    _qubit_gate_m_ideal: List[qt.Qobj]
-    _qubit_gate_p_ideal: List[qt.Qobj]
-    _qubit_gate_m_real: qt.Qobj
-    _qubit_gate_p_real: qt.Qobj
-    _parity_mapping_ideal: List[qt.Qobj]
-    _parity_mapping_real: qt.Qobj
-    _qubit_projs_ideal: List[qt.Qobj]
-    _qubit_projs_real: List[qt.Qobj]
-    _qubit_reset_real: qt.Qobj
-    _qubit_reset_ideal: [qt.Qobj]
+    # # processes:
+    # _identity: qt.Qobj
+    # _idling_real: qt.Qobj
+    # _idling_ideal: List[qt.Qobj]
+    # _qubit_gate_m_ideal: List[qt.Qobj]
+    # _qubit_gate_p_ideal: List[qt.Qobj]
+    # _qubit_gate_m_real: qt.Qobj
+    # _qubit_gate_p_real: qt.Qobj
+    # _parity_mapping_ideal: List[qt.Qobj]
+    # _parity_mapping_real: qt.Qobj
+    # _qubit_projs_ideal: List[qt.Qobj]
+    # _qubit_projs_real: List[qt.Qobj]
+    # _qubit_reset_real: qt.Qobj
+    # _qubit_reset_ideal: List[qt.Qobj]
 
-    # ideal_process_switches
-    idling_is_ideal: bool = False
-    gate_1_is_ideal: bool = True
-    parity_mapping_is_ideal: bool = False
-    gate_2_is_ideal: bool = True
-    qubit_measurement_is_ideal: bool = False
-    qubit_reset_is_ideal: bool = True
 
     def __init__(
         self,
         fsweep: FlexibleSweep,
         sim_para: Dict[str, Any],
     ):
         super().__init__(fsweep, sim_para)
@@ -138,53 +423,14 @@
         # if type(qubit) == scq.Transmon:
         #     self._gate_axis = "x"
         # elif type(qubit) == scq.Fluxonium:
         #     self._gate_axis = "x"
         # else:
         #     raise ValueError("Unknown qubit type.")
         self._gate_axis = "x"
-
-    # utils ############################################################
-    @staticmethod
-    def _current_parity(meas_record: MeasurementRecord):
-        # with adaptive qubit pulse, detecting "1" meaning a parity flip
-        return sum(meas_record) % 2
-
-    @staticmethod
-    @overload
-    def _kraus_to_super(
-        qobj_list: List[qt.Qobj]
-    ) -> qt.Qobj:
-        ...
-
-    @staticmethod
-    @overload
-    def _kraus_to_super(
-        qobj_list: Callable[[MeasurementRecord], List[qt.Qobj]]
-    ) -> Callable[[MeasurementRecord], qt.Qobj]:
-        ...
-        
-    @staticmethod
-    def _kraus_to_super(
-        qobj_list: List[qt.Qobj] | Callable[[MeasurementRecord], List[qt.Qobj]]
-    ) -> qt.Qobj | Callable[[MeasurementRecord], qt.Qobj]:
-        """
-        Convert a list of Kraus operators to a superoperator. It also works
-        for a function that returns a list of Kraus operators.
-        """
-        if isinstance(qobj_list, qt.Qobj):
-            # Qobj is callable and we should detect it before checking callable
-            raise TypeError("The input should be a list of Qobj or a function.")
-        
-        if isinstance(qobj_list, list):
-            return sum([qt.to_super(qobj) for qobj in qobj_list])
-        elif callable(qobj_list):
-            return lambda meas_record: sum([qt.to_super(qobj) for qobj in qobj_list(meas_record)])
-        else:
-            raise TypeError("The input should be a list of Qobj or a function.")
         
     # overall properties ################################################
     @property
     def _total_simulation_time(self) -> float:
         return (
             self._idling_time
             + self._parity_mapping_time
@@ -233,51 +479,14 @@
             res_mode_idx=self._res_mode_idx, superop=False,
         )   # may be used later
 
     @property
     def _idling_time(self) -> float:
         return float(self.fsweep["T_W"] * (1 - self.idling_is_ideal))
 
-    def idle(
-        self,
-        step: int | str,
-        graph: EvolutionTree,
-        init_nodes: StateEnsemble,
-        correctable_single_photon_loss: bool = True,
-    ) -> StateEnsemble:
-        """
-        Idling process.
-
-        Add one idling edge to every node in the initial ensemble.
-        """
-        final_nodes = StateEnsemble()
-
-        if correctable_single_photon_loss:
-            accepted_states_num = 2
-        else:
-            accepted_states_num = 1
-
-        for node in init_nodes.active_nodes():
-            edge_idling = PropagatorEdge(
-                f"ID ({step})",
-                self._idling_real,  # when ideal, time=0, it's already the identity, no need to change
-                self._idling_ideal[:accepted_states_num],
-            )
-            final_nodes.append(StateNode())
-
-            graph.add_node(final_nodes[-1])
-
-            graph.add_edge_connect(
-                edge_idling,
-                node,
-                final_nodes[-1],
-            )
-
-        return final_nodes
-    
     # qubit gate #######################################################
     def frame_transform(
         self,
         propagator: qt.Qobj,
         time: float,
         type: Literal[
             "rot2current", 
@@ -408,74 +617,14 @@
     
     @property
     def _qubit_gate_2_time(self) -> float:
         """Currently the gate time is the same for both ideal and real cases."""
         return float(self.fsweep["tau_p_eff"])
         # return float(self.fsweep["tau_p_eff"] * (1 - self.gate_2_is_ideal))
 
-    def qubit_gate_1(
-        self,
-        step: int | str,
-        graph: EvolutionTree,
-        init_nodes: StateEnsemble,
-    ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
-
-        for node in init_nodes.active_nodes():
-            edge_qubit_gate = PropagatorEdge(
-                f"G1 ({step})",
-                (
-                    self._qubit_gate_p_real 
-                    if not self.gate_1_is_ideal 
-                    else self._kraus_to_super(self._qubit_gate_p_ideal)
-                ),
-                self._qubit_gate_p_ideal,
-            )
-            final_nodes.append(StateNode())
-
-            graph.add_node(final_nodes[-1])
-
-            graph.add_edge_connect(
-                edge_qubit_gate,
-                node,
-                final_nodes[-1],
-            )
-
-        return final_nodes
-    
-    def qubit_gate_2(
-        self,
-        step: int | str,
-        graph: EvolutionTree,
-        init_nodes: StateEnsemble,
-    ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
-
-        for node in init_nodes.active_nodes():
-            edge_qubit_gate = PropagatorEdge(
-                f"G2 ({step})",
-                (
-                    self._qubit_gate_2_map_real 
-                    if not self.gate_2_is_ideal 
-                    else self._kraus_to_super(self._qubit_gate_2_map_ideal)
-                ),
-                self._qubit_gate_2_map_ideal,
-            )
-            final_nodes.append(StateNode())
-
-            graph.add_node(final_nodes[-1])
-
-            graph.add_edge_connect(
-                edge_qubit_gate,
-                node,
-                final_nodes[-1],
-            )
-
-        return final_nodes
-    
     # parity mapping ###################################################
     def _build_parity_mapping_process(
         self,
     ):
         self._parity_mapping_ideal = self._idling_ideal_by_time(self._parity_mapping_time)[:1]
 
         self._parity_mapping_real = self._idling_real_by_time(self._parity_mapping_time)
@@ -523,48 +672,41 @@
         Since a bit of phase has been accumulated during the qubit gates,
         we don't need to apply a full pi rotation.
 
         This property returns the actual rotation needed.
         """
         qubit_gate_time_tot = self._qubit_gate_1_time + self._qubit_gate_2_time
         return np.pi - self._average_pm_interaction * qubit_gate_time_tot / 2
-
+    
     def parity_mapping(
         self,
         step: int | str,
         graph: EvolutionTree,
         init_nodes: StateEnsemble,
     ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
-
-        for node in init_nodes.active_nodes():
-            edge_parity_mapping = PropagatorEdge(
-                name = f"PM ({step})",
-                real_map = (
-                    self._parity_mapping_real
-                    if not self.parity_mapping_is_ideal 
-                    else self._kraus_to_super(self._parity_mapping_constructed)
-                ),
-                ideal_maps = (
-                    self._parity_mapping_ideal
-                    if not self.parity_mapping_is_ideal
-                    else self._parity_mapping_constructed
-                )
-            )
-            final_nodes.append(StateNode())
-
-            graph.add_node(final_nodes[-1])
-
-            graph.add_edge_connect(
-                edge_parity_mapping,
-                node,
-                final_nodes[-1],
+        """
+        Overwrite the base class parity mapping - as when the parity_mapping_is_ideal 
+        is true, the self._parity_mapping_ideal is not TP and can't serve as the 
+        ideal map for actual process.
+        """
+        edge_parity_mapping = PropagatorEdge(
+            name = f"PM ({step})",
+            real_map = (
+                self._parity_mapping_real
+                if not self.parity_mapping_is_ideal 
+                else self._kraus_to_super(self._parity_mapping_constructed)
+            ),
+            ideal_maps = (
+                self._parity_mapping_ideal
+                if not self.parity_mapping_is_ideal
+                else self._parity_mapping_constructed
             )
+        )
 
-        return final_nodes
+        return self._add_leaves(graph, init_nodes.active_nodes(), edge_parity_mapping)
 
     # qubit measurement ################################################
     def _build_qubit_measurement_process(
         self,
     ):
         # ideal process
         self._qubit_projs_constructed = cat_ideal.qubit_projectors(
@@ -620,48 +762,46 @@
 
     def qubit_measurement(
         self,
         step: int | str,
         graph: EvolutionTree,
         init_nodes: StateEnsemble,
     ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
+        all_final_nodes = StateEnsemble()
 
-        for node in init_nodes.active_nodes():
-            for idx in range(len(self._qubit_projs_ideal)):
-                # final_node is trash if not accepted
-                trashed = idx >= len(self._accepted_measurement_outcome_pool)
-
-                edge_qubit_measurement = MeasurementEdge(
-                    name = f"MS ({step})",
-                    outcome = self._measurement_outcome_pool[idx],
-                    real_map = (
-                        self._qubit_projs_real[idx] 
-                        if not self.qubit_measurement_is_ideal 
-                        else qt.to_super(self._qubit_projs_constructed[idx])
-                    ),
-                    ideal_map = (
-                        [self._qubit_projs_ideal[idx]]
-                        if not self.qubit_measurement_is_ideal 
-                        else [self._qubit_projs_constructed[idx]]
-                    ),
-                )                    
-
-                final_node = StateNode()
-                final_node.terminated = trashed
-                final_nodes.append(final_node)
-                graph.add_node(final_node)
-
-                graph.add_edge_connect(
-                    edge_qubit_measurement,
-                    node,
-                    final_node,
-                )
+        for idx in range(len(self._qubit_projs_ideal)):
+            # final_node is trash if not accepted
+            trashed = idx >= len(self._accepted_measurement_outcome_pool)
+
+            edge_qubit_measurement = MeasurementEdge(
+                name = f"MS ({step})",
+                outcome = self._measurement_outcome_pool[idx],
+                real_map = (
+                    self._qubit_projs_real[idx] 
+                    if not self.qubit_measurement_is_ideal 
+                    else qt.to_super(self._qubit_projs_constructed[idx])
+                ),
+                ideal_map = (
+                    [self._qubit_projs_ideal[idx]]
+                    if not self.qubit_measurement_is_ideal 
+                    else [self._qubit_projs_constructed[idx]]
+                ),
+            )                    
 
-        return final_nodes
+            final_nodes = self._add_leaves(
+                graph, init_nodes.active_nodes(), edge_qubit_measurement
+            )
+
+            for node in final_nodes.active_nodes():
+                node.terminated = trashed
+
+            all_final_nodes.nodes += final_nodes.nodes
+            
+
+        return all_final_nodes
 
     # qubit reset ######################################################
     def _build_qubit_reset_process(
         self,
     ):
         reset_rot_ideal = cat_ideal.qubit_rot_propagator(
             res_dim=self.res_dim, qubit_dim=self.qubit_dim,
@@ -710,73 +850,14 @@
             # already failed
             return [self._identity]
         
     @property
     def _qubit_reset_time(self) -> float:
         return float(self.fsweep["tau_p_eff"] * 2 * (1 - self.qubit_reset_is_ideal))
         
-    def qubit_reset(
-        self,
-        step: int | str,
-        graph: EvolutionTree,
-        init_nodes: StateEnsemble,
-    ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
-
-        for node in init_nodes.active_nodes():
-            edge_qubit_reset = PropagatorEdge(
-                f"RS ({step})",
-                (
-                    self._qubit_reset_map_real 
-                    if not self.qubit_reset_is_ideal 
-                    else self._kraus_to_super(self._qubit_reset_map_ideal)
-                ),
-                self._qubit_reset_map_ideal,
-            )
-            final_nodes.append(StateNode())
-
-            graph.add_node(final_nodes[-1])
-
-            graph.add_edge_connect(
-                edge_qubit_reset,
-                node,
-                final_nodes[-1],
-            )
-
-        return final_nodes
-    
-    # check point ######################################################
-    def check_point(
-        self,
-        step: int | str,
-        graph: EvolutionTree,
-        init_nodes: StateEnsemble,
-    ) -> StateEnsemble:
-        final_nodes = StateEnsemble()
-
-        for node in init_nodes.active_nodes():
-            for success in [True, False]:
-                edge_check_point = CheckPointEdge(
-                    name = f"CP ({step})",
-                    success = success,
-                )
-                final_node = StateNode()
-                final_node.terminated = not success
-                final_nodes.append(final_node)
-
-                graph.add_node(final_nodes[-1])
-
-                graph.add_edge_connect(
-                    edge_check_point,
-                    node,
-                    final_nodes[-1],
-                )
-
-        return final_nodes
-
     # overall generation ###############################################
     def build_all_processes(
         self,
     ):
         
         builds = [
             self._build_idling_process,
```

### Comparing `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/edge.py` & `chencrafts-1.3/chencrafts/bsqubits/QEC_graph/edge.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/graph.py` & `chencrafts-1.3/chencrafts/bsqubits/QEC_graph/graph.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/QEC_graph/node.py` & `chencrafts-1.3/chencrafts/bsqubits/QEC_graph/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,15 @@
 Node = StateNode    # for now, the only node type is StateNode
 
 
 class StateEnsemble:
 
     def __init__(
         self, 
-        nodes: [List[StateNode] | None] = None,
+        nodes: List[StateNode] | None = None,
         # note: Do not use [] as the default value, it will be shared by 
         # all the instances, as it's a mutable object
     ):
         if nodes is None:
             nodes = []
         self.nodes: List[StateNode] = nodes
 
@@ -538,14 +538,20 @@
         return sum([node.probability for node in self.nodes])
     
     @property
     def state(self) -> qt.Qobj:
         """
         Calculate the total state
         """
+        for node in self.nodes:
+            try:
+                node.state
+            except AttributeError:
+                raise AttributeError(f"A node {node} has not been evolved.")
+
         if not self.is_trace_1():
             warn("The total trace is not 1. The averaged state is not "
                  "physical. \n")
         return sum([node.state for node in self.nodes])
 
     @property
     def fidelity(self) -> float:
```

### Comparing `chencrafts-1.1/chencrafts/bsqubits/__init__.py` & `chencrafts-1.3/chencrafts/bsqubits/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/batched_custom_sweeps.py` & `chencrafts-1.3/chencrafts/bsqubits/batched_custom_sweeps.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/cat_ideal.py` & `chencrafts-1.3/chencrafts/bsqubits/cat_ideal.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/cat_real.py` & `chencrafts-1.3/chencrafts/bsqubits/cat_real.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from scqubits.core.hilbert_space import HilbertSpace
 from scqubits.core.param_sweep import ParameterSweep
 from scqubits.core.namedslots_array import NamedSlotsNdarray
 
 from chencrafts.cqed.mode_assignment import two_mode_dressed_esys
 from chencrafts.cqed.qt_helper import oprt_in_basis, direct_sum
 from chencrafts.cqed.pulses import DRAGGaussian, Gaussian
+from chencrafts.settings import QUTIP_VERSION
 
 from typing import Dict, List, Tuple, Callable, Any, Literal
 import warnings
 
 Esys = Tuple[np.ndarray, np.ndarray]
 
 # ##############################################################################
@@ -438,21 +439,25 @@
         H0_ss = H0_ss - phase_quantum * cycle_num
 
         try:
             pulse.reset()
         except AttributeError:
             pass
 
+        options = dict(
+            nsteps=1000000,
+            atol=1e-10,
+        )
+        if QUTIP_VERSION[0] < 5:
+            options = qt.Options(**options)
+
         prop = qt.propagator(
             H = lambda t, args: H0_ss + H1_ss * pulse(t),
             t = pulse.duration,
-            options = qt.Options(
-                nsteps=1000000,
-                atol=1e-10,
-            ),
+            options = options,
         )
 
         return prop
     
     if num_cpus > 1:
         try:
             from multiprocess import Pool
```

### Comparing `chencrafts-1.1/chencrafts/bsqubits/derive_var.py` & `chencrafts-1.3/chencrafts/bsqubits/derive_var.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/error_rates.py` & `chencrafts-1.3/chencrafts/bsqubits/error_rates.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/pulse_utils.py` & `chencrafts-1.3/chencrafts/bsqubits/pulse_utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/bsqubits/systems.py` & `chencrafts-1.3/chencrafts/bsqubits/systems.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/__init__.py` & `chencrafts-1.3/chencrafts/cqed/__init__.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/block_diag.py` & `chencrafts-1.3/chencrafts/cqed/block_diag.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/crit_photon_num.py` & `chencrafts-1.3/chencrafts/cqed/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/custom_sweeps/crit_photon_num.py` & `chencrafts-1.3/chencrafts/cqed/custom_sweeps/crit_photon_num.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/custom_sweeps/decoherence.py` & `chencrafts-1.3/chencrafts/cqed/custom_sweeps/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/custom_sweeps/utils.py` & `chencrafts-1.3/chencrafts/cqed/custom_sweeps/utils.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/decoherence.py` & `chencrafts-1.3/chencrafts/cqed/decoherence.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/flexible_sweep.py` & `chencrafts-1.3/chencrafts/cqed/flexible_sweep.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/mode_assignment.py` & `chencrafts-1.3/chencrafts/cqed/mode_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         if drs_idx is not None:
             if drs_idx < len(evals):
                 evec = evecs[drs_idx]
                 eval = evals[drs_idx]
 
                 if adjust_phase:
                     # make the "principle_val" have zero phase
-                    principle_val = evec.data[idx, 0]
+                    principle_val = evec.full()[idx, 0]
                     principle_val_phase = (principle_val) / np.abs(principle_val)
                     evec /= principle_val_phase
         organized_evals[bare_idx] = eval
         organized_evecs[bare_idx] = evec            
 
     return organized_evals, organized_evecs
```

### Comparing `chencrafts-1.1/chencrafts/cqed/pulses.py` & `chencrafts-1.3/chencrafts/cqed/pulses.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/qt_helper.py` & `chencrafts-1.3/chencrafts/cqed/qt_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,31 +259,31 @@
 # ##############################################################################
 def normalization_factor(ket_or_dm: qt.Qobj):
     """
     Return the normalization factor (N) of a ket or a density matrix (Qobj).
     Such factor makes Qobj / N normalized.
     """
     if qt.isket(ket_or_dm):
-        return np.sqrt(((ket_or_dm.dag() * ket_or_dm).tr()).real)
+        return np.sqrt((ket_or_dm * ket_or_dm.dag()).tr()).real
     elif qt.isoper(ket_or_dm):
         return (ket_or_dm.tr()).real
     else:
         raise ValueError("The object is neither a ket nor a density matrix.")
     
 # ##############################################################################
 # direct sum
 def _direct_sum_ket(ket1: qt.Qobj, ket2: qt.Qobj) -> qt.Qobj:
     return qt.Qobj(np.concatenate((ket1.full(), ket2.full())))
 
 def _direct_sum_op(A: qt.Qobj, B: qt.Qobj) -> qt.Qobj:
     shape_A = np.array(A.shape)
     shape_B = np.array(B.shape)
 
-    A = np.pad(A, ((0, shape_B[0]), (0, shape_B[1])), mode="constant")
-    B = np.pad(B, ((shape_A[0], 0), (shape_A[1], 0)), mode="constant")
+    A = np.pad(A.full(), ((0, shape_B[0]), (0, shape_B[1])), mode="constant")
+    B = np.pad(B.full(), ((shape_A[0], 0), (shape_A[1], 0)), mode="constant")
 
     return qt.Qobj(A + B)
 
 def _direct_sum_superop(A: qt.Qobj, B: qt.Qobj) -> qt.Qobj:
     raise NotImplementedError(
         "It seems that there is no general way to direct sum two superoperators."
         "For two subsystem's evolution, their noises may be correlated, and a simple"
```

### Comparing `chencrafts-1.1/chencrafts/cqed/scq_helper.py` & `chencrafts-1.3/chencrafts/cqed/scq_helper.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/spec_poly_fit.py` & `chencrafts-1.3/chencrafts/cqed/spec_poly_fit.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/cqed/special_states.py` & `chencrafts-1.3/chencrafts/cqed/special_states.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import qutip as qt
 from typing import List, Tuple
 
 import scqubits as scq
+from chencrafts.settings import QUTIP_VERSION
 
 def coherent_coef_list(n, alpha) -> np.ndarray:
     coef = np.exp(-alpha*alpha.conjugate()/2)
     list = [coef]
     for idx in range(1, n):
         coef *= alpha / np.sqrt(idx)
         list.append(coef)
@@ -26,17 +27,21 @@
     for idx in range(1, n):
         coef *= alpha / np.sqrt(idx)
         list.append(-coef * idx**2)
     return np.array(list)
 
 def sum_of_basis(basis: List[qt.Qobj], coef_list: List[complex]) -> qt.Qobj:
     dims = basis[0].dims
-    N = np.prod(np.array(dims))
 
-    state = qt.zero_ket(N, dims=dims)
+    if QUTIP_VERSION[0] >= 5:
+        state = qt.zero_ket(dimensions=dims[0])
+    else:
+        N = np.prod(np.array(dims))
+        state = qt.zero_ket(N, dims=dims)
+
     for idx in range(len(coef_list)):
         state = state + basis[idx] * coef_list[idx]
     return state.unit()
 
 def coherent(basis: List[qt.Qobj], alpha: complex) -> qt.Qobj:
     # check all Nones
     available_dim = 0
@@ -66,14 +71,18 @@
         disp_list = [disp for phase, disp in phase_disp_pair]
         max_disp = np.max(np.abs(disp_list))
         max_n = int(max_disp**2 + 5 * max_disp)
 
         basis = [qt.fock(max_n, n) for n in range(max_n)]
 
     dims = basis[0].dims
-    N = np.prod(np.array(dims))
-    state = qt.zero_ket(N, dims=dims)
+
+    if QUTIP_VERSION[0] >= 5:
+        state = qt.zero_ket(dimensions=dims[0])
+    else:
+        N = np.prod(np.array(dims))
+        state = qt.zero_ket(N, dims=dims)
     
     for phase, disp in phase_disp_pair:
         state += phase * coherent(basis, disp)
 
     return state.unit()
```

### Comparing `chencrafts-1.1/chencrafts/cqed/symbolic_bosons.py` & `chencrafts-1.3/chencrafts/cqed/symbolic_bosons.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/projects/fluxonium_tunable_coupler.py` & `chencrafts-1.3/chencrafts/projects/fluxonium_tunable_coupler.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/projects/protomon_disorder.py` & `chencrafts-1.3/chencrafts/projects/protomon_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/projects/protomon_full_disorder.py` & `chencrafts-1.3/chencrafts/projects/protomon_full_disorder.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/settings.py` & `chencrafts-1.3/chencrafts/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,8 +11,13 @@
 
 # a switch for displaying of progress bar; default: show only in ipython
 if executed_in_ipython():
     PROGRESSBAR_DISABLED = False
     IN_IPYTHON = True
 else:
     PROGRESSBAR_DISABLED = True
-    IN_IPYTHON = False
+    IN_IPYTHON = False
+
+
+# qutip version related settings
+import qutip as qt
+QUTIP_VERSION = tuple(map(int, qt.__version__.split(".")))
```

### Comparing `chencrafts-1.1/chencrafts/toolbox/__init__.py` & `chencrafts-1.3/chencrafts/toolbox/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     dill_dump,
     dill_load,
 )
 from chencrafts.toolbox.plot import (
     color_palettes,
     color_cyclers,
     color_iters,
+    set_color_cycler,
     PiecewiseLinearNorm,
     remove_repeated_legend,
     filter,
     bar_plot_compare,
     plot_dictionary_2d
 )
 from chencrafts.toolbox.gadgets import (
@@ -73,14 +74,15 @@
     'load_variable_dict',
     'dill_dump',
     'dill_load',
 
     'color_palettes',
     'color_cyclers',
     'color_iters',
+    'set_color_cycler',
     'PiecewiseLinearNorm',
     'remove_repeated_legend',
     'filter',
     'bar_plot_compare',
     'plot_dictionary_2d',
 
     'capacitance_2_EC',
```

### Comparing `chencrafts-1.1/chencrafts/toolbox/data_processing.py` & `chencrafts-1.3/chencrafts/toolbox/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,14 +318,17 @@
         The amplitude of the decay rate.
     b: float. 
         The decay rate.
     c: float.
         The offset of the decay rate.
 
     """
+    t_array = np.array(t_array)
+    data_array = np.array(data_array)
+    
     # find the envelope of the curve using numpy
     if extract_envelope:
         top_envelope, bottom_envelope = find_envelope(data_array)
         data_array = top_envelope - bottom_envelope
 
     # find the decay rate by fitting the envelope
     fit_func = lambda x, a, b, c: a * np.exp(-b * x) + c
```

### Comparing `chencrafts-1.1/chencrafts/toolbox/gadgets.py` & `chencrafts-1.3/chencrafts/toolbox/gadgets.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/toolbox/optimize.py` & `chencrafts-1.3/chencrafts/toolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/toolbox/plot.py` & `chencrafts-1.3/chencrafts/toolbox/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 )
 color_cyclers = dict([
     (key, cycler(color = color_palettes[key])) for key in color_palettes
 ])
 color_iters = dict([
     (key, cycle(color_palettes[key])) for key in color_palettes
 ])
+def set_color_cycler(cycler_name):
+    rcParams["axes.prop_cycle"] = color_cyclers[cycler_name]
 
 def remove_repeated_legend(ax=None):
     """remove repeated legend"""
     if ax is None:
         ax = plt.gca()
     handles, labels = ax.get_legend_handles_labels()
     by_label = dict(zip(labels, handles))
```

### Comparing `chencrafts-1.1/chencrafts/toolbox/save.py` & `chencrafts-1.3/chencrafts/toolbox/save.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts/toolbox/useless.py` & `chencrafts-1.3/chencrafts/toolbox/useless.py`

 * *Files identical despite different names*

### Comparing `chencrafts-1.1/chencrafts.egg-info/PKG-INFO` & `chencrafts-1.3/chencrafts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: chencrafts
-Version: 1.1
-Summary: CHEN CRAFTS, my personal toolbox!
-Home-page: https://github.com/Harrinive/chencrafts
-Author: Danyang Chen
-Author-email: DanyangChen2026@u.northwestern.edu
-License: MIT
+Version: 1.3
+Summary: A personal toolbox for superconducting qubits and quantum mechanics.
+Author-email: Danyang Chen <DanyangChen2026@u.northwestern.edu>
+License: BSD
+Project-URL: Homepage, https://github.com/Harrinive/chencrafts
+Project-URL: Repository, https://github.com/Harrinive/chencrafts
 Keywords: personal toolbox,superconducting qubits,quantum mechanics
-Platform: Linux
-Platform: Mac OSX
-Platform: Unix
-Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: matplotlib
 Requires-Dist: scipy
-Requires-Dist: tqdm
 Requires-Dist: pandas
+Requires-Dist: tqdm
 Requires-Dist: dill
 Requires-Dist: pathos
 Requires-Dist: scqubits
 Requires-Dist: IPython
 Provides-Extra: cqed
-Requires-Dist: torch; extra == "cqed"
+Requires-Dist: torch>=1.7; extra == "cqed"
 Requires-Dist: multiprocess; extra == "cqed"
 Provides-Extra: bsqubits
-Requires-Dist: networkx; extra == "bsqubits"
+Requires-Dist: networkx>=2.4; extra == "bsqubits"
 
+CHENCRAFTS, Danyang's personal toolbox!
+=================================
 
 There are four main parts in this package: `Toolbox`, `cqed`, `bsqubits`, and `projects`. They serves for different purposes in Danyang's research.
 
 
 ## Modules
 - `Toolbox` (or `tb`): Toolbox includes functions for optimization, saving and loading data, etc. It is a general toolbox for all the projects.
```

### Comparing `chencrafts-1.1/chencrafts.egg-info/SOURCES.txt` & `chencrafts-1.3/chencrafts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+.gitignore
 LICENSE
 MANIFEST.in
 README.md
+meta.yaml
 pyproject.toml
-requirements.txt
-setup.py
+.github/workflows/publish_to_pypi.yml
 chencrafts/__init__.py
 chencrafts/py.typed
+chencrafts/pyrightconfig.json
 chencrafts/settings.py
 chencrafts/version.py
 chencrafts.egg-info/PKG-INFO
 chencrafts.egg-info/SOURCES.txt
 chencrafts.egg-info/dependency_links.txt
-chencrafts.egg-info/not-zip-safe
 chencrafts.egg-info/requires.txt
 chencrafts.egg-info/top_level.txt
 chencrafts/bsqubits/__init__.py
 chencrafts/bsqubits/batched_custom_sweeps.py
 chencrafts/bsqubits/cat_ideal.py
 chencrafts/bsqubits/cat_real.py
 chencrafts/bsqubits/derive_var.py
```

### Comparing `chencrafts-1.1/tests/test_optimization.py` & `chencrafts-1.3/tests/test_optimization.py`

 * *Files identical despite different names*

