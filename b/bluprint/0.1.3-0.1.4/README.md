# Comparing `tmp/bluprint-0.1.3.tar.gz` & `tmp/bluprint-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluprint-0.1.3.tar", last modified: Tue Feb  6 06:01:35 2024, max compression
+gzip compressed data, was "bluprint-0.1.4.tar", last modified: Sun Apr 28 04:38:22 2024, max compression
```

## Comparing `bluprint-0.1.3.tar` & `bluprint-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.848747 bluprint-0.1.3/
--rw-r--r--   0 igor       (501) staff       (20)     1068 2023-12-10 22:02:31.000000 bluprint-0.1.3/LICENSE
--rw-r--r--   0 igor       (501) staff       (20)       28 2023-12-24 01:45:36.000000 bluprint-0.1.3/MANIFEST.in
--rw-r--r--   0 igor       (501) staff       (20)     4522 2024-02-06 06:01:35.848270 bluprint-0.1.3/PKG-INFO
--rw-r--r--   0 igor       (501) staff       (20)     4168 2024-02-06 06:01:22.000000 bluprint-0.1.3/README.rst
--rw-r--r--   0 igor       (501) staff       (20)     3243 2024-02-06 06:01:22.000000 bluprint-0.1.3/pyproject.toml
--rw-r--r--   0 igor       (501) staff       (20)       38 2024-02-06 06:01:35.848873 bluprint-0.1.3/setup.cfg
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.817084 bluprint-0.1.3/src/
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.827690 bluprint-0.1.3/src/bluprint/
--rw-r--r--   0 igor       (501) staff       (20)        0 2023-12-12 09:33:52.000000 bluprint-0.1.3/src/bluprint/__init__.py
--rw-r--r--   0 igor       (501) staff       (20)     1972 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/binary.py
--rw-r--r--   0 igor       (501) staff       (20)     7654 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/cli.py
--rw-r--r--   0 igor       (501) staff       (20)     1480 2023-12-12 09:33:52.000000 bluprint-0.1.3/src/bluprint/colors.py
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.835278 bluprint-0.1.3/src/bluprint/create/
--rw-r--r--   0 igor       (501) staff       (20)        0 2023-12-12 09:33:52.000000 bluprint-0.1.3/src/bluprint/create/__init__.py
--rw-r--r--   0 igor       (501) staff       (20)      818 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/create/errors.py
--rw-r--r--   0 igor       (501) staff       (20)     3077 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/create/py_project.py
--rw-r--r--   0 igor       (501) staff       (20)      773 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/create/r_project.py
--rw-r--r--   0 igor       (501) staff       (20)      860 2023-12-12 09:33:52.000000 bluprint-0.1.3/src/bluprint/errors.py
--rw-r--r--   0 igor       (501) staff       (20)     1812 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/index.py
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.837758 bluprint-0.1.3/src/bluprint/notebook/
--rw-r--r--   0 igor       (501) staff       (20)     2242 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/notebook/jupyter.py
--rw-r--r--   0 igor       (501) staff       (20)      677 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/notebook/progress.py
--rw-r--r--   0 igor       (501) staff       (20)       57 2023-12-12 09:33:52.000000 bluprint-0.1.3/src/bluprint/notebook/quarto.py
--rw-r--r--   0 igor       (501) staff       (20)     1573 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/notebook/rmarkdown.py
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.842361 bluprint-0.1.3/src/bluprint/template/
--rw-r--r--   0 igor       (501) staff       (20)     6148 2023-12-18 22:56:35.000000 bluprint-0.1.3/src/bluprint/template/.DS_Store
--rw-r--r--   0 igor       (501) staff       (20)     3190 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/.gitignore
--rw-r--r--   0 igor       (501) staff       (20)       17 2023-12-24 01:45:36.000000 bluprint-0.1.3/src/bluprint/template/.pdm-python
--rw-r--r--   0 igor       (501) staff       (20)      516 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/README.md
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.844070 bluprint-0.1.3/src/bluprint/template/conf/
--rw-r--r--   0 igor       (501) staff       (20)       22 2023-12-24 01:45:36.000000 bluprint-0.1.3/src/bluprint/template/conf/config.yaml
--rw-r--r--   0 igor       (501) staff       (20)       28 2023-12-22 11:50:44.000000 bluprint-0.1.3/src/bluprint/template/conf/data.yaml
--rw-r--r--   0 igor       (501) staff       (20)       43 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/conf/workflows.yaml
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.844626 bluprint-0.1.3/src/bluprint/template/data/
--rw-r--r--   0 igor       (501) staff       (20)       23 2023-12-22 11:50:44.000000 bluprint-0.1.3/src/bluprint/template/data/example_data.csv
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.846272 bluprint-0.1.3/src/bluprint/template/notebooks/
--rw-r--r--   0 igor       (501) staff       (20)     1596 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/notebooks/example_jupyternb.ipynb
--rw-r--r--   0 igor       (501) staff       (20)      515 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/notebooks/example_quarto.qmd
--rw-r--r--   0 igor       (501) staff       (20)      423 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/notebooks/example_rmarkdown.Rmd
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.847119 bluprint-0.1.3/src/bluprint/template/placeholder_name/
--rw-r--r--   0 igor       (501) staff       (20)        0 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template/placeholder_name/__init__.py
--rw-r--r--   0 igor       (501) staff       (20)       73 2023-12-24 01:45:36.000000 bluprint-0.1.3/src/bluprint/template/placeholder_name/example.py
--rw-r--r--   0 igor       (501) staff       (20)      195 2023-12-24 01:45:36.000000 bluprint-0.1.3/src/bluprint/template/placeholder_name.Rproj
--rw-r--r--   0 igor       (501) staff       (20)      355 2023-12-24 01:45:36.000000 bluprint-0.1.3/src/bluprint/template/pyproject.toml
--rw-r--r--   0 igor       (501) staff       (20)     1069 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/template.py
--rw-r--r--   0 igor       (501) staff       (20)     2756 2024-02-06 06:01:22.000000 bluprint-0.1.3/src/bluprint/workflow.py
-drwxr-xr-x   0 igor       (501) staff       (20)        0 2024-02-06 06:01:35.847694 bluprint-0.1.3/src/bluprint.egg-info/
--rw-r--r--   0 igor       (501) staff       (20)     4522 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/PKG-INFO
--rw-r--r--   0 igor       (501) staff       (20)     1349 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/SOURCES.txt
--rw-r--r--   0 igor       (501) staff       (20)        1 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/dependency_links.txt
--rw-r--r--   0 igor       (501) staff       (20)       47 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/entry_points.txt
--rw-r--r--   0 igor       (501) staff       (20)       97 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/requires.txt
--rw-r--r--   0 igor       (501) staff       (20)        9 2024-02-06 06:01:35.000000 bluprint-0.1.3/src/bluprint.egg-info/top_level.txt
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/
+-rw-r--r--   0 igor      (1000) igor      (1000)     1068 2023-11-24 16:08:59.000000 bluprint-0.1.4/LICENSE
+-rw-r--r--   0 igor      (1000) igor      (1000)       28 2023-12-26 11:35:41.000000 bluprint-0.1.4/MANIFEST.in
+-rw-r--r--   0 igor      (1000) igor      (1000)     4918 2024-04-28 04:38:22.950477 bluprint-0.1.4/PKG-INFO
+-rw-r--r--   0 igor      (1000) igor      (1000)     4564 2024-02-22 16:05:17.000000 bluprint-0.1.4/README.rst
+-rw-r--r--   0 igor      (1000) igor      (1000)     3243 2024-04-28 04:02:59.000000 bluprint-0.1.4/pyproject.toml
+-rw-r--r--   0 igor      (1000) igor      (1000)       38 2024-04-28 04:38:22.950477 bluprint-0.1.4/setup.cfg
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/
+-rw-r--r--   0 igor      (1000) igor      (1000)        0 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/__init__.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     1972 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/binary.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     7654 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/cli.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     1480 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/colors.py
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/create/
+-rw-r--r--   0 igor      (1000) igor      (1000)        0 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/create/__init__.py
+-rw-r--r--   0 igor      (1000) igor      (1000)      818 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/errors.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     3077 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/py_project.py
+-rw-r--r--   0 igor      (1000) igor      (1000)      773 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/create/r_project.py
+-rw-r--r--   0 igor      (1000) igor      (1000)      860 2024-01-18 06:34:23.000000 bluprint-0.1.4/src/bluprint/errors.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     1812 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/index.py
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/notebook/
+-rw-r--r--   0 igor      (1000) igor      (1000)     2242 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/jupyter.py
+-rw-r--r--   0 igor      (1000) igor      (1000)      677 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/progress.py
+-rw-r--r--   0 igor      (1000) igor      (1000)       57 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/notebook/quarto.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     1573 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/notebook/rmarkdown.py
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/
+-rw-r--r--   0 igor      (1000) igor      (1000)     3190 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/.gitignore
+-rw-r--r--   0 igor      (1000) igor      (1000)       17 2024-01-24 05:11:11.000000 bluprint-0.1.4/src/bluprint/template/.pdm-python
+-rw-r--r--   0 igor      (1000) igor      (1000)      516 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/README.md
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/conf/
+-rw-r--r--   0 igor      (1000) igor      (1000)       22 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/conf/config.yaml
+-rw-r--r--   0 igor      (1000) igor      (1000)       28 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/conf/data.yaml
+-rw-r--r--   0 igor      (1000) igor      (1000)       43 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/conf/workflows.yaml
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.940477 bluprint-0.1.4/src/bluprint/template/data/
+-rw-r--r--   0 igor      (1000) igor      (1000)       23 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/data/example_data.csv
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint/template/notebooks/
+-rw-r--r--   0 igor      (1000) igor      (1000)     1596 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_jupyternb.ipynb
+-rw-r--r--   0 igor      (1000) igor      (1000)      515 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_quarto.qmd
+-rw-r--r--   0 igor      (1000) igor      (1000)      423 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/notebooks/example_rmarkdown.Rmd
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint/template/placeholder_name/
+-rw-r--r--   0 igor      (1000) igor      (1000)        0 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name/__init__.py
+-rw-r--r--   0 igor      (1000) igor      (1000)       73 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name/example.py
+-rw-r--r--   0 igor      (1000) igor      (1000)      195 2023-12-26 11:35:41.000000 bluprint-0.1.4/src/bluprint/template/placeholder_name.Rproj
+-rw-r--r--   0 igor      (1000) igor      (1000)      350 2024-04-28 04:02:44.000000 bluprint-0.1.4/src/bluprint/template/pyproject.toml
+-rw-r--r--   0 igor      (1000) igor      (1000)     1069 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/template.py
+-rw-r--r--   0 igor      (1000) igor      (1000)     2756 2024-02-06 04:12:41.000000 bluprint-0.1.4/src/bluprint/workflow.py
+drwxr-xr-x   0 igor      (1000) igor      (1000)        0 2024-04-28 04:38:22.950477 bluprint-0.1.4/src/bluprint.egg-info/
+-rw-r--r--   0 igor      (1000) igor      (1000)     4918 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/PKG-INFO
+-rw-r--r--   0 igor      (1000) igor      (1000)     1317 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/SOURCES.txt
+-rw-r--r--   0 igor      (1000) igor      (1000)        1 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/dependency_links.txt
+-rw-r--r--   0 igor      (1000) igor      (1000)       47 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/entry_points.txt
+-rw-r--r--   0 igor      (1000) igor      (1000)       97 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/requires.txt
+-rw-r--r--   0 igor      (1000) igor      (1000)        9 2024-04-28 04:38:22.000000 bluprint-0.1.4/src/bluprint.egg-info/top_level.txt
```

### Comparing `bluprint-0.1.3/LICENSE` & `bluprint-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/PKG-INFO` & `bluprint-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluprint
-Version: 0.1.3
+Version: 0.1.4
 Author: igor-sb
 License: MIT
 Requires-Python: ==3.11.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: notebook>=7.0.6
 Requires-Dist: fire>=0.5.0
