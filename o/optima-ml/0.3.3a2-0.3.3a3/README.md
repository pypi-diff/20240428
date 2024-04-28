# Comparing `tmp/optima_ml-0.3.3a2.tar.gz` & `tmp/optima_ml-0.3.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima_ml-0.3.3a2.tar", last modified: Sun Apr 28 13:24:27 2024, max compression
+gzip compressed data, was "optima_ml-0.3.3a3.tar", last modified: Sun Apr 28 13:25:01 2024, max compression
```

## Comparing `optima_ml-0.3.3a2.tar` & `optima_ml-0.3.3a3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.991722 optima_ml-0.3.3a2/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.3a2/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.983722 optima_ml-0.3.3a2/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.3a2/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.983722 optima_ml-0.3.3a2/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.3a2/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-04-27 00:05:49.000000 optima_ml-0.3.3a2/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.3a2/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.3a2/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-27 00:05:49.000000 optima_ml-0.3.3a2/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.983722 optima_ml-0.3.3a2/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    86145 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.3a2/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-04-28 12:14:59.000000 optima_ml-0.3.3a2/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    79732 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80230 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    17912 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-04-28 12:14:59.000000 optima_ml-0.3.3a2/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-04-28 12:14:59.000000 optima_ml-0.3.3a2/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-04-27 00:05:49.000000 optima_ml-0.3.3a2/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.3a2/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.3a2/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)    98138 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.3a2/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.3a2/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)   117575 2024-04-28 13:24:27.991722 optima_ml-0.3.3a2/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)   116177 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)   117575 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-28 13:24:27.000000 optima_ml-0.3.3a2/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-28 13:24:27.991722 optima_ml-0.3.3a2/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-04-27 00:05:49.000000 optima_ml-0.3.3a2/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:24:27.987722 optima_ml-0.3.3a2/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    34759 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    25341 2024-04-28 13:17:19.000000 optima_ml-0.3.3a2/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6471 2024-04-27 00:05:49.000000 optima_ml-0.3.3a2/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.3a2/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.3a2/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.3a3/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.3a3/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.3a3/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.3a3/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-04-17 06:54:34.000000 optima_ml-0.3.3a3/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    86860 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10090 2024-04-17 06:54:34.000000 optima_ml-0.3.3a3/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    81175 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80230 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    17991 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-04-28 12:14:59.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.3a3/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.3a3/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)   100879 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.3a3/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.3a3/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)   120177 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-04-28 13:25:01.000000 optima_ml-0.3.3a3/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-04-28 13:25:01.367689 optima_ml-0.3.3a3/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    34780 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    25631 2024-04-28 13:24:45.000000 optima_ml-0.3.3a3/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6471 2024-04-27 00:05:49.000000 optima_ml-0.3.3a3/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6399 2023-11-02 02:48:49.000000 optima_ml-0.3.3a3/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.3a3/tests/test_preprocessing.py
```

### Comparing `optima_ml-0.3.3a2/LICENSE` & `optima_ml-0.3.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/builtin/evaluation.py` & `optima_ml-0.3.3a3/OPTIMA/builtin/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/builtin/figures_of_merit.py` & `optima_ml-0.3.3a3/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/builtin/inputs.py` & `optima_ml-0.3.3a3/OPTIMA/builtin/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/builtin/search_space.py` & `optima_ml-0.3.3a3/OPTIMA/builtin/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/evaluation.py` & `optima_ml-0.3.3a3/OPTIMA/core/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,18 +319,22 @@
                     headers=[best_trials_fit.index.name] + list(best_trials_fit.columns),
                     tablefmt="fancy_grid",
                 )
 
         # go through results by iterating over the best trials for each target metric, print the corresponding configs,
         # copy best checkpoints to results folder and save output paths for later evaluation
         # first prepare the dataframe that will contain the best configs, meaning the hyperparameters of the best trials
-        # for each target metric, once determined using the best value and once using the fit
+        # for each target metric, once determined using the best value and once using the fit. Since the first
+        # checkpointing epoch and the checkpointing frequency are not relevant hyperparameters, skip those entries.
         optimize_name_list = optimize_name if isinstance(optimize_name, list) else [optimize_name]
+        hps_names = list(search_space.keys())
+        hps_names.remove("first_checkpoint_epoch")
+        hps_names.remove("checkpoint_frequency")
         model_configs_df = pd.DataFrame(
-            index=list(search_space.keys()) + ["epochs", "seed"],
+            index=hps_names + ["epochs", "seed"],
             columns=list(*zip(optimize_name_list, [f"{metric} fit" for metric in optimize_name_list]))
             if not skip_fit_evaluation
             else optimize_name_list,
         )
         model_configs_df.index.name = "Hyperparameter"
         optimization_results_string += "\n\nBest configs:\n"
 
