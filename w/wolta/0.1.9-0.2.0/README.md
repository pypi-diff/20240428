# Comparing `tmp/wolta-0.1.9.tar.gz` & `tmp/wolta-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.9.tar", last modified: Thu Apr 11 11:06:16 2024, max compression
+gzip compressed data, was "wolta-0.2.0.tar", last modified: Sat Apr 27 23:19:11 2024, max compression
```

## Comparing `wolta-0.1.9.tar` & `wolta-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.837572 wolta-0.1.9/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0    17575 2024-04-11 11:06:16.836547 wolta-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    16268 2024-04-10 00:49:00.000000 wolta-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 11:06:16.837572 wolta-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-04-11 11:06:12.000000 wolta-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.796640 wolta-0.1.9/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.9/wolta/__init__.py
--rw-rw-rw-   0        0        0    11388 2024-04-11 11:06:12.000000 wolta-0.1.9/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.9/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.9/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.9/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.835392 wolta-0.1.9/wolta.egg-info/
--rw-rw-rw-   0        0        0    17575 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 23:19:11.711461 wolta-0.2.0/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    20060 2024-04-27 23:19:11.710462 wolta-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18630 2024-04-27 23:19:00.000000 wolta-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 23:19:11.711461 wolta-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2024-04-27 23:10:01.000000 wolta-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 23:19:11.667423 wolta-0.2.0/wolta/
+-rw-rw-rw-   0        0        0      115 2024-04-27 21:13:06.000000 wolta-0.2.0/wolta/__init__.py
+-rw-rw-rw-   0        0        0    12216 2024-04-27 19:19:42.000000 wolta-0.2.0/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.2.0/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    32432 2024-04-27 21:58:26.000000 wolta-0.2.0/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.2.0/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-27 23:19:11.709462 wolta-0.2.0/wolta.egg-info/
+-rw-rw-rw-   0        0        0    20060 2024-04-27 23:19:11.000000 wolta-0.2.0/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-27 23:19:11.000000 wolta-0.2.0/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 23:19:11.000000 wolta-0.2.0/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-27 23:19:11.000000 wolta-0.2.0/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-27 23:19:11.000000 wolta-0.2.0/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.9/LICENSE.txt` & `wolta-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.9/PKG-INFO` & `wolta-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.9
+Version: 0.2.0
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE.txt
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: hyperopt
 Requires-Dist: catboost
 Requires-Dist: imblearn
+Requires-Dist: lightgbm
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
 Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
@@ -109,14 +110,37 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### make_null
+
+**Returns**: pandas dataframe or numpy array
+
+**Parameters**:
+
+* matrix (pandas dataframe or numpy array)
+* replace, string, the text which will converted to null
+* type, {'df', 'np'}, by default 'df'
+
+***
+
+### seek_null
+
+**Returns**: boolean
+
+**Parameters**:
+
+* df, pandas dataframe
+* print_columns, boolean, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
@@ -317,29 +341,54 @@
 
 **Parameters**:
 
 * y_test, _1D numpy array_
 * y_pred, _1D numpy array_
 * metrics, _list of string_, this list can only have values the table below:
 
+For 'clf':
+
 | value | full name      |
 | --- |----------------|
 | acc | accuracy score |
 | f1 | f1 score       |
 | hamming | hamming loss   |
 | jaccard | jaccard score |
 | log | log loss |
 | mcc | matthews corrcoef |
 | precision | precision score |
 | recall | recall score |
 | zol | zero one loss |
 
 by default, ['acc']
+<br>
+
+For 'reg':
+
+| value   | full name                          |
+|---------|------------------------------------|
+| var     | explained variance                 |
+| max     | max error                          |
+| abs     | neg mean absolute error            |
+| sq      | neg mean squared error             |
+| rsq     | neg root mean squared error        |
+| log     | neg mean squared log error         |
+| rlog    | neg mean squared log error         |
+| medabs  | neg median absolute error          |
+| poisson | neg mean poisson deviance          |
+| gamma   | neg mean gamma deviance            |
+| per     | neg mean absolute percentage error |
+| d2abs   | d2 absolute error score            |
+| d2pin   | d2 pinball score                   |
+| d2twe   | d2 tweedie score                   |
+
+by default, ['sq']
 
 * average, string, {'weighted', 'micro', 'macro', 'binary', 'samples'}, by default, 'weighted'