@@ -14,88 +14,84 @@
 Requires-Dist: nbstripout>=0.6.1
 
 .. image:: docs/source/images/bluprint_logo.png
 
 Bluprint
 ========
 
-**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint projects allow Jupyter and RMarkdown notebooks seamless access to configuration, data and shared code, using best coding practices, in this type of project structure::
+**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint allows seamless access to configuration, data and shared code in this type of project structure created by ``bluprint create my_project``::
 
     my_project
     ├── conf
     │   └── data.yaml
     ├── data
     │   ├── emailed
     │   │   └── messy.xlsx
     │   └── user_processed.csv
     ├── notebooks
     │   └── process.ipynb
     └── my_project
         └── shared_code.py
 
-
-Features
---------
-
-* Configuration, data and shared code (Python/R scripts) separated from notebooks.
-
-* Mixing of any or all Python/R scripts and Jupyter/RMarkdown notebooks.
-
-* Consistent access to configuration and data, e.g. ``data.emailed.messy`` (Python) automatically resolves to */path/to/my_project/data/emailed/messy.xlsx*.
-
-* Consistent access to project modules, e.g. ``from my_project import shared_code`` in any notebook in any sub-directory.
-
-* Share project easily; just copy the project directory and run ``pdm install``.
-
-* Reproducibility: Python and R dependencies are version locked.
-
-* Works with tools for notebook linting, testing, CI/CD and workflows.
-
-* Bluprint projects are Python packages; use ``pip install /path/to/my_project`` to reuse shared code across projects.
-
-
-Usage
------
-
-``bluprint create my_project`` creates a project skeleton similar to the example shown above. Once created, we can add data files and store all file paths relative to the *my_project/data* directory, in the *data.yaml*:
+Storing paths relative to the *my_project* directory in *conf/data.yaml*:
 
 .. code:: yaml
 
     emailed:
         messy: 'emailed/messy.xlsx'
     user:
         processed: 'user_processed.csv'
 
