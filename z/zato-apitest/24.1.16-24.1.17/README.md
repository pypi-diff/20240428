# Comparing `tmp/zato_apitest-24.1.16.tar.gz` & `tmp/zato_apitest-24.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.16.tar", last modified: Sun Apr 28 08:57:41 2024, max compression
+gzip compressed data, was "zato_apitest-24.1.17.tar", last modified: Sun Apr 28 09:21:40 2024, max compression
```

## Comparing `zato_apitest-24.1.16.tar` & `zato_apitest-24.1.17.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.522915 zato_apitest-24.1.16/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.16/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.16/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.16/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.16/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-28 08:57:41.522915 zato_apitest-24.1.16/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2635 2024-04-28 08:55:45.000000 zato_apitest-24.1.16/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.514915 zato_apitest-24.1.16/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.16/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.16/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4417 2024-04-28 08:57:24.000000 zato_apitest-24.1.16/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.16/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     5139 2024-04-28 07:51:06.000000 zato_apitest-24.1.16/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3094 2024-04-28 08:54:26.000000 zato_apitest-24.1.16/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.16/src/zato/apitest/steps/__init__.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    30995 2024-04-28 08:55:21.000000 zato_apitest-24.1.16/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.16/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.16/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13732 2024-04-28 07:50:51.000000 zato_apitest-24.1.16/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 08:57:41.518915 zato_apitest-24.1.16/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 08:57:39.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 08:57:41.000000 zato_apitest-24.1.16/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.846760 zato_apitest-24.1.17/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.17/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.17/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 09:21:40.846760 zato_apitest-24.1.17/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.17/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.17/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-28 09:21:40.846760 zato_apitest-24.1.17/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2635 2024-04-28 09:21:06.000000 zato_apitest-24.1.17/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.842760 zato_apitest-24.1.17/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.842760 zato_apitest-24.1.17/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.17/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.842760 zato_apitest-24.1.17/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.17/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.17/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.842760 zato_apitest-24.1.17/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.17/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     5203 2024-04-28 09:20:07.000000 zato_apitest-24.1.17/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3094 2024-04-28 08:54:26.000000 zato_apitest-24.1.17/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.842760 zato_apitest-24.1.17/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.17/src/zato/apitest/steps/__init__.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    30995 2024-04-28 08:55:21.000000 zato_apitest-24.1.17/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.17/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.17/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    13732 2024-04-28 07:50:51.000000 zato_apitest-24.1.17/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-28 09:21:40.846760 zato_apitest-24.1.17/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2349 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-28 09:21:38.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-28 09:21:40.000000 zato_apitest-24.1.17/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.16/LICENSE.txt` & `zato_apitest-24.1.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/PKG-INFO` & `zato_apitest-24.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.16
+Version: 24.1.17
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
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.16 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.17 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.16/setup.py` & `zato_apitest-24.1.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Proprietary product. This is not open source software, reproduction is prohibited.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.16'
+version = '24.1.17'
 
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
-version = '24.1.16' LONG_DESCRIPTION = """ Write API tests for your [API
+version = '24.1.17' LONG_DESCRIPTION = """ Write API tests for your [API
 integrations](https://zato.io) in plain English, with no programming needed.
 Here is how it looks: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/
 _r_o_o_t_/_s_t_a_t_i_c_/_i_m_g_/_a_p_i_t_e_s_t_/_a_p_i_t_e_s_t_._j_p_g_) More information about API testing at
 https://zato.io. """ def parse_requirements(requirements): # type: ignore
 ignored = ['#', 'setuptools', '-e'] with open(requirements) as f: return [line
 for line in f if line.strip() and not any(line.startswith(prefix) for prefix in
 ignored)] setup( name = 'zato-apitest', version = version, scripts = ['src/
```

### Comparing `zato_apitest-24.1.16/src/zato/apitest/__init__.py` & `zato_apitest-24.1.17/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato/apitest/cli.py` & `zato_apitest-24.1.17/src/zato/apitest/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,21 +67,22 @@
     sys.exit(_run.handle(path, verbose, ctx.args))
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 @click.command()
 @click.argument('path', default=tempfile.gettempdir(), type=click.Path(exists=True, file_okay=False, resolve_path=True))
+@click.option('-v', '--verbose', is_flag=True)
 @click.pass_context
-def demo(ctx:'Context', path:'str') -> 'None':
+def demo(ctx:'Context', path:'str', verbose:'bool') -> 'None':
     # We're not using tempfile.mkdtemp because we may as well be run
     # in a user-provided directory.
     path = os.path.join(path, 'apitest.' + uuid.uuid4().hex)
     cli_init(ctx, path, False)
-    _ = _run.handle(path, is_verbose=False)
+    _ = _run.handle(path, is_verbose=verbose)
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 main.add_command(init) # type: ignore
 main.add_command(run) # type: ignore
 main.add_command(demo) # type: ignore
```

### Comparing `zato_apitest-24.1.16/src/zato/apitest/init.py` & `zato_apitest-24.1.17/src/zato/apitest/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 '''
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 CONFIG_INI = """
 [behave]
-options=--format pretty
+options=--format pretty --show-timings --no-source --no-logcapture --logging-level=INFO
 
 [user]
 sample=Hello
 """
 
 # ################################################################################################################################
 # ################################################################################################################################
```

### Comparing `zato_apitest-24.1.16/src/zato/apitest/run.py` & `zato_apitest-24.1.17/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato/apitest/steps/common.py` & `zato_apitest-24.1.17/src/zato/apitest/steps/common.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato/apitest/steps/json.py` & `zato_apitest-24.1.17/src/zato/apitest/steps/json.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato/apitest/typing_.py` & `zato_apitest-24.1.17/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato/apitest/util.py` & `zato_apitest-24.1.17/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.16/src/zato_apitest.egg-info/PKG-INFO` & `zato_apitest-24.1.17/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.16
+Version: 24.1.17
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
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.16 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.17 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.16/src/zato_apitest.egg-info/SOURCES.txt` & `zato_apitest-24.1.17/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