@@ -361,17 +365,20 @@
                     model_config_to_evaluate[
                         "trial_id"
                     ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                     break
             model_configs_to_evaluate.append(model_config_to_evaluate)
 
             # Add the hyperparameters to the dataframe containing the configs of the best trials. For hierarchical
-            # search spaces, not all hyperparameters must have a value, so insert "-" for those
+            # search spaces, not all hyperparameters must have a value, so insert "-" for those. Since the checkpointing
+            # frequency and the first checkpoint epoch are not relevant hyperparameters, skip those entries.
             model_config = model_configs_to_evaluate[-1]
             for hp in model_configs_df.index:
+                if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
+                    continue
                 hp_value = model_config.get(hp)
                 model_configs_df.loc[hp, metric] = hp_value if hp_value is not None else "-"
 
             # create the target folder for the following crossvalidation
             target_folder = os.path.join(results_dir, metric if len(best_trials.index) > 1 else "", "best_value")
             dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
             if not os.path.exists(target_folder):
@@ -391,14 +398,16 @@
                         model_config_to_evaluate[
                             "trial_id"
                         ] = trial_id  # best_trail is full path to the optimization folder while trails in trial_list as only the names
                         break
                 model_configs_to_evaluate.append(model_config_to_evaluate)
                 model_config = model_configs_to_evaluate[-1]
                 for hp in model_configs_df.index:
+                    if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
+                        continue
                     hp_value = model_config.get(hp)
                     model_configs_df.loc[hp, f"{metric} fit"] = hp_value if hp_value is not None else "-"
                 target_folder = os.path.join(results_dir, metric if len(best_trials_fit.index) > 1 else "", "best_fit")
                 dirs_to_evaluate.append(target_folder)  # mark target_folder to be evaluated later
                 if not os.path.exists(target_folder):
                     os.makedirs(target_folder, exist_ok=True)
 
@@ -560,14 +569,16 @@
             optimization_str = f"training events: {[targets_train[targets_train[:, j] == 1].shape[0] for j in range(targets_train.shape[1])]}\n"
             optimization_str += f"validation events: {[targets_val[targets_val[:, j] == 1].shape[0] for j in range(targets_val.shape[1])]}\n"
             if run_config.use_testing_dataset:
                 optimization_str += f"test events: {[targets_test[targets_test[:, j] == 1].shape[0] for j in range(targets_test.shape[1])]}\n"
         optimization_str += "input variables: {}\n\n".format(", ".join(input_handler.get_vars()))
         optimization_str += "search space:\n"
         for hp in search_space.keys():
+            if hp in ["first_checkpoint_epoch", "checkpoint_frequency"]:
+                continue
             optimization_str += f"\t{hp}: {search_space[hp]}\n"
 
         # write results to file
         if write_results:
             with open(os.path.join(results_dir, "results.txt"), "w") as results_file:
                 results_file.write(
                     optimization_str
```

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/inputs.py` & `optima_ml-0.3.3a3/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/model.py` & `optima_ml-0.3.3a3/OPTIMA/core/model.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/search_space.py` & `optima_ml-0.3.3a3/OPTIMA/core/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/tools.py` & `optima_ml-0.3.3a3/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/training.py` & `optima_ml-0.3.3a3/OPTIMA/core/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         targets_train: Optional[Any] = None,
         weights_train: Optional[Any] = None,
         inputs_val: Optional[Any] = None,
         targets_val: Optional[Any] = None,
         weights_val: Optional[Any] = None,
         restore_best_weights: bool = False,
         create_checkpoints: bool = True,
+        first_checkpoint_epoch: int = 1,
+        checkpoint_frequency: int = 1,
         report_event: Optional[Event] = None,
         report_queue: Optional[Queue] = None,
         report_queue_read_event: Optional[Event] = None,
         termination_event: Optional[Event] = None,
         in_tune_session: bool = True,
         verbose: int = 0,
     ) -> None:
@@ -134,20 +136,26 @@
             Data structure containing the event weights of the validation dataset. (Default value = None)
         restore_best_weights : bool
             Whether to restore model weights from the epoch with the best value of the target metric. If ``False``, the
             model weights obtained at the last step of training are used. (Default value = False)
         create_checkpoints : bool
             Whether to save a checkpoint of the current and best model and the state of the early stopper at the end of
             each epoch. (Default value = True)
+        first_checkpoint_epoch : int
+            The first epoch after which a checkpoint should be saved. (Default value = 1)
+        checkpoint_frequency : int
+            Controls how often a checkpoint of the model weights and the early stopper state are saved. If the current
+            epoch number (when starting to count from 1) minus the ``first_checkpoint_epoch`` is divisible by
+            ``checkpoint_frequency``, a checkpoint is created. (Default value = 1)
         report_event : Optional[Event]
             `Multiprocessing` ``event`` triggered to tell the parent process the results dictionary has been added to the
             ``report_queue``. If not provided, report results directly to Tune. (Default value = None)
         report_queue : Optional[Queue]
-            `Multiprocessing` ``queue`` to send the results dictionary to the parent process. If not provided, report
-            results directly to Tune. (Default value = None)
+            `Multiprocessing` ``queue`` to send the current epoch number and the results dictionary to the parent
+            process. If not provided, report results directly to Tune. (Default value = None)
         report_queue_read_event : Optional[Event]
             `Multiprocessing` ``event`` triggered by the parent process when the results dictionary has been read from the
             ``report_queue`` and reported to `Tune`. If not provided, report results directly to Tune. (Default value = None)
         termination_event : Optional[Event]
             `Multiprocessing` ``event`` triggered by the parent process to signify that the training should be terminated. (Default value = None)
         in_tune_session : bool
             If not in a `Tune` session, no results need to be reported. (Default value = True)
@@ -183,18 +191,21 @@
         self.min_delta = min_delta
         self.patience_improvement = patience_improvement
         self.patience_overfitting = patience_overfitting
         self.overfitting_conditions = overfitting_conditions
 
         # various other settings
         self.create_checkpoints = create_checkpoints
+        self.first_checkpoint_epoch = first_checkpoint_epoch
+        self.checkpoint_frequency = checkpoint_frequency
         self.restore_best_weights = restore_best_weights
         self.verbose = verbose
 
         # status variables to keep track of the current status of the optimization
+        self.current_epoch = 0
         self.wait = 0
         self.wait_overfitting = 0
         self.best = np.Inf if self.monitor_op == np.less else -np.Inf
         self.best_metrics = (
             {}
         )  # will contain the values of the metrics for the best epoch (epoch with best monitor value)
         self.best_weighted_metrics = (
@@ -282,14 +293,18 @@
             The number of epochs since the start of the training.
         logs : Optional[dict]
             Dictionary containing the metrics reported during training and validation. (Default value = None)
         **kwargs : dict
             Additional keyword arguments that may be necessary for ML framework specific functionality, e.g. saving the
             model. They are provided to any call of a member function.
         """
+        # update the current epoch. The value given here as epoch is the epoch number of the just finished epoch. Since
+        # the "current" epoch is the next one, we need to add one.
+        self.current_epoch = epoch + 1
+
         # calculate all custom metrics on both training and validation data and add them to this epoch's logs
         if len(self.custom_metrics) > 0:
             logs = self.calc_custom_metrics(logs, **kwargs)
 
         # calculate the composite metrics
         if len(self.composite_metrics) > 0:
             logs = self.calc_composite_metrics(logs, **kwargs)
@@ -297,21 +312,25 @@
         # do the early stopping including updating the status variables. If the training should be terminated due to
         # early stopping, this internally calls self.stop_training()
         is_improvement = self._do_early_stopping(epoch, logs, **kwargs)
 
         # checkpoint the model and the early stopper status if checkpoints are requested. For this, a directory in the
         # current working dir (which is specific for this trial) is created and the current model, the best model and
         # the early stopper state is dumped there
-        if self.create_checkpoints:
+        if (
+            self.create_checkpoints
+            and epoch + 1 >= self.first_checkpoint_epoch
+            and (epoch + 1 - self.first_checkpoint_epoch) % self.checkpoint_frequency == 0
+        ):
             # save current model
             os.makedirs("checkpoint_dir", exist_ok=True)
             self.save_model(output_dir="checkpoint_dir", model_name="model", **kwargs)
 
             # save model again as best model if there was an improvement; TODO: replace this with a copy?
-            if is_improvement or epoch == 0:
+            if is_improvement or epoch + 1 == self.first_checkpoint_epoch:
                 self.save_model(output_dir="checkpoint_dir", model_name="best_model", **kwargs)
 
             # save early stopper state
             self.save_state(path=os.path.join("checkpoint_dir", "early_stopper"), **kwargs)
 
         # report to Tune if we are in a Tune session
         if self.in_tune_session:
@@ -329,27 +348,31 @@
                 current_composite,
                 **kwargs,
             )
 
             # report the results back to tune by activating the report event and putting the results into the queue
             if self.report_directly:
                 time_before_report = time.time()
-                if self.create_checkpoints:
+                if (
+                    self.create_checkpoints
+                    and epoch + 1 >= self.first_checkpoint_epoch
+                    and (epoch + 1 - self.first_checkpoint_epoch) % self.checkpoint_frequency == 0
+                ):
                     checkpoint = train.Checkpoint.from_directory("checkpoint_dir")
                     train.report(results, checkpoint=checkpoint)
                 else:
                     train.report(results)
                 if time.time() - time_before_report > 2:
                     logging.warning(
                         "Reporting results took {} seconds, which may be a performance bottleneck.".format(
                             time.time() - time_before_report
                         )
                     )
             else:
-                self.report_queue.put(results)
+                self.report_queue.put((epoch, results))
                 self.report_event.set()
 
                 # wait until the report_queue_read_event is set. When tune terminates the trial, this process should also
                 # be terminated externally, so we usually don't have to take care of that here. However sometimes this
                 # termination fails, which we unfortunately can only detect once the parent process is terminated, which
                 # would be too late. We still check, if the main process is still alive (in case it is killed or an error
                 # occurs), but limit the time or waiting to a total 600 seconds before this subprocess self-terminates
@@ -725,15 +748,15 @@
             model. They are provided to any call of a member function.
         """
         if self.wait >= self.patience_improvement and self.verbose > 0:
             print("Epoch {}: Early stopping...".format(self.stopped_epoch + 1))
         elif self.wait_overfitting >= self.patience_overfitting and self.verbose > 0:
             print("Epoch {}: Early stopping due to overfitting...".format(self.stopped_epoch + 1))
 
-    state_type = tuple[int, int, Union[float, int], dict, dict, dict, dict, Any, int, int, bool, Union[float, int]]
+    state_type = tuple[int, int, int, Union[float, int], dict, dict, dict, dict, Any, int, int, bool, Union[float, int]]
 
     def _get_state(self, **kwargs: dict) -> state_type:
         """Returns the values of all attributes needed to restore the state of the early stopper.
 
         This includes the number of epochs since the last improvement (``self.wait``), the number of epochs since the last
         time no `overfitting condition` was violated (``self.wait_overfitting``), the best target metric value seen
         (``self.best``), the dictionaries containing the values of the `native`, `weighted native`, `custom` and
@@ -751,14 +774,15 @@
 
         Returns
         -------
         state_type
             The tuple containing all state variables.
         """
         return (
+            self.current_epoch,
             self.wait,
             self.wait_overfitting,
             self.best,
             self.best_metrics,
             self.best_weighted_metrics,
             self.best_custom_metrics,
             self.best_composite_metrics,
@@ -777,14 +801,15 @@
         state : state_type
             Early stopper state to restore from.
         **kwargs : dict
             Additional keyword arguments that may be necessary for ML framework specific functionality, e.g. saving the
             model. They are provided to any call of a member function.
         """
         (
+            self.current_epoch,
             self.wait,
             self.wait_overfitting,
             self.best,
             self.best_metrics,
             self.best_weighted_metrics,
             self.best_custom_metrics,
             self.best_composite_metrics,
```

### Comparing `optima_ml-0.3.3a2/OPTIMA/core/variable_optimization.py` & `optima_ml-0.3.3a3/OPTIMA/core/variable_optimization.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/defaults.py` & `optima_ml-0.3.3a3/OPTIMA/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
 # general settings for the optimization
 model_type = 'Keras'  # the library used to build the model, possible values: 'Keras' and 'Lightning'
 monitor_name = 'val_loss'  # metric that is used for the optimization, early stopping and the evaluation
 monitor_op = 'min'  # operator corresponding to the metric to monitor
 optimize_on_best_value = False  # should the highest value of the metric to monitor be used as target for the optimization (that may be an outlier) or the current value (that may have gotten worse due to overtraining)?
 restore_on_best_checkpoint = False  # if True, any reloads will use the best model so far (based on metic value) instead of the last one
+checkpoint_frequency = 1  # how many epochs to wait between saving checkpoints
 max_epochs = 200  # maximum number of epoch before terminating the training; this can be something very large because the Early Stopping and ASHA will take care of the termination
 early_stopping_patience = 6  # number of consecutive epochs without improvement (of the metric to monitor) before terminating the training
 overtraining_patience = 6  # number of consecutive epochs with overtraining detected (at least one overtraining condition is fulfilled) before terminating the training; only used when OT conditions are defined
 random_seed = 42  # random seed to make optimization deterministic (within the limits of parallelization); set to None to disable
 
 # settings for the evaluation and crossvalidation
 fit_min_R_squared = 0.9  # min. R-squared of the fit; if less, the fit is rejected (and consequently the trial is ignored for the evaluation)
```

### Comparing `optima_ml-0.3.3a2/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima_ml-0.3.3a3/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/hardware_configs/common.py` & `optima_ml-0.3.3a3/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima_ml-0.3.3a3/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/helpers/manage_ray_nodes.py` & `optima_ml-0.3.3a3/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/keras/model.py` & `optima_ml-0.3.3a3/OPTIMA/keras/model.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/keras/tools.py` & `optima_ml-0.3.3a3/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/keras/training.py` & `optima_ml-0.3.3a3/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/lightning/inputs.py` & `optima_ml-0.3.3a3/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/lightning/training.py` & `optima_ml-0.3.3a3/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/optima.py` & `optima_ml-0.3.3a3/OPTIMA/optima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.3alpha2"
+__version__ = "0.3.3alpha3"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
@@ -186,14 +186,16 @@
                 targets_train=targets_train,
                 targets_val=targets_val,
                 weights_train=normalized_weights_train,
                 weights_val=normalized_weights_val,
                 restore_best_weights=restore_best_weights,
                 verbose=verbose,
                 create_checkpoints=create_checkpoints,
+                first_checkpoint_epoch=model_config["first_checkpoint_epoch"],
+                checkpoint_frequency=model_config["checkpoint_frequency"],
                 report_event=report_event,
                 report_queue=report_queue,
                 report_queue_read_event=report_queue_read_event,
                 termination_event=termination_event,
                 in_tune_session=in_tune_session
             )
         elif run_config.model_type == "Lightning":
@@ -213,14 +215,16 @@
                 targets_train=targets_train,
                 targets_val=targets_val,
                 weights_train=normalized_weights_train,
                 weights_val=normalized_weights_val,
                 restore_best_weights=restore_best_weights,
                 verbose=verbose,
                 create_checkpoints=create_checkpoints,
+                first_checkpoint_epoch=model_config["first_checkpoint_epoch"],
+                checkpoint_frequency=model_config["checkpoint_frequency"],
                 report_event=report_event,
                 report_queue=report_queue,
                 report_queue_read_event=report_queue_read_event,
                 termination_event=termination_event,
                 in_tune_session=in_tune_session
             )
 