-Then retrieve the automatically parsed full paths, for example in *process.ipynb* above:
+allows you access them in a Python script or Jupyter notebook anywhere within the project:
 
 .. code:: python
 
-    # bluprint_conf is a helper package for loading configs 
     from bluprint_conf import load_data_yaml
-    from my_project.shared_code import process_data
-    import pandas as pd
 
-    data = load_data_yaml() # default arg: conf/data.yaml
+    data = load_data_yaml() # By default loads conf/data.yaml
     print(data)
     #> {
     #>   'emailed': {
     #>     'messy': '/path/to/my_project/data/emailed/messy.xlsx'
     #>   },
     #>   'user': {
     #> 	   'processed': '/path/to/my_project/data/user_processed.csv'
-    #>   }
+    #>   },
+    #>   'remote': {
+    #>     'extras': 's3://path/to/extra_data.csv'
+    #>   },
     #> }
 
+    # Load data in a portable manner
+    import pandas as pd
     messy_df = pd.read_xlsx(data.emailed.messy)
+    extras_df = pd.read_xlsx(data.remote.extras)
+
+    # Load shared code functions as Python modules
+    from my_project.shared_code import transform_data
+    transformed_df = transform_data(messy_df, extras_df)
 
-    processed_df = process_data(messy_df)
+    # Save output
+    transformed_df.to_csv(data.user.processed)
 