+* algo_type, {'clf', 'reg'}, 'clf' by default
 
 ```python
 import numpy as np
 from wolta.model_tools import get_score
 
 y_test = np.load('test.npy')
 y_pred = np.load('pred.npy')
@@ -369,14 +418,64 @@
 from wolta.model_tools import get_avg_options
 
 print(get_avg_options())
 ```
 
 ***
 
+### compare_models
+
+**Returns**: nothing, just prints out the results
+
+**Parameters**:
+
+* algo_type, {'clf', 'reg'}
+* algorithms, list of string, if the first element is 'all' then it gets results for every algorithm.
+
+for 'clf':
+
+| value | full name |
+|-------|-----------|
+| cat   | catboost  |
+| ada | adaboost  |
+| dtr | decision tree |
+| raf | random forest |
+| lbm | lightgbm |
+| ext | extra tree |
+| log | logistic regression |
+| knn | knn |
+| gnb | gaussian nb |
+| rdg | ridge |
+| bnb | bernoulli nb |
+| svc | svc |
+| per | perceptron |
+| mnb | multinomial nb |
+
+for 'reg':
+
+| value | full name         |
+|-------|-------------------|
+| cat   | catboost          |
+| ada   | adaboost          |
+| dtr   | decision tree     |
+| raf   | random forest     |
+| lbm   | lightgbm          |
+| ext   | extra tree        |
+| lin   | linear regression |
+| knn   | knn               |
+| svr   | svr               |
+
+* metrics, list of string, its values must be acceptable for get_score method
+* X_train
+* y_train
+* X_test
+* y_test
+
+***
+
 ### do_combinations
 
 **Returns**: list of the int lists
 
 **Parameters**:
 * indexes, _list of int_
 * min_item, _int_, it is the minimum amount of index inside a combination
```

### Comparing `wolta-0.1.9/README.md` & `wolta-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -86,14 +86,37 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### make_null
+
+**Returns**: pandas dataframe or numpy array
+
+**Parameters**:
+
+* matrix (pandas dataframe or numpy array)
+* replace, string, the text which will converted to null
+* type, {'df', 'np'}, by default 'df'
+
+***
+
+### seek_null
+
+**Returns**: boolean
+
+**Parameters**:
+
+* df, pandas dataframe
+* print_columns, boolean, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
@@ -294,29 +317,54 @@
 
 **Parameters**:
 
 * y_test, _1D numpy array_
 * y_pred, _1D numpy array_
 * metrics, _list of string_, this list can only have values the table below:
 
+For 'clf':
+
 | value | full name      |
 | --- |----------------|
 | acc | accuracy score |
 | f1 | f1 score       |
 | hamming | hamming loss   |
 | jaccard | jaccard score |
 | log | log loss |
 | mcc | matthews corrcoef |
 | precision | precision score |
 | recall | recall score |
 | zol | zero one loss |
 
 by default, ['acc']
+<br>
+
+For 'reg':
+
+| value   | full name                          |
+|---------|------------------------------------|
+| var     | explained variance                 |
+| max     | max error                          |
+| abs     | neg mean absolute error            |
+| sq      | neg mean squared error             |
+| rsq     | neg root mean squared error        |
+| log     | neg mean squared log error         |
+| rlog    | neg mean squared log error         |
+| medabs  | neg median absolute error          |
+| poisson | neg mean poisson deviance          |
+| gamma   | neg mean gamma deviance            |
+| per     | neg mean absolute percentage error |
+| d2abs   | d2 absolute error score            |
+| d2pin   | d2 pinball score                   |
+| d2twe   | d2 tweedie score                   |
+
+by default, ['sq']
 
 * average, string, {'weighted', 'micro', 'macro', 'binary', 'samples'}, by default, 'weighted'
