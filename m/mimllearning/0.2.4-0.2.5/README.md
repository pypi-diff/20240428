# Comparing `tmp/mimllearning-0.2.4.tar.gz` & `tmp/mimllearning-0.2.5.tar.gz`

## Comparing `mimllearning-0.2.4.tar` & `mimllearning-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.4/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.4/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/instance.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/demo_MIML.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/tests.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.4/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.4/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.5/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.5/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/tutorial/demo_MIML.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/tutorial/tests.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.5/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.5/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.5/PKG-INFO
```

### Comparing `mimllearning-0.2.4/readme.md` & `mimllearning-0.2.5/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.5/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/miml_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,23 +24,27 @@
         self.x_train = x_train
         self.y_train = y_train
         self.generate_apr()
         #for _ in range(3):
         self.grow()
         #    self.discriminate()
 
-    def predict_bag(self, bag):
+    def predict(self, bag: np.array) -> int:
         """
+        Predict the label of the bag
 
         Parameters
         ----------
-        bag
+        bag: np.ndarray of shape(n_instances, n_features)
+            features values of a bag
 
         Returns
         -------
+        label: int
+            Predicted label of the bag
 
         """
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
```

### Comparing `mimllearning-0.2.4/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/data/arff_to_csv.py` & `mimllearning-0.2.5/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/data/bag.py` & `mimllearning-0.2.5/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/data/instance.py` & `mimllearning-0.2.5/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/data/load_datasets.py` & `mimllearning-0.2.5/src/miml/data/load_datasets.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/data/miml_dataset.py` & `mimllearning-0.2.5/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.5/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.5/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.5/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.5/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/test/data_test.py` & `mimllearning-0.2.5/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.2.5/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.2.5/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.2.5/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/tutorial/classifiers_tutorial.py` & `mimllearning-0.2.5/src/miml/tutorial/classifiers_tutorial.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/tutorial/demo_MIML.ipynb` & `mimllearning-0.2.5/src/miml/tutorial/demo_MIML.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/src/miml/tutorial/tests.py` & `mimllearning-0.2.5/src/miml/tutorial/tests.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/README.md` & `mimllearning-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.4/pyproject.toml` & `mimllearning-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.4"
+version = "0.2.5"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.4/PKG-INFO` & `mimllearning-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.4
+Version: 0.2.5
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