-    processed_df.to_csv(data.user.processed)
 
-For a working demonstration of a shareable project https://github.com/igor-sb/bluprint-demo/.
+.. note::
+
+    For a working demonstration of a shareable project see https://github.com/igor-sb/bluprint-demo/.
+
+Features
+--------
+
+- Write portable notebooks by loading configs with `load_data_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.data.load_data_yaml>`_ and `load_config_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.config.load_config_yaml>`_
+- R/Python packages automatically version-locked using `renv <https://rstudio.github.io/renv/>`_ and `PDM <https://pdm-project.org/latest/>`_
+- Import shared code as Python modules
+- Install shared code across projects with `pip install <https://igor-sb.github.io/bluprint/prod_projects.html>`_
+- Use both Python and R notebooks in a single project (see `Python/R projects </https://igor-sb.github.io/bluprint/getting_started.html#python-r-projects>`_)
+- Share projects by copying a project directory and running *pdm install*
+- Works with common IDEs (RStudio, VSCode), notebook tools for linting (`nbqa <https://nbqa.readthedocs.io/en/latest/>`_), notebook version control (`nbstripout <https://github.com/kynan/nbstripout>`_) or workflows (`Ploomber <https://github.com/ploomber/ploomber>`_)
 
 Documentation
 -------------
 
 Full documentation available at: https://igor-sb.github.io/bluprint/.
 
 