+* algo_type, {'clf', 'reg'}, 'clf' by default
 
 ```python
 import numpy as np
 from wolta.model_tools import get_score
 
 y_test = np.load('test.npy')
 y_pred = np.load('pred.npy')
@@ -346,14 +394,64 @@
 from wolta.model_tools import get_avg_options
 
 print(get_avg_options())
 ```
 
 ***
 
+### compare_models
+
+**Returns**: nothing, just prints out the results
+
+**Parameters**:
+
+* algo_type, {'clf', 'reg'}
+* algorithms, list of string, if the first element is 'all' then it gets results for every algorithm.
+
+for 'clf':
+
+| value | full name |
+|-------|-----------|
+| cat   | catboost  |
+| ada | adaboost  |
+| dtr | decision tree |
+| raf | random forest |
+| lbm | lightgbm |
+| ext | extra tree |
+| log | logistic regression |
+| knn | knn |
+| gnb | gaussian nb |
+| rdg | ridge |
+| bnb | bernoulli nb |
+| svc | svc |
+| per | perceptron |
+| mnb | multinomial nb |
+
+for 'reg':
+
+| value | full name         |
+|-------|-------------------|
+| cat   | catboost          |
+| ada   | adaboost          |
+| dtr   | decision tree     |
+| raf   | random forest     |
+| lbm   | lightgbm          |
+| ext   | extra tree        |
+| lin   | linear regression |
+| knn   | knn               |
+| svr   | svr               |
+
+* metrics, list of string, its values must be acceptable for get_score method
+* X_train
+* y_train
+* X_test
+* y_test
+
+***
+
 ### do_combinations
 
 **Returns**: list of the int lists
 
 **Parameters**:
 * indexes, _list of int_
 * min_item, _int_, it is the minimum amount of index inside a combination
```

### Comparing `wolta-0.1.9/setup.py` & `wolta-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
     author_email="<sadikefe69@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['scikit-learn', 'pandas', 'numpy', 'hyperopt', 'catboost', 'imblearn'],
