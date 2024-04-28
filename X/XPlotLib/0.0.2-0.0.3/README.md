# Comparing `tmp/xplotlib-0.0.2.tar.gz` & `tmp/xplotlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplotlib-0.0.2.tar", last modified: Thu Apr 25 04:23:46 2024, max compression
+gzip compressed data, was "xplotlib-0.0.3.tar", last modified: Sun Apr 28 05:34:59 2024, max compression
```

## Comparing `xplotlib-0.0.2.tar` & `xplotlib-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.909131 xplotlib-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 04:23:40.000000 xplotlib-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 04:23:46.909131 xplotlib-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 04:23:40.000000 xplotlib-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 04:23:40.000000 xplotlib-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 04:23:46.909131 xplotlib-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.901131 xplotlib-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.905131 xplotlib-0.0.2/src/XPlotLib/
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/BandgapAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/DOSAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/XPlotLibUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:40.000000 xplotlib-0.0.2/src/XPlotLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:23:46.905131 xplotlib-0.0.2/src/XPlotLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 04:23:46.000000 xplotlib-0.0.2/src/XPlotLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 05:34:51.000000 xplotlib-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 05:34:59.869901 xplotlib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 05:34:51.000000 xplotlib-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 05:34:51.000000 xplotlib-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-28 05:34:59.869901 xplotlib-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.865901 xplotlib-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/src/XPlotLib/
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/BandgapAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/DOSAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/XPlotLibUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/src/XPlotLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/top_level.txt
```

### Comparing `xplotlib-0.0.2/LICENSE` & `xplotlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.2/PKG-INFO` & `xplotlib-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xplotlib-0.0.2/setup.cfg` & `xplotlib-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = XPlotLib
-version = 0.0.2
+version = 0.0.3
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Libary to plot experimental and theoretical XRay data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `xplotlib-0.0.2/src/XPlotLib/BandgapAnalyzer.py` & `xplotlib-0.0.3/src/XPlotLib/BandgapAnalyzer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
-from .XPlotLibUtils import non_uniform_savgol
+from .XPlotLibUtils import non_uniform_savgol, ryd_to_ev
 
 class BandgapAnalyzer():
     def __init__(self):
         self.xes_exp_spectra = {}
         self.xes_calc_spectra = {}
         self.xas_exp_spectra = {}
         self.xas_calc_spectra = {}
@@ -13,14 +13,17 @@
         self.xes_xlims = None
         self.xas_xlims = None
         self.subplot_labels = [['XES' , 'XAS'], ['2nd der.', '2nd der.']]
         self.xes_arrow = None
         self.xas_arrow = None
         self.title = None
 
+        self.gs_onsets = []
+        self.es_onsets = []
+
     def __load_spectrum(self, path, names, skiprows, sep):
         headers = [[f'{header}_energy', f'{header}_intensity'] for header in names]
         headers = [item for sublist in headers for item in sublist]
         return pd.read_csv(path, sep=sep, skiprows=skiprows, header=None, names=headers)
     
     def __normalize(self, list):
         abs_max = max(max(list), -min(list))
@@ -118,14 +121,17 @@
         exp_spectra[name][f'{name}_smoothed_2nd'] = np.gradient(np.gradient(y_smoothed, x), x)
 
         if show:
             # plot the smoothed data
             if onset_region:
                 fig, (ax, ax_onset) = plt.subplots(1,2, figsize=(10,6))
                 ax_onset.set_xlim(onset_region)
+                ax_onset.set_xlim(onset_region)
+                y_onset = exp_spectra[name].loc[(exp_spectra[name][f'{name}_energy'] >= onset_region[0]) & (exp_spectra[name][f'{name}_energy'] <= onset_region[1]), f'{name}_intensity']
+                ax_onset.set_ylim(min(y_onset), max(y_onset))
                 ax_onset.plot(x, y, label='Raw data')
                 ax_onset.plot(x, y_smoothed, label='Smoothed data')
                 ax_onset.legend()
             else:
                 fig, ax = plt.subplots()
             ax.plot(x, y, label='Raw data')
             ax.plot(x, y_smoothed, label='Smoothed data')
@@ -213,26 +219,26 @@
 
         # XES
         if self.xes_xlims:
             axes[0,0].set_xlim(self.xes_xlims)
             axes[1,0].set_xlim(self.xes_xlims)
         for xes_exp_name in xes_exp_names:
             axes[0,0].plot(self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy'], self.__normalize(self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_intensity']), label=xes_exp_name)
-            axes[1,0].plot(self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy'], self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_smoothed_2nd'])
+            axes[1,0].plot(self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy'],  self.__normalize(self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_smoothed_2nd']))
         for xes_calc_name in xes_calc_names:
             axes[0,0].plot(self.xes_calc_spectra[xes_calc_name][f'{xes_calc_name}_energy'], self.__normalize(self.xes_calc_spectra[xes_calc_name][f'{xes_calc_name}_intensity']), label=xes_calc_name)
 
 
         # XAS
         if self.xas_xlims:
             axes[0,1].set_xlim(self.xas_xlims)
             axes[1,1].set_xlim(self.xas_xlims)
         for xas_exp_name in xas_exp_names:
             axes[0,1].plot(self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy'], self.__normalize(self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_intensity']), label=xas_exp_name)
-            axes[1,1].plot(self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy'], self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_smoothed_2nd'])
+            axes[1,1].plot(self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy'],  self.__normalize(self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_smoothed_2nd']))
         for xas_calc_name in xas_calc_names:
             axes[0,1].plot(self.xas_calc_spectra[xas_calc_name][f'{xas_calc_name}_energy'], self.__normalize(self.xas_calc_spectra[xas_calc_name][f'{xas_calc_name}_intensity']), label=xas_calc_name)
 
         # remove space between subplots
         fig.subplots_adjust(wspace=0, hspace=0)
 
         if self.title:
@@ -264,8 +270,50 @@
             if self.xes_arrow:
                 xy, xytext, text, text_rot = self.xes_arrow
                 axes[1,0].annotate(text, xy=xy, xytext=xytext, arrowprops=dict(facecolor='black', shrink=0.05), ha='center', va='center', rotation=text_rot)
 
             # annotate first XAS peak
             if self.xas_arrow:
                 xy, xytext, text, text_rot = self.xas_arrow
-                axes[1,1].annotate(text, xy=xy, xytext=xytext, arrowprops=dict(facecolor='black', shrink=0.05), ha='center', va='center', rotation=text_rot)
+                axes[1,1].annotate(text, xy=xy, xytext=xytext, arrowprops=dict(facecolor='black', shrink=0.05), ha='center', va='center', rotation=text_rot)
+
+    
+    def __find_onset(self, path, binding, fermi):
+        df = pd.read_csv(path, sep='\\s+', header=None, names=['energy', 'intensity1', 'intensity2', 'intensity3'])
+        onset = min(df.loc[df['intensity1']>0]['energy']) + (binding + fermi) * ryd_to_ev
+        return onset
+    
+
+    """
+    Load unbrodened spectra to determine core hole shift
+
+    Parameters
+    ----------
+    dir : str
+        Directory containing the spectra
+    GS_file : str
+        File containing the ground state XAS spectrum
+    ES_file : str
+        File containing the excited state XAS spectrum
+    GS_binding : float
+        Binding energy of the ground state
+    GS_fermi : float
+        Fermi energy of the ground state
+    ES_fermi : float
+        Fermi energy of the excited state
+    """
+    def load_unbroadend(self, dir, GS_file, ES_file, GS_binding, GS_fermi, ES_fermi):
+        self.gs_onsets.append(self.__find_onset(f'{dir}/{GS_file}', GS_binding, GS_fermi))
+        self.es_onsets.append(self.__find_onset(f'{dir}/{ES_file}', GS_binding, ES_fermi))
+
+    """
+    Calculate the core hole shift using all previously loaded unbrodened spectra
+
+    Returns
+    -------
+    float
+        Core hole shift
+    """
+    def calc_core_hole_shift(self):
+        return min(self.es_onsets) - min(self.gs_onsets)
+
+
```

