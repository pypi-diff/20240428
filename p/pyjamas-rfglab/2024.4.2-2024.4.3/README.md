# Comparing `tmp/pyjamas-rfglab-2024.4.2.tar.gz` & `tmp/pyjamas-rfglab-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjamas-rfglab-2024.4.2.tar", last modified: Wed Apr 24 16:49:57 2024, max compression
+gzip compressed data, was "pyjamas-rfglab-2024.4.3.tar", last modified: Sat Apr 27 21:11:42 2024, max compression
```

## Comparing `pyjamas-rfglab-2024.4.2.tar` & `pyjamas-rfglab-2024.4.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.937870 pyjamas-rfglab-2024.4.2/
--rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.4.2/MANIFEST.in
--rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-04-24 16:49:57.936980 pyjamas-rfglab-2024.4.2/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.865958 pyjamas-rfglab-2024.4.2/pyjamas/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.4.2/pyjamas/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.890367 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/adjustcontrast.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchanalysis.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12069 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchflatfield.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchprojectconcat.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6823 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchresize.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifierdialogABC.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifiertype.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandnpropagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/findseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/logregression.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/matplotlibdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/measurepoly.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/neuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/nonmax_suppr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/propagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/rescuneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/svm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/textdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/texteditdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/timepoints.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dragdropmainwindow.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.892195 pyjamas-rfglab-2024.4.2/pyjamas/external/
--rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.4.2/pyjamas/external/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.4.2/pyjamas/external/pascal_voc_io.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/orthogonalviewswindow.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52457 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjscore.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjseventfilter.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjsthreads.py
--rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.4.2/pyjamas/pyjamas.tif
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.896294 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/
--rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rannotation.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rpolyline.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rvector2d.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.910721 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcallback.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbabout.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbannotations.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    82216 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbbatchprocess.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbclassifiers.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52357 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbio.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbmeasure.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcboptions.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbplugins.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.913529 pyjamas-rfglab-2024.4.2/pyjamas/rimage/
--rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/csgraph.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimcore.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.928825 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/classifier_types.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rawimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_sog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimlr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrescunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimsvm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.930957 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/
--rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/base.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.4.2/pyjamas/rutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.932304 pyjamas-rfglab-2024.4.2/pyjamas/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/conftest.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.935326 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7505 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/pjsfixtures.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_image.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16118 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_io.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.936321 pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     2562 2024-04-24 16:49:57.000000 pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-04-24 16:49:57.938007 pyjamas-rfglab-2024.4.2/setup.cfg
--rw-r--r--   0 rodrigo    (501) staff       (20)     3061 2024-04-17 16:34:42.000000 pyjamas-rfglab-2024.4.2/setup.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.677949 pyjamas-rfglab-2024.4.3/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.4.3/MANIFEST.in
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-04-27 21:11:42.677064 pyjamas-rfglab-2024.4.3/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.3/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.596897 pyjamas-rfglab-2024.4.3/pyjamas/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.4.3/pyjamas/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.3/pyjamas/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.621135 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/adjustcontrast.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchanalysis.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12069 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchflatfield.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchprojectconcat.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6823 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchresize.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/classifierdialogABC.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/classifiertype.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/expandnpropagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/expandseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/findseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/logregression.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/matplotlibdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/measurepoly.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/neuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/nonmax_suppr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/propagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/rescuneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/svm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/textdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/texteditdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dialogs/timepoints.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/dragdropmainwindow.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.623098 pyjamas-rfglab-2024.4.3/pyjamas/external/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.4.3/pyjamas/external/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.4.3/pyjamas/external/pascal_voc_io.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/orthogonalviewswindow.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52457 2024-04-27 21:10:45.000000 pyjamas-rfglab-2024.4.3/pyjamas/pjscore.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.3/pyjamas/pjseventfilter.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/pjsthreads.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.4.3/pyjamas/pyjamas.tif
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.626886 pyjamas-rfglab-2024.4.3/pyjamas/rannotations/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.4.3/pyjamas/rannotations/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rannotation.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rpolyline.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rvector2d.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.641466 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcallback.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbabout.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbannotations.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    82216 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbbatchprocess.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbclassifiers.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52357 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbio.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbmeasure.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcboptions.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbplugins.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.644988 pyjamas-rfglab-2024.4.3/pyjamas/rimage/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/csgraph.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimcore.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.669021 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/classifier_types.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_rawimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_sog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimlr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimrescunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimsvm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.671372 pyjamas-rfglab-2024.4.3/pyjamas/rplugins/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.3/pyjamas/rplugins/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.4.3/pyjamas/rplugins/base.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.4.3/pyjamas/rutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.673030 pyjamas-rfglab-2024.4.3/pyjamas/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/conftest.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.675819 pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7505 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/pjsfixtures.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/test_image.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16118 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/test_io.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-27 21:11:42.676557 pyjamas-rfglab-2024.4.3/pyjamas_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2562 2024-04-27 21:11:41.000000 pyjamas-rfglab-2024.4.3/pyjamas_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-04-27 21:11:42.678142 pyjamas-rfglab-2024.4.3/setup.cfg
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3170 2024-04-27 21:10:45.000000 pyjamas-rfglab-2024.4.3/setup.py
```

### Comparing `pyjamas-rfglab-2024.4.2/PKG-INFO` & `pyjamas-rfglab-2024.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjamas-rfglab
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: PyJAMAS is Just A More Awesome SIESTA
 Home-page: https://bitbucket.org/rfg_lab/pyjamas
 Author: Rodrigo Fernandez-Gonzalez
 Author-email: rodrigo.fernandez.gonzalez@utoronto.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjamas-rfglab-2024.4.2/README.md` & `pyjamas-rfglab-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/LICENSE` & `pyjamas-rfglab-2024.4.3/pyjamas/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/adjustcontrast.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/adjustcontrast.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchanalysis.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchanalysis.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchflatfield.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchflatfield.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchprojectconcat.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchprojectconcat.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchresize.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/batchresize.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifierdialogABC.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/classifierdialogABC.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifiertype.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/classifiertype.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandnpropagateseeds.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/expandnpropagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandseeds.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/expandseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/findseeds.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/findseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/logregression.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/logregression.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/matplotlibdialog.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/matplotlibdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/measurepoly.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/measurepoly.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/neuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/neuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/nonmax_suppr.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/nonmax_suppr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/propagateseeds.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/propagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/rescuneuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/rescuneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/svm.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/svm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/textdialog.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/textdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/texteditdialog.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/texteditdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/timepoints.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dialogs/timepoints.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/dragdropmainwindow.py` & `pyjamas-rfglab-2024.4.3/pyjamas/dragdropmainwindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/external/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/external/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/external/pascal_voc_io.py` & `pyjamas-rfglab-2024.4.3/pyjamas/external/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/orthogonalviewswindow.py` & `pyjamas-rfglab-2024.4.3/pyjamas/orthogonalviewswindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/pjscore.py` & `pyjamas-rfglab-2024.4.3/pyjamas/pjscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     livewire_gaussian_sigma: float = 0.
     balloon_crop_size: int = 50  # crop size used to inflate balloons
     livewire_shortest_path_fn = tuple(rimcore.rimage.livewire_shortest_path_fns.values())[0]  # fn to calculate shortest path between two pixels
 
     undo_stack_size: int = 500
 
     # Read version.
