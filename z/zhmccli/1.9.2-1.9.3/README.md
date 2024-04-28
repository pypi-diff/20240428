# Comparing `tmp/zhmccli-1.9.2.tar.gz` & `tmp/zhmccli-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmccli-1.9.2.tar", last modified: Mon Dec 18 13:28:49 2023, max compression
+gzip compressed data, was "zhmccli-1.9.3.tar", last modified: Tue Feb 13 14:47:33 2024, max compression
```

## Comparing `zhmccli-1.9.2.tar` & `zhmccli-1.9.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:28:49.633606 zhmccli-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2023-12-18 13:28:11.000000 zhmccli-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-18 13:28:41.000000 zhmccli-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-12-18 13:28:49.633606 zhmccli-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-12-18 13:28:11.000000 zhmccli-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-18 13:28:11.000000 zhmccli-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 13:28:49.633606 zhmccli-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-12-18 13:28:11.000000 zhmccli-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:28:49.633606 zhmccli-1.9.2/zhmccli/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21540 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17175 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_capacitygroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14942 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_character_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14450 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    43110 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_cpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11106 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_hba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    34913 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_lpar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25429 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    22579 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_nic.py
--rw-r--r--   0 runner    (1001) docker     (127)    92768 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_storagegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18150 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_storagevolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    47796 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23920 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13031 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_vfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_vstorageresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_cmd_vswitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    56577 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16936 2023-12-18 13:28:11.000000 zhmccli-1.9.2/zhmccli/zhmccli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:28:49.633606 zhmccli-1.9.2/zhmccli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:28:49.000000 zhmccli-1.9.2/zhmccli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:47:33.562971 zhmccli-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-02-13 14:46:50.000000 zhmccli-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-13 14:47:24.000000 zhmccli-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-02-13 14:47:33.562971 zhmccli-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-13 14:46:50.000000 zhmccli-1.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-13 14:46:50.000000 zhmccli-1.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 14:47:33.562971 zhmccli-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-02-13 14:46:50.000000 zhmccli-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:47:33.558971 zhmccli-1.9.3/zhmccli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17175 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_capacitygroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14919 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_character_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43110 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_hba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25429 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_nic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92768 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_storagegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18150 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_storagevolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48089 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23920 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13031 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_vfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_vstorageresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_cmd_vswitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56577 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16936 2024-02-13 14:46:50.000000 zhmccli-1.9.3/zhmccli/zhmccli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:47:33.562971 zhmccli-1.9.3/zhmccli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:47:33.000000 zhmccli-1.9.3/zhmccli.egg-info/zip-safe
```

### Comparing `zhmccli-1.9.2/LICENSE` & `zhmccli-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/MANIFEST.in` & `zhmccli-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/PKG-INFO` & `zhmccli-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.9.2
+Version: 1.9.3
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -39,16 +39,17 @@
 Requires-Dist: click-spinner>=0.1.6
 Requires-Dist: progressbar2>=3.12.0
 Requires-Dist: six>=1.14.0; python_version <= "3.9"
 Requires-Dist: six>=1.16.0; python_version >= "3.10"
 Requires-Dist: tabulate>=0.8.2; python_version <= "3.9"
 Requires-Dist: tabulate>=0.8.8; python_version >= "3.10"
 Requires-Dist: python-dateutil>=2.8.2
-Requires-Dist: prompt-toolkit<2.0.0,>=1.0.15; python_version == "2.7"
-Requires-Dist: prompt-toolkit>=2.0.1; python_version >= "3.5"
+Requires-Dist: prompt-toolkit>=1.0.15; python_version == "2.7"
+Requires-Dist: prompt-toolkit>=2.0.1; python_version == "3.5"
+Requires-Dist: prompt-toolkit>=3.0.13; python_version >= "3.6"
 Requires-Dist: PyYAML>=5.3.1; python_version <= "3.5"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: jsonschema>=3.0.1
 Requires-Dist: yamlloader>=0.5.5
 Requires-Dist: urllib3>=1.26.9; python_version == "3.5"
 Requires-Dist: urllib3>=1.26.18; python_version >= "3.6"
```

### Comparing `zhmccli-1.9.2/README.rst` & `zhmccli-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/requirements.txt` & `zhmccli-1.9.3/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 six>=1.14.0; python_version <= '3.9' # MIT
 six>=1.16.0; python_version >= '3.10' # MIT
 tabulate>=0.8.2; python_version <= '3.9' # MIT
 tabulate>=0.8.8; python_version >= '3.10' # MIT
 python-dateutil>=2.8.2  # Apache, BSD
 
 # prompt-toolkit is pulled in by click-repl.
