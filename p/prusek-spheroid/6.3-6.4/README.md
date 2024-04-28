# Comparing `tmp/prusek_spheroid-6.3.tar.gz` & `tmp/prusek_spheroid-6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-6.3.tar", last modified: Tue Apr 16 10:01:36 2024, max compression
+gzip compressed data, was "prusek_spheroid-6.4.tar", last modified: Sun Apr 28 10:16:22 2024, max compression
```

## Comparing `prusek_spheroid-6.3.tar` & `prusek_spheroid-6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 10:01:36.958614 prusek_spheroid-6.3/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 10:01:36.958412 prusek_spheroid-6.3/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-6.3/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 10:01:36.957239 prusek_spheroid-6.3/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    18728 2024-04-16 10:01:30.000000 prusek_spheroid-6.3/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-6.3/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-6.3/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-6.3/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-6.3/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-6.3/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-6.3/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-6.3/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-6.3/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-6.3/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-6.3/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 10:01:36.958201 prusek_spheroid-6.3/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 10:01:36.000000 prusek_spheroid-6.3/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-16 10:01:36.000000 prusek_spheroid-6.3/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-16 10:01:36.000000 prusek_spheroid-6.3/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-16 10:01:36.000000 prusek_spheroid-6.3/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-16 10:01:36.000000 prusek_spheroid-6.3/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-16 10:01:36.958657 prusek_spheroid-6.3/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-16 10:01:35.000000 prusek_spheroid-6.3/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-28 10:16:22.810788 prusek_spheroid-6.4/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-28 10:16:22.810488 prusek_spheroid-6.4/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-6.4/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-28 10:16:22.809315 prusek_spheroid-6.4/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19023 2024-04-28 09:51:14.000000 prusek_spheroid-6.4/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-6.4/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-6.4/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5215 2024-04-28 09:57:13.000000 prusek_spheroid-6.4/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-6.4/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-6.4/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-6.4/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-6.4/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-6.4/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-6.4/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-6.4/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-28 10:16:22.810241 prusek_spheroid-6.4/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-28 10:16:22.000000 prusek_spheroid-6.4/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-28 10:16:22.000000 prusek_spheroid-6.4/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-28 10:16:22.000000 prusek_spheroid-6.4/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-28 10:16:22.000000 prusek_spheroid-6.4/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-28 10:16:22.000000 prusek_spheroid-6.4/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-28 10:16:22.810835 prusek_spheroid-6.4/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-28 10:16:19.000000 prusek_spheroid-6.4/setup.py
```

### Comparing `prusek_spheroid-6.3/PKG-INFO` & `prusek_spheroid-6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 6.3
+Version: 6.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-6.3/README.md` & `prusek_spheroid-6.4/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-6.4/prusek_spheroid/ContoursClassGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,22 @@
                     cv.line(img_with, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
                     if not cv.imwrite(
                             os.path.join(self.output_segmented_path, "results", filename.replace('.bmp', '.png')),
                             img_with):
                         print(
                             f"FAILED to save image: {os.path.join(self.output_segmented_path, 'results', filename.replace('.bmp', '.png'))}")
 
+                    if self.calculate_properties:
+                        contour_data = {
+                            'MaskName': os.path.basename(filename),
+                            'ContourOrder': 1
+                        }
+
+                        all_contour_data.append(contour_data)
+
                 else:
                     img_without = img.copy()
                     mask_without = np.zeros_like(img_gray)
                     mask_with = np.zeros_like(img_gray)
 
                     for contour in outer_contours:
                         contour = np.array(contour, dtype=np.int32)
```

### Comparing `prusek_spheroid-6.3/prusek_spheroid/GUI.py` & `prusek_spheroid-6.4/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-6.4/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-6.4/prusek_spheroid/characteristic_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -78,37 +78,55 @@
 
     # Určení ortogonálního průměru jako menší z dvou párů stran
     orthogonal_diameter = min(distances[0::2] + distances[1::2])
 
     return orthogonal_diameter
 
 def calculate_all(contour):
-    area = calculate_area_from_contour(contour)
-    perimeter = calculate_perimeter_from_contour(contour)
-    eq_diam = calculate_equivalent_diameter_from_contour(contour)
-    circularity = calculate_circularity_from_contour(contour)
-    feret_diameter_max, feret_diameter_min, feret_aspect_ratio = calculate_feret_properties_from_contour(contour)
-    feret_max_orthogonal_distance = calculate_orthogonal_diameter(contour)
-    major_axis_length, minor_axis_length = calculate_diameters_from_contour(contour)
-    compactness = calculate_compactness_from_contour(contour)
-    convexity = calculate_convexity_from_contour(contour)
-    solidity = calculate_solidity_from_contour(contour)
-    sphericity = calculate_sphericity_from_contour(contour)
+    if contour is not None:
+        area = calculate_area_from_contour(contour)
+        perimeter = calculate_perimeter_from_contour(contour)
+        eq_diam = calculate_equivalent_diameter_from_contour(contour)
+        circularity = calculate_circularity_from_contour(contour)
+        feret_diameter_max, feret_diameter_min, feret_aspect_ratio = calculate_feret_properties_from_contour(contour)
+        feret_max_orthogonal_distance = calculate_orthogonal_diameter(contour)
+        major_axis_length, minor_axis_length = calculate_diameters_from_contour(contour)
+        compactness = calculate_compactness_from_contour(contour)
+        convexity = calculate_convexity_from_contour(contour)
+        solidity = calculate_solidity_from_contour(contour)
+        sphericity = calculate_sphericity_from_contour(contour)
 
-    data = {
-        "Area": area,
-        "Perimeter": perimeter,
-        "EquivalentDiameter": eq_diam,
-        "Circularity": circularity,
-        "FeretDiameterMax": feret_diameter_max,
-        "FeretDiameterMaxOrthogonalDistance": feret_max_orthogonal_distance,
-        "FeretDiameterMin": feret_diameter_min,
-        "FeretAspectRatio": feret_aspect_ratio,
-        "LengthMajorDiameterThroughCentroid": major_axis_length,
-        "LengthMinorDiameterThroughCentroid": minor_axis_length,
-        "Compactness": compactness,
-        "Convexity": convexity,
-        "Solidity": solidity,
-        "Sphericity": sphericity
-    }
+        data = {
+            "Area": area,
+            "Perimeter": perimeter,
+            "EquivalentDiameter": eq_diam,
+            "Circularity": circularity,
+            "FeretDiameterMax": feret_diameter_max,
+            "FeretDiameterMaxOrthogonalDistance": feret_max_orthogonal_distance,
+            "FeretDiameterMin": feret_diameter_min,
+            "FeretAspectRatio": feret_aspect_ratio,
+            "LengthMajorDiameterThroughCentroid": major_axis_length,
+            "LengthMinorDiameterThroughCentroid": minor_axis_length,
+            "Compactness": compactness,
+            "Convexity": convexity,
+            "Solidity": solidity,
+            "Sphericity": sphericity
+        }
+    else:
+        data = {
+            "Area": "---",
+            "Perimeter": "---",
+            "EquivalentDiameter": "---",
+            "Circularity": "---",
+            "FeretDiameterMax": "---",
+            "FeretDiameterMaxOrthogonalDistance": "---",
+            "FeretDiameterMin": "---",
+            "FeretAspectRatio": "---",
+            "LengthMajorDiameterThroughCentroid": "---",
+            "LengthMinorDiameterThroughCentroid": "---",
+            "Compactness": "---",
+            "Convexity": "---",
+            "Solidity": "---",
+            "Sphericity": "---"
+        }
 
     return data
```

### Comparing `prusek_spheroid-6.3/prusek_spheroid/conversion.py` & `prusek_spheroid-6.4/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/file_management.py` & `prusek_spheroid-6.4/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/image_processing.py` & `prusek_spheroid-6.4/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/merge_directories.py` & `prusek_spheroid-6.4/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/methods.py` & `prusek_spheroid-6.4/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/metrics.py` & `prusek_spheroid-6.4/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-6.4/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-6.4/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 6.3
+Version: 6.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-6.3/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-6.4/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.3/setup.py` & `prusek_spheroid-6.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="6.3",
+    version="6.4",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

