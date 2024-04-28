# Comparing `tmp/luma-ml-0.7.1.tar.gz` & `tmp/luma-ml-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.1.tar", last modified: Tue Apr 23 16:20:04 2024, max compression
+gzip compressed data, was "luma-ml-0.7.2.tar", last modified: Sun Apr 28 08:56:41 2024, max compression
```

## Comparing `luma-ml-0.7.1.tar` & `luma-ml-0.7.2.tar`

### file list

```diff
@@ -1,90 +1,88 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.247055 luma-ml-0.7.1/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.1/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-23 16:20:04.246658 luma-ml-0.7.1/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-23 15:45:00.000000 luma-ml-0.7.1/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.230214 luma-ml-0.7.1/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10349 2024-04-23 15:02:10.000000 luma-ml-0.7.1/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.1/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.231884 luma-ml-0.7.1/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-21 11:35:44.000000 luma-ml-0.7.1/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.1/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.1/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.1/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.1/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.1/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.232982 luma-ml-0.7.1/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.1/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.1/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.1/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.1/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.1/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.1/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.233887 luma-ml-0.7.1/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.7.1/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-18 09:50:34.000000 luma-ml-0.7.1/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11480 2024-04-18 20:49:42.000000 luma-ml-0.7.1/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.235090 luma-ml-0.7.1/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.1/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.1/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.1/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.1/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.1/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.235964 luma-ml-0.7.1/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.1/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2696 2024-04-21 13:53:19.000000 luma-ml-0.7.1/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14826 2024-04-23 15:24:58.000000 luma-ml-0.7.1/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.236723 luma-ml-0.7.1/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1473 2024-04-21 11:35:58.000000 luma-ml-0.7.1/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5742 2024-04-21 11:35:59.000000 luma-ml-0.7.1/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1553 2024-04-21 11:36:01.000000 luma-ml-0.7.1/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1648 2024-04-21 11:36:02.000000 luma-ml-0.7.1/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.237181 luma-ml-0.7.1/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.1/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.237908 luma-ml-0.7.1/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.1/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.1/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.1/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-04-21 11:36:06.000000 luma-ml-0.7.1/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.239811 luma-ml-0.7.1/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     1154 2024-04-23 15:01:38.000000 luma-ml-0.7.1/luma/neural/activation.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4350 2024-04-23 16:17:50.000000 luma-ml-0.7.1/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-23 16:10:06.000000 luma-ml-0.7.1/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    22320 2024-04-23 16:19:59.000000 luma-ml-0.7.1/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2681 2024-04-23 14:55:20.000000 luma-ml-0.7.1/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16804 2024-04-23 15:06:00.000000 luma-ml-0.7.1/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    20835 2024-04-21 11:36:11.000000 luma-ml-0.7.1/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.1/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.240030 luma-ml-0.7.1/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.1/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.240733 luma-ml-0.7.1/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.1/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.1/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.1/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.1/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.241576 luma-ml-0.7.1/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.1/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.1/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.1/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.243482 luma-ml-0.7.1/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.1/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.1/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.1/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.1/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.1/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.1/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.1/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.243921 luma-ml-0.7.1/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.1/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.1/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.244981 luma-ml-0.7.1/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1701 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-23 16:20:04.247154 luma-ml-0.7.1/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-23 15:45:10.000000 luma-ml-0.7.1/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.245998 luma-ml-0.7.1/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.1/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2108 2024-04-23 16:13:28.000000 luma-ml-0.7.1/test/__test.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2059 2024-04-21 12:40:24.000000 luma-ml-0.7.1/test/_mlp.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.545930 luma-ml-0.7.2/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.2/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-28 08:56:41.545574 luma-ml-0.7.2/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-28 08:56:35.000000 luma-ml-0.7.2/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.517832 luma-ml-0.7.2/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10290 2024-04-28 08:49:23.000000 luma-ml-0.7.2/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.2/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.521151 luma-ml-0.7.2/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.2/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.2/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.2/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.2/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.2/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.2/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.525297 luma-ml-0.7.2/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.2/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.2/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.2/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.2/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.2/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.2/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.526201 luma-ml-0.7.2/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-04-28 07:19:53.000000 luma-ml-0.7.2/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.2/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11588 2024-04-28 08:33:36.000000 luma-ml-0.7.2/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.528856 luma-ml-0.7.2/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.2/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.2/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.2/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.2/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.2/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.529747 luma-ml-0.7.2/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.2/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-25 18:52:30.000000 luma-ml-0.7.2/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15126 2024-04-28 08:49:04.000000 luma-ml-0.7.2/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.530789 luma-ml-0.7.2/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.2/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.2/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.2/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.2/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.530972 luma-ml-0.7.2/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.2/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.532778 luma-ml-0.7.2/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.2/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.2/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.2/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-04-21 11:36:06.000000 luma-ml-0.7.2/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.534456 luma-ml-0.7.2/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)     4379 2024-04-28 05:47:17.000000 luma-ml-0.7.2/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-24 13:56:17.000000 luma-ml-0.7.2/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25256 2024-04-28 08:53:42.000000 luma-ml-0.7.2/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-04-27 18:48:15.000000 luma-ml-0.7.2/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6772 2024-04-28 08:56:03.000000 luma-ml-0.7.2/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-04-28 05:47:13.000000 luma-ml-0.7.2/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.2/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.534954 luma-ml-0.7.2/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.2/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.536290 luma-ml-0.7.2/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.2/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.2/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.2/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.2/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.538502 luma-ml-0.7.2/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.2/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.2/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.2/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.542136 luma-ml-0.7.2/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.2/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.2/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.2/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.2/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.2/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.2/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.2/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.542703 luma-ml-0.7.2/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.2/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.2/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.544224 luma-ml-0.7.2/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1662 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-28 08:56:41.000000 luma-ml-0.7.2/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-28 08:56:41.545997 luma-ml-0.7.2/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-04-28 08:56:37.000000 luma-ml-0.7.2/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-28 08:56:41.544858 luma-ml-0.7.2/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.2/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      917 2024-04-28 08:55:29.000000 luma-ml-0.7.2/test/__test.py
```

### Comparing `luma-ml-0.7.1/LICENSE` & `luma-ml-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/PKG-INFO` & `luma-ml-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
-Home-page: https://github.com/ChanLumerico/LUMA
+Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,15 +108,15 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.1</td>
+                    <td>0.7.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
                     <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.1 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.2 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
-github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
+github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.07k-red][GitHub code size in bytes][Code Style]
+5.13k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.1
+Latest Version 0.7.2
 Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.1/README.md` & `luma-ml-0.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,15 +89,15 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.1</td>
+                    <td>0.7.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
                     <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.07k-red][GitHub code size in bytes][Code Style]
+5.13k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.1
+Latest Version 0.7.2
 Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.1/luma/__import__.py` & `luma-ml-0.7.2/luma/__import__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from luma.core.main import Luma
 from luma.core.base import ModelBase, ParadigmBase, MetricBase, VisualBase
