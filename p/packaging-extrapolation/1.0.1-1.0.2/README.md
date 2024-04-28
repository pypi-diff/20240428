# Comparing `tmp/packaging_extrapolation-1.0.1.tar.gz` & `tmp/packaging-extrapolation-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\my_work\????\py_work\new\packaging_extrapolation\dist\.tmp-4_9st7o4\packaging_extrapolation-1.0.1.tar", last modified: Fri Feb 16 04:58:20 2024, max compression
+gzip compressed data, was "F:\my_work\????\py_work\new\packaging_extrapolation\dist\.tmp-8hvgvgem\packaging-extrapolation-1.0.2.tar", last modified: Sun Apr 28 13:14:53 2024, max compression
```

## Comparing `packaging_extrapolation-1.0.1.tar` & `packaging-extrapolation-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/
--rw-rw-rw-   0        0        0     1090 2023-05-30 02:26:11.000000 packaging_extrapolation-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     8534 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6722 2024-02-16 04:55:33.000000 packaging_extrapolation-1.0.1/README.md
--rw-rw-rw-   0        0        0      873 2024-02-16 04:58:01.000000 packaging_extrapolation-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-10-14 14:27:21.000000 packaging_extrapolation-1.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation/
--rw-rw-rw-   0        0        0     8760 2024-01-13 14:10:05.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation/Extrapolation.py
--rw-rw-rw-   0        0        0    11175 2024-02-07 12:50:15.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation/UtilLog.py
--rw-rw-rw-   0        0        0    10845 2024-02-16 04:52:37.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation/UtilTools.py
--rw-rw-rw-   0        0        0        0 2023-10-15 13:34:55.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/
--rw-rw-rw-   0        0        0     8534 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-02-16 04:58:20.000000 packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-30 02:26:11.000000 packaging-extrapolation-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9564 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7752 2024-02-20 12:43:12.000000 packaging-extrapolation-1.0.2/README.md
+-rw-rw-rw-   0        0        0      873 2024-04-28 13:14:38.000000 packaging-extrapolation-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-10-14 14:27:21.000000 packaging-extrapolation-1.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation/
+-rw-rw-rw-   0        0        0     8760 2024-01-13 14:10:05.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation/Extrapolation.py
+-rw-rw-rw-   0        0        0    11175 2024-02-07 12:50:15.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation/UtilLog.py
+-rw-rw-rw-   0        0        0    12401 2024-04-28 13:08:45.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation/UtilTools.py
+-rw-rw-rw-   0        0        0        0 2023-10-15 13:34:55.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/
+-rw-rw-rw-   0        0        0     9564 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 13:14:53.000000 packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/top_level.txt
```

### Comparing `packaging_extrapolation-1.0.1/LICENSE` & `packaging-extrapolation-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `packaging_extrapolation-1.0.1/PKG-INFO` & `packaging-extrapolation-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: packaging_extrapolation
-Version: 1.0.1
+Name: packaging-extrapolation
+Version: 1.0.2
 Summary: Extrapolation methods for complete basis sets
 Author-email: ZHAOKAI XI <xizaokaiz@foxmail.com>
 License: MIT License
         
         Copyright (c) [2023] [ZhaoKai Xi]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 
 ## About
 
 * This package contains partial extrapolation methods in quantum chemistry, written using the extrapolation method proposed in the literature. Extrapolation to the CBS limit can be done by entering two successive energies.
 
 ## Quickly Use
 
-* Please use the `pip` command to install: `pip install packaging_extrapolation` or `python3 -m pip install packaging_extrapolation`
+* Please use the `pip` command to install: `pip install packaging-extrapolation` or `python3 -m pip install packaging-extrapolation`
 * Please make sure the package is the latest: `pip install --upgrade packaging_extrapolation`
 * After installation, test the example in `src/packaging_extrapolation/examples/examples_energy.py` to see if you get results.
   * Extrapolation Method Calls: `python  examples_energy.py -m "Klopper_1986" -xe -76.0411795 -ye -76.0603284 -low 2 -high 3 -a 4.25`
   * `-m`: extrapolation method name.
   * `-xe`: energy for E(X).
   * `-ye`: energy for E(Y).
   * `-low`: cardinal number for X.
@@ -126,21 +126,21 @@
 NH2,-55.5749363,-55.5878344
 NH3,-56.1972947,-56.2127423
 NO2,-204.0664514,-204.1137363
 ```
 
 
 