+    install_requires=['scikit-learn', 'pandas', 'numpy', 'hyperopt', 'catboost', 'imblearn', 'lightgbm'],
     keywords=['python', 'machine', 'learning', 'machine learning', 'data science', 'data'],
     py_modules=['data_tools', 'model_tools', 'progressive_tools', 'feature_tools'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

### Comparing `wolta-0.1.9/wolta/data_tools.py` & `wolta-0.2.0/wolta/data_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -448,7 +448,38 @@
     border_one = mean - std
     border_two = mean + std
 
     if amin >= border_one or amax <= border_two:
         return False
     else:
         return True
+
+
+def seek_null(df, print_columns=False):
+    null_columns = []
+
+    for col in df.columns:
+        if df[col].isna().sum() > 0:
+            null_columns.append(col)
+
+            if print_columns:
+                print('{} has {} null values'.format(col, str(df[col].isna().sum())))
+
+    return null_columns
+
+
+def make_null(matrix, replace, type='df'):
+    if type == 'df':
+        for i in range(matrix.shape[1]):
+            for j in range(matrix.shape[0]):
+                if matrix.iloc[j, i] == replace:
+                    matrix.iloc[j, i] = None
+
+        return matrix
+
+    elif type == 'np':
+        for i in range(matrix.shape[1]):
+            for j in range(matrix.shape[0]):
+                if matrix[j, i] == replace:
+                    matrix.iloc[j, i] = None
+
+        return matrix
```

### Comparing `wolta-0.1.9/wolta/feature_tools.py` & `wolta-0.2.0/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.9/wolta/progressive_tools.py` & `wolta-0.2.0/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.9/wolta.egg-info/PKG-INFO` & `wolta-0.2.0/wolta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.9
+Version: 0.2.0
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE.txt
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: hyperopt
 Requires-Dist: catboost
 Requires-Dist: imblearn
+Requires-Dist: lightgbm
 
 
 # WOLTA DOCUMENTATION
 
 Wolta is designed for making simplify the frequently used processes which includes Pandas, Numpy and Scikit-Learn in Machine Learning.
 <br><br>
 Currently there are four modules inside the library, which are 'data_tools', 'model_tools', 'progressive_tools' and 'feature_tools'
@@ -109,14 +110,37 @@
 
 df = pd.read_csv('data.csv')
 df['output'] = make_numerics(df['output'])
 ```
 
 ***
 
+### make_null
+
+**Returns**: pandas dataframe or numpy array
+
+**Parameters**:
+
+* matrix (pandas dataframe or numpy array)
+* replace, string, the text which will converted to null
+* type, {'df', 'np'}, by default 'df'
+
+***
+
+### seek_null
+
+**Returns**: boolean
+
+**Parameters**:
+
+* df, pandas dataframe
+* print_columns, boolean, False by default
+
+***
+
 ### transform_data
 
 **Returns**:
 1. transformed X
 2. transformed y
 3. if strategy ends with 'm', amin_x
 4. if strategy ends with 'm', amin_y
@@ -317,29 +341,54 @@
 
 **Parameters**:
 
 * y_test, _1D numpy array_
 * y_pred, _1D numpy array_
 * metrics, _list of string_, this list can only have values the table below:
 
+For 'clf':
+
 | value | full name      |
 | --- |----------------|
 | acc | accuracy score |
 | f1 | f1 score       |
 | hamming | hamming loss   |
 | jaccard | jaccard score |
 | log | log loss |
 | mcc | matthews corrcoef |
 | precision | precision score |
 | recall | recall score |
 | zol | zero one loss |
 
 by default, ['acc']
+<br>
+
+For 'reg':
+
+| value   | full name                          |
+|---------|------------------------------------|
+| var     | explained variance                 |
+| max     | max error                          |
+| abs     | neg mean absolute error            |
+| sq      | neg mean squared error             |
+| rsq     | neg root mean squared error        |
+| log     | neg mean squared log error         |
+| rlog    | neg mean squared log error         |
+| medabs  | neg median absolute error          |
+| poisson | neg mean poisson deviance          |
+| gamma   | neg mean gamma deviance            |
+| per     | neg mean absolute percentage error |
+| d2abs   | d2 absolute error score            |
+| d2pin   | d2 pinball score                   |
+| d2twe   | d2 tweedie score                   |
+
+by default, ['sq']
 
 * average, string, {'weighted', 'micro', 'macro', 'binary', 'samples'}, by default, 'weighted'
+* algo_type, {'clf', 'reg'}, 'clf' by default
 
 ```python
 import numpy as np
 from wolta.model_tools import get_score
 
 y_test = np.load('test.npy')
 y_pred = np.load('pred.npy')
@@ -369,14 +418,64 @@
 from wolta.model_tools import get_avg_options
 
 print(get_avg_options())
 ```
 
 ***
 
+### compare_models
+
+**Returns**: nothing, just prints out the results
+
+**Parameters**:
+
+* algo_type, {'clf', 'reg'}
+* algorithms, list of string, if the first element is 'all' then it gets results for every algorithm.
+
+for 'clf':
+
+| value | full name |
+|-------|-----------|
+| cat   | catboost  |
+| ada | adaboost  |
+| dtr | decision tree |
+| raf | random forest |
+| lbm | lightgbm |
+| ext | extra tree |
+| log | logistic regression |
+| knn | knn |
+| gnb | gaussian nb |
+| rdg | ridge |
+| bnb | bernoulli nb |
+| svc | svc |
+| per | perceptron |
+| mnb | multinomial nb |
+
+for 'reg':
+
+| value | full name         |
+|-------|-------------------|
+| cat   | catboost          |
+| ada   | adaboost          |
+| dtr   | decision tree     |
+| raf   | random forest     |
+| lbm   | lightgbm          |
+| ext   | extra tree        |
+| lin   | linear regression |
+| knn   | knn               |
+| svr   | svr               |
+
+* metrics, list of string, its values must be acceptable for get_score method
+* X_train
+* y_train
+* X_test
+* y_test
+
+***
+
 ### do_combinations
 
 **Returns**: list of the int lists
 
 **Parameters**:
 * indexes, _list of int_
 * min_item, _int_, it is the minimum amount of index inside a combination
```

