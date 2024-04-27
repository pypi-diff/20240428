# Comparing `tmp/oresat-configs-0.4.0.tar.gz` & `tmp/oresat_configs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-configs-0.4.0.tar", last modified: Thu Mar  7 04:52:28 2024, max compression
+gzip compressed data, was "oresat_configs-0.5.0.tar", last modified: Sat Apr 27 22:33:19 2024, max compression
```

## Comparing `oresat-configs-0.4.0.tar` & `oresat_configs-0.5.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.925583 oresat-configs-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/build_and_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/docs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/oresat0/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/docs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/oresat0_5/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/docs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/oresat1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.929583 oresat-configs-0.4.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/scripts/gen_beacon_rst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.933583 oresat-configs-0.4.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.933583 oresat-configs-0.4.0/docs/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/yamls/beacon_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/yamls/card_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/docs/yamls/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.933583 oresat-configs-0.4.0/oresat_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/_yaml_to_od.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.937583 oresat-configs-0.4.0/oresat_configs/base/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/battery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/cfc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/dxwifi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/fw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/gps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/imu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/reaction_wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/solar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/star_tracker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/base/sw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/beacon_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/card_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/card_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/cards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.937583 oresat-configs-0.4.0/oresat_configs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat0/battery_overlay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat0/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.937583 oresat-configs-0.4.0/oresat_configs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat0_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat0_5/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.937583 oresat-configs-0.4.0/oresat_configs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/oresat1/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/oresat_configs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/gen_dbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/gen_dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/gen_fw_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/gen_xtce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/list_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/pdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/print_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/scripts/sdo_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/oresat_configs/standard_objects.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/oresat_configs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-07 04:52:28.000000 oresat-configs-0.4.0/oresat_configs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:52:28.941583 oresat-configs-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/tests/test_config_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/tests/test_oresat0.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/tests/test_oresat0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-07 04:52:14.000000 oresat-configs-0.4.0/tests/test_oresat1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.690468 oresat_configs-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/build_and_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat0_5/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/scripts/gen_beacon_rst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/beacon_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/card_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/_yaml_to_od.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/adcs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/battery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/cfc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/diode_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/dxwifi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/fw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/gps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/reaction_wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/solar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/star_tracker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/sw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/beacon_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/card_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/card_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/cards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/battery_overlay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0_5/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat1/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_dbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25953 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_fw_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_xtce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/list_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/pdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/print_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/sdo_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/standard_objects.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_config_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat1.py
```

### Comparing `oresat-configs-0.4.0/.github/workflows/pypi.yaml` & `oresat_configs-0.5.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/.github/workflows/tests.yaml` & `oresat_configs-0.5.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/.gitignore` & `oresat_configs-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/LICENSE` & `oresat_configs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/PKG-INFO` & `oresat_configs-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.4.0
+Version: 0.5.0
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat-configs-0.4.0/README.md` & `oresat_configs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/docs/Makefile` & `oresat_configs-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/docs/conf.py` & `oresat_configs-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/docs/make.bat` & `oresat_configs-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/docs/scripts/gen_beacon_rst.py` & `oresat_configs-0.5.0/docs/scripts/gen_beacon_rst.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/docs/yamls/card_config.rst` & `oresat_configs-0.5.0/docs/yamls/card_config.rst`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/__init__.py` & `oresat_configs-0.5.0/oresat_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/__main__.py` & `oresat_configs-0.5.0/oresat_configs/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/_yaml_to_od.py` & `oresat_configs-0.5.0/oresat_configs/_yaml_to_od.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/__init__.py` & `oresat_configs-0.5.0/oresat_configs/base/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 
 _CONFIGS_DIR = os.path.dirname(os.path.abspath(__file__))
 FW_COMMON_CONFIG_PATH = f"{_CONFIGS_DIR}/fw_common.yaml"
 SW_COMMON_CONFIG_PATH = f"{_CONFIGS_DIR}/sw_common.yaml"
 C3_CONFIG_PATH = f"{_CONFIGS_DIR}/c3.yaml"
 BAT_CONFIG_PATH = f"{_CONFIGS_DIR}/battery.yaml"
 SOLAR_CONFIG_PATH = f"{_CONFIGS_DIR}/solar.yaml"
-IMU_CONFIG_PATH = f"{_CONFIGS_DIR}/imu.yaml"
+ADCS_CONFIG_PATH = f"{_CONFIGS_DIR}/adcs.yaml"
 RW_CONFIG_PATH = f"{_CONFIGS_DIR}/reaction_wheel.yaml"
 GPS_CONFIG_PATH = f"{_CONFIGS_DIR}/gps.yaml"
 ST_CONFIG_PATH = f"{_CONFIGS_DIR}/star_tracker.yaml"
 DXWIFI_CONFIG_PATH = f"{_CONFIGS_DIR}/dxwifi.yaml"
 CFC_CONFIG_PATH = f"{_CONFIGS_DIR}/cfc.yaml"
+DIODE_CONFIG_PATH = f"{_CONFIGS_DIR}/diode_test.yaml"
```