-| Functions                                                    |
-| ------------------------------------------------------------ |
-| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol). |
-| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy. |
-| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files. |
-| `train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
+| Functions                                                                                                                                                                                       |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol).                                                                                                         |
+| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol).                                                                                                     |
+| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol).                                                                                                           |
+| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol).                                                                                                |
+| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy.                                                            |
+| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files.                                                                                                       |
+| `UtilLog.train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
```

### Comparing `packaging_extrapolation-1.0.1/README.md` & `packaging-extrapolation-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## About
 
 * This package contains partial extrapolation methods in quantum chemistry, written using the extrapolation method proposed in the literature. Extrapolation to the CBS limit can be done by entering two successive energies.
 
 ## Quickly Use
 
-* Please use the `pip` command to install: `pip install packaging_extrapolation` or `python3 -m pip install packaging_extrapolation`
+* Please use the `pip` command to install: `pip install packaging-extrapolation` or `python3 -m pip install packaging-extrapolation`
 * Please make sure the package is the latest: `pip install --upgrade packaging_extrapolation`
 * After installation, test the example in `src/packaging_extrapolation/examples/examples_energy.py` to see if you get results.
   * Extrapolation Method Calls: `python  examples_energy.py -m "Klopper_1986" -xe -76.0411795 -ye -76.0603284 -low 2 -high 3 -a 4.25`
   * `-m`: extrapolation method name.
   * `-xe`: energy for E(X).
   * `-ye`: energy for E(Y).
   * `-low`: cardinal number for X.
@@ -91,21 +91,21 @@
 NH2,-55.5749363,-55.5878344
 NH3,-56.1972947,-56.2127423
 NO2,-204.0664514,-204.1137363
 ```
 
 
 
-| Functions                                                    |
-| ------------------------------------------------------------ |
-| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol). |
-| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy. |
-| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files. |
-| `train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
+| Functions                                                                                                                                                                                       |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol).                                                                                                         |
+| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol).                                                                                                     |
+| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol).                                                                                                           |
+| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol).                                                                                                |
+| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy.                                                            |
+| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files.                                                                                                       |
+| `UtilLog.train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
```

