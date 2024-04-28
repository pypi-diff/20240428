# Comparing `tmp/viirs-tools-0.1.0.tar.gz` & `tmp/viirs-tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viirs-tools-0.1.0.tar", last modified: Fri Apr 12 22:49:47 2024, max compression
+gzip compressed data, was "viirs-tools-0.1.1.tar", last modified: Sun Apr 28 20:00:43 2024, max compression
```

## Comparing `viirs-tools-0.1.0.tar` & `viirs-tools-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/
--rw-r--r--   0 andmin    (1000) users      (984)    11358 2024-04-12 22:48:16.000000 viirs-tools-0.1.0/LICENSE
--rw-r--r--   0 andmin    (1000) users      (984)    17178 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)     3589 2024-04-12 22:29:57.000000 viirs-tools-0.1.0/README.md
--rw-r--r--   0 andmin    (1000) users      (984)       38 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/setup.cfg
--rw-r--r--   0 andmin    (1000) users      (984)      927 2024-04-12 22:46:13.000000 viirs-tools-0.1.0/setup.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools/
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools/Assimilator/
--rw-r--r--   0 andmin    (1000) users      (984)     4362 2024-04-12 18:39:53.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/Assimilator.py
--rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/Reading.py
--rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/ReadingHelpers.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/__init__.py
--rw-r--r--   0 andmin    (1000) users      (984)     7759 2024-04-12 22:02:41.000000 viirs-tools-0.1.0/viirs_tools/CloudMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     3683 2024-04-12 21:14:32.000000 viirs-tools-0.1.0/viirs_tools/NightMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     2672 2024-04-12 21:19:10.000000 viirs-tools-0.1.0/viirs_tools/Utils.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-0.1.0/viirs_tools/__init__.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools.egg-info/
--rw-r--r--   0 andmin    (1000) users      (984)    17178 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)      447 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 andmin    (1000) users      (984)        1 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 andmin    (1000) users      (984)       30 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/requires.txt
--rw-r--r--   0 andmin    (1000) users      (984)       12 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/
+-rw-r--r--   0 andmin    (1000) users      (984)    11358 2024-04-12 22:48:16.000000 viirs-tools-0.1.1/LICENSE
+-rw-r--r--   0 andmin    (1000) users      (984)    17191 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)     3591 2024-04-16 16:53:39.000000 viirs-tools-0.1.1/README.md
+-rw-r--r--   0 andmin    (1000) users      (984)       38 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/setup.cfg
+-rw-r--r--   0 andmin    (1000) users      (984)      939 2024-04-28 17:06:20.000000 viirs-tools-0.1.1/setup.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.786798 viirs-tools-0.1.1/viirs_tools/
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.787798 viirs-tools-0.1.1/viirs_tools/Assimilator/
+-rw-r--r--   0 andmin    (1000) users      (984)     4351 2024-04-19 22:01:45.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/Assimilator.py
+-rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/Reading.py
+-rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/ReadingHelpers.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/__init__.py
+-rw-r--r--   0 andmin    (1000) users      (984)     8664 2024-04-28 17:05:50.000000 viirs-tools-0.1.1/viirs_tools/CloudMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     3683 2024-04-12 21:14:32.000000 viirs-tools-0.1.1/viirs_tools/NightMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     3159 2024-04-28 16:41:06.000000 viirs-tools-0.1.1/viirs_tools/Utils.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-0.1.1/viirs_tools/__init__.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.787798 viirs-tools-0.1.1/viirs_tools.egg-info/
+-rw-r--r--   0 andmin    (1000) users      (984)    17191 2024-04-28 20:00:42.000000 viirs-tools-0.1.1/viirs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)      447 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 andmin    (1000) users      (984)        1 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       30 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/requires.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       12 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/top_level.txt
```

### Comparing `viirs-tools-0.1.0/LICENSE` & `viirs-tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.0/PKG-INFO` & `viirs-tools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viirs-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for processing VIIRS data
 Home-page: https://github.com/Veon2479/viirs-tools
 Author: Andrey Shuliak
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -206,15 +206,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Keywords: viirs,satellite,remote sensing,meteorology
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray
 Provides-Extra: assimilator
 Requires-Dist: netcdf4; extra == "assimilator"
 
