# Comparing `tmp/PyPulseHeatPipe-1.0.4.tar.gz` & `tmp/PyPulseHeatPipe-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPulseHeatPipe-1.0.4.tar", last modified: Sun Apr 28 10:24:45 2024, max compression
+gzip compressed data, was "PyPulseHeatPipe-1.0.6.tar", last modified: Sun Apr 28 10:40:24 2024, max compression
```

## Comparing `PyPulseHeatPipe-1.0.4.tar` & `PyPulseHeatPipe-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672936 PyPulseHeatPipe-1.0.4/
--rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.4/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     2340 2024-04-28 10:24:45.672864 PyPulseHeatPipe-1.0.4/PKG-INFO
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.670042 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/
--rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)    12710 2024-04-28 10:05:05.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/analysis.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672032 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     2340 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      346 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       70 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       16 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)     1798 2023-10-28 16:14:01.000000 PyPulseHeatPipe-1.0.4/README.md
--rw-r--r--   0 nirmal     (501) staff       (20)       79 2024-04-28 10:24:45.673275 PyPulseHeatPipe-1.0.4/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      773 2024-04-28 10:23:55.000000 PyPulseHeatPipe-1.0.4/setup.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672186 PyPulseHeatPipe-1.0.4/test/
--rw-r--r--   0 nirmal     (501) staff       (20)    12724 2023-06-19 22:23:29.000000 PyPulseHeatPipe-1.0.4/test/test_analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:40:24.466605 PyPulseHeatPipe-1.0.6/
+-rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.6/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2359 2024-04-28 10:40:24.466532 PyPulseHeatPipe-1.0.6/PKG-INFO
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:40:24.464726 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe/
+-rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)    12710 2024-04-28 10:05:05.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe/analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:40:24.465845 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2359 2024-04-28 10:40:24.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      346 2024-04-28 10:40:24.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2024-04-28 10:40:24.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       70 2024-04-28 10:40:24.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       16 2024-04-28 10:40:24.000000 PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)     1817 2024-04-28 10:39:11.000000 PyPulseHeatPipe-1.0.6/README.md
+-rw-r--r--   0 nirmal     (501) staff       (20)       79 2024-04-28 10:40:24.466803 PyPulseHeatPipe-1.0.6/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      773 2024-04-28 10:39:55.000000 PyPulseHeatPipe-1.0.6/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:40:24.465966 PyPulseHeatPipe-1.0.6/test/
+-rw-r--r--   0 nirmal     (501) staff       (20)    12724 2023-06-19 22:23:29.000000 PyPulseHeatPipe-1.0.6/test/test_analysis.py
```

### Comparing `PyPulseHeatPipe-1.0.4/LICENSE` & `PyPulseHeatPipe-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.4/PKG-INFO` & `PyPulseHeatPipe-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.4
+Version: 1.0.6
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,29 +24,29 @@
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 
 # for pkg upgrade
 pip install --upgrade PyPulseHeatPipe
 ```
-## Useage: 
-### imorting the module
+## Usage:  
+### importing the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath", "sample_name")
+    analysis = PulseHeatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
-### to creat blank file
+### to create blank file
     analysis.blank_file()
 
-## list of avilable functions
+## list of available functions
 0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
@@ -71,23 +71,23 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain at least following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | pulse |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
 
 beta = horizontal angle of PHP
 
-phase = phase split of the working fluid
+pulse = pulse generation in the working fluid (y=1/n=0)
```

### Comparing `PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/analysis.py` & `PyPulseHeatPipe-1.0.6/PyPulseHeatPipe/analysis.py`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/PKG-INFO` & `PyPulseHeatPipe-1.0.6/PyPulseHeatPipe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.4
+Version: 1.0.6
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,29 +24,29 @@
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 
 # for pkg upgrade
 pip install --upgrade PyPulseHeatPipe
 ```
-## Useage: 
-### imorting the module
+## Usage:  
+### importing the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath", "sample_name")
+    analysis = PulseHeatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
-### to creat blank file
+### to create blank file
     analysis.blank_file()
 
-## list of avilable functions
+## list of available functions
 0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
@@ -71,23 +71,23 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain at least following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | pulse |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
 
 beta = horizontal angle of PHP
 
-phase = phase split of the working fluid
+pulse = pulse generation in the working fluid (y=1/n=0)
```

### Comparing `PyPulseHeatPipe-1.0.4/README.md` & `PyPulseHeatPipe-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 
 # for pkg upgrade
 pip install --upgrade PyPulseHeatPipe
 ```
-## Useage: 
-### imorting the module
+## Usage:  
+### importing the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath", "sample_name")
+    analysis = PulseHeatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
-### to creat blank file
+### to create blank file
     analysis.blank_file()
 
-## list of avilable functions
+## list of available functions
 0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
@@ -52,23 +52,23 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain at least following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | pulse |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
 
 beta = horizontal angle of PHP
 
-phase = phase split of the working fluid
+pulse = pulse generation in the working fluid (y=1/n=0)
```

### Comparing `PyPulseHeatPipe-1.0.4/setup.py` & `PyPulseHeatPipe-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='PyPulseHeatPipe',
-        version='1.0.4',
+        version='1.0.6',
         license='GNU',
         url='https://github.com/nirmalparmarphd/PyPulseHeatPipe',
         description='The data analysis Python package for the Pulsating Heat Pipe experimental data', 
         long_description=long_description,
         long_description_content_type='text/markdown',
         author='Nirmal Parmar, PhD',
         author_email='nirmalparmarphd@gmail.com',
```

### Comparing `PyPulseHeatPipe-1.0.4/test/test_analysis.py` & `PyPulseHeatPipe-1.0.6/test/test_analysis.py`

 * *Files identical despite different names*

