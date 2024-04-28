# Comparing `tmp/pypayment-1.7.8.tar.gz` & `tmp/pypayment-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypayment-1.7.8.tar", last modified: Tue Dec  5 11:49:59 2023, max compression
+gzip compressed data, was "pypayment-1.7.9.tar", last modified: Mon Dec 11 17:59:19 2023, max compression
```

## Comparing `pypayment-1.7.8.tar` & `pypayment-1.7.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.997244 pypayment-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-05 11:49:58.997244 pypayment-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-12-05 11:49:48.000000 pypayment-1.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.993244 pypayment-1.7.8/pypayment/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.993244 pypayment-1.7.8/pypayment/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/enums/commission.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/enums/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.997244 pypayment-1.7.8/pypayment/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14391 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/betatransfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/lava.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/payok.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/qiwi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-12-05 11:49:48.000000 pypayment-1.7.8/pypayment/providers/yoomoney.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.997244 pypayment-1.7.8/pypayment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-05 11:49:58.000000 pypayment-1.7.8/pypayment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-05 11:49:58.000000 pypayment-1.7.8/pypayment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 11:49:58.000000 pypayment-1.7.8/pypayment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-05 11:49:58.000000 pypayment-1.7.8/pypayment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-05 11:49:58.000000 pypayment-1.7.8/pypayment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-05 11:49:48.000000 pypayment-1.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-05 11:49:58.997244 pypayment-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-05 11:49:48.000000 pypayment-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 11:49:58.997244 pypayment-1.7.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/test_lava.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/test_payok.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/test_qiwi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-05 11:49:48.000000 pypayment-1.7.8/test/test_yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.351702 pypayment-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-11 17:59:19.351702 pypayment-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-12-11 17:59:10.000000 pypayment-1.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.347702 pypayment-1.7.9/pypayment/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.347702 pypayment-1.7.9/pypayment/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/enums/commission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/enums/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.347702 pypayment-1.7.9/pypayment/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14391 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/betatransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/lava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/payok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-12-11 17:59:10.000000 pypayment-1.7.9/pypayment/providers/yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.351702 pypayment-1.7.9/pypayment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-11 17:59:19.000000 pypayment-1.7.9/pypayment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-11 17:59:19.000000 pypayment-1.7.9/pypayment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 17:59:19.000000 pypayment-1.7.9/pypayment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-11 17:59:19.000000 pypayment-1.7.9/pypayment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-11 17:59:19.000000 pypayment-1.7.9/pypayment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-11 17:59:10.000000 pypayment-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-11 17:59:19.351702 pypayment-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-11 17:59:10.000000 pypayment-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:59:19.351702 pypayment-1.7.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/test_lava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/test_payok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/test_qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-11 17:59:10.000000 pypayment-1.7.9/test/test_yoomoney.py
```

### Comparing `pypayment-1.7.8/PKG-INFO` & `pypayment-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.7.8
+Version: 1.7.9
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.7.8 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.9 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pypayment-1.7.8/README.md` & `pypayment-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/__init__.py` & `pypayment-1.7.9/pypayment/__init__.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/exceptions.py` & `pypayment-1.7.9/pypayment/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/payment.py` & `pypayment-1.7.9/pypayment/payment.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/providers/betatransfer.py` & `pypayment-1.7.9/pypayment/providers/betatransfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,23 +118,23 @@
         max_amount=50000
     )
     """YooMoney payment type."""
     QIWI = BetaTransferGateway(
         name="Qiwi",
         currency=BetaTransferCurrency.RUB,
         commission_in_percent=12,
-        min_amount=300,
+        min_amount=100,
         max_amount=50000
     )
     """Qiwi payment type."""
     QIWI_CARD = BetaTransferGateway(
         name="Qiwi2",
         currency=BetaTransferCurrency.RUB,
         commission_in_percent=12,
-        min_amount=100,
+        min_amount=500,
         max_amount=50000
     )
     """Qiwi Card payment type."""
     RUB_CARD = BetaTransferGateway(
         name="Card",
         currency=BetaTransferCurrency.RUB,
         commission_in_percent=12,
```

### Comparing `pypayment-1.7.8/pypayment/providers/lava.py` & `pypayment-1.7.9/pypayment/providers/lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/providers/payok.py` & `pypayment-1.7.9/pypayment/providers/payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/providers/qiwi.py` & `pypayment-1.7.9/pypayment/providers/qiwi.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment/providers/yoomoney.py` & `pypayment-1.7.9/pypayment/providers/yoomoney.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/pypayment.egg-info/PKG-INFO` & `pypayment-1.7.9/pypayment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.7.8
+Version: 1.7.9
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.7.8 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.9 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pypayment-1.7.8/pypayment.egg-info/SOURCES.txt` & `pypayment-1.7.9/pypayment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/setup.py` & `pypayment-1.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/test/test_lava.py` & `pypayment-1.7.9/test/test_lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/test/test_payok.py` & `pypayment-1.7.9/test/test_payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/test/test_qiwi.py` & `pypayment-1.7.9/test/test_qiwi.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.8/test/test_yoomoney.py` & `pypayment-1.7.9/test/test_yoomoney.py`

 * *Files identical despite different names*