@@ -115,18 +111,16 @@
 References
 ----------
 
 Bluprint integrates:
 
 * `PDM <https://pdm-project.org/latest/>`_
 * `OmegaConf <https://omegaconf.readthedocs.io/>`_
-* Python's native import system
-* R package `renv <https://rstudio.github.io/renv/>`_
-* R package `here <https://here.r-lib.org/>`_ 
-* R package `reticulate <https://rstudio.github.io/reticulate/>`_
+* Python's native import system `importlib <https://docs.python.org/3/library/importlib.html>`_
+* R packages `{renv} <https://rstudio.github.io/renv/>`_, `{here} <https://here.r-lib.org/>`_ and `{reticulate} <https://rstudio.github.io/reticulate/>`_
 
 Bluprint is heavily inspired by these resources:
 
 * Author's own frustration of dealing with malfunctioning notebooks for over a decade.
 * `Cookiecutter Data Science <https://drivendata.github.io/cookiecutter-data-science/>`_
 * `RStudio Projects <https://support.posit.co/hc/en-us/articles/200526207-Using-RStudio-Projects>`_
 * `Ploomber <https://github.com/ploomber/ploomber>`_
```

### Comparing `bluprint-0.1.3/README.rst` & `bluprint-0.1.4/src/bluprint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,97 @@
+Metadata-Version: 2.1
+Name: bluprint
+Version: 0.1.4
+Author: igor-sb
+License: MIT
+Requires-Python: ==3.11.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: notebook>=7.0.6
+Requires-Dist: fire>=0.5.0
+Requires-Dist: omegaconf>=2.3.0
+Requires-Dist: tqdm>=4.66.1
+Requires-Dist: bluprint-conf>=0.1.0
+Requires-Dist: nbstripout>=0.6.1
+
 .. image:: docs/source/images/bluprint_logo.png
 
 Bluprint
 ========
 
-**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint projects allow Jupyter and RMarkdown notebooks seamless access to configuration, data and shared code, using best coding practices, in this type of project structure::
+**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint allows seamless access to configuration, data and shared code in this type of project structure created by ``bluprint create my_project``::
 
     my_project
     ├── conf
     │   └── data.yaml
     ├── data
     │   ├── emailed
     │   │   └── messy.xlsx
     │   └── user_processed.csv
     ├── notebooks
     │   └── process.ipynb
     └── my_project
         └── shared_code.py
 
-
-Features
---------
-
-* Configuration, data and shared code (Python/R scripts) separated from notebooks.
-
-* Mixing of any or all Python/R scripts and Jupyter/RMarkdown notebooks.
-
-* Consistent access to configuration and data, e.g. ``data.emailed.messy`` (Python) automatically resolves to */path/to/my_project/data/emailed/messy.xlsx*.
-
-* Consistent access to project modules, e.g. ``from my_project import shared_code`` in any notebook in any sub-directory.
-
-* Share project easily; just copy the project directory and run ``pdm install``.
-
-* Reproducibility: Python and R dependencies are version locked.
-
-* Works with tools for notebook linting, testing, CI/CD and workflows.
-
-* Bluprint projects are Python packages; use ``pip install /path/to/my_project`` to reuse shared code across projects.
-
-
-Usage
------
-
-``bluprint create my_project`` creates a project skeleton similar to the example shown above. Once created, we can add data files and store all file paths relative to the *my_project/data* directory, in the *data.yaml*:
+Storing paths relative to the *my_project* directory in *conf/data.yaml*:
 
 .. code:: yaml
 
     emailed:
         messy: 'emailed/messy.xlsx'
     user:
         processed: 'user_processed.csv'
 
-Then retrieve the automatically parsed full paths, for example in *process.ipynb* above:
+allows you access them in a Python script or Jupyter notebook anywhere within the project:
 
 .. code:: python
 
-    # bluprint_conf is a helper package for loading configs 
     from bluprint_conf import load_data_yaml
-    from my_project.shared_code import process_data
-    import pandas as pd
 
-    data = load_data_yaml() # default arg: conf/data.yaml
+    data = load_data_yaml() # By default loads conf/data.yaml
     print(data)
     #> {
     #>   'emailed': {
     #>     'messy': '/path/to/my_project/data/emailed/messy.xlsx'
     #>   },
     #>   'user': {
     #> 	   'processed': '/path/to/my_project/data/user_processed.csv'
