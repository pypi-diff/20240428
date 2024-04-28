# Comparing `tmp/pyhasura-1.0.8.tar.gz` & `tmp/pyhasura-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.8.tar", last modified: Fri Apr 26 02:44:55 2024, max compression
+gzip compressed data, was "pyhasura-1.0.9.tar", last modified: Fri Apr 26 14:10:38 2024, max compression
```

## Comparing `pyhasura-1.0.8.tar` & `pyhasura-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.340172 pyhasura-1.0.8/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.8/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:44:55.339960 pyhasura-1.0.8/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.8/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.339155 pyhasura-1.0.8/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.8/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.8/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.8/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    14675 2024-04-26 02:44:41.000000 pyhasura-1.0.8/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.339721 pyhasura-1.0.8/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.8/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-26 02:44:55.340212 pyhasura-1.0.8/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.8/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 14:10:38.057595 pyhasura-1.0.9/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.9/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 14:10:38.057397 pyhasura-1.0.9/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.9/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 14:10:38.056241 pyhasura-1.0.9/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.9/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.9/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.9/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    14766 2024-04-26 13:32:02.000000 pyhasura-1.0.9/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 14:10:38.057126 pyhasura-1.0.9/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 14:10:38.000000 pyhasura-1.0.9/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-26 14:10:38.000000 pyhasura-1.0.9/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-26 14:10:38.000000 pyhasura-1.0.9/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-26 14:10:38.000000 pyhasura-1.0.9/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-26 14:10:38.000000 pyhasura-1.0.9/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.9/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-26 14:10:38.057653 pyhasura-1.0.9/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.9/setup.py
```

### Comparing `pyhasura-1.0.8/LICENSE` & `pyhasura-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.8/PKG-INFO` & `pyhasura-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.8/README.md` & `pyhasura-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.8/pyhasura/flatten_dict.py` & `pyhasura-1.0.9/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.8/pyhasura/hasura_client.py` & `pyhasura-1.0.9/pyhasura/hasura_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,14 @@
     DATAFRAME = 2
     ARROW = 3
     NATURAL = 4
     PARQUET = 5
     CSV = 6
 
 
-def load_data_from_base64(base64_string):
-    # Decode the base64 string to bytes
-    binary_data = base64.b64decode(base64_string)
-
-    # Create a temporary file in memory
-    with tempfile.NamedTemporaryFile(delete=False) as temp_file:
-        temp_file.write(binary_data)
-        return temp_file.name
-
-
 def create_empty_arrays(n):
     return [[] for _ in range(n)]
 
 
 def compute_deltas(numbers):
     """
     Computes the deltas (differences) between consecutive elements in an array of numbers.
@@ -140,16 +130,18 @@
         return flatten_result
 
     def _transform_to_arrow(self):
         flatten_result = {key: pa.Table.from_pandas(pd.DataFrame(flatten_nested_dicts(val))) for key, val in
                           self.native_result.items()}
         return flatten_result
 
-    def execute(self, query, variables=None, output_format=ExportFormat.NATURAL):
-        self.native_result = self.client.execute(gql(query), variables)
+    def execute(self, query, variables=None, output_format=ExportFormat.NATURAL, operation_name=None):
+        op = gql(query)
+        operation_name = operation_name if operation_name is not None else op.definitions[0].name.value
+        self.native_result = self.client.execute(gql(query), variables, operation_name=operation_name)
         self.result = self.native_result
         return self.convert_output_format(output_format)
 
     def _get_file_path(self, extension):
         return os.path.join(self.output_dir, extension)
 
     @staticmethod
@@ -227,15 +219,15 @@
             for k in range(lower, upper + 1):
                 kmedoids = KMedoids(n_clusters=min(k, len(self.vectorized_result[key]) - 1), random_state=42)
                 kmedoids.fit(self.vectorized_result[key])
                 costs.append(kmedoids.inertia_)
             clustered[key] = get_ordinal_of_smallest_number(compute_deltas(costs)) + 2
         return clustered
 
-    def anomalies_training(self, output_dir=None):
+    def anomalies_training(self, output_dir=None, base64_encoded_data=False):
         """
         Train anomaly detection models and save them to the specified output directory.
 
         :param output_dir: Optional. The directory to save the trained models. If not specified, the models will be saved in the current working directory.
         :type output_dir: str
 
         :return: A dictionary containing the filenames of the saved models, with keys as the model names.
@@ -244,18 +236,22 @@
         if output_dir is not None:
             self.output_dir = output_dir
         self.vectorize_result()
         clf = IsolationForest(contamination=0.1, random_state=42)
         filenames = {}
         for key in self.vectorized_result:
             clf.fit(self.vectorized_result[key])
-            filename = os.path.join(self.output_dir, key + '.pkl')
-            with open(filename, 'wb') as model_file:
-                pickle.dump(clf, model_file)
-            filenames[key] = filename
+            temp_dir = tempfile.mkdtemp()
+            filename = os.path.join(self.output_dir, temp_dir, key + '.pkl')
+            if base64_encoded_data:
+                filenames[key] = base64.b64encode(pickle.dumps(clf))
+            else:
+                with open(filename, 'wb') as model_file:
+                    pickle.dump(clf, model_file)
+                    filenames[key] = filename
         return filenames
 
     def anomalies(self, training_files=None, threshold=0, training_base64=None):
         """
         Args:
             training_files: A dictionary containing the file paths of the training files for each key. If provided, the pre-trained isolation forest models will be loaded from these files.
             threshold: A float value representing the threshold for anomaly detection. Only the anomalies with a score below this threshold will be included in the result. Defaults to 0 if not provided.
```

### Comparing `pyhasura-1.0.8/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.9/pyhasura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.8/pyproject.toml` & `pyhasura-1.0.9/pyproject.toml`

 * *Files identical despite different names*

