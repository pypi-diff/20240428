# Comparing `tmp/ibeam-0.5.2.tar.gz` & `tmp/ibeam-0.5.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibeam-0.5.2.tar", last modified: Sun Apr 28 04:07:53 2024, max compression
+gzip compressed data, was "ibeam-0.5.2rc4.tar", last modified: Sun Apr 28 04:15:36 2024, max compression
```

## Comparing `ibeam-0.5.2.tar` & `ibeam-0.5.2rc4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.417612 ibeam-0.5.2/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    11527 2024-04-28 04:07:53.415779 ibeam-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    10623 2024-04-01 05:52:03.000000 ibeam-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.339253 ibeam-0.5.2/ibeam/
--rw-rw-rw-   0        0        0       74 2024-04-28 04:06:51.000000 ibeam-0.5.2/ibeam/__init__.py
--rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.2/ibeam/config.py
--rw-rw-rw-   0        0        0     6781 2024-04-01 06:33:58.000000 ibeam-0.5.2/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.366470 ibeam-0.5.2/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.2/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/gateway_client.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.383466 ibeam-0.5.2/ibeam/src/handlers/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:52:09.000000 ibeam-0.5.2/ibeam/src/handlers/__init__.py
--rw-rw-rw-   0        0        0    13148 2024-04-01 06:33:58.000000 ibeam-0.5.2/ibeam/src/handlers/http_handler.py
--rw-rw-rw-   0        0        0     1500 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/handlers/inputs_handler.py
--rw-rw-rw-   0        0        0    20297 2024-04-15 03:27:57.000000 ibeam-0.5.2/ibeam/src/handlers/login_handler.py
--rw-rw-rw-   0        0        0     5236 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/handlers/process_handler.py
--rw-rw-rw-   0        0        0     6567 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/handlers/secrets_handler.py
--rw-rw-rw-   0        0        0    10485 2024-04-01 06:37:20.000000 ibeam-0.5.2/ibeam/src/handlers/strategy_handler.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.2/ibeam/src/health_server.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.390490 ibeam-0.5.2/ibeam/src/login/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:52:15.000000 ibeam-0.5.2/ibeam/src/login/__init__.py
--rw-rw-rw-   0        0        0     6582 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/login/driver.py
--rw-rw-rw-   0        0        0     4906 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/login/targets.py
--rw-rw-rw-   0        0        0     2292 2024-04-28 04:04:24.000000 ibeam-0.5.2/ibeam/src/logs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.402597 ibeam-0.5.2/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/notification_resend_handler.py
--rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.2/ibeam/src/two_fa_selector.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.409875 ibeam-0.5.2/ibeam/src/utils/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:53:41.000000 ibeam-0.5.2/ibeam/src/utils/__init__.py
--rw-rw-rw-   0        0        0      305 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/utils/py_utils.py
--rw-rw-rw-   0        0        0     1454 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/utils/selenium_utils.py
--rw-rw-rw-   0        0        0     7784 2024-04-01 06:19:12.000000 ibeam-0.5.2/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.413385 ibeam-0.5.2/ibeam.egg-info/
--rw-rw-rw-   0        0        0    11527 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-28 04:07:53.418636 ibeam-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1387 2024-04-28 04:06:41.000000 ibeam-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.240797 ibeam-0.5.2rc4/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.2rc4/LICENSE
+-rw-rw-rw-   0        0        0    11530 2024-04-28 04:15:36.238801 ibeam-0.5.2rc4/PKG-INFO
+-rw-rw-rw-   0        0        0    10623 2024-04-01 05:52:03.000000 ibeam-0.5.2rc4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.155801 ibeam-0.5.2rc4/ibeam/
+-rw-rw-rw-   0        0        0       78 2024-04-28 04:15:29.000000 ibeam-0.5.2rc4/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.2rc4/ibeam/config.py
+-rw-rw-rw-   0        0        0     6781 2024-04-01 06:33:58.000000 ibeam-0.5.2rc4/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.187801 ibeam-0.5.2rc4/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.2rc4/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/gateway_client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.206802 ibeam-0.5.2rc4/ibeam/src/handlers/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:09.000000 ibeam-0.5.2rc4/ibeam/src/handlers/__init__.py
+-rw-rw-rw-   0        0        0    13148 2024-04-01 06:33:58.000000 ibeam-0.5.2rc4/ibeam/src/handlers/http_handler.py
+-rw-rw-rw-   0        0        0     1500 2023-09-07 18:11:53.000000 ibeam-0.5.2rc4/ibeam/src/handlers/inputs_handler.py
+-rw-rw-rw-   0        0        0    20297 2024-04-15 03:27:57.000000 ibeam-0.5.2rc4/ibeam/src/handlers/login_handler.py
+-rw-rw-rw-   0        0        0     5236 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/handlers/process_handler.py
+-rw-rw-rw-   0        0        0     6567 2023-09-07 18:11:53.000000 ibeam-0.5.2rc4/ibeam/src/handlers/secrets_handler.py
+-rw-rw-rw-   0        0        0    10485 2024-04-01 06:37:20.000000 ibeam-0.5.2rc4/ibeam/src/handlers/strategy_handler.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.2rc4/ibeam/src/health_server.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.213803 ibeam-0.5.2rc4/ibeam/src/login/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:15.000000 ibeam-0.5.2rc4/ibeam/src/login/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/login/driver.py
+-rw-rw-rw-   0        0        0     4906 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/login/targets.py
+-rw-rw-rw-   0        0        0     2292 2024-04-28 04:04:24.000000 ibeam-0.5.2rc4/ibeam/src/logs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.226804 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.2rc4/ibeam/src/two_fa_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.233803 ibeam-0.5.2rc4/ibeam/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:53:41.000000 ibeam-0.5.2rc4/ibeam/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-09-07 18:11:53.000000 ibeam-0.5.2rc4/ibeam/src/utils/py_utils.py
+-rw-rw-rw-   0        0        0     1454 2023-09-07 18:11:53.000000 ibeam-0.5.2rc4/ibeam/src/utils/selenium_utils.py
+-rw-rw-rw-   0        0        0     7784 2024-04-01 06:19:12.000000 ibeam-0.5.2rc4/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:15:36.236801 ibeam-0.5.2rc4/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    11530 2024-04-28 04:15:35.000000 ibeam-0.5.2rc4/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2024-04-28 04:15:36.000000 ibeam-0.5.2rc4/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:15:35.000000 ibeam-0.5.2rc4/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-04-28 04:15:35.000000 ibeam-0.5.2rc4/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-28 04:15:35.000000 ibeam-0.5.2rc4/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2024-04-28 04:15:36.241802 ibeam-0.5.2rc4/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2024-04-28 04:06:41.000000 ibeam-0.5.2rc4/setup.py
```

### Comparing `ibeam-0.5.2/LICENSE` & `ibeam-0.5.2rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/PKG-INFO` & `ibeam-0.5.2rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.2
+Version: 0.5.2rc4
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.2 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc4 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.5.2/README.md` & `ibeam-0.5.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/config.py` & `ibeam-0.5.2rc4/ibeam/config.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/ibeam_starter.py` & `ibeam-0.5.2rc4/ibeam/ibeam_starter.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/gateway_client.py` & `ibeam-0.5.2rc4/ibeam/src/gateway_client.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/http_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/inputs_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/login_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/login_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/process_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/process_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/secrets_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/secrets_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/handlers/strategy_handler.py` & `ibeam-0.5.2rc4/ibeam/src/handlers/strategy_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/health_server.py` & `ibeam-0.5.2rc4/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/login/driver.py` & `ibeam-0.5.2rc4/ibeam/src/login/driver.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/login/targets.py` & `ibeam-0.5.2rc4/ibeam/src/login/targets.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/logs.py` & `ibeam-0.5.2rc4/ibeam/src/logs.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/two_fa_handlers/notification_resend_handler.py` & `ibeam-0.5.2rc4/ibeam/src/two_fa_handlers/notification_resend_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/two_fa_selector.py` & `ibeam-0.5.2rc4/ibeam/src/two_fa_selector.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/utils/selenium_utils.py` & `ibeam-0.5.2rc4/ibeam/src/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam/src/var.py` & `ibeam-0.5.2rc4/ibeam/src/var.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/ibeam.egg-info/PKG-INFO` & `ibeam-0.5.2rc4/ibeam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.2
+Version: 0.5.2rc4
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.2 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc4 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.5.2/ibeam.egg-info/SOURCES.txt` & `ibeam-0.5.2rc4/ibeam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2/setup.py` & `ibeam-0.5.2rc4/setup.py`

 * *Files identical despite different names*

