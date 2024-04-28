# Comparing `tmp/es_testbed-0.5.4.tar.gz` & `tmp/es_testbed-0.6.0.tar.gz`

## Comparing `es_testbed-0.5.4.tar` & `es_testbed-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,96 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/__init__.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/defaults.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/py.typed
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/base.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/ilm.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/plan.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/tracker.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entities/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entities/alias.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entities/data_stream.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entities/entity.py
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entities/index.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/componentmgr.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/data_streammgr.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/entitymgr.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/ilmmgr.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/indexmgr.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/snapshotmgr.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/templatemgr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/helpers/__init__.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/helpers/es_api.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 es_testbed-0.5.4/src/es_testbed/helpers/utils.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_testbed-0.5.4/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_testbed-0.5.4/LICENSE
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 es_testbed-0.5.4/README.md
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 es_testbed-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 es_testbed-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/coverage_html.js
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_17bd492d087794b9___init___py.html
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_17bd492d087794b9_test_cls_ilm_py.html
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_17bd492d087794b9_test_cls_tracker_py.html
+-rw-r--r--   0        0        0    12659 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_17bd492d087794b9_test_defaults_py.html
+-rw-r--r--   0        0        0    46989 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_17bd492d087794b9_test_utils_py.html
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_5d92fa905a1d3e20___init___py.html
+-rw-r--r--   0        0        0    51432 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_5d92fa905a1d3e20_base_py.html
+-rw-r--r--   0        0        0    76619 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_5d92fa905a1d3e20_ilm_py.html
+-rw-r--r--   0        0        0    55262 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_5d92fa905a1d3e20_plan_py.html
+-rw-r--r--   0        0        0    19793 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_5d92fa905a1d3e20_tracker_py.html
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_684879e5f25da111___init___py.html
+-rw-r--r--   0        0        0    17240 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_684879e5f25da111_alias_py.html
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_684879e5f25da111_data_stream_py.html
+-rw-r--r--   0        0        0    13138 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_684879e5f25da111_entity_py.html
+-rw-r--r--   0        0        0    53828 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_684879e5f25da111_index_py.html
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6___init___py.html
+-rw-r--r--   0        0        0    20779 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_componentmgr_py.html
+-rw-r--r--   0        0        0    32750 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_data_streammgr_py.html
+-rw-r--r--   0        0        0    26963 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_entitymgr_py.html
+-rw-r--r--   0        0        0    21929 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_ilmmgr_py.html
+-rw-r--r--   0        0        0    47238 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_indexmgr_py.html
+-rw-r--r--   0        0        0    17638 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_snapshotmgr_py.html
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_689e0199004d67b6_templatemgr_py.html
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_72ef0405fdf841ab___init___py.html
+-rw-r--r--   0        0        0   157952 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_72ef0405fdf841ab_es_api_py.html
+-rw-r--r--   0        0        0    53262 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_72ef0405fdf841ab_utils_py.html
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_9e00aab3b961c475___init___py.html
+-rw-r--r--   0        0        0    17140 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_9e00aab3b961c475_alias_py.html
+-rw-r--r--   0        0        0    14961 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_9e00aab3b961c475_data_stream_py.html
+-rw-r--r--   0        0        0    13886 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_9e00aab3b961c475_entity_py.html
+-rw-r--r--   0        0        0    53872 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_9e00aab3b961c475_index_py.html
+-rw-r--r--   0        0        0    29407 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df___init___py.html
+-rw-r--r--   0        0        0    22452 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_basic_data_streams_py.html
+-rw-r--r--   0        0        0    22640 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_basic_frozen_py.html
+-rw-r--r--   0        0        0    21979 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_basic_rollover_py.html
+-rw-r--r--   0        0        0    24403 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_cold_ds_py.html
+-rw-r--r--   0        0        0    24643 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_cold_indices_py.html
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_cold_py.html
+-rw-r--r--   0        0        0    24415 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_frozen_ds_py.html
+-rw-r--r--   0        0        0    24512 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_frozen_indices_py.html
+-rw-r--r--   0        0        0    15542 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_frozen_py.html
+-rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_hot_py.html
+-rw-r--r--   0        0        0    24769 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a40f6d277e0496df_test_rollover_frozen_py.html
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    92748 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_a44f0ac069e85531_conftest_py.html
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902___init___py.html
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_componentmgr_py.html
+-rw-r--r--   0        0        0    32786 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_data_streammgr_py.html
+-rw-r--r--   0        0        0    28917 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_entitymgr_py.html
+-rw-r--r--   0        0        0    23102 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_ilmmgr_py.html
+-rw-r--r--   0        0        0    47199 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_indexmgr_py.html
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_snapshotmgr_py.html
+-rw-r--r--   0        0        0    24053 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_e41b34ddf7b70902_templatemgr_py.html
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d___init___py.html
+-rw-r--r--   0        0        0    62980 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d__base_py.html
+-rw-r--r--   0        0        0    55222 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d__plan_py.html
+-rw-r--r--   0        0        0    38428 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d_defaults_py.html
+-rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d_exceptions_py.html
+-rw-r--r--   0        0        0    76479 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/d_f43263c25e31810d_ilm_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/favicon_32.png
+-rw-r--r--   0        0        0    17077 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/keybd_open.png
+-rw-r--r--   0        0        0    16736 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 es_testbed-0.6.0/cov_html/style.css
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/__init__.py
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/_base.py
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/_plan.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/defaults.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/exceptions.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/ilm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/py.typed
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/classes/tracker.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/entities/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/entities/alias.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/entities/data_stream.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/entities/entity.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/entities/index.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/helpers/__init__.py
+-rw-r--r--   0        0        0    16605 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/helpers/es_api.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/helpers/utils.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/__init__.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/componentmgr.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/data_streammgr.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/entitymgr.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/ilmmgr.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/indexmgr.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/snapshotmgr.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 es_testbed-0.6.0/src/es_testbed/mgrs/templatemgr.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 es_testbed-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_testbed-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 es_testbed-0.6.0/README.md
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 es_testbed-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 es_testbed-0.6.0/PKG-INFO
```

### Comparing `es_testbed-0.5.4/src/es_testbed/defaults.py` & `es_testbed-0.6.0/src/es_testbed/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 
 MAPPING: dict = {
     'properties': {
         '@timestamp': {'type': 'date'},
         'message': {'type': 'keyword'},
         'number': {'type': 'long'},
         'nested': {'properties': {'key': {'type': 'keyword'}}},
-        'deep': {'properties': {'l1': {'properties': {'l2': {'properties': {'l3': {'type': 'keyword'}}}}}}},
+        'deep': {
+            'properties': {
+                'l1': {
+                    'properties': {'l2': {'properties': {'l3': {'type': 'keyword'}}}}
+                }
+            }
+        },
     }
 }
 
 NAMEMAPPER: t.Dict[str, str] = {
     'index': 'idx',
     'data_stream': 'ds',
     'component': 'cmp',
@@ -43,15 +49,20 @@
 }
 
 TESTPLAN: dict = {
     'type': 'indices',
     'prefix': 'es-testbed',
     'repository': None,
     'rollover_alias': None,
-    'ilm': {'enabled': False, 'tiers': ['hot', 'delete'], 'forcemerge': False, 'max_num_segments': 1},
+    'ilm': {
+        'enabled': False,
+        'tiers': ['hot', 'delete'],
+        'forcemerge': False,
+        'max_num_segments': 1,
+    },
     'defaults': {
         'entity_count': 3,
         'docs': 10,
         'match': True,
         'searchable': None,
     },
     'entities': [],
@@ -71,15 +82,17 @@
         'storage': 'shared_cache',
     },
 }
 
 TIMEOUT_DEFAULT: str = '30'
 TIMEOUT_ENVVAR: str = 'ES_TESTBED_TIMEOUT'
 
-IlmPhase: t.TypeAlias = t.Dict[str, t.Union[str, t.Dict[str, str], t.Dict[str, t.Dict[str, t.Dict[str, str]]]]]
+IlmPhase: t.TypeAlias = t.Dict[
+    str, t.Union[str, t.Dict[str, str], t.Dict[str, t.Dict[str, t.Dict[str, str]]]]
+]
 
 
 def ilmhot() -> IlmPhase:
     return {'actions': {'rollover': {'max_primary_shard_size': '1gb', 'max_age': '1d'}}}
 
 
 def ilmwarm() -> IlmPhase:
```

### Comparing `es_testbed-0.5.4/src/es_testbed/exceptions.py` & `es_testbed-0.6.0/src/es_testbed/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class TestbedException(Exception):  # parent exception
     """
     Base class for all exceptions raised by the tool which are not Elasticsearch
     or es_client exceptions.
     """
 
+    __test__ = False
+
 
 class MissingArgument(TestbedException):
     """
     An expected argument was missing
     """
 
 
@@ -27,24 +29,30 @@
 
 
 class TestbedFailure(TestbedException):
     """
     Whatever we were trying to do failed.
     """
 
+    __test__ = False
+
 
 class TestbedMisconfig(TestbedException):
     """
     There was a misconfiguration encountered.
     """
 
+    __test__ = False
+
 
 class TestPlanMisconfig(TestbedMisconfig):
     """
     There was a misconfiguration in a TestPlan.
     """
 
