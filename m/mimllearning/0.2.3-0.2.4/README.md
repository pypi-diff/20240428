# Comparing `tmp/mimllearning-0.2.3.tar.gz` & `tmp/mimllearning-0.2.4.tar.gz`

## Comparing `mimllearning-0.2.3.tar` & `mimllearning-0.2.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.3/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.3/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/instance.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/tutorial/demo_MIML.ipynb
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/tutorial/tests.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.3/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.3/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.3/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.4/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.4/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/demo_MIML.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/tests.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.4/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.4/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.4/PKG-INFO
```

### Comparing `mimllearning-0.2.3/readme.md` & `mimllearning-0.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.4/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/classifier/miml_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         ----------
         x_train : np.ndarray
             Features values of bags in the training set.
         y_train : np.ndarray
             Labels of bags in the training set.
         """
         self.generate_apr(x_train, y_train)
-        print(self.apr)
 
     def predict(self, bag: np.array) -> int:
         """
         Predict the label of the bag
 
         Parameters
         ----------
```

### Comparing `mimllearning-0.2.3/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         ----------
         x_train
         y_train
         """
         self.x_train = x_train
         self.y_train = y_train
         self.generate_apr()
-        for _ in range(3):
-            self.grow()
-            print("APR ID: ", self.apr)
+        #for _ in range(3):
+        self.grow()
+        #    self.discriminate()
 
     def predict_bag(self, bag):
         """
 
         Parameters
         ----------
         bag
@@ -95,15 +95,43 @@
                 apr = (apr_min, apr_max)
                 new_aprs.append(apr)
                 new_aprs_size.append(self.size(apr))
 
         # actualizamos nuestro apr
         self.apr = new_aprs[new_aprs_size.index(min(new_aprs_size))]
 
-    def discriminate(self):
-        pass
+    def discriminate(self, margin=0.1):
+        selected_features = []
+        negative_bag_indices = np.where(self.y_train == 0)[0]
+        while negative_bag_indices:
+            discrimination_counts = np.zeros(self.x_train.shape[1])
+
+            for bag_index in negative_bag_indices:
+                for instance in self.x_train[bag_index]:
+                    for feature_index in range(self.x_train.shape[1]):
+                        if (instance[feature_index] < self.apr[0][feature_index] - margin or
+                                instance[feature_index] > self.apr[1][feature_index] + margin):
+                            discrimination_counts[feature_index] += 1
+
+            if not np.any(discrimination_counts):
+                break
+
+            max_discrimination_feature = np.argmax(discrimination_counts)
+            selected_features.append(max_discrimination_feature)
+
+            # Remove instances strongly discriminated by the selected feature
+            new_negative_instances_indices = []
+            for bag_index in negative_bag_indices:
+                for instance in self.x_train[bag_index]:
+                    if (instance[max_discrimination_feature] < self.apr[0][max_discrimination_feature] - margin or
+                            instance[max_discrimination_feature] > self.apr[1][max_discrimination_feature] + margin):
+                        pass
+                        #new_negative_instances_indices.append(instance_index)
+            negative_instances_indices = new_negative_instances_indices
+
+        return selected_features
 
     def size(self, apr):
         size = 0
         for i in range(self.apr[0].shape[0]):
             size += apr[1][i] - apr[0][i]
         return size
```

### Comparing `mimllearning-0.2.3/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/data/arff_to_csv.py` & `mimllearning-0.2.4/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/data/bag.py` & `mimllearning-0.2.4/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/data/instance.py` & `mimllearning-0.2.4/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/data/load_datasets.py` & `mimllearning-0.2.4/src/miml/data/load_datasets.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/data/miml_dataset.py` & `mimllearning-0.2.4/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.4/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.4/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.4/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.4/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/test/data_test.py` & `mimllearning-0.2.4/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.2.4/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.2.4/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.2.4/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/tutorial/classifiers_tutorial.py` & `mimllearning-0.2.4/src/miml/tutorial/classifiers_tutorial.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/tutorial/demo_MIML.ipynb` & `mimllearning-0.2.4/src/miml/tutorial/demo_MIML.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/src/miml/tutorial/tests.py` & `mimllearning-0.2.4/src/miml/tutorial/tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,10 +5,12 @@
 from miml.transformation import ArithmeticTransformation
 
 dataset_train = load_dataset("../datasets/miml_birds_random_80train.arff", delimiter="'")
 dataset_test = load_dataset("../datasets/miml_birds_random_20test.arff", delimiter="'")
 
 classifier_mi = MIMLtoMIBRClassifier(AllPositiveAPRClassifier())
 classifier_mi.fit(dataset_train)
+classifier_mi.evaluate(dataset_test)
 
 classifier_mi = MIMLtoMIBRClassifier(IteratedDiscrimAPRClassifier())
 classifier_mi.fit(dataset_train)
+classifier_mi.evaluate(dataset_test)
```

### Comparing `mimllearning-0.2.3/README.md` & `mimllearning-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.3/pyproject.toml` & `mimllearning-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.3"
+version = "0.2.4"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.3/PKG-INFO` & `mimllearning-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.3
+Version: 0.2.4
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

