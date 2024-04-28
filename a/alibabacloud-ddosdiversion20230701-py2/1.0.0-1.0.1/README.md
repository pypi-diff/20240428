# Comparing `tmp/alibabacloud_ddosdiversion20230701_py2-1.0.0.tar.gz` & `tmp/alibabacloud_ddosdiversion20230701_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ddosdiversion20230701_py2-1.0.0.tar", last modified: Wed Dec 13 02:14:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ddosdiversion20230701_py2-1.0.1.tar", last modified: Sun Apr 28 06:56:15 2024, max compression
```

## Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0.tar` & `alibabacloud_ddosdiversion20230701_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2532 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1063 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1146 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5545 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/client.py
--rw-r--r--   0 root         (0) root         (0)    32228 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2532 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2953 2023-12-13 02:14:21.000000 alibabacloud_ddosdiversion20230701_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/client.py
+-rw-r--r--   0 root         (0) root         (0)    33912 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      520 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-28 06:56:15.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2953 2024-04-28 06:56:14.000000 alibabacloud_ddosdiversion20230701_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/LICENSE` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/PKG-INFO` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ddosdiversion20230701_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DdosDiversion (20230701) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/README-CN.md` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/README.md` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/client.py` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701/models.py` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class ConfigNetStatusRequest(TeaModel):
     def __init__(self, net=None, regions=None, sale_id=None, status=None, sub_nets=None):
+        # The CIDR block of the anti-DDoS diversion instance.
         self.net = net  # type: str
+        # The regions in which the CIDR block needs to be advertised or withdrawn from advertising. If you leave this parameter empty, the CIDR blocks in all regions are configured.
+        # 
+        # >  You can call the [QueryNetList](~~2639086~~) operation to obtain the regions of the CIDR blocks.
         self.regions = regions  # type: list[str]
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id  # type: str
+        # The status of the CIDR block. Valid values:
+        # 
+        # *   enable: advertises the CIDR block.
+        # *   disable: withdraws the advertising of the CIDR block.
         self.status = status  # type: str
+        # The subnet CIDR blocks of the CIDR block.
         self.sub_nets = sub_nets  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ConfigNetStatusRequest, self).to_map()
@@ -45,16 +55,22 @@
         if m.get('SubNets') is not None:
             self.sub_nets = m.get('SubNets')
         return self
 
 
 class ConfigNetStatusResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code  # type: long
+        # The response parameters.
         self.message = message  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ConfigNetStatusResponseBody, self).to_map()
@@ -84,17 +100,14 @@
 class ConfigNetStatusResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ConfigNetStatusResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ConfigNetStatusResponse, self).to_map()
         if _map is not None:
             return _map
@@ -118,18 +131,28 @@
             temp_model = ConfigNetStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstanceRequest(TeaModel):
     def __init__(self, name=None, num=None, page=None, sale_id=None, status=None):
+        # The name of the instance.
         self.name = name  # type: str
+        # The number of entries per page. Default value: 100.
         self.num = num  # type: long
+        # The page number. Default value: 1
         self.page = page  # type: long
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id  # type: str
+        # The status of the instance. Valid values:
+        # 
+        # *   normal
+        # *   expired
+        # *   deleting
+        # *   stopped
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstanceRequest, self).to_map()
@@ -367,69 +390,67 @@
         if m.get('Total') is not None:
             self.total = m.get('Total')
         return self
 
 
 class ListInstanceResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code  # type: long
-        self.data = data  # type: list[ListInstanceResponseBodyData]
+        # The returned result.
+        self.data = data  # type: ListInstanceResponseBodyData
+        # The response parameters.
         self.message = message  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
+            self.data.validate()
 
     def to_map(self):
         _map = super(ListInstanceResponseBody, self).to_map()
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
 
     def from_map(self, m=None):
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
 
 
 class ListInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -453,19 +474,30 @@
             temp_model = ListInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryNetListRequest(TeaModel):
     def __init__(self, main_net=None, mode=None, net=None, num=None, page=None, sale_id=None):
+        # The primary CIDR block of the anti-DDoS diversion instance for which an extended CIDR block is configured. If no extended CIDR blocks are configured for the anti-DDoS diversion instance, leave this parameter empty.
         self.main_net = main_net  # type: str
+        # The scheduling mode. Valid values:
+        # 
+        # *   manual: manual scheduling
+        # *   netflow-auto: automatic scheduling
         self.mode = mode  # type: str
+        # The CIDR block of the anti-DDoS diversion instance.
+        # 
+        # >  If no extended CIDR blocks are configured for the anti-DDoS diversion instance, this parameter specifies the CIDR block of the instance. If an extended CIDR block is configured for the anti-DDoS diversion instance, this parameter specifies the extended CIDR block that is configured for the instance. If this parameter is specified, the MainNet parameter is required.
         self.net = net  # type: str
+        # The number of entries per page. Default value: 100.
         self.num = num  # type: long
+        # The page number. Default value: 1
         self.page = page  # type: long
+        # The ID of the anti-DDoS diversion instance.
         self.sale_id = sale_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(QueryNetListRequest, self).to_map()
@@ -502,17 +534,15 @@
         if m.get('SaleId') is not None:
             self.sale_id = m.get('SaleId')
         return self
 
 
 class QueryNetListResponseBodyDataNetsDDoSDefenseCleanTh(TeaModel):
     def __init__(self, mbps=None, pps=None):
-        # Mbps。
         self.mbps = mbps  # type: int
-        # Pps。
         self.pps = pps  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(QueryNetListResponseBodyDataNetsDDoSDefenseCleanTh, self).to_map()
@@ -662,16 +692,16 @@
         self.declared = declared  # type: list[QueryNetListResponseBodyDataNetsDeclared]
         self.declared_state = declared_state  # type: int
         self.fwd_effect = fwd_effect  # type: long
         self.gmt_create = gmt_create  # type: str
         self.gmt_modify = gmt_modify  # type: str
         self.mode = mode  # type: str
         self.net = net  # type: str
-        self.net_extend = net_extend  # type: long
-        self.net_main = net_main  # type: str
+        self.net_extend = net_extend  # type: str
+        self.net_main = net_main  # type: long
         self.net_type = net_type  # type: str
         self.sale_id = sale_id  # type: str
         self.upstream_type = upstream_type  # type: str
         self.user_id = user_id  # type: str
 
     def validate(self):
         if self.ddo_sdefense:
@@ -801,69 +831,67 @@
         if m.get('Total') is not None:
             self.total = m.get('Total')
         return self
 
 
 class QueryNetListResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
+        # The status code.
+        # 
+        # *   **200**: The request was successful.
+        # *   Other codes: The request failed.
         self.code = code  # type: long
-        self.data = data  # type: list[QueryNetListResponseBodyData]
+        # The CIDR blocks.
+        self.data = data  # type: QueryNetListResponseBodyData
+        # The response parameters.
         self.message = message  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
+            self.data.validate()
 
     def to_map(self):
         _map = super(QueryNetListResponseBody, self).to_map()
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
 
     def from_map(self, m=None):
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
 
 
 class QueryNetListResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: QueryNetListResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(QueryNetListResponse, self).to_map()
         if _map is not None:
             return _map
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/alibabacloud_ddosdiversion20230701_py2.egg-info/PKG-INFO` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/alibabacloud_ddosdiversion20230701_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ddosdiversion20230701-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DdosDiversion (20230701) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddosdiversion20230701_py2-1.0.0/setup.py` & `alibabacloud_ddosdiversion20230701_py2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ddosdiversion20230701_py2.
 
-Created on 13/12/2023
+Created on 28/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ddosdiversion20230701"
 NAME = "alibabacloud_ddosdiversion20230701_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DdosDiversion (20230701) SDK Library for Python2"
```