+    __test__ = False
+
 
 class TimeoutException(TestbedException):
     """
     An process took too long to complete
     """
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/ilm.py` & `es_testbed-0.6.0/src/es_testbed/ilm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """ILM Defining Class"""
 
 import typing as t
 from os import getenv
 from time import sleep
 from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.defaults import PAUSE_ENVVAR, PAUSE_DEFAULT
-from es_testbed.exceptions import NameChanged, ResultNotExpected, TestbedMisconfig
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger
+from .defaults import PAUSE_ENVVAR, PAUSE_DEFAULT
+from .exceptions import NameChanged, ResultNotExpected, TestbedMisconfig
+from .helpers.es_api import get_ilm_phases, ilm_explain, ilm_move, resolver
+from .helpers.utils import getlogger
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
 
 # pylint: disable=missing-docstring
 
 # ## Example ILM explain output
 # {
@@ -45,56 +47,70 @@
 #     'step': 'complete',
 #     'step_time_millis': 0,
 #     'time_since_index_creation': '5.65m'
 # }
 
 
 class IlmTracker:
+    """ILM Phase Tracking Class"""
 
-    def __init__(self, client: Elasticsearch, name: str):
+    def __init__(self, client: 'Elasticsearch', name: str):
         self.logger = getlogger('es_testbed.IlmTracker')
         self.client = client
         self.name = self.resolve(name)  # A single index name
         self._explain = DotMap(self.get_explain_data())
-        self._phases = es_api.get_ilm_phases(self.client, self._explain.policy)
+        self._phases = get_ilm_phases(self.client, self._explain.policy)
 
     @property
-    def current_step(self) -> dict:
+    def current_step(self) -> t.Dict:
+        """Return the current ILM step information"""
         return {
             'phase': self._explain.phase,
             'action': self._explain.action,
             'name': self._explain.step,
         }
 
     @property
     def explain(self) -> DotMap:
+        """Return the current stored value of ILM Explain"""
         return self._explain
 
     @property
     def next_phase(self) -> str:
+        """Return the next phase in the index's ILM journey"""
         retval = None
         if self._explain.phase == 'delete':
             self.logger.warning('Already on "delete" phase. No more phases to advance')
         else:
-            curr = self.pnum(self._explain.phase)  # A numeric representation of the current phase
-            # A list of any remaining phases in the policy with a higher number than the current
-            remaining = [self.pnum(x) for x in self.policy_phases if self.pnum(x) > curr]
+            curr = self.pnum(self._explain.phase)  # A numeric representation
+            # A list of any remaining phases in the policy with a higher number than
+            # the current
+            remaining = [
+                self.pnum(x) for x in self.policy_phases if self.pnum(x) > curr
+            ]
             if remaining:  # If any:
                 retval = self.pname(remaining[0])
                 # Get the phase name from the number stored in the first element
         return retval
 
     @property
     def policy_phases(self) -> t.Sequence[str]:
+        """Return a list of phases in the ILM policy"""
         return list(self._phases.keys())
 
     def advance(
-        self, phase: t.Union[str, None] = None, action: t.Union[str, None] = None, name: t.Union[str, None] = None
+        self,
+        phase: t.Union[str, None] = None,
+        action: t.Union[str, None] = None,
+        name: t.Union[str, None] = None,
     ) -> None:
+        """Advance index to next ILM phase"""
+
         def wait(phase: str) -> None:
+            """Wait for the phase change"""
             counter = 0
             sleep(1.5)  # Initial wait since we set ILM to poll every second
             while self._explain.phase != phase:
                 sleep(PAUSE_VALUE)
                 self.update()
                 counter += 1
                 self.count_logging(counter)
@@ -102,44 +118,50 @@
         if self._explain.phase == 'delete':
             self.logger.warning('Already on "delete" phase. No more phases to advance')
         else:
             self.logger.debug('current_step: %s', self.current_step)
             next_step = self.next_step(phase, action=action, name=name)
             self.logger.debug('next_step: %s', next_step)
             if next_step:
-                es_api.ilm_move(self.client, self.name, self.current_step, next_step)
+                ilm_move(self.client, self.name, self.current_step, next_step)
                 wait(phase)
                 self.logger.info('Index %s now on phase %s', self.name, phase)
             else:
                 self.logger.error('next_step is a None value')
                 self.logger.error('current_step: %s', self.current_step)
 
     def count_logging(self, counter: int) -> None:
+        """Log messages based on how big counter is"""
         # Send a message every 10 loops
         if counter % 40 == 0:
             self.logger.info('Still working... Explain: %s', self._explain.asdict)
         if counter == 480:
             msg = 'Taking too long! Giving up on waiting'
             self.logger.critical(msg)
             raise ResultNotExpected(msg)
 
     def get_explain_data(self) -> t.Dict:
+        """Get the ILM explain data and return it"""
         try:
-            return es_api.ilm_explain(self.client, self.name)
+            return ilm_explain(self.client, self.name)
         except NameChanged as err:
             self.logger.debug('Passing along upstream exception...')
             raise NameChanged from err
         except ResultNotExpected as err:
             msg = f'Unable to get ilm_explain API call results. Error: {err}'
             self.logger.critical(msg)
             raise ResultNotExpected(msg) from err
 
     def next_step(
-        self, phase: t.Union[str, None] = None, action: t.Union[str, None] = None, name: t.Union[str, None] = None
+        self,
+        phase: t.Union[str, None] = None,
+        action: t.Union[str, None] = None,
+        name: t.Union[str, None] = None,
     ) -> t.Dict:
+        """Determine the next ILM step based on the current phase, action, and name"""
         err1 = bool((action is not None) and (name is None))
         err2 = bool((action is None) and (name is not None))
         if err1 or err2:
             msg = 'If either action or name is specified, both must be'
             self.logger.critical(msg)
             raise TestbedMisconfig(msg)
         if not phase:
@@ -147,53 +169,65 @@
         retval = {'phase': phase}
         if action:
             retval['action'] = action
             retval['name'] = name
         return retval
 
     def pnum(self, phase: str) -> int:
+        """Map a phase name to a phase number"""
         _ = {'new': 0, 'hot': 1, 'warm': 2, 'cold': 3, 'frozen': 4, 'delete': 5}
         return _[phase]
 
     def pname(self, num: int) -> str:
+        """Map a phase number to a phase name"""
         _ = {0: 'new', 1: 'hot', 2: 'warm', 3: 'cold', 4: 'frozen', 5: 'delete'}
         return _[num]
 
     def resolve(self, name: str) -> str:
         """Resolve that we have an index and NOT an alias or a datastream"""
-        res = es_api.resolver(self.client, name)
+        res = resolver(self.client, name)
         if len(res['aliases']) > 0 or len(res['data_streams']) > 0:
             msg = f'{name} is not an index: {res}'
             self.logger.critical(msg)
             raise ResultNotExpected(msg)
         if len(res['indices']) > 1:
-            msg = f'{name} resolved to multiple indices: {res['indices']}'
+            msg = f'{name} resolved to multiple indices: {res["indices"]}'
             self.logger.critical(msg)
             raise ResultNotExpected(msg)
         return res['indices'][0]['name']
 
     def update(self) -> None:
+        """Update self._explain with the latest from :py:meth:`get_explain_data`"""
         try:
             self._explain = DotMap(self.get_explain_data())
         except NameChanged as err:
             self.logger.debug('Passing along upstream exception...')
             raise NameChanged from err
 
     def wait4complete(self) -> None:
+        """Wait for the ILM phase change to complete both the action and step"""
         counter = 0
         self.logger.debug('Waiting for current action and step to complete')
-        self.logger.debug('Action: %s --- Step: %s', self._explain.action, self._explain.step)
-        while not bool(self._explain.action == 'complete' and self._explain.step == 'complete'):
+        self.logger.debug(
+            'Action: %s --- Step: %s', self._explain.action, self._explain.step
+        )
+        while not bool(
+            self._explain.action == 'complete' and self._explain.step == 'complete'
+        ):
             counter += 1
             sleep(PAUSE_VALUE)
             if counter % 10 == 0:
-                self.logger.debug('Action: %s --- Step: %s', self._explain.action, self._explain.step)
+                self.logger.debug(
+                    'Action: %s --- Step: %s', self._explain.action, self._explain.step
+                )
             try:
                 self.count_logging(counter)
             except ResultNotExpected as err:
-                self.logger.critical('Breaking the loop. Explain: %s', self._explain.toDict())
+                self.logger.critical(
+                    'Breaking the loop. Explain: %s', self._explain.toDict()
+                )
                 raise ResultNotExpected from err
             try:
                 self.update()
             except NameChanged as err:
                 self.logger.debug('Passing along upstream exception...')
                 raise NameChanged from err
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/plan.py` & `es_testbed-0.6.0/src/es_testbed/_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 """TestPlan Class Definition"""
 
 import typing as t
 from dotmap import DotMap
-from es_testbed.defaults import TESTPLAN
-from es_testbed.helpers.utils import build_ilm_policy, getlogger, randomstr
+from .defaults import TESTPLAN
+from .helpers.utils import build_ilm_policy, getlogger, randomstr
 
 # pylint: disable=missing-docstring
 
 
 class PlanBuilder:
 
