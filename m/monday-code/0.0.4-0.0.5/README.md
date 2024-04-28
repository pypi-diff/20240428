# Comparing `tmp/monday_code-0.0.4.tar.gz` & `tmp/monday_code-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday_code-0.0.4.tar", last modified: Tue Apr 16 08:58:01 2024, max compression
+gzip compressed data, was "monday_code-0.0.5.tar", last modified: Sun Apr 28 06:08:16 2024, max compression
```

## Comparing `monday_code-0.0.4.tar` & `monday_code-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.012638 monday_code-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 08:57:53.000000 monday_code-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-16 08:58:01.012638 monday_code-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-16 08:57:53.000000 monday_code-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-16 08:57:53.000000 monday_code-0.0.4/README_FOR_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.004638 monday_code-0.0.4/monday_code/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.008638 monday_code-0.0.4/monday_code/api/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api/secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api/secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45643 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api/storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.008638 monday_code-0.0.4/monday_code/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/models/validate_secret_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-16 08:57:53.000000 monday_code-0.0.4/monday_code/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.012638 monday_code-0.0.4/monday_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-16 08:58:00.000000 monday_code-0.0.4/monday_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-16 08:58:00.000000 monday_code-0.0.4/monday_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:58:00.000000 monday_code-0.0.4/monday_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:58:00.000000 monday_code-0.0.4/monday_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 08:58:00.000000 monday_code-0.0.4/monday_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-16 08:57:53.000000 monday_code-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:58:01.012638 monday_code-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-16 08:57:53.000000 monday_code-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:58:01.012638 monday_code-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-16 08:57:53.000000 monday_code-0.0.4/test/test_validate_secret_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 06:08:10.000000 monday_code-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-28 06:08:16.777480 monday_code-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-28 06:08:10.000000 monday_code-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-28 06:08:10.000000 monday_code-0.0.5/README_FOR_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.769481 monday_code-0.0.5/monday_code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.773481 monday_code-0.0.5/monday_code/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/secret_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30735 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45643 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.773481 monday_code-0.0.5/monday_code/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/validate_secret_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/monday_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-28 06:08:10.000000 monday_code-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 06:08:16.777480 monday_code-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-28 06:08:10.000000 monday_code-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secret_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_validate_secret_response.py
```

### Comparing `monday_code-0.0.4/PKG-INFO` & `monday_code-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monday-code
-Version: 0.0.4
+Version: 0.0.5
 Summary: mcode-sdk-api
 Home-page: 
 Author: Monday.Com
 Author-email: support@monday.com
 License: MIT
 Keywords: monday-code
 Description-Content-Type: text/markdown
```

### Comparing `monday_code-0.0.4/README.md` & `monday_code-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/README_FOR_PYPI.md` & `monday_code-0.0.5/README_FOR_PYPI.md`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/__init__.py` & `monday_code-0.0.5/monday_code/__init__.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/api/queue_api.py` & `monday_code-0.0.5/monday_code/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/api/secret_api.py` & `monday_code-0.0.5/monday_code/api/secret_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/api/secure_storage_api.py` & `monday_code-0.0.5/monday_code/api/secure_storage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictStr
+from typing import Any
 from monday_code.models.secure_storage_data_contract import SecureStorageDataContract
 
 from monday_code.api_client import ApiClient, RequestSerialized
 from monday_code.api_response import ApiResponse
 from monday_code.rest import RESTResponseType
 
 
@@ -245,15 +246,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
@@ -496,15 +497,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
@@ -763,15 +764,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
```

### Comparing `monday_code-0.0.4/monday_code/api/storage_api.py` & `monday_code-0.0.5/monday_code/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/api_client.py` & `monday_code-0.0.5/monday_code/api_client.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/api_response.py` & `monday_code-0.0.5/monday_code/api_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/configuration.py` & `monday_code-0.0.5/monday_code/configuration.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/exceptions.py` & `monday_code-0.0.5/monday_code/exceptions.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/__init__.py` & `monday_code-0.0.5/monday_code/models/__init__.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/get_by_key_from_storage404_response.py` & `monday_code-0.0.5/monday_code/models/get_by_key_from_storage404_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/get_by_key_from_storage500_response.py` & `monday_code-0.0.5/monday_code/models/get_by_key_from_storage500_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/increment_counter_params.py` & `monday_code-0.0.5/monday_code/models/increment_counter_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/json_value.py` & `monday_code-0.0.5/monday_code/models/json_value.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/period.py` & `monday_code-0.0.5/monday_code/models/period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/publish_message_params.py` & `monday_code-0.0.5/monday_code/models/publish_message_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/publish_message_response.py` & `monday_code-0.0.5/monday_code/models/publish_message_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/secure_storage_data_contract.py` & `monday_code-0.0.5/monday_code/models/secure_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/storage_data_contract.py` & `monday_code-0.0.5/monday_code/models/storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/validate_secret_params.py` & `monday_code-0.0.5/monday_code/models/validate_secret_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/models/validate_secret_response.py` & `monday_code-0.0.5/monday_code/models/validate_secret_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code/rest.py` & `monday_code-0.0.5/monday_code/rest.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/monday_code.egg-info/PKG-INFO` & `monday_code-0.0.5/monday_code.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monday-code
-Version: 0.0.4
+Version: 0.0.5
 Summary: mcode-sdk-api
 Home-page: 
 Author: Monday.Com
 Author-email: support@monday.com
 License: MIT
 Keywords: monday-code
 Description-Content-Type: text/markdown
```

### Comparing `monday_code-0.0.4/monday_code.egg-info/SOURCES.txt` & `monday_code-0.0.5/monday_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/pyproject.toml` & `monday_code-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/setup.py` & `monday_code-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "monday-code"
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `monday_code-0.0.4/test/test_get_by_key_from_storage404_response.py` & `monday_code-0.0.5/test/test_get_by_key_from_storage404_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_get_by_key_from_storage500_response.py` & `monday_code-0.0.5/test/test_get_by_key_from_storage500_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_increment_counter_params.py` & `monday_code-0.0.5/test/test_increment_counter_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_json_value.py` & `monday_code-0.0.5/test/test_json_value.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_period.py` & `monday_code-0.0.5/test/test_period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_publish_message_params.py` & `monday_code-0.0.5/test/test_publish_message_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_publish_message_response.py` & `monday_code-0.0.5/test/test_publish_message_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_queue_api.py` & `monday_code-0.0.5/test/test_queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_secret_api.py` & `monday_code-0.0.5/test/test_secret_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_secure_storage_api.py` & `monday_code-0.0.5/test/test_secure_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_secure_storage_data_contract.py` & `monday_code-0.0.5/test/test_secure_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_storage_api.py` & `monday_code-0.0.5/test/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_storage_data_contract.py` & `monday_code-0.0.5/test/test_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_validate_secret_params.py` & `monday_code-0.0.5/test/test_validate_secret_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.4/test/test_validate_secret_response.py` & `monday_code-0.0.5/test/test_validate_secret_response.py`

 * *Files identical despite different names*

