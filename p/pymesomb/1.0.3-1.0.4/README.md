# Comparing `tmp/pymesomb-1.0.3.tar.gz` & `tmp/pymesomb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymesomb-1.0.3.tar", last modified: Mon Jan 29 19:00:19 2024, max compression
+gzip compressed data, was "pymesomb-1.0.4.tar", last modified: Sun Apr 28 07:27:14 2024, max compression
```

## Comparing `pymesomb-1.0.3.tar` & `pymesomb-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 hachther   (502) staff       (20)        0 2024-01-29 19:00:19.347164 pymesomb-1.0.3/
--rw-r--r--   0 hachther   (502) staff       (20)        0 2024-01-24 15:15:00.000000 pymesomb-1.0.3/LICENSE
--rw-r--r--   0 hachther   (502) staff       (20)        0 2024-01-24 15:15:00.000000 pymesomb-1.0.3/MANIFEST.in
--rw-r--r--   0 hachther   (502) staff       (20)     3589 2024-01-29 19:00:19.346203 pymesomb-1.0.3/PKG-INFO
--rw-r--r--   0 hachther   (502) staff       (20)     2731 2024-01-24 15:15:00.000000 pymesomb-1.0.3/README.md
-drwxr-xr-x   0 hachther   (502) staff       (20)        0 2024-01-29 19:00:19.340003 pymesomb-1.0.3/pymesomb/
--rw-r--r--   0 hachther   (502) staff       (20)      133 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/__init__.py
--rw-r--r--   0 hachther   (502) staff       (20)      635 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/exceptions.py
--rw-r--r--   0 hachther   (502) staff       (20)      100 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/mesomb.py
--rw-r--r--   0 hachther   (502) staff       (20)     3719 2024-01-24 15:17:22.000000 pymesomb-1.0.3/pymesomb/models.py
--rw-r--r--   0 hachther   (502) staff       (20)     9946 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/operations.py
--rw-r--r--   0 hachther   (502) staff       (20)     2958 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/signature.py
--rw-r--r--   0 hachther   (502) staff       (20)      222 2024-01-24 15:15:00.000000 pymesomb-1.0.3/pymesomb/utils.py
-drwxr-xr-x   0 hachther   (502) staff       (20)        0 2024-01-29 19:00:19.345041 pymesomb-1.0.3/pymesomb.egg-info/
--rw-r--r--   0 hachther   (502) staff       (20)     3589 2024-01-29 19:00:19.000000 pymesomb-1.0.3/pymesomb.egg-info/PKG-INFO
--rw-r--r--   0 hachther   (502) staff       (20)      342 2024-01-29 19:00:19.000000 pymesomb-1.0.3/pymesomb.egg-info/SOURCES.txt
--rw-r--r--   0 hachther   (502) staff       (20)        1 2024-01-29 19:00:19.000000 pymesomb-1.0.3/pymesomb.egg-info/dependency_links.txt
--rw-r--r--   0 hachther   (502) staff       (20)        9 2024-01-29 19:00:19.000000 pymesomb-1.0.3/pymesomb.egg-info/requires.txt
--rw-r--r--   0 hachther   (502) staff       (20)        9 2024-01-29 19:00:19.000000 pymesomb-1.0.3/pymesomb.egg-info/top_level.txt
--rw-r--r--   0 hachther   (502) staff       (20)       38 2024-01-29 19:00:19.347705 pymesomb-1.0.3/setup.cfg
--rw-r--r--   0 hachther   (502) staff       (20)      826 2024-01-24 15:15:00.000000 pymesomb-1.0.3/setup.py
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2024-04-28 07:27:14.887741 pymesomb-1.0.4/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      531 2024-04-28 07:19:45.000000 pymesomb-1.0.4/HISTORY.md
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        0 2023-05-29 14:21:36.000000 pymesomb-1.0.4/LICENSE
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        0 2023-05-29 14:21:36.000000 pymesomb-1.0.4/MANIFEST.in
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3646 2024-04-28 07:27:14.887741 pymesomb-1.0.4/PKG-INFO
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     2731 2023-07-25 12:53:49.000000 pymesomb-1.0.4/README.md
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2024-04-28 07:27:14.887741 pymesomb-1.0.4/pymesomb/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      133 2023-07-25 12:15:22.000000 pymesomb-1.0.4/pymesomb/__init__.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      635 2023-05-29 15:36:39.000000 pymesomb-1.0.4/pymesomb/exceptions.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      100 2023-07-25 10:42:01.000000 pymesomb-1.0.4/pymesomb/mesomb.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3731 2024-04-28 07:18:28.000000 pymesomb-1.0.4/pymesomb/models.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     9946 2024-01-24 15:03:35.000000 pymesomb-1.0.4/pymesomb/operations.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     2958 2023-07-25 12:08:05.000000 pymesomb-1.0.4/pymesomb/signature.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      756 2024-04-28 07:18:28.000000 pymesomb-1.0.4/pymesomb/utils.py
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2024-04-28 07:27:14.887741 pymesomb-1.0.4/pymesomb.egg-info/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3646 2024-04-28 07:27:14.000000 pymesomb-1.0.4/pymesomb.egg-info/PKG-INFO
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      353 2024-04-28 07:27:14.000000 pymesomb-1.0.4/pymesomb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        1 2024-04-28 07:27:14.000000 pymesomb-1.0.4/pymesomb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        9 2024-04-28 07:27:14.000000 pymesomb-1.0.4/pymesomb.egg-info/requires.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        9 2024-04-28 07:27:14.000000 pymesomb-1.0.4/pymesomb.egg-info/top_level.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)       38 2024-04-28 07:27:14.887741 pymesomb-1.0.4/setup.cfg
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      826 2024-04-28 07:20:02.000000 pymesomb-1.0.4/setup.py
```

### Comparing `pymesomb-1.0.3/PKG-INFO` & `pymesomb-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pymesomb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python client for MeSomb services.
 Home-page: https://github.com/hachther/mesomb-python-client.git
 Download-URL: https://pypi.org/project/pymesomb/
 Author: Hachther LLC
 Author-email: contact@hachther.com
 License: MIT
 Keywords: MeSomb,MobileMoney,OrangeMoney
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
 
 <h1 align="center">Welcome to pymesomb 👋</h1>
 <p>
   <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
   <a href="https://mesomb.hachther.com/en/api/v1.1/schema/" target="_blank">
     <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
   </a>
