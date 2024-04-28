# Comparing `tmp/ibeam-0.5.2rc5.tar.gz` & `tmp/ibeam-0.5.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibeam-0.5.2rc5.tar", last modified: Sun Apr 28 04:20:45 2024, max compression
+gzip compressed data, was "ibeam-0.5.2rc6.tar", last modified: Sun Apr 28 04:21:35 2024, max compression
```

## Comparing `ibeam-0.5.2rc5.tar` & `ibeam-0.5.2rc6.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.846143 ibeam-0.5.2rc5/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.2rc5/LICENSE
--rw-rw-rw-   0        0        0    11530 2024-04-28 04:20:45.845144 ibeam-0.5.2rc5/PKG-INFO
--rw-rw-rw-   0        0        0    10623 2024-04-01 05:52:03.000000 ibeam-0.5.2rc5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.764150 ibeam-0.5.2rc5/ibeam/
--rw-rw-rw-   0        0        0       78 2024-04-28 04:20:39.000000 ibeam-0.5.2rc5/ibeam/__init__.py
--rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.2rc5/ibeam/config.py
--rw-rw-rw-   0        0        0     6781 2024-04-01 06:33:58.000000 ibeam-0.5.2rc5/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.792168 ibeam-0.5.2rc5/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.2rc5/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/gateway_client.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.812143 ibeam-0.5.2rc5/ibeam/src/handlers/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:52:09.000000 ibeam-0.5.2rc5/ibeam/src/handlers/__init__.py
--rw-rw-rw-   0        0        0    13148 2024-04-01 06:33:58.000000 ibeam-0.5.2rc5/ibeam/src/handlers/http_handler.py
--rw-rw-rw-   0        0        0     1500 2023-09-07 18:11:53.000000 ibeam-0.5.2rc5/ibeam/src/handlers/inputs_handler.py
--rw-rw-rw-   0        0        0    20297 2024-04-15 03:27:57.000000 ibeam-0.5.2rc5/ibeam/src/handlers/login_handler.py
--rw-rw-rw-   0        0        0     5236 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/handlers/process_handler.py
--rw-rw-rw-   0        0        0     6567 2023-09-07 18:11:53.000000 ibeam-0.5.2rc5/ibeam/src/handlers/secrets_handler.py
--rw-rw-rw-   0        0        0    10485 2024-04-01 06:37:20.000000 ibeam-0.5.2rc5/ibeam/src/handlers/strategy_handler.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.2rc5/ibeam/src/health_server.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.819173 ibeam-0.5.2rc5/ibeam/src/login/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:52:15.000000 ibeam-0.5.2rc5/ibeam/src/login/__init__.py
--rw-rw-rw-   0        0        0     6582 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/login/driver.py
--rw-rw-rw-   0        0        0     4906 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/login/targets.py
--rw-rw-rw-   0        0        0     2292 2024-04-28 04:04:24.000000 ibeam-0.5.2rc5/ibeam/src/logs.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.832178 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/notification_resend_handler.py
--rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.2rc5/ibeam/src/two_fa_selector.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.839182 ibeam-0.5.2rc5/ibeam/src/utils/
--rw-rw-rw-   0        0        0        0 2024-04-28 03:53:41.000000 ibeam-0.5.2rc5/ibeam/src/utils/__init__.py
--rw-rw-rw-   0        0        0      305 2023-09-07 18:11:53.000000 ibeam-0.5.2rc5/ibeam/src/utils/py_utils.py
--rw-rw-rw-   0        0        0     1454 2023-09-07 18:11:53.000000 ibeam-0.5.2rc5/ibeam/src/utils/selenium_utils.py
--rw-rw-rw-   0        0        0     7784 2024-04-01 06:19:12.000000 ibeam-0.5.2rc5/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:20:45.842143 ibeam-0.5.2rc5/ibeam.egg-info/
--rw-rw-rw-   0        0        0    11530 2024-04-28 04:20:45.000000 ibeam-0.5.2rc5/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2024-04-28 04:20:45.000000 ibeam-0.5.2rc5/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 04:20:45.000000 ibeam-0.5.2rc5/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2024-04-28 04:20:45.000000 ibeam-0.5.2rc5/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-28 04:20:45.000000 ibeam-0.5.2rc5/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2024-04-28 04:20:45.849187 ibeam-0.5.2rc5/setup.cfg
--rw-rw-rw-   0        0        0     1461 2024-04-28 04:20:27.000000 ibeam-0.5.2rc5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.751138 ibeam-0.5.2rc6/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.2rc6/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-04-28 04:21:26.000000 ibeam-0.5.2rc6/MANIFEST.in
+-rw-rw-rw-   0        0        0    11530 2024-04-28 04:21:35.750127 ibeam-0.5.2rc6/PKG-INFO
+-rw-rw-rw-   0        0        0    10623 2024-04-01 05:52:03.000000 ibeam-0.5.2rc6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.671137 ibeam-0.5.2rc6/ibeam/
+-rw-rw-rw-   0        0        0       78 2024-04-28 04:21:31.000000 ibeam-0.5.2rc6/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.2rc6/ibeam/config.py
+-rw-rw-rw-   0        0        0     6781 2024-04-01 06:33:58.000000 ibeam-0.5.2rc6/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.702147 ibeam-0.5.2rc6/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.2rc6/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/gateway_client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.719113 ibeam-0.5.2rc6/ibeam/src/handlers/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:09.000000 ibeam-0.5.2rc6/ibeam/src/handlers/__init__.py
+-rw-rw-rw-   0        0        0    13148 2024-04-01 06:33:58.000000 ibeam-0.5.2rc6/ibeam/src/handlers/http_handler.py
+-rw-rw-rw-   0        0        0     1500 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/ibeam/src/handlers/inputs_handler.py
+-rw-rw-rw-   0        0        0    20297 2024-04-15 03:27:57.000000 ibeam-0.5.2rc6/ibeam/src/handlers/login_handler.py
+-rw-rw-rw-   0        0        0     5236 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/handlers/process_handler.py
+-rw-rw-rw-   0        0        0     6567 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/ibeam/src/handlers/secrets_handler.py
+-rw-rw-rw-   0        0        0    10485 2024-04-01 06:37:20.000000 ibeam-0.5.2rc6/ibeam/src/handlers/strategy_handler.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.2rc6/ibeam/src/health_server.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.727121 ibeam-0.5.2rc6/ibeam/src/login/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:15.000000 ibeam-0.5.2rc6/ibeam/src/login/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/login/driver.py
+-rw-rw-rw-   0        0        0     4906 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/login/targets.py
+-rw-rw-rw-   0        0        0     2292 2024-04-28 04:04:24.000000 ibeam-0.5.2rc6/ibeam/src/logs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.738140 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.2rc6/ibeam/src/two_fa_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.745146 ibeam-0.5.2rc6/ibeam/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:53:41.000000 ibeam-0.5.2rc6/ibeam/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/ibeam/src/utils/py_utils.py
+-rw-rw-rw-   0        0        0     1454 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/ibeam/src/utils/selenium_utils.py
+-rw-rw-rw-   0        0        0     7784 2024-04-01 06:19:12.000000 ibeam-0.5.2rc6/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:21:35.748147 ibeam-0.5.2rc6/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    11530 2024-04-28 04:21:35.000000 ibeam-0.5.2rc6/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2024-04-28 04:21:35.000000 ibeam-0.5.2rc6/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:21:35.000000 ibeam-0.5.2rc6/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-04-28 04:21:35.000000 ibeam-0.5.2rc6/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-28 04:21:35.000000 ibeam-0.5.2rc6/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      132 2023-09-07 18:11:53.000000 ibeam-0.5.2rc6/requirements.txt
+-rw-rw-rw-   0        0        0      142 2024-04-28 04:21:35.753113 ibeam-0.5.2rc6/setup.cfg
+-rw-rw-rw-   0        0        0     1461 2024-04-28 04:20:27.000000 ibeam-0.5.2rc6/setup.py
```

### Comparing `ibeam-0.5.2rc5/LICENSE` & `ibeam-0.5.2rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/PKG-INFO` & `ibeam-0.5.2rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.2rc5
+Version: 0.5.2rc6
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
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc5 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc6 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.5.2rc5/README.md` & `ibeam-0.5.2rc6/README.md`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/config.py` & `ibeam-0.5.2rc6/ibeam/config.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/ibeam_starter.py` & `ibeam-0.5.2rc6/ibeam/ibeam_starter.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/gateway_client.py` & `ibeam-0.5.2rc6/ibeam/src/gateway_client.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/http_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/inputs_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/login_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/login_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/process_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/process_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/secrets_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/secrets_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/handlers/strategy_handler.py` & `ibeam-0.5.2rc6/ibeam/src/handlers/strategy_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/health_server.py` & `ibeam-0.5.2rc6/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/login/driver.py` & `ibeam-0.5.2rc6/ibeam/src/login/driver.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/login/targets.py` & `ibeam-0.5.2rc6/ibeam/src/login/targets.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/logs.py` & `ibeam-0.5.2rc6/ibeam/src/logs.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/two_fa_handlers/notification_resend_handler.py` & `ibeam-0.5.2rc6/ibeam/src/two_fa_handlers/notification_resend_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/two_fa_selector.py` & `ibeam-0.5.2rc6/ibeam/src/two_fa_selector.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/utils/selenium_utils.py` & `ibeam-0.5.2rc6/ibeam/src/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam/src/var.py` & `ibeam-0.5.2rc6/ibeam/src/var.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.2rc5/ibeam.egg-info/PKG-INFO` & `ibeam-0.5.2rc6/ibeam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.2rc5
+Version: 0.5.2rc6
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
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc5 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2rc6 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.5.2rc5/ibeam.egg-info/SOURCES.txt` & `ibeam-0.5.2rc6/ibeam.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 ibeam/__init__.py
 ibeam/config.py
 ibeam/ibeam_starter.py
 ibeam.egg-info/PKG-INFO
 ibeam.egg-info/SOURCES.txt
```

### Comparing `ibeam-0.5.2rc5/setup.py` & `ibeam-0.5.2rc6/setup.py`

 * *Files identical despite different names*