-# prompt-toolkit>=2.0 conflicts with ipython and jupyter-console.
 # prompt-toolkit>=3.0 does not support py27.
-prompt-toolkit>=1.0.15,<2.0.0; python_version == '2.7'
-prompt-toolkit>=2.0.1; python_version >= '3.5'
+prompt-toolkit>=1.0.15; python_version == '2.7'
+prompt-toolkit>=2.0.1; python_version == '3.5'
+prompt-toolkit>=3.0.13; python_version >= '3.6'
 
 # PyYAML 5.3 has removed support for Python 3.4
 # PyYAML 5.3 fixed narrow build error on Python 2.7
 # PyYAML 5.3.1 addressed issue 38100 reported by safety
 # PyYAML 5.2 addressed issue 38639 reported by safety
 # PyYAML 5.4 fixes safety issue 39611
 # PyYAML 5.3 has wheel archives for Python 2.7, 3.5 - 3.9
```

### Comparing `zhmccli-1.9.2/setup.py` & `zhmccli-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/__init__.py` & `zhmccli-1.9.3/zhmccli/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_adapter.py` & `zhmccli-1.9.3/zhmccli/_cmd_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_capacitygroup.py` & `zhmccli-1.9.3/zhmccli/_cmd_capacitygroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_certificates.py` & `zhmccli-1.9.3/zhmccli/_cmd_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_character_rule.py` & `zhmccli-1.9.3/zhmccli/_cmd_character_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,14 @@
         'index',
         'min-characters',
         'max-characters',
         'alphabetic',
         'numeric',
         'special',
         'custom-character-sets',
-        'description',
     ]
 
     additions = {}
     additions['index'] = {}
 
     password_rule = find_password_rule(cmd_ctx, console, password_rule_name)
     character_rules = password_rule.get_property('character-rules')
```

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_console.py` & `zhmccli-1.9.3/zhmccli/_cmd_console.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_cpc.py` & `zhmccli-1.9.3/zhmccli/_cmd_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_hba.py` & `zhmccli-1.9.3/zhmccli/_cmd_hba.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_info.py` & `zhmccli-1.9.3/zhmccli/_cmd_info.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_ldap_server_definition.py` & `zhmccli-1.9.3/zhmccli/_cmd_ldap_server_definition.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_lpar.py` & `zhmccli-1.9.3/zhmccli/_cmd_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_metrics.py` & `zhmccli-1.9.3/zhmccli/_cmd_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_nic.py` & `zhmccli-1.9.3/zhmccli/_cmd_nic.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_partition.py` & `zhmccli-1.9.3/zhmccli/_cmd_partition.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_password_rule.py` & `zhmccli-1.9.3/zhmccli/_cmd_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_port.py` & `zhmccli-1.9.3/zhmccli/_cmd_port.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_session.py` & `zhmccli-1.9.3/zhmccli/_cmd_session.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_storagegroup.py` & `zhmccli-1.9.3/zhmccli/_cmd_storagegroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_storagevolume.py` & `zhmccli-1.9.3/zhmccli/_cmd_storagevolume.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_unmanaged_cpc.py` & `zhmccli-1.9.3/zhmccli/_cmd_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_user.py` & `zhmccli-1.9.3/zhmccli/_cmd_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,35 +761,39 @@
         # - mfa-userid-override
         like_props = {}
         _update(like_props, like_user, 'type')
         _update(like_props, like_user, 'disabled')
         _update(like_props, like_user, 'authentication-type')
         _update(like_props, like_user, 'password-rule-uri')
         _update(like_props, like_user, 'force-password-change')
-        _update(like_props, like_user, 'ldap-server-definition-uri')
-        _update(like_props, like_user, 'userid-on-ldap-server')
+        if like_user.get_property('authentication-type') == 'ldap':
+            # Specifying those for non-LDAP users fails
+            _update(like_props, like_user, 'ldap-server-definition-uri')
+            _update(like_props, like_user, 'userid-on-ldap-server')
         _update(like_props, like_user, 'session-timeout')
         _update(like_props, like_user, 'verify-timeout')
         _update(like_props, like_user, 'idle-timeout')
-        _update(like_props, like_user, 'min-pw-change-time')
+        if like_user.get_property('authentication-type') == 'local':
+            _update(like_props, like_user, 'min-pw-change-time')
         _update(like_props, like_user, 'max-failed-logins')
         _update(like_props, like_user, 'disable-delay')
         _update(like_props, like_user, 'inactivity-timeout')
         _update(like_props, like_user, 'disruptive-pw-required')
         _update(like_props, like_user, 'disruptive-text-required')
         _update(like_props, like_user, 'allow-remote-access')
         _update(like_props, like_user, 'allow-management-interfaces')
         _update(like_props, like_user, 'max-web-services-api-sessions')
         _update(like_props, like_user, 'web-services-api-session-idle-timeout')
         _update(like_props, like_user, 'multi-factor-authentication-required')
-        # The following are only present if mfa required:
-        _update(like_props, like_user, 'mfa-types')
-        _update(like_props, like_user, 'primary-mfa-server-definition-uri')
-        _update(like_props, like_user, 'backup-mfa-server-definition-uri')
-        _update(like_props, like_user, 'mfa-policy')
+        if like_user.get_property('multi-factor-authentication-required'):
+            # Specifying those for non-MFA users fails
+            _update(like_props, like_user, 'mfa-types')
+            _update(like_props, like_user, 'primary-mfa-server-definition-uri')
+            _update(like_props, like_user, 'backup-mfa-server-definition-uri')
+            _update(like_props, like_user, 'mfa-policy')
 
     # Determine user properties from options
 
     option_props = options_to_properties(org_options, name_map)
 
     if org_options['password-rule'] in (None, ''):
         pass  # omit -> HMC sets to default
```

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_user_role.py` & `zhmccli-1.9.3/zhmccli/_cmd_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_vfunction.py` & `zhmccli-1.9.3/zhmccli/_cmd_vfunction.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_vstorageresource.py` & `zhmccli-1.9.3/zhmccli/_cmd_vstorageresource.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_cmd_vswitch.py` & `zhmccli-1.9.3/zhmccli/_cmd_vswitch.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_helper.py` & `zhmccli-1.9.3/zhmccli/_helper.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli/_version.py` & `zhmccli-1.9.3/zhmccli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.U.dev1": A not yet released version M.N.U
 #: * "M.N.U": A released version M.N.U