### Comparing `oresat-configs-0.4.0/oresat_configs/base/battery.yaml` & `oresat_configs-0.5.0/oresat_configs/base/battery.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/c3.yaml` & `oresat_configs-0.5.0/oresat_configs/base/c3.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/cfc.yaml` & `oresat_configs-0.5.0/oresat_configs/base/cfc.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/dxwifi.yaml` & `oresat_configs-0.5.0/oresat_configs/base/dxwifi.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     access_type: rw
     value_descriptions:
       'off': 0
       boot: 1
       standby: 2
       film: 3
       transmit: 4
+      purge: 5
       error: 0xff
 
   - index: 0x4001
     name: radio
     object_type: record
     subindexes:
       - subindex: 0x1
```

### Comparing `oresat-configs-0.4.0/oresat_configs/base/fw_common.yaml` & `oresat_configs-0.5.0/oresat_configs/base/fw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/gps.yaml` & `oresat_configs-0.5.0/oresat_configs/base/gps.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/imu.yaml` & `oresat_configs-0.5.0/oresat_configs/base/adcs.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -47,29 +47,32 @@
     object_type: record
     subindexes:
       - subindex: 0x1
         name: x
         data_type: int16
         description: x acceleration
         access_type: ro
-        unit: milli-g
+        unit: g
+        scale_factor: 0.001
 
       - subindex: 0x2
         name: y
         data_type: int16
         description: y acceleration
         access_type: ro
-        unit: milli-g
+        unit: g
+        scale_factor: 0.001
 
       - subindex: 0x3
         name: z
         data_type: int16
         description: z acceleration
-        unit: milli-g
+        unit: g
         access_type: ro
+        scale_factor: 0.001
 
       - subindex: 0x4
         name: x_raw
         data_type: uint16
         description: raw x acceleration value
         access_type: ro
 
@@ -100,169 +103,181 @@
       - subindex: 0x1
         name: x
         data_type: int16
         description: +z mag 1 x-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x2
         name: y
         data_type: int16
         description: +z mag 1 y-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x3
         name: z
         data_type: int16
         description: +z mag 1 z-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
   - index: 0x4004
     name: pos_z_magnetometer_2
     object_type: record
     description: +z endcard magnetometer 2 data
     subindexes:
       - subindex: 0x1
         name: x
         data_type: int16
         description: +z mag 2 x-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x2
         name: y
         data_type: int16
         description: +z mag 2 y-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x3
         name: z
         data_type: int16
         description: +z mag 2 z-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
   - index: 0x4005
     name: min_z_magnetometer_1
     object_type: record
     description: -z endcard magnetometer 1 data
     subindexes:
       - subindex: 0x1
         name: x
         data_type: int16
         description: -z mag 1 x-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x2
         name: y
         data_type: int16
         description: -z mag 1 y-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x3
         name: z
         data_type: int16
         description: -z mag 1 z-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
   - index: 0x4006
     name: min_z_magnetometer_2
     object_type: record
     description: -z endcard magnetometer 2 data
     subindexes:
       - subindex: 0x1
         name: x
         data_type: int16
         description: -z mag 2 x-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x2
         name: y
         data_type: int16
         description: -z mag 2 y-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
       - subindex: 0x3
         name: z
         data_type: int16
         description: -z mag 2 z-axis magnetic field
         access_type: ro
         low_limit: -8192
         high_limit: 8192
-        unit: milligauss
+        unit: gauss
+        scale_factor: 0.001
 
   - index: 0x4007
     name: magnetorquer
     object_type: record
     subindexes:
       - subindex: 0x1
         name: current_x
         data_type: int32
         description: current feedback in the x-axis
         access_type: ro
         unit: uA
-        
+
       - subindex: 0x2
         name: current_y
         data_type: int32
         description: current feedback in the y-axis
         access_type: ro
         unit: uA
-        
+
       - subindex: 0x3
         name: current_z
         data_type: int32
         description: current feedback in the y-axis
         access_type: ro
         unit: uA
 
       - subindex: 0x4
         name: current_x_setpoint
         data_type: int32
         description: Setpoint for current in thex x-axis
         access_type: rw
         unit: uA
