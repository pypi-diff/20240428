# Comparing `tmp/mimllearning-0.2.1.tar.gz` & `tmp/mimllearning-0.2.2.tar.gz`

## Comparing `mimllearning-0.2.1.tar` & `mimllearning-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.2.1/.gitattributes
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.1/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.1/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.2.1/documentation/Formato datos tfg.png
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/instance.py
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.1/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.1/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.2/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.2/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/tutorial/demo_MIML.ipynb
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/tutorial/tests.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.2/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.2/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.2/PKG-INFO
```

### Comparing `mimllearning-0.2.1/readme.md` & `mimllearning-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.2/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/classifier/miml_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         x_train
         y_train
         """
         self.x_train = x_train
         self.y_train = y_train
         self.generate_apr()
         self.grow()
+        print(self.apr)
 
     def predict_bag(self, bag):
         """
 
         Parameters
         ----------
         bag
@@ -67,30 +68,40 @@
 
     def grow(self):
 
         not_positives_bag_in_apr = []
 
         for bag_index in self.positive_bag_indices:
             for instance in self.x_train[bag_index]:
-                if not np.all(instance >= self.apr[0]) or not np.all(instance <= self.apr[1]):
-                    not_positives_bag_in_apr.append(bag_index)
+                if np.all(instance >= self.apr[0]) and np.all(instance <= self.apr[1]):
+                    # There is already an instance of the bag in apr
+                    break
+            else:
+                # If any instance in apr we need to get one of the bag
+                not_positives_bag_in_apr.append(bag_index)
+
+        if not not_positives_bag_in_apr:
+            return
 
         # calculate new apr with not_positive_bag_in_apr and compare size
         new_aprs = []
         new_aprs_size = []
-        apr_min, apr_max = None, None
+
         for bag_index in not_positives_bag_in_apr:
             for instance in self.x_train[bag_index]:
                 apr_min = np.minimum(self.apr[0], instance)
                 apr_max = np.maximum(self.apr[1], instance)
-            apr = (apr_min, apr_max)
-            new_aprs.append(apr)
-            new_aprs_size.append(self.size(apr))
+                apr = (apr_min, apr_max)
+                new_aprs.append(apr)
+                new_aprs_size.append(self.size(apr))
 
         # actualizamos nuestro apr
-        self.apr = new_aprs[new_aprs_size.index(max(new_aprs_size))]
+        self.apr = new_aprs[new_aprs_size.index(min(new_aprs_size))]
+
+    def discriminate(self):
+        pass
 
     def size(self, apr):
         size = 0
         for i in range(self.apr[0].shape[0]):
             size += apr[1][i] - apr[0][i]
         return size
```

### Comparing `mimllearning-0.2.1/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         return self.predict(bags[0][0])
 
     def evaluate(self, dataset_test: MIMLDataset):
         """
 
         Parameters
         ----------
-        dataset_test
+        dataset_test: MIMLDataset
+            Dataset to test the classifier
         """
         super().evaluate(dataset_test)
 
         datasets = self.transformation.transform_dataset(dataset_test)
 
         results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
         for i, bag in enumerate(datasets[0][0]):
```

### Comparing `mimllearning-0.2.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/data/arff_to_csv.py` & `mimllearning-0.2.2/src/miml/data/arff_to_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-def arff_to_csv(file, delimiter="'"):
+def arff_to_csv(file: str, delimiter: str = "'") -> None:
     """
     Convert MIML Arff to CSV.
 
     Parameters
     ----------
-    file : string
+    file : str
         Filepath of the file to be converted
 
-    delimiter : string ( ' or " ), default = '
-        Delimiter used in arff file for the start and end of the bag values
+    delimiter : str, default = '
+        Delimiter used in arff file for the start and end of the bag values ( ' or " )
 
     """
 
     arff = open(file)
     csv = open(file[:-5] + ".csv", "w")
     attrib = []
     flag = 0
```

### Comparing `mimllearning-0.2.1/src/miml/data/bag.py` & `mimllearning-0.2.2/src/miml/data/bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
     def set_attribute(self, instance: int, attribute, value: float) -> None:
         """
         Update value from attributes
 
         Parameters
         ----------
-        instance : string
+        instance : int
             Index of instance to be updated
 
         attribute: int/str
             Attribute name/index_instance of the bag to be updated
 
         value: float
             New value for the update
```

### Comparing `mimllearning-0.2.1/src/miml/data/instance.py` & `mimllearning-0.2.2/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/data/load_datasets.py` & `mimllearning-0.2.2/src/miml/data/load_datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 import os
 
 from .bag import Bag
 from .instance import Instance
 from .miml_dataset import MIMLDataset
 
 
-def load_dataset(file, delimiter="\""):
+def load_dataset(file: str, delimiter: str = "\"") -> MIMLDataset:
     """
     Function to load a dataset
 
     Parameters
     ----------
-
     file : str
         Path of the dataset file
     delimiter : str
         Character to separate instances in bag of the arff files
+
+    Returns
+    ----------
+    dataset : MIMLDataset
+        Dataset loaded
     """
     if file[-4:] == ".csv":
         return load_dataset_csv(file)
     elif file[-5:] == ".arff":
         return load_dataset_arff(file, delimiter)
     else:
         print("Error")
         # TODO: Control de errores
 
 
-def load_dataset_csv(file, header=0):
+def load_dataset_csv(file: str, header=0):
     """
     Function to load a dataset in csv format
 
     Parameters
     ----------
     file : str
         Path of the dataset file