-__version__ = '1.9.2'
+__version__ = '1.9.3'
```

### Comparing `zhmccli-1.9.2/zhmccli/zhmccli.py` & `zhmccli-1.9.3/zhmccli/zhmccli.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli.egg-info/PKG-INFO` & `zhmccli-1.9.3/zhmccli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.9.2
+Version: 1.9.3
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -39,16 +39,17 @@
 Requires-Dist: click-spinner>=0.1.6
 Requires-Dist: progressbar2>=3.12.0
 Requires-Dist: six>=1.14.0; python_version <= "3.9"
 Requires-Dist: six>=1.16.0; python_version >= "3.10"
 Requires-Dist: tabulate>=0.8.2; python_version <= "3.9"
 Requires-Dist: tabulate>=0.8.8; python_version >= "3.10"
 Requires-Dist: python-dateutil>=2.8.2
-Requires-Dist: prompt-toolkit<2.0.0,>=1.0.15; python_version == "2.7"
-Requires-Dist: prompt-toolkit>=2.0.1; python_version >= "3.5"
+Requires-Dist: prompt-toolkit>=1.0.15; python_version == "2.7"
+Requires-Dist: prompt-toolkit>=2.0.1; python_version == "3.5"
+Requires-Dist: prompt-toolkit>=3.0.13; python_version >= "3.6"
 Requires-Dist: PyYAML>=5.3.1; python_version <= "3.5"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: jsonschema>=3.0.1
 Requires-Dist: yamlloader>=0.5.5
 Requires-Dist: urllib3>=1.26.9; python_version == "3.5"
 Requires-Dist: urllib3>=1.26.18; python_version >= "3.6"
```

### Comparing `zhmccli-1.9.2/zhmccli.egg-info/SOURCES.txt` & `zhmccli-1.9.3/zhmccli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhmccli-1.9.2/zhmccli.egg-info/requires.txt` & `zhmccli-1.9.3/zhmccli.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,28 @@
 PyYAML>=5.3.1
 
 [:python_version <= "3.9"]
 six>=1.14.0
 tabulate>=0.8.2
 
 [:python_version == "2.7"]
-prompt-toolkit<2.0.0,>=1.0.15
+prompt-toolkit>=1.0.15
 
 [:python_version == "3.5"]
+prompt-toolkit>=2.0.1
 urllib3>=1.26.9
 
 [:python_version >= "3.10"]
 six>=1.16.0
 tabulate>=0.8.8
 
 [:python_version >= "3.12"]
 PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1
 
-[:python_version >= "3.5"]
-prompt-toolkit>=2.0.1
-
 [:python_version >= "3.6"]
 click>=8.0.2
 click-repl>=0.2
+prompt-toolkit>=3.0.13
 urllib3>=1.26.18
 
 [:python_version >= "3.6" and python_version <= "3.11"]
 PyYAML!=5.4.0,!=5.4.1,>=5.3.1
```

