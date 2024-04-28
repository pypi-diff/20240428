# Comparing `tmp/PyPulseHeatPipe-1.0.3.tar.gz` & `tmp/PyPulseHeatPipe-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPulseHeatPipe-1.0.3.tar", last modified: Mon Jun 19 23:05:38 2023, max compression
+gzip compressed data, was "PyPulseHeatPipe-1.0.4.tar", last modified: Sun Apr 28 10:24:45 2024, max compression
```

## Comparing `PyPulseHeatPipe-1.0.3.tar` & `PyPulseHeatPipe-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255387 PyPulseHeatPipe-1.0.3/
--rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.3/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     2039 2023-06-19 23:05:38.255429 PyPulseHeatPipe-1.0.3/PKG-INFO
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.254054 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/
--rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)    12723 2023-06-19 22:52:55.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/analysis.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255010 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     2039 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      346 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       70 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       16 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)     1686 2023-06-19 22:40:16.000000 PyPulseHeatPipe-1.0.3/README.md
--rw-r--r--   0 nirmal     (501) staff       (20)       79 2023-06-19 23:05:38.255602 PyPulseHeatPipe-1.0.3/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      773 2023-06-19 22:31:12.000000 PyPulseHeatPipe-1.0.3/setup.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255157 PyPulseHeatPipe-1.0.3/test/
--rw-r--r--   0 nirmal     (501) staff       (20)    12724 2023-06-19 22:23:29.000000 PyPulseHeatPipe-1.0.3/test/test_analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672936 PyPulseHeatPipe-1.0.4/
+-rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.4/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2340 2024-04-28 10:24:45.672864 PyPulseHeatPipe-1.0.4/PKG-INFO
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.670042 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/
+-rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)    12710 2024-04-28 10:05:05.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672032 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2340 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      346 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       70 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       16 2024-04-28 10:24:45.000000 PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)     1798 2023-10-28 16:14:01.000000 PyPulseHeatPipe-1.0.4/README.md
+-rw-r--r--   0 nirmal     (501) staff       (20)       79 2024-04-28 10:24:45.673275 PyPulseHeatPipe-1.0.4/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      773 2024-04-28 10:23:55.000000 PyPulseHeatPipe-1.0.4/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2024-04-28 10:24:45.672186 PyPulseHeatPipe-1.0.4/test/
+-rw-r--r--   0 nirmal     (501) staff       (20)    12724 2023-06-19 22:23:29.000000 PyPulseHeatPipe-1.0.4/test/test_analysis.py
```

### Comparing `PyPulseHeatPipe-1.0.3/LICENSE` & `PyPulseHeatPipe-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.3/PKG-INFO` & `PyPulseHeatPipe-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.3
+Version: 1.0.4
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+Requires-Dist: gitpython
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: openpyxl
 
 # PulseHeatPipe
 
 [PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
+
+# for pkg upgrade
+pip install --upgrade PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
+### to creat blank file
+    analysis.blank_file()
 
 ## list of avilable functions
+0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
 7. plot_all_data
@@ -57,19 +71,19 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
```

### Comparing `PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/analysis.py` & `PyPulseHeatPipe-1.0.4/test/test_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
         useage: data = analysis.data_chop(df, Tmin, Tmax)
         here, Tmin/Tmax is a suitable value (int) from the data.
         default values: Tmin=300, Tmax=400
         """
         Tmina = data['Te[K]'].min()
         Tmaxa = data['Te[K]'].max()
-        assert Tmin < Tmax, f"Entered wrong values: Correct range [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa,4)}]"
+        assert Tmin < Tmax, f"Entered wrong values: Correct range [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa,4)} ]"
         print(f"Optimal range of temperature(Te) for data selection: [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa)}]")
         data_T = data[data['Te[K]'] <= Tmax]
         data_T = data_T[data_T['Te[K]'] >= Tmin]
         return data_T
     
         # data mixing and re-arranging
     def data_stat(self, data:pd.DataFrame, property = 'Te[K]'):
```

### Comparing `PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/PKG-INFO` & `PyPulseHeatPipe-1.0.4/PyPulseHeatPipe.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.3
+Version: 1.0.4
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
 Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+Requires-Dist: gitpython
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: openpyxl
 
 # PulseHeatPipe
 
 [PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
+
+# for pkg upgrade
+pip install --upgrade PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
+### to creat blank file
+    analysis.blank_file()
 
 ## list of avilable functions
+0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
 7. plot_all_data
@@ -57,19 +71,19 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
```

### Comparing `PyPulseHeatPipe-1.0.3/README.md` & `PyPulseHeatPipe-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # PulseHeatPipe
 
 [PyPulseHeatPipe](https://pypi.org/project/PyPulseHeatPipe/) is a Python Library for data analysis and for data plotting/visualisation specifically for PHP experimental data.
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
+
+# for pkg upgrade
+pip install --upgrade PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
     from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
     analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
     df, df_conv = analysis.data_etl()
+### to creat blank file
+    analysis.blank_file()
 
 ## list of avilable functions
+0. blank_file
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
 6. best_TP
 7. plot_all_data
@@ -46,23 +52,23 @@
 # for ETL
 df, df_conv = analysis.data_etl()
 
 # for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
-**NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
+**NOTE**: The experimental data file must prepared in '.xlsx' format. The data must contain atleast following columns with mentioned titles:
 
 >**samle_data.xlsx format**
 
-| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| t(min) | Tc[C] | Te[C] | P[mmHg] | Q[W] | alpha | beta | phase |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 | 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
 | --- | --- | --- | --- | --- | --- | --- | --- |
 
 here,
 
 alpha = vertical angle of PHP
 
 beta = horizontal angle of PHP
 
-phase = phase split of the working fluid
+phase = phase split of the working fluid
```

### Comparing `PyPulseHeatPipe-1.0.3/setup.py` & `PyPulseHeatPipe-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='PyPulseHeatPipe',
-        version='1.0.3',
+        version='1.0.4',
         license='GNU',
         url='https://github.com/nirmalparmarphd/PyPulseHeatPipe',
         description='The data analysis Python package for the Pulsating Heat Pipe experimental data', 
         long_description=long_description,
         long_description_content_type='text/markdown',
         author='Nirmal Parmar, PhD',
         author_email='nirmalparmarphd@gmail.com',
```

### Comparing `PyPulseHeatPipe-1.0.3/test/test_analysis.py` & `PyPulseHeatPipe-1.0.4/PyPulseHeatPipe/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,135 +7,135 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 sns.set()
 
 ## Data Analysis
 class PulseHeatPipe:
     """
-    ## PulseHeatPipe is a Python library to perform thermodynamic data analysis on experimental data of pulsating heat pipe. This library is developed to estimate optimal working condition based on the change in Gibbs free energy in the pusating heat pipe.
+    ## PulseHeatPipe is a Python library to perform thermodynamic data analysis on experimental data of pulsating heat pipe. This library is developed to estimate optimal working condition based on the change in Gibbs free energy in the pulsating heat pipe.
 
     Please find more detail at https://github.com/nirmalparmarphd/PyPulseHeatPipe 
 
-    ## Useage: 
-    ### imorting the module
-    from PyPulseHeatPipe import PulsHeatPipe, DataVisualisation
+    ## Usage: 
+    ### importing the module
+    from PyPulseHeatPipe import PulsHeatPipe, DataVisualization
     ### setting working directory
-    analysis = PulseHaatPipe("datapath", "sample)
+    analysis = PulseHeatPipe("datapath", "sample)
     ### for a class help 
     help(analysis)
     ### for a function help
     help(analysis.data_etl)
     ### using a function from the class
     df, df_conv = analysis.data_etl
     """
     def __init__(self, datapath:str, sample:str):
         self.T_k = 273.15 # To convert in kelvin
         self.P_const = 750.062 # To convert in bar
         self.R_const = 8.314 # Real Gas constant
         self.dG_standard = 30.9 # dG of water
-        self.P_standard = 1 # atomospher pressure
+        self.P_standard = 1 # atmosphere pressure
         self.datapath = datapath
         self.sample = sample
         print(f"Datapath loaded for working directory: {self.datapath}\n")
         print(f"Sample name saved as: {self.sample}")
 
     # sample xlsx blank file
     def blank_file(self, blank='blank.xlsx'):
         """
-        blank_file is a method to generate a blank sample (.xlsx) file to prepare data file that can futher used in thermodynamic analysis. 
+        blank_file is a method to generate a blank sample (.xlsx) file to prepare data file that can further used in thermodynamic analysis. 
         
-        't(min)'= timestemp,
-        'Te[C]'= Eveporator Temperature,
-        'Tc[C]'= Condensor Temperature,
+        'time'= timestamp,
+        'Te[C]'= Evaporator Temperature,
+        'Tc[C]'= Condenser Temperature,
         'P[mmHg]'= Pressure of PHP,
         'Q[W]'= Power Supply,
         'alpha'= Horizontal Angle of PHP,
         'beta'= Vertical Angle of PHP, 
-        'phase'= Visible phase split (y/n)
+        'pulse'= Visible pulse generation (y=1/n=0)
 
-        useage: analysis = PulseHeatPipe("path")
+        usage: analysis = PulseHeatPipe("path")
                 analysis.blank_file()
         """
         self.blank = blank
-        df_blank = pd.DataFrame({'t(min)':[1] ,'Te[C]':[1], 'Tc[C]':[1],'P[mmHg]':[1], 'Q[W]':[1], 'alpha':[1], 'beta':[1], 'phase':[1]})
+        df_blank = pd.DataFrame({'time':[1] ,'Te[C]':[1], 'Tc[C]':[1],'P[mmHg]':[1], 'Q[W]':[1], 'alpha':[1], 'beta':[1], 'pulse':[1]})
         # creating blank file
         df_blank_out = df_blank.to_excel(self.datapath + self.blank)
-        msg = (f"### {self.blank} file is created. Please enter the experimental data in this file. Do not ulter or change of the column's head. ###");
+        msg = (f"### {self.blank} file is created. Please enter the experimental data in this file. Do not alter or change of the column's head. ###")
         return msg
     
     # data ETL    
     def data_etl(self, name='*', ext='.xlsx'):
         """
         data_etl loads experimental data from all experimental data files (xlsx).
         Filters data and keeps only important columns.
         Combine selected data and save to csv file.
-        Conver units to MKS [K, bar] system and save to csv file. 
+        Convert units to MKS [K, bar] system and save to csv file. 
 
-        useage: analysis = PulseHeatPipe("path", "sample")
+        usage: analysis = PulseHeatPipe("path", "sample")
                 df, df_conv = analysis.data_etl()
         """
         self.name = name
         self.ext = ext
         data_filenames_list = glob.glob((self.datapath + self.name + self.ext))
         df_frames = []
         print('list of files considered for ETL: \n',data_filenames_list)
         for i in range(0, len(data_filenames_list)) :
             # loading data in loop
             df_raw = pd.read_excel(data_filenames_list[i])
-            selected_columns = ['t(min)' ,'Te[C]', 'Tc[C]','P[mmHg]', 'Q[W]', 'alpha', 'beta', 'phase']
+            selected_columns = ['time' ,'Te[C]', 'Tc[C]','P[mmHg]', 'Q[W]', 'alpha', 'beta', 'pulse']
             df_selected_columns = df_raw[selected_columns]
             df_frames.append(df_selected_columns)
         df = pd.concat(df_frames, axis=0, ignore_index=True).dropna()
       
-        df_conv_fram = [df['t(min)'], df['Te[C]']+self.T_k, df['Tc[C]']+self.T_k, df['Te[C]']-df['Tc[C]'] , df['P[mmHg]']/self.P_const, df['Q[W]'], (df['Te[C]']-df['Tc[C]'])/df['Q[W]'] , df['alpha'], df['beta'], df['phase']]
+        df_conv_fram = [df['time'], df['Te[C]']+self.T_k, df['Tc[C]']+self.T_k, df['Te[C]']-df['Tc[C]'] , df['P[mmHg]']/self.P_const, df['Q[W]'], (df['Te[C]']-df['Tc[C]'])/df['Q[W]'] , df['alpha'], df['beta'], df['pulse']]
         df_conv = pd.concat(df_conv_fram, axis=1, ignore_index=True).dropna()
-        df_conv_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'phase']
+        df_conv_columns = ['time' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'pulse']
         df_conv.columns = df_conv_columns
         # saving
         df_out = df.to_csv(self.datapath + self.sample + "_combined_data.csv")
         df_conv_out = df_conv.to_csv(self.datapath + self.sample + "_combined_converted_data.csv")
         print(f"### Compiled and converted data is saved at: {self.datapath}'{self.sample}_combined_converted_data.csv' ###")
         return df, df_conv
     
     # to calculate gibbs free energy at given (T[K],P[bar])
     def gibbs_fe(self, data:pd.DataFrame):
         """
-        gibbs_fe calculates the chagne in the gibbs free energy at a given vacuum pressure and temperature.
+        gibbs_fe calculates the change in the gibbs free energy at a given vacuum pressure and temperature.
         dG = dG' + RTln(P/P')
         here, R = 8.314 [J/molK]
         P and P' = Pressure [bar]
         T = Temperature [K]
 
-        useage: df_gfe = analysis.gibbs_fe(data)
+        usage: df_gfe = analysis.gibbs_fe(data)
         """
         Te = (data['Te[K]']) 
         Tc = (data['Tc[K]'])  
         P_vacuum = (data['P[bar]']) # converting to bar
         dG_vacuume_Te = self.R_const * Te * np.log(P_vacuum/self.P_standard)
         dG_vacuume_Tc = self.R_const * Tc * np.log(P_vacuum/self.P_standard)
         dG = dG_vacuume_Te - dG_vacuume_Tc
-        selected_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'phase', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
+        selected_columns = ['time' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'pulse', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         data = pd.concat([data, dG_vacuume_Te, dG_vacuume_Tc, dG], axis=1, ignore_index=True)
         data.columns = selected_columns
         data_out = data.to_csv(self.datapath + "gfe_combined.csv")
         msg = print(f"Gibbs Free Energy calculated data saved at: {self.datapath}'gfe_combined.csv")
         return data
     
     # To select data from specific Te range
     def data_chop(self, data:pd.DataFrame, Tmin=300, Tmax=400):
         """ 
         data_chop function is used to chop the data for the selected temperature value from the Te[K] column.
 
-        useage: data = analysis.data_chop(df, Tmin, Tmax)
+        usage: data = analysis.data_chop(df, Tmin, Tmax)
         here, Tmin/Tmax is a suitable value (int) from the data.
         default values: Tmin=300, Tmax=400
         """
         Tmina = data['Te[K]'].min()
         Tmaxa = data['Te[K]'].max()
-        assert Tmin < Tmax, f"Entered wrong values: Correct range [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa,4)} ]"
+        assert Tmin < Tmax, f"Entered wrong values: Correct range [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa,4)}]"
         print(f"Optimal range of temperature(Te) for data selection: [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa)}]")
         data_T = data[data['Te[K]'] <= Tmax]
         data_T = data_T[data_T['Te[K]'] >= Tmin]
         return data_T
     
         # data mixing and re-arranging
     def data_stat(self, data:pd.DataFrame, property = 'Te[K]'):
@@ -153,15 +153,15 @@
         return df_mean, df_std
     
     # prepare average values for all thermal properties
     def data_property_avg(self, df_mean:pd.DataFrame, df_std:pd.DataFrame):
         """
         data_property_avg calculates average values of measured thermal properties for the given experiment data.
 
-        useage: analysis.data_property_avg(df_mean, df_std)
+        usage: analysis.data_property_avg(df_mean, df_std)
         """
         # avg values 
         Tc_avg = df_mean['Tc[K]'].mean()
         P_avg = df_mean['P[bar]'].mean()
         dT_avg = df_mean['dT[K]'].mean()
         TR_avg = df_mean['TR[K/W]'].mean()
         GFE_avg = df_mean['GFE_Tc[KJ/mol]'].mean()
@@ -180,15 +180,15 @@
         return print(msg)
     
     # find optimal G(T,P) of PHP
     def best_TP(self, data:pd.DataFrame):
         """ 
         best_TP finds best G(T,P) with lowest dG (Change in Gibbs Free Energy for Te->Tc values at constant Pressure) from the experimental dataset.
 
-        useage: analysis.best_TP(data)
+        usage: analysis.best_TP(data)
         """
         df_opt = data[data['dG[KJ/mol]'] == data['dG[KJ/mol]'].min()]
         df_opt_idx = df_opt.index
         Tc_opt = data['Tc[K]'].loc[df_opt_idx]
         Te_opt = data['Te[K]'].loc[df_opt_idx]
         dT_opt = data['dT[K]'].loc[df_opt_idx]
         P_opt = data['P[bar]'].loc[df_opt_idx]
@@ -197,70 +197,70 @@
         TR_opt = data['TR[K/W]'].loc[df_opt_idx]
         msg = (f'Optimal G(T,P) condition at lowest (optimal) dG[{round(dG_opt.iloc[0],4)}]\n'
                f'Tc optimal:        {round(Tc_opt.iloc[0],4)}[K] \n'
                f'Te optimal:        {round(Te_opt.iloc[0],4)}[K] \n'
                f'P  optimal:        {round(P_opt.iloc[0],4)}[bar] \n'
                f'dT optimal:        {round(dT_opt.iloc[0],4)}[K] \n'
                f'TR optimal:        {round(TR_opt.iloc[0],4)}[K/W] \n'
-               f'GFE optimal:       dG({round(Te_opt.iloc[0],4)}, {round(P_opt.iloc[0],4)}) = {round(GFE_opt.iloc[0],4)} [KJ/mol]\n');
+               f'GFE optimal:       dG({round(Te_opt.iloc[0],4)}, {round(P_opt.iloc[0],4)}) = {round(GFE_opt.iloc[0],4)} [KJ/mol]\n')
         return print(msg)
     
 ## Data Visualisation
 class DataVisualisation(PulseHeatPipe):
     """ ## Data Visualisation class to plot PHP data.
 
-        ## useage: 
+        ## usage: 
         ### importing module
         from analysis import DataVisualisation
         ### creating the reference variable
         visual = DataVisualisation('sample')
         ### data visualisation; eg. plotting all data
         visual.plot_all_data()
     """
     def __init__(self, datapath: str, sample: str):
         super().__init__(datapath, sample)
         
     def plot_all_data(self, data:pd.DataFrame):
         """ Data Visualisation
             
-            useage: visual.plot_all_data(data)
+            usage: visual.plot_all_data(data)
         """
         plt.figure(figsize=(10,5))
         sns.lineplot(data)
         plt.xlabel('Data')
         plt.ylabel('Properties')
         plt.title(f"All Data - {self.sample}")
         plt.legend()
 
     def plot_Te_Tc(self, data:pd.DataFrame):
         """ Data Visualisation
             
-            useage: visual.plot_Te_Tc(data)
+            usage: visual.plot_Te_Tc(data)
         """
         plt.figure(figsize=(10,5))
         plt.plot(data['Te[K]'], label = 'Te[K]')
         plt.plot(data['Tc[K]'], label = 'Tc[K]')
         plt.xlabel('Te[K]')
         plt.ylabel('Tc[K]')
         plt.title(f"Te[K] vs Tc[K] - {self.sample}")
         plt.legend()
 
     def plot_eu(self, df_mean:pd.DataFrame, df_std:pd.DataFrame, property:str, point='.k', eu='r'):
         """ Data Visualisation
             
-            useage: visual.plot_eu(df_mean, df_std, property='Tc[K]', point='.k', eu='r')
+            usage: visual.plot_eu(df_mean, df_std, property='Tc[K]', point='.k', eu='r')
                     here, choose value from property list: ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         """
         self.property = property
         self.xproperty = 'Te[K]'
         self.point = point
         self.eu = eu
         properties = ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         if self.property in properties:    
-            plt.figure(figsize=(10,5));
+            plt.figure(figsize=(10,5))
             plt.plot(df_mean[self.xproperty], df_mean[self.property], self.point, label=self.property)
             idx = df_std.index
             df_mean_idx = df_mean.loc[idx]
             plt.fill_between(df_std[self.xproperty], df_mean_idx[self.property] - 2* df_std[self.property], df_mean_idx[self.property] + 2* df_std[self.property],color=self.eu, alpha=0.2, label='Expanded Uncertainty')
             plt.xlabel(self.xproperty)
             plt.ylabel(self.property)
             plt.title(f"Expanded Uncertainty - {self.sample}")
```