-        
+
       - subindex: 0x5
         name: current_y_setpoint
         data_type: int32
         description: Setpoint for current in the y-axis
         access_type: rw
         unit: uA
-        
+
       - subindex: 0x6
         name: current_z_setpoint
         data_type: int32
         description: Setpoint for current in thex z-axis
         access_type: rw
         unit: uA
 
@@ -345,19 +360,19 @@
     event_timer_ms: 1000
 
   - num: 8
     fields:
       - [magnetorquer, current_x]
       - [magnetorquer, pwm_x]
     event_timer_ms: 1000
-    
+
   - num: 9
     fields:
       - [magnetorquer, current_y]
-      - [magnetorquer, pwm_z]
+      - [magnetorquer, pwm_y]
     event_timer_ms: 1000
 
   - num: 10
     fields:
       - [magnetorquer, current_z]
       - [magnetorquer, pwm_z]
     event_timer_ms: 1000
```

### Comparing `oresat-configs-0.4.0/oresat_configs/base/solar.yaml` & `oresat_configs-0.5.0/oresat_configs/base/solar.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/star_tracker.yaml` & `oresat_configs-0.5.0/oresat_configs/base/star_tracker.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/base/sw_common.yaml` & `oresat_configs-0.5.0/oresat_configs/base/sw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/beacon_config.py` & `oresat_configs-0.5.0/oresat_configs/beacon_config.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/card_config.py` & `oresat_configs-0.5.0/oresat_configs/card_config.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/card_info.py` & `oresat_configs-0.5.0/oresat_configs/card_info.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/cards.csv` & `oresat_configs-0.5.0/oresat_configs/cards.csv`

 * *Files 10% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 rw_1,Reaction Wheel 1,0x3C,stm32,0x20,false,
 rw_2,Reaction Wheel 2,0x40,stm32,0x21,false,
 rw_3,Reaction Wheel 3,0x44,stm32,0x22,false,
 rw_4,Reaction Wheel 4,0x48,stm32,0x23,false,
 dxwifi,DxWiFi,0x4C,octavo,0x1B,false,
 cfc_processor,CFC Processor,0x50,octavo,0x1D,false,cfc_sensor
 cfc_sensor,CFC Sensor,0x0,none,0x1E,false,
+diode_test,Diode Test,0x54,stm32,0x11,false,
```

### Comparing `oresat-configs-0.4.0/oresat_configs/constants.py` & `oresat_configs-0.5.0/oresat_configs/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,14 @@
     SOLAR_MODULE_5 = 0x1C
     SOLAR_MODULE_6 = 0x20
     SOLAR_MODULE_7 = 0x24
     SOLAR_MODULE_8 = 0x28
     STAR_TRACKER_1 = 0x2C
     STAR_TRACKER_2 = 0x30
     GPS = 0x34
-    IMU = 0x38
+    ADCS = 0x38
     REACTION_WHEEL_1 = 0x3C
     REACTION_WHEEL_2 = 0x40
     REACTION_WHEEL_3 = 0x44
     REACTION_WHEEL_4 = 0x48
     DXWIFI = 0x4C
     CFC = 0x50
```

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat0/__init__.py` & `oresat_configs-0.5.0/oresat_configs/oresat0/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """OreSat0 object dictionary and beacon constants."""
 
 import os
 
 from ..base import (
+    ADCS_CONFIG_PATH,
     BAT_CONFIG_PATH,
     C3_CONFIG_PATH,
     DXWIFI_CONFIG_PATH,
     FW_COMMON_CONFIG_PATH,
     GPS_CONFIG_PATH,
-    IMU_CONFIG_PATH,
     SOLAR_CONFIG_PATH,
     ST_CONFIG_PATH,
     SW_COMMON_CONFIG_PATH,
     ConfigPaths,
 )
 
 _CONFIGS_DIR = os.path.dirname(os.path.abspath(__file__))
@@ -24,12 +24,12 @@
 CARD_CONFIGS_PATH: ConfigPaths = {
     "c3": (C3_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "battery_1": (BAT_CONFIG_PATH, FW_COMMON_CONFIG_PATH, BAT_OVERLAY_CONFIG_PATH),
     "solar_1": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_2": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_3": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_4": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
-    "adcs": (IMU_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
+    "adcs": (ADCS_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "gps": (GPS_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "star_tracker_1": (ST_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "dxwifi": (DXWIFI_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
 }
```

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat0/battery_overlay.yaml` & `oresat_configs-0.5.0/oresat_configs/oresat0/battery_overlay.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat0/beacon.yaml` & `oresat_configs-0.5.0/oresat_configs/oresat0/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat0_5/__init__.py` & `oresat_configs-0.5.0/oresat_configs/oresat0_5/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """OreSat0.5 object dictionary and beacon constants."""
 
 import os
 
 from ..base import (
+    ADCS_CONFIG_PATH,
     BAT_CONFIG_PATH,
     C3_CONFIG_PATH,
     CFC_CONFIG_PATH,
+    DIODE_CONFIG_PATH,
     DXWIFI_CONFIG_PATH,
     FW_COMMON_CONFIG_PATH,
     GPS_CONFIG_PATH,
-    IMU_CONFIG_PATH,
     RW_CONFIG_PATH,
     SOLAR_CONFIG_PATH,
     ST_CONFIG_PATH,
     SW_COMMON_CONFIG_PATH,
     ConfigPaths,
 )
 
