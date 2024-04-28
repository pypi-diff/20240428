# Comparing `tmp/progress-table-1.3.2.tar.gz` & `tmp/progress-table-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-1.3.2.tar", last modified: Sat Apr  6 12:00:35 2024, max compression
+gzip compressed data, was "progress-table-2.0.0.tar", last modified: Sun Apr 28 18:31:15 2024, max compression
```

## Comparing `progress-table-1.3.2.tar` & `progress-table-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.893101 progress-table-1.3.2/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-1.3.2/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-06 12:00:35.893101 progress-table-1.3.2/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4143 2024-03-12 12:06:20.000000 progress-table-1.3.2/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.889768 progress-table-1.3.2/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      287 2024-04-06 12:00:21.000000 progress-table-1.3.2/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.889768 progress-table-1.3.2/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-1.3.2/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-1.3.2/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-1.3.2/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.893101 progress-table-1.3.2/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.2/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    29325 2024-04-06 11:02:30.000000 progress-table-1.3.2/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3132 2024-04-04 15:47:39.000000 progress-table-1.3.2/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.893101 progress-table-1.3.2/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-06 12:00:35.000000 progress-table-1.3.2/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-1.3.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      593 2024-04-06 12:00:35.000000 progress-table-1.3.2/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-06 12:00:35.000000 progress-table-1.3.2/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-06 12:00:35.000000 progress-table-1.3.2/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-06 12:00:35.000000 progress-table-1.3.2/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-1.3.2/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-06 12:00:35.893101 progress-table-1.3.2/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-04 15:47:39.000000 progress-table-1.3.2/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-06 12:00:35.893101 progress-table-1.3.2/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-1.3.2/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1860 2024-04-06 12:00:21.000000 progress-table-1.3.2/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.0.0/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4852 2024-04-28 18:31:15.864310 progress-table-2.0.0/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4088 2024-04-28 18:30:30.000000 progress-table-2.0.0/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-28 18:30:30.000000 progress-table-2.0.0/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.0.0/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.0.0/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.0.0/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.0.0/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    45615 2024-04-28 18:30:41.000000 progress-table-2.0.0/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5170 2024-04-28 18:30:30.000000 progress-table-2.0.0/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4852 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.0.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      593 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.0.0/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-28 18:31:15.864310 progress-table-2.0.0/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.0.0/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.0.0/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1849 2024-04-28 18:30:30.000000 progress-table-2.0.0/tests/test_examples_automated.py
```

### Comparing `progress-table-1.3.2/LICENSE.txt` & `progress-table-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/PKG-INFO` & `progress-table-2.0.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.3.2
+Version: 1.2.3
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: colorama
 
 > Note: versions 1.X introduced new features and changes of default behaviour.
 >
 > The old version is still available as `progress_table.ProgressTableV0`.
 >
 > New features include:
 > * Nested progress bar support
```

### Comparing `progress-table-1.3.2/progress_table/v0/progress_table.py` & `progress-table-2.0.0/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/progress_table/v0/symbols.py` & `progress-table-2.0.0/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/progress_table.egg-info/PKG-INFO` & `progress-table-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.3.2
+Version: 2.0.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,120 +15,115 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: colorama
 
-> Note: versions 1.X introduced new features and changes of default behaviour.
+> Version 2.X introduces new features and new interactive modes.
 >
-> The old version is still available as `progress_table.ProgressTableV0`.
->
-> New features include:
-> * Nested progress bar support
-> * Custom table styles support
-> * Color customization on row level support
-> * Adding columns automatically, without calling `add_column`
-> * Continuous progress bar when iterator length is unknown
-> * Pandas and numpy being only optional dependencies
-> * Other minor changes
+> New features allow for previously impossible applications, see examples below.
 
 # Progress Table
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fprogress-table%2Fjson)](https://pypi.org/project/progress-table)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fprogress-table%2Fjson)](https://pypi.org/project/progress-table)
 
 Lightweight utility to display the progress of your process as a pretty table in the command line.
-Alternative to TQDM whenever you want to track metrics produced by your process.
-
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-table-example.png?raw=true)
-
-Designed to monitor machine learning experiments, but can be used for any metrics-producing process.
-Allows you to quickly see what's going on with your process.
-Increases readability and simplifies your command line logging.
 