@@ -232,29 +232,29 @@
 ## Installation
 
 To install `viirs-tools`, you can use pip:
 ```
  pip install viirs-tools 
 ```
 
-If you want to use the `Assimilation` extra module, which allows you to download data from NASA servers:
+If you want to use the `Assimilator` extra module, which allows you to download data from NASA servers:
 ``` 
 pip install viirs-tools[assimilator]
  ```
 Note that this module functions rely on the [cmrfetch](https://github.com/bmflynn/cmrfetch) package, you need to install and configure it first.
 
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
    + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + day_night_img: Day/night cloud mask based on the previous 2
+   + `day_night_img`: Day/night cloud mask based on the previous 2
 
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
 3. **Utils**:
    - Just some helpful functions
```

### Comparing `viirs-tools-0.1.0/README.md` & `viirs-tools-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 ## Installation
 
 To install `viirs-tools`, you can use pip:
 ```
  pip install viirs-tools 
 ```
 
-If you want to use the `Assimilation` extra module, which allows you to download data from NASA servers:
+If you want to use the `Assimilator` extra module, which allows you to download data from NASA servers:
 ``` 
 pip install viirs-tools[assimilator]
  ```
 Note that this module functions rely on the [cmrfetch](https://github.com/bmflynn/cmrfetch) package, you need to install and configure it first.
 
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
    + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + day_night_img: Day/night cloud mask based on the previous 2
+   + `day_night_img`: Day/night cloud mask based on the previous 2
 
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
 3. **Utils**:
    - Just some helpful functions
@@ -49,8 +49,8 @@
 	3. **ReadingHelpers**
 		- Contains some helper functions for reading files that aren't supported by `SatPy` module (some examples of using them in the previous module)
 
 
 ## References
 [^1]: M.Piper, T.Bahr (2015). A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS.
 
-[^2]: W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014). The New VIIRS 375 m active fire detection data product: Algorithm description and initial assessment.
+[^2]: W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014). The New VIIRS 375 m active fire detection data product: Algorithm description and initial assessment.
```

### Comparing `viirs-tools-0.1.0/setup.py` & `viirs-tools-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     name='viirs-tools',
     description='Python library for processing VIIRS data',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/Veon2479/viirs-tools',
     license=license_text,
     author='Andrey Shuliak',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'xarray',
     ],
     extras_require={
         'assimilator': ['netcdf4']
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: Apache Software License',
         'Topic :: Scientific/Engineering :: Atmospheric Science'
     ],
     keywords=['viirs', 'satellite', 'remote sensing', 'meteorology'],
 
 )
```

### Comparing `viirs-tools-0.1.0/viirs_tools/Assimilator/Assimilator.py` & `viirs-tools-0.1.1/viirs_tools/Assimilator/Assimilator.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     with ProcessPoolExecutor(max_workers=workers) as executor:
         futures = []
         cur_d = end_d
         next_d = end_d + timedelta(days=1)
         while (cur_d >= start_d):
             cur_d_s = cur_d.strftime('%Y-%m-%d')
             next_d_s = next_d.strftime('%Y-%m-%d')