-    #>   }
+    #>   },
+    #>   'remote': {
+    #>     'extras': 's3://path/to/extra_data.csv'
+    #>   },
     #> }
 
+    # Load data in a portable manner
+    import pandas as pd
     messy_df = pd.read_xlsx(data.emailed.messy)
+    extras_df = pd.read_xlsx(data.remote.extras)
+
+    # Load shared code functions as Python modules
+    from my_project.shared_code import transform_data
+    transformed_df = transform_data(messy_df, extras_df)
 
-    processed_df = process_data(messy_df)
+    # Save output
+    transformed_df.to_csv(data.user.processed)
 
-    processed_df.to_csv(data.user.processed)
 
-For a working demonstration of a shareable project https://github.com/igor-sb/bluprint-demo/.
+.. note::
+
+    For a working demonstration of a shareable project see https://github.com/igor-sb/bluprint-demo/.
+
+Features
+--------
+
+- Write portable notebooks by loading configs with `load_data_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.data.load_data_yaml>`_ and `load_config_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.config.load_config_yaml>`_
+- R/Python packages automatically version-locked using `renv <https://rstudio.github.io/renv/>`_ and `PDM <https://pdm-project.org/latest/>`_
+- Import shared code as Python modules
+- Install shared code across projects with `pip install <https://igor-sb.github.io/bluprint/prod_projects.html>`_
+- Use both Python and R notebooks in a single project (see `Python/R projects </https://igor-sb.github.io/bluprint/getting_started.html#python-r-projects>`_)
+- Share projects by copying a project directory and running *pdm install*
+- Works with common IDEs (RStudio, VSCode), notebook tools for linting (`nbqa <https://nbqa.readthedocs.io/en/latest/>`_), notebook version control (`nbstripout <https://github.com/kynan/nbstripout>`_) or workflows (`Ploomber <https://github.com/ploomber/ploomber>`_)
 
 Documentation
 -------------
 
 Full documentation available at: https://igor-sb.github.io/bluprint/.
 
 
@@ -100,18 +111,16 @@
 References
 ----------
 
 Bluprint integrates:
 
 * `PDM <https://pdm-project.org/latest/>`_
 * `OmegaConf <https://omegaconf.readthedocs.io/>`_
-* Python's native import system
-* R package `renv <https://rstudio.github.io/renv/>`_
-* R package `here <https://here.r-lib.org/>`_ 
-* R package `reticulate <https://rstudio.github.io/reticulate/>`_
+* Python's native import system `importlib <https://docs.python.org/3/library/importlib.html>`_
+* R packages `{renv} <https://rstudio.github.io/renv/>`_, `{here} <https://here.r-lib.org/>`_ and `{reticulate} <https://rstudio.github.io/reticulate/>`_
 
 Bluprint is heavily inspired by these resources:
 
 * Author's own frustration of dealing with malfunctioning notebooks for over a decade.
 * `Cookiecutter Data Science <https://drivendata.github.io/cookiecutter-data-science/>`_
 * `RStudio Projects <https://support.posit.co/hc/en-us/articles/200526207-Using-RStudio-Projects>`_
 * `Ploomber <https://github.com/ploomber/ploomber>`_
```

### Comparing `bluprint-0.1.3/pyproject.toml` & `bluprint-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bluprint"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = [
 	{name = "igor-sb"},
 ]
 readme = "README.rst"
 license = { text = "MIT" }
 requires-python = "==3.11.*"
