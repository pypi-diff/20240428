# Comparing `tmp/mpl_ascii-0.1.0.tar.gz` & `tmp/mpl_ascii-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.1.0.tar", last modified: Thu Apr 25 19:32:49 2024, max compression
+gzip compressed data, was "mpl_ascii-0.2.0.tar", last modified: Sun Apr 28 12:46:46 2024, max compression
```

## Comparing `mpl_ascii-0.1.0.tar` & `mpl_ascii-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,49 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.104809 mpl_ascii-0.1.0/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.084809 mpl_ascii-0.1.0/.github/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.084809 mpl_ascii-0.1.0/.github/workflows/
--rw-rw-r--   0 chris     (1000) chris     (1000)      992 2024-04-25 17:23:19.000000 mpl_ascii-0.1.0/.github/workflows/python-package.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)     3107 2024-04-25 16:48:20.000000 mpl_ascii-0.1.0/.gitignore
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.1.0/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     1504 2024-04-25 17:19:45.000000 mpl_ascii-0.1.0/Makefile
--rw-r--r--   0 chris     (1000) chris     (1000)      877 2024-04-25 19:32:49.104809 mpl_ascii-0.1.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      593 2024-04-25 19:09:36.000000 mpl_ascii-0.1.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.092809 mpl_ascii-0.1.0/examples/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_chart.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      761 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      903 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_label_1.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1011 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_label_2.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1084 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_label_3.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      675 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_label_4.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      669 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_label_5.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/bar_stacked.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/barh.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1135 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/broken_barh.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      736 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/categorical_variables.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/cohere.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      998 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/cohere_single_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1286 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/csd_demo.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      679 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/double_plot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1124 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/hist_best_fit_line.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1019 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/hist_simple.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1665 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/hist_simple_colors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1188 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/lines_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1151 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/scatter_multi_color.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      627 2024-04-25 16:44:32.000000 mpl_ascii-0.1.0/examples/simple_plot.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.092809 mpl_ascii-0.1.0/mpl_ascii/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8914 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      856 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/ascii_canvas.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1629 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/color_map.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3987 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/draw.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1340 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/overlay.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.1.0/mpl_ascii/tools.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.100809 mpl_ascii-0.1.0/mpl_ascii.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)      877 2024-04-25 19:32:49.000000 mpl_ascii-0.1.0/mpl_ascii.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1604 2024-04-25 19:32:49.000000 mpl_ascii-0.1.0/mpl_ascii.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-04-25 19:32:49.000000 mpl_ascii-0.1.0/mpl_ascii.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       18 2024-04-25 19:32:49.000000 mpl_ascii-0.1.0/mpl_ascii.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-04-25 19:32:49.000000 mpl_ascii-0.1.0/mpl_ascii.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      401 2024-04-25 19:14:11.000000 mpl_ascii-0.1.0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      144 2024-04-25 18:43:05.000000 mpl_ascii-0.1.0/requirements.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-25 19:32:49.104809 mpl_ascii-0.1.0/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.092809 mpl_ascii-0.1.0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-04-25 16:45:15.000000 mpl_ascii-0.1.0/tests/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-25 19:32:49.100809 mpl_ascii-0.1.0/tests/accept/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8585 2024-04-25 17:19:59.000000 mpl_ascii-0.1.0/tests/accept/bar_chart.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     8585 2024-04-25 17:19:59.000000 mpl_ascii-0.1.0/tests/accept/bar_color.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     8426 2024-04-25 17:20:01.000000 mpl_ascii-0.1.0/tests/accept/bar_label_1.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:01.000000 mpl_ascii-0.1.0/tests/accept/bar_label_2.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:02.000000 mpl_ascii-0.1.0/tests/accept/bar_label_3.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7359 2024-04-25 17:20:02.000000 mpl_ascii-0.1.0/tests/accept/bar_label_4.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7267 2024-04-25 17:20:03.000000 mpl_ascii-0.1.0/tests/accept/bar_label_5.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     8426 2024-04-25 17:20:04.000000 mpl_ascii-0.1.0/tests/accept/bar_stacked.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:00.000000 mpl_ascii-0.1.0/tests/accept/barh.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7359 2024-04-25 17:20:04.000000 mpl_ascii-0.1.0/tests/accept/broken_barh.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)    21803 2024-04-25 17:20:05.000000 mpl_ascii-0.1.0/tests/accept/categorical_variables.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)    14723 2024-04-25 17:20:06.000000 mpl_ascii-0.1.0/tests/accept/cohere.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7271 2024-04-25 17:20:07.000000 mpl_ascii-0.1.0/tests/accept/cohere_single_plot.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)    14823 2024-04-25 17:20:08.000000 mpl_ascii-0.1.0/tests/accept/csd_demo.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:08.000000 mpl_ascii-0.1.0/tests/accept/double_plot.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:09.000000 mpl_ascii-0.1.0/tests/accept/hist_best_fit_line.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)    14815 2024-04-25 17:20:11.000000 mpl_ascii-0.1.0/tests/accept/hist_simple.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)    14815 2024-04-25 17:20:10.000000 mpl_ascii-0.1.0/tests/accept/hist_simple_colors.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     8868 2024-04-25 17:20:12.000000 mpl_ascii-0.1.0/tests/accept/lines_multi_color.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     8799 2024-04-25 17:20:12.000000 mpl_ascii-0.1.0/tests/accept/scatter_multi_color.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     7405 2024-04-25 17:20:13.000000 mpl_ascii-0.1.0/tests/accept/simple_plot.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-25 16:45:15.000000 mpl_ascii-0.1.0/tests/test_overlay.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.492310 mpl_ascii-0.2.0/.github/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.496310 mpl_ascii-0.2.0/.github/workflows/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      992 2024-04-25 17:23:19.000000 mpl_ascii-0.2.0/.github/workflows/python-package.yml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3107 2024-04-25 16:48:20.000000 mpl_ascii-0.2.0/.gitignore
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-04-25 16:42:37.000000 mpl_ascii-0.2.0/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1472 2024-04-27 12:42:39.000000 mpl_ascii-0.2.0/Makefile
+-rw-r--r--   0 chris     (1000) chris     (1000)    20434 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)    20125 2024-04-28 08:08:12.000000 mpl_ascii-0.2.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.500310 mpl_ascii-0.2.0/examples/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1306 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_chart.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      827 2024-04-28 08:03:54.000000 mpl_ascii-0.2.0/examples/bar_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      903 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_1.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1011 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_2.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1084 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_3.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      675 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_4.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      669 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_label_5.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1012 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/bar_stacked.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1036 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/barh.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      736 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/categorical_variables.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1069 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/cohere.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      998 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/cohere_single_plot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1286 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/csd_demo.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      747 2024-04-28 08:04:51.000000 mpl_ascii-0.2.0/examples/double_plot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1124 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_best_fit_line.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1019 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_simple.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1665 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/hist_simple_colors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1188 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/lines_multi_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1218 2024-04-28 08:05:08.000000 mpl_ascii-0.2.0/examples/scatter_multi_color.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      627 2024-04-25 16:44:32.000000 mpl_ascii-0.2.0/examples/simple_plot.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.500310 mpl_ascii-0.2.0/mpl_ascii/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8963 2024-04-28 12:43:13.000000 mpl_ascii-0.2.0/mpl_ascii/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      856 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/ascii_canvas.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1629 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/color_map.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3987 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/draw.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1340 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/overlay.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      274 2024-04-25 16:43:43.000000 mpl_ascii-0.2.0/mpl_ascii/tools.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/mpl_ascii.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)    20434 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      945 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       18 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-04-28 12:46:46.000000 mpl_ascii-0.2.0/mpl_ascii.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      429 2024-04-28 12:44:22.000000 mpl_ascii-0.2.0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      144 2024-04-25 18:43:05.000000 mpl_ascii-0.2.0/requirements.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-04-28 12:46:46.504310 mpl_ascii-0.2.0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-04-25 16:45:15.000000 mpl_ascii-0.2.0/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4510 2024-04-25 16:45:15.000000 mpl_ascii-0.2.0/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.1.0/.github/workflows/python-package.yml` & `mpl_ascii-0.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/.gitignore` & `mpl_ascii-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/LICENSE` & `mpl_ascii-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/Makefile` & `mpl_ascii-0.2.0/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 DATA_DIR=data
 LOCATION:=$(DATA_DIR)/plots
 TEST_LOCATION:=$(DATA_DIR)/tests