@@ -335,14 +339,15 @@
             logging.warning(f"Starting the subprocess and prepare training took {time.time()-start_time}s which may be a performance bottleneck.")
 
         if run_config.model_type == "Keras":
             model.fit(
                 train_data,
                 validation_data=val_data,
                 epochs=model_config["max_epochs"],
+                initial_epoch=early_stopper.current_epoch,  # when continuing the training, set the correct epoch number
                 callbacks=[early_stopper, *[c[0](**c[1]) for c in run_config.callbacks]],
                 verbose=verbose
             )
         elif run_config.model_type == "Lightning":
             # set correct number of cpu cores; TODO: this for some reason currently only works with pytorch-gpu and is ignored by pytorch??
             from torch import get_num_threads, get_num_interop_threads, set_num_threads, set_num_interop_threads
             if get_num_threads() != num_threads:
@@ -358,14 +363,15 @@
                 accelerator='auto',
                 num_sanity_val_steps=0,  # this messes with the reporting to Tune since it calls the Callbacks
                 enable_progress_bar=False,
                 enable_model_summary=False,
                 logger=False,  # logging is done via Tune
                 enable_checkpointing=False,  # checkpointing is done in the early stopper
             )
+            trainer.fit_loop.epoch_progress.current.processed = early_stopper.current_epoch  # when continuing the training, set the correct epoch number
             trainer.fit(model, pl_data_module)
 
         # if requested, save the final model
         if "final_model_path" in model_config.keys():
             if not os.path.exists(os.path.dirname(model_config["final_model_path"])):
                 os.makedirs(os.path.dirname(model_config["final_model_path"]), exist_ok=True)
             if run_config.model_type == "Keras":
