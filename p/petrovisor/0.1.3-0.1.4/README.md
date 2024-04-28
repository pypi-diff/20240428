# Comparing `tmp/petrovisor-0.1.3.tar.gz` & `tmp/petrovisor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrovisor-0.1.3.tar", last modified: Sat Apr 13 05:33:43 2024, max compression
+gzip compressed data, was "petrovisor-0.1.4.tar", last modified: Sun Apr 28 10:46:02 2024, max compression
```

## Comparing `petrovisor-0.1.3.tar` & `petrovisor-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-13 05:33:38.000000 petrovisor-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-13 05:33:43.569536 petrovisor-0.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-04-13 05:33:38.000000 petrovisor-0.1.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-13 05:33:38.000000 petrovisor-0.1.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-04-13 05:33:43.573536 petrovisor-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-04-13 05:33:38.000000 petrovisor-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.561536 petrovisor-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/api/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/increments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/internal_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    48356 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/pivot_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/psharp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/reference_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    63537 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/workspace_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/protocols/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/datastructs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/requests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2637 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/petrovisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_entities_and_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_reference_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.873441 petrovisor-0.1.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-28 10:45:58.000000 petrovisor-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-28 10:46:02.873441 petrovisor-0.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-04-28 10:45:58.000000 petrovisor-0.1.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-28 10:45:58.000000 petrovisor-0.1.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-28 10:46:02.873441 petrovisor-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-04-28 10:45:58.000000 petrovisor-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.861441 petrovisor-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.865441 petrovisor-0.1.4/src/petrovisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.865441 petrovisor-0.1.4/src/petrovisor/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.865441 petrovisor-0.1.4/src/petrovisor/api/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/increments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/internal_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/enums/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.869441 petrovisor-0.1.4/src/petrovisor/api/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29822 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48466 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/pivot_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/psharp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/reference_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60533 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/methods/workspace_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.869441 petrovisor-0.1.4/src/petrovisor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/entity_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/models/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.869441 petrovisor-0.1.4/src/petrovisor/api/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/protocols/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.869441 petrovisor-0.1.4/src/petrovisor/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/datastructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/api/utils/validators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2705 2024-04-28 10:45:58.000000 petrovisor-0.1.4/src/petrovisor/petrovisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.873441 petrovisor-0.1.4/src/petrovisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-28 10:46:02.000000 petrovisor-0.1.4/src/petrovisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-28 10:46:02.000000 petrovisor-0.1.4/src/petrovisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:46:02.000000 petrovisor-0.1.4/src/petrovisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 10:46:02.000000 petrovisor-0.1.4/src/petrovisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 10:46:02.000000 petrovisor-0.1.4/src/petrovisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:46:02.873441 petrovisor-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 10:45:58.000000 petrovisor-0.1.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-28 10:45:58.000000 petrovisor-0.1.4/tests/test_entities_and_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-28 10:45:58.000000 petrovisor-0.1.4/tests/test_reference_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-28 10:45:58.000000 petrovisor-0.1.4/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-28 10:45:58.000000 petrovisor-0.1.4/tests/test_units.py
```

### Comparing `petrovisor-0.1.3/LICENSE` & `petrovisor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/PKG-INFO` & `petrovisor-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.3/README.md` & `petrovisor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/pyproject.toml` & `petrovisor-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/setup.cfg` & `petrovisor-0.1.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/base.py` & `petrovisor-0.1.4/src/petrovisor/api/base.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/dtypes/data_grids.py` & `petrovisor-0.1.4/src/petrovisor/api/enums/data_grids.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/dtypes/increments.py` & `petrovisor-0.1.4/src/petrovisor/api/enums/increments.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/dtypes/items.py` & `petrovisor-0.1.4/src/petrovisor/api/enums/items.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/dtypes/ml.py` & `petrovisor-0.1.4/src/petrovisor/api/enums/ml.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/data_grids.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/data_grids.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/dataframes.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import io
 import re
 import copy
 from datetime import datetime
 import pandas as pd
 
-from petrovisor.api.dtypes.internal_dtypes import SignalType
+from petrovisor.api.enums.internal_dtypes import SignalType
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsSignalsRequests,
     SupportsEntitiesRequests,
     SupportsDataFrames,
 )
 
@@ -475,15 +475,18 @@
             if column_name == date_col:
                 date_index = i
                 break
 
         # 'Depth' column
         depth_index = None
         for i, column_name in enumerate(col_names):
-            if column_name == depth_col:
+            if (
+                column_name == depth_col
+                or self.get_column_name_without_unit(column_name) == depth_col
+            ):
                 depth_index = i
                 break
 
         # get signal info
         def _get_signal_info(
             column_name: str, signal_names: List[str], signals: Optional[Dict] = None
         ):
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/files.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/files.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/items.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,19 @@
     Any,
     Optional,
     Union,
     List,
     Dict,
 )
 
-from petrovisor.api.dtypes.items import ItemType
+import time
+
+from petrovisor.api.enums.items import ItemType
 from petrovisor.api.utils.helper import ApiHelper
+from petrovisor.api.utils.requests import ApiRequests
 from petrovisor.api.protocols.protocols import SupportsRequests
 
 
 # Items API calls
 class ItemsMixin(SupportsRequests):
     """
     Items API calls
@@ -85,15 +88,20 @@
         if not route:
             raise ValueError(
                 f"PetroVisor::delete_item(): "
                 f"unknown item type: '{item_type}'. "
                 f"Known item types: {list(self.ItemRoutes.keys())}"
             )
         name = self.get_item_name(item, **kwargs)
-        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        # make sure item is really deleted
+        waiting_time = 3  # in seconds
+        while self.item_exists(ItemType.RefTable, name):
+            self.delete(f"{route}/{self.encode(name)}", **kwargs)
+            time.sleep(waiting_time)
+        return ApiRequests.success()
 
     # add or edit item
     def add_item(self, item_type: str, item: Dict, **kwargs) -> Any:
         """
         Add or edit item
 
         Parameters
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/logs.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/logs.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/ml.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/ml.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     Union,
     List,
     Dict,
 )
 
 from uuid import UUID
 
-from petrovisor.api.dtypes.items import ItemType
-from petrovisor.api.dtypes.ml import (
+from petrovisor.api.enums.items import ItemType
+from petrovisor.api.enums.ml import (
     MLModelType,
     MLNormalizationType,
 )
+from petrovisor.api.utils.validators import Validator
 from petrovisor.api.utils.helper import ApiHelper
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
     SupportsPsharpRequests,
 )
 
@@ -505,75 +506,22 @@
         Get ML Model Type
 
         Parameters
         ----------
         type : str, MLModelType
             ML Model type
         """
-        if isinstance(type, MLModelType):
-            return type
-        # prepare name for comparison
-        type = ApiHelper.get_comparison_string(type, **kwargs)
-        if type in ("regression", "reg"):
-            return MLModelType.Regression
-        elif type in ("binaryclassification", "binaryclass", "binclass", "bin"):
-            return MLModelType.BinaryClassification
-        elif type in (
-            "multipleclassification",
-            "multiclassification",
-            "multipleclass",
-            "multiclass",
-            "multiple",
-            "multi",
-        ):
-            return MLModelType.MultipleClassification
-        elif type in ("clustering", "cluster"):
-            return MLModelType.Clustering
-        elif type in ("naivebayes", "bayes"):
-            return MLModelType.NaiveBayes
-        elif type in ("naivebayescategorical", "bayescategorical"):
-            return MLModelType.NaiveBayesCategorical
-        raise ValueError(
-            f"PetroVisor::get_ml_model_enum(): "
-            f"unknown data type: '{type}'! "
-            f"Should be one of: {[t.name for t in MLModelType]}"
-        )
+        return Validator.get_ml_model_type_enum(type, **kwargs)
 
     # get ML Normalization Type enum
     def get_ml_normalization_type_enum(
         self, type: Union[str, MLNormalizationType], **kwargs
     ) -> MLNormalizationType:
         """
         Get ML Normalization Type
 
         Parameters
         ----------
         type : str, MLNormalizationType
             ML Normalization type
         """
-        if isinstance(type, MLNormalizationType):
-            return type
-        # prepare name for comparison
-        type = ApiHelper.get_comparison_string(type, **kwargs)
-        if type in ("auto", "automatic"):
-            return MLNormalizationType.Auto
-        elif type in ("minmax",):
-            return MLNormalizationType.MinMax
-        elif type in ("meanvariance", "meanvar"):
-            return MLNormalizationType.MeanVariance
-        elif type in ("logmeanvariance", "logmeanvar"):
-            return MLNormalizationType.LogMeanVariance
-        elif type in ("binning", "bin"):
-            return MLNormalizationType.Binning
-        elif type in ("supervisedbinning", "supervisedbin", "superbin"):
-            return MLNormalizationType.SupervisedBinning
-        elif type in ("robustscaling", "robust"):
-            return MLNormalizationType.RobustScaling
-        elif type in ("lpnorm", "lp"):
-            return MLNormalizationType.LpNorm
-        elif type in ("globalcontrast", "contrast"):
-            return MLNormalizationType.GlobalContrast
-        raise ValueError(
-            f"PetroVisor::get_ml_normalization_enum(): "
-            f"unknown data type: '{type}'! "
-            f"Should be one of: {[t.name for t in MLNormalizationType]}"
-        )
+        return Validator.get_ml_normalization_type_enum(type, **kwargs)
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/pivot_tables.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/pivot_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import (
     Any,
     Optional,
     Union,
     Dict,
 )
 import warnings
+import time
 
 from petrovisor.api.utils.helper import ApiHelper
 from petrovisor.api.utils.requests import ApiRequests
-from petrovisor.api.dtypes.items import ItemType
+from petrovisor.api.enums.items import ItemType
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
     SupportsSignalsRequests,
     SupportsDataFrames,
 )
 
@@ -178,8 +179,12 @@
         ----------
         name : str
             Pivot table name
         """
         route = "PivotTables"
         if not self.item_exists(ItemType.PivotTable, name):
             return ApiRequests.success()
-        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        # delete data
+        self.delete_pivot_table_data(name)
+        # delete item
+        self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        return ApiRequests.success()
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/psharp.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/psharp.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/reference_tables.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/reference_tables.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,40 +2,46 @@
     Any,
     Optional,
     Union,
     List,
     Dict,
 )
 