-            step_path = os.path.join(path, f'{cur_d_s}_{next_d_s}')
+            step_path = os.path.join(path, f'{cur_d_s}')
 
             _get_data_for_interval(
                 step_path,
                 cur_d_s, next_d_s,
                 names,
                 geobox,
                 dconc
```

### Comparing `viirs-tools-0.1.0/viirs_tools/Assimilator/Reading.py` & `viirs-tools-0.1.1/viirs_tools/Assimilator/Reading.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.0/viirs_tools/Assimilator/ReadingHelpers.py` & `viirs-tools-0.1.1/viirs_tools/Assimilator/ReadingHelpers.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.0/viirs_tools/CloudMask.py` & `viirs-tools-0.1.1/viirs_tools/CloudMask.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,15 +47,48 @@
     cm = xr.where(cm & t6, 0, 1)
 
     cm = xr.where(nmask == 0, cm, math.nan)
 
     return cm
 
 
-def _thermal_img(bi4, bi5, nmask):
+def _fire_day_img(ri1, ri2, bi5, nmask):
+    """
+        Day reflectance & termal I-bands cloud test
+        Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
+        The New VIIRS 375 m active fire detection data product:
+            Algorithm description and initial assessment
+    Args:
+        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
+        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
+        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+    Returns:
+        (list|np.ndarray|xr.Dataset): integer cloud mask,
+            0 is cloud, 1 is clear pixel
+            Can contain NaN values
+    """
+    cm = xr.where(bi5 < 265, 0, 1)
+
+    sum_ri = ri1 + ri2
+
+    t2 = xr.where(sum_ri > 90, 0, 1)
+    t2 = xr.where(bi5 < 295, t2, 1)
+
+    t3 = xr.where(sum_ri > 70, 0, 1)
+    t3 = xr.where(bi5 < 285, t2, 1)
+
+    cm = xr.where(t2 == 0, 0, cm)
+    cm = xr.where(t3 == 0, 0, cm)
+
+    cm = xr.where(nmask == 0, cm, math.nan)
+    return cm
+
+
+def _fire_night_img(bi4, bi5, nmask):
     """
         Night termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
         bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
@@ -105,61 +138,54 @@
     return _rsnpp_day_img(
         ri1, ri2, ri3,
         bi4, bi5,
         nmask
     )
 
 
-def thermal_img(bi4, bi5, nmask):
+def fire_day_img(ri1, ri2, bi5, nmask):
     """
-        Night termal I-bands cloud test
+        Day reflectance & termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
+        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
         bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
         nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
     Returns:
         (list|np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
-    Utils._check_data(bi4)
+    Utils._check_data(ri1)
+    Utils._check_data(ri2)
     Utils._check_data(bi5)
-    return _thermal_img(bi4, bi5, nmask)
+    return _fire_day_img(ri1, ri2, bi5, nmask)
 
 
-def day_night_img(ri1, ri2, ri3, bi4, bi5, nmask):
+def fire_night_img(bi4, bi5, nmask):
     """
-        Wrapper for getting cloud mask for any time
-        using RSNPP and thermal cloud masks algs
+        Night termal I-bands cloud test
+        Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
+        The New VIIRS 375 m active fire detection data product:
+            Algorithm description and initial assessment
     Args:
-        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
-        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
-        ri3 (list|np.ndarray|xr.Dataset): I03 in reflectance calibration
         bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
         bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
         nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
     Returns:
         (list|np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
-    Utils._check_data(ri1)
-    Utils._check_data(ri2)
-    Utils._check_data(ri3)
     Utils._check_data(bi4)
     Utils._check_data(bi5)
-    Utils._check_data(nmask)
-
-    dcm = _rsnpp_day_img(ri1, ri2, ri3, bi4, bi5, nmask)
-    ncm = _thermal_img(bi4, bi5, nmask)
-
-    return xr.where(nmask, ncm, dcm)
+    return _fire_night_img(bi4, bi5, nmask)
 
 
 # Public xr.Dataset wrappers:
 
 
 def rsnpp_day_img_ds(ds, nmask):
     """
@@ -189,61 +215,56 @@
         ds['I03'],
         ds['I04'],
         ds['I05'],
         nmask
     )
 
 
-def thermal_img_ds(ds, nmask):
+def fire_day_img_ds(ds, nmask):
     """
-        Wrapper for Night termal I-bands cloud test for xr.Dataset
+        Wrapper for Day reflectance & termal I-bands cloud test for xr.Dataset
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        ds (xr.Dataset): dataset with I01-I05 bands data
+        ds (xr.Dataset): dataset with I01, I02, I05 bands data
         nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
     Returns:
         (xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     if not isinstance(ds, xr.Dataset):
         raise ValueError(
             "Incorrect input data format"
         )
-    return thermal_img(
-        ds['I04'],
+    return fire_day_img(
+        ds['I01'],
+        ds['I02'],
         ds['I05'],
         nmask
     )
 
 
-def day_night_img_ds(ds, nmask):
+def fire_night_img_ds(ds, nmask):
     """
-        Wrapper for getting cloud mask for any time
-        using RSNPP and thermal cloud masks algs
-        from xr.Dataset object
+        Wrapper for Night termal I-bands cloud test for xr.Dataset
+        Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
+        The New VIIRS 375 m active fire detection data product:
+            Algorithm description and initial assessment
     Args:
-        ds (xr.Dataset): dataset with I01-I05 bands data
+        ds (xr.Dataset): dataset with I04, I05 bands data
         nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
     Returns:
         (xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     if not isinstance(ds, xr.Dataset):
         raise ValueError(
             "Incorrect input data format"
         )
-    if not isinstance(nmask, xr.DataArray):
-        raise ValueError(
-            "Incorrect input data format"
-        )
-    return day_night_img(
-        ds['I01'],
-        ds['I02'],
-        ds['I03'],
+    return fire_night_img(
         ds['I04'],
         ds['I05'],
         nmask
     )
```

### Comparing `viirs-tools-0.1.0/viirs_tools/NightMask.py` & `viirs-tools-0.1.1/viirs_tools/NightMask.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.0/viirs_tools/Utils.py` & `viirs-tools-0.1.1/viirs_tools/Utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import xarray as xr
 import numpy as np
+import math
 
 # Internal functions:
 
 
 def _check_data(data):
     """
         Check object for being of appropriate type
@@ -96,7 +97,25 @@
         return np.logical_not(np.isnan(data))
     elif isinstance(data, (xr.DataArray, xr.Dataset)):
         return data.notnull()
     else:
         raise ValueError(
             "Input data is not array (built-in, np or xr) object"
         )
+
+
+def merge_masks(day_cm, night_cm, nm):
+    """
+        Merge day and night cloud masks
+    Args:
+        day_cm(list|np.ndarray|xr.DataArray):
+            day cloud mask
+        night_cm(list|np.ndarray|xr.DataArray):
+            night cloud mask
+        nm(list|np.ndarray|xr.DataArray):
+            binary night mask
+    Returns:
+        (list|np.ndarray|xr.DataArray):
+            merged cloud mask
+    """
+    mask = xr.where(nm == 0, day_cm, night_cm)
+    return mask
```

### Comparing `viirs-tools-0.1.0/viirs_tools.egg-info/PKG-INFO` & `viirs-tools-0.1.1/viirs_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viirs-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for processing VIIRS data
 Home-page: https://github.com/Veon2479/viirs-tools
 Author: Andrey Shuliak
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -206,15 +206,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Keywords: viirs,satellite,remote sensing,meteorology
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray
 Provides-Extra: assimilator
 Requires-Dist: netcdf4; extra == "assimilator"
 
@@ -232,29 +232,29 @@
 ## Installation
 
 To install `viirs-tools`, you can use pip:
 ```
  pip install viirs-tools 
 ```
 
-If you want to use the `Assimilation` extra module, which allows you to download data from NASA servers:
+If you want to use the `Assimilator` extra module, which allows you to download data from NASA servers:
 ``` 
 pip install viirs-tools[assimilator]
  ```
 Note that this module functions rely on the [cmrfetch](https://github.com/bmflynn/cmrfetch) package, you need to install and configure it first.
 
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
    + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + day_night_img: Day/night cloud mask based on the previous 2
+   + `day_night_img`: Day/night cloud mask based on the previous 2
 
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
 3. **Utils**:
    - Just some helpful functions
```