-    def __init__(self, settings: t.Dict = None, default_entities: bool = True, autobuild: t.Optional[bool] = True):
+    def __init__(
+        self,
+        settings: t.Dict = None,
+        default_entities: bool = True,
+        autobuild: t.Optional[bool] = True,
+    ):
         self.logger = getlogger('es_testbed.PlanBuilder')
         self.default_entities = default_entities
         if settings is None:
             settings = TESTPLAN
         self.settings = settings
         self._plan = DotMap(TESTPLAN)
+        self._plan.cleanup = 'UNKNOWN'  # Future use?
         if autobuild:
             self.setup()
 
         # ## Example settings
         # settings={
         #   'type': 'indices',       # Default is indices? Or should it be data_streams?
         #   'prefix': 'es-testbed',  # Provide this value as a default
         #   'rollover_alias': False, # Only respected if 'type' == 'indices'.
-        #                            # Will rollover after creation and filling 1st index
-        #                            # If True, will be overridden to value of alias name
+        #                            # Will rollover after creation and filling 1st
+        #                            # If True, will be overridden to value of alias
         #                            # If False, will be overridden with None
-        #   'uniq': 'my-unique-str', # If not provided, randomstr(length=8, lowercase=True)
+        #   'uniq': 'my-unique-str', # If not provided, randomstr()
         #   'repository':            # Only used for cold/frozen tier for snapshots
         #   'ilm': {                 # All of these ILM values are defaults
         #     'enabled': False,
         #     'tiers': ['hot', 'delete'],
         #     'forcemerge': False,
         #     'max_num_segments': 1,
         #   }
         #
-        # # If these keys aren't specified per entity, then all entities will get this treatment
+        # # If these keys aren't specified per entity, then all entities will get this
+        # # treatment
         # # EXCEPT for the is_write_index for aliases and data_streams
         #
         #   'defaults': {
         #     'entity_count': 3,
         #     'docs': 10,
         #     'match': True,
         #     'searchable': tier...
         #   }
         #
-        # # Manually specifying entities makes sense for individual indices, but not so much for
+        # # Manually specifying entities makes sense for individual indices, but not so
+        # # much for
         # # alias-backed indices or data_streams
         #   'entities': [
         #    {
         #      'docs': 10,
         #      'match': True,
         #      'searchable': 'frozen'
         #    },
@@ -65,57 +73,58 @@
         #      'match': True,
         #      'searchable': 'hot'
         #    },
         #   ]
         # }
 
     @property
-    def plan(self):
+    def plan(self) -> DotMap:
         return self._plan
 
-    def _create_failsafes(self):
-        self._plan.failsafes = DotMap()
-        items = ['index', 'data_stream', 'snapshot', 'ilm', 'template', 'component', 'entity_type']
-        for i in items:
-            self._plan.failsafes[i] = []
-
-    def _create_lists(self):
+    def _create_lists(self) -> None:
         names = [
             'indices',
             'data_stream',
             'snapshots',
             'ilm_policies',
             'index_templates',
             'component_templates',
-            'entity_mgrs',
         ]
         for name in names:
             self._plan[name] = []
 
     def add_entity(
-        self, docs: t.Optional[int] = 10, match: t.Optional[bool] = True, searchable: t.Optional[str] = None
+        self,
+        docs: t.Optional[int] = 10,
+        match: t.Optional[bool] = True,
+        searchable: t.Optional[str] = None,
     ) -> None:
         entity = {'docs': docs, 'match': match}
         if searchable:
             entity['searchable'] = searchable
         self._plan.entities.append(entity)
 
     def make_default_entities(self) -> None:
         defs = TESTPLAN['defaults']  # Start with defaults
         if 'defaults' in self._plan:
             defs = self._plan.defaults
-        kwargs = {'docs': defs['docs'], 'match': defs['match'], 'searchable': defs['searchable']}
+        kwargs = {
+            'docs': defs['docs'],
+            'match': defs['match'],
+            'searchable': defs['searchable'],
+        }
         for _ in range(0, defs['entity_count']):
             self.add_entity(**kwargs)
-        self.logger.debug('Plan will create %s (backing) indices', len(self._plan.entities))
+        self.logger.debug(
+            'Plan will create %s (backing) indices', len(self._plan.entities)
+        )
 
     def setup(self) -> None:
         self._plan.uniq = randomstr(length=8, lowercase=True)
         self._create_lists()
-        self._create_failsafes()
         self.update(self.settings)  # Override with settings.
         self.update_rollover_alias()
         self.update_ilm()
         if not self._plan.entities:
             if self.default_entities:
                 self.make_default_entities()
         self.logger.debug('Test Plan: %s', self._plan.pprint())
@@ -130,19 +139,23 @@
             setdefault = True
         if isinstance(self._plan.ilm, dict):
             _ = DotMap(self._plan.ilm)
             self._plan.ilm = _
         if isinstance(self._plan.ilm, DotMap):
             if 'enabled' not in self._plan.ilm:
                 # Override with defaults
-                self.logger.debug('plan.ilm does not have key "enabled". Overriding with defaults')
+                self.logger.debug(
+                    'plan.ilm does not have key "enabled". Overriding with defaults'
+                )
                 setdefault = True
         elif isinstance(self._plan.ilm, bool):
             if self._plan.ilm:
-                self.logger.warning('"plan.ilm: True" is incorrect. Use plan.ilm.enabled: True')
+                self.logger.warning(
+                    '"plan.ilm: True" is incorrect. Use plan.ilm.enabled: True'
+                )
             self.logger.debug('plan.ilm is boolean. Overriding with defaults')
             setdefault = True
         if setdefault:
             self.logger.debug('Setting defaults for ILM')
             self._plan.ilm = DotMap(TESTPLAN['ilm'])
         ilm = self._plan.ilm
         for entity in self._plan.entities:
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entities/alias.py` & `es_testbed-0.6.0/src/es_testbed/entities/alias.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """Alias Entity Class"""
 
 import typing as t
-from elasticsearch8 import Elasticsearch
-from es_testbed.helpers.utils import getlogger
-from es_testbed.helpers import es_api
 from .entity import Entity
+from ..helpers.es_api import resolver, rollover
+from ..helpers.utils import getlogger
+
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Alias(Entity):
 
-    def __init__(self, client: Elasticsearch, name: str = None, autobuild: t.Optional[bool] = True):
-        super().__init__(client=client, name=name, autobuild=autobuild)
+    def __init__(
+        self,
+        client: 'Elasticsearch',
+        name: t.Union[str, None] = None,
+    ):
         self.logger = getlogger('es_testbed.Alias')
+        super().__init__(client=client, name=name)
 
     def rollover(self) -> None:
-        es_api.rollover(self.client, self.name)
+        rollover(self.client, self.name)
 
     def verify(self, index_list: t.Sequence[str]) -> bool:
         retval = False
-        res = es_api.resolver(self.client, self.name)
+        res = resolver(self.client, self.name)
         for idx, alias in enumerate(res['aliases']):
             if alias['name'] == self.name:
                 self.logger.debug('Confirm match of alias %s at index %s', alias, idx)
             else:
                 continue
             if alias['indices'] == index_list:
-                self.logger.debug('Confirm match of indices backed by alias %s', self.name)
+                self.logger.debug(
+                    'Confirm match of indices backed by alias %s', self.name
+                )
                 retval = True
                 break
         return retval
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entities/entity.py` & `es_testbed-0.6.0/src/es_testbed/entities/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """Base Entity Class"""
 
 import typing as t
-from elasticsearch8 import Elasticsearch
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger
+from ..helpers.es_api import find_write_index, get_ds_current, resolver
 
-# pylint: disable=missing-docstring,too-many-arguments
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+
+# pylint: disable=missing-docstring,too-many-arguments,R0903
 
 
 class Entity:
 
-    def __init__(self, client: Elasticsearch, name: str = None, autobuild: t.Optional[bool] = True):
+    def __init__(
+        self,
+        client: 'Elasticsearch',
+        name: t.Union[str, None] = None,
+    ):
         self.client = client
         self.name = name  # This will change with entity name changes
         self.aka = []  # Aliases, in other words
-        self.logger = getlogger('es_testbed.Entity')
-        if autobuild:
-            self.setup()
 
     @property
     def am_i_write_idx(self) -> bool:
         if self.name.startswith('.ds-'):  # Datastream
-            ds = es_api.resolver(self.client, self.name)['indices'][0]['data_stream']
-            return bool(self.name == es_api.get_ds_current(self.client, ds))
-        return bool(self.name == es_api.find_write_index(self.client, self.name))
-
-    def setup(self):
-        pass
-
-    def teardown(self):
-        pass
+            ds = resolver(self.client, self.name)['indices'][0]['data_stream']
+            return bool(self.name == get_ds_current(self.client, ds))
+        return bool(self.name == find_write_index(self.client, self.name))
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entities/index.py` & `es_testbed-0.6.0/src/es_testbed/entities/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 """Index Entity Class"""
 
 import typing as t
 from os import getenv
-from elasticsearch8 import Elasticsearch
 from es_wait import Exists
