# Comparing `tmp/gym_jiminy_toolbox-1.8.4-py3-none-any.whl.zip` & `tmp/gym_jiminy_toolbox-1.8.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12839 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/py.typed
--rw-r--r--  2.0 unx      272 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/math/__init__.py
--rw-r--r--  2.0 unx     7946 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/math/qhull.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/math/spline.py
--rw-r--r--  2.0 unx      270 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/wrappers/__init__.py
--rw-r--r--  2.0 unx     3053 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
--rw-r--r--  2.0 unx     4921 b- defN 24-Apr-19 21:51 gym_jiminy/toolbox/wrappers/meta_envs.py
--rw-r--r--  2.0 unx      933 b- defN 24-Apr-19 21:52 gym_jiminy_toolbox-1.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 21:52 gym_jiminy_toolbox-1.8.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-19 21:52 gym_jiminy_toolbox-1.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1075 b- defN 24-Apr-19 21:52 gym_jiminy_toolbox-1.8.4.dist-info/RECORD
-12 files, 36932 bytes uncompressed, 10991 bytes compressed:  70.2%
+Zip file size: 12840 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/py.typed
+-rw-r--r--  2.0 unx      272 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/math/__init__.py
+-rw-r--r--  2.0 unx     7946 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/math/qhull.py
+-rw-r--r--  2.0 unx    18359 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/math/spline.py
+-rw-r--r--  2.0 unx      270 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/wrappers/__init__.py
+-rw-r--r--  2.0 unx     3053 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
+-rw-r--r--  2.0 unx     4921 b- defN 24-Apr-28 20:51 gym_jiminy/toolbox/wrappers/meta_envs.py
+-rw-r--r--  2.0 unx      933 b- defN 24-Apr-28 20:52 gym_jiminy_toolbox-1.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 20:52 gym_jiminy_toolbox-1.8.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-28 20:52 gym_jiminy_toolbox-1.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1075 b- defN 24-Apr-28 20:52 gym_jiminy_toolbox-1.8.5.dist-info/RECORD
+12 files, 36932 bytes uncompressed, 10992 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: gym_jiminy/toolbox/wrappers/frame_rate_limiter.py
 Comment: 
 
 Filename: gym_jiminy/toolbox/wrappers/meta_envs.py
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.4.dist-info/METADATA
+Filename: gym_jiminy_toolbox-1.8.5.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.4.dist-info/WHEEL
+Filename: gym_jiminy_toolbox-1.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.4.dist-info/top_level.txt
+Filename: gym_jiminy_toolbox-1.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_toolbox-1.8.4.dist-info/RECORD
+Filename: gym_jiminy_toolbox-1.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gym_jiminy_toolbox-1.8.4.dist-info/METADATA` & `gym_jiminy_toolbox-1.8.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-toolbox
-Version: 1.8.4
+Version: 1.8.5
 Summary: Generic Reinforcement learning toolbox based on Pytorch for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 3 - Alpha
@@ -14,10 +14,10 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<3.13
-Requires-Dist: gym-jiminy ~=1.8.4
+Requires-Dist: gym-jiminy ~=1.8.5
 Requires-Dist: scipy >=1.9.2
```

## Comparing `gym_jiminy_toolbox-1.8.4.dist-info/RECORD` & `gym_jiminy_toolbox-1.8.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 gym_jiminy/toolbox/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gym_jiminy/toolbox/math/__init__.py,sha256=fJBmFKSbDxHTBtWX_dmu5p3xomaazzs5et2dOM1RZbc,272
 gym_jiminy/toolbox/math/qhull.py,sha256=80WmgA_WBoBk-jYpXkSb_J3zO_AteKuWp413hXW4TWk,7946
 gym_jiminy/toolbox/math/spline.py,sha256=ad4rfZy0zyXwZ0mpDzKnsyLOlH2fHXxuqeoz9_sisHk,18359
 gym_jiminy/toolbox/wrappers/__init__.py,sha256=O3pwKYZTi7nFit0IdKV9YhT7dYGjY-O6fIsR6jAPpig,270
 gym_jiminy/toolbox/wrappers/frame_rate_limiter.py,sha256=klhRjr-Ag7VrV7o_pIs80dCRFzRPaEoDpTR3PKEgESY,3053
 gym_jiminy/toolbox/wrappers/meta_envs.py,sha256=ppOkhyZoYW6NO1q4iQi5_8cpq4vaxNttvxGslK39FTo,4921
-gym_jiminy_toolbox-1.8.4.dist-info/METADATA,sha256=lMlqRaDobaWW6WIgwpgO3LtXDRhS5LpNBqybY61tfPQ,933
-gym_jiminy_toolbox-1.8.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gym_jiminy_toolbox-1.8.4.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
-gym_jiminy_toolbox-1.8.4.dist-info/RECORD,,
+gym_jiminy_toolbox-1.8.5.dist-info/METADATA,sha256=doGQAdEb8SI_QX74Ho7We2te5sEAnnZvL4onJa22BGk,933
+gym_jiminy_toolbox-1.8.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gym_jiminy_toolbox-1.8.5.dist-info/top_level.txt,sha256=c6Ipde11Sivat1D9sNj6sn3TCpadD0Qqk9fMzWYQLko,11
+gym_jiminy_toolbox-1.8.5.dist-info/RECORD,,
```