-    __version__: str = '2024.4.2'
+    __version__: str = '2024.4.3'
 
     def __init__(self):
         self.initData()  # Initialize object variables.
         self.setupUI()  # Build the GUI.
 
     def setupUI(self):
         self.app = QtWidgets.QApplication(sys.argv)
```

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/pjseventfilter.py` & `pyjamas-rfglab-2024.4.3/pyjamas/pjseventfilter.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/pjsthreads.py` & `pyjamas-rfglab-2024.4.3/pyjamas/pjsthreads.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/pyjamas.tif` & `pyjamas-rfglab-2024.4.3/pyjamas/pyjamas.tif`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rannotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rannotation.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rannotation.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rpolyline.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rpolyline.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rvector2d.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rannotations/rvector2d.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcallback.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcallback.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbabout.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbabout.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbannotations.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbannotations.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbbatchprocess.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbbatchprocess.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbclassifiers.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbclassifiers.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbimage.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbio.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbio.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbmeasure.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbmeasure.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcboptions.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcboptions.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbplugins.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rcallbacks/rcbplugins.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/csgraph.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/csgraph.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimcore.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimcore.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchclassifier.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchml.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchneuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/batchrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rawimage.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_rawimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_sog.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/featurecalculator_sog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimclassifier.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimlr.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimlr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimml.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimneuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrescunet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimrescunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimsvm.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimsvm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimunet.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimml/rimunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimutils.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rimage/rimutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rplugins/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rplugins/base.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rplugins/base.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/rutils.py` & `pyjamas-rfglab-2024.4.3/pyjamas/rutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/tests/__init__.py` & `pyjamas-rfglab-2024.4.3/pyjamas/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/tests/conftest.py` & `pyjamas-rfglab-2024.4.3/pyjamas/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/pjsfixtures.py` & `pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/pjsfixtures.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_image.py` & `pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_io.py` & `pyjamas-rfglab-2024.4.3/pyjamas/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/SOURCES.txt` & `pyjamas-rfglab-2024.4.3/pyjamas_rfglab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.2/setup.py` & `pyjamas-rfglab-2024.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     install_requires=["ipywidgets>=8.0.4",
                       "joblib>=1.2.0", "lxml>=4.9.2", "matplotlib>=3.7.1",
                       "nbformat>=5.7.0",
                       "networkx>=2.8.4",
                       "numba==0.57.1",  ## 0.59.1 fails with "Measure polylines" 2024/04/17
                       "numpy==1.23.5",  ## 1.24.3 has an error when exporting mat files.
                       "opencv-python-headless==4.6.0.66",  ## greater than this will not work on Big Sur 2024/04/17
-                      "pandas>=1.5.3", "pyqt6==6.5.0", "scikit-image>=0.21.0",
+                      "pandas>=1.5.3",
+                      "pyqt6==6.4.2", ## 6.4.2 is the last version that works in Windows 11 2024/04/27
+                      "scikit-image>=0.21.0",
                       "scikit-learn>=1.2.2",
                       "scipy>=1.10.1", "seaborn>=0.13.0", "setuptools>=67.8.0",
                       "shapely>=2.0.1",
                       "tensorflow>=2.11.0"],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
```

