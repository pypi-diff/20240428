# Comparing `tmp/ibeam-0.5.1.tar.gz` & `tmp/ibeam-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibeam-0.5.1.tar", last modified: Mon Nov  6 16:41:06 2023, max compression
+gzip compressed data, was "ibeam-0.5.2.tar", last modified: Sun Apr 28 04:07:53 2024, max compression
```

## Comparing `ibeam-0.5.1.tar` & `ibeam-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 16:41:06.142175 ibeam-0.5.1/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    11286 2023-11-06 16:41:06.142175 ibeam-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    10621 2023-09-07 18:11:53.000000 ibeam-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 16:41:06.063634 ibeam-0.5.1/ibeam/
--rw-rw-rw-   0        0        0       74 2023-11-06 16:33:01.000000 ibeam-0.5.1/ibeam/__init__.py
--rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.1/ibeam/config.py
--rw-rw-rw-   0        0        0     6733 2023-10-25 19:20:22.000000 ibeam-0.5.1/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2023-11-06 16:41:06.110933 ibeam-0.5.1/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.1/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.1/ibeam/src/gateway_client.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.1/ibeam/src/health_server.py
--rw-rw-rw-   0        0        0     2039 2023-09-07 18:11:53.000000 ibeam-0.5.1/ibeam/src/logs.py
-drwxrwxrwx   0        0        0        0 2023-11-06 16:41:06.142175 ibeam-0.5.1/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.1/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.1/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.1/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.1/ibeam/src/two_fa_handlers/notification_resend_handler.py
--rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.1/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.1/ibeam/src/two_fa_selector.py
--rw-rw-rw-   0        0        0     7611 2023-10-25 19:35:02.000000 ibeam-0.5.1/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2023-11-06 16:41:06.079668 ibeam-0.5.1/ibeam.egg-info/
--rw-rw-rw-   0        0        0    11286 2023-11-06 16:41:05.000000 ibeam-0.5.1/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-11-06 16:41:05.000000 ibeam-0.5.1/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 16:41:05.000000 ibeam-0.5.1/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-11-06 16:41:05.000000 ibeam-0.5.1/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-06 16:41:05.000000 ibeam-0.5.1/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-11-06 16:41:06.157820 ibeam-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-09-07 18:11:53.000000 ibeam-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.417612 ibeam-0.5.2/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    11527 2024-04-28 04:07:53.415779 ibeam-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10623 2024-04-01 05:52:03.000000 ibeam-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.339253 ibeam-0.5.2/ibeam/
+-rw-rw-rw-   0        0        0       74 2024-04-28 04:06:51.000000 ibeam-0.5.2/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-10-25 19:22:13.000000 ibeam-0.5.2/ibeam/config.py
+-rw-rw-rw-   0        0        0     6781 2024-04-01 06:33:58.000000 ibeam-0.5.2/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.366470 ibeam-0.5.2/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.5.2/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0     4462 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/gateway_client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.383466 ibeam-0.5.2/ibeam/src/handlers/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:09.000000 ibeam-0.5.2/ibeam/src/handlers/__init__.py
+-rw-rw-rw-   0        0        0    13148 2024-04-01 06:33:58.000000 ibeam-0.5.2/ibeam/src/handlers/http_handler.py
+-rw-rw-rw-   0        0        0     1500 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/handlers/inputs_handler.py
+-rw-rw-rw-   0        0        0    20297 2024-04-15 03:27:57.000000 ibeam-0.5.2/ibeam/src/handlers/login_handler.py
+-rw-rw-rw-   0        0        0     5236 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/handlers/process_handler.py
+-rw-rw-rw-   0        0        0     6567 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/handlers/secrets_handler.py
+-rw-rw-rw-   0        0        0    10485 2024-04-01 06:37:20.000000 ibeam-0.5.2/ibeam/src/handlers/strategy_handler.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.5.2/ibeam/src/health_server.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.390490 ibeam-0.5.2/ibeam/src/login/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:52:15.000000 ibeam-0.5.2/ibeam/src/login/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/login/driver.py
+-rw-rw-rw-   0        0        0     4906 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/login/targets.py
+-rw-rw-rw-   0        0        0     2292 2024-04-28 04:04:24.000000 ibeam-0.5.2/ibeam/src/logs.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.402597 ibeam-0.5.2/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5534 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     3148 2023-10-25 18:56:30.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      405 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2609 2023-11-06 16:31:15.000000 ibeam-0.5.2/ibeam/src/two_fa_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.409875 ibeam-0.5.2/ibeam/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-28 03:53:41.000000 ibeam-0.5.2/ibeam/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/utils/py_utils.py
+-rw-rw-rw-   0        0        0     1454 2023-09-07 18:11:53.000000 ibeam-0.5.2/ibeam/src/utils/selenium_utils.py
+-rw-rw-rw-   0        0        0     7784 2024-04-01 06:19:12.000000 ibeam-0.5.2/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2024-04-28 04:07:53.413385 ibeam-0.5.2/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    11527 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-28 04:07:53.000000 ibeam-0.5.2/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-28 04:07:53.418636 ibeam-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2024-04-28 04:06:41.000000 ibeam-0.5.2/setup.py
```

### Comparing `ibeam-0.5.1/LICENSE` & `ibeam-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/PKG-INFO` & `ibeam-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.1
+Version: 0.5.2
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: selenium==4.12.*
+Requires-Dist: cryptography==40.0.*
+Requires-Dist: pyvirtualdisplay==3.0.*
+Requires-Dist: apscheduler==3.10.*
+Requires-Dist: psutil==5.9.*
+Requires-Dist: requests==2.30.*
+Requires-Dist: pillow==9.5.*
 
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 <p align="center">
     <a id="ibeam" href="#ibeam">
         <img src="https://github.com/Voyz/ibeam/blob/master/media/ibeam_logo.png" alt="IBeam logo" title="IBeam logo" width="600"/>
