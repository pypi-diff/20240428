# Comparing `tmp/nue-0.0.6.tar.gz` & `tmp/nue-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nue-0.0.6.tar", last modified: Fri Apr 26 21:57:18 2024, max compression
+gzip compressed data, was "nue-0.0.7.tar", last modified: Sun Apr 28 02:35:47 2024, max compression
```

## Comparing `nue-0.0.6.tar` & `nue-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:57:18.949522 nue-0.0.6/
--rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.6/LICENSE
--rw-r--r--   0 juanvera   (501) staff       (20)     1070 2024-04-26 21:57:18.949173 nue-0.0.6/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)     1572 2024-04-26 21:49:31.000000 nue-0.0.6/README.md
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:57:18.947490 nue-0.0.6/models/
--rw-r--r--   0 juanvera   (501) staff       (20)      924 2024-04-26 15:20:27.000000 nue-0.0.6/models/__init__.py
--rw-r--r--   0 juanvera   (501) staff       (20)     3538 2024-04-26 12:46:29.000000 nue-0.0.6/models/linreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     4000 2024-04-26 02:56:06.000000 nue-0.0.6/models/logreg.py
--rw-r--r--   0 juanvera   (501) staff       (20)     6694 2024-04-26 12:51:41.000000 nue-0.0.6/models/nn.py
-drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-26 21:57:18.948667 nue-0.0.6/nue.egg-info/
--rw-r--r--   0 juanvera   (501) staff       (20)     1070 2024-04-26 21:57:18.000000 nue-0.0.6/nue.egg-info/PKG-INFO
--rw-r--r--   0 juanvera   (501) staff       (20)      226 2024-04-26 21:57:18.000000 nue-0.0.6/nue.egg-info/SOURCES.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-26 21:57:18.000000 nue-0.0.6/nue.egg-info/dependency_links.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-26 21:57:18.000000 nue-0.0.6/nue.egg-info/requires.txt
--rw-r--r--   0 juanvera   (501) staff       (20)        7 2024-04-26 21:57:18.000000 nue-0.0.6/nue.egg-info/top_level.txt
--rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-26 21:57:18.949596 nue-0.0.6/setup.cfg
--rw-r--r--   0 juanvera   (501) staff       (20)     1010 2024-04-26 21:56:55.000000 nue-0.0.6/setup.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-28 02:35:47.071931 nue-0.0.7/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1062 2024-04-22 16:56:55.000000 nue-0.0.7/LICENSE
+-rw-r--r--   0 juanvera   (501) staff       (20)     1070 2024-04-28 02:35:47.071688 nue-0.0.7/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)     1808 2024-04-27 02:26:41.000000 nue-0.0.7/README.md
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-28 02:35:47.067763 nue-0.0.7/models/
+-rw-r--r--   0 juanvera   (501) staff       (20)      924 2024-04-26 15:20:27.000000 nue-0.0.7/models/__init__.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     3538 2024-04-26 12:46:29.000000 nue-0.0.7/models/linreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     4000 2024-04-26 02:56:06.000000 nue-0.0.7/models/logreg.py
+-rw-r--r--   0 juanvera   (501) staff       (20)     6704 2024-04-28 02:34:28.000000 nue-0.0.7/models/nn.py
+drwxr-xr-x   0 juanvera   (501) staff       (20)        0 2024-04-28 02:35:47.071118 nue-0.0.7/nue.egg-info/
+-rw-r--r--   0 juanvera   (501) staff       (20)     1070 2024-04-28 02:35:47.000000 nue-0.0.7/nue.egg-info/PKG-INFO
+-rw-r--r--   0 juanvera   (501) staff       (20)      226 2024-04-28 02:35:47.000000 nue-0.0.7/nue.egg-info/SOURCES.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        1 2024-04-28 02:35:47.000000 nue-0.0.7/nue.egg-info/dependency_links.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       24 2024-04-28 02:35:47.000000 nue-0.0.7/nue.egg-info/requires.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)        7 2024-04-28 02:35:47.000000 nue-0.0.7/nue.egg-info/top_level.txt
+-rw-r--r--   0 juanvera   (501) staff       (20)       38 2024-04-28 02:35:47.072043 nue-0.0.7/setup.cfg
+-rw-r--r--   0 juanvera   (501) staff       (20)     1010 2024-04-28 02:35:24.000000 nue-0.0.7/setup.py
```

### Comparing `nue-0.0.6/LICENSE` & `nue-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nue-0.0.6/PKG-INFO` & `nue-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.6
+Version: 0.0.7
 Summary: A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. 
 Home-page: https://vxnuaj.github.io/nue/
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.6/models/__init__.py` & `nue-0.0.7/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.6/models/linreg.py` & `nue-0.0.7/models/linreg.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.6/models/logreg.py` & `nue-0.0.7/models/logreg.py`

 * *Files identical despite different names*

### Comparing `nue-0.0.6/models/nn.py` & `nue-0.0.7/models/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
         """
         Perform a forward pass through the neural network.
 
         :return: The predicted probabilities for each class
         :rtype: numpy.ndarray
         """
         w1, b1, w2, b2 = self.params
-        z1 = np.dot(w1, self.input)
+        z1 = np.dot(w1, self.input) + b1
         a1 = self.ReLU(z1)
-        z2 = np.dot(w2, a1)
+        z2 = np.dot(w2, a1) + b2
         self.pred = self.softmax(z2)
         self.outputs = z1, a1, z2
         return self.pred
     
     def ReLU(self, z):
         """
         Apply the Rectified Linear Unit (ReLU) activation function element-wise to the input.
```

### Comparing `nue-0.0.6/nue.egg-info/PKG-INFO` & `nue-0.0.7/nue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nue
-Version: 0.0.6
+Version: 0.0.7
 Summary: A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. 
 Home-page: https://vxnuaj.github.io/nue/
 Author: vxnuaj
 Author-email: jv.100420@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nue-0.0.6/setup.py` & `nue-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
-DEFAULTV = '0.0.6'
+VERSION = '0.0.7'
+DEFAULTV = '0.0.7'
 DESCRIPTION = 'A deep learning framework sculpted for seamless implementation of models, geared towards entry level learners. '
 
 setup(
     name='nue',
     version= VERSION,
     default_version= DEFAULTV,
     packages=find_packages(exclude = ['examples', 'docs', 'dist', 'test']),
```