-TEST_DIR:=tests
 
-ACCEPTANCE_DIR=$(TEST_DIR)/accept
+ACCEPTANCE_DIR=examples
 
 MPL_ASCII_FILES=$(wildcard mpl_ascii/*.py)
 EXAMPLES_PY_FILES=$(wildcard examples/*.py)
 EXAMPLES_FILE_NAMES_WO_EXT=$(basename $(notdir $(EXAMPLES_PY_FILES)))
 
 ALL_PLOTS_NAMES=$(basename $(notdir $(EXAMPLES_PY_FILES)))
 
@@ -41,18 +40,18 @@
 accept: $(addprefix $(ACCEPTANCE_DIR)/,$(ALL_PLOTS_TXT))
 	@true
 
 all.png: $(addprefix $(LOCATION)/,$(ALL_PLOTS_PNG))
 	@true
 
 
-%.txt: examples/plots/%.txt
+%.txt: $(LOCATION)/%.txt
 	@true
 
-%.png: examples/plots/%.png
+%.png: $(LOCATION)/%.png
 	@true
 
 test-%.success: $(ACCEPTANCE_DIR)/%.txt
 	@mkdir -p $(TEST_LOCATION)
 	@if [ -n "$$(git diff $<)" ]; then \
 		echo "\033[1m[\033[1;31mTEST FAILED:\033[1;93m $<\033[0m\033[1m]\033[0m"; \
 		exit 1; \
```

### Comparing `mpl_ascii-0.1.0/examples/bar_chart.py` & `mpl_ascii-0.2.0/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/bar_color.py` & `mpl_ascii-0.2.0/examples/bar_label_4.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import argparse
 import matplotlib as mpl
 
-
 mpl.use("module://mpl_ascii")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("--out", type=str)
 
     args = parser.parse_args()
     out = args.out
 
     import matplotlib.pyplot as plt
+    import numpy as np
 
-    fig, ax = plt.subplots()
+    fruit_names = ['Coffee', 'Salted Caramel', 'Pistachio']
+    fruit_counts = [4000, 2000, 7000]
 
-    fruits = ['apple', 'blueberry', 'cherry', 'orange']
-    counts = [40, 100, 30, 55]
-    bar_labels = ['red', 'blue', '_red', 'orange']
-    bar_colors = ['tab:red', 'tab:blue', 'tab:red', 'tab:orange']
-
-    ax.bar(fruits, counts, label=bar_labels, color=bar_colors)
-
-    ax.set_ylabel('fruit supply')
-    ax.set_title('Fruit supply by kind and color')
-    ax.legend(title='Fruit color')
+    fig, ax = plt.subplots()
+    bar_container = ax.bar(fruit_names, fruit_counts)
+    ax.set(ylabel='pints sold', title='Gelato sales by flavor', ylim=(0, 8000))
+    ax.bar_label(bar_container, fmt='{:,.0f}')
 
     if out:
         fig.savefig(out)
-    plt.show()
+
+    plt.show()
```

### Comparing `mpl_ascii-0.1.0/examples/bar_label_1.py` & `mpl_ascii-0.2.0/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/bar_label_2.py` & `mpl_ascii-0.2.0/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/bar_label_3.py` & `mpl_ascii-0.2.0/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/bar_label_5.py` & `mpl_ascii-0.2.0/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/bar_stacked.py` & `mpl_ascii-0.2.0/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/barh.py` & `mpl_ascii-0.2.0/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/broken_barh.py` & `mpl_ascii-0.2.0/examples/lines_multi_color.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 import argparse
 import matplotlib as mpl
 
+
 mpl.use("module://mpl_ascii")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("--out", type=str)
 
     args = parser.parse_args()
     out = args.out
-
     import matplotlib.pyplot as plt
+    import numpy as np
+
+    # Set up the figure and axes
+    fig, ax = plt.subplots(figsize=(10, 6))
+
+    # Create an array of x values
+    x = np.linspace(-2 * np.pi, 2 * np.pi, 400)
+
+    # Generate different continuous functions
+    y1 = -x**2 - 4*x - 1
+    y2 = np.tan(x)
+    y3 = 8*np.exp(-x**2)  # Gaussian
+    y4 = x**3 - 6*x**2 + 9*x  # Cubic polynomial
 
-# Horizontal bar plot with gaps
-    fig, ax = plt.subplots()
-    ax.broken_barh([(110, 30), (150, 10)], (10, 9), facecolors='tab:blue')
-    ax.broken_barh([(10, 50), (100, 20), (130, 10)], (20, 9),
-                facecolors=('tab:orange', 'tab:green', 'tab:red'))
-    ax.set_ylim(5, 35)
-    ax.set_xlim(0, 200)
-    ax.set_xlabel('seconds since start')
-    ax.set_yticks([15, 25], labels=['Bill', 'Jim'])     # Modify y-axis tick labels
-    ax.grid(True)                                       # Make grid lines visible
-    ax.annotate('race interrupted', (61, 25),
-                xytext=(0.8, 0.9), textcoords='axes fraction',
-                arrowprops=dict(facecolor='black', shrink=0.05),
-                fontsize=16,
-                horizontalalignment='right', verticalalignment='top')
 
 
+    # Plot the functions
+    ax.plot(x, y1, label='-x**2 - 4x - 1')
+    ax.plot(x, y2, label='tan(x)', clip_on=True)
+    ax.plot(x, y3, label='8exp(-x^2)')
+    ax.plot(x, y4, label='x^3 - 6x^2 + 9x')
+
+    # Set labels, title, and legend
+    ax.set_title('Plot of Continuous Functions')
+    ax.set_xlabel('x')
+    ax.set_ylabel('f(x)')
+    ax.set_ylim(-10, 10)  # Limit y-axis to avoid extreme values from tan(x)
+    ax.legend()
+
+    # Add grid
+    ax.grid(True)
+
+    # Show the plot
+
     if out:
         fig.savefig(out)
-    plt.show()
+
+    plt.show()
```

### Comparing `mpl_ascii-0.1.0/examples/categorical_variables.py` & `mpl_ascii-0.2.0/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/cohere.py` & `mpl_ascii-0.2.0/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/cohere_single_plot.py` & `mpl_ascii-0.2.0/examples/cohere_single_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/csd_demo.py` & `mpl_ascii-0.2.0/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/double_plot.py` & `mpl_ascii-0.2.0/examples/simple_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 
     import matplotlib.pyplot as plt
     import numpy as np
 
     # Data for plotting
     t = np.arange(0.0, 2.0, 0.01)
     s = 1 + np.sin(2 * np.pi * t)
-    c = 1 + np.cos(2 * np.pi * t)
 
     fig, ax = plt.subplots()
     ax.plot(t, s)
-    ax.plot(t, c)
 
     ax.set(xlabel='time (s)', ylabel='voltage (mV)',
         title='About as simple as it gets, folks')
     # ax.grid()
 
-    plt.show()
     if out:
         fig.savefig(out)
+
+    plt.show()
```

### Comparing `mpl_ascii-0.1.0/examples/hist_best_fit_line.py` & `mpl_ascii-0.2.0/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/hist_simple.py` & `mpl_ascii-0.2.0/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/hist_simple_colors.py` & `mpl_ascii-0.2.0/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/examples/scatter_multi_color.py` & `mpl_ascii-0.2.0/examples/scatter_multi_color.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import argparse
 import matplotlib as mpl
+import mpl_ascii
 
+mpl_ascii.AXES_WIDTH=100
+mpl_ascii.AXES_HEIGHT=40
 
 mpl.use("module://mpl_ascii")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("--out", type=str)
```

### Comparing `mpl_ascii-0.1.0/examples/simple_plot.py` & `mpl_ascii-0.2.0/examples/double_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import argparse
 import matplotlib as mpl
+import mpl_ascii
+
+mpl_ascii.AXES_WIDTH=100
+mpl_ascii.AXES_HEIGHT=40
 
 
 mpl.use("module://mpl_ascii")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument("--out", type=str)
@@ -13,19 +17,20 @@
 
     import matplotlib.pyplot as plt
     import numpy as np
 
     # Data for plotting
     t = np.arange(0.0, 2.0, 0.01)
     s = 1 + np.sin(2 * np.pi * t)
+    c = 1 + np.cos(2 * np.pi * t)
 
     fig, ax = plt.subplots()
     ax.plot(t, s)
+    ax.plot(t, c)
 
     ax.set(xlabel='time (s)', ylabel='voltage (mV)',
         title='About as simple as it gets, folks')
     # ax.grid()
 
+    plt.show()
     if out:
         fig.savefig(out)
-
-    plt.show()
```

### Comparing `mpl_ascii-0.1.0/mpl_ascii/__init__.py` & `mpl_ascii-0.2.0/mpl_ascii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 import numpy as np
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
 from mpl_ascii.color_map import map_color_to_ascii
 from mpl_ascii.draw import draw_bar, draw_frame, draw_line, draw_x_ticks, draw_y_ticks
 from mpl_ascii.tools import linear_transform
 
-
+AXES_WIDTH = 150
+AXES_HEIGHT = 40
 
 class RendererAscii(RendererAgg):
 
     def __init__(self, width, height, dpi):
         super(RendererAscii, self).__init__(width, height, dpi)
         self.texts = []
         self.tick_info = []
@@ -64,16 +65,16 @@
         return self.renderer
 
     def to_txt(self, sep="\n", tw=240, invert=False, threshold=200):
         self.draw()
 
         figure = self.figure
 
-        axes_width = 150
-        axes_height = 40
+        axes_height = AXES_HEIGHT
+        axes_width = AXES_WIDTH
 
         frame_buffer_left = 1
         frame_buffer_right = 1
         frame_buffer_top = 1
         frame_buffer_bottom = 1
```

### Comparing `mpl_ascii-0.1.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.2.0/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/mpl_ascii/color_map.py` & `mpl_ascii-0.2.0/mpl_ascii/color_map.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/mpl_ascii/draw.py` & `mpl_ascii-0.2.0/mpl_ascii/draw.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/mpl_ascii/overlay.py` & `mpl_ascii-0.2.0/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.1.0/tests/test_overlay.py` & `mpl_ascii-0.2.0/tests/test_overlay.py`

 * *Files identical despite different names*