### Comparing `packaging_extrapolation-1.0.1/pyproject.toml` & `packaging-extrapolation-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
-name = "packaging_extrapolation"
+name = "packaging-extrapolation"
 authors = [
     {name = "ZHAOKAI XI", email = "xizaokaiz@foxmail.com"},
 ]
 description = "Extrapolation methods for complete basis sets"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
     "numpy","pandas","scipy","scikit-learn","matplotlib"
 ]
 keywords = ["basis set","extrapolation","quantum chemistry"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `packaging_extrapolation-1.0.1/src/packaging_extrapolation/Extrapolation.py` & `packaging-extrapolation-1.0.2/src/packaging_extrapolation/Extrapolation.py`

 * *Files identical despite different names*

### Comparing `packaging_extrapolation-1.0.1/src/packaging_extrapolation/UtilLog.py` & `packaging-extrapolation-1.0.2/src/packaging_extrapolation/UtilLog.py`

 * *Files identical despite different names*

### Comparing `packaging_extrapolation-1.0.1/src/packaging_extrapolation/UtilTools.py` & `packaging-extrapolation-1.0.2/src/packaging_extrapolation/UtilTools.py`

 * *Files 12% similar despite different names*

```diff
@@ -341,7 +341,59 @@
     result = least_squares(loss_model, x0=init_guess,
                            args=(model, x_energy_list, y_energy_list,
                                  limit_list, temp))
     # result = minimize(loss_model, x0=init_guess,
     #                   args=(model, x_energy_list, y_energy_list,
     #                         limit_list, temp), bounds=[(1, 10)], constraints=constraints)
     return result.x[0]
+
+# 训练函数，返回能量和alpha列表
+def train(model, *, method, x_energy_list, y_energy_list, limit_list=None, init_guess=0.001, level='dt', tolerance=1e-6):
+    # 默认需要拟合参数，默认需要拟合
+    flag = True
+    if limit_list is None:
+        flag = False
+    energy_list = []
+    alpha_list = []
+    if is_series(x_energy_list):
+        x_energy_list = to_list(x_energy_list)
+    if is_series(y_energy_list):
+        y_energy_list = to_list(y_energy_list)
+    if is_series(limit_list):
+        limit_list = to_list(limit_list)
+
+    # 判断基数
+    if level == 'dt':
+        low_card = 2
+        high_card = 3
+    elif level == 'tq':
+        low_card = 3
+        high_card = 4
+    elif level == 'q5':
+        low_card = 4
+        high_card = 5
+    else:
+        raise ValueError('Invalid level name')
+    model.update_method(method)
+    model.update_card(low_card, high_card)
+
+    for i in range(len(x_energy_list)):
+        x_energy = x_energy_list[i]
+        y_energy = y_energy_list[i]
+
+        # 更新能量
+        model.update_energy(x_energy, y_energy)
+
+        # 为ture，则拟合
+        if flag:
+            limit = limit_list[i]
+            alpha = opt_alpha(model.loss_function, limit, init_guess, tolerance)
+            alpha_list.append(alpha)
+            energy = calc_energy(model, alpha)
+
+        else:
+            energy = calc_energy(model)
+
+        energy_list.append(energy)
+    if flag:
+        return energy_list, alpha_list
+    return energy_list
```

### Comparing `packaging_extrapolation-1.0.1/src/packaging_extrapolation.egg-info/PKG-INFO` & `packaging-extrapolation-1.0.2/src/packaging_extrapolation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-extrapolation
-Version: 1.0.1
+Version: 1.0.2
 Summary: Extrapolation methods for complete basis sets
 Author-email: ZHAOKAI XI <xizaokaiz@foxmail.com>
 License: MIT License
         
         Copyright (c) [2023] [ZhaoKai Xi]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 
 ## About
 
 * This package contains partial extrapolation methods in quantum chemistry, written using the extrapolation method proposed in the literature. Extrapolation to the CBS limit can be done by entering two successive energies.
 
 ## Quickly Use
 
-* Please use the `pip` command to install: `pip install packaging_extrapolation` or `python3 -m pip install packaging_extrapolation`
+* Please use the `pip` command to install: `pip install packaging-extrapolation` or `python3 -m pip install packaging-extrapolation`
 * Please make sure the package is the latest: `pip install --upgrade packaging_extrapolation`
 * After installation, test the example in `src/packaging_extrapolation/examples/examples_energy.py` to see if you get results.
   * Extrapolation Method Calls: `python  examples_energy.py -m "Klopper_1986" -xe -76.0411795 -ye -76.0603284 -low 2 -high 3 -a 4.25`
   * `-m`: extrapolation method name.
   * `-xe`: energy for E(X).
   * `-ye`: energy for E(Y).
   * `-low`: cardinal number for X.
@@ -126,21 +126,21 @@
 NH2,-55.5749363,-55.5878344
 NH3,-56.1972947,-56.2127423
 NO2,-204.0664514,-204.1137363
 ```
 
 
 
-| Functions                                                    |
-| ------------------------------------------------------------ |
-| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol). |
-| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol). |
-| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol). |
-| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy. |
-| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files. |
-| `train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
+| Functions                                                                                                                                                                                       |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `UtilTools.calc_MAD(y_true, y_pred)`: Calculate the Mean Absolute Deviation (kcal/mol).                                                                                                         |
+| `UtilTools.calc_max_MAD(y_true, y_pred)`: Calculate the Maximum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_min_MAD(y_true, y_pred)`: Calculate the Minimum Absolute Deviation (kcal/mol).                                                                                                  |
+| `UtilTools.calc_RMSE(y_true, y_pred)`: Calculate the Root Mean Square Deviation (kcal/mol).                                                                                                     |
+| `UtilTools.calc_MSD(y_true, y_pred)`: Calculate the Mean Square Deviation (kcal/mol).                                                                                                           |
+| `UtilTools.calc_MaxPosMAD(y_true, y_pred)`: Calculate the Maximum Positive Deviation (kcal/mol).                                                                                                |
+| `UtilTools.train_alpha(*,  model, method, x_energy_list, y_energy_list, alpha, low_card, high_card)`: Calculate extrapolated energy.                                                            |
+| `UtilLog.extract_energy(input_path, output_path)`: Extracting energy from many log files.                                                                                                       |
+| `UtilLog.train_all(*, model, method, x_energy_list, y_energy_list, low_card, high_card, limit_list, init_guess=0.001, temp='RMSD')` : Optimizing extrapolation parameters with `RMSD` or `MAD`. |
```

