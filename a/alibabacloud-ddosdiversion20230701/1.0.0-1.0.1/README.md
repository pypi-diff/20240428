# Comparing `tmp/alibabacloud_ddosdiversion20230701-1.0.0.tar.gz` & `tmp/alibabacloud_ddosdiversion20230701-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ddosdiversion20230701-1.0.0.tar", last modified: Wed Dec 13 02:14:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ddosdiversion20230701-1.0.1.tar", last modified: Sun Apr 28 06:56:52 2024, max compression
```

## Comparing `alibabacloud_ddosdiversion20230701-1.0.0.tar` & `alibabacloud_ddosdiversion20230701-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11744 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/client.py
--rw-r--r--   0 root         (0) root         (0)    32064 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2661 2023-12-13 02:14:06.000000 alibabacloud_ddosdiversion20230701-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11744 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/client.py
+-rw-r--r--   0 root         (0) root         (0)    33748 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-04-28 06:56:52.000000 alibabacloud_ddosdiversion20230701-1.0.1/setup.py
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/LICENSE` & `alibabacloud_ddosdiversion20230701-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/PKG-INFO` & `alibabacloud_ddosdiversion20230701-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ddosdiversion20230701
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DdosDiversion (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ddosdiversion-20230701/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/README-CN.md` & `alibabacloud_ddosdiversion20230701-1.0.1/README-CN.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ddosdiversion-20230701/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/README.md` & `alibabacloud_ddosdiversion20230701-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ddosdiversion-20230701/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/client.py` & `alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701/models.py` & `alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,28 @@
         self,
         net: str = None,
         regions: List[str] = None,
         sale_id: str = None,
         status: str = None,
         sub_nets: List[str] = None,
     ):
+        # The CIDR block of the anti-DDoS diversion instance.
         self.net = net
+        # The regions in which the CIDR block needs to be advertised or withdrawn from advertising. If you leave this parameter empty, the CIDR blocks in all regions are configured.
+        # 
+        # >  You can call the [QueryNetList](~~2639086~~) operation to obtain the regions of the CIDR blocks.
         self.regions = regions
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id
+        # The status of the CIDR block. Valid values:
+        # 
+        # *   enable: advertises the CIDR block.
+        # *   disable: withdraws the advertising of the CIDR block.
         self.status = status
+        # The subnet CIDR blocks of the CIDR block.
         self.sub_nets = sub_nets
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -58,16 +68,22 @@
 class ConfigNetStatusResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
     ):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code
+        # The response parameters.
         self.message = message
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -102,17 +118,14 @@
         body: ConfigNetStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -143,18 +156,28 @@
         self,
         name: str = None,
         num: int = None,
         page: int = None,
         sale_id: str = None,
         status: str = None,
     ):
+        # The name of the instance.
         self.name = name
+        # The number of entries per page. Default value: 100.
         self.num = num
+        # The page number. Default value: 1
         self.page = page
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id
+        # The status of the instance. Valid values:
+        # 
+        # *   normal
+        # *   expired
+        # *   deleting
+        # *   stopped
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -424,56 +447,57 @@
         return self
 
 
 class ListInstanceResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
-        data: List[ListInstanceResponseBodyData] = None,
+        data: ListInstanceResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code
+        # The returned result.
         self.data = data
+        # The response parameters.
         self.message = message
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
+            self.data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
-        result['Data'] = []
         if self.data is not None:
-            for k in self.data:
-                result['Data'].append(k.to_map() if k else None)
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        self.data = []
         if m.get('Data') is not None:
-            for k in m.get('Data'):
-                temp_model = ListInstanceResponseBodyData()
-                self.data.append(temp_model.from_map(k))
+            temp_model = ListInstanceResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -485,17 +509,14 @@
         body: ListInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -527,19 +548,30 @@
         main_net: str = None,
         mode: str = None,
         net: str = None,
         num: int = None,
         page: int = None,
         sale_id: str = None,
     ):
+        # The primary CIDR block of the anti-DDoS diversion instance for which an extended CIDR block is configured. If no extended CIDR blocks are configured for the anti-DDoS diversion instance, leave this parameter empty.
         self.main_net = main_net
+        # The scheduling mode. Valid values:
+        # 
+        # *   manual: manual scheduling
+        # *   netflow-auto: automatic scheduling
         self.mode = mode
+        # The CIDR block of the anti-DDoS diversion instance.
+        # 
+        # >  If no extended CIDR blocks are configured for the anti-DDoS diversion instance, this parameter specifies the CIDR block of the instance. If an extended CIDR block is configured for the anti-DDoS diversion instance, this parameter specifies the extended CIDR block that is configured for the instance. If this parameter is specified, the MainNet parameter is required.
         self.net = net
+        # The number of entries per page. Default value: 100.
         self.num = num
+        # The page number. Default value: 1
         self.page = page
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -580,17 +612,15 @@
 
 class QueryNetListResponseBodyDataNetsDDoSDefenseCleanTh(TeaModel):
     def __init__(
         self,
         mbps: int = None,
         pps: int = None,
     ):
-        # Mbps。
         self.mbps = mbps
-        # Pps。
         self.pps = pps
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -754,16 +784,16 @@
         declared: List[QueryNetListResponseBodyDataNetsDeclared] = None,
         declared_state: int = None,
         fwd_effect: int = None,
         gmt_create: str = None,
         gmt_modify: str = None,
         mode: str = None,
         net: str = None,
-        net_extend: int = None,
-        net_main: str = None,
+        net_extend: str = None,
+        net_main: int = None,
         net_type: str = None,
         sale_id: str = None,
         upstream_type: str = None,
         user_id: str = None,
     ):
         self.ddo_sdefense = ddo_sdefense
         self.declared = declared
@@ -916,56 +946,57 @@
         return self
 
 
 class QueryNetListResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
-        data: List[QueryNetListResponseBodyData] = None,
+        data: QueryNetListResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code
+        # The CIDR blocks.
         self.data = data
+        # The response parameters.
         self.message = message
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
+            self.data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
-        result['Data'] = []
         if self.data is not None:
-            for k in self.data:
-                result['Data'].append(k.to_map() if k else None)
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        self.data = []
         if m.get('Data') is not None:
-            for k in m.get('Data'):
-                temp_model = QueryNetListResponseBodyData()
-                self.data.append(temp_model.from_map(k))
+            temp_model = QueryNetListResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -977,17 +1008,14 @@
         body: QueryNetListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/alibabacloud_ddosdiversion20230701.egg-info/PKG-INFO` & `alibabacloud_ddosdiversion20230701-1.0.1/alibabacloud_ddosdiversion20230701.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ddosdiversion20230701
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DdosDiversion (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ddosdiversion-20230701/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ddosdiversion20230701-1.0.0/setup.py` & `alibabacloud_ddosdiversion20230701-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ddosdiversion20230701.
 
-Created on 13/12/2023
+Created on 28/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ddosdiversion20230701"
 NAME = "alibabacloud_ddosdiversion20230701" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DdosDiversion (20230701) SDK Library for Python"
```

