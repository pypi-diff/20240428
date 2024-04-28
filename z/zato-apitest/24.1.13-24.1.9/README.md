# Comparing `tmp/zato_apitest-24.1.13.tar.gz` & `tmp/zato-apitest-24.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.13.tar", last modified: Sat Apr 27 18:48:49 2024, max compression
+gzip compressed data, was "zato-apitest-24.1.9.tar", last modified: Tue Mar 12 11:43:29 2024, max compression
```

## Comparing `zato_apitest-24.1.13.tar` & `zato-apitest-24.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    42880 2019-06-24 21:01:23.000000 zato_apitest-24.1.13/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.13/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.13/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.13/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2635 2024-04-27 18:48:18.000000 zato_apitest-24.1.13/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.525514 zato_apitest-24.1.13/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.525514 zato_apitest-24.1.13/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      227 2024-03-10 13:49:27.000000 zato_apitest-24.1.13/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.525514 zato_apitest-24.1.13/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1816 2024-03-10 14:48:12.000000 zato_apitest-24.1.13/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4343 2024-04-27 18:33:31.000000 zato_apitest-24.1.13/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      226 2024-03-11 14:35:24.000000 zato_apitest-24.1.13/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     5180 2024-04-27 18:33:26.000000 zato_apitest-24.1.13/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1882 2024-03-11 14:38:08.000000 zato_apitest-24.1.13/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      172 2024-03-11 12:18:58.000000 zato_apitest-24.1.13/src/zato/apitest/steps/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    30149 2024-04-27 18:44:22.000000 zato_apitest-24.1.13/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22533 2024-04-26 17:52:57.000000 zato_apitest-24.1.13/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7341 2024-03-11 14:38:39.000000 zato_apitest-24.1.13/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13748 2024-03-11 14:38:52.000000 zato_apitest-24.1.13/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-27 18:48:49.529514 zato_apitest-24.1.13/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-27 18:48:47.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-27 18:48:49.000000 zato_apitest-24.1.13/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    42880 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato-apitest-24.1.9/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato-apitest-24.1.9/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato-apitest-24.1.9/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-03-12 11:43:29.672277 zato-apitest-24.1.9/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2634 2024-03-12 11:43:11.000000 zato-apitest-24.1.9/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      227 2024-03-10 13:49:27.000000 zato-apitest-24.1.9/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1816 2024-03-10 14:48:12.000000 zato-apitest-24.1.9/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4343 2024-03-11 14:35:09.000000 zato-apitest-24.1.9/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      226 2024-03-11 14:35:24.000000 zato-apitest-24.1.9/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4721 2024-03-11 14:47:07.000000 zato-apitest-24.1.9/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1882 2024-03-11 14:38:08.000000 zato-apitest-24.1.9/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      172 2024-03-11 12:18:58.000000 zato-apitest-24.1.9/src/zato/apitest/steps/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29777 2024-03-12 11:41:01.000000 zato-apitest-24.1.9/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22095 2024-03-12 11:34:29.000000 zato-apitest-24.1.9/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7341 2024-03-11 14:38:39.000000 zato-apitest-24.1.9/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13748 2024-03-11 14:38:52.000000 zato-apitest-24.1.9/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-03-12 11:43:29.668277 zato-apitest-24.1.9/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2348 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-03-12 11:43:27.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-03-12 11:43:29.000000 zato-apitest-24.1.9/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.13/LICENSE.txt` & `zato-apitest-24.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/PKG-INFO` & `zato-apitest-24.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.13
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.13 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.13/setup.py` & `zato-apitest-24.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.13'
+version = '24.1.9'
 
 LONG_DESCRIPTION = """
 
 Write API tests for your [API integrations](https://zato.io) in plain English, with no programming needed.
 
 Here is how it looks:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- """ Copyright (C) 2024, Zato Source s.r.o. https://
 zato.io Proprietary product. This is not open source software, reproduction is
 prohibited. """ # stdlib import os from setuptools import setup, find_packages
-version = '24.1.13' LONG_DESCRIPTION = """ Write API tests for your [API
+version = '24.1.9' LONG_DESCRIPTION = """ Write API tests for your [API
 integrations](https://zato.io) in plain English, with no programming needed.
 Here is how it looks: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/
 _r_o_o_t_/_s_t_a_t_i_c_/_i_m_g_/_a_p_i_t_e_s_t_/_a_p_i_t_e_s_t_._j_p_g_) More information about API testing at
 https://zato.io. """ def parse_requirements(requirements): # type: ignore
 ignored = ['#', 'setuptools', '-e'] with open(requirements) as f: return [line
 for line in f if line.strip() and not any(line.startswith(prefix) for prefix in
 ignored)] setup( name = 'zato-apitest', version = version, scripts = ['src/
```

### Comparing `zato_apitest-24.1.13/src/zato/apitest/__init__.py` & `zato-apitest-24.1.9/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/src/zato/apitest/cli.py` & `zato-apitest-24.1.9/src/zato/apitest/cli.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/src/zato/apitest/init.py` & `zato-apitest-24.1.9/src/zato/apitest/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,49 +91,36 @@
     # You can also compare responses directly with files disk
     And response is equal to that from "demo.json"
 """
 
 DEMO_JSON_REQ = """{"hello":"world"}"""
 DEMO_JSON_RESP = """{"action":{"code":0, "msg":"How do you do?", "flow":["Ack", "Done"]}}"""
 
-Demo_XML = """<?xml version="1.0" encoding="UTF-8"?><root/>"""
-
 # ################################################################################################################################
 # ################################################################################################################################
 
 def handle(base_path:'str') -> 'None':
     """ Sets up runtime directories and sample features.
     """
     # Top-level directory for tests
     features_dir = os.path.join(base_path, 'features')
     os.mkdir(features_dir)
 
     # Requests and responses
     request_json_dir = os.path.join(base_path, 'features', 'json', 'request')
     response_json_dir = os.path.join(base_path, 'features', 'json', 'response')
 
-    request_xml_dir = os.path.join(base_path, 'features', 'xml', 'request')
-    response_xml_dir = os.path.join(base_path, 'features', 'xml', 'response')
-
     os.makedirs(request_json_dir)
     os.makedirs(response_json_dir)
 
-    os.makedirs(request_xml_dir)
-    os.makedirs(response_xml_dir)
-
     # Demo feature
     _ = open(os.path.join(features_dir, 'demo.feature'), 'w').write(DEMO_FEATURE)
     _ = open(os.path.join(request_json_dir, 'demo.json'), 'w').write(DEMO_JSON_REQ)
     _ = open(os.path.join(response_json_dir, 'demo.json'), 'w').write(DEMO_JSON_RESP)
 
-    # Demo XML
-
-    _ = open(os.path.join(request_xml_dir, 'demo.xml'), 'w').write(Demo_XML)
-    _ = open(os.path.join(response_xml_dir, 'demo.xml'), 'w').write(Demo_XML)
-
     # Add environment.py
     _ = open(os.path.join(features_dir, 'environment.py'), 'w').write(ENVIRONMENT)
 
     # Add steps
     steps_dir = os.path.join(features_dir, 'steps')
     os.mkdir(steps_dir)
     _ = open(os.path.join(steps_dir, 'steps.py'), 'w').write(STEPS)
```

### Comparing `zato_apitest-24.1.13/src/zato/apitest/run.py` & `zato-apitest-24.1.9/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/src/zato/apitest/steps/common.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,62 +72,53 @@
             # If no response_format is set, assume it's the same as the request format.
             # If the request format hasn't been specified either, assume 'RAW'.
             response_format = ctx.zato.request.get('response_format', ctx.zato.request.get('format', 'JSON'))
 
             if response_format == 'JSON':
                 ctx.zato.response.data_impl = json.loads(ctx.zato.response.data_text)
 
-            elif response_format in {'RAW', 'FORM', 'XML'}:
+            elif response_format == 'RAW':
+                ctx.zato.response.data_impl = ctx.zato.response.data_text
+
+            elif response_format == 'FORM':
                 ctx.zato.response.data_impl = ctx.zato.response.data_text
 
     except Exception as e:
         logger.warn('Caught an exception while invoking `%s` with `%s`; req=`%s`; resp=`%s`, (%s)',
             ctx.zato.full_address, ctx.zato.request.method, ctx.zato.request.data, response_data, e.args[0])
         raise
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-@when('this scenario is invoked')
-def when_this_scenario_is_invoked(ctx:'Context', adapters:'anylistnone'=None) -> 'None':
-    pass
-
-# ################################################################################################################################
-# ################################################################################################################################
-
 def invoke_http(ctx:'Context', adapters:'anylistnone'=None) -> 'None':
 
     adapters = adapters or []
     method = ctx.zato.request.get('method', 'GET')
     address = ctx.zato.request.get('address')
     url_path = ctx.zato.request.get('url_path', '/')
     qs = ctx.zato.request.get('query_string', '')
     files = None
     data = ''
 
     if 'data_impl' in ctx.zato.request:
-        if ctx.zato.request.get('is_xml'):
+        if ctx.zato.request.is_xml:
             data = etree.tostring(ctx.zato.request.data_impl)
-        elif ctx.zato.request.get('is_json'):
+        elif ctx.zato.request.is_json:
             data = json.dumps(ctx.zato.request.data_impl, indent=2)
             ctx.zato.request.headers['Content-Type'] = 'application/json'
-        elif ctx.zato.request.get('is_raw'):
+        elif ctx.zato.request.is_raw:
             data = ctx.zato.request.data_impl
-        elif ctx.zato.request.get('is_form'):
+        elif ctx.zato.request.is_form:
             data = ctx.zato.request.get('form', '')
             files = ctx.zato.request.get('files', None)
             ctx.zato.request.headers['Content-Type'] = 'application/x-www-form-urlencoded'
-
             if files is not None:
                 # multipart/formdata should let requests set the content-type header
                 del ctx.zato.request.headers['Content-Type']
-        else:
-            # Default to JSON
-            data = json.dumps(ctx.zato.request.data_impl, indent=2)
-            ctx.zato.request.headers['Content-Type'] = 'application/json'
 
     ctx.zato.request.method = method
     ctx.zato.request.data = data
     ctx.zato.full_address = '{}{}{}'.format(address, url_path, qs)
 
     auth = None
 
@@ -235,19 +226,17 @@
 
     ctx.zato.request.data = data
 
     if ctx.zato.request.get('is_json'):
         ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
     elif ctx.zato.request.get('is_raw'):
         ctx.zato.request.data_impl = ctx.zato.request.data
-    elif ctx.zato.request.get('is_xml'):
-        data = ctx.zato.request.data.encode('utf8')
-        ctx.zato.request.data_impl = etree.fromstring(data) # type: ignore
     else:
-        ctx.zato.request.data_impl = json.loads(ctx.zato.request.data)
+        if not ctx.zato.request.format:
+            raise ValueError('Format not set, cannot proceed')
 
 # ################################################################################################################################
 
 @given('request "{request_path}"')
 @util.obtain_values
 def given_request(ctx:'Context', request_path:'str') -> 'None':
     return given_request_impl(ctx, util.get_data(ctx, 'request', request_path))
@@ -274,15 +263,15 @@
 
     files[name] = open(full_path, 'rb')
 
     ctx.zato.request.files = files
 
 # ################################################################################################################################
 
-@given('form field "{name}" is "{value}"')
+@given('request param "{name}" is "{value}"')
 @util.obtain_values
 def given_request_param(ctx:'Context', name:'str', value:'any_') -> 'None':
     ctx.zato.request.data_impl = None
     form = ctx.zato.request.get('form', {})
     if name in form:
         if isinstance(form[name], list):
             form[name].append(value)
@@ -356,22 +345,14 @@
 @util.obtain_values
 def given_i_store_a_random_date_under_name(ctx:'Context', name:'str', format:'str') -> 'None':
     ctx.zato.user_ctx[name] = util.rand_date(ctx.zato.date_formats[format])
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-@given('I encode "{value}" using Base64 under "{name}"')
-@util.obtain_values
-def given_i_encode_value_using_base64_under_name(ctx:'Context', value:'str', name:'str') -> 'None':
-    ctx.zato.user_ctx[name] = value.encode('base64','strict')
-
-# ################################################################################################################################
-# ################################################################################################################################
-
 @then('context is cleaned up')
 @util.obtain_values
 def then_context_is_cleaned_up(ctx:'Context') -> 'None':
     ctx.zato = util.new_context(ctx, '')
 
 # ################################################################################################################################
 
@@ -511,15 +492,15 @@
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 @then('I store "{path}" from response under "{name}", default "{default}"')
 @util.obtain_values
 def then_store_path_under_name_with_default(ctx:'Context', path:'str', name:'str', default:'str') -> 'None':
-    if ctx.zato.request.get('is_xml'):
+    if ctx.zato.request.is_xml:
         value = ctx.zato.response.data_impl.xpath(path)
         if value:
             if len(value) == 1:
                 value = value[0].text
             else:
                 value = [elem.text for elem in value]
         else:
@@ -556,40 +537,54 @@
 def _response_is_equal_to(ctx:'Context', expected:'any_') -> 'bool':
     assert_equals(expected, ctx.zato.response.data_impl)
     return True
 
 # ################################################################################################################################
 
 @then('response is equal to that from "{path}"')
+@needs_json
 @util.obtain_values
 def then_response_is_equal_to_that_from(ctx:'Context', path:'str') -> 'bool':
-    data = util.get_data(ctx, 'response', path)
-    if ctx.zato.request.is_json:
-        data = json.loads(data)
-    return _response_is_equal_to(ctx, data)
+    return _response_is_equal_to(ctx, json.loads(util.get_data(ctx, 'response', path)))
 
 # ################################################################################################################################
 
 @then('JSON response is equal to "{expected}"')
 @needs_json
 @util.obtain_values
 def then_response_is_equal_to(ctx:'Context', expected:'any_') -> 'bool':
     return _response_is_equal_to(ctx, json.loads(expected))
 
 # ################################################################################################################################
+
+#@then('response is equal to "{expected}"')
+#@needs_json
+#@util.obtain_values
+#def then_response_is_equal_to(ctx:'Context', expected:'any_') -> 'None':
+#    return _response_is_equal_to(ctx, expected)
+
+# ################################################################################################################################
 # ################################################################################################################################
 
 @then('I sleep for "{sleep_time}"')
 @util.obtain_values
 def then_i_sleep_for(ctx:'Context', sleep_time:'int') -> 'None':
     time.sleep(float(sleep_time))
 
 # ################################################################################################################################
 # ################################################################################################################################
 
+@given('I encode "{value}" using Base64 under "{name}"')
+@util.obtain_values
+def given_i_encode_value_using_base64_under_name(ctx:'Context', value:'str', name:'str') -> 'None':
+    ctx.zato.user_ctx[name] = value.encode('base64','strict')
+
+# ################################################################################################################################
+# ################################################################################################################################
+
 def variable_is(variable:'any_', value:'any_') -> 'None':
     expected_value = ast.literal_eval(value)
     assert variable == expected_value, 'Value `{}` is not equal to expected `{}`'.format(variable, expected_value)
 
 # ################################################################################################################################
 
 @then('variable "{variable}" is a list "{value}"')
```

### Comparing `zato_apitest-24.1.13/src/zato/apitest/steps/json.py` & `zato-apitest-24.1.9/src/zato/apitest/steps/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,23 +276,14 @@
     actual = get_pointer(ctx.zato.response.data_impl, path)
     assert isinstance(actual, bool), \
         'Expected a bool in {}, got a `{}`'.format(path, type(actual))
     return True
 
 # ################################################################################################################################
 
-@then('path "{path}" is any string')
-@util.obtain_values
-def then_json_pointer_is_any_string(ctx:'Context', path:'str') -> 'bool':
-    actual = get_pointer(ctx.zato.response.data_impl, path)
-    assert isinstance(actual, str), 'Expected a str in {}, got a `{}`'.format(path, type(actual))
-    return True
-
-# ################################################################################################################################
-
 @then('path "{path}" is a list "{value}"')
 @util.obtain_values
 def then_json_pointer_is_a_list(ctx:'Context', path:'str', value:'any_') -> 'bool':
     return assert_value(ctx, path, value, util.parse_list)
 
 # ################################################################################################################################
```

### Comparing `zato_apitest-24.1.13/src/zato/apitest/typing_.py` & `zato-apitest-24.1.9/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/src/zato/apitest/util.py` & `zato-apitest-24.1.9/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.13/src/zato_apitest.egg-info/PKG-INFO` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.13
+Version: 24.1.9
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.13 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.9 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.13/src/zato_apitest.egg-info/SOURCES.txt` & `zato-apitest-24.1.9/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