```

### Comparing `bluprint-0.1.3/src/bluprint/binary.py` & `bluprint-0.1.4/src/bluprint/binary.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/cli.py` & `bluprint-0.1.4/src/bluprint/cli.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/colors.py` & `bluprint-0.1.4/src/bluprint/colors.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/create/errors.py` & `bluprint-0.1.4/src/bluprint/create/errors.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/create/py_project.py` & `bluprint-0.1.4/src/bluprint/create/py_project.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/create/r_project.py` & `bluprint-0.1.4/src/bluprint/create/r_project.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/errors.py` & `bluprint-0.1.4/src/bluprint/errors.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/index.py` & `bluprint-0.1.4/src/bluprint/index.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/notebook/jupyter.py` & `bluprint-0.1.4/src/bluprint/notebook/jupyter.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/notebook/progress.py` & `bluprint-0.1.4/src/bluprint/notebook/progress.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/notebook/rmarkdown.py` & `bluprint-0.1.4/src/bluprint/notebook/rmarkdown.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/template/.gitignore` & `bluprint-0.1.4/src/bluprint/template/.gitignore`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/template/README.md` & `bluprint-0.1.4/src/bluprint/template/README.md`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/template/notebooks/example_jupyternb.ipynb` & `bluprint-0.1.4/src/bluprint/template/notebooks/example_jupyternb.ipynb`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/template/notebooks/example_quarto.qmd` & `bluprint-0.1.4/src/bluprint/template/notebooks/example_quarto.qmd`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/template.py` & `bluprint-0.1.4/src/bluprint/template.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint/workflow.py` & `bluprint-0.1.4/src/bluprint/workflow.py`

 * *Files identical despite different names*

### Comparing `bluprint-0.1.3/src/bluprint.egg-info/PKG-INFO` & `bluprint-0.1.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,82 @@
-Metadata-Version: 2.1
-Name: bluprint
-Version: 0.1.3
-Author: igor-sb
-License: MIT
-Requires-Python: ==3.11.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: notebook>=7.0.6
-Requires-Dist: fire>=0.5.0
-Requires-Dist: omegaconf>=2.3.0
-Requires-Dist: tqdm>=4.66.1
-Requires-Dist: bluprint-conf>=0.1.0
-Requires-Dist: nbstripout>=0.6.1
-
 .. image:: docs/source/images/bluprint_logo.png
 
 Bluprint
 ========
 
-**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint projects allow Jupyter and RMarkdown notebooks seamless access to configuration, data and shared code, using best coding practices, in this type of project structure::
+**Bluprint** is a command line utility for streamlined exploratory data science projects. Bluprint allows seamless access to configuration, data and shared code in this type of project structure created by ``bluprint create my_project``::
 
     my_project
     ├── conf
     │   └── data.yaml
     ├── data
     │   ├── emailed
     │   │   └── messy.xlsx
     │   └── user_processed.csv
     ├── notebooks
     │   └── process.ipynb
     └── my_project
         └── shared_code.py
 
-
-Features
---------
-
-* Configuration, data and shared code (Python/R scripts) separated from notebooks.
-
-* Mixing of any or all Python/R scripts and Jupyter/RMarkdown notebooks.
-
-* Consistent access to configuration and data, e.g. ``data.emailed.messy`` (Python) automatically resolves to */path/to/my_project/data/emailed/messy.xlsx*.
-
-* Consistent access to project modules, e.g. ``from my_project import shared_code`` in any notebook in any sub-directory.
-
-* Share project easily; just copy the project directory and run ``pdm install``.
-
-* Reproducibility: Python and R dependencies are version locked.
-
-* Works with tools for notebook linting, testing, CI/CD and workflows.
-
-* Bluprint projects are Python packages; use ``pip install /path/to/my_project`` to reuse shared code across projects.
-
-
-Usage
------
-
-``bluprint create my_project`` creates a project skeleton similar to the example shown above. Once created, we can add data files and store all file paths relative to the *my_project/data* directory, in the *data.yaml*:
+Storing paths relative to the *my_project* directory in *conf/data.yaml*:
 
 .. code:: yaml
 
     emailed:
         messy: 'emailed/messy.xlsx'
     user:
         processed: 'user_processed.csv'
 
-Then retrieve the automatically parsed full paths, for example in *process.ipynb* above:
+allows you access them in a Python script or Jupyter notebook anywhere within the project:
 
 .. code:: python
 
-    # bluprint_conf is a helper package for loading configs 
     from bluprint_conf import load_data_yaml
-    from my_project.shared_code import process_data
-    import pandas as pd
 
-    data = load_data_yaml() # default arg: conf/data.yaml
+    data = load_data_yaml() # By default loads conf/data.yaml
     print(data)
     #> {
     #>   'emailed': {
     #>     'messy': '/path/to/my_project/data/emailed/messy.xlsx'
     #>   },
     #>   'user': {
     #> 	   'processed': '/path/to/my_project/data/user_processed.csv'