@@ -110,14 +109,17 @@
 * LinkedIn: [@hachther](https://linkedin.com/in/hachther)
 
 ## Show your support
 
 Give a ⭐️ if this project helped you!
 
 
+# 1.0.4 (2024-04-28)
+- Add function to detect phone number operator in cameroon
+
 # 1.0.3 (2024-01-24)
 - Handle case when trxID is not string 
 - Fix crash to display response
 - Add raw_response in TransactionResponse to store MeSomb response.
 
 # 1.0.2 (2023-07-25)
 ## === BREAKING CHANGES ===
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pymesomb Version: 1.0.3 Summary: Python client for
+Metadata-Version: 2.1 Name: pymesomb Version: 1.0.4 Summary: Python client for
 MeSomb services. Home-page: https://github.com/hachther/mesomb-python-
 client.git Download-URL: https://pypi.org/project/pymesomb/ Author: Hachther
 LLC Author-email: contact@hachther.com License: MIT Keywords:
 MeSomb,MobileMoney,OrangeMoney Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests
+File: LICENSE
                     ************ WWeellccoommee ttoo ppyymmeessoommbb ?ð??? ************
 [Version]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_T_w_i_t_t_e_r_:_ _h_a_c_h_t_h_e_r_]
 > Python client for MeSomb Services > > You can check the full [documentation
 of the api here](https://mesomb.hachther.com/en/api/v1.1/schema/) ### ð 
 [Homepage](https://mesomb.com) ## Install ```sh pip3 install pymesomb ``` ##
 Usage ### Collect money from an account ```python from pymesomb.operations
 import PaymentOperation from pymesomb.utils import RandomGenerator from
@@ -26,14 +26,15 @@
 ('', '', '') response = operation.get_status() print(response.name) ``` ### Get
 transactions by IDs ```python from pymesomb.operations import PaymentOperation
 operation = PaymentOperation('', '', '') response = operation.get_transactions(
 ['ID1', 'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
 hachther.com>** * Website: https://www.hachther.com * Twitter: [@hachther]
 (https://twitter.com/hachther) * Github: [@hachther](https://github.com/
 hachther) * LinkedIn: [@hachther](https://linkedin.com/in/hachther) ## Show
-your support Give a â­ï¸ if this project helped you! # 1.0.3 (2024-01-24) -
+your support Give a â­ï¸ if this project helped you! # 1.0.4 (2024-04-28) -
+Add function to detect phone number operator in cameroon # 1.0.3 (2024-01-24) -
 Handle case when trxID is not string - Fix crash to display response - Add
 raw_response in TransactionResponse to store MeSomb response. # 1.0.2 (2023-07-
 25) ## === BREAKING CHANGES === Only one parameter is now passed to
 make_deposit and make_collect. The parameter is a Map that will contain all
 details of your request. All method is now returning MeSomb model not dict #
 1.0.0 (2022-10-20) First release of the module.
```

### Comparing `pymesomb-1.0.3/README.md` & `pymesomb-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymesomb-1.0.3/pymesomb/exceptions.py` & `pymesomb-1.0.4/pymesomb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymesomb-1.0.3/pymesomb/models.py` & `pymesomb-1.0.4/pymesomb/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def __str__(self):
         return '{}: {}'.format(self.status, self.message)
 
     def is_operation_success(self):
         return self.success
 
     def is_transaction_success(self):
-        return self.success and self.status == 'SUCCESS'
+        return self.success and self.transaction.status == 'SUCCESS'
 
 
 class ApplicationBalance:
     def __init__(self, data):
         self.country = data.get("country")
         self.currency = data.get("currency")
         self.provider = data.get("provider")
```

### Comparing `pymesomb-1.0.3/pymesomb/operations.py` & `pymesomb-1.0.4/pymesomb/operations.py`

 * *Files identical despite different names*

### Comparing `pymesomb-1.0.3/pymesomb/signature.py` & `pymesomb-1.0.4/pymesomb/signature.py`

 * *Files identical despite different names*

### Comparing `pymesomb-1.0.3/pymesomb.egg-info/PKG-INFO` & `pymesomb-1.0.4/pymesomb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pymesomb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python client for MeSomb services.
 Home-page: https://github.com/hachther/mesomb-python-client.git
 Download-URL: https://pypi.org/project/pymesomb/
 Author: Hachther LLC
 Author-email: contact@hachther.com
 License: MIT
 Keywords: MeSomb,MobileMoney,OrangeMoney
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
 
 <h1 align="center">Welcome to pymesomb 👋</h1>
 <p>
   <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
   <a href="https://mesomb.hachther.com/en/api/v1.1/schema/" target="_blank">
     <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
   </a>
@@ -110,14 +109,17 @@
 * LinkedIn: [@hachther](https://linkedin.com/in/hachther)
 
 ## Show your support
 
 Give a ⭐️ if this project helped you!
 
 
+# 1.0.4 (2024-04-28)
+- Add function to detect phone number operator in cameroon
+
 # 1.0.3 (2024-01-24)
 - Handle case when trxID is not string 
 - Fix crash to display response
 - Add raw_response in TransactionResponse to store MeSomb response.
 
 # 1.0.2 (2023-07-25)
 ## === BREAKING CHANGES ===
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pymesomb Version: 1.0.3 Summary: Python client for
+Metadata-Version: 2.1 Name: pymesomb Version: 1.0.4 Summary: Python client for
 MeSomb services. Home-page: https://github.com/hachther/mesomb-python-
 client.git Download-URL: https://pypi.org/project/pymesomb/ Author: Hachther
 LLC Author-email: contact@hachther.com License: MIT Keywords:
 MeSomb,MobileMoney,OrangeMoney Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests
+File: LICENSE
                     ************ WWeellccoommee ttoo ppyymmeessoommbb ?ð??? ************
 [Version]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_T_w_i_t_t_e_r_:_ _h_a_c_h_t_h_e_r_]
 > Python client for MeSomb Services > > You can check the full [documentation
 of the api here](https://mesomb.hachther.com/en/api/v1.1/schema/) ### ð 
 [Homepage](https://mesomb.com) ## Install ```sh pip3 install pymesomb ``` ##
 Usage ### Collect money from an account ```python from pymesomb.operations
 import PaymentOperation from pymesomb.utils import RandomGenerator from
@@ -26,14 +26,15 @@
 ('', '', '') response = operation.get_status() print(response.name) ``` ### Get
 transactions by IDs ```python from pymesomb.operations import PaymentOperation
 operation = PaymentOperation('', '', '') response = operation.get_transactions(
 ['ID1', 'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
 hachther.com>** * Website: https://www.hachther.com * Twitter: [@hachther]
 (https://twitter.com/hachther) * Github: [@hachther](https://github.com/
 hachther) * LinkedIn: [@hachther](https://linkedin.com/in/hachther) ## Show
-your support Give a â­ï¸ if this project helped you! # 1.0.3 (2024-01-24) -
+your support Give a â­ï¸ if this project helped you! # 1.0.4 (2024-04-28) -
+Add function to detect phone number operator in cameroon # 1.0.3 (2024-01-24) -
 Handle case when trxID is not string - Fix crash to display response - Add
 raw_response in TransactionResponse to store MeSomb response. # 1.0.2 (2023-07-
 25) ## === BREAKING CHANGES === Only one parameter is now passed to
 make_deposit and make_collect. The parameter is a Map that will contain all
 details of your request. All method is now returning MeSomb model not dict #
 1.0.0 (2022-10-20) First release of the module.
```

### Comparing `pymesomb-1.0.3/setup.py` & `pymesomb-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pymesomb',
-    version='1.0.3',
+    version='1.0.4',
     description='Python client for MeSomb services.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Hachther LLC',
     author_email='contact@hachther.com',
```