+import warnings
 from datetime import datetime
 import time
 import pandas as pd
 import numpy as np
 from pandas.api.types import (
     is_bool_dtype,
     is_numeric_dtype,
     is_string_dtype,
     is_datetime64_dtype,
 )
 
-from petrovisor.api.dtypes.internal_dtypes import RefTableColumnType
+from petrovisor.api.enums.internal_dtypes import RefTableColumnType
 from petrovisor.api.utils.helper import ApiHelper
 from petrovisor.api.utils.requests import ApiRequests
-from petrovisor.api.dtypes.items import ItemType
+from petrovisor.api.enums.items import ItemType
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
     SupportsSignalsRequests,
+    SupportsUnitsRequests,
     SupportsDataFrames,
 )
 
 
 # Reference Table API calls
 class RefTableMixin(
-    SupportsDataFrames, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests
+    SupportsDataFrames,
+    SupportsSignalsRequests,
+    SupportsItemRequests,
+    SupportsUnitsRequests,
+    SupportsRequests,
 ):
     """
     Reference Table API calls
     """
 
     # get reference table names
     def get_ref_table_names(self, **kwargs) -> Any:
@@ -50,14 +56,26 @@
         Get reference table data info
 
         Parameters
         ----------
         name : str
             Reference table name
         """
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            waiting_time = 3  # in seconds
+            max_retries = 10
+            i = 0
+            item = self.get_item(ItemType.RefTable, name, **kwargs)
+            while not item and i < max_retries:
+                time.sleep(waiting_time)
+                item = self.get_item(ItemType.RefTable, name, **kwargs)
+                i += 1
+        if item:
+            return item
         return self.get_item(ItemType.RefTable, name, **kwargs)
 
     # add reference table
     def add_ref_table(
         self,
         name: str,
         df: Union[pd.DataFrame, Dict],
@@ -74,115 +92,174 @@
         If reference table already exists the provided DataFrame should follow the exact same schema.
 
         Parameters
         ----------
         name : str
             Reference table name
         df : DataFrame, dict
-            DataFrame or dictionary, where keys are column names and values are column values or predefined types, such as 'str', 'float', 'bool', 'datetime64[s]'.
+            DataFrame or dictionary, where keys are column names and values are column values or predefined types,
+            such as 'str', 'float', 'bool', 'datetime64[s]'.
         description : str, default None
             Reference table description
         key_col : str, default 'Key'
             Key column name
         date_col : str, default None
-            Date column name. Default names 'Date' (compatible with date column in P# table), 'Timestamp' (compatible with the internal time column name in RefTable), 'Time' (typically used as displayed name)
+            Date column name. Default names
+            'Date' (compatible with date column in P# table),
+            'Timestamp' (compatible with the internal time column name in RefTable),
+            'Time' (typically used as displayed name)
         entity_col : str, default 'Entity'
             Entity column name
         skip_existing_data : bool, default False
             Whether to skip or overwrite existing data that has same combination of 'Entity', 'Timestamp', 'Key'
         chunksize : int, default None
             Chunk size for splitting request into multiple smaller requests.
         """
         if isinstance(df, dict):
             df = RefTableMixinHelper.create_dataframe(df)
 
         # add definition if it doesn't exists
         is_empty = df.empty
         if not self.item_exists(ItemType.RefTable, name):
 
-            # date column
-            df_date_cols = set()
-            for col in RefTableMixinHelper.get_set(
-                date_col, default={"Date", "Timestamp", "Time"}
-            ):
-                if col in df.columns:
-                    df_date_cols.add(col)
-            if "Timestamp" in df_date_cols:
-                df_date_col = "Timestamp"
-            elif "Date" in df_date_cols:
-                df_date_col = "Date"
-            elif "Time" in df_date_cols:
-                df_date_col = "Time"
-            else:
-                df_date_col = df_date_cols.pop() if df_date_cols else None
+            df_columns = list(df.columns)
+            df_columns_without_unit = [
+                self.get_column_name_without_unit(col) for col in df.columns
+            ]
+            index_columns = []
+
+            def get_column_by_name(name, columns):
+                for idx, col in enumerate(columns):
+                    if self.get_column_name_without_unit(col) == name:
+                        return col
+                return None
 
             # entity column
-            df_entity_cols = set()
-            for col in RefTableMixinHelper.get_set(entity_col, default="Entity"):
-                if col in df.columns:
-                    df_entity_cols.add(col)
-            if "Entity" in df_entity_cols:
-                df_entity_col = "Entity"
+            df_entity_col = None
+            for col in RefTableMixinHelper.get_list(entity_col, default="Entity"):
+                if col in df_columns:
+                    df_entity_col = col
+                    index_columns.append(df_entity_col)
+                    break
+            if df_entity_col is None:
+                if len(df_columns) <= len(index_columns):
+                    raise ValueError(
+                        "PetroVisor::add_ref_table(): 'Entity' column is not specified"
+                    )
+                df_entity_col = df_columns[len(index_columns)]
+                index_columns.append(df_entity_col)
             else:
-                df_entity_col = df_entity_cols.pop() if df_entity_cols else None
+                # put index columns in front
+                df_columns = [
+                    *index_columns,
+                    *[col for col in df_columns if col not in index_columns],
+                ]
 
-            # key column
-            df_key_cols = set()
-            for col in RefTableMixinHelper.get_set(key_col, default="Key"):
-                if col in df.columns:
-                    df_key_cols.add(col)
-            if "Key" in df_key_cols:
-                df_key_col = "Key"
-            elif df_key_cols:
-                df_key_col = df_key_cols.pop()
+            # date column
+            df_date_col = None
+            for col in RefTableMixinHelper.get_list(
+                date_col, default=["Timestamp", "Date", "Time"]
+            ):
+                if col in df_columns:
+                    df_date_col = col
+                    index_columns.append(df_date_col)
+                    break
+            if df_date_col is None:
+                if len(df_columns) <= len(index_columns):
+                    raise ValueError(
+                        "PetroVisor::add_ref_table(): 'Timestamp' column is not specified"
+                    )
+                df_date_col = df_columns[len(index_columns)]
+                index_columns.append(df_date_col)
             else:
+                # put index columns in front
+                df_columns = [
+                    *index_columns,
+                    *[col for col in df_columns if col not in index_columns],
+                ]
+
+            # check for columns with invalid name
+            # reserved column names: "ID", "Entity", "Timestamp"
+            reserved_columns = {"ID", "Entity", "Timestamp"}
+            key_value_columns = [
+                self.get_column_name_without_unit(col)
+                for col in df_columns
+                if col not in index_columns
+            ]
+            invalid_columns = reserved_columns.intersection(key_value_columns)
+            if invalid_columns:
                 raise ValueError(
-                    "PetroVisor::add_ref_table(): " "'Key' column is not specified"
+                    f"PetroVisor::add_ref_table(): "
+                    f"Column names {invalid_columns} are not allowed to be used as regular column names."
                 )
 
-            # reserved column names: "ID", "Timestamp", "Entity"
-            reserved_columns = {"ID", "Entity", "Timestamp"}
-            if df_date_col:
-                reserved_columns = reserved_columns.union({df_date_col})
-            if df_entity_col:
-                reserved_columns = reserved_columns.union({df_entity_col})
-            reserved_columns = reserved_columns.union({df_key_col})
-            value_columns = [col for col in df.columns if col not in reserved_columns]
+            # key column
+            df_key_col = None
+            for col in RefTableMixinHelper.get_list(key_col, default="Key"):
+                if col in df_columns:
+                    df_key_col = col
+                    index_columns.append(df_key_col)
+                    break
+                elif col in df_columns_without_unit:
+                    df_key_col = get_column_by_name(col, df_columns)
+                    index_columns.append(df_key_col)
+                    break
+            if df_key_col is None:
+                if len(df_columns) <= len(index_columns):
+                    raise ValueError(
+                        "PetroVisor::add_ref_table(): 'Key' column is not specified"
+                    )
+                df_key_col = df_columns[len(index_columns)]
+                index_columns.append(df_key_col)
+            else:
+                # put index columns in front
+                df_columns = [
+                    *index_columns,
+                    *[col for col in df_columns if col not in index_columns],
+                ]
+
+            value_columns = [col for col in df_columns if col not in index_columns]
+
+            # reorder columns
+            if list(df.columns[: len(index_columns)]) != index_columns:
+                df = df[[*index_columns, *value_columns]]
+
             column_types = df.dtypes
             options = {
                 "Name": name,
                 "Description": description or "",
                 "Key": {
-                    "Name": df_key_col,
+                    "Name": self.get_column_name_without_unit(df_key_col),
                     "UnitName": self.get_column_unit(df_key_col) or " ",
                     "ColumnType": RefTableMixinHelper.get_ref_table_column_type(
                         column_types[df_key_col]
                     ),
                 },
                 "Values": [
                     {
-                        "Name": col,
+                        "Name": self.get_column_name_without_unit(col),
                         "UnitName": self.get_column_unit(col) or " ",
                         "ColumnType": RefTableMixinHelper.get_ref_table_column_type(
                             column_types[col]
                         ),
                     }
                     for col in value_columns
                 ],
             }
             options = ApiHelper.update_dict(options, **kwargs)
             result = self.add_item(ItemType.RefTable, options, **kwargs)
             if is_empty:
                 return result
         if is_empty:
             return ApiRequests.success()
-        # save data to already exists RefTable
+        # check that RefTable was created
         waiting_time = 3  # in seconds
         while not self.item_exists(ItemType.RefTable, name):
             time.sleep(waiting_time)
+        # save data to already exists RefTable
         return self.save_ref_table_data(
             name,
             df,
             skip_existing_data=skip_existing_data,
             chunksize=chunksize,
             **kwargs,
         )