@@ -260,14 +267,14 @@
 
 [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/Advanced-Secrets
 
 [troubleshooting]: https://github.com/Voyz/ibeam/wiki/Troubleshooting
 
 [issues]: https://github.com/Voyz/ibeam/issues
 
-[gateway]: https://interactivebrokers.github.io/cpwebapi/
+[gateway]: https://ibkrcampus.com/ibkr-api-page/webapi-doc/
 
 [ibc]: https://github.com/IbcAlpha/IBC
 
 [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-docker
 
 [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.1 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
-text/markdown License-File: LICENSE *This library is currently being beta-
-tested. See something that's broken? Did we get something wrong? [Create an
-issue and let us know!][issues]*
+text/markdown License-File: LICENSE Requires-Dist: selenium==4.12.* Requires-
+Dist: cryptography==40.0.* Requires-Dist: pyvirtualdisplay==3.0.* Requires-
+Dist: apscheduler==3.10.* Requires-Dist: psutil==5.9.* Requires-Dist:
+requests==2.30.* Requires-Dist: pillow==9.5.* *This library is currently being
+beta-tested. See something that's broken? Did we get something wrong? [Create
+an issue and let us know!][issues]*
                                  _[_I_B_e_a_m_ _l_o_g_o_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_i_b_e_a_m_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
 IBeam is an authentication and maintenance tool used for the [Interactive
 Brokers Client Portal Web API Gateway.][gateway] Features: * **Facilitates
 continuous headless run of the Gateway.** * **No physical display required** -
 virtual display buffer can be used instead. * **No interaction from the user
@@ -124,10 +127,10 @@
 Configuration [gateway-configuration]: https://github.com/Voyz/ibeam/wiki/
 Gateway-Configuration [inputs-and-outputs]: https://github.com/Voyz/ibeam/wiki/
 Inputs-And-Outputs [two-fa]: https://github.com/Voyz/ibeam/wiki/Two-Factor-
 Authentication [tls-and-https]: https://github.com/Voyz/ibeam/wiki/TLS-
 Certificates-and-HTTPS [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/
 Advanced-Secrets [troubleshooting]: https://github.com/Voyz/ibeam/wiki/
 Troubleshooting [issues]: https://github.com/Voyz/ibeam/issues [gateway]:
-https://interactivebrokers.github.io/cpwebapi/ [ibc]: https://github.com/
+https://ibkrcampus.com/ibkr-api-page/webapi-doc/ [ibc]: https://github.com/
 IbcAlpha/IBC [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-
 docker [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

### Comparing `ibeam-0.5.1/README.md` & `ibeam-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,14 @@
 
 [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/Advanced-Secrets
 
 [troubleshooting]: https://github.com/Voyz/ibeam/wiki/Troubleshooting
 
 [issues]: https://github.com/Voyz/ibeam/issues
 
-[gateway]: https://interactivebrokers.github.io/cpwebapi/
+[gateway]: https://ibkrcampus.com/ibkr-api-page/webapi-doc/
 
 [ibc]: https://github.com/IbcAlpha/IBC
 
 [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-docker
 
 [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

#### html2text {}

```diff
@@ -115,10 +115,10 @@
 [gateway-configuration]: https://github.com/Voyz/ibeam/wiki/Gateway-
 Configuration [inputs-and-outputs]: https://github.com/Voyz/ibeam/wiki/Inputs-
 And-Outputs [two-fa]: https://github.com/Voyz/ibeam/wiki/Two-Factor-
 Authentication [tls-and-https]: https://github.com/Voyz/ibeam/wiki/TLS-
 Certificates-and-HTTPS [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/
 Advanced-Secrets [troubleshooting]: https://github.com/Voyz/ibeam/wiki/
 Troubleshooting [issues]: https://github.com/Voyz/ibeam/issues [gateway]:
-https://interactivebrokers.github.io/cpwebapi/ [ibc]: https://github.com/
+https://ibkrcampus.com/ibkr-api-page/webapi-doc/ [ibc]: https://github.com/
 IbcAlpha/IBC [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-
 docker [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

### Comparing `ibeam-0.5.1/ibeam/config.py` & `ibeam-0.5.2/ibeam/config.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/ibeam_starter.py` & `ibeam-0.5.2/ibeam/ibeam_starter.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     http_handler = HttpHandler(
         inputs_handler=inputs_handler,
         base_url=cnf.GATEWAY_BASE_URL,
         route_validate=cnf.ROUTE_VALIDATE,
         route_tickle=cnf.ROUTE_TICKLE,
         route_logout=cnf.ROUTE_LOGOUT,
         route_reauthenticate=cnf.ROUTE_REAUTHENTICATE,
+        route_initialise=cnf.ROUTE_INITIALISE,
         request_timeout=cnf.REQUEST_TIMEOUT,
     )
 
     driver_factory = DriverFactory(
         driver_path=cnf.CHROME_DRIVER_PATH,
         ui_scaling=cnf.UI_SCALING,
         page_load_timeout=cnf.PAGE_LOAD_TIMEOUT,
```

### Comparing `ibeam-0.5.1/ibeam/src/gateway_client.py` & `ibeam-0.5.2/ibeam/src/gateway_client.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/health_server.py` & `ibeam-0.5.2/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/logs.py` & `ibeam-0.5.2/ibeam/src/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import logging
 import os
 import sys
+from pathlib import Path
 
 initialized = False
 
 
 def initialize(log_format: str,
                log_level: str,
                log_to_file: bool,
@@ -58,14 +59,18 @@
         return datetime.datetime.now().strftime(self.date_format)
 
     def get_filename(self, timestamp):
         return f'{self.baseFilename}__{timestamp}.txt'
 
     def _open(self):
         self.timestamp = self.get_timestamp()
-        return open(self.get_filename(self.timestamp), self.mode, encoding=self.encoding)
+        try:
+            return open(self.get_filename(self.timestamp), self.mode, encoding=self.encoding)
+        except FileNotFoundError:
+            Path(self.baseFilename).parent.mkdir(parents=True, exist_ok=True)
+            return open(self.get_filename(self.timestamp), self.mode, encoding=self.encoding)
 
     def emit(self, record):
         if self.get_timestamp() != self.timestamp:
             self.stream = self._open()
 
         super().emit(record)
```

### Comparing `ibeam-0.5.1/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.5.2/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.5.2/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/two_fa_handlers/notification_resend_handler.py` & `ibeam-0.5.2/ibeam/src/two_fa_handlers/notification_resend_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/two_fa_selector.py` & `ibeam-0.5.2/ibeam/src/two_fa_selector.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.5.1/ibeam/src/var.py` & `ibeam-0.5.2/ibeam/src/var.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 
 ROUTE_VALIDATE = os.environ.get('IBEAM_ROUTE_VALIDATE', '/v1/portal/sso/validate')
 """Gateway route with validation call."""
 
 ROUTE_REAUTHENTICATE = os.environ.get('IBEAM_ROUTE_REAUTHENTICATE', '/v1/portal/iserver/reauthenticate?force=true')
 """Gateway route with reauthentication call."""
 
+ROUTE_INITIALISE = os.environ.get('IBEAM_ROUTE_INITIALISE', '/v1/api/iserver/auth/ssodh/init')
+"""Gateway route with session initialisation call."""
+
 ROUTE_AUTH_STATUS = os.environ.get('IBEAM_ROUTE_AUTH_STATUS', '/v1/api/iserver/auth/status')
 """Gateway route with authentication status call."""
 
 ROUTE_TICKLE = os.environ.get('IBEAM_ROUTE_TICKLE', '/v1/api/tickle')
 """Gateway route with tickle call."""
 
 ROUTE_LOGOUT = os.environ.get('IBEAM_ROUTE_LOGOUT', '/v1/api/logout')
@@ -129,15 +132,15 @@
 
 IBKEY_PROMO_EL_CLASS = os.environ.get('IBEAM_IBKEY_PROMO_EL_CLASS', 'CLASS_NAME@@ibkey-promo-skip')
 """HTML element class containing the ibkey promo skip button."""
 
 AUTHENTICATION_STRATEGY = os.environ.get('IBEAM_AUTHENTICATION_STRATEGY', 'B')
 """The authentication strategy used by IBeam."""
 
-MAX_STATUS_CHECK_RETRIES = int(os.environ.get('IBEAM_MAX_STATUS_CHECK_RETRIES', 15))
+MAX_STATUS_CHECK_RETRIES = int(os.environ.get('IBEAM_MAX_STATUS_CHECK_RETRIES', 120))
 """How many times to reattempt the status check."""
 
 MAX_REAUTHENTICATE_RETRIES = int(os.environ.get('IBEAM_MAX_REAUTHENTICATE_RETRIES', 3))
 """How many times to reattempt the reauthentication before restarting the Gateway."""
 
 UI_SCALING = float(os.environ.get('IBEAM_UI_SCALING', 1))
 """The resolution UI scaling to be used by the browser."""
@@ -164,8 +167,8 @@
 
 TWO_FA_SELECT_TARGET = os.environ.get('IBEAM_TWO_FA_SELECT_TARGET', 'IB Key')
 """Option that is to be chosen in the 2FA select dropdown"""
 
 CUSTOM_TWO_FA_HANDLER = os.environ.get('IBEAM_CUSTOM_TWO_FA_HANDLER', 'custom_two_fa_handler.CustomTwoFaHandler')
 """Fully qualified path of the custom 2FA handler in the inputs directory."""
 
-all_variables = {item: value for item, value in vars().items() if (not item.startswith("__") and item.isupper())}
+all_variables = {key: value for key, value in vars().items() if (not key.startswith("__") and key.isupper() and key != 'UNDEFINED')}
```

### Comparing `ibeam-0.5.1/ibeam.egg-info/PKG-INFO` & `ibeam-0.5.2/ibeam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.5.1
+Version: 0.5.2
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: selenium==4.12.*
+Requires-Dist: cryptography==40.0.*
+Requires-Dist: pyvirtualdisplay==3.0.*
+Requires-Dist: apscheduler==3.10.*
+Requires-Dist: psutil==5.9.*
+Requires-Dist: requests==2.30.*
+Requires-Dist: pillow==9.5.*
 
 *This library is currently being beta-tested. See something that's broken? Did we get something
 wrong? [Create an issue and let us know!][issues]*
 
 <p align="center">
     <a id="ibeam" href="#ibeam">
         <img src="https://github.com/Voyz/ibeam/blob/master/media/ibeam_logo.png" alt="IBeam logo" title="IBeam logo" width="600"/>
@@ -260,14 +267,14 @@
 
 [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/Advanced-Secrets
 
 [troubleshooting]: https://github.com/Voyz/ibeam/wiki/Troubleshooting
 
 [issues]: https://github.com/Voyz/ibeam/issues
 
-[gateway]: https://interactivebrokers.github.io/cpwebapi/
+[gateway]: https://ibkrcampus.com/ibkr-api-page/webapi-doc/
 
 [ibc]: https://github.com/IbcAlpha/IBC
 
 [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-docker
 
 [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.5.1 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.5.2 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
-text/markdown License-File: LICENSE *This library is currently being beta-
-tested. See something that's broken? Did we get something wrong? [Create an
-issue and let us know!][issues]*
+text/markdown License-File: LICENSE Requires-Dist: selenium==4.12.* Requires-
+Dist: cryptography==40.0.* Requires-Dist: pyvirtualdisplay==3.0.* Requires-
+Dist: apscheduler==3.10.* Requires-Dist: psutil==5.9.* Requires-Dist:
+requests==2.30.* Requires-Dist: pillow==9.5.* *This library is currently being
+beta-tested. See something that's broken? Did we get something wrong? [Create
+an issue and let us know!][issues]*
                                  _[_I_B_e_a_m_ _l_o_g_o_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_i_b_e_a_m_?_l_a_b_e_l_=_v_e_r_s_i_o_n_]
 IBeam is an authentication and maintenance tool used for the [Interactive
 Brokers Client Portal Web API Gateway.][gateway] Features: * **Facilitates
 continuous headless run of the Gateway.** * **No physical display required** -
 virtual display buffer can be used instead. * **No interaction from the user
@@ -124,10 +127,10 @@
 Configuration [gateway-configuration]: https://github.com/Voyz/ibeam/wiki/
 Gateway-Configuration [inputs-and-outputs]: https://github.com/Voyz/ibeam/wiki/
 Inputs-And-Outputs [two-fa]: https://github.com/Voyz/ibeam/wiki/Two-Factor-
 Authentication [tls-and-https]: https://github.com/Voyz/ibeam/wiki/TLS-
 Certificates-and-HTTPS [advanced-secrets]: https://github.com/Voyz/ibeam/wiki/
 Advanced-Secrets [troubleshooting]: https://github.com/Voyz/ibeam/wiki/
 Troubleshooting [issues]: https://github.com/Voyz/ibeam/issues [gateway]:
-https://interactivebrokers.github.io/cpwebapi/ [ibc]: https://github.com/
+https://ibkrcampus.com/ibkr-api-page/webapi-doc/ [ibc]: https://github.com/
 IbcAlpha/IBC [ib-gateway-docker]: https://github.com/UnusualAlpha/ib-gateway-
 docker [secret-manager-docs]: https://cloud.google.com/secret-manager/docs
```