@@ -487,19 +493,21 @@
     if run_in_subprocess:
         while (not termination_event.is_set()) and p.is_alive():
             if in_tune_session:
                 if checkpoint_event.is_set():
                     checkpoint_queue.put(train.get_checkpoint())
                     checkpoint_event.clear()
                 if report_event.is_set():
-                    results = report_queue.get()
-                    if create_checkpoints:
+                    epoch, results = report_queue.get()
+                    if (create_checkpoints and epoch + 1 >= model_config["first_checkpoint_epoch"] and
+                            (epoch + 1 - model_config["first_checkpoint_epoch"]) % model_config["checkpoint_frequency"] == 0):
                         checkpoint = train.Checkpoint.from_directory("checkpoint_dir")
                     time_before_report = time.time()
-                    if create_checkpoints:
+                    if (create_checkpoints and epoch + 1 >= model_config["first_checkpoint_epoch"] and
+                            (epoch + 1 - model_config["first_checkpoint_epoch"]) % model_config["checkpoint_frequency"] == 0):
                         train.report(results, checkpoint=checkpoint)
                     else:
                         train.report(results)
                     report_event.clear()
                     report_queue_read_event.set()
                     if time.time() - time_before_report > 2:
                         logging.warning(
@@ -575,16 +583,20 @@
             if isinstance(run_config.search_space[hp], dict) and "supports_mutation" not in run_config.search_space[hp].keys():
                 run_config.search_space[hp]["supports_mutation"] = True
     if run_config.model_type == 'Keras' and not hasattr(run_config, 'compile_model'):
         for hp in mutatable_hps_compile:
             if isinstance(run_config.search_space[hp], dict) and "supports_mutation" not in run_config.search_space[hp].keys():
                 run_config.search_space[hp]["supports_mutation"] = True
 
-    # add the maximum number of epochs to the search space
+    # add the maximum number of epochs and the first epoch to checkpoint and the checkpoint frequency to the search space.
+    # Here, we want to start checkpointing after checkpoint_frequency epochs, so set first_checkpoint_epoch to
+    # checkpoint_frequency
     run_config.search_space["max_epochs"] = run_config.max_epochs
+    run_config.search_space["first_checkpoint_epoch"] = run_config.checkpoint_frequency
+    run_config.search_space["checkpoint_frequency"] = run_config.checkpoint_frequency
 
     # build the search space for optuna
     search_space_optuna = functools.partial(
         OPTIMA.core.search_space.optuna_search_space,
         OPTIMA.core.search_space.serialize_conditions(run_config.search_space)
     )
 
@@ -1039,14 +1051,30 @@
             }
         else:
             best_hp_values_optuna = None
 
         # prepare the search space for PBT and get the mutatable subset of the search space
         search_space_PBT, hyperparams_to_mutate = OPTIMA.core.search_space.prepare_search_space_for_PBT(run_config.search_space, best_hp_values_optuna)
 