-from luma.core.super import Estimator, Transformer, Optimizer, Evaluator, Visualizer
+from luma.core.super import (
+    Estimator,
+    Transformer,
+    Optimizer,
+    Evaluator,
+    Visualizer,
+    NeuralModel,
+)
 from luma.core.super import Supervised, Unsupervised, Distance
 
 from luma.interface.exception import (
     NotFittedError,
     NotConvergedError,
     UnsupportedParameterError,
     ModelExtensionError,
@@ -12,25 +19,26 @@
 )
 from luma.interface.typing import (
     TensorLike,
     Matrix,
     Vector,
     Tensor,
     Scalar,
+    ClassType,
 )
 from luma.interface.util import (
     DecisionTreeNode,
     NearestNeighbors,
     SilhouetteUtil,
     DBUtil,
     KernelUtil,
-    ActivationUtil,
     InitUtil,
     Clone,
     ParamRange,
+    TrainProgress,
 )
 
 from luma.classifier.discriminant import (
     LDAClassifier,
     QDAClassifier,
     RDAClassifier,
     KDAClassifier,
@@ -66,31 +74,37 @@
 from luma.ensemble.forest import RandomForestClassifier, RandomForestRegressor
 from luma.ensemble.vote import VotingClassifier, VotingRegressor
 from luma.ensemble.bagging import BaggingClassifier, BaggingRegressor
 from luma.ensemble.boost import AdaBoostClassifier, AdaBoostRegressor
 from luma.ensemble.boost import GradientBoostingClassifier, GradientBoostingRegressor
 from luma.ensemble.stack import StackingClassifier, StackingRegressor
 
-from luma.neural.activation import ReLU, LeakyReLU, ELU, Tanh, Sigmoid
 from luma.neural.optimizer import (
     SGDOptimizer,
     MomentumOptimizer,
     RMSPropOptimizer,
     AdamOptimizer,
     AdaGradOptimizer,
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
-from luma.neural.network import MLPClassifier, MLPRegressor
 from luma.neural.base import Layer, Loss, Initializer
-from luma.neural.layer import Convolution, Pooling, Dense, Dropout, Flatten, Sequential
-from luma.neural.loss import SoftmaxLoss, CrossEntropyLoss, MSELoss
+from luma.neural.layer import (
+    Convolution,
+    Pooling,
+    Dense,
+    Dropout,
+    Flatten,
+    Activation,
+    Sequential,
+)
+from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
@@ -166,26 +180,26 @@
 
     # ------------------- [ luma.core ] ------------------------
     Luma
 
     ModelBase, ParadigmBase, MetricBase, VisualBase
 
     Estimator, Transformer, Optimizer, Evaluator, Visualizer,
-    Supervised, Unsupervised, Distance
+    Supervised, Unsupervised, Distance, NeuralModel
 
     # ----------------- [ luma.interface ] ---------------------
     NotFittedError, NotConvergedError,
     UnsupportedParameterError, ModelExtensionError,
     InvalidRangeError
 
-    TensorLike, Matrix, Vector, Tensor, Scalar
+    TensorLike, Matrix, Vector, Tensor, Scalar, ClassType
 
     DecisionTreeNode, NearestNeighbors,
-    SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil,
-    InitUtil, Clone, ParamRange
+    SilhouetteUtil, DBUtil, KernelUtil, InitUtil, Clone,
+    ParamRange, TrainProgress
 
     # ----------------- [ luma.classifier ] --------------------
     LDAClassifier, QDAClassifier, RDAClassifier, KDAClassifier
 
     LogisticRegressor, SoftmaxRegressor
 
     GaussianNaiveBayes, BernoulliNaiveBayes
@@ -224,27 +238,24 @@
     GradientBoostingClassifier, GradientBoostingRegressor
 
     StackingClassifier, StackingRegressor
 
     # ------------------- [ luma.neural ] ----------------------
     PerceptronClassifier, PerceptronRegressor
 
-    MLPClassifier, MLPRegressor
-
-    ReLU, LeakyReLU, ELU, Tanh, Sigmoid
-
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
     Layer, Loss, Initializer
 
-    Convolution, Pooling, Dense, Dropout, Flatten, Sequential
+    Convolution, Pooling, Dense, Dropout, Flatten, Activation,
+    Sequential
 
-    SoftmaxLoss, CrossEntropyLoss, MSELoss
+    CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
```

### Comparing `luma-ml-0.7.1/luma/__init__.py` & `luma-ml-0.7.2/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/discriminant.py` & `luma-ml-0.7.2/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/logistic.py` & `luma-ml-0.7.2/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/naive_bayes.py` & `luma-ml-0.7.2/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/neighbors.py` & `luma-ml-0.7.2/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/svm.py` & `luma-ml-0.7.2/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/classifier/tree.py` & `luma-ml-0.7.2/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/affinity.py` & `luma-ml-0.7.2/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/density.py` & `luma-ml-0.7.2/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/hierarchy.py` & `luma-ml-0.7.2/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/kmeans.py` & `luma-ml-0.7.2/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/mixture.py` & `luma-ml-0.7.2/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/clustering/spectral.py` & `luma-ml-0.7.2/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/core/base.py` & `luma-ml-0.7.2/luma/core/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import Any, Dict
 
 from luma.core.main import Luma
 from luma.interface.util import ParamRange
 
 
-__all__ = ("ModelBase", "ParadigmBase", "MetricBase", "VisualBase")
+__all__ = (
+    "ModelBase",
+    "ParadigmBase",
+    "MetricBase",
+    "VisualBase",
+    "NeuralBase",
+)
 
 
 class ModelBase(Luma):
     """
     The ModelBase class serves as a superclass for core machine learning components
     involved in modeling and data transformation. It provides a foundational base
     for classes like Estimator and Transformer, encapsulating shared functionalities
@@ -147,11 +153,34 @@
 
     """
 
     def __validate__(self) -> None:
         return super().__validate__()
 
     def __alloc__(self, *args, **kwargs) -> None:
+        return super().__alloc__(*args, **kwargs)
+
+    def __dealloc__(self) -> None:
+        return super().__dealloc__()
+
+
+class NeuralBase(Luma):
+    """
+    This class provides the foundational attributes and methods that are common
+    across different types of neural network models. It is not intended to be
+    instantiated directly but should be subclassed by specific types of neural
+    models that implement the specific functionalities.
+
+    Inheritances
+    ------------
+    `NeuralModel`
+
+    """
+
+    def __validate__(self) -> None:
+        return super().__validate__()
+
+    def __alloc__(self, *args, **kwargs) -> None:
         return super().__alloc__(*args, **kwargs)
 
     def __dealloc__(self) -> None:
         return super().__dealloc__()
```

### Comparing `luma-ml-0.7.1/luma/core/super.py` & `luma-ml-0.7.2/luma/core/super.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "Transformer",
     "Optimizer",
     "Evaluator",
     "Visualizer",
     "Supervised",
     "Unsupervised",
     "Distance",
+    "NeuralModel",
 )
 
 
 class Estimator(ModelBase, metaclass=ABCMeta):
     """
     An estimator is a mathematical model or algorithm
     used to make predictions or estimates based on data.
@@ -81,27 +82,14 @@
           estimators for improved performance or functionality. When
           integrating `TimeSeries` models with `Meta` estimators,
           special consideration is needed to ensure compatibility and
           effective integration.
 
         """
 
-    class NeuralNet:
-        """
-        An inner class of `Estimator` dedicated to neural networks.
-
-        Neural networks are computational models inspired by the human brain,
-        consisting of layers of interconnected nodes (neurons) that process
-        information through weighted connections. These models include an input
-        layer to receive data, hidden layers that perform computations, and an
-        output layer to deliver results.
-        """
-
-        def dump(self, **kwargs) -> None: ...
-
     @abstractmethod
     def fit(self, *args) -> Self: ...
 
     @abstractmethod
     def predict(self, *args) -> Any: ...
 
     @abstractmethod
@@ -338,16 +326,14 @@
     """
     Supervised learning is a type of machine learning where the algorithm learns
     to make predictions or decisions by training on a labeled dataset.
     In this approach, the algorithm is provided with input data and corresponding
     target labels, and it learns to map the inputs to the correct outputs.
     """
 
-    def __init__(self, *args) -> None: ...
-
 
 class Unsupervised(ParadigmBase):
     """
     Unsupervised learning is a machine learning paradigm where the algorithm
     is given input data without explicit target labels. Instead of making predictions,
     the algorithm's goal is to discover hidden patterns, structures,
     or relationships within the data.
@@ -359,16 +345,14 @@
     Get assigned labels:
     ```py
         @property
         def labels(self) -> Vector
     ```
     """
 
-    def __init__(self, *args) -> None: ...
-
     @property
     def labels(self) -> Any: ...
 
 
 class Distance(MetricBase, metaclass=ABCMeta):
     """
     In mathematics and machine learning, distance is a measure of how much "separation"
@@ -381,10 +365,30 @@
     ```py
         @staticmethod
         @abstractmethod
         def compute(*args) -> float
     ```
     """
 
-    @staticmethod
     @abstractmethod
-    def compute(*args) -> float: ...
+    def score(*args) -> float: ...
+
+
+class NeuralModel(NeuralBase, metaclass=ABCMeta):
+    """
+    Neural networks are computational models inspired by the human brain,
+    consisting of layers of interconnected nodes (neurons) that process
+    information through weighted connections. These models include an input
+    layer to receive data, hidden layers that perform computations, and an
+    output layer to deliver results.
+    """
+
+    def __init_model__(self) -> None:
+        self.running_loss_: list[float] = []
+        self.train_loss_: list[float] = []
+        self.valid_loss_: list[float] = []
+
+    @abstractmethod
+    def train(self, **kwargs) -> list[float]: ...
+
+    @abstractmethod
+    def eval(self, **kwargs) -> list[float]: ...
```

### Comparing `luma-ml-0.7.1/luma/ensemble/bagging.py` & `luma-ml-0.7.2/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/ensemble/boost.py` & `luma-ml-0.7.2/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/ensemble/forest.py` & `luma-ml-0.7.2/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/ensemble/stack.py` & `luma-ml-0.7.2/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/ensemble/vote.py` & `luma-ml-0.7.2/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/interface/exception.py` & `luma-ml-0.7.2/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/interface/util.py` & `luma-ml-0.7.2/luma/interface/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Any, AnyStr, Callable, Literal, Optional, Type, TypeGuard
+from typing import Any, Callable, Iterable, Literal, Type, TypeGuard
+from rich.progress import Progress, BarColumn, TextColumn
 import numpy as np
 
 from luma.interface.exception import UnsupportedParameterError, InvalidRangeError
 from luma.interface.typing import Matrix, Scalar
-from luma.neural import activation, init
+from luma.neural import init
 
 
 __all__ = (
     "DecisionTreeNode",
     "NearestNeighbors",
     "SilhouetteUtil",
     "DBUtil",
     "KernelUtil",
     "ActivationUtil",
     "InitUtil",
     "Clone",
     "ParamRange",
+    "TrainProgress",
 )
 
 
 class DecisionTreeNode:
     """
     Internal class for node used in tree-based models.
 
@@ -107,15 +109,18 @@
         self.labels = labels
         self.distances = distances
 
     @property
     def avg_dist_others(self) -> Matrix:
         others = set(self.labels) - {self.cluster}
         sub_avg = [
-            np.mean(self.distances[self.idx][self.labels == other]) for other in others
+            np.mean(
+                self.distances[self.idx][self.labels == other],
+            )
+            for other in others
         ]
 
         return np.mean(sub_avg)
 
     @property
     def avg_dist_within(self) -> Matrix | int:
         within_cluster = self.distances[self.idx][self.labels == self.cluster]
@@ -260,85 +265,14 @@
             return self.sigmoid_kernel
         elif self.kernel in ("laplacian", "lap"):
             return self.laplacian_kernel
         else:
             raise UnsupportedParameterError(self.kernel)
 
 
-class ActivationUtil:
-    """
-    Internal class for activaiton functions used in neural networks.
-
-    Properties
-    ----------
-    For getting an activation function class:
-    ```py
-    @property
-    def activation_type(self) -> type
-    ```
-
-    Notes
-    -----
-    When the passed activation is `None`, an identity activation is
-    returned, with its function and gradient being identity functions.
-
-    Examples
-    --------
-    >>> act = ActivationUtil(activation='relu')
-    >>> relu = act.activation_type
-    ReLU()
-
-    """
-
-    FuncType = Optional[
-        Literal[
-            "relu",
-            "ReLU",
-            "leaky-relu",
-            "leaky-ReLU",
-            "elu",
-            "ELU",
-            "tanh",
-            "sigmoid",
-            "sig",
-        ]
-    ]
-
-    def __init__(self, activation: str) -> None:
-        self.activation = activation
-
-    @property
-    def activation_type(self) -> type:
-        if self.activation is None:
-            return self._return_identity()
-
-        if self.activation in ("relu", "ReLU"):
-            return activation.ReLU
-        elif self.activation in ("leaky-relu", "leaky-ReLU"):
-            return activation.LeakyReLU
-        elif self.activation in ("elu", "ELU"):
-            return activation.ELU
-        elif self.activation in ("tanh"):
-            return activation.Tanh
-        elif self.activation in ("sigmoid", "sig"):
-            return activation.Sigmoid
-        else:
-            raise UnsupportedParameterError(self.activation)
-
-    def _return_identity(self) -> type:
-        class _Identity:
-            def func(self, X: Matrix) -> Matrix:
-                return X
-
-            def grad(self, X: Matrix) -> Matrix:
-                return X
-
-        return _Identity
-
-
 class Clone:
     """
     A utility class for cloning LUMA models.
 
     This class creates a copy of a given LUMA model,
     which can be either an Estimator or a Transformer.
     The clone includes all parameters of the original model.
@@ -417,17 +351,21 @@
     Notes
     -----
     - When setting a custom range for `param_range`, it must follow the form of
         "lower_bound,upper_bound". (i.e. `-inf,20`, `-5,5`)
     - For open intervals, add '<' inside the range. (i.e. `0<,+inf`, `0<,<10`)
     """
 
-    type RangeStr = AnyStr
+    type RangeStr = str
 
-    def __init__(self, param_range: RangeStr, param_type: Type[Scalar] = None) -> None:
+    def __init__(
+        self,
+        param_range: RangeStr,
+        param_type: Type[Scalar] = None,
+    ) -> None:
         self.param_range = param_range
 
         if param_type is None:
             self.param_type = int | float
         else:
             if not ParamRange.validate_type(param_type):
                 raise UnsupportedParameterError(param_type)
@@ -482,48 +420,108 @@
 
 class InitUtil:
     """
     An utility class for weight initializers used in neural networks.
 
     Parameters
     ----------
-    `initializer` : Name of an initializer (`InitType`)
-    `activation` : Name of an activation function (`FuncType`)
+    `initializer` : Name of an initializer (`InitStr`)
 
     Properties
     ----------
     To get the corresponding initializer type:
     ```py
     @property
     def initializer_type(self) -> type | None
     # `None` for random init
     ```
     """
 
-    InitType = Literal["he", "kaiming", "xavier", "auto", "random"]
+    InitStr = Literal["he", "kaiming", "xavier", "glorot"] | None
 
-    def __init__(
-        self,
-        initializer: InitType,
-        activation: ActivationUtil.FuncType,
-    ) -> None:
+    def __init__(self, initializer: InitStr) -> None:
         self.initializer = initializer
-        self.activation = activation
 
     @property
     def initializer_type(self) -> type | None:
-        if self.initializer == "auto":
-            return self._auto_init()
-        else:
-            return self._manual_init()
-
-    def _manual_init(self) -> type | None:
+        if self.initializer is None:
+            return None
         if self.initializer in ("he", "kaiming"):
             return init.KaimingInit
-        elif self.initializer in ("xavier"):
+        elif self.initializer in ("xavier", "glorot"):
             return init.XavierInit
 
-    def _auto_init(self) -> type | None:
-        if self.activation in ("relu", "ReLU"):
-            return init.KaimingInit
-        elif self.activation in ("tanh", "sigmoid", "sig"):
-            return init.XavierInit
+
+class TrainProgress:
+    """
+    An utility class for managing auto-updating progress bar during training.
+
+    It facilitates the progress bar from the module `rich`, which provides
+    well-structured progress bar with colored indications for better readability.
+
+    Property
+    --------
+    To get an iterable object from `rich.progress.Progress`:
+    ```py
+    (property) progress: (self: Self@TrainProgress) -> Iterable
+    ```
+
+    Exmaples
+    --------
+    Create an instance for `TrainProgress`:
+    >>> train_prog = TrainProgress(n_epochs=100)
+
+    Generate a task and update the progress bar:
+    ```py
+    with train_prog.progress as progress:
+        train_prog.add_task(progress=progress, model=AnyModelInstance)
+
+        for epoch in range(n_epochs):
+            train_prog.update(progress=progress, cur=epoch, losses=[...])
+            # losses is a list of [train_loss, valid_loss]
+    ```
+    """
+
+    def __init__(self, n_epochs: int, bar_width: int = 50) -> None:
+        self.n_epochs = n_epochs
+        self.bar_width = bar_width
+        self.task = None
+
+    @property
+    def progress(self) -> Iterable:
+        return Progress(
+            TextColumn("[progress.description]{task.description}"),
+            BarColumn(bar_width=self.bar_width),
+            TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
+            TextColumn("[bold green]{task.fields[train_loss]:.4f}"),
+            TextColumn("[bold red]{task.fields[valid_loss]:.4f}"),
+            expand=True,
+        )
+
+    def _check_task_exist(self) -> None:
+        if self.task is None:
+            raise RuntimeError(f"'{type(self).__name__}' does not have any tasks!")
+
+    def add_task(self, progress: Progress, model: object) -> None:
+        self.task = progress.add_task(
+            f"[purple]Start {type(model).__name__} training "
+            + f"with {self.n_epochs} epochs.",
+            total=self.n_epochs,
+            train_loss=0.0,
+            valid_loss=0.0,
+        )
+
+    def update(
+        self,
+        progress: Progress,
+        cur: int,
+        losses: list[float, float],
+    ) -> None:
+        self._check_task_exist()
+        progress.update(
+            self.task,
+            advance=1,
+            train_loss=losses[0],
+            valid_loss=losses[1],
+            description=f"Epoch: {cur}/{self.n_epochs} - "
+            + f"Train/Valid Loss: {losses[0]:.4f}/{losses[1]:.4f}",
+        )
```

### Comparing `luma-ml-0.7.1/luma/metric/classification.py` & `luma-ml-0.7.2/luma/metric/classification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import numpy as np
 
-from luma.interface.typing import Matrix
+from luma.interface.typing import Matrix, ClassType
 from luma.core.super import Evaluator
 
 
 __all__ = ("Accuracy", "Precision", "Recall", "F1Score", "Specificity")
 
 
+@ClassType.non_instantiable()
 class Accuracy(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean(y_true == y_pred)
 
 
+@ClassType.non_instantiable()
 class Precision(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         true_positives = np.sum((y_true == 1) & (y_pred == 1))
         false_positives = np.sum((y_true == 0) & (y_pred == 1))
         return true_positives / (true_positives + false_positives)
 
 
+@ClassType.non_instantiable()
 class Recall(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         true_positives = np.sum((y_true == 1) & (y_pred == 1))
         false_negatives = np.sum((y_true == 1) & (y_pred == 0))
         return true_positives / (true_positives + false_negatives)
 
 
+@ClassType.non_instantiable()
 class F1Score(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         precision = Precision.score(y_true, y_pred)
         recall = Recall.score(y_true, y_pred)
         return 2 * (precision * recall) / (precision + recall)
 
 
+@ClassType.non_instantiable()
 class Specificity(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         true_negatives = np.sum((y_true == 0) & (y_pred == 0))
         false_positives = np.sum((y_true == 0) & (y_pred == 1))
         return true_negatives / (true_negatives + false_positives)
```

### Comparing `luma-ml-0.7.1/luma/metric/clustering.py` & `luma-ml-0.7.2/luma/metric/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 from scipy.spatial.distance import pdist, squareform
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.core.super import Evaluator, Visualizer
 from luma.interface.util import SilhouetteUtil, DBUtil
-from luma.interface.typing import Matrix
+from luma.interface.typing import Matrix, ClassType
 
 
 __all__ = ("SilhouetteCoefficient", "DaviesBouldin", "Inertia")
 
 
 class SilhouetteCoefficient(Evaluator, Visualizer):
     """
@@ -107,30 +107,31 @@
         plt.tight_layout()
 
         if show:
             plt.show()
         return ax
 
 
+@ClassType.non_instantiable()
 class DaviesBouldin(Evaluator):
     """
     The Davies-Bouldin Index (DBI) is a metric for evaluating clustering
     algorithms. It compares the average distance within clusters to the
     distance between clusters. Lower DBI values indicate better clustering,
     with compact and well-separated clusters.
 
     Parameters
     ----------
     `data` : Original data
     `labels` : Labels assigned by clustering estimator
 
     """
 
-    @staticmethod
-    def score(data: Matrix, labels: Matrix) -> float:
+    @classmethod
+    def score(cls, data: Matrix, labels: Matrix) -> float:
         util = DBUtil(data=data, labels=labels)
         centroids = util.cluster_centroids
         scatter = util.within_cluster_scatter
         separation = util.separation
 
         n_clusters = len(centroids)
         db_values = np.zeros(n_clusters)
@@ -146,14 +147,15 @@
 
             db_values[i] = max_ratio
         db_index = np.mean(db_values)
 
         return db_index
 
 
+@ClassType.non_instantiable()
 class Inertia(Evaluator):
     """
     Inertia in clustering quantifies the compactness of clusters by measuring
     the sum of squared distances between data points and their respective
     cluster centroids. It serves as a key metric to evaluate the quality of
     cluster assignments in algorithms like K-means. A lower inertia value
     indicates more cohesive clusters, where data points are closer to their
@@ -163,16 +165,16 @@
     Parameters
     ----------
     `data` : Original data
     `centroids`: Centroids(or medoids for certain algorithm)
 
     """
 
-    @staticmethod
-    def score(data: Matrix, centroids: Matrix) -> float:
+    @classmethod
+    def score(cls, data: Matrix, centroids: Matrix) -> float:
         sq_dist = (data[:, np.newaxis, :] - centroids[np.newaxis, :, :]) ** 2
         dist = np.sqrt(sq_dist.sum(axis=2))
 
         closest = np.argmin(dist, axis=1)
         inertia = sum((dist[i, closest[i]] ** 2) for i in range(len(data)))
 
         return inertia
```

### Comparing `luma-ml-0.7.1/luma/metric/regression.py` & `luma-ml-0.7.2/luma/metric/regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-from typing import *
 import numpy as np
 
-from luma.interface.typing import Matrix
+from luma.interface.typing import Matrix, ClassType
 from luma.core.super import Evaluator
 
 
 __all__ = (
     "MeanAbsoluteError",
     "MeanSquaredError",
     "RootMeanSquaredError",
     "MeanAbsolutePercentageError",
     "RSquaredScore",
     "AdjustedRSquaredScore",
 )
 
 
+@ClassType.non_instantiable()
 class MeanAbsoluteError(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean(np.abs(y_true - y_pred))
 
 
+@ClassType.non_instantiable()
 class MeanSquaredError(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean((y_true - y_pred) ** 2)
 
 
+@ClassType.non_instantiable()
 class RootMeanSquaredError(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         return np.sqrt(np.mean((y_true - y_pred) ** 2))
 
 
+@ClassType.non_instantiable()
 class MeanAbsolutePercentageError(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         return np.mean(np.abs((y_true - y_pred) / y_true)) * 100
 
 
+@ClassType.non_instantiable()
 class RSquaredScore(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix) -> float:
         y_bar = np.mean(y_true)
         sst = np.sum((y_true - y_bar) ** 2)
         ssr = np.sum((y_true - y_pred) ** 2)
         r2 = 1 - (ssr / sst)
         return r2
 
 
+@ClassType.non_instantiable()
 class AdjustedRSquaredScore(Evaluator):
-    @staticmethod
-    def score(y_true: Matrix, y_pred: Matrix, n_predictors: int) -> float:
+    @classmethod
+    def score(cls, y_true: Matrix, y_pred: Matrix, n_predictors: int) -> float:
         m = len(y_true)
         y_bar = np.mean(y_true)
         sst = np.sum((y_true - y_bar) ** 2)
         ssr = np.sum((y_true - y_pred) ** 2)
         r2 = 1 - (ssr / sst)
         r2_adj = 1 - ((1 - r2) * (m - 1) / (m - n_predictors - 1))
         return r2_adj
```

### Comparing `luma-ml-0.7.1/luma/migrate/port.py` & `luma-ml-0.7.2/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/model_selection/cv.py` & `luma-ml-0.7.2/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/model_selection/fold.py` & `luma-ml-0.7.2/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/model_selection/search.py` & `luma-ml-0.7.2/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/model_selection/split.py` & `luma-ml-0.7.2/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/neural/base.py` & `luma-ml-0.7.2/luma/neural/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 import numpy as np
 
-from luma.interface.typing import Matrix, Tensor, Vector
+from luma.interface.typing import Matrix, Tensor, TensorLike
 from luma.core.base import ModelBase
 from luma.interface.util import InitUtil
 
 
 __all__ = ("Layer", "Loss", "Initializer")
 
 
@@ -34,55 +34,54 @@
     To get its parameter size (weights, biases):
     ```py
     (property) param_size: Tuple[int, int]
     ```
     """
 
     def __init__(self) -> None:
-        self.input_: Tensor = None
-        self.weights_: Tensor = None
-        self.biases_: Vector = None
-
-        self.dX: Tensor = None
-        self.dW: Tensor = None
-        self.dB: Tensor = None
+        self.input_: TensorLike = None
+        self.output_: TensorLike = None
+
+        self.weights_: TensorLike = None
+        self.biases_: TensorLike = None
+
+        self.dX: TensorLike = None
+        self.dW: TensorLike = None
+        self.dB: TensorLike = None
 
         self.optimizer: object = None
         self.out_shape: tuple = None
 
-    def forward(self) -> Tensor: ...
+    def forward(self) -> TensorLike: ...
 
-    def backward(self) -> Tensor: ...
+    def backward(self) -> TensorLike: ...
 
     def update(self) -> None:
         if self.optimizer is None:
             return
         weights_, biases_ = self.optimizer.update(
             self.weights_, self.biases_, self.dW, self.dB
         )
         self.weights_ = Tensor(weights_)
         self.biases_ = Tensor(biases_)
 
     def init_params(self, w_shape: tuple, b_shape: tuple) -> None:
-        init_type_: type = InitUtil(
-            self.initializer,
-            self.activation,
-        ).initializer_type
+        init_type_: type = InitUtil(self.initializer).initializer_type
 
         if init_type_ is None:
             self.weights_ = 0.01 * self.rs_.randn(*w_shape)
         else:
             if len(w_shape) == 2:
                 self.weights_ = init_type_(self.random_state).init_2d(*w_shape)
             elif len(w_shape) == 4:
                 self.weights_ = init_type_(self.random_state).init_4d(*w_shape)
             else:
                 NotImplemented
 
-        self.biases_: Matrix = np.zeros(b_shape)
+        self.biases_: TensorLike = np.zeros(b_shape)
 
     @property
     def param_size(self) -> Tuple[int, int]:
         w_size, b_size = 0, 0
         if self.weights_ is not None:
             w_size += len(self.weights_.flatten())
         if self.biases_ is not None:
```

### Comparing `luma-ml-0.7.1/luma/neural/init.py` & `luma-ml-0.7.2/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/neural/layer.py` & `luma-ml-0.7.2/luma/neural/layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import Any, List, Literal, Self, Tuple
+from enum import Enum
+from typing import Any, List, Literal, Self, Tuple, Type
 import numpy as np
 
 from luma.core.super import Optimizer
-from luma.interface.typing import Matrix, Tensor
-from luma.interface.util import ActivationUtil, InitUtil, Clone
+from luma.interface.typing import Matrix, Tensor, ClassType
+from luma.interface.util import InitUtil, Clone
 from luma.interface.exception import UnsupportedParameterError
-from luma.neural.base import Layer, Loss
+from luma.neural.base import Layer
 
 
 __all__ = (
     "Convolution",
     "Pooling",
     "Dense",
     "Dropout",
     "Flatten",
+    "Activation",
     "Sequential",
 )
 
 
 class Convolution(Layer):
     """
     A convolutional layer in a neural network convolves learnable filters
@@ -30,16 +32,15 @@
     ----------
     `in_channels` : Number of input channels
     `out_channels` : Number of output channels(filters)
     `filter_size`: Size of each filter
     `stride` : Step size for filters during convolution
     `padding` : Padding stratagies
     (`valid` for no padding, `same` for typical 0-padding)
-    `activation` : Type of activation function
-    `initializer` : Type of weight initializer (default 'auto')
+    `initializer` : Type of weight initializer (default `None`)
     `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
     `lambda_` : L2-regularization strength
     `random_state` : Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
@@ -52,34 +53,29 @@
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
-        activation: ActivationUtil.FuncType = "relu",
-        initializer: InitUtil.InitType = "auto",
+        initializer: InitUtil.InitStr = None,
         optimizer: Optimizer = None,
         lambda_: float = 0.0,
         random_state: int = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
-        self.activation = activation
         self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
-
-        act = ActivationUtil(self.activation)
-        self.act_ = act.activation_type()
         self.rs_ = np.random.RandomState(self.random_state)
 
         self.init_params(
             w_shape=(
                 self.out_channels,
                 self.in_channels,
                 self.filter_size,
@@ -140,15 +136,14 @@
                 sampled_result = result[
                     pad_h : padded_h - pad_h : self.stride,
                     pad_w : padded_w - pad_w : self.stride,
                 ]
                 out[i, f] = sampled_result[:out_height, :out_width]
 
         out += self.biases_[:, :, np.newaxis, np.newaxis]
-        out = self.act_.func(out)
         return out
 
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         batch_size, channels, height, width = X.shape
         pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
 
@@ -189,18 +184,17 @@
                 dX_padded[i, c] = np.fft.irfftn(temp, s=(padded_h, padded_w))
 
         self.dX = (
             dX_padded[:, :, pad_h:-pad_h, pad_w:-pad_w]
             if pad_h > 0 or pad_w > 0
             else dX_padded
         )
-        self.dX = self.act_.grad(self.dX)
         return self.dX
 
-    def _get_padding_dim(self, height: int, width: int) -> Tuple[int, int, int, int]:
+    def _get_padding_dim(self, height: int, width: int) -> Tuple[int, ...]:
         if self.padding == "same":
             pad_h = pad_w = (self.filter_size - 1) // 2
             padded_h = height + 2 * pad_h
             padded_w = width + 2 * pad_w
 
         elif self.padding == "valid":
             pad_h = pad_w = 0
@@ -321,17 +315,16 @@
     data. They play a crucial role in capturing intricate patterns and
     features during the training process.
 
     Parameters
     ----------
     `in_features` : Number of input features
     `out_features`:  Number of output features
-    `activation` : Activation function (Use `Sigmoid` for final dense layer)
-    `initializer` : Type of weight initializer (default `auto`)
-    `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
+    `initializer` : Type of weight initializer (default `None`)
+    `optimizer` : Optimizer for weight update
     `lambda_` : L2-regularization strength
     `random_state` : Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 2D-array(`Matrix`).
 
@@ -340,31 +333,26 @@
         ```
     """
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
-        activation: ActivationUtil.FuncType = "relu",
-        initializer: InitUtil.InitType = "auto",
+        initializer: InitUtil.InitStr = None,
         optimizer: Optimizer = None,
         lambda_: float = 0.0,
         random_state: int = None,
     ) -> None:
         super().__init__()
         self.in_features = in_features
         self.out_features = out_features
-        self.activation = activation
         self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
-
-        act = ActivationUtil(self.activation)
-        self.act_ = act.activation_type()
         self.rs_ = np.random.RandomState(self.random_state)
 
         self.init_params(
             w_shape=(self.in_features, self.out_features),
             b_shape=(1, self.out_features),
         )
         self.set_param_ranges(
@@ -376,21 +364,19 @@
         )
         self.check_param_ranges()
 
     def forward(self, X: Matrix) -> Matrix:
         self.input_ = X
 
         out = np.dot(X, self.weights_) + self.biases_
-        out = self.act_.func(out)
         self.out_shape = out.shape
         return out
 
     def backward(self, d_out: Matrix) -> Matrix:
         X = self.input_
-        d_out = self.act_.grad(d_out)
 
         self.dX = np.dot(d_out, self.weights_.T)
         self.dW = np.dot(X.T, d_out)
         self.dW += 2 * self.lambda_ * self.weights_
         self.dB = np.sum(d_out, axis=0, keepdims=True)
 
         return self.dX
@@ -411,40 +397,39 @@
     Notes
     -----
     - During inference, dropout is typically turned off, and the layer behaves
       as the identity function.
 
     """
 
-    def __init__(self, dropout_rate: float = 0.5, random_state: int = None) -> None:
+    def __init__(
+        self,
+        dropout_rate: float = 0.5,
+        random_state: int = None,
+    ) -> None:
         super().__init__()
         self.dropout_rate = dropout_rate
         self.random_state = random_state
-
-        self.mask_: Tensor = None
         self.rs_ = np.random.RandomState(self.random_state)
+        self.mask_ = None
 
         self.set_param_ranges({"dropout_rate": ("0,1", None)})
         self.check_param_ranges()
 
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
-        self.input_ = X
-        self.out_shape = self.input_.shape
-
         if is_train:
-            self.mask_ = (
-                self.rs_.rand(*X.shape) < self.dropout_rate
-            ) / self.dropout_rate
-            return X * self.mask_
+            self.mask_ = self.rs_.rand(*X.shape) < (1 - self.dropout_rate)
+            return X * self.mask_ / (1 - self.dropout_rate)
         else:
             return X
 
     def backward(self, d_out: Tensor) -> Tensor:
-        dX = d_out * self.mask_ if self.mask_ is not None else d_out
-        return dX
+        if self.mask_ is not None:
+            return d_out * self.mask_ / (1 - self.dropout_rate)
+        return d_out
 
 
 class Flatten(Layer):
     """
     A flatten layer reshapes the input tensor into a 2D array(`Matrix`),
     collapsing all dimensions except the batch dimension.
 
@@ -464,14 +449,196 @@
         return out
 
     def backward(self, d_out: Matrix) -> Tensor:
         dX = d_out.reshape(self.input_.shape)
         return dX
 
 
+@ClassType.non_instantiable()
+class Activation:
+    """
+    An Activation Layer in a neural network applies a specific activation
+    function to the input it receives, transforming the input to activate
+    or deactivate neurons within the network. This function can be linear
+    or non-linear, such as Sigmoid, ReLU, or Tanh, which helps to introduce
+    non-linearity into the model, allowing it to learn complex patterns.
+
+    Notes
+    -----
+    - This class is not instantiable, meaning that a solitary use of it
+        is not available.
+
+    - All the activation functions are included inside `Activation`.
+
+    Examples
+    --------
+    >>> # Activation() <- Impossible
+    >>> Activation.Linear()
+    >>> Activation.ReLU()
+
+    """
+
+    type FuncType = Type
+
+    class Linear(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            return X
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out
+            return self.dX
+
+    class ReLU(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.input_ = X
+            return np.maximum(0, X)
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out.copy()
+            self.dX[self.input_ <= 0] = 0
+            return self.dX
+
+    class Sigmoid(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.output_ = 1 / (1 + np.exp(-X))
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * self.output_ * (1 - self.output_)
+            return self.dX
+
+    class Tanh(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.output_ = np.tanh(X)
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * (1 - np.square(self.output_))
+            return self.dX
+
+    class LeakyReLU(Layer):
+        def __init__(self, alpha: float = 0.01) -> None:
+            super().__init__()
+            self.alpha = alpha
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.input_ = X
+            return np.where(X > 0, X, X * self.alpha)
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * np.where(self.input_ > 0, 1, self.alpha)
+            return self.dX
+
+    class Softmax(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            e_X = np.exp(X - np.max(X, axis=-1, keepdims=True))
+            return e_X / np.sum(e_X, axis=-1, keepdims=True)
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = np.empty_like(d_out)
+            for i, (y, dy) in enumerate(zip(self.output_, d_out)):
+                y = y.reshape(-1, 1)
+                jacobian_matrix = np.diagflat(y) - np.dot(y, y.T)
+
+                self.dX[i] = np.dot(jacobian_matrix, dy)
+
+            return self.dX
+
+    class ELU(Layer):
+        def __init__(self, alpha: float = 1.0) -> None:
+            super().__init__()
+            self.alpha = alpha
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.input_ = X
+            self.output_ = np.where(X > 0, X, self.alpha * (np.exp(X) - 1))
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * np.where(
+                self.input_ > 0,
+                1,
+                self.output_ + self.alpha,
+            )
+            return self.dX
+
+    class SELU(Layer):
+        def __init__(
+            self,
+            lambda_: float = 1.0507,
+            alpha: float = 1.67326,
+        ) -> None:
+            super().__init__()
+            self.lambda_ = lambda_
+            self.alpha = alpha
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.input_ = X
+            self.output_ = self.lambda_ * np.where(
+                X > 0, X, self.alpha * (np.exp(X) - 1)
+            )
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = (
+                d_out
+                * self.lambda_
+                * np.where(
+                    self.input_ > 0,
+                    1,
+                    self.alpha * np.exp(self.input_),
+                )
+            )
+            return self.dX
+
+    class Softplus(Layer):
+        def __init__(self) -> None:
+            super().__init__()
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.output_ = np.log1p(np.exp(X))
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * (1 - 1 / (1 + np.exp(self.output_)))
+            return self.dX
+
+    class Swish(Layer):
+        def __init__(self, beta: float = 1.0) -> None:
+            super().__init__()
+            self.beta = beta
+
+        def forward(self, X: Tensor) -> Tensor:
+            self.input_ = X
+            self.sigmoid = 1 / (1 + np.exp(-self.beta * X))
+            self.output_ = X * self.sigmoid
+            return self.output_
+
+        def backward(self, d_out: Tensor) -> Tensor:
+            self.dX = d_out * (
+                self.sigmoid + self.input_ * self.sigmoid * (1 - self.sigmoid)
+            )
+            return self.dX
+
+
 class Sequential(Layer):
     """
     Sequential represents a linear arrangement of layers in a neural network
     model. Each layer is added sequentially, with data flowing from one layer
     to the next in the order they are added. This organization simplifies the
     construction of neural networks, especially for straightforward architectures,
     by mirroring the logical flow of data from input through hidden layers to
@@ -484,38 +651,28 @@
 
     Methods
     -------
     For setting an optimizer of each layer:
     ```py
     def set_optimizer(self, optimizer: Optimizer) -> None
     ```
-    For setting a loss function of the model:
-    ```py
-    def set_loss(self, loss_func: Loss) -> None
-    ```
     To add additional layer:
     ```py
     def add(self, layer: Layer) -> None
     ```
-    To compute loss:
-    ```py
-    def get_loss(y: Matrix, out: Matrix) -> float
-    ```
     Specials
     --------
-    - You can use `+` operator to add a layer or another instance of `Sequential`.
-
-    - By calling its instance, `forward`, `backward`, and `update`
-        is automatically called (single cycle) and the loss is returned.
+    - You can use `+` operator to add a layer or another instance
+        of `Sequential`.
 
-    - Use `repr()` to print out its structural configuration.
+    - Calling its instance performs a single forwarding.
 
     Notes
     -----
-    - Before any execution, an optimizer and a loss function must be assigned.
+    - Before any execution, an optimizer must be assigned.
 
     - For multi-class classification, the target variable `y`
         must be one-hot encoded.
 
     Examples
     --------
     ```py
@@ -525,154 +682,109 @@
         ...,
         ("drop", Dropout(0.1)),
         ("flat", Flatten()),
         ("dense_1", Dense(384, 32, activation="relu")),
         ("dense_2", Dense(32, 10, activation="softmax")),
     )
     model.set_optimizer(AnyOptimizer())
-    model.set_loss(AnyLoss())
-    ```
-    To use automated cyclic run:
-    >>> model(X, y, is_train=True)
-
-    Manual run:
-    >>> model.forward(X, is_train=True)
-    >>> model.backward(d_out)
-    >>> model.update()
 
+    out = model(X, is_train=True) # model.forward(X, is_train=True)
+    model.backward(d_out) # assume d_out is the gradient w.r.t. loss
+    model.update()
+    ```
     """
 
-    trainable: List[Layer] = [Convolution, Dense]
-    only_for_train: List[Layer] = [Dropout]
+    @ClassType.non_instantiable()
+    class LayerType(Enum):
+        ONLY_TRAIN: Tuple[Layer] = (Dropout,)
 
-    def __init__(
-        self,
-        *layers: Layer | Tuple[str, Layer],
-        verbose: bool = False,
-    ) -> None:
+    def __init__(self, *layers: Layer | Tuple[str, Layer]) -> None:
         self.layers: List[Tuple[str, Layer]] = list()
         for layer in layers:
             self.add(layer)
 
         self.optimizer = None
         self.loss_func_ = None
-        self.verbose = verbose
 
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         self.input_ = X
         out = X
 
-        for name, layer in self.layers:
-            if Sequential._check_only_for_train(layer):
+        for _, layer in self.layers:
+            if Sequential._check_only_train(layer):
                 out = layer.forward(out, is_train=is_train)
             else:
                 out = layer.forward(out)
-            if self.verbose:
-                print(f"[Sequential] Feed-forwarded '{name}'")
 
         self.out_shape = out.shape
         return out
 
     def backward(self, d_out: Matrix) -> None:
-        for name, layer in reversed(self.layers):
+        for _, layer in reversed(self.layers):
             d_out = layer.backward(d_out)
-            if self.verbose:
-                print(f"[Sequential] Backpropagated '{name}'")
 
     def update(self) -> None:
-        self._check_no_optimizer_loss()
-        for name, layer in reversed(self.layers):
+        self._check_no_optimizer()
+        for _, layer in reversed(self.layers):
             layer.update()
-            if self.verbose and Sequential._check_trainable_layer(layer):
-                print(f"[Sequential] Updated '{name}'")
 
     def set_optimizer(self, optimizer: Optimizer, **params: Any) -> None:
         self.optimizer = optimizer
         self.optimizer.set_params(**params, ignore_missing=True)
 
         for _, layer in self.layers:
             layer.optimizer = Clone(self.optimizer).get
 
-    def set_loss(self, loss_func: Loss) -> None:
-        self.loss_func_ = loss_func
-
-    def get_loss(self, y: Matrix, out: Matrix) -> float:
-        return self.loss_func_.loss(y, out)
-
-    @classmethod
-    def _check_only_for_train(cls, layer: Layer) -> bool:
-        return type(layer) in cls.only_for_train
-
     @classmethod
-    def _check_trainable_layer(cls, layer: Layer) -> bool:
-        return layer in cls.trainable
+    def _check_only_train(cls, layer: Layer) -> bool:
+        return type(layer) in cls.LayerType.ONLY_TRAIN.value
 
-    def _check_no_optimizer_loss(self) -> None:
+    def _check_no_optimizer(self) -> None:
         if self.optimizer is None:
             raise RuntimeError(
                 f"'{self}' has no optimizer! "
                 + f"Call '{self}().set_optimizer' to assign an optimizer."
             )
-        if self.loss_func_ is None:
-            raise RuntimeError(
-                f"'{self}' has no loss function! "
-                + f"Call '{self}().set_loss' to assign a loss function."
-            )
 
     def add(self, layer: Layer | Tuple[str, Layer]) -> None:
         if not isinstance(layer, tuple):
             layer = (str(layer), layer)
         self.layers.append(layer)
 
+        if self.optimizer is not None:
+            self.set_optimizer(self.optimizer)
+        if self.loss_func_ is not None:
+            self.set_loss(self.loss_func_)
+
     @property
     def param_size(self) -> Tuple[int, int]:
         w_size, b_size = 0, 0
         for _, layer in self.layers:
             w_, b_ = layer.param_size
             w_size += w_
             b_size += b_
 
         return w_size, b_size
 
-    def __call__(self, X: Tensor, y: Matrix, is_train: bool = False) -> float:
-        self._check_no_optimizer_loss()
-        out = self.forward(X, is_train=is_train)
-        d_out = self.loss_func_.grad(y, out)
-
-        self.backward(d_out)
-        self.update()
-        return self.get_loss(y, out)
+    def __call__(self, X: Tensor, is_train: bool = False) -> float:
+        return self.forward(X, is_train=is_train)
 
     def __add__(self, other: Layer | Self) -> Self:
         if isinstance(other, Layer):
             self.add(other)
         elif isinstance(other, Self):
             for layer in other.layers:
                 self.add(layer)
         else:
             raise TypeError(
                 "Unsupported operand type(s) for +: '{}' and '{}'".format(
                     type(self).__name__, type(other).__name__
                 )
             )
-        if self.optimizer is not None:
-            self.set_optimizer(self.optimizer)
-        if self.loss_func_ is not None:
-            self.set_loss(self.loss_func_)
 
         return self
 
+    def __getitem__(self, index: int) -> Tuple[str, Layer]:
+        return self.layers[index]
+
     def __str__(self) -> str:
         return super().__str__()
-
-    def __repr__(self) -> str:
-        rep = f"{type(self).__name__} Configuration\n"
-        rep += "-" * 70 + "\n"
-        for name, layer in self.layers:
-            rep += f"({name}) {repr(layer)}\n"
-
-        w_size, b_size = self.param_size
-        rep += f"\nTotal Layers: {len(self.layers)}"
-        rep += f"\nTotal Params: ({w_size:,} weights, {b_size:,} biases)"
-        rep += f" -> {w_size + b_size:,}\n"
-        rep += "-" * 70
-        return rep
```

### Comparing `luma-ml-0.7.1/luma/neural/loss.py` & `luma-ml-0.7.2/luma/neural/loss.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 import numpy as np
 
 from luma.interface.typing import Matrix
 from luma.neural.base import Loss
 
 
-__all__ = ("SoftmaxLoss", "CrossEntropyLoss", "MSELoss")
+__all__ = ("CrossEntropy", "BinaryCrossEntropy", "MSELoss")
 
 
-class SoftmaxLoss(Loss):
+class CrossEntropy(Loss):
     """
     Combines the softmax activation and cross-entropy loss into
     a single class, which is commonly used for multi-class
     classification problems. This loss function is particularly
     useful when the classes are mutually exclusive.
 
     This class assumes the true and predicted target values
     are one-hot encoded.
     """
 
-    def __init__(self) -> None:
+    def __init__(self):
         super().__init__()
 
+    def _softmax(self, y_pred: Matrix) -> Matrix:
+        exp_shift = np.exp(y_pred - np.max(y_pred, axis=1, keepdims=True))
+        softmax_out = exp_shift / np.sum(exp_shift, axis=1, keepdims=True)
+
+        return softmax_out
+
     def loss(self, y_true: Matrix, y_pred: Matrix) -> float:
-        m = y_true.shape[0]
-        y_pred = self._clip(y_pred)
-        loss = -np.sum(y_true * np.log(y_pred)) / m
+        softmax_probs = self._softmax(y_pred)
+        clipped_probs = np.clip(softmax_probs, self.epsilon, 1.0)
+
+        loss = -np.sum(y_true * np.log(clipped_probs)) / y_true.shape[0]
         return loss
 
     def grad(self, y_true: Matrix, y_pred: Matrix) -> Matrix:
-        m = y_true.shape[0]
-        y_pred = self._clip(y_pred)
-        grad = (y_pred - y_true) / m
+        softmax_probs = self._softmax(y_pred)
+        grad = (softmax_probs - y_true) / y_true.shape[0]
         return grad
 
 
-class CrossEntropyLoss(Loss):
+class BinaryCrossEntropy(Loss):
     """
     Computes the cross entropy loss between true labels and
-    predicted probabilities, which is widely used for `binary`
+    predicted probabilities, which is widely used for binary
     classification problems.
 
     This class assumes the true and predicted target values
     are one-hot encoded.
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def loss(self, y_true: Matrix, y_pred: Matrix) -> float:
+    def _sigmoid(self, z: Matrix) -> Matrix:
+        return 1 / (1 + np.exp(-z))
+
+    def loss(self, y_true: Matrix, y_predZ: Matrix) -> float:
         m = y_true.shape[0]
-        y_pred = self._clip(y_pred)
+        y_pred = self._sigmoid(y_predZ)
+        y_pred = np.clip(y_pred, self.epsilon, 1 - self.epsilon)
+
         loss = -np.sum(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
         loss /= m
         return loss
 
-    def grad(self, y_true: Matrix, y_pred: Matrix) -> Matrix:
+    def grad(self, y_true: Matrix, y_predZ: Matrix) -> Matrix:
         m = y_true.shape[0]
-        y_pred = self._clip(y_pred)
-        return (y_pred - y_true) / (y_pred * (1 - y_pred)) / m
+        y_pred = self._sigmoid(y_predZ)
+        return (y_pred - y_true) / m
 
 
 class MSELoss(Loss):
     """
     Calculates the mean squared error between the predicted values
     and the true values, typically used for regression problems.
     Mean squared error is a common measure of the accuracy of a regression
```

### Comparing `luma-ml-0.7.1/luma/neural/optimizer.py` & `luma-ml-0.7.2/luma/neural/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,19 @@
         super().__init__()
         self.learning_rate = learning_rate
 
         self.set_param_ranges({"learning_rate": ("0<,+inf", None)})
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
     def _update_weights(self, W: Tensor, dW: Tensor) -> Tensor:
         updated = []
         for w, grad_w in zip(W, dW):
@@ -57,15 +61,19 @@
 
         self.set_param_ranges(
             {"learning_rate": ("0<,+inf", None), "momentum": ("0,1", None)}
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
     def _update_weights(self, W: Tensor, dW: Tensor) -> Tensor:
         if self.vel_weights is None:
             self.vel_weights = [np.zeros_like(w) for w in W]
@@ -107,15 +115,19 @@
 
         self.set_param_ranges(
             {"learning_rate": ("0<,+inf", None), "decay_rate": ("0,1", None)}
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
     def _update_weights(self, W: Tensor, dW: Tensor) -> Tensor:
         if self.sq_grad_weights is None:
             self.sq_grad_weights = [np.zeros_like(w) for w in W]
@@ -178,15 +190,19 @@
                 "beta_2": ("0,1", None),
                 "epsilon": ("0<,1", None),
             }
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         if not (weights is None and biases is None):
             self.t += 1
 
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
@@ -238,15 +254,19 @@
         self.grad_accum_weights = None
         self.grad_accum_biases = None
 
         self.set_param_ranges({"learning_rate": ("0<,+inf", None)})
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
     def _update_weights(self, W: Tensor, dW: Tensor) -> Tensor:
         if self.grad_accum_weights is None:
             self.grad_accum_weights = [np.zeros_like(w) for w in W]
@@ -285,15 +305,19 @@
         self.accum_grads_b = None
         self.accum_updates_b = None
 
         self.set_param_ranges({"rho": ("0,+inf", None), "epsilon": ("0<,1", None)})
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
     def _update_weights(self, W: Tensor, dW: Tensor) -> Tensor:
         if self.accum_grads_w is None:
             self.accum_grads_w = [np.zeros_like(w) for w in W]
@@ -372,15 +396,19 @@
                 "beta_2": ("0,1", None),
                 "epsilon": ("0<,1", None),
             }
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         if not (weights is None and biases is None):
             self.t += 1
 
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
@@ -453,15 +481,19 @@
                 "epsilon": ("0<,1", None),
                 "weight_decay": ("0,1", None),
             }
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         if not (weights is None and biases is None):
             self.t += 1
 
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
 
@@ -536,15 +568,19 @@
                 "beta_2": ("0,1", None),
                 "epsilon": ("0<,1", None),
             }
         )
         self.check_param_ranges()
 
     def update(
-        self, weights: Tensor, biases: Tensor, grad_weights: Tensor, grad_biases: Tensor
+        self,
+        weights: Tensor,
+        biases: Tensor,
+        grad_weights: Tensor,
+        grad_biases: Tensor,
     ) -> Tuple[Tensor, Tensor]:
         if not (weights is None and biases is None):
             self.t += 1
 
         super().update(weights, biases, grad_weights, grad_biases)
         return self.updated_weights, self.updated_biases
```

### Comparing `luma-ml-0.7.1/luma/neural/single.py` & `luma-ml-0.7.2/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/pipe/pipeline.py` & `luma-ml-0.7.2/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/preprocessing/encoder.py` & `luma-ml-0.7.2/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/preprocessing/imputer.py` & `luma-ml-0.7.2/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/preprocessing/outlier.py` & `luma-ml-0.7.2/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/preprocessing/scaler.py` & `luma-ml-0.7.2/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/reduction/linear.py` & `luma-ml-0.7.2/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/reduction/manifold.py` & `luma-ml-0.7.2/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/reduction/selection.py` & `luma-ml-0.7.2/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/general.py` & `luma-ml-0.7.2/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/linear.py` & `luma-ml-0.7.2/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/neighbors.py` & `luma-ml-0.7.2/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/poly.py` & `luma-ml-0.7.2/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/robust.py` & `luma-ml-0.7.2/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/svm.py` & `luma-ml-0.7.2/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/regressor/tree.py` & `luma-ml-0.7.2/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/visual/eda.py` & `luma-ml-0.7.2/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma/visual/evaluation.py` & `luma-ml-0.7.2/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.1/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.2/luma_ml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
-Home-page: https://github.com/ChanLumerico/LUMA
+Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.13k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,15 +108,15 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.1</td>
+                    <td>0.7.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
                     <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.1 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.2 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
-github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
+github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.07k-red][GitHub code size in bytes][Code Style]
+5.13k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.1
+Latest Version 0.7.2
 Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.1/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.2/luma_ml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 luma/metric/distance.py
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
-luma/neural/activation.py
 luma/neural/base.py
 luma/neural/init.py
 luma/neural/layer.py
 luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
@@ -62,9 +61,8 @@
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
 test/__local__.py
-test/__test.py
-test/_mlp.py
+test/__test.py
```

### Comparing `luma-ml-0.7.1/setup.py` & `luma-ml-0.7.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.1",
+    version="0.7.2",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ChanLumerico/LUMA",
+    url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.12",
-    install_requires=["numpy", "scipy", "pandas", "matplotlib", "seaborn"],
+    install_requires=[
+        "numpy",
+        "scipy",
+        "pandas",
+        "matplotlib",
+        "seaborn",
+    ],
 )
```

