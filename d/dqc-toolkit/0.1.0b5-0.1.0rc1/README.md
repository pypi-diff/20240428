# Comparing `tmp/dqc_toolkit-0.1.0b5.tar.gz` & `tmp/dqc_toolkit-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc_toolkit-0.1.0b5.tar", last modified: Mon Apr 15 18:10:56 2024, max compression
+gzip compressed data, was "dqc_toolkit-0.1.0rc1.tar", last modified: Tue Apr 23 18:03:43 2024, max compression
```

## Comparing `dqc_toolkit-0.1.0b5.tar` & `dqc_toolkit-0.1.0rc1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 18:10:56.802258 dqc_toolkit-0.1.0b5/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b5/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 18:10:56.800966 dqc_toolkit-0.1.0b5/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b5/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 18:10:56.779702 dqc_toolkit-0.1.0b5/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc_toolkit-0.1.0b5/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)    14962 2024-04-15 17:44:18.000000 dqc_toolkit-0.1.0b5/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 18:10:56.789097 dqc_toolkit-0.1.0b5/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      329 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7254 2024-04-15 17:48:40.000000 dqc_toolkit-0.1.0b5/dqc/utils/_curation.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/dqc/utils/_dataprocessing.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4680 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/dqc/utils/_sanitychecks.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/dqc/utils/logging.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 18:10:56.797291 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 18:10:56.000000 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      431 2024-04-15 18:10:56.000000 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-15 18:10:56.000000 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-15 18:10:56.000000 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-15 18:10:56.000000 dqc_toolkit-0.1.0b5/dqc_toolkit.egg-info/top_level.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1659 2024-04-15 18:09:08.000000 dqc_toolkit-0.1.0b5/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-15 18:10:56.802419 dqc_toolkit-0.1.0b5/setup.cfg
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 18:10:56.796200 dqc_toolkit-0.1.0b5/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc_toolkit-0.1.0b5/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b5/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6124 2024-04-15 17:52:51.000000 dqc_toolkit-0.1.0b5/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.355005 dqc_toolkit-0.1.0rc1/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4693 2024-04-23 18:03:43.354399 dqc_toolkit-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1652 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.334724 dqc_toolkit-0.1.0rc1/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      115 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    15192 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.343010 dqc_toolkit-0.1.0rc1/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      353 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7220 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_curation.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3117 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_sanitychecks.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/logging.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1943 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/noise_utils.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      635 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/version.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.351783 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4693 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      471 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1684 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-23 18:03:43.355143 dqc_toolkit-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.350078 dqc_toolkit-0.1.0rc1/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6342 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/test_crossval.py
```

### Comparing `dqc_toolkit-0.1.0b5/LICENSE` & `dqc_toolkit-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b5/dqc/base.py` & `dqc_toolkit-0.1.0rc1/dqc/base.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b5/dqc/crossval.py` & `dqc_toolkit-0.1.0rc1/dqc/crossval.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 tqdm.pandas()
 
 
 class CrossValCurate(BaseCurate):
     """
     Args:
         curate_feature_extractor (Union[str, TfidfVectorizer, CountVectorizer, SentenceTransformer], optional): Feature extraction method to be used during curation. Accepts string values 'TfidfVectorizer', 'CountVectorizer' which map to `sklearn.feature_extraction.text.TfidfVectorizer` and `sklearn.feature_extraction.text.CountVectorizer` objects respectively. Also accepts explicit instances of `sklearn.feature_extraction.text.TfidfVectorizer` / `sklearn.feature_extraction.text.CountVectorizer`.  Additionally, supports `SentenceTransformer` model object or a string matching the name of a `SentenceTransformer` model hosted on HuggingFace Model Hub. Defaults to 'TfidfVectorizer'.
-        curate_model (str, optional): Machine learning model that is trained with `curate_feature_extractor` features during curation. Accepts any instance of scikit-learn classifier that implement `predict_proba()' method. Defaults to `sklearn.linear_model.LogisticRegression`.
-        calibration_method (Union[str, None], optional): Approach to be used for calibration of `curate_model` predictions. Defaults to None.
+        curate_model (str, optional): Machine learning model that is trained with `curate_feature_extractor` based features during curation. Accepts any instance of scikit-learn classifier that implement `predict_proba()` method. Defaults to `sklearn.linear_model.LogisticRegression`.
+        calibration_method (Union[str, None], optional): Approach to be used for calibration of `curate_model` predictions. Defaults to 'calibrate_using_baseline'.
         correctness_threshold (float, optional): Minimum prediction probability using `curate_model` to consider the corresponding sample as 'correctly labelled'. Defaults to 0.5.
         n_splits (int, optional): Number of splits to use when running cross-validation based curation.
         verbose (bool, optional): Sets the verbosity level during execution. `True` indicates logging level INFO and `False` indicates logging level 'ERROR'.
 
     Examples:
     Assuming `data` is a pandas dataframe containing samples with noisy labels, here is how you would use `CrossValCurate` -
     ```python
@@ -258,17 +258,18 @@
         Args:
             data_with_noisy_labels (pd.DataFrame): Input data with corresponding noisy labels
             X_col_name (str): Column to be used to extract input features.
             y_col_name (str): Label column in the data.
         Returns:
 
             pd.DataFrame: Input Data samples with \n
-                1) Corresponding predicted_labels using CrossValCurate \n
-                2) Prediction probabilities \n
-                3) An indicator variable `is_label_correct` capturing label correctness
+                1) 'predicted_label' - Predicted labels using CrossValCurate \n
+                2) 'prediction_probability' - Corresponding prediction probabilities \n
+                3) 'label_correctness_score' - Label correctness scores based on prediction probabilities \n
+                4) 'is_label_correct' - An indicator variable (True / False) classifying samples as correctly / incorrectly labelled.
         """
         _is_valid(data_with_noisy_labels, X_col_name, y_col_name)
         n_splits = self.n_splits
         options["num_samples"] = len(data_with_noisy_labels)
 
         # TBD
         # 'max_features': min(options["num_samples"] // 10, options.get("max_features", 1000))