+        # for PBT, we need a checkpoint on the last epoch of each perturbation interval. If the burn-in period and the
+        # perturbation interval are both divisible by the checkpointing frequency, this works out. If the burn-in period
+        # is not divisible by the checkpointing frequency, set the first checkpoint to be at the end of the burn-in
+        # period. If the perturbation interval is not divisible by the checkpointing frequency, set the checkpointing
+        # frequency to the perturbation interval.
+        if run_config.burn_in_period % run_config.checkpoint_frequency != 0:
+            print(f"The PBT burn-in period of {run_config.burn_in_period} epochs is not divisible by the checkpointing "
+                  f"frequency of {run_config.checkpoint_frequency} epochs. Creating the first checkpoint after "
+                  f"{run_config.burn_in_period} epochs.")
+            search_space_PBT["first_checkpoint_epoch"] = run_config.burn_in_period
+        if run_config.perturbation_interval % run_config.checkpoint_frequency != 0:
+            print(f"The PBT perturbation interval of {run_config.perturbation_interval} epochs is not divisible by the "
+                  f"checkpointing frequency of {run_config.checkpoint_frequency} epochs. Setting the checkpointing "
+                  f"frequency to {run_config.perturbation_interval} epochs.")
+            search_space_PBT["checkpoint_frequency"] = run_config.perturbation_interval
+
         # print the updated search space
         print("Updated search space:")
         print(search_space_PBT)
 
         # since the search algorithm is completely ignored when using PBT, we cannot do the same trick to include the
         # random seed as for Optuna. Fortunately, PBT only optimizes hyperparameters provided in hyperparams_to_mutate,
         # so we can simply add a new search space entry for the seed. Unfortunately, the only way to make the sampling