@@ -191,17 +268,17 @@
     def load_ref_table_data(
         self,
         name: str,
         entity: Optional[Union[str, Dict, List[str], List[Dict]]] = None,
         date_start: Optional[Union[datetime, str]] = None,
         date_end: Optional[Union[datetime, str]] = None,
         where_expression: Optional[str] = None,
+        options: Optional[Dict] = None,
         date_col: Optional[str] = "Timestamp",
         entity_col: Optional[str] = "Entity",
-        options: Optional[Dict] = None,
         **kwargs,
     ) -> pd.DataFrame:
         """
         Load reference table data
 
         Parameters
         ----------
@@ -211,22 +288,36 @@
             Entity object(s) or Entity name(s)
         date_start : str, datetime, None
             Start Date or None
         date_end : str, datetime, None
             End Date or None
         where_expression : str, default None
             SQL like WHERE expression
-        date_col : str, default 'Date'
-            Date column name. Default names 'Date' (compatible with date column in P# table), 'Timestamp' (compatible with the internal time column name in RefTable), 'Time' (typically used as displayed name)
+        options : dict, None, default None
+            Options to retrieve data
+        date_col : str, default 'Timestamp'
+            Date column name. Default names
+            'Date' (compatible with date column in P# table),
+            'Timestamp' (compatible with the internal time column name in RefTable),
+            'Time' (typically used as displayed name)
         entity_col : str, default 'Entity'
             Entity column name
-        options : dict, None, default Noe
-            Options to retrieve data
         """
         route = "RefTables"