-    #>   }
+    #>   },
+    #>   'remote': {
+    #>     'extras': 's3://path/to/extra_data.csv'
+    #>   },
     #> }
 
+    # Load data in a portable manner
+    import pandas as pd
     messy_df = pd.read_xlsx(data.emailed.messy)
+    extras_df = pd.read_xlsx(data.remote.extras)
+
+    # Load shared code functions as Python modules
+    from my_project.shared_code import transform_data
+    transformed_df = transform_data(messy_df, extras_df)
 
-    processed_df = process_data(messy_df)
+    # Save output
+    transformed_df.to_csv(data.user.processed)
 
-    processed_df.to_csv(data.user.processed)
 
-For a working demonstration of a shareable project https://github.com/igor-sb/bluprint-demo/.
+.. note::
+
+    For a working demonstration of a shareable project see https://github.com/igor-sb/bluprint-demo/.
+
+Features
+--------
+
+- Write portable notebooks by loading configs with `load_data_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.data.load_data_yaml>`_ and `load_config_yaml() <https://igor-sb.github.io/bluprint-conf/html/reference.html#bluprint_conf.config.load_config_yaml>`_
+- R/Python packages automatically version-locked using `renv <https://rstudio.github.io/renv/>`_ and `PDM <https://pdm-project.org/latest/>`_
+- Import shared code as Python modules
+- Install shared code across projects with `pip install <https://igor-sb.github.io/bluprint/prod_projects.html>`_
+- Use both Python and R notebooks in a single project (see `Python/R projects </https://igor-sb.github.io/bluprint/getting_started.html#python-r-projects>`_)
+- Share projects by copying a project directory and running *pdm install*
+- Works with common IDEs (RStudio, VSCode), notebook tools for linting (`nbqa <https://nbqa.readthedocs.io/en/latest/>`_), notebook version control (`nbstripout <https://github.com/kynan/nbstripout>`_) or workflows (`Ploomber <https://github.com/ploomber/ploomber>`_)
 
 Documentation
 -------------
 
 Full documentation available at: https://igor-sb.github.io/bluprint/.
 
 
@@ -115,18 +96,16 @@
 References
 ----------
 
 Bluprint integrates:
 
 * `PDM <https://pdm-project.org/latest/>`_
 * `OmegaConf <https://omegaconf.readthedocs.io/>`_
-* Python's native import system
-* R package `renv <https://rstudio.github.io/renv/>`_
-* R package `here <https://here.r-lib.org/>`_ 
-* R package `reticulate <https://rstudio.github.io/reticulate/>`_
+* Python's native import system `importlib <https://docs.python.org/3/library/importlib.html>`_
+* R packages `{renv} <https://rstudio.github.io/renv/>`_, `{here} <https://here.r-lib.org/>`_ and `{reticulate} <https://rstudio.github.io/reticulate/>`_
 
 Bluprint is heavily inspired by these resources:
 
 * Author's own frustration of dealing with malfunctioning notebooks for over a decade.
 * `Cookiecutter Data Science <https://drivendata.github.io/cookiecutter-data-science/>`_
 * `RStudio Projects <https://support.posit.co/hc/en-us/articles/200526207-Using-RStudio-Projects>`_
 * `Ploomber <https://github.com/ploomber/ploomber>`_
```

### Comparing `bluprint-0.1.3/src/bluprint.egg-info/SOURCES.txt` & `bluprint-0.1.4/src/bluprint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 src/bluprint/create/errors.py
 src/bluprint/create/py_project.py
 src/bluprint/create/r_project.py
 src/bluprint/notebook/jupyter.py
 src/bluprint/notebook/progress.py
 src/bluprint/notebook/quarto.py
 src/bluprint/notebook/rmarkdown.py
-src/bluprint/template/.DS_Store
 src/bluprint/template/.gitignore
 src/bluprint/template/.pdm-python
 src/bluprint/template/README.md
 src/bluprint/template/placeholder_name.Rproj
 src/bluprint/template/pyproject.toml
 src/bluprint/template/conf/config.yaml
 src/bluprint/template/conf/data.yaml
```