```

### Comparing `dqc_toolkit-0.1.0b5/dqc/utils/_curation.py` & `dqc_toolkit-0.1.0rc1/dqc/utils/_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,13 +182,13 @@
         n_splits (int, optional): The number of splits. Defaults to 5.
 
     Returns:
         StratifiedKFold: Currently, a StratifiedKFold object.
     """
 
     if strategy == "stratified_kfold":
-        cv = StratifiedKFold(n_splits=n_splits, shuffle=False, random_state=None)
+        cv = StratifiedKFold(n_splits=n_splits)
         return cv.split(df[X_col_name], df[y_col_name_int])
 
     raise ValueError(
         f"Data splitting strategy {strategy} not supported. Please use `strategy='stratified_kfold'`"
     )
```

### Comparing `dqc_toolkit-0.1.0b5/dqc/utils/_dataprocessing.py` & `dqc_toolkit-0.1.0rc1/dqc/utils/_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b5/dqc/utils/logging.py` & `dqc_toolkit-0.1.0rc1/dqc/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0b5/pyproject.toml` & `dqc_toolkit-0.1.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dqc-toolkit"
-version = "0.1.0-beta5"
+version = "0.1.0-rc1"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -51,17 +51,17 @@
   "pytest>=8.1.1",
 	"mkdocs==1.5.3",
 	"mkdocs-material==9.5.17",
 	"mkdocstrings[python]==0.24.3",
 	"mkdocstrings-crystal==0.3.7"
 ]
 [project.urls]
-Homepage = "https://github.com/sumanthprabhu/C2"
-Source = "https://github.com/sumanthprabhu/C2"
-Tracker = "https://github.com/sumanthprabhu/C2/issues"
+Homepage = "https://github.com/sumanthprabhu/DQC-Toolkit"
+Source = "https://github.com/sumanthprabhu/DQC-Toolkit"
+Tracker = "https://github.com/sumanthprabhu/DQC-Toolkit/issues"
 
 [tool.setuptools.packages.find]
 exclude=["notebooks", "docs"]
 
 [tool.ruff]
 lint.ignore = [
     "F401",  # Ignore 'unused import' error
```

### Comparing `dqc_toolkit-0.1.0b5/tests/test_crossval.py` & `dqc_toolkit-0.1.0rc1/tests/test_crossval.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import StratifiedKFold
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 
+import dqc
 from dqc import CrossValCurate
 from dqc.utils import add_asymmetric_noise
 
 sio = StringIO()
 
 
 def sample_dataframe_for_stratified_split(
@@ -217,13 +218,20 @@
     cvc = CrossValCurate(calibration_method=calibration_method, verbose=verbose)
     data = cvc.fit_transform(data)
 
 
 @pytest.mark.parametrize("noise_prob", [0.1])
 @pytest.mark.parametrize("random_state", [None, 1])
 def test_add_asymmetric_noise(data, noise_prob, random_state):
-    noisy_labels = add_asymmetric_noise(
+    noisy_labels, observed_noise_ratio = add_asymmetric_noise(
         data["label"], noise_prob=noise_prob, random_state=random_state
     )
 
-    assert isinstance(noisy_labels, pd.Series)
+    assert isinstance(noisy_labels, pd.Series) and isinstance(
+        observed_noise_ratio, float
+    )
     assert len(noisy_labels) == len(data["label"])
+
+
+def test_show_versions():
+    dqc_info = dqc.show_versions()
+    assert type(dqc_info) == dict and len(dqc_info.keys()) == 7
```