### Comparing `xplotlib-0.0.2/src/XPlotLib/DOSAnalyzer.py` & `xplotlib-0.0.3/src/XPlotLib/DOSAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import numpy as np
 
 # from bokeh.plotting import figure, show
 # from bokeh.palettes import Colorblind8 as palette
 # from bokeh.models import CheckboxGroup, CustomJS
 # from bokeh.layouts import column, row
 import matplotlib.pyplot as plt
+from .XPlotLibUtils import ryd_to_ev
 
-Ryd = 13.605698066 # Rydberg energy to eV
 
 
 class DOSAnalyzer:
     def __init__(self):
         self.dos_dfs = []
         self.active_xes_dos = {}
         self.active_xas_dos = {}
@@ -171,20 +171,20 @@
             # add each column to list of possible active dos
             self.active_xes_dos.update({col: False for col in headers if col != 'ENERGY'})
             self.active_xas_dos.update({col: False for col in headers if col != 'ENERGY'})
 
         dos = self.__join_dos_dfs__(dos_parts)
 
         # convert rydberg to eV
-        dos['ENERGY'] = dos['ENERGY'] * Ryd
+        dos['ENERGY'] = dos['ENERGY'] * ryd_to_ev
 
         # shift energy to correct scale for each of the sites
         for site_name, binding_energy in binding_energies.items():
             site_dos = dos.filter(regex=f'{site_name}.*', axis=1)