@@ -77,24 +81,29 @@
             bag = Bag(key)
             dataset.add_bag(bag)
         dataset.add_instance(key, instance)
 
     return dataset
 
 
-def load_dataset_arff(file, delimiter="\""):
+def load_dataset_arff(file: str, delimiter: str = "\"") -> MIMLDataset:
     """
     Function to load a dataset in arff format
 
     Parameters
     ----------
     file : str
         Path of the dataset file
     delimiter : str
         Delimiter of instances in a bag in the arff file
+
+    Returns
+    -------
+    dataset : MIMLDataset
+        Dataset loaded
     """
     dataset = MIMLDataset()
     arff_file = open(file)
     features_name = []
     labels_name = []
     flag = 0
     for line in arff_file:
```

### Comparing `mimllearning-0.2.1/src/miml/data/miml_dataset.py` & `mimllearning-0.2.2/src/miml/data/miml_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         Parameters
         ----------
         key_bag : str
             Key of the bag which contains the instance to be deleted
         """
         self.data.pop(key_bag)
 
-    def get_instance(self, key_bag, index_instance):
+    def get_instance(self, key_bag, index_instance) -> Instance:
         """
         Get an Instance of the dataset
 
         Parameters
         ----------
         key_bag : str
             Key of the bag
@@ -279,15 +279,15 @@
         -------
         instance : Instance
             Instance of Instance class
         """
         # TODO: check
         return self.get_bag(key_bag).get_instance(index_instance)
 
-    def get_number_instances(self):
+    def get_number_instances(self) -> int:
         """
         Get numbers of instances of the dataset
 
         Returns
         ----------
         numbers of instances: int
             Numbers of instances of the dataset
@@ -317,15 +317,15 @@
             Key of the bag which contains the instance to be deleted
 
         index_instance : int
             Index of the instance to be deleted
         """
         self.get_bag(key_bag).delete_instance(index_instance)
 
-    def get_attribute(self, bag, instance, attribute):
+    def get_attribute(self, bag, instance, attribute) -> float:
         """
         Get value of an attribute of the bag
 
         Parameters
         ----------
         bag : str
             Key of the bag which contains the attribute
@@ -337,39 +337,39 @@
             Index/Name of the attribute
 
         Returns
         -------
         value : float
             Value of the attribute
         """
-        self.get_instance(bag, instance).get_attribute(attribute)
+        return self.get_instance(bag, instance).get_attribute(attribute)
 
-    def set_attribute(self, key_bag, index_instance, attribute, value):
+    def set_attribute(self, key_bag: str, index_instance: int, attribute, value: float) -> None:
         """
         Update value from attributes
 
             Parameters
             ----------
-            key_bag : string
+            key_bag : str
                 Bag key of the dataset
 
             index_instance : int
                 Index of the instance
 
             attribute: int/str
                 Attribute of the dataset
 
             value: float
                 New value for the update
             """
         self.get_instance(key_bag, index_instance).set_attribute(attribute, value)
 
-    def add_attribute(self, position, values=None):
+    def add_attribute(self, position: int, values=None) -> None:
         """
-        Add attribute to the bag
+        Add attribute to the dataset
 
         Parameters
         ----------
         position : int
             Index for the new attribute
 
         values:  numpy array
@@ -378,34 +378,43 @@
         # TODO: Test
         for bag_index, bag in enumerate(self.data.keys()):
             add_values = values[bag_index]
             if values is None:
                 add_values = np.zeros(self.data[bag].get_number_instances)
             self.data[bag].add_attribute(position, add_values)
 
-    def delete_attribute(self, position):
+    def delete_attribute(self, position: int) -> None:
+
+        """
+        Delete attribute of the dataset
+
+        Parameters
+        ----------
+        position : int
+            Index of the attribute to be deleted
+        """
+
         for bag in self.data.keys():
             self.data[bag].delete_attribute(position)
 
-    def show_dataset(self, head=None, attributes=None, labels=None):
+    def show_dataset(self, head: int = None, attributes=None, labels=None) -> None:
         """
         Function to show information about the dataset
 
         Parameters
         ----------
             head : int
                 Number of the nth firsts bag to show
 
             attributes: List of string
                 Attributes to show
 
             labels : List of string
                 Labels to show
         """
-        # TODO: Formatearlo para que se vea bonito
         # TODO: Hacer algo como head y tail de pandas, ponerlo como parametro quizas, tambien lista atributos y labels
         #  a mostrar opcionales
         print("Name: ", self.get_name())
         print("Features: ", self.get_features_name())
         print("Labels: ", self.get_labels_name())
         print("Bags:")
         count = 0
```

### Comparing `mimllearning-0.2.1/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.2/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.2/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.2/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.2/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/test/data_test.py` & `mimllearning-0.2.2/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.2.2/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.2.2/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.2.2/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/src/miml/tutorial/classifiers_tutorial.py` & `mimllearning-0.2.2/src/miml/tutorial/classifiers_tutorial.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/README.md` & `mimllearning-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.1/pyproject.toml` & `mimllearning-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.1"
+version = "0.2.2"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.1/PKG-INFO` & `mimllearning-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.1
+Version: 0.2.2
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