-from es_testbed.defaults import PAUSE_DEFAULT, PAUSE_ENVVAR, TIMEOUT_DEFAULT, TIMEOUT_ENVVAR
-from es_testbed.exceptions import NameChanged, ResultNotExpected
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger, mounted_name
 from .entity import Entity
 from ..ilm import IlmTracker
+from ..defaults import (
+    PAUSE_DEFAULT,
+    PAUSE_ENVVAR,
+    TIMEOUT_DEFAULT,
+    TIMEOUT_ENVVAR,
+)
+from ..exceptions import NameChanged, ResultNotExpected
+from ..helpers.es_api import snapshot_name
+from ..helpers.utils import getlogger, mounted_name
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
 TIMEOUT_VALUE = float(getenv(TIMEOUT_ENVVAR, default=TIMEOUT_DEFAULT))
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Index(Entity):
 
     def __init__(
         self,
-        client: Elasticsearch = None,
-        name: str = None,
-        autobuild: t.Optional[bool] = True,
+        client: 'Elasticsearch',
+        name: t.Union[str, None] = None,
         snapmgr=None,
         policy_name: str = None,
     ):
-        super().__init__(client=client, name=name, autobuild=autobuild)
         self.logger = getlogger('es_testbed.Index')
+        super().__init__(client=client, name=name)
         self.policy_name = policy_name
         self.ilm_tracker = None
         self.snapmgr = snapmgr
         self.track_ilm(self.name)
 
     @property
     def _get_target(self) -> str:
@@ -56,71 +62,99 @@
         return target
 
     @property
     def phase_tuple(self) -> t.Tuple[str, str]:
         """Return the current phase and the target phase as a Tuple"""
         return self.ilm_tracker.explain.phase, self._get_target
 
-    def _loop_until_target(self):
-        current, target = self.phase_tuple
-        while current != target:
-            self.logger.debug('Attempting to move %s to ILM phase %s', self.name, target)
-            self.ilm_tracker.advance(phase=target)
-            # At this point, it's "in" a searchable tier, but the index name hasn't changed yet
-            newidx = mounted_name(self.name, target)
-            self.logger.debug('Waiting for ILM phase change to complete. New index: %s', newidx)
-            kwargs = {'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
-            test = Exists(self.client, **kwargs)
-            test.wait_for_it()
-            self.logger.info('ILM advance to phase %s completed', target)
-            self.aka.append(self.name)  # Append the old name to the AKA list
-            self.name = newidx
-            self.track_ilm(self.name)  # Refresh the ilm_tracker with the new index name
-            current, target = self.phase_tuple
+    # This is maybe unnecessary. This is for progressing ILM, e.g. from
+    # hot -> warm -> cold -> frozen (and even through delete).
+    #
+    # def _loop_until_target(self) -> None:
+    #     current, target = self.phase_tuple
+    #     while current != target:
+    #         self.logger.debug(
+    #             'Attempting to move %s to ILM phase %s', self.name, target
+    #         )
+    #         self.ilm_tracker.advance(phase=target)
+    #         # At this point, it's "in" a searchable tier, but the index name hasn't
+    #         # changed yet
+    #         newidx = mounted_name(self.name, target)
+    #         self.logger.debug(
+    #             'Waiting for ILM phase change to complete. New index: %s', newidx
+    #         )
+    #         kwargs = {
+    #             'name': newidx,
+    #             'kind': 'index',
+    #             'pause': PAUSE_VALUE,
+    #             'timeout': TIMEOUT_VALUE,
+    #         }
+    #         test = Exists(self.client, **kwargs)
+    #         test.wait_for_it()
+    #         self.logger.info('ILM advance to phase %s completed', target)
+    #         self.aka.append(self.name)  # Append the old name to the AKA list
+    #         self.name = newidx
+    #         self.track_ilm(self.name)  # Refresh the ilm_tracker with the new name
+    #         current, target = self.phase_tuple
 
     def manual_ss(self, scheme) -> None:
-        """If we are NOT using ILM but have specified searchable snapshots in the plan entities"""
+        """
+        If we are NOT using ILM but have specified searchable snapshots in the plan
+        entities
+        """
         if 'searchable' in scheme and scheme['searchable'] is not None:
             self.snapmgr.add(self.name, scheme['searchable'])
             # Replace self.name with the renamed name
             self.name = mounted_name(self.name, scheme['searchable'])
 
     def mount_ss(self, scheme: dict) -> None:
         """If the index is planned to become a searchable snapshot, we do that now"""
         self.logger.debug('Checking if %s should be a searchable snapshot', self.name)
         if self.am_i_write_idx:
-            self.logger.info('%s is the write_index. Cannot mount as searchable snapshot', self.name)
+            self.logger.debug(
+                '%s is the write_index. Cannot mount as searchable snapshot', self.name
+            )
             return
         if not self.policy_name:  # If we have this, chances are we have a policy
             self.logger.debug('No ILM policy found. Switching to manual mode')
             self.manual_ss(scheme)
             return
         current = self.ilm_tracker.explain.phase
         target = self._get_target
         if current != target:
-            self.logger.debug('Attempting to move %s to ILM phase %s', self.name, target)
+            self.logger.debug(
+                'Attempting to move %s to ILM phase %s', self.name, target
+            )
             self.ilm_tracker.advance(phase=target)
-            # At this point, it's "in" a searchable tier, but the index name hasn't changed yet
+            # At this point, it's "in" a searchable tier, but the index name hasn't
+            # changed yet
             newidx = mounted_name(self.name, target)
-            self.logger.debug('Waiting for ILM phase change to complete. New index: %s', newidx)
-            kwargs = {'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
+            self.logger.debug(
+                'Waiting for ILM phase change to complete. New index: %s', newidx
+            )
+            kwargs = {
+                'name': newidx,
+                'kind': 'index',
+                'pause': PAUSE_VALUE,
+                'timeout': TIMEOUT_VALUE,
+            }
             test = Exists(self.client, **kwargs)
             test.wait_for_it()
             try:
                 self.ilm_tracker.wait4complete()
             except NameChanged:
                 try:
                     self.track_ilm(newidx)
                     self.ilm_tracker.wait4complete()
                 except NameChanged as err:
                     self.logger.critical('Index name mismatch. Cannot continue')
                     raise ResultNotExpected from err
             self.logger.info('ILM advance to phase %s completed', target)
             self.logger.debug('Getting snapshot name for tracking...')
-            snapname = es_api.snapshot_name(self.client, newidx)
+            snapname = snapshot_name(self.client, newidx)
             self.logger.debug('Snapshot %s backs %s', snapname, newidx)
             self.snapmgr.add_existing(snapname)
             self.aka.append(self.name)  # Append the old name to the AKA list
             self.name = newidx
             self.track_ilm(self.name)  # Refresh the ilm_tracker with the new index name
 
     def track_ilm(self, name: str) -> None:
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/componentmgr.py` & `es_testbed-0.6.0/src/es_testbed/mgrs/componentmgr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 """Component Template Entity Manager Class"""
 
 import typing as t
-from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.exceptions import ResultNotExpected
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger, mapping_component, setting_component
 from .entitymgr import EntityMgr
+from ..exceptions import ResultNotExpected
+from ..helpers.es_api import exists, put_comp_tmpl
+from ..helpers.utils import getlogger, mapping_component, setting_component
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+    from dotmap import DotMap
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class ComponentMgr(EntityMgr):
     kind = 'component'
     listname = 'component_templates'
 
-    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = True):
-        super().__init__(client=client, plan=plan, autobuild=autobuild)
+    def __init__(
+        self,
+        client: t.Union['Elasticsearch', None] = None,
+        plan: t.Union['DotMap', None] = None,
+        autobuild: t.Optional[bool] = True,
+    ):
         self.logger = getlogger('es_testbed.ComponentMgr')
+        super().__init__(client=client, plan=plan, autobuild=autobuild)
 
     @property
-    def components(self):
+    def components(self) -> t.Sequence[t.Dict]:
+        """Return a list of component template dictionaries"""
         retval = []
-        kw = {'ilm_policy': self.plan.ilm_policies[-1], 'rollover_alias': self.plan.rollover_alias}
+        kw = {
+            'ilm_policy': self.plan.ilm_policies[-1],
+            'rollover_alias': self.plan.rollover_alias,
+        }
         retval.append(setting_component(**kw))
         retval.append(mapping_component())
         return retval
 
-    @property
-    def logdisplay(self) -> str:
-        return 'component template'
-
-    def setup(self):
+    def setup(self) -> None:
+        """Setup the entity manager"""
         for component in self.components:
-            es_api.put_comp_tmpl(self.client, self.name, component)
-            if not es_api.exists(self.client, self.kind, self.name):
-                raise ResultNotExpected(f'Unable to verify creation of component template {self.name}')
+            put_comp_tmpl(self.client, self.name, component)
+            if not exists(self.client, self.kind, self.name):
+                raise ResultNotExpected(
+                    f'Unable to verify creation of component template {self.name}'
+                )
             self.appender(self.name)
-            self.logger.info('Created component template: "%s"', self.last)
-        self.logger.info('Successfully created all component templates.')
+        self.logger.info(
+            'Successfully created all component templates: %s', self.entity_list
+        )
         self.success = True
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/ilmmgr.py` & `es_testbed-0.6.0/src/es_testbed/mgrs/ilmmgr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 """ILM Policy Entity Manager Class"""
 
 import typing as t
-from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.exceptions import ResultNotExpected
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import build_ilm_policy, getlogger
 from .entitymgr import EntityMgr
+from ..exceptions import ResultNotExpected
+from ..helpers.es_api import exists, put_ilm
+from ..helpers.utils import build_ilm_policy, getlogger
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+    from dotmap import DotMap
 
 # pylint: disable=missing-docstring
 
 
 class IlmMgr(EntityMgr):
     kind = 'ilm'
     listname = 'ilm_policies'
 
-    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = True):
-        super().__init__(client=client, plan=plan, autobuild=autobuild)
+    def __init__(
+        self,
+        client: t.Union['Elasticsearch', None] = None,
+        plan: t.Union['DotMap', None] = None,
+        autobuild: t.Optional[bool] = True,
+    ):
         self.logger = getlogger('es_testbed.IlmMgr')