-            site_dos.insert(loc=0, column='ENERGY', value=dos['ENERGY'] + binding_energy * Ryd)
+            site_dos.insert(loc=0, column='ENERGY', value=dos['ENERGY'] + binding_energy * ryd_to_ev)
             self.dos_dfs.append(site_dos)
 
     """
     Load DOS of the same atom from directory with given regex and name (this can include multiple files .dos1, .dos2, ...)
 
     Parameters
     ----------
@@ -218,18 +218,18 @@
             # add each column to list of possible active dos
             self.active_xes_dos.update({col: False for col in headers if col != 'ENERGY'})
             self.active_xas_dos.update({col: False for col in headers if col != 'ENERGY'})
 
         dos = self.__join_dos_dfs__(dos_parts)
 
         # convert rydberg to eV
-        dos['ENERGY'] = dos['ENERGY'] * Ryd
+        dos['ENERGY'] = dos['ENERGY'] * ryd_to_ev
 
         # shift energy to correct scale
-        dos['ENERGY'] = dos['ENERGY'] + binding_Energy * Ryd
+        dos['ENERGY'] = dos['ENERGY'] + binding_Energy * ryd_to_ev
         
 
         self.dos_dfs.append(dos)
 
     """
     Load XES or XAS spectrum from file
```

### Comparing `xplotlib-0.0.2/src/XPlotLib/XPlotLibUtils.py` & `xplotlib-0.0.3/src/XPlotLib/XPlotLibUtils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 
+ryd_to_ev = 13.605698066
+
 def non_uniform_savgol(x, y, window, polynom):
     """
     Applies a Savitzky-Golay filter to y with non-uniform spacing
     as defined in x
 
     This is based on https://dsp.stackexchange.com/questions/1676/savitzky-golay-smoothing-filter-for-not-equally-spaced-data
     The borders are interpolated like scipy.signal.savgol_filter would do
```

### Comparing `xplotlib-0.0.2/src/XPlotLib.egg-info/PKG-INFO` & `xplotlib-0.0.3/src/XPlotLib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