-## Purpose
+* Alternative to TQDM whenever you want to track metrics produced by your process
+* Designed to monitor ML experiments, but works for any metrics-producing process
+* Allows you to see at a glance what's going on with your process
+* Increases readability and simplifies your command line logging
 
-Change this:
+### Change this:
 
 ![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-before3.gif?raw=true)
 
-Into this:
+### Into this:
 
 ![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-after4.gif?raw=true)
 
-## Example
+## Examples
+
+* Neural network training
+
+![example-training](images/examples-training.gif)
+
+* Progress of multi-threaded downloads
+
+![example-download](images/examples-download.gif)
+
+* Simulation and interactive display of Brownian motion
+
+![example-brown2d](images/examples-brown2d.gif)
+
+* Display of a game board
 
-> Click here for examples of integration with deep learning libraries:
-> [integrations.md](https://github.com/gahaalt/progress-table/blob/main/integrations.md).
+![example-tictactoe](images/examples-tictactoe.gif)
+
+## Quick start code
 
 ```python
 import random
-import sys
 import time
 
 from progress_table import ProgressTable
 
 # Create table object:
-table = ProgressTable()
+table = ProgressTable(num_decimal_places=1)
 
-# Or customize its settings:
-table = ProgressTable(
-    columns=["step"],
-    refresh_rate=20,
-    num_decimal_places=4,
-    default_column_width=None,
-    default_column_color=None,
-    default_column_alignment=None,
-    default_column_aggregate=None,
-    default_row_color=None,
-    embedded_progress_bar=True,
-    pbar_show_throughput=True,
-    pbar_show_progress=False,
-    print_row_on_update=True,
-    reprint_header_every_n_rows=30,
-    custom_format=None,
-    table_style="round",
-    file=sys.stdout,
-)
-
-# You (optionally) define the columns at the beginning
-table.add_column("x", width=3)
-table.add_column("x root", color="red")
-table.add_column("random average", color=["bright", "red"], aggregate="mean")
+# You can (optionally) define the columns at the beginning
+table.add_column("x", color="bold red")
 
 for step in range(10):
     x = random.randint(0, 200)
 
-    # There are two ways to add new values:
+    # You can add entries in a compact way
     table["x"] = x
-    table["step"] = step
-    # Second:
-    table.update("x root", x ** 0.5)
-    table.update("x squared", x ** 2)
 
-    # Display the progress bar by wrapping the iterator
+    # Or you can use the update method
+    table.update("x", value=x, weight=1.0)
+
+    # Display the progress bar by wrapping an iterator or an integer
     for _ in table(10):  # -> Equivalent to `table(range(10))`
-        # You can use weights for aggregated values
-        table.update("random average", random.random(), weight=1)
+        # Set and get values from the table
+        table["y"] = random.randint(0, 200)
+        table["x-y"] = table["x"] - table["y"]
+        table.update("average x-y", value=table["x-y"], weight=1.0, aggregate="mean")
         time.sleep(0.1)
 
     # Go to the next row when you're ready
     table.next_row()
 
-# Close the table when it's ready
+# Close the table when it's finished
 table.close()
 
-# Export your data
-data = table.to_list()
-pandas_df = table.to_df()  # Requires pandas to be installed
-np_array = table.to_numpy()  # Requires numpy to be installed
 ```
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/example-output4.gif?raw=true)
+> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs/integrations.md)
+> page to see examples of integration with deep learning libraries.
+
+## Advanced usage
+
+Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs/advanced-usage.md) page for more information.
+
+## Troubleshooting
+
+### Exceesive output
+
+Progress Table works correctly in most consoles, but there are some exceptions:
+
+* Some cloud logging consoles (e.g. kubernetes) don't support `\r` properly.
+  You can still use ProgressTable, but with `interactive=0` option. This mode will not display progress bars.
+* Some consoles like `PyCharm Python Console` or `IDLE` don't support cursor movement.
+  You can still use ProgressTable, but with `interactive=1` option. This mode displays only 1 progress bar at once.
+
+> By default `interactive=2`. You can change the default `interactive` by
+> setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
 
 ## Installation
 
 Install Progress Table easily with pip:
 
 ```
 pip install progress-table
```