+        super().__init__(client=client, plan=plan, autobuild=autobuild)
 
-    @property
-    def logdisplay(self) -> str:
-        return 'ILM policy'
-
-    def get_policy(self):
+    def get_policy(self) -> t.Dict:
+        """Return the configured ILM policy"""
         d = self.plan.ilm
         kwargs = {
             'tiers': d.tiers,
             'forcemerge': d.forcemerge,
             'max_num_segments': d.max_num_segments,
             'repository': self.plan.repository,
         }
         return build_ilm_policy(**kwargs)
 
-    def setup(self):
+    def setup(self) -> None:
+        """Setup the entity manager"""
         if self.plan.ilm.enabled:
             self.plan.ilm.policy = self.get_policy()
-            es_api.put_ilm(self.client, self.name, policy=self.plan.ilm.policy)
+            put_ilm(self.client, self.name, policy=self.plan.ilm.policy)
             # Verify existence
-            if not es_api.exists(self.client, 'ilm', self.name):
-                raise ResultNotExpected(f'Unable to verify creation of ilm policy {self.name}')
+            if not exists(self.client, 'ilm', self.name):
+                raise ResultNotExpected(
+                    f'Unable to verify creation of ilm policy {self.name}'
+                )
             # This goes first because the length of entity_list determines the suffix
             self.appender(self.name)
             self.logger.info('Successfully created ILM policy: %s', self.last)
         else:
             self.appender(None)  # This covers self.plan.ilm_policies[-1]
             self.logger.info('No ILM policy created.')
         self.success = True
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/indexmgr.py` & `es_testbed-0.6.0/src/es_testbed/mgrs/indexmgr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,136 @@
 """Index Entity Manager Class"""
 
 import typing as t
-from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger, setting_component
 from .entitymgr import EntityMgr
 from .snapshotmgr import SnapshotMgr
 from ..entities import Alias, Index
+from ..helpers.es_api import create_index, fill_index
+from ..helpers.utils import getlogger, setting_component
 
-# pylint: disable=missing-docstring,too-many-arguments,broad-exception-caught,too-many-instance-attributes
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+    from dotmap import DotMap
+
+# pylint: disable=missing-docstring
 
 
 class IndexMgr(EntityMgr):
     kind = 'index'
     listname = 'indices'
 
     def __init__(
         self,
-        client: Elasticsearch = None,
-        plan: DotMap = None,
+        client: t.Union['Elasticsearch', None] = None,
+        plan: t.Union['DotMap', None] = None,
         autobuild: t.Optional[bool] = True,
-        snapmgr: SnapshotMgr = None,
+        snapmgr: t.Union[SnapshotMgr, None] = None,
     ):
         self.doc_incr = 0
         self.snapmgr = snapmgr
         self.alias = None  # Only used for tracking the rollover alias
-        super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.IndexMgr')
+        super().__init__(client=client, plan=plan, autobuild=autobuild)
 
     @property
     def indexlist(self) -> t.Sequence[str]:
+        """Return a list of index names currently being managed"""
         return [x.name for x in self.entity_list]
 
     @property
-    def policy_name(self) -> str:
+    def policy_name(self) -> t.Union[str, None]:
+        """Return the name of the ILM policy, if it exists"""
         if len(self.plan.ilm_policies) > 0:
             return self.plan.ilm_policies[-1]
         return None
 
     def _rollover_path(self) -> None:
+        """This is the execution path for rollover indices"""
         if not self.entity_list:
-            kw = {'ilm_policy': self.policy_name, 'rollover_alias': self.plan.rollover_alias}
+            kw = {
+                'ilm_policy': self.policy_name,
+                'rollover_alias': self.plan.rollover_alias,
+            }
             cfg = setting_component(**kw)['settings']
             acfg = {self.plan.rollover_alias: {'is_write_index': True}}
-            self.logger.debug('No indices created yet. Starting with a rollover alias index...')
-            es_api.create_index(self.client, self.name, aliases=acfg, settings=cfg)
-            self.logger.debug('Created %s with rollover alias %s', self.name, self.plan.rollover_alias)
+            self.logger.debug(
+                'No indices created yet. Starting with a rollover alias index...'
+            )
+            create_index(self.client, self.name, aliases=acfg, settings=cfg)
+            self.logger.debug(
+                'Created %s with rollover alias %s', self.name, self.plan.rollover_alias
+            )
             self.track_alias()
         else:
             self.alias.rollover()
             if self.policy_name:  # We have an ILM policy
                 self.logger.debug('Going to wait now...')
                 self.last.ilm_tracker.wait4complete()
                 self.logger.debug('The wait is over!')
 
     def add(self, value) -> None:
+        """Create a single index"""
         # In this case, value is a single array element from plan.entities
         self.logger.debug('Creating index: %s', value)
-        es_api.create_index(self.client, value)
+        create_index(self.client, value)
 
     def add_indices(self) -> None:
+        """Add indices according to plan"""
         for scheme in self.plan.entities:
             if self.plan.rollover_alias:
                 self._rollover_path()
             else:
                 self.add(self.name)
             self.filler(scheme)
             self.track_index(self.name)
         self.logger.debug('Created indices: %s', self.indexlist)
         if self.plan.rollover_alias:
             if not self.alias.verify(self.indexlist):
-                self.logger.error('Unable to confirm rollover of alias "%s" was successfully executed')
+                self.logger.error(
+                    'Unable to confirm rollover of alias "%s" was successfully executed'
+                )
 
     def filler(self, scheme) -> None:
         """If the scheme from the TestPlan says to write docs, do it"""
         # scheme is a single array element from plan.entities
         self.logger.debug('Adding docs to %s', self.name)
         if scheme['docs'] > 0:
-            es_api.fill_index(
-                self.client, name=self.name, count=scheme['docs'], start_num=self.doc_incr, match=scheme['match']
+            fill_index(
+                self.client,
+                name=self.name,
+                count=scheme['docs'],
+                start_num=self.doc_incr,
+                match=scheme['match'],
             )
         self.doc_incr += scheme['docs']
 
     def searchable(self) -> None:
         """If the indices were marked as searchable snapshots, we do that now"""
         for idx, scheme in enumerate(self.plan.entities):
-            old = self.entity_list[idx].name
             self.entity_list[idx].mount_ss(scheme)
-            new = self.entity_list[idx].name
-            # Replace the old index name in self.failsafe with the new one at the same list position
-            pos = [i for i, value in enumerate(self.failsafe) if value == old]
-            self.failsafe[pos[0]] = new
 
     def setup(self) -> None:
+        """Setup the entity manager"""
         self.logger.debug('Beginning setup...')
         if self.plan.rollover_alias:
             self.logger.debug('rollover_alias is True...')
         self.add_indices()
         self.searchable()
         self.logger.info('Successfully created indices: %s', self.indexlist)
         self.success = True
 
     def track_alias(self) -> None:
+        """Track a rollover alias"""
         self.logger.debug('Tracking alias: %s', self.plan.rollover_alias)
         self.alias = Alias(client=self.client, name=self.plan.rollover_alias)
 
     def track_index(self, name: str) -> None:
+        """Track an index and append that tracking entity to entity_list"""
         self.logger.debug('Tracking index: %s', name)
-        entity = Index(client=self.client, name=name, snapmgr=self.snapmgr, policy_name=self.policy_name)
-        self.failsafe.append(name)
+        entity = Index(
+            client=self.client,
+            name=name,
+            snapmgr=self.snapmgr,
+            policy_name=self.policy_name,
+        )
         self.entity_list.append(entity)
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/snapshotmgr.py` & `es_testbed-0.6.0/src/es_testbed/mgrs/templatemgr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-"""Snapshot Entity Manager Class"""
+"""Index Template Entity Manager Class"""
 
 import typing as t
-from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger
 from .entitymgr import EntityMgr
-
-# pylint: disable=missing-docstring
-
-
-class SnapshotMgr(EntityMgr):
-    kind = 'snapshot'
-    listname = 'snapshots'
-
-    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = False):
+from ..exceptions import ResultNotExpected
+from ..helpers.es_api import exists, put_idx_tmpl
+from ..helpers.utils import getlogger
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+    from dotmap import DotMap
+
+# pylint: disable=missing-docstring,too-many-arguments
+
+
+class TemplateMgr(EntityMgr):
+    """Index Template entity manager"""
+
+    kind = 'template'
+    listname = 'index_templates'
+
+    def __init__(
+        self,
+        client: t.Union['Elasticsearch', None] = None,
+        plan: t.Union['DotMap', None] = None,
+        autobuild: t.Optional[bool] = True,
+    ):
+        self.logger = getlogger('es_testbed.TemplateMgr')
         super().__init__(client=client, plan=plan, autobuild=autobuild)