@@ -1079,15 +1107,15 @@
                 ),
                 param_space=search_space_PBT if not replay else None,
                 run_config=train.RunConfig(
                     name=name,
                     storage_path=os.path.abspath(storage_path),  # with Ray 2.7 this needs to be absolute, otherwise Ray complains about write permissions?
                     stop=stopper,
                     checkpoint_config=train.CheckpointConfig(
-                        num_to_keep=2*max(run_config.perturbation_interval, run_config.burn_in_period)+2,
+                        num_to_keep=None,
                         # checkpoint_score_attribute=optimize_name,
                         # checkpoint_score_order=optimize_op
                     ),
                     failure_config=train.FailureConfig(
                         max_failures=-1,
                     ),
                     # callbacks=[JsonLoggerCallback(), CSVLoggerCallback()],
```

### Comparing `optima_ml-0.3.3a2/OPTIMA/resources/config_verification.py` & `optima_ml-0.3.3a3/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/OPTIMA/resources/pbt_with_seed.py` & `optima_ml-0.3.3a3/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/PKG-INFO` & `optima_ml-0.3.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.3a2
+Version: 0.3.3a3
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -393,20 +393,21 @@
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
-| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+|-----------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `checkpoint_frequency` *(int)*    | `1`           | The number of epochs to wait between consecutive checkpoints for each model. Since this is only useful to restore the training progress if the optimization is interrupted, this should be set so that, on average, a checkpoint is created every few minutes. For the initial and main hyperparameter optimization, the first checkpoint for each trial is created after `checkpoint_frequency` epochs. Since for Population Based Training, a checkpoint must be created after the last epoch in each perturbation interval, the `checkpoint_frequency` is overwritten with the `perturbation_interval`, unless it is divisible by the `checkpointing_frequency`. The first checkpoint will be created after `checkpointing_frequency` epochs if the `burn_in_period` is divisible by the `checkpointing_frequency`, and after `burn_in_period` epochs otherwise. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima_ml-0.3.3a2/README.md` & `optima_ml-0.3.3a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -354,20 +354,21 @@
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
-| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+|-----------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `checkpoint_frequency` *(int)*    | `1`           | The number of epochs to wait between consecutive checkpoints for each model. Since this is only useful to restore the training progress if the optimization is interrupted, this should be set so that, on average, a checkpoint is created every few minutes. For the initial and main hyperparameter optimization, the first checkpoint for each trial is created after `checkpoint_frequency` epochs. Since for Population Based Training, a checkpoint must be created after the last epoch in each perturbation interval, the `checkpoint_frequency` is overwritten with the `perturbation_interval`, unless it is divisible by the `checkpointing_frequency`. The first checkpoint will be created after `checkpointing_frequency` epochs if the `burn_in_period` is divisible by the `checkpointing_frequency`, and after `burn_in_period` epochs otherwise. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima_ml-0.3.3a2/optima_ml.egg-info/PKG-INFO` & `optima_ml-0.3.3a3/optima_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.3a2
+Version: 0.3.3a3
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
@@ -393,20 +393,21 @@
 | `weighted_native_metrics` *(list)* | `[]`          | A list of references to a metric class native to the used ML backend. Each entry must be a tuple of the form `("name", (ClassReference, {"kwarg1": kwarg1, ...}))`. Their values are calculated separately on the training and validation datasets and reported as `"train_name" and "val_name". Event weights are applied. Currently, weighted metrics are not supported for Lightning (see https://github.com/Lightning-AI/torchmetrics/issues/784).                                                                                                                                                                                                                                                                     |
 | `custom_metrics` *(list)*          | `[]`          | A list of custom metrics. Each entry must be a tuple of the form `("name", callable)`. `callable` needs to accept target values, model prediction and sample weights and return a number or a boolean. Their values are calculated at the end of each epoch separately on the training and validation datasets and reported as `"train_name" and "val_name".                                                                                                                                                                                                                                                                                                                                                               |
 | `composite_metrics` *(list)*       | `[]`          | A list of composite metrics. These are metrics that combine the values of already existing metrics. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a number or a boolean. They are calculated at the end of each epoch and allow all native, weighted native and custom metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. It is possible to mix training and validation metrics, allowing e.g. to assess the generalization gap. The value of composite metrics is reported as "name" without a prefix. |
 | `overtraining_conditions` *(list)* | `[]`          | A list of overtraining conditions. These are special composite metrics that should return `True` when overtraining is detected and `False` otherwise. Each entry must be a tuple of the form `("name", (metric_name1, metric_name2, ...), callable)` where `callable` accepts the same number of positional arguments as the number of provided metric names and returns a boolean. They are calculated at the end of each epoch and allow all native, weighted native, custom and composite metrics as well as metrics directly reported by the ML backend (e.g. validation loss) as inputs. Naturally, it is possible to mix training and validation metrics. The value of overtraining conditions is not reported.      |
 
 #### Training
 
-| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                   |
-|-----------------------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                             |
-| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                      |
-| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                           |
-| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training. |
+| Parameter                         | Default value | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+|-----------------------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `max_epochs` *(int)*              | `200`         | The maximal number of epochs until the training is terminated. Early stopping may terminate the training earlier.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| `early_stopping_patience` *(int)* | `6`           | The maximal number of consecutive epochs without an improvement of the target metric before early-stopping the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| `overtraining_patience` *(int)*   | `6`           | The maximal number of consecutive epochs with overtraining detected (i.e. at least one overtraining condition detected overtraining) before early-stopping the training. This is ignored if no overtraining conditions are defined.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| `callbacks` *(list)*              | `[]`          | A list of references to a callback class native to the used ML backend (i.e. a subclass of `keras.callbacks.Callback` for Keras or `lightning.pytorch.callbacks.Callback` for Lightning. Each entry must be a tuple of the form `(ClassReference, {"kwarg1": kwarg1, ...})`. The callbacks are only used during the training.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| `checkpoint_frequency` *(int)*    | `1`           | The number of epochs to wait between consecutive checkpoints for each model. Since this is only useful to restore the training progress if the optimization is interrupted, this should be set so that, on average, a checkpoint is created every few minutes. For the initial and main hyperparameter optimization, the first checkpoint for each trial is created after `checkpoint_frequency` epochs. Since for Population Based Training, a checkpoint must be created after the last epoch in each perturbation interval, the `checkpoint_frequency` is overwritten with the `perturbation_interval`, unless it is divisible by the `checkpointing_frequency`. The first checkpoint will be created after `checkpointing_frequency` epochs if the `burn_in_period` is divisible by the `checkpointing_frequency`, and after `burn_in_period` epochs otherwise. |
 
 #### Hyperparameter optimization
 
 ##### General
 
 | Parameter                             | Default value                                                                                                                 | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `optima_ml-0.3.3a2/optima_ml.egg-info/SOURCES.txt` & `optima_ml-0.3.3a3/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/setup.py` & `optima_ml-0.3.3a3/setup.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/tests/test_builtin.py` & `optima_ml-0.3.3a3/tests/test_builtin.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,15 @@
     expected_metrics = {"train_difference_loss", "val_difference_loss", "best_train_difference_loss",
                         "best_val_difference_loss", "last_valid_val_difference_loss", "train_plus_val_loss",
                         "best_train_plus_val_loss", "early_stopped"}
     while True:
         report_event.wait(timeout=1)
         if report_event.is_set():
             report_event.clear()
-            report = report_queue.get()
+            epoch, report = report_queue.get()
             print(f"Early stopper reported (epoch {i+1}): {report}")
             assert set(report.keys()) == expected_metrics
             report_queue_read_event.set()
             i += 1
         elif termination_event.is_set():
             termination_event.clear()
             break
@@ -786,15 +786,15 @@
     expected_metrics = {"train_difference_loss", "val_difference_loss", "best_train_difference_loss",
                         "best_val_difference_loss", "last_valid_val_difference_loss", "train_plus_val_loss",
                         "best_train_plus_val_loss", "early_stopped"}
     while True:
         report_event.wait(timeout=1)
         if report_event.is_set():
             report_event.clear()
-            report = report_queue.get()
+            epoch, report = report_queue.get()
             print(f"Early stopper reported (epoch {i + 1}): {report}")
             assert set(report.keys()) == expected_metrics
             report_queue_read_event.set()
             i += 1
         elif termination_event.is_set():
             termination_event.clear()
             break
@@ -843,15 +843,15 @@
     expected_metrics = {"train_difference_loss", "val_difference_loss", "best_train_difference_loss",
                         "best_val_difference_loss", "last_valid_val_difference_loss", "train_plus_val_loss",
                         "best_train_plus_val_loss", "early_stopped"}
     while True:
         report_event.wait(timeout=1)
         if report_event.is_set():
             report_event.clear()
-            report = report_queue.get()
+            epoch, report = report_queue.get()
             print(f"Early stopper reported (epoch {i + 1}): {report}")
             assert set(report.keys()) == expected_metrics
             report_queue_read_event.set()
             i += 1
         elif termination_event.is_set():
             termination_event.clear()
             break
```

### Comparing `optima_ml-0.3.3a2/tests/test_core.py` & `optima_ml-0.3.3a3/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,14 +402,19 @@
 
     # get metrics
     custom_metrics = run_config.custom_metrics
     composite_metrics = run_config.composite_metrics
     native_metrics = run_config.native_metrics
     weighted_native_metrics = run_config.weighted_native_metrics
 
+    # get the search space and add a few entries
+    run_config.search_space["max_epochs"] = run_config.max_epochs
+    run_config.search_space["first_checkpoint_epoch"] = run_config.checkpoint_frequency
+    run_config.search_space["checkpoint_frequency"] = run_config.checkpoint_frequency
+
     # evaluation; get the raw metric values to compare
     best_trials_test, best_trials_fit_test, configs_df_test, _, raw_metric_values_test = \
         evaluation.evaluate_experiment(analysis,
                                        optima.train_model,
                                        run_config,
                                        run_config.monitor_name,
                                        run_config.monitor_op,
```

### Comparing `optima_ml-0.3.3a2/tests/test_integration.py` & `optima_ml-0.3.3a3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/tests/test_integration_sameMachine.py` & `optima_ml-0.3.3a3/tests/test_integration_sameMachine.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.3a2/tests/test_preprocessing.py` & `optima_ml-0.3.3a3/tests/test_preprocessing.py`

 * *Files identical despite different names*