### Comparing `progress-table-1.3.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.0.0/progress_table.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.2.3
+Version: 2.0.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,121 +13,117 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: colorama
 
-> Note: versions 1.X introduced new features and changes of default behaviour.
+> Version 2.X introduces new features and new interactive modes.
 >
-> The old version is still available as `progress_table.ProgressTableV0`.
->
-> New features include:
-> * Nested progress bar support
-> * Custom table styles support
-> * Color customization on row level support
-> * Adding columns automatically, without calling `add_column`
-> * Continuous progress bar when iterator length is unknown
-> * Pandas and numpy being only optional dependencies
-> * Other minor changes
+> New features allow for previously impossible applications, see examples below.
 
 # Progress Table
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fprogress-table%2Fjson)](https://pypi.org/project/progress-table)
 [![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fprogress-table%2Fjson)](https://pypi.org/project/progress-table)
 
 Lightweight utility to display the progress of your process as a pretty table in the command line.
-Alternative to TQDM whenever you want to track metrics produced by your process.
-
-![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-table-example.png?raw=true)
-
-Designed to monitor machine learning experiments, but can be used for any metrics-producing process.
-Allows you to quickly see what's going on with your process.
-Increases readability and simplifies your command line logging.
 
-## Purpose
+* Alternative to TQDM whenever you want to track metrics produced by your process
+* Designed to monitor ML experiments, but works for any metrics-producing process
+* Allows you to see at a glance what's going on with your process
+* Increases readability and simplifies your command line logging
 
-Change this:
+### Change this:
 
 ![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-before3.gif?raw=true)
 
-Into this:
+### Into this:
 
 ![example](https://github.com/gahaalt/progress-table/blob/main/images/progress-after4.gif?raw=true)
 
-## Example
+## Examples
+
+* Neural network training
+
+![example-training](images/examples-training.gif)
+
+* Progress of multi-threaded downloads
+
+![example-download](images/examples-download.gif)
+
+* Simulation and interactive display of Brownian motion
+
+![example-brown2d](images/examples-brown2d.gif)
+
+* Display of a game board
 
-> Click here for examples of integration with deep learning libraries:
-> [integrations.md](https://github.com/gahaalt/progress-table/blob/main/integrations.md).
+![example-tictactoe](images/examples-tictactoe.gif)
+
+## Quick start code
 
 ```python
 import random
-import sys
 import time
 
 from progress_table import ProgressTable
 
 # Create table object:
-table = ProgressTable()
+table = ProgressTable(num_decimal_places=1)
 
-# Or customize its settings:
-table = ProgressTable(
-    columns=["step"],
-    refresh_rate=20,
-    num_decimal_places=4,
-    default_column_width=None,
-    default_column_color=None,
-    default_column_alignment=None,
-    default_column_aggregate=None,
-    default_row_color=None,
-    embedded_progress_bar=True,
-    pbar_show_throughput=True,
-    pbar_show_progress=False,
-    print_row_on_update=True,
-    reprint_header_every_n_rows=30,
-    custom_format=None,
-    table_style="round",
-    file=sys.stdout,
-)
-
-# You (optionally) define the columns at the beginning
-table.add_column("x", width=3)
-table.add_column("x root", color="red")
-table.add_column("random average", color=["bright", "red"], aggregate="mean")
+# You can (optionally) define the columns at the beginning
+table.add_column("x", color="bold red")
 
 for step in range(10):
     x = random.randint(0, 200)
 
-    # There are two ways to add new values:
+    # You can add entries in a compact way
     table["x"] = x
-    table["step"] = step
-    # Second:
-    table.update("x root", x ** 0.5)
-    table.update("x squared", x ** 2)
 
-    # Display the progress bar by wrapping the iterator
+    # Or you can use the update method
+    table.update("x", value=x, weight=1.0)
+
+    # Display the progress bar by wrapping an iterator or an integer
     for _ in table(10):  # -> Equivalent to `table(range(10))`
-        # You can use weights for aggregated values
-        table.update("random average", random.random(), weight=1)
+        # Set and get values from the table
+        table["y"] = random.randint(0, 200)
+        table["x-y"] = table["x"] - table["y"]
+        table.update("average x-y", value=table["x-y"], weight=1.0, aggregate="mean")
         time.sleep(0.1)
 
     # Go to the next row when you're ready
     table.next_row()
 
-# Close the table when it's ready
+# Close the table when it's finished
 table.close()
 
-# Export your data
-data = table.to_list()
-pandas_df = table.to_df()  # Requires pandas to be installed
-np_array = table.to_numpy()  # Requires numpy to be installed
 ```
 
-![example](https://github.com/gahaalt/progress-table/blob/main/images/example-output4.gif?raw=true)
+> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs/integrations.md)
+> page to see examples of integration with deep learning libraries.
+
+## Advanced usage
+
+Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs/advanced-usage.md) page for more information.
+
+## Troubleshooting
+
+### Exceesive output
+
+Progress Table works correctly in most consoles, but there are some exceptions:
+
+* Some cloud logging consoles (e.g. kubernetes) don't support `\r` properly.
+  You can still use ProgressTable, but with `interactive=0` option. This mode will not display progress bars.
+* Some consoles like `PyCharm Python Console` or `IDLE` don't support cursor movement.
+  You can still use ProgressTable, but with `interactive=1` option. This mode displays only 1 progress bar at once.
+
+> By default `interactive=2`. You can change the default `interactive` by
+> setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
 
 ## Installation
 
 Install Progress Table easily with pip:
 
 ```
 pip install progress-table
```

### Comparing `progress-table-1.3.2/progress_table.egg-info/SOURCES.txt` & `progress-table-2.0.0/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/setup.py` & `progress-table-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/tests/test_docs_automated.py` & `progress-table-2.0.0/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `progress-table-1.3.2/tests/test_examples_automated.py` & `progress-table-2.0.0/tests/test_examples_automated.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 #  Copyright (c) 2022-2024 Szymon Mikler
 
 import hashlib
 import importlib
-import random
 import sys
 from glob import glob
 from io import StringIO
 
 EXPECTED_OUTPUTS = {
-    "examples.nn_training": "7e50cfd539e3e1799ecd5a7e7b7a7e18",
-    "examples.cumulating": "b5b7bc9b8232545ebfd5ca777bddacb4",
-    "examples.fibonacci": "bae5411af4bf8a4326f1bce59ca9aad9",
-    "examples.features": "474d4aff94a3070d2300d78d4159e0a6",
+    "examples.training": "14af860a37118c16aec4604e5629e5ed",
+    "examples.tictactoe": "056841a6cbf7456cd3daacbff356088a",
+    "examples.brown2d": "c0f37fdfcfc2db6ef465473c67c05d83",
 }
 
 
-def set_seed():
-    random.seed(42)
-
-
 def capture_example_stdout(main_fn):
     # To eliminate run to run variation of the example outputs we need to be independent from the execution speed
     # This includes removing the influence of:
     # * refresh rate
     # * throughput display
+
     override_kwds = dict(
-        refresh_rate=1000000000,
         pbar_show_throughput=False,
+        refresh_rate=0,
     )
 
     # We will replace stdout with custom StringIO and check whether example stdout is as expected
     out_buffer = StringIO()
     sys.stdout = out_buffer
-    set_seed()
-    main_fn(**override_kwds)
+    main_fn(random_seed=42, **override_kwds)
     sys.stdout = sys.__stdout__
     return out_buffer.getvalue()
 
 
 def test_all_examples():
     # Testing whether examples run exactly as intended
 
     outputs = {}
     for module in glob("examples/*"):
         module = module.replace(".py", "").replace("/", ".")
+
+        if module not in EXPECTED_OUTPUTS:
+            print(f"Skipping example: {module}")
+            continue
         print(f"Running example: {module}")
+
         main_fn = importlib.import_module(module).main
         out_str = capture_example_stdout(main_fn)
 
         md5hash = hashlib.md5(out_str.encode()).hexdigest()
         outputs[module] = md5hash
 
     err_msg = []
```