-        self.logger = getlogger('es_testbed.SnapshotMgr')
 
-    def add(self, index: str, tier: str) -> None:
-        msg = f'Creating snapshot of index {index} and mounting in the {tier} tier...'
-        self.logger.info(msg)
-        es_api.do_snap(self.client, self.plan.repository, self.name, index, tier=tier)
+    @property
+    def patterns(self) -> t.Sequence[str]:
+        """Return the list of index patterns associated with this template"""
+        _ = []
+        _.append(f"{self.get_pattern('index')}*")
+        _.append(f"{self.get_pattern('data_stream')}*")
+        return _
+
+    def get_pattern(self, kind: str) -> str:
+        """Return the a formatted index search pattern string"""
+        return f'{self.plan.prefix}-{self.ident(dkey=kind)}-{self.plan.uniq}'
+
+    def setup(self) -> None:
+        """Setup the entity manager"""
+        ds = {} if self.plan.type == 'data_stream' else None
+        put_idx_tmpl(
+            self.client,
+            self.name,
+            self.patterns,
+            components=self.plan.component_templates,
+            data_stream=ds,
+        )
+        if not exists(self.client, self.kind, self.name):
+            raise ResultNotExpected(
+                f'Unable to verify creation of index template {self.name}'
+            )
         self.appender(self.name)
-        self.logger.info('Successfully created snapshot "%s"', self.last)
+        self.logger.info('Successfully created index template: %s', self.last)
         self.success = True
-
-    def add_existing(self, name: str) -> None:
-        """Add a snapshot that's already been created, e.g. by ILM promotion"""
-        self.logger.info('Adding snapshot %s to list...', name)
-        self.appender(name)
-        self.success = True
-
-    def setup(self):
-        pass
-
-    def teardown(self):  # We override the parent method here to speed things up.
-        if self.entity_list:
-            if not self.success:
-                msg = f'Setup did not complete successfully. ' f'Manual cleanup of {self.kind}s may be necessary.'
-                self.logger.warning(msg)
-            self.logger.info('Cleaning up any existing snapshots...')
-            es_api.delete(self.client, self.kind, ','.join(self.entity_list), repository=self.plan.repository)
-            self.logger.info('Cleanup of snapshots completed.')
-            self.entity_list = []
-            self.failsafe = []
```

### Comparing `es_testbed-0.5.4/src/es_testbed/classes/entitymgrs/templatemgr.py` & `es_testbed-0.6.0/src/es_testbed/mgrs/snapshotmgr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-"""Index Template Entity Manager Class"""
+"""Snapshot Entity Manager Class"""
 
 import typing as t
-from dotmap import DotMap
-from elasticsearch8 import Elasticsearch
-from es_testbed.exceptions import ResultNotExpected
-from es_testbed.helpers import es_api
-from es_testbed.helpers.utils import getlogger
 from .entitymgr import EntityMgr
+from ..helpers.es_api import do_snap
+from ..helpers.utils import getlogger
 
-# pylint: disable=missing-docstring,too-many-arguments
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
+    from dotmap import DotMap
 
+# pylint: disable=missing-docstring
 
-class TemplateMgr(EntityMgr):
-    kind = 'template'
-    listname = 'index_templates'
+
+class SnapshotMgr(EntityMgr):
+    kind = 'snapshot'
+    listname = 'snapshots'
 
     def __init__(
-        self, client: t.Union[Elasticsearch, None] = None, plan: DotMap = None, autobuild: t.Optional[bool] = True
+        self,
+        client: t.Union['Elasticsearch', None] = None,
+        plan: t.Union['DotMap', None] = None,
+        autobuild: t.Optional[bool] = False,
     ):
+        self.logger = getlogger('es_testbed.SnapshotMgr')
         super().__init__(client=client, plan=plan, autobuild=autobuild)
-        self.logger = getlogger('es_testbed.TemplateMgr')
 
-    @property
-    def logdisplay(self) -> str:
-        return 'index template'
-
-    @property
-    def patterns(self) -> t.Sequence[str]:
-        _ = []
-        _.append(f"{self.get_pattern('index')}*")
-        _.append(f"{self.get_pattern('data_stream')}*")
-        return _
-
-    def get_pattern(self, kind: str) -> str:
-        return f'{self.plan.prefix}-{self.ident(dkey=kind)}-{self.plan.uniq}'
-
-    def setup(self):
-        ds = {} if self.plan.type == 'data_stream' else None
-        es_api.put_idx_tmpl(
-            self.client, self.name, self.patterns, components=self.plan.component_templates, data_stream=ds
-        )
-        if not es_api.exists(self.client, self.kind, self.name):
-            raise ResultNotExpected(f'Unable to verify creation of index template {self.name}')
+    def add(self, index: str, tier: str) -> None:
+        """Perform a snapshot and add it to the entity_list"""
+        msg = f'Creating snapshot of index {index} and mounting in the {tier} tier...'
+        self.logger.info(msg)
+        do_snap(self.client, self.plan.repository, self.name, index, tier=tier)
         self.appender(self.name)
-        self.logger.debug('Successfully created index template: %s', self.last)
+        self.logger.info('Successfully created snapshot "%s"', self.last)
+        self.success = True
+
+    def add_existing(self, name: str) -> None:
+        """Add a snapshot that's already been created, e.g. by ILM promotion"""
+        self.logger.info('Adding snapshot %s to list...', name)
+        self.appender(name)
         self.success = True
```

### Comparing `es_testbed-0.5.4/src/es_testbed/helpers/es_api.py` & `es_testbed-0.6.0/src/es_testbed/helpers/es_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 """Functions that make Elasticsearch API Calls"""
 
 import typing as t
 from os import getenv
-from elasticsearch8 import Elasticsearch, exceptions as esx
+from elasticsearch8.exceptions import NotFoundError
 from es_wait import Exists, Snapshot
-from es_testbed.defaults import MAPPING, PAUSE_DEFAULT, PAUSE_ENVVAR
-from es_testbed import exceptions as exc
-from es_testbed.helpers.utils import doc_gen, get_routing, getlogger, mounted_name, storage_type
+from ..defaults import MAPPING, PAUSE_DEFAULT, PAUSE_ENVVAR
+from ..exceptions import (
+    NameChanged,
+    ResultNotExpected,
+    TestbedFailure,
+    TestbedMisconfig,
+    TimeoutException,
+)
+from ..helpers.utils import (
+    doc_gen,
+    get_routing,
+    getlogger,
+    mounted_name,
+    storage_type,
+)
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 LOGGER = getlogger(__name__)
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
-# pylint: disable=broad-except
+# pylint: disable=broad-except,W0707
 
 
-def emap(kind: str, es: Elasticsearch, value=None) -> t.Dict[str, t.Any]:
+def emap(kind: str, es: 'Elasticsearch', value=None) -> t.Dict[str, t.Any]:
     """Return a value from a dictionary"""
     _ = {
         'alias': {
             'delete': es.indices.delete_alias,
             'exists': es.indices.exists_alias,
             'get': es.indices.get_alias,
             'kwargs': {'index': value, 'expand_wildcards': ['open', 'closed']},
@@ -61,88 +76,121 @@
             'plural': 'component template(s)',
             'key': 'component_templates',
         },
         'snapshot': {
             'delete': es.snapshot.delete,
             'exists': es.snapshot.get,
             'get': es.snapshot.get,
-            'kwargs': {},
+            'kwargs': {'snapshot': value},
             'plural': 'snapshot(s)',
         },
     }
     return _[kind]
 
 
-def change_ds(client: Elasticsearch, actions: t.Union[str, None] = None) -> None:
+def change_ds(client: 'Elasticsearch', actions: t.Union[str, None] = None) -> None:
     """Change/Modify/Update a datastream"""
     try:
         client.indices.modify_data_stream(actions=actions, body=None)
     except Exception as err:
-        raise exc.ResultNotExpected(f'Unable to modify datastreams. {err}') from err
+        raise ResultNotExpected(f'Unable to modify datastreams. {err}') from err
 
 
-def create_data_stream(client: Elasticsearch, name: str) -> None:
+def create_data_stream(client: 'Elasticsearch', name: str) -> None:
     """Create a datastream"""
     try:
         client.indices.create_data_stream(name=name)
         test = Exists(client, name=name, kind='datastream', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(f'Unable to create datastream {name}. Error: {err}') from err
+        raise TestbedFailure(
+            f'Unable to create datastream {name}. Error: {err}'
+        ) from err
 
 
 def create_index(
-    client: Elasticsearch,
+    client: 'Elasticsearch',
     name: str,
     aliases: t.Union[t.Dict, None] = None,
     settings: t.Union[t.Dict, None] = None,
     tier: str = 'hot',
 ) -> None:
     """Create named index"""
     if not settings:
         settings = get_routing(tier=tier)
     else:
         settings.update(get_routing(tier=tier))
-    client.indices.create(index=name, aliases=aliases, mappings=MAPPING, settings=settings)
+    client.indices.create(
+        index=name, aliases=aliases, mappings=MAPPING, settings=settings
+    )
     try:
         test = Exists(client, name=name, kind='index', pause=PAUSE_VALUE)
         test.wait_for_it()
-    except exc.TimeoutException as err:
-        raise exc.ResultNotExpected(f'Failed to create index {name}') from err
+    except TimeoutException as err:
+        raise ResultNotExpected(f'Failed to create index {name}') from err
     return exists(client, 'index', name)
 
 
-def delete(client: Elasticsearch, kind: str, name: str, repository: t.Union[str, None] = None) -> None:
+def verify(
+    client: 'Elasticsearch',
+    kind: str,
+    name: str,
+    repository: t.Union[str, None] = None,
+) -> bool:
+    """Verify that whatever was deleted is actually deleted"""
+    success = True
+    items = ','.split(name)
+    for item in items:
+        result = exists(client, kind, item, repository=repository)
+        if result:  # That means it's still in the cluster
+            success = False
+    return success
+
+
+def delete(
+    client: 'Elasticsearch',
+    kind: str,
+    name: str,
+    repository: t.Union[str, None] = None,
+) -> bool:
     """Delete the named object of type kind"""
     which = emap(kind, client)
     func = which['delete']
-    if name is None:  # Typically only with ilm
-        LOGGER.debug('"%s" has a None value for name', kind)
-        return
-    try:
-        if kind == 'snapshot':
-            func(snapshot=name, repository=repository)
-        elif kind == 'index':
-            func(index=name)
+    success = False
+    if name is not None:  # Typically only with ilm
+        try:
+            if kind == 'snapshot':
+                res = func(snapshot=name, repository=repository)
+            elif kind == 'index':
+                res = func(index=name)
+            else:
+                res = func(name=name)
+        except NotFoundError as err:
+            LOGGER.warning('%s named %s not found: %s', kind, name, err)
+            success = True
+        except Exception as err:
+            raise ResultNotExpected(f'Unexpected result: {err}') from err
+        if 'acknowledged' in res and res['acknowledged']:
+            success = True
+            LOGGER.info('Deleted %s: "%s"', which['plural'], name)
         else:
-            func(name=name)
-    except esx.NotFoundError:
-        LOGGER.warning('%s named %s not found.', kind, name)
-    except Exception as err:
-        raise exc.ResultNotExpected(f'Unexpected result: {err}') from err
-    if exists(client, kind, name, repository=repository):
-        LOGGER.critical('Unable to delete "%s" %s', kind, name)
-        raise exc.ResultNotExpected(f'{kind} "{name}" still exists.')
-    LOGGER.info('Successfully deleted %s: "%s"', which['plural'], name)
+            success = verify(client, kind, name, repository=repository)
+    else:
+        LOGGER.debug('"%s" has a None value for name', kind)
+    return success
 
 
-def do_snap(client: Elasticsearch, repo: str, snap: str, idx: str, tier: str = 'cold') -> None:
+def do_snap(
+    client: 'Elasticsearch', repo: str, snap: str, idx: str, tier: str = 'cold'
+) -> None:
     """Perform a snapshot"""
     client.snapshot.create(repository=repo, snapshot=snap, indices=idx)
-    test = Snapshot(client, action='snapshot', snapshot=snap, repository=repo, pause=1, timeout=60)
+    test = Snapshot(
+        client, action='snapshot', snapshot=snap, repository=repo, pause=1, timeout=60
+    )
     test.wait_for_it()
 
     # Mount the index accordingly
     client.searchable_snapshots.mount(
         repository=repo,
         snapshot=snap,
         index=idx,
@@ -151,51 +199,54 @@
         storage=storage_type(tier),
         wait_for_completion=True,
     )
     # Fix aliases
     fix_aliases(client, idx, mounted_name(idx, tier))
 
 
-def exists(client: Elasticsearch, kind: str, name: str, repository: str = None) -> bool:
+def exists(
+    client: 'Elasticsearch', kind: str, name: str, repository: t.Union[str, None] = None
+) -> bool:
     """Return boolean existence of the named kind of object"""
     if name is None:
         return False
     retval = True
     func = emap(kind, client)['exists']
     try:
         if kind == 'snapshot':
             retval = func(snapshot=name, repository=repository)
         elif kind == 'ilm':
             retval = func(name=name)
         elif kind in ['index', 'data_stream']:
             retval = func(index=name)
         else:
             retval = func(name=name)
-    except esx.NotFoundError:
+    except NotFoundError:
         retval = False
     except Exception as err:
-        raise exc.ResultNotExpected(f'Unexpected result: {err}') from err
+        raise ResultNotExpected(f'Unexpected result: {err}') from err
     return retval
 
 
 def fill_index(
-    client: Elasticsearch,
+    client: 'Elasticsearch',
     name: t.Union[str, None] = None,
     count: t.Union[int, None] = None,
     start_num: t.Union[int, None] = None,
     match: bool = True,
 ) -> None:
     """
     Create and fill the named index with mappings and settings as directed
 
     :param client: ES client
     :param name: Index name
     :param count: The number of docs to create
     :param start_number: Where to start the incrementing number
-    :param match: Whether to use the default values for key (True) or random strings (False)
+    :param match: Whether to use the default values for key (True) or random strings
+        (False)
 
     :type client: es
     :type name: str
     :type count: int
     :type start_number: int
     :type match: bool
 
@@ -204,219 +255,252 @@
     """
     for doc in doc_gen(count=count, start_at=start_num, match=match):
         client.index(index=name, document=doc)
     client.indices.flush(index=name)
     client.indices.refresh(index=name)
 
 
-def find_write_index(client: Elasticsearch, name: str) -> t.AnyStr:
+def find_write_index(client: 'Elasticsearch', name: str) -> t.AnyStr:
     """Find the write_index for an alias by searching any index the alias points to"""
     retval = None
     for alias in get_aliases(client, name):
         retval = get_write_index(client, alias)
         if retval:
             break
     return retval
 
 
-def fix_aliases(client: Elasticsearch, oldidx: str, newidx: str) -> None:
+def fix_aliases(client: 'Elasticsearch', oldidx: str, newidx: str) -> None:
     """Fix aliases using the new and old index names as data"""
     # Delete the original index
     client.indices.delete(index=oldidx)
     # Add the original index name as an alias to the mounted index
     client.indices.put_alias(index=f'{newidx}', name=oldidx)
 
 
-def get(client: Elasticsearch, kind: str, pattern: str) -> t.Sequence[str]:
+def get(
+    client: 'Elasticsearch',
+    kind: str,
+    pattern: str,
+    repository: t.Union[str, None] = None,
+) -> t.Sequence[str]:
     """get any/all objects of type kind matching pattern"""
     if pattern is None:
         msg = f'"{kind}" has a None value for pattern'
         LOGGER.error(msg)
-        raise exc.TestbedMisconfig(msg)
+        raise TestbedMisconfig(msg)
     which = emap(kind, client, value=pattern)
     func = which['get']
     kwargs = which['kwargs']
+    if kind == 'snapshot':
+        kwargs['repository'] = repository
     try:
         result = func(**kwargs)
-    except Exception as err:
-        raise exc.ResultNotExpected(f'Unexpected result: {err}') from err
-    if kind in ['data_stream', 'template', 'component']:
+    except NotFoundError:
+        LOGGER.debug('%s pattern "%s" had zero matches', kind, pattern)
+        return []
+    except Exception as err:
+        raise ResultNotExpected(f'Unexpected result: {err}') from err
+    if kind == 'snapshot':
+        retval = [x['snapshot'] for x in result['snapshots']]
+    elif kind in ['data_stream', 'template', 'component']:
         retval = [x['name'] for x in result[which['key']]]
     else:
         # ['alias', 'ilm', 'index']
         retval = list(result.keys())
     return retval
 
 
-def get_aliases(client: Elasticsearch, name: str) -> t.Sequence[str]:
+def get_aliases(client: 'Elasticsearch', name: str) -> t.Sequence[str]:
     """Get aliases from index 'name'"""
     res = client.indices.get(index=name)
     try:
         retval = list(res[name]['aliases'].keys())
     except KeyError:
         retval = None
     return retval
 
 
-def get_backing_indices(client: Elasticsearch, name: str) -> t.Sequence[str]:
+def get_backing_indices(client: 'Elasticsearch', name: str) -> t.Sequence[str]:
     """Get the backing indices from the named data_stream"""
     resp = resolver(client, name)
     data_streams = resp['data_streams']
     retval = []
     if data_streams:
         if len(data_streams) > 1:
-            raise exc.ResultNotExpected(f'Expected only a single data_stream matching {name}')
+            raise ResultNotExpected(
+                f'Expected only a single data_stream matching {name}'
+            )
         retval = data_streams[0]['backing_indices']
     return retval
 
 
-def get_ds_current(client: Elasticsearch, name: str) -> str:
+def get_ds_current(client: 'Elasticsearch', name: str) -> str:
     """
     Find which index is the current 'write' index of the datastream
     This is best accomplished by grabbing the last backing_index
     """
     backers = get_backing_indices(client, name)
     retval = None
     if backers:
         retval = backers[-1]
     return retval
 
 
-def get_ilm(client: Elasticsearch, pattern: str) -> t.Union[t.Dict[str, str], None]:
+def get_ilm(client: 'Elasticsearch', pattern: str) -> t.Union[t.Dict[str, str], None]:
     """Get any ILM entity in ES that matches pattern"""
     try:
         return client.ilm.get_lifecycle(name=pattern)
     except Exception as err:
         msg = f'Unable to get ILM lifecycle matching {pattern}. Error: {err}'
         LOGGER.critical(msg)
-        raise exc.ResultNotExpected(msg) from err
+        raise ResultNotExpected(msg) from err
 
 
-def get_ilm_phases(client: Elasticsearch, name: str) -> t.Dict:
+def get_ilm_phases(client: 'Elasticsearch', name: str) -> t.Dict:
     """Return the policy/phases part of the ILM policy identified by 'name'"""
     ilm = get_ilm(client, name)
     try:
         return ilm[name]['policy']['phases']
     except KeyError as err:
         msg = f'Unable to get ILM lifecycle named {name}. Error: {err}'
         LOGGER.critical(msg)
-        raise exc.ResultNotExpected(msg) from err
+        raise ResultNotExpected(msg) from err
 
 
-def get_write_index(client: Elasticsearch, name: str) -> str:
+def get_write_index(client: 'Elasticsearch', name: str) -> str:
     """
     Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_alias`
 
     :param client: A client connection object
     :param name: An alias name
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type name: str
 
-    :returns: The the index name associated with the alias that is designated ``is_write_index``
-    :rtype: str
+    :returns: The the index name associated with the alias that is designated
+    ``is_write_index``
     """
     response = client.indices.get_alias(index=name)
     retval = None
     for index in list(response.keys()):
         try:
             if response[index]['aliases'][name]['is_write_index']:
                 retval = index
                 break
         except KeyError:
             continue
     return retval
 
 
-def snapshot_name(client: Elasticsearch, name: str) -> t.Union[t.AnyStr, None]:
+def snapshot_name(client: 'Elasticsearch', name: str) -> t.Union[t.AnyStr, None]:
     """Get the name of the snapshot behind the mounted index data"""
     res = {}
     if exists(client, 'index', name):  # Can jump straight to nested keys if it exists
         res = client.indices.get(index=name)[name]['settings']['index']
     try:
         retval = res['store']['snapshot']['snapshot_name']
     except KeyError:
         LOGGER.error('%s is not a searchable snapshot')
         retval = None
     return retval
 
 
-def ilm_explain(client: Elasticsearch, name: str) -> t.Union[t.Dict, None]:
+def ilm_explain(client: 'Elasticsearch', name: str) -> t.Union[t.Dict, None]:
     """Return the results from the ILM Explain API call for the named index"""
     try:
         retval = client.ilm.explain_lifecycle(index=name)['indices'][name]
     except KeyError:
         LOGGER.debug('Index name changed')
         new = list(client.ilm.explain_lifecycle(index=name)['indices'].keys())[0]
         retval = client.ilm.explain_lifecycle(index=new)['indices'][new]
-    except esx.NotFoundError as err:
+    except NotFoundError as err:
         LOGGER.warning('Datastream/Index Name changed. %s was not found', name)
-        raise exc.NameChanged(f'{name} was not found, likely due to a name change') from err
+        raise NameChanged(f'{name} was not found, likely due to a name change') from err
     except Exception as err:
         msg = f'Unable to get ILM information for index {name}'
         LOGGER.critical(msg)
-        raise exc.ResultNotExpected(f'{msg}. Exception: {err}') from err
+        raise ResultNotExpected(f'{msg}. Exception: {err}') from err
     return retval
 
 
-def ilm_move(client: Elasticsearch, name: str, current_step: t.Dict, next_step: t.Dict) -> None:
+def ilm_move(
+    client: 'Elasticsearch', name: str, current_step: t.Dict, next_step: t.Dict
+) -> None:
     """Move index 'name' from the current step to the next step"""
     try:
-        client.ilm.move_to_step(index=name, current_step=current_step, next_step=next_step)
+        client.ilm.move_to_step(
+            index=name, current_step=current_step, next_step=next_step
+        )
     except Exception as err:
         msg = f'Unable to move index {name} to ILM next step: {next}. Error: {err}'
         LOGGER.critical(msg)
-        raise exc.ResultNotExpected(msg)
+        raise ResultNotExpected(msg, err)
 
 
-def put_comp_tmpl(client: Elasticsearch, name: str, component: t.Dict) -> None:
+def put_comp_tmpl(client: 'Elasticsearch', name: str, component: t.Dict) -> None:
     """Publish a component template"""
     try:
-        client.cluster.put_component_template(name=name, template=component, create=True)
+        client.cluster.put_component_template(
+            name=name, template=component, create=True
+        )
         test = Exists(client, name=name, kind='component', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(f'Unable to create component template {name}. Error: {err}') from err
+        raise TestbedFailure(
+            f'Unable to create component template {name}. Error: {err}'
+        ) from err
 
 
 def put_idx_tmpl(
-    client, name: str, index_patterns: list, components: list, data_stream: t.Union[t.Dict, None] = None
+    client,
+    name: str,
+    index_patterns: list,
+    components: list,
+    data_stream: t.Union[t.Dict, None] = None,
 ) -> None:
     """Publish an index template"""
     try:
         client.indices.put_index_template(
             name=name,
             composed_of=components,
             data_stream=data_stream,
             index_patterns=index_patterns,
             create=True,
         )
         test = Exists(client, name=name, kind='template', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(f'Unable to create index template {name}. Error: {err}') from err
+        raise TestbedFailure(
+            f'Unable to create index template {name}. Error: {err}'
+        ) from err
 
 
-def put_ilm(client: Elasticsearch, name: str, policy: t.Union[t.Dict, None] = None) -> None:
+def put_ilm(
+    client: 'Elasticsearch', name: str, policy: t.Union[t.Dict, None] = None
+) -> None:
     """Publish an ILM Policy"""
     try:
         client.ilm.put_lifecycle(name=name, policy=policy)
     except Exception as err:
-        raise exc.TestbedFailure(f'Unable to put index lifecycle policy {name}. Error: {err}') from err
+        raise TestbedFailure(
+            f'Unable to put index lifecycle policy {name}. Error: {err}'
+        ) from err
 
 
-def resolver(client: Elasticsearch, name: str) -> dict:
+def resolver(client: 'Elasticsearch', name: str) -> dict:
     """
     Resolve details about the entity, be it an index, alias, or data_stream
 
-    Because you can pass search patterns and aliases as name, each element comes back as an array:
+    Because you can pass search patterns and aliases as name, each element comes back
+    as an array:
 
     {'indices': [], 'aliases': [], 'data_streams': []}
 
-    If you only resolve a single index or data stream, you will still have a 1-element list
+    If you only resolve a single index or data stream, you will still have a 1-element
+    list
     """
     return client.indices.resolve_index(name=name, expand_wildcards=['open', 'closed'])
 
 
-def rollover(client: Elasticsearch, name: str) -> None:
+def rollover(client: 'Elasticsearch', name: str) -> None:
     """Rollover alias or datastream identified by name"""
     client.indices.rollover(alias=name, wait_for_active_shards='all')
```

### Comparing `es_testbed-0.5.4/.gitignore` & `es_testbed-0.6.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 *$py.class
 
 # C extensions
 *.so
 
 
 .flake8
+pylintrc
+pylintrc.toml
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -141,14 +143,15 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+mypy.ini
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # pytype static type analyzer
```

### Comparing `es_testbed-0.5.4/LICENSE` & `es_testbed-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.4/README.md` & `es_testbed-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.4/pyproject.toml` & `es_testbed-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'datastream',
     'repository',
     'snapshot',
 ]
 dependencies = [
     'dotmap==1.3.30',
     'es_client==8.13.3',
-    'es-wait==0.3.3',
+    'es-wait==0.3.5',
 ]
 
 [project.optional-dependencies]
 test = [
     'mock',
     'requests',
     'pytest >=7.2.1',
@@ -103,16 +103,17 @@
 all = [
   'style',
   'typing',
 ]
 
 [tool.black]
 target-version = ['py38']
-line-length = 120
+line-length = 88
 skip-string-normalization = true
+include = '\.pyi?$'
 
 [tool.ruff]
 target-version = 'py38'
 line-length = 120
 select = [
   'A',
   'ARG',
```

### Comparing `es_testbed-0.5.4/PKG-INFO` & `es_testbed-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-testbed
-Version: 0.5.4
+Version: 0.6.0
 Summary: Library to help with building and tearing down indices, data streams, repositories and snapshots
 Project-URL: Documentation, https://github.com/untergeek/es-testbed#readme
 Project-URL: Issues, https://github.com/untergeek/es-testbed/issues
 Project-URL: Source, https://github.com/untergeek/es-testbed
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: dotmap==1.3.30
 Requires-Dist: es-client==8.13.3
-Requires-Dist: es-wait==0.3.3
+Requires-Dist: es-wait==0.3.5
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.2.1; extra == 'test'
```