@@ -26,18 +27,19 @@
     "battery_1": (BAT_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_1": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_2": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_3": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_4": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_5": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_6": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
-    "adcs": (IMU_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
+    "adcs": (ADCS_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_1": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_2": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_3": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_4": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "gps": (GPS_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "star_tracker_1": (ST_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "dxwifi": (DXWIFI_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "cfc_processor": (CFC_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "cfc_sensor": None,
+    "diode_test": (DIODE_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
 }
```

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat0_5/beacon.yaml` & `oresat_configs-0.5.0/oresat_configs/oresat0_5/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/oresat1/__init__.py` & `oresat_configs-0.5.0/oresat_configs/oresat1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """OreSat1 object dictionary and beacon constants."""
 
 import os
 
 from ..base import (
+    ADCS_CONFIG_PATH,
     BAT_CONFIG_PATH,
     C3_CONFIG_PATH,
     CFC_CONFIG_PATH,
     DXWIFI_CONFIG_PATH,
     FW_COMMON_CONFIG_PATH,
     GPS_CONFIG_PATH,
-    IMU_CONFIG_PATH,
     RW_CONFIG_PATH,
     SOLAR_CONFIG_PATH,
     ST_CONFIG_PATH,
     SW_COMMON_CONFIG_PATH,
     ConfigPaths,
 )
 
@@ -29,15 +29,15 @@
     "solar_2": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_3": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_4": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_5": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_6": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_7": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "solar_8": (SOLAR_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
-    "adcs": (IMU_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
+    "adcs": (ADCS_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_1": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_2": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_3": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "rw_4": (RW_CONFIG_PATH, FW_COMMON_CONFIG_PATH),
     "gps": (GPS_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "star_tracker_1": (ST_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
     "star_tracker_2": (ST_CONFIG_PATH, SW_COMMON_CONFIG_PATH),
```

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/gen_dbc.py` & `oresat_configs-0.5.0/oresat_configs/scripts/gen_dbc.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/gen_dcf.py` & `oresat_configs-0.5.0/oresat_configs/scripts/gen_dcf.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/gen_fw_files.py` & `oresat_configs-0.5.0/oresat_configs/scripts/gen_fw_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     parser.add_argument(
         "--oresat",
         default=Consts.default().arg,
         choices=[m.arg for m in Consts],
         type=lambda x: x.lower().removeprefix("oresat"),
         help="oresat mission, defaults to %(default)s",
     )
-    parser.add_argument("card", help="card name; c3, battery, solar, imu, or reaction_wheel")
+    parser.add_argument(
+        "card", help="card name; c3, battery, solar, adcs, reaction_wheel, or diode_test"
+    )
     parser.add_argument("-d", "--dir-path", default=".", help='output directory path, default: "."')
     return parser
 
 
 def register_subparser(subparsers: Any) -> None:
     """Registers an ArgumentParser as a subcommand of another parser.
 
@@ -191,14 +193,16 @@
                 line += f"0x{ord(i):04X}, "
             line += f"0x{0:04X}"  # add the '\0'
             line += "},"
         elif obj.data_type in canopen.objectdictionary.datatypes.INTEGER_TYPES:
             line += f"0x{obj.default:X},"
         elif obj.data_type == canopen.objectdictionary.datatypes.BOOLEAN:
             line += f"{int(obj.default)},"
+        elif obj.data_type in canopen.objectdictionary.datatypes.FLOAT_TYPES:
+            line += f"{obj.default},"
         else:
             line += f"{remove_node_id(obj.default)},"
 
         if index not in _SKIP_INDEXES:
             lines.append(line)
     elif isinstance(obj, canopen.objectdictionary.Array):
         name = format_name(obj.name)
@@ -278,14 +282,16 @@
                 line += f"0x{0:04X}"  # add the '\0'
                 line += "},"
                 lines.append(line)
             elif obj[i].data_type in canopen.objectdictionary.datatypes.INTEGER_TYPES:
                 lines.append(f"{INDENT8}.{name} = 0x{obj[i].default:X},")
             elif obj[i].data_type == canopen.objectdictionary.datatypes.BOOLEAN:
                 lines.append(f"{INDENT8}.{name} = {int(obj[i].default)},")
+            elif obj[i].data_type in canopen.objectdictionary.datatypes.FLOAT_TYPES:
+                lines.append(f"{INDENT8}.{name} = {obj[i].default},")
             else:
                 lines.append(f"{INDENT8}.{name} = {remove_node_id(obj[i].default)},")
 
         lines.append(INDENT4 + "},")
 
     return lines
 
@@ -680,14 +686,16 @@
         od = config.od_db["solar_1"]
     elif arg_card in ["battery", "bat"]:
         od = config.od_db["battery_1"]
     elif arg_card in ["imu", "adcs"]:
         od = config.od_db["adcs"]
     elif arg_card in ["rw", "reaction_wheel"]:
         od = config.od_db["rw_1"]
+    elif arg_card in ["diode", "diode_test"]:
+        od = config.od_db["diode_test"]
     elif arg_card == "base":
         od = config.fw_base_od
     else:
         print(f"invalid oresat card: {args.card}")
         sys.exit()
 
     write_canopennode(od, args.dir_path)
```

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/gen_xtce.py` & `oresat_configs-0.5.0/oresat_configs/scripts/gen_xtce.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/list_cards.py` & `oresat_configs-0.5.0/oresat_configs/scripts/list_cards.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/pdo.py` & `oresat_configs-0.5.0/oresat_configs/scripts/pdo.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/print_od.py` & `oresat_configs-0.5.0/oresat_configs/scripts/print_od.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/scripts/sdo_transfer.py` & `oresat_configs-0.5.0/oresat_configs/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs/standard_objects.yaml` & `oresat_configs-0.5.0/oresat_configs/standard_objects.yaml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/oresat_configs.egg-info/PKG-INFO` & `oresat_configs-0.5.0/oresat_configs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.4.0
+Version: 0.5.0
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat-configs-0.4.0/oresat_configs.egg-info/SOURCES.txt` & `oresat_configs-0.5.0/oresat_configs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 oresat_configs.egg-info/PKG-INFO
 oresat_configs.egg-info/SOURCES.txt
 oresat_configs.egg-info/dependency_links.txt
 oresat_configs.egg-info/entry_points.txt
 oresat_configs.egg-info/requires.txt
 oresat_configs.egg-info/top_level.txt
 oresat_configs/base/__init__.py
+oresat_configs/base/adcs.yaml
 oresat_configs/base/battery.yaml
 oresat_configs/base/c3.yaml
 oresat_configs/base/cfc.yaml
+oresat_configs/base/diode_test.yaml
 oresat_configs/base/dxwifi.yaml
 oresat_configs/base/fw_common.yaml
 oresat_configs/base/gps.yaml
-oresat_configs/base/imu.yaml
 oresat_configs/base/reaction_wheel.yaml
 oresat_configs/base/solar.yaml
 oresat_configs/base/star_tracker.yaml
 oresat_configs/base/sw_common.yaml
 oresat_configs/oresat0/__init__.py
 oresat_configs/oresat0/battery_overlay.yaml
 oresat_configs/oresat0/beacon.yaml
```

### Comparing `oresat-configs-0.4.0/pyproject.toml` & `oresat_configs-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/tests/__init__.py` & `oresat_configs-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-configs-0.4.0/tests/test_config_types.py` & `oresat_configs-0.5.0/tests/test_config_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """Tests all the card configs, with dataclass CardConfig"""
         card_paths = [
             base.FW_COMMON_CONFIG_PATH,
             base.SW_COMMON_CONFIG_PATH,
             base.C3_CONFIG_PATH,
             base.BAT_CONFIG_PATH,
             base.SOLAR_CONFIG_PATH,
-            base.IMU_CONFIG_PATH,
+            base.ADCS_CONFIG_PATH,
             base.RW_CONFIG_PATH,
             base.GPS_CONFIG_PATH,
             base.ST_CONFIG_PATH,
             base.DXWIFI_CONFIG_PATH,
             base.CFC_CONFIG_PATH,
             oresat0.BAT_OVERLAY_CONFIG_PATH,
         ]
```