+
+        # get table columns specs
+        ref_table_info = self.get_ref_table_data_info(name)
+        if not ref_table_info:
+            warnings.warn(
+                "PetroVisor::load_ref_table_data():: "
+                f"Couldn't retrieve ref table '{name}' columns information. Trying to retrieve data only.",
+                RuntimeWarning,
+            )
+
+        # retrieve data
         filter_options = options if options else {}
         if entity:
             if isinstance(
                 entity,
                 (
                     list,
                     tuple,
@@ -252,87 +343,158 @@
             filter_options["WhereExpression"] = where_expression
         filter_options = ApiHelper.update_dict(filter_options, **kwargs)
 
         # get filtered data
         data = self.post(
             f"{route}/{self.encode(name)}/Data", data=filter_options, **kwargs
         )
-        ref_table_info = self.get_ref_table_data_info(name)
-        columns = [f"{d['Name']} [{d['UnitName']}]" for d in ref_table_info["Values"]]
-        key_column = (
-            f"{ref_table_info['Key']['Name']} [{ref_table_info['Key']['UnitName']}]"
-        )
-        columns = [entity_col or "Entity", date_col or "Date", key_column, *columns]
-        df = pd.DataFrame(data=data, columns=columns)
+
+        if not ref_table_info:
+            # assign data without column names
+            df = pd.DataFrame(data=data)
+        else:
+            columns = [
+                f"{d['Name']} [{d['UnitName']}]" for d in ref_table_info["Values"]
+            ]
+            key_column = (
+                f"{ref_table_info['Key']['Name']} [{ref_table_info['Key']['UnitName']}]"
+            )
+            columns = [
+                entity_col or "Entity",
+                date_col or "Timestamp",
+                key_column,
+                *columns,
+            ]
+            # assign data and column names
+            df = pd.DataFrame(data=data, columns=columns)
         return df
 
     # save data to reference table
     def save_ref_table_data(
         self,
         name: str,
         df: pd.DataFrame,
         skip_existing_data: Optional[bool] = False,
         chunksize: Optional[int] = None,
+        date_col: Optional[str] = "Timestamp",
+        entity_col: Optional[str] = "Entity",
         **kwargs,
     ):
         """
         Save reference table data
 
         Parameters
         ----------
         name : str
             Reference table name
         df : DataFrame, dict
-            DataFrame or dictionary, where keys are column names and values are column values or predefined types, such as 'str', 'float', 'bool', 'datetime64[s]'.
+            DataFrame or dictionary, where keys are column names and values are column values or predefined types,
+            such as 'str', 'float', 'bool', 'datetime64[s]'.
         skip_existing_data : bool, default False
             Whether to skip or overwrite existing data that has same combination of 'Entity', 'Timestamp', 'Key'
         chunksize : int, default None
             Chunk size for splitting request into multiple smaller requests.
+        date_col : str, default 'Timestamp'
+            Date column name. Default names
+            'Date' (compatible with date column in P# table),
+            'Timestamp' (compatible with the internal time column name in RefTable),
+            'Time' (typically used as displayed name)
+        entity_col : str, default 'Entity'
+            Entity column name
         """
         route = "RefTables"
 
+        # get table columns specs
+        ref_table_info = self.get_ref_table_data_info(name)
+        if not ref_table_info:
+            warnings.warn(
+                "PetroVisor::save_ref_table_data():: "
+                f"Couldn't retrieve ref table '{name}' columns information. Trying to save data now.",
+                RuntimeWarning,
+            )
+
         # create DataFrame in case if it is passed as dictionary
         def create_dataframe(d: Dict):
             df = pd.DataFrame()
             for c, d in d.items():
                 if isinstance(d, (str, type)):
                     df[c] = pd.Series(dtype=d)
                 else:
                     df[c] = d
             return df
 
         if isinstance(df, dict):
             df = create_dataframe(df)
 
-        if df is not None and not df.empty:
-            if chunksize and (df.shape[0] > chunksize):
-                # num_chunks = int(math.ceil(df.shape[0] / chunksize))
-                # step = max(1, int(math.floor(0.1 * df.shape[0] / chunksize)))
-                i = 0
-
-                for start in range(0, df.shape[0], chunksize):
-                    end = min(start + chunksize, df.shape[0])
-
-                    self.save_ref_table_data(
-                        name,
-                        df[start:end],
-                        skip_existing_data=skip_existing_data,
-                        chunksize=chunksize,
-                        **kwargs,
-                    )
-                    i += 1
-                return ApiRequests.success()
-            # save data
-            data = df.astype("string").to_json(orient="values")
-            return self.put(
-                f"{route}/{self.encode(name)}/Data/String",
-                query={"skipExistingData": skip_existing_data},
-                data=data,
+        if df is None or df.empty:
+            return ApiRequests.success()
+
+        # convert units if don't match with storage
+        if ref_table_info:
+            # ref table units
+            columns = [(d["Name"], d["UnitName"]) for d in ref_table_info["Values"]]
+            key_column = (
+                ref_table_info["Key"]["Name"],
+                ref_table_info["Key"]["UnitName"],
             )
-        return ApiRequests.success()
+            columns = [
+                (entity_col or "Entity", ""),
+                (date_col or "Timestamp", ""),
+                key_column,
+                *columns,
+            ]
+            df_columns = [self.get_column_name_and_unit(col) for col in df.columns]
+            if len(df_columns) != len(columns):
+                raise ValueError(
+                    "PetroVisor::save_ref_table_data():: "
+                    "Number of columns do not match. "
+                    f"RefTable columns: {columns}, DataFrame columns: {df_columns}."
+                )
+            for idx, ((_, unit), (_, df_col_unit)) in enumerate(
+                zip(columns, df_columns)
+            ):
+                df_col = df.columns[idx]
+                if (
+                    unit
+                    and df_col_unit
+                    and unit != df_col_unit
+                    and unit not in (" ", "%")
+                ):
+                    dtype = df[df_col].dtype
+                    df[df_col] = self.convert_units(
+                        df[df_col].values,
+                        source=df_col_unit,
+                        target=unit,
+                    )
+                    df[df_col] = df[df_col].astype(dtype)
+
+        if chunksize and (df.shape[0] > chunksize):
+            # num_chunks = int(math.ceil(df.shape[0] / chunksize))
+            # step = max(1, int(math.floor(0.1 * df.shape[0] / chunksize)))
+            i = 0
+
+            for start in range(0, df.shape[0], chunksize):
+                end = min(start + chunksize, df.shape[0])
+                self.save_ref_table_data(
+                    name,
+                    df[start:end],
+                    skip_existing_data=skip_existing_data,
+                    chunksize=chunksize,
+                    **kwargs,
+                )
+                i += 1
+            return ApiRequests.success()
+
+        # save data
+        data = df.astype("string").to_json(orient="values")
+        return self.put(
+            f"{route}/{self.encode(name)}/Data/String",
+            query={"skipExistingData": skip_existing_data},
+            data=data,
+        )
 
     # delete reference table data
     def delete_ref_table_data(
         self,
         name: str,
         date_start: Optional[Union[datetime, float]] = None,
         date_end: Optional[Union[datetime, float]] = None,
@@ -347,14 +509,17 @@
             Reference table name
         date_start : str, datetime, None
             Start Date or None
         date_end : str, datetime, None
             End Date or None
         """
         route = "RefTables"
+        if not self.item_exists(ItemType.RefTable, name):
+            return ApiRequests.success()
+
         if date_start or date_end:
             date_start = self.get_json_valid_value(date_start, "time", **kwargs) or ""
             date_end = self.get_json_valid_value(date_start, "time", **kwargs) or ""
             if date_start and not date_end:
                 date_end = date_start
             elif not date_start and date_end:
                 date_start = date_end
@@ -381,15 +546,19 @@
         ----------
         name : str
             Reference table name
         """
         route = "RefTables"
         if not self.item_exists(ItemType.RefTable, name):
             return ApiRequests.success()
-        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        # delete data
+        self.delete_ref_table_data(name)
+        # delete item
+        self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        return ApiRequests.success()
 
 
 # Reference table mixin helper
 class RefTableMixinHelper:
 
     # create DataFrame in case if it is passed as dictionary
     @staticmethod
@@ -398,23 +567,25 @@
         for c, d in d.items():
             if isinstance(d, (str, type)):
                 df[c] = pd.Series(dtype=d)
             else:
                 df[c] = d
         return df
 
-    # get set given a value and default
+    # get list given a value and default
     @staticmethod
-    def get_set(col, default=None):
+    def get_list(col, default=None):
         """
-        Get set given a value and default
+        Get list given a value and default
         """
         if isinstance(col, (set, tuple, list)):
-            return set(col)
-        return {col} if col else RefTableMixinHelper.get_set(default) if default else {}
+            return list(col)
+        return (
+            [col] if col else RefTableMixinHelper.get_list(default) if default else []
+        )
 
     # get reference column type
     @staticmethod
     def get_ref_table_column_type(dtype):
         """
         Get reference column type
         """
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/signals.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/signals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 from typing import (
     Any,
     Optional,
     Union,
     List,
+    Set,
     Dict,
     Tuple,
 )
 
 from datetime import datetime
 import pandas as pd
 import numpy as np
 import warnings
-import sys
 
+from petrovisor.api.utils.validators import Validator
+from petrovisor.api.utils.requests import ApiRequests
 from petrovisor.api.utils.helper import ApiHelper
-from petrovisor.api.dtypes.items import ItemType
-from petrovisor.api.dtypes.internal_dtypes import SignalType
-from petrovisor.api.dtypes.increments import (
+from petrovisor.api.enums.items import ItemType
+from petrovisor.api.enums.internal_dtypes import SignalType
+from petrovisor.api.enums.increments import (
     TimeIncrement,
     DepthIncrement,
 )
+from petrovisor.api.models.signal import Signal
+from petrovisor.api.models.entity import Entity
+from petrovisor.api.models.entity_set import EntitySet
+from petrovisor.api.models.hierarchy import Hierarchy
+from petrovisor.api.models.scope import Scope
+from petrovisor.api.models.context import Context
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
     SupportsDataFrames,
     SupportsContextRequests,
     SupportsEntitiesRequests,
+    SupportsUnitsRequests,
 )
 
 
 # Signals API calls
 class SignalsMixin(
     SupportsDataFrames,
     SupportsContextRequests,
     SupportsEntitiesRequests,
     SupportsItemRequests,
+    SupportsUnitsRequests,
     SupportsRequests,
 ):
     """
     Signals API calls
     """
 
     # get signal type
@@ -113,41 +123,15 @@
         ----------
         signal : str, dict
             Signal object or Signal name
         """
         measurement_name = self.get_signal_measurement_name(signal, **kwargs)
         return self.get_measurement_unit_names(measurement_name, **kwargs)
 
-    # get measurement 'Units'
-    def get_measurement_units(self, measurement: str, **kwargs) -> Any:
-        """
-        Get measurement units
-
-        Parameters
-        ----------
-        measurement : str
-            Measurement name
-        """
-        route = "Units"
-        return self.get(f"{route}/{self.encode(measurement)}/Units", **kwargs)
-
-    # get measurement 'Unit' names
-    def get_measurement_unit_names(self, measurement: str, **kwargs) -> Any:
-        """
-        Get measurement unit names
-
-        Parameters
-        ----------
-        measurement : str
-            Measurement name
-        """
-        units = self.get_measurement_units(measurement, **kwargs)
-        return [unit["Name"] for unit in units]
-
-    # get 'Signal'
+    # get signal
     def get_signal(
         self, name: str, short_name: Optional[str] = "", **kwargs
     ) -> Optional[Dict]:
         """
         Get signal by name or short name
 
         Parameters
@@ -162,15 +146,15 @@
             signal = self.get(f"{route}/{self.encode(short_name)}/Signal", **kwargs)
         else:
             signal = None
         if signal is None:
             return self.get(f"{route}/{self.encode(name)}", **kwargs)
         return None
 
-    # get 'Signals'
+    # get signals
     def get_signals(
         self,
         signal_type: Union[str, SignalType] = "",
         entity: Optional[Union[Any, str]] = None,
         **kwargs,
     ) -> List[Dict]:
         """
@@ -197,15 +181,15 @@
                 signal_type=None, entity=entity, **kwargs
             )
             if signal_names and signals:
                 return [s for s in signals if s["Name"] in signal_names]
             return []
         return signals if signals is not None else []
 
-    # get 'Signal' names
+    # get signal names
     def get_signal_names(
         self,
         signal_type: Optional[str] = "",
         entity: Optional[Union[Any, str]] = None,
         **kwargs,
     ) -> List[str]:
         """
@@ -237,40 +221,99 @@
             signals = self.get_signals(signal_type=signal_type, entity=None, **kwargs)
             return [e["Name"] for e in signals]
         # get all signals
         else:
             signal_names = self.get(f"{route}", **kwargs)
         return signal_names if signal_names is not None else []
 
-    # add 'Signals'
-    def add_signals(self, signals: List, **kwargs) -> Any:
+    # add signal
+    def add_signal(self, signal: Union[Signal, Dict[str, Any]], **kwargs) -> Any:
+        """
+        Add signal
+
+        Parameters
+        ----------
+        signal : Signal | dict
+            Signal
+        """
+        route = "Signals"
+        if isinstance(signal, Signal):
+            validated_signal = signal.model_dump(by_alias=True)
+        elif isinstance(signal, dict):
+            validated_signal = signal
+        else:
+            raise ValueError(
+                "PetroVisor::add_signal(): "
+                "Invalid type. Signal should be of type dict or Signal."
+            )
+        return self.post(f"{route}", data=validated_signal, **kwargs)
+
+    # add signals
+    def add_signals(
+        self, signals: List[Union[Signal, Dict[str, Any]]], **kwargs
+    ) -> Any:
         """
         Add multiple signals
 
         Parameters
         ----------
-        signals : list
+        signals : list[Signal | dict]
             List of signals
         """
         route = "Signals"
-        return self.post(f"{route}/Add", data=signals, **kwargs)
+        validated_signals = [
+            e.model_dump(by_alias=True) if isinstance(e, Signal) else e
+            for e in signals
+            if isinstance(e, dict) or isinstance(e, Signal)
+        ]
+        return self.post(f"{route}/Add", data=validated_signals, **kwargs)
+
+    # delete signal
+    def delete_signal(
+        self, signal: Union[Signal, Dict[str, Any], str], **kwargs
+    ) -> Any:
+        """
+        Delete signal
 
-    # delete 'Signals'
-    def delete_signals(self, signals: List, **kwargs) -> Any:
+        Parameters
+        ----------
+        signal : Signal | dict | str
+            Signal
+        """
+        route = "Signals"
+        if isinstance(signal, Signal):
+            name = signal.name
+        else:
+            name = ApiHelper.get_object_name(signal)
+        if not name:
+            return ApiRequests.success()
+        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
+
+    # delete signals
+    def delete_signals(
+        self, signals: List[Union[Signal, Dict[str, Any], str]], **kwargs
+    ) -> Any:
         """
         Delete multiple signals
 
         Parameters
         ----------
-        signals : list
+        signals : list[Signal | dict | str]
             List of signals
         """
         route = "Signals"
-        for signal_name in signals:
-            self.delete(f"{route}/{self.encode(signal_name)}", **kwargs)
+        names = [
+            s.name if isinstance(s, Signal) else ApiHelper.get_object_name(s)
+            for s in signals
+            if s
+        ]
+        names = [name for name in names if name]
+        for name in names:
+            self.delete(f"{route}/{self.encode(name)}", **kwargs)
+        return ApiRequests.success()
 
     # get data range
     def get_data_range(
         self,
         signal_type: Optional[str] = None,
         signal: Optional[str] = None,
         entity: Optional[Union[str, List[str]]] = None,
@@ -456,21 +499,23 @@
             )
         return self.post(f"{route}/Cleanse", data=data_with_options, **kwargs)
 
     # load signals data
     def load_signals_data(
         self,
         signals: Union[str, List[Union[str, Dict, Tuple[Any, str]]]],
-        context: Union[str, Dict] = None,
-        entity_set: Union[str, Dict, List[Union[str, Dict]]] = None,
-        scope: Union[str, Dict] = None,
-        hierarchy: Union[str, Dict] = None,
-        scenario: Union[str, Dict] = None,
+        scenario: str = None,
+        context: Union[str, Dict[str, Any], Context] = None,
+        scope: Union[str, Dict[str, Any], Scope] = None,
+        entity_set: Union[str, Dict[str, Any], EntitySet] = None,
+        hierarchy: Union[str, Dict[str, Any], Hierarchy] = None,
+        entities: Union[
+            Union[str, Dict[str, Any], Entity], List[Union[str, Dict[str, Any], Entity]]
+        ] = None,
         entity_type: Union[str, List[str]] = None,
-        entities: Union[Union[str, Dict], List[Union[str, Dict]]] = None,
         time_start: Union[str, datetime] = None,
         time_end: Union[str, datetime] = None,
         time_step: Union[str, TimeIncrement] = None,
         depth_start: float = None,
         depth_end: float = None,
         depth_step: Union[str, DepthIncrement] = None,
         depth_unit: float = None,
@@ -479,30 +524,29 @@
         """
         Load signals data
 
         Parameters
         ----------
         signals : str | list[str] | list[dict|object]
             Signal name(s) or Signal objects. Single signal or multiple signals
-        context : Union[str, dict, object]
-            Context name or object
-        entity_set : str  | list[str], default None
-            Entity set or list of Entities. If None, then all entities of requested entity type will be considered
-        scope : str, default None
-            Scope name
-        hierarchy : str, default None
-            Hierarchy name
         scenario : str, default None
             Scenario name
+        context : str | dict | Context
+            Context or context name
+        scope : str | dict | Scope, default None
+            Scope or scope name
+        entity_set : str | dict | EntitySet, default None
+            Entity set or entity set name
+        hierarchy : str | dict | Hierarchy, default None
+            Hierarchy or hierarchy name
+        entities : str | dict | Entity | list[str | dict | Entity], default None
+            Entity or list of Entities
         entity_type : str | list[str], default None
             Entity type. Used when entity_set, entities or context is not provided.
-            If None, then all entities will be considered.
             If not None, will filter out entities defined in entity_set.
-        entities : str | list[str], default None
-            Entity or list of Entities
         time_start : datetime, str, default None
             Start of time range
         time_end : datetime, str, default None
             End of time range
         time_step : str, TimeIncrement, default None
             Step of time range, e.g. 'Daily', 'Hourly'
         depth_start : datetime, float, None, default None
@@ -535,29 +579,28 @@
             return s
 
         signals = [get_signal_and_unit(s) for s in signal_names]
         signal_names = [s["Name"] for s in signals]
         if not signals:
             if not signal_names:
                 warnings.warn(
-                    "load_signals_data():: No signals were provided.",
+                    "PetroVisor::load_signals_data():: No signals were provided.",
                     RuntimeWarning,
                 )
             else:
                 warnings.warn(
-                    f"load_signals_data():: Couldn't find signals {signal_names}.",
+                    f"PetroVisor::load_signals_data():: Couldn't find signals {signal_names}.",
                     RuntimeWarning,
                 )
             return None
 
         # get context
         context = (
             self.get_context(
                 context,
-                context=context,
                 entity_set=entity_set,
                 scope=scope,
                 hierarchy=hierarchy,
                 entity_type=entity_type,
                 entities=entities,
                 time_start=time_start,
                 time_end=time_end,
@@ -573,15 +616,15 @@
         hierarchy = ApiHelper.get_object_name(context.get("Hierarchy", None) or "")
 
         # get entity set
         entities = entity_set.get("Entities", None) or []
         if not entities:
             raise ValueError(
                 "load_signals_data():: "
-                f"entity set is empty! Please provide non empty entity_set, or list of entities, or define entity_type."
+                "entity set is empty! Please provide non empty entity_set, or list of entities, or define entity_type."
             )
         entity_names = [ApiHelper.get_object_name(e) for e in entities]
 
         # define signal types
         signal_types = {
             "static": [s for s in signals if s["SignalType"] in {"Static", "String"}],
             "time": [
@@ -592,17 +635,17 @@
             "depth": [
                 s
                 for s in signals
                 if s["SignalType"] in {"DepthDependent", "StringDepthDependent"}
             ],
         }
         signal_types = {k: v for k, v in signal_types.items() if v}
-        has_static_signals = signal_types.get("static", None) is not None
         has_time_signals = signal_types.get("time", None) is not None
-        has_depth_signals = signal_types.get("depth", None) is not None
+        # has_depth_signals = signal_types.get("depth", None) is not None
+        # has_static_signals = signal_types.get("static", None) is not None
 
         # get scope range
         time_start = None
         time_end = None
         time_step = None
         depth_start = None
         depth_end = None
@@ -613,67 +656,57 @@
             time_end = scope.get("End", None)
             time_step = scope.get("TimeIncrement", None)
             if time_step:
                 time_step = str(self.get_time_increment_enum(time_step).name)
             else:
                 time_step = str(TimeIncrement.EverySecond.name)
             if not time_start or pd.isnull(time_start):
-                # might use later in case there will evidence that it is faster
-                # time_start = np.min(
-                #     [
-                #         pd.to_datetime(
-                #             (self.get_data_range(s["SignalType"]) or {}).get(
-                #                 "Start", ""
-                #             )
-                #         )
-                #         for s in ["TimeDependent", "StringTimeDependent"]
-                #     ]
-                # )
-                time_start = np.min(
-                    [
-                        pd.to_datetime(
-                            (
-                                self.get_data_range(
-                                    s["SignalType"],
-                                    signal=s["Name"],
-                                    entity=entity_names,
-                                )
-                                or {}
-                            ).get("Start", "")
-                        )
-                        for s in time_signals
-                    ]
-                )
+                # may use later in case there will evidence that it is faster
+                # time_starts: List[Any] = [
+                #     pd.to_datetime(
+                #         (self.get_data_range(s["SignalType"]) or {}).get("Start", "")
+                #     )
+                #     for s in ["TimeDependent", "StringTimeDependent"]
+                # ]
+                time_starts: List[Any] = [
+                    pd.to_datetime(
+                        (
+                            self.get_data_range(
+                                s["SignalType"],
+                                signal=s["Name"],
+                                entity=entity_names,
+                            )
+                            or {}
+                        ).get("Start", "")
+                    )
+                    for s in time_signals
+                ]
+                time_start = np.min(time_starts)
             if not time_end or pd.isnull(time_end):
-                # might use later in case there will evidence that it is faster
-                # time_end = np.max(
-                #     [
-                #         pd.to_datetime(
-                #             (
-                #                 self.get_data_range(s["SignalType"]) or {}
-                #             ).get("End", "")
-                #         )
-                #         for s in ["TimeDependent", "StringTimeDependent"]
-                #     ]
-                # )
-                time_end = np.max(
-                    [
-                        pd.to_datetime(
-                            (
-                                self.get_data_range(
-                                    s["SignalType"],
-                                    signal=s["Name"],
-                                    entity=entity_names,
-                                )
-                                or {}
-                            ).get("End", "")
-                        )
-                        for s in time_signals
-                    ]
-                )
+                # may use later in case there will be evidence that it is faster
+                # time_end: List[Any] = [
+                #     pd.to_datetime(
+                #         (self.get_data_range(s["SignalType"]) or {}).get("End", "")
+                #     )
+                #     for s in ["TimeDependent", "StringTimeDependent"]
+                # ]
+                time_ends: List[Any] = [
+                    pd.to_datetime(
+                        (
+                            self.get_data_range(
+                                s["SignalType"],
+                                signal=s["Name"],
+                                entity=entity_names,
+                            )
+                            or {}
+                        ).get("End", "")
+                    )
+                    for s in time_signals
+                ]
+                time_end = np.max(time_ends)
 
             # convert to ISO time format '%Y-%m-%dT%H:%M:%S.%f'
             time_start = self.datetime_to_string(pd.to_datetime(time_start))
             time_end = self.datetime_to_string(pd.to_datetime(time_end))
 
         depth_signals = signal_types.get("depth", None)
         if depth_signals:
@@ -705,15 +738,15 @@
                         self.get_data_range(
                             s["SignalType"], signal=s["Name"], entity=entity_names
                         )
                         or {}
                     ).get("End", None)
                     for s in depth_signals
                 ]
-                depth_end = np.min([v for v in depth_ends if v is not None] or None)
+                depth_end = np.max([v for v in depth_ends if v is not None] or None)
                 depth_end = (
                     depth_end if depth_end is not None else np.finfo(np.float64).max
                 )
 
             # convert to float
             depth_start = float(depth_start)
             depth_end = float(depth_end)
@@ -725,47 +758,24 @@
         use_filters = False  # use when is more reliable
         if use_filters:
             unit_names = [s["UnitName"] for s in signals]
             signals_with_units_map = {
                 s["Name"]: f"{s['Name']} [{s['UnitName']}]" for s in signals
             }
             data_rqst = {
-                # "Name": "string",
-                # "EntityNamePattern": "string",
-                # "SignalNamePattern": "string",
-                # "ShowEmptyRows": true,
-                # "ShowEmptyColumns": true,
-                # "HierarchyName": "string",
-                # "EntityType": "string",
-                # "DataTypes": [
-                #  "None"
-                # ],
-                # "EntitySetName": "string",
                 "CheckedEntities": entity_names,
                 "CheckedSignals": signal_names,
                 "CheckedUnits": unit_names,
-                # "ScopeName": "string",
-                # "ChartDefinitionName": "string",
-                # "ScenarioNames": [
-                #  "string"
-                # ],
-                # "IncludeWorkspaceData": true,
-                # "TimeStart": "2024-04-12T20:42:22.961Z",
-                # "TimeEnd": "2024-04-12T20:42:22.961Z",
-                # "TimeStep": "EverySecond",
-                # "DepthStart": 0,
-                # "DepthEnd": 0,
-                # "DepthStep": "TenthMeter"
             }
             if scenario:
                 if not isinstance(scenario, (list, tuple, set)):
                     scenarios = list(scenario)
                 else:
                     scenarios = [scenario]
-                data_rqst["Scenario"] = scenarios
+                data_rqst["ScenarioNames"] = scenarios
             if hierarchy:
                 data_rqst["HierarchyName"] = hierarchy
             if time_start is not None:
                 data_rqst["TimeStart"] = time_start
             if time_end is not None:
                 data_rqst["TimeEnd"] = time_end
             if time_step is not None:
@@ -870,185 +880,105 @@
                     for s in data_type_signals
                 }
 
                 # retrieve numeric data
                 if signals_with_units_num:
                     if data_type == "time":
                         data_rqst = {
-                            # "Requests": [
-                            #    {
-                            #        "Entity": "string",
-                            #        "Signal": "string",
-                            #        "Unit": "string"
-                            #    }
-                            #  ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_num,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
-                            # "Hierarchy": "string",
                             "TimeIncrement": time_step,
                             "Start": time_start,
                             "End": time_end,
-                            # "Options": {
-                            #     "WithGaps": true,
-                            #     "GapValue": "NaN",
-                            #     "GapStringValue": ""
-                            # }
                         }
                         if hierarchy:
                             data_rqst["Hierarchy"] = hierarchy
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         # if num_gap_value is not None:
                         #     data_rqst["Options"] = {"WithGaps": True, "GapStringValue": num_gap_value}
                         data_num = self.post("Data/Time/Retrieve", data=data_rqst)
                     elif data_type == "depth":
                         data_rqst = {
-                            # "Requests": [
-                            #     {
-                            #         "Entity": "string",
-                            #         "Signal": "string",
-                            #         "Unit": "string"
-                            #     }
-                            # ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_num,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
                             "DepthIncrement": depth_step,
                             "StartDepth": depth_start,
                             "EndDepth": depth_end,
-                            # "Options": {
-                            #     "WithGaps": true,
-                            #     "GapValue": "NaN",
-                            #     "GapStringValue": ""
-                            # },
-                            # "DepthUnit": depth_unit,
                         }
-                        if depth_unit is not None:
+                        if depth_unit:
                             data_rqst["DepthUnit"] = depth_unit
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         # if num_gap_value is not None:
                         #     data_rqst["Options"] = {"WithGaps": True, "GapStringValue": num_gap_value}
                         data_num = self.post("Data/Depth/Retrieve", data=data_rqst)
                     else:
                         data_rqst = {
-                            # "Requests": [
-                            #    {
-                            #        "Entity": "string",
-                            #        "Signal": "string",
-                            #        "Unit": "string"
-                            #    }
-                            #  ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_num,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
-                            # "Hierarchy": "string",
                         }
                         if hierarchy:
                             data_rqst["Hierarchy"] = hierarchy
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         data_num = self.post("Data/Static/Retrieve", data=data_rqst)
                 else:
                     data_num = []
 
                 # retrieve string data
                 if signals_with_units_str:
                     if data_type == "time":
                         data_rqst = {
-                            # "Requests": [
-                            #    {
-                            #        "Entity": "string",
-                            #        "Signal": "string",
-                            #        "Unit": "string"
-                            #    }
-                            #  ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_str,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
-                            # "Hierarchy": "string",
                             "TimeIncrement": time_step,
                             "Start": time_start,
                             "End": time_end,
-                            # "Options": {
-                            #     "WithGaps": true,
-                            #     "GapValue": "NaN",
-                            #     "GapStringValue": ""
-                            # }
                         }
                         if hierarchy:
                             data_rqst["Hierarchy"] = hierarchy
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         # if num_gap_value is not None:
                         #     data_rqst["Options"] = {"WithGaps": True, "GapStringValue": str_gap_value}
                         data_str = self.post("Data/StringTime/Retrieve", data=data_rqst)
                     elif data_type == "depth":
                         data_rqst = {
-                            # "Requests": [
-                            #     {
-                            #         "Entity": "string",
-                            #         "Signal": "string",
-                            #         "Unit": "string"
-                            #     }
-                            # ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_str,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
                             "DepthIncrement": depth_step,
                             "StartDepth": depth_start,
                             "EndDepth": depth_end,
-                            # "Options": {
-                            #     "WithGaps": true,
-                            #     "GapValue": "NaN",
-                            #     "GapStringValue": ""
-                            # },
-                            # "DepthUnit": "string",
                         }
-                        if depth_unit is not None:
+                        if depth_unit:
                             data_rqst["DepthUnit"] = depth_unit
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         # if num_gap_value is not None:
                         #     data_rqst["Options"] = {"WithGaps": True, "GapStringValue": str_gap_value}
-                        data_num = self.post(
+                        data_str = self.post(
                             "Data/StringDepth/Retrieve", data=data_rqst
                         )
                     else:
                         data_rqst = {
-                            # "Requests": [
-                            #    {
-                            #        "Entity": "string",
-                            #        "Signal": "string",
-                            #        "Unit": "string"
-                            #    }
-                            #    ],
                             "Combinations": {
                                 "Entities": entity_names,
                                 "Signals": signals_with_units_str,
                             },
-                            # "TopRecords": 0,
-                            # "Scenario": "string",
-                            # "Hierarchy": "string",
                         }
                         if hierarchy:
                             data_rqst["Hierarchy"] = hierarchy
                         if scenario:
                             data_rqst["Scenario"] = scenario
                         data_str = self.post("Data/String/Retrieve", data=data_rqst)
                 else:
@@ -1062,15 +992,15 @@
                 elif data_str:
                     data = data_str
                 else:
                     data = []
 
                 if not data:
                     warnings.warn(
-                        f"load_signals_data():: Couldn't retrieve any {data_type} data.",
+                        f"PetroVisor::load_signals_data():: Couldn't retrieve any {data_type} data.",
                         RuntimeWarning,
                     )
                     continue
 
                 if data_type == "time":
                     # create DataFrame by normalizing json
                     df_normalized = pd.json_normalize(
@@ -1109,24 +1039,24 @@
                         index="Entity", columns="Signal", values="Data"
                     )
                     df.columns.name = None
                     df = df.rename(columns=signals_with_units_map)
                     df = df.reset_index()
                     df_static = df
 
-        def reorder_columns(df, signals, signal_names):
+        def reorder_columns(df, signal_names):
             non_signal_columns = [
                 col
                 for col in df.columns
                 if self.get_column_name_without_unit(col) not in signal_names
             ]
             return df[
                 [
                     *non_signal_columns,
-                    *[f"{s['Name']} [{s['UnitName']}]" for s in signals],
+                    *[col for col in df.columns if col not in non_signal_columns],
                 ]
             ]
 
         # merge all tables
         df = None
         if df_time is not None:
             df = df_time
@@ -1135,26 +1065,28 @@
                 df = pd.merge(df, df_depth, on="Entity")
                 columns = df.columns.tolist()
                 columns.remove("Depth")
                 columns.insert(2, "Depth")
                 df = df[columns]
             else:
                 df = df_depth
+            if depth_unit:
+                df = df.rename(columns={"Depth": f"Depth [{depth_unit}]"})
         if df_static is not None:
             if df is not None:
                 df = pd.merge(df, df_static, on="Entity")
             else:
                 df = df_static
         if df is None:
             warnings.warn(
-                f"load_signals_data():: Couldn't retrieve any data.",
+                "PetroVisor::load_signals_data():: Couldn't retrieve any data.",
                 RuntimeWarning,
             )
             return df
-        return reorder_columns(df, signals, signal_names)
+        return reorder_columns(df, signal_names)
 
     # load data
     def load_data(
         self,
         data_type: Union[str, SignalType],
         data: List,
         start: Optional[Union[datetime, float]] = None,
@@ -1477,37 +1409,15 @@
         Get SignalType enum
 
         Parameters
         ----------
         signal_type : str, SignalType
             Signal type
         """
-        if isinstance(signal_type, SignalType):
-            return signal_type
-        # prepare name for comparison
-        signal_type = ApiHelper.get_comparison_string(signal_type, **kwargs)
-        if signal_type in ("static", "staticnumeric"):
-            return SignalType.Static
-        elif signal_type in ("time", "timenumeric", "timedependent"):
-            return SignalType.TimeDependent
-        elif signal_type in ("depth", "depthnumeric", "depthdependent"):
-            return SignalType.DepthDependent
-        elif signal_type in ("string", "staticstring"):
-            return SignalType.String
-        elif signal_type in ("stringtime", "timestring", "stringtimedependent"):
-            return SignalType.StringTimeDependent
-        elif signal_type in ("stringdepth", "depthstring", "stringdepthdependent"):
-            return SignalType.StringDepthDependent
-        elif signal_type in ("pvt", "pvtnumeric"):
-            return SignalType.PVT
-        raise ValueError(
-            f"PetroVisor::get_signal_type_name(): "
-            f"unknown data type: '{signal_type}'! "
-            f"Should be one of: {[t.name for t in SignalType]}"
-        )
+        return Validator.get_signal_type_enum(signal_type, **kwargs)
 
     # get time or depth increment name
     def get_increment_enum(
         self,
         increment: Union[str, TimeIncrement, DepthIncrement],
         signal_type: Union[str, SignalType],
         **kwargs,
@@ -1540,98 +1450,169 @@
         Get TimeIncrement enum
 
         Parameters
         ----------
         increment_type : str, TimeIncrement
             Increment
         """
-        if isinstance(increment_type, TimeIncrement):
-            return increment_type
-        # prepare name for comparison
-        increment_type = ApiHelper.get_comparison_string(increment_type, **kwargs)
-        if increment_type in ("hourly", "h", "hr", "hour", "1h", "1hr", "1hour"):
-            return TimeIncrement.Hourly
-        elif increment_type in ("daily", "d", "day", "1d", "1day"):
-            return TimeIncrement.Daily
-        elif increment_type in ("monthly", "m", "month", "1m", "1month"):
-            return TimeIncrement.Monthly
-        elif increment_type in ("yearly", "y", "year", "1y", "1year"):
-            return TimeIncrement.Yearly
-        elif increment_type in ("quarterly", "q", "3m", "3month", "quarter"):
-            return TimeIncrement.Quarterly
-        elif increment_type in ("everyminute", "min", "minute", "1min", "1minute"):
-            return TimeIncrement.EveryMinute
-        elif increment_type in (
-            "everysecond",
-            "s",
-            "sec",
-            "second",
-            "1s",
-            "1sec",
-            "1second",
-        ):
-            return TimeIncrement.EverySecond
-        elif increment_type in ("everyfiveminute", "5min", "5minutes"):
-            return TimeIncrement.EveryFiveMinutes
-        elif increment_type in ("everyfifteenminutes", "15min", "15minutes"):
-            return TimeIncrement.EveryFifteenMinutes
-        raise ValueError(
-            f"PetroVisor::get_time_increment_enum(): "
-            f"unknown time increment: '{increment_type}'! "
-            f"Should be one of: {[inc.name for inc in TimeIncrement]}"
-        )
+        return Validator.get_time_increment_enum(increment_type, **kwargs)
 
     # get depth increment name
     def get_depth_increment_enum(
         self, increment_type: Union[str, DepthIncrement], **kwargs
     ) -> DepthIncrement:
         """
         Get DepthIncrement enum
 
         Parameters
         ----------
         increment_type : str, DepthIncrement
             Increment
         """
-        if isinstance(increment_type, DepthIncrement):
-            return increment_type
-        # prepare name for comparison
-        increment_type = ApiHelper.get_comparison_string(increment_type, **kwargs)
-        if increment_type in ("meter", "m", "1meter", "1m"):
-            return DepthIncrement.Meter
-        elif increment_type in (
-            "halfmeter",
-            "halfm",
-            ".5meter",
-            ".5m",
-            "0.5meter",
-            "0.5m",
-        ):
-            return DepthIncrement.HalfMeter
-        elif increment_type in ("tenthmeter", ".1meter", ".1m", "0.1meter", "0.1m"):
-            return DepthIncrement.TenthMeter
-        elif increment_type in (
-            "eightmeter",
-            ".125meter",
-            ".125m",
-            "0.125meter",
-            "0.125m",
-        ):
-            return DepthIncrement.EighthMeter
-        elif increment_type in ("foot", "ft", "1foot", "1ft"):
-            return DepthIncrement.Foot
-        elif increment_type in (
-            "halffoot",
-            "halfft",
-            ".5foot",
-            ".5feet",
-            ".5ft",
-            "0.5foot",
-            "0.5feet",
-            "0.5ft",
-        ):
-            return DepthIncrement.HalfFoot
-        raise ValueError(
-            f"PetroVisor::get_depth_increment_enum(): "
-            f"unknown depth increment: '{increment_type}'! "
-            f"Should be one of: {[inc.name for inc in DepthIncrement]}"
+        return Validator.get_depth_increment_enum(increment_type, **kwargs)
+
+    # get ordered time increments
+    def get_time_increments_ordered(
+        self, reverse: bool = False, **kwargs
+    ) -> List[TimeIncrement]:
+        """
+        Get TimeIncrement enums ordered
+
+        Parameters
+        ----------
+        reverse : bool, default False
+            If False - ascending order, if True - descending order
+        """
+        increments = [
+            TimeIncrement.EverySecond,
+            TimeIncrement.EveryMinute,
+            TimeIncrement.EveryFiveMinutes,
+            TimeIncrement.EveryFifteenMinutes,
+            TimeIncrement.Hourly,
+            TimeIncrement.Daily,
+            TimeIncrement.Monthly,
+            TimeIncrement.Quarterly,
+            TimeIncrement.Yearly,
+        ]
+        if reverse:
+            return increments[::-1]
+        return increments
+
+    # get smallest time increment
+    def get_time_increments_min(
+        self,
+        increment_types: Union[
+            List[Union[str, TimeIncrement]], Set[Union[str, TimeIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[TimeIncrement]:
+        """
+        Get smallest TimeIncrement
+
+        Parameters
+        ----------
+        increment_types : list[str | TimeIncrement]
+            Increments
+        """
+        increments = set(
+            [self.get_time_increment_enum(increment) for increment in increment_types]
         )
+        for increment in self.get_time_increments_ordered():
+            if increment in increments:
+                return increment
+        return None
+
+    # get largest time increment
+    def get_time_increments_max(
+        self,
+        increment_types: Union[
+            List[Union[str, TimeIncrement]], Set[Union[str, TimeIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[TimeIncrement]:
+        """
+        Get largest TimeIncrement enum
+
+        Parameters
+        ----------
+        increment_types : list[str | TimeIncrement]
+            Increments
+        """
+        increments = set(
+            [self.get_time_increment_enum(increment) for increment in increment_types]
+        )
+        for increment in self.get_time_increments_ordered(reverse=True):
+            if increment in increments:
+                return increment
+        return None
+
+    # get ordered depth increments
+    def get_depth_increments_ordered(
+        self, reverse: bool = False, **kwargs
+    ) -> List[DepthIncrement]:
+        """
+        Get DepthIncrement enums ordered
+
+        Parameters
+        ----------
+        reverse : bool, default False
+            If False - ascending order, if True - descending order
+        """
+        increments = [
+            DepthIncrement.TenthMeter,
+            DepthIncrement.EighthMeter,
+            DepthIncrement.HalfFoot,
+            DepthIncrement.Foot,
+            DepthIncrement.HalfMeter,
+            DepthIncrement.Meter,
+        ]
+        if reverse:
+            return increments[::-1]
+        return increments
+
+    # get smallest depth increment
+    def get_depth_increments_min(
+        self,
+        increment_types: Union[
+            List[Union[str, DepthIncrement]], Set[Union[str, DepthIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[DepthIncrement]:
+        """
+        Get smallest DepthIncrement
+
+        Parameters
+        ----------
+        increment_types : list[str | DepthIncrement]
+            Increments
+        """
+        increments = set(
+            [self.get_depth_increment_enum(increment) for increment in increment_types]
+        )
+        for increment in self.get_depth_increments_ordered():
+            if increment in increments:
+                return increment
+        return None
+
+    # get largest depth increment
+    def get_depth_increments_max(
+        self,
+        increment_types: Union[
+            List[Union[str, DepthIncrement]], Set[Union[str, DepthIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[DepthIncrement]:
+        """
+        Get largest DepthIncrement enum
+
+        Parameters
+        ----------
+        increment_types : list[str | DepthIncrement]
+            Increments
+        """
+        increments = set(
+            [self.get_depth_increment_enum(increment) for increment in increment_types]
+        )
+        for increment in self.get_depth_increments_ordered(reverse=True):
+            if increment in increments:
+                return increment
+        return None
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/workflows.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/workflows.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/methods/workspace_values.py` & `petrovisor-0.1.4/src/petrovisor/api/methods/workspace_values.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/protocols/protocols.py` & `petrovisor-0.1.4/src/petrovisor/api/protocols/protocols.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import (
     Any,
     Optional,
     Union,
+    Tuple,
     List,
+    Set,
     Dict,
 )
 
 try:
     from typing import Protocol
 except BaseException:
     from typing_extensions import Protocol
 
+import numpy as np
 import pandas as pd
 from datetime import datetime
 
-from petrovisor.api.dtypes.internal_dtypes import SignalType
-from petrovisor.api.dtypes.increments import (
+from petrovisor.api.enums.internal_dtypes import SignalType
+from petrovisor.api.enums.increments import (
     TimeIncrement,
     DepthIncrement,
 )
 
 
 # PetroVisor requests protocol
 class SupportsRequests(Protocol):
@@ -193,14 +196,91 @@
     ) -> SignalType: ...
 
     # get signal type route
     def get_signal_type_route(
         self, signal_type: Union[str, SignalType], **kwargs
     ) -> str: ...
 
+    # get time increment name
+    def get_time_increment_enum(
+        self, increment_type: Union[str, TimeIncrement], **kwargs
+    ) -> TimeIncrement: ...
+
+    # get depth increment name
+    def get_depth_increment_enum(
+        self, increment_type: Union[str, DepthIncrement], **kwargs
+    ) -> DepthIncrement: ...
+
+    # get ordered time increments
+    def get_time_increments_ordered(
+        self, reverse: bool = False, **kwargs
+    ) -> List[TimeIncrement]: ...
+
+    # get smallest time increment
+    def get_time_increments_min(
+        self,
+        increment_types: Union[
+            List[Union[str, TimeIncrement]], Set[Union[str, TimeIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[TimeIncrement]: ...
+
+    # get largest time increment
+    def get_time_increments_max(
+        self,
+        increment_types: Union[
+            List[Union[str, TimeIncrement]], Set[Union[str, TimeIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[TimeIncrement]: ...
+
+    # get ordered depth increments
+    def get_depth_increments_ordered(
+        self, reverse: bool = False, **kwargs
+    ) -> List[DepthIncrement]: ...
+
+    # get smallest depth increment
+    def get_depth_increments_min(
+        self,
+        increment_types: Union[
+            List[Union[str, DepthIncrement]], Set[Union[str, DepthIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[DepthIncrement]: ...
+
+    # get largest depth increment
+    def get_depth_increments_max(
+        self,
+        increment_types: Union[
+            List[Union[str, DepthIncrement]], Set[Union[str, DepthIncrement]]
+        ],
+        **kwargs,
+    ) -> Optional[DepthIncrement]: ...
+
+
+# Units requests protocol
+class SupportsUnitsRequests(Protocol):
+    # get measurement 'Units'
+    def get_measurement_units(self, measurement: str, **kwargs) -> Any: ...
+
+    # get measurement 'Unit' names
+    def get_measurement_unit_names(self, measurement: str, **kwargs) -> Any: ...
+
+    # get measurements
+    def get_measurements(self, **kwargs) -> Any: ...
+
+    # convert values from one unit to another
+    def convert_units(
+        self,
+        values: Union[float, List[float], np.ndarray, pd.Series, None] = None,
+        source: str = None,
+        target: str = None,
+        **kwargs,
+    ) -> Union[float, List[float], None]: ...
+
 
 # PetroVisor Contex requests protocol
 class SupportsContextRequests(Protocol):
     # get 'Context'
     def get_context(
         self,
         name: Union[str, Dict],
@@ -301,9 +381,25 @@
         psharp_table: Union[Dict, List],
         dropna: bool = True,
         with_entity_column: bool = True,
         groupby_entity: bool = False,
         **kwargs,
     ) -> Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]: ...
 
+    # get column name without unit
+    def get_column_name_without_unit(self, column_name: str, **kwargs) -> str: ...
+
     # get column unit
     def get_column_unit(self, column_name: str, **kwargs) -> str: ...
+
+    # get column name and unit
+    def get_column_name_and_unit(
+        self, column_name: str, **kwargs
+    ) -> Tuple[str, str]: ...
+
+    # convert datetime to string
+    def datetime_to_string(
+        self,
+        d: Union[datetime, str],
+        format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%f",
+        **kwargs,
+    ) -> str: ...
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/utils/datastructs.py` & `petrovisor-0.1.4/src/petrovisor/api/utils/datastructs.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/utils/helper.py` & `petrovisor-0.1.4/src/petrovisor/api/utils/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         """
         if isinstance(obj, str):
             return obj
         elif obj is None:
             return ""
         try:
             return ApiHelper.get_field(obj, field, ignore_case=True) or ""
-        except:
+        except Exception:
             return str(obj)
 
     # update dictionary
     @staticmethod
     def update_dict(d: Dict, **kwargs) -> Dict:
         """
         Update dictionary fields with keyword argument values
@@ -388,24 +388,26 @@
             UUID(value)
         except ValueError:
             return False
         return True
 
     # is iterable
     @staticmethod
-    def is_iterable(x: Any, **kwargs) -> bool:
+    def is_iterable(x: Any, exclude_str: bool = True, **kwargs) -> bool:
         """
         Is iterable object
 
         Parameters
         ----------
         x : Any
             Object
+        exclude_str : bool, default True
+            Whether to exclude str as iterable
         """
-        if hasattr(x, "__len__"):
+        if hasattr(x, "__iter__") and (not isinstance(x, str) or not exclude_str):
             return True
         return False
 
     # is empty
     @staticmethod
     def is_empty(x: Any, **kwargs) -> bool:
         """
@@ -477,15 +479,21 @@
         """
         if isinstance(x, list):
             return x
         elif isinstance(x, (pd.DataFrame, pd.Series)):
             return cast(list, x.values.tolist())
         elif isinstance(x, np.ndarray):
             return cast(list, x.tolist())
-        elif isinstance(x, (set,)):
+        elif isinstance(
+            x,
+            (
+                set,
+                tuple,
+            ),
+        ):
             return list(x)
         elif isinstance(x, (dict,)):
             return list(x.items())
         return [x]
 
     # get file extension
     @staticmethod
```

### Comparing `petrovisor-0.1.3/src/petrovisor/api/utils/login.py` & `petrovisor-0.1.4/src/petrovisor/api/utils/login.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.3/src/petrovisor/api/utils/requests.py` & `petrovisor-0.1.4/src/petrovisor/api/utils/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         method_name = method.upper().strip()
 
         # convert data to json string
         if data and not isinstance(data, str):
             data = json.dumps(data)
 
         # request secs
-        timeout = 59 * 60  # time out limit in seconds (3540)
+        timeout = None  # no timeout
         max_retries = (
             1  # increased to 3 times in case of 400 Bad Request or 4004 Not Found
         )
         waiting_time = 5  # in seconds
 
         # get response
         response = None
```

### Comparing `petrovisor-0.1.3/src/petrovisor/petrovisor.py` & `petrovisor-0.1.4/src/petrovisor/petrovisor.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # import api methods
 from petrovisor.api.base import RequestsMixin
 from petrovisor.api.methods.items import ItemsMixin
 from petrovisor.api.methods.entities import EntitiesMixin
 from petrovisor.api.methods.contexts import ContextMixin
 from petrovisor.api.methods.signals import SignalsMixin
+from petrovisor.api.methods.units import UnitsMixin
 from petrovisor.api.methods.workspace_values import WorkspaceValuesMixin
 from petrovisor.api.methods.psharp import PsharpMixin
 from petrovisor.api.methods.reference_tables import RefTableMixin
 from petrovisor.api.methods.pivot_tables import PivotTableMixin
 from petrovisor.api.methods.dataframes import DataFrameMixin
 from petrovisor.api.methods.ml import MLMixin
 from petrovisor.api.methods.workflows import WorkflowsMixin
@@ -17,17 +18,18 @@
 from petrovisor.api.methods.logs import LogsMixin
 
 
 # PetroVisor API calls
 class PetroVisor(
     RequestsMixin,
     ItemsMixin,
+    UnitsMixin,
     EntitiesMixin,
-    ContextMixin,
     SignalsMixin,
+    ContextMixin,
     WorkspaceValuesMixin,
     PsharpMixin,
     RefTableMixin,
     PivotTableMixin,
     MLMixin,
     WorkflowsMixin,
     FilesMixin,
```

### Comparing `petrovisor-0.1.3/src/petrovisor.egg-info/PKG-INFO` & `petrovisor-0.1.4/src/petrovisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.3/src/petrovisor.egg-info/SOURCES.txt` & `petrovisor-0.1.4/src/petrovisor.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,38 +8,52 @@
 src/petrovisor.egg-info/PKG-INFO
 src/petrovisor.egg-info/SOURCES.txt
 src/petrovisor.egg-info/dependency_links.txt
 src/petrovisor.egg-info/requires.txt
 src/petrovisor.egg-info/top_level.txt
 src/petrovisor/api/__init__.py
 src/petrovisor/api/base.py
-src/petrovisor/api/dtypes/__init__.py
-src/petrovisor/api/dtypes/data_grids.py
-src/petrovisor/api/dtypes/increments.py
-src/petrovisor/api/dtypes/internal_dtypes.py
-src/petrovisor/api/dtypes/items.py
-src/petrovisor/api/dtypes/ml.py
+src/petrovisor/api/enums/__init__.py
+src/petrovisor/api/enums/data_grids.py
+src/petrovisor/api/enums/increments.py
+src/petrovisor/api/enums/internal_dtypes.py
+src/petrovisor/api/enums/items.py
+src/petrovisor/api/enums/ml.py
 src/petrovisor/api/methods/__init__.py
 src/petrovisor/api/methods/contexts.py
 src/petrovisor/api/methods/data_grids.py
 src/petrovisor/api/methods/dataframes.py
 src/petrovisor/api/methods/entities.py
 src/petrovisor/api/methods/files.py
 src/petrovisor/api/methods/items.py
 src/petrovisor/api/methods/logs.py
 src/petrovisor/api/methods/ml.py
 src/petrovisor/api/methods/pivot_tables.py
 src/petrovisor/api/methods/psharp.py
 src/petrovisor/api/methods/reference_tables.py
 src/petrovisor/api/methods/signals.py
+src/petrovisor/api/methods/units.py
 src/petrovisor/api/methods/workflows.py
 src/petrovisor/api/methods/workspace_values.py
+src/petrovisor/api/models/__init__.py
+src/petrovisor/api/models/base_model.py
+src/petrovisor/api/models/context.py
+src/petrovisor/api/models/entity.py
+src/petrovisor/api/models/entity_set.py
+src/petrovisor/api/models/hierarchy.py
+src/petrovisor/api/models/scope.py
+src/petrovisor/api/models/signal.py
+src/petrovisor/api/models/unit.py
 src/petrovisor/api/protocols/__init__.py
 src/petrovisor/api/protocols/protocols.py
 src/petrovisor/api/utils/__init__.py
 src/petrovisor/api/utils/datastructs.py
+src/petrovisor/api/utils/general.py
 src/petrovisor/api/utils/helper.py
 src/petrovisor/api/utils/login.py
 src/petrovisor/api/utils/requests.py
+src/petrovisor/api/utils/validators.py
 tests/test_api.py
 tests/test_entities_and_signals.py
-tests/test_reference_tables.py
+tests/test_reference_tables.py
+tests/test_signals.py
+tests/test_units.py
```

### Comparing `petrovisor-0.1.3/tests/test_entities_and_signals.py` & `petrovisor-0.1.4/tests/test_entities_and_signals.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 from petrovisor import PetroVisor
 import pandas as pd
 import numpy as np
-import pytest
 
 
-def test_signals_by_entity(pv_api: PetroVisor):
+def test_signals_by_entity(api: PetroVisor):
     """
     Test retrieving signals by entity type
     """
     # add new entity
-    entity_name = r"_entity with special characters %*,$&^§()#//=2!~*'"  # except '?', ';'
-    pv_api.add_item('Entity', {
-        'Name': entity_name,
-        'EntityTypeName': 'Well',
-        'Alias': '',
-        'IsOpportunity': False,
-    })
+    entity_name = (
+        r"_entity with special characters %*,$&^§()#//=2!~*'"  # except '?', ';'
+    )
+    api.add_item(
+        "Entity",
+        {
+            "Name": entity_name,
+            "EntityTypeName": "Well",
+            "Alias": "",
+            "IsOpportunity": False,
+        },
+    )
     # rename entity
-    new_entity_name = entity_name.replace('_entity', '_renamed entity')
+    new_entity_name = entity_name.replace("_entity", "_renamed entity")
     # pv_api.rename_entity(old_name=entity_name, new_name=new_entity_name)
     # delete entity
     # pv_api.delete_entity(new_entity_name)
     # add signal
-    signal_name = 'Time Signal'
-    signal_unit = ' '
+    signal_name = "Time Signal"
+    signal_unit = " "
     max_length = 29
-    short_signal_name = signal_name[:max_length] if len(signal_name) > max_length else signal_name
-    pv_api.add_item('Signal', {
-        'Name': signal_name,
-        'ShortName': short_signal_name,
-        'SignalType': 'TimeDependent',
-        'MeasurementName': 'Dimensionless',
-        'StorageUnitName': signal_unit,
-        'AggregationType': 'Sum',
-        'ContainerAggregationType': 'Sum',
-    })
+    short_signal_name = (
+        signal_name[:max_length] if len(signal_name) > max_length else signal_name
+    )
+    api.add_item(
+        "Signal",
+        {
+            "Name": signal_name,
+            "ShortName": short_signal_name,
+            "SignalType": "TimeDependent",
+            "MeasurementName": "Dimensionless",
+            "StorageUnitName": signal_unit,
+            "AggregationType": "Sum",
+            "ContainerAggregationType": "Sum",
+        },
+    )
     # add signal data
     num_rows = 5
     signal_col = f"{signal_name} [{signal_unit}]"
-    df = pd.DataFrame({'Entity': np.repeat(entity_name, num_rows),
-                       'Date': pd.date_range("2023-11-29", periods=num_rows, freq="D"),
-                       signal_col: np.random.rand(num_rows)})
-    pv_api.save_table_data(df)
+    df = pd.DataFrame(
+        {
+            "Entity": np.repeat(entity_name, num_rows),
+            "Date": pd.date_range("2023-11-29", periods=num_rows, freq="D"),
+            signal_col: np.random.rand(num_rows),
+        }
+    )
+    api.save_table_data(df)
     # get signals by entity
-    entity_signals = pv_api.get_signals(entity=entity_name, signal_type='time')
-    assert signal_name in [s['Name'] for s in entity_signals]
+    entity_signals = api.get_signals(entity=entity_name, signal_type="time")
+    assert signal_name in [s["Name"] for s in entity_signals]
```

### Comparing `petrovisor-0.1.3/tests/test_reference_tables.py` & `petrovisor-0.1.4/tests/test_reference_tables.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,66 @@
-from petrovisor import PetroVisor
+from petrovisor import PetroVisor, ItemType
 import pandas as pd
 import numpy as np
+import uuid
 
 
-def test_ref_tables(pv_api: PetroVisor):
+def test_ref_tables(api: PetroVisor):
 
     # create entity
     entity_name = "Well 001"
-    pv_api.add_item('Entity', {
-        'Name': entity_name,
-        'EntityTypeName': 'Well',
-        'Alias': '',
-        'IsOpportunity': False,
-    })
+    api.add_item(
+        "Entity",
+        {
+            "Name": entity_name,
+            "EntityTypeName": "Well",
+            "Alias": "",
+            "IsOpportunity": False,
+        },
+    )
 
     # create dataframe
     num_rows = int(10)
-    columns = list('ABCDEF')
-    df = pd.DataFrame(np.random.uniform(0, 1, size=(num_rows, len(columns))), columns=columns)
-
-    df['Entity'] = None
-    df.loc[:num_rows // 2, 'Entity'] = entity_name
-    df['Time'] = None
-    df['Key'] = [str(i) for i in range(0, len(df))]
-
-    df = df[['Entity', 'Time', 'Key', *columns]]
-    df['Key'] = df['Key'].values.astype(str)
-
-    name = 'PyTest New RefTable'
-
-    # delete table if exists
-    pv_api.delete_ref_table(name)
+    columns = list("ABCDEF")
+    df = pd.DataFrame(
+        np.random.uniform(0, 1, size=(num_rows, len(columns))), columns=columns
+    )
+
+    df["Entity"] = None
+    df.loc[: num_rows // 2, "Entity"] = entity_name
+    df["Time"] = None
+    df["Key"] = [str(i) for i in range(0, len(df))]
+
+    df = df[["Entity", "Time", "Key", *columns]]
+    df["Key"] = df["Key"].values.astype(str)
+
+    # create unique name to avoid interference
+    name = str(uuid.uuid4())
+    while api.item_exists(ItemType.RefTable, name):
+        name = str(uuid.uuid4())
 
     # add new reference table
-    pv_api.add_ref_table(name, df, description='Testing API from Python')
+    api.add_ref_table(name, df, description="Testing API from Python")
 
     # add data to already existing table
-    pv_api.add_ref_table(name, df, description='Testing API from Python')
+    api.add_ref_table(name, df, description="Testing API from Python")
 
     # check that table was created
-    ref_table_info = pv_api.get_ref_table_data_info(name)
-    assert ref_table_info
+    assert api.get_ref_table_data_info(name)
 
     # save data and overwrite existing data
     # meaning that rows with the same 'Entity', 'Timestamp/Date/Time', 'Key' will be overwritten
-    pv_api.save_ref_table_data(name, df, skip_existing_data=False)
+    api.save_ref_table_data(name, df, skip_existing_data=False)
 
     # save data but keep existing data
     # meaning that rows with the same 'Entity', 'Timestamp/Date/Time', 'Key' will be not overwritten
-    pv_api.save_ref_table_data(name, df, skip_existing_data=True)
+    api.save_ref_table_data(name, df, skip_existing_data=True)
 
     # load table
-    df = pv_api.load_ref_table_data(name)
+    df = api.load_ref_table_data(name)
     assert df.shape[0] == num_rows
 
+    # delete reference table data
+    api.delete_ref_table_data(name)
+
     # delete reference table
-    pv_api.delete_ref_table_data(name)
-    pv_api.delete_ref_table(name)
+    api.delete_ref_table(name)
```

