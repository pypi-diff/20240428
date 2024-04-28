# Comparing `tmp/tokenterminal-1.0.1.tar.gz` & `tmp/tokenterminal-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenterminal-1.0.1.tar", last modified: Wed Jun  2 08:22:31 2021, max compression
+gzip compressed data, was "tokenterminal-2.0.0.tar", last modified: Sun Apr 28 15:06:27 2024, max compression
```

## Comparing `tokenterminal-1.0.1.tar` & `tokenterminal-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 08:22:31.653849 tokenterminal-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2021-06-02 08:22:31.653849 tokenterminal-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-02 08:22:31.653849 tokenterminal-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 08:22:31.653849 tokenterminal-1.0.1/tokenterminal/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/tokenterminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/tokenterminal/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2021-06-02 08:22:24.000000 tokenterminal-1.0.1/tokenterminal/tokenterminal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 08:22:31.653849 tokenterminal-1.0.1/tokenterminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2021-06-02 08:22:31.000000 tokenterminal-1.0.1/tokenterminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-06-02 08:22:31.000000 tokenterminal-1.0.1/tokenterminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-02 08:22:31.000000 tokenterminal-1.0.1/tokenterminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-06-02 08:22:31.000000 tokenterminal-1.0.1/tokenterminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-06-02 08:22:31.000000 tokenterminal-1.0.1/tokenterminal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/tests/test_tokenterminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/tokenterminal/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/tokenterminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/tokenterminal/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-04-28 15:06:19.000000 tokenterminal-2.0.0/tokenterminal/tokenterminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:06:27.242063 tokenterminal-2.0.0/tokenterminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-28 15:06:27.000000 tokenterminal-2.0.0/tokenterminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-28 15:06:27.000000 tokenterminal-2.0.0/tokenterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:06:27.000000 tokenterminal-2.0.0/tokenterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 15:06:27.000000 tokenterminal-2.0.0/tokenterminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 15:06:27.000000 tokenterminal-2.0.0/tokenterminal.egg-info/top_level.txt
```

### Comparing `tokenterminal-1.0.1/LICENSE` & `tokenterminal-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenterminal-1.0.1/PKG-INFO` & `tokenterminal-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,98 @@
 Metadata-Version: 2.1
 Name: tokenterminal
-Version: 1.0.1
+Version: 2.0.0
 Summary: Unofficial Token Terminal API client.
 Home-page: https://github.com/itzmestar/tokenterminal
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
-Description: # Token Terminal
-        
-        [![Python 3.5](https://img.shields.io/badge/python-3.5-blue.svg)](https://www.python.org/downloads/release/python-350/)
-        [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
-        [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-        [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
-        [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-        
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        [![Build](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml)
-        
-        -------
-        
-        ### Unofficial [Token Terminal API](https://www.tokenterminal.com/) client in python
-        
-        For more information, see [Token Terminal API Documentation](https://docs.tokenterminal.com/)
-        
-        ### Installation:
-        
-        use pip to install:
-        
-        ``` 
-        pip install tokenterminal
-        ```
-        
-        -----------
-        
-        ### Authentication:
-        
-        Pass API key in object initialization.
-        
-        -----------
-        
-        ### Example usage:
-        
-        ```
-        from tokenterminal import TokenTerminal
-        
-        # object initialization
-        token_terminal = TokenTerminal(key='xxxxx-xxxx-xxxx-xxxx-xxxxxxxx')
-        
-        # Fetch all data for projects' 
-        projects_data = token_terminal.get_all_projects()
-        
-        for project_info in projects_data:
-            print(project_info)
-        
-        # Fetch project's historical metrics
-        
-        project_metrics = token_terminal.get_historical_metrics('0x')
-        for metrics in project_metrics:
-            print(metrics)
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.18.4
+
+# Token Terminal
+
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+-------
+
+### Unofficial [Token Terminal API](https://www.tokenterminal.com/) client in python
+
+For more information, see [Token Terminal API Documentation](https://docs.tokenterminal.com/)
+
+### Installation:
+
+use pip to install:
+
+``` 
+pip install tokenterminal
+```
+
+-----------
+
+### Authentication:
+
+Pass API key in object initialization.
+
+-----------
+
+### Example usage:
+
+```
+from tokenterminal import TokenTerminal
+
+# object initialization
+token_terminal = TokenTerminal(key='xxxxx-xxxx-xxxx-xxxx-xxxxxxxx')
+
+# Fetch all data for projects' 
+projects_data = token_terminal.get_all_projects()
+
+for project_info in projects_data:
+    print(project_info)
+
+# Fetch project's historical metrics
+
+project_metrics = token_terminal.get_historical_metrics('0x')
+for metrics in project_metrics:
+    print(metrics)
+
+# To retrieve the metric availability for a project.
+reponse = token_terminal.get_metric_availability(project_id=project_id)
+
+# To retrieve metric aggregation data for one project.
+reponse = token_terminal.get_metric_aggregations(project_id=project_id)
+
+# Get financial statement for a project
+reponse = token_terminal.get_financial_statement(
+    project_id=project_id, 
+    timestamp_granularity='week',
+    interval='1m'
+    )
+
+# Get list of all available market sectors that are available
+reponse = token_terminal.get_market_sectors()
+
+# Get list of all metrics
+reponse = token_terminal.get_all_metrics()
+
+# To retrieve metric aggregations for multiple projects.
+project_ids = ['aave', 'uniswap']
+reponse = token_terminal.get_projects_metric_aggregations(project_ids=project_ids)
+```
+-------
+#### Donate & Help maintain the library
+
+[![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
+
+-------
```

### Comparing `tokenterminal-1.0.1/README.md` & `tokenterminal-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Token Terminal
 
-[![Python 3.5](https://img.shields.io/badge/python-3.5-blue.svg)](https://www.python.org/downloads/release/python-350/)
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-[![Build](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml)
-
 -------
 
 ### Unofficial [Token Terminal API](https://www.tokenterminal.com/) client in python
 
 For more information, see [Token Terminal API Documentation](https://docs.tokenterminal.com/)
 
 ### Installation:
@@ -47,8 +43,37 @@
     print(project_info)
 
 # Fetch project's historical metrics
 
 project_metrics = token_terminal.get_historical_metrics('0x')
 for metrics in project_metrics:
     print(metrics)
-```
+
+# To retrieve the metric availability for a project.
+reponse = token_terminal.get_metric_availability(project_id=project_id)
+
+# To retrieve metric aggregation data for one project.
+reponse = token_terminal.get_metric_aggregations(project_id=project_id)
+
+# Get financial statement for a project
+reponse = token_terminal.get_financial_statement(
+    project_id=project_id, 
+    timestamp_granularity='week',
+    interval='1m'
+    )
+
+# Get list of all available market sectors that are available
+reponse = token_terminal.get_market_sectors()
+
+# Get list of all metrics
+reponse = token_terminal.get_all_metrics()
+
+# To retrieve metric aggregations for multiple projects.
+project_ids = ['aave', 'uniswap']
+reponse = token_terminal.get_projects_metric_aggregations(project_ids=project_ids)
+```
+-------
+#### Donate & Help maintain the library
+
+[![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
+
+-------
```

### Comparing `tokenterminal-1.0.1/setup.py` & `tokenterminal-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tokenterminal-1.0.1/tokenterminal.egg-info/PKG-INFO` & `tokenterminal-2.0.0/tokenterminal.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,98 @@
 Metadata-Version: 2.1
 Name: tokenterminal
-Version: 1.0.1
+Version: 2.0.0
 Summary: Unofficial Token Terminal API client.
 Home-page: https://github.com/itzmestar/tokenterminal
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
-Description: # Token Terminal
-        
-        [![Python 3.5](https://img.shields.io/badge/python-3.5-blue.svg)](https://www.python.org/downloads/release/python-350/)
-        [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
-        [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-        [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
-        [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-        
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        [![Build](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/itzmestar/tokenterminal/actions/workflows/python-package.yml)
-        
-        -------
-        
-        ### Unofficial [Token Terminal API](https://www.tokenterminal.com/) client in python
-        
-        For more information, see [Token Terminal API Documentation](https://docs.tokenterminal.com/)
-        
-        ### Installation:
-        
-        use pip to install:
-        
-        ``` 
-        pip install tokenterminal
-        ```
-        
-        -----------
-        
-        ### Authentication:
-        
-        Pass API key in object initialization.
-        
-        -----------
-        
-        ### Example usage:
-        
-        ```
-        from tokenterminal import TokenTerminal
-        
-        # object initialization
-        token_terminal = TokenTerminal(key='xxxxx-xxxx-xxxx-xxxx-xxxxxxxx')
-        
-        # Fetch all data for projects' 
-        projects_data = token_terminal.get_all_projects()
-        
-        for project_info in projects_data:
-            print(project_info)
-        
-        # Fetch project's historical metrics
-        
-        project_metrics = token_terminal.get_historical_metrics('0x')
-        for metrics in project_metrics:
-            print(metrics)
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.18.4
+
+# Token Terminal
+
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+-------
+
+### Unofficial [Token Terminal API](https://www.tokenterminal.com/) client in python
+
+For more information, see [Token Terminal API Documentation](https://docs.tokenterminal.com/)
+
+### Installation:
+
+use pip to install:
+
+``` 
+pip install tokenterminal
+```
+
+-----------
+
+### Authentication:
+
+Pass API key in object initialization.
+
+-----------
+
+### Example usage:
+
+```
+from tokenterminal import TokenTerminal
+
+# object initialization
+token_terminal = TokenTerminal(key='xxxxx-xxxx-xxxx-xxxx-xxxxxxxx')
+
+# Fetch all data for projects' 
+projects_data = token_terminal.get_all_projects()
+
+for project_info in projects_data:
+    print(project_info)
+
+# Fetch project's historical metrics
+
+project_metrics = token_terminal.get_historical_metrics('0x')
+for metrics in project_metrics:
+    print(metrics)
+
+# To retrieve the metric availability for a project.
+reponse = token_terminal.get_metric_availability(project_id=project_id)
+
+# To retrieve metric aggregation data for one project.
+reponse = token_terminal.get_metric_aggregations(project_id=project_id)
+
+# Get financial statement for a project
+reponse = token_terminal.get_financial_statement(
+    project_id=project_id, 
+    timestamp_granularity='week',
+    interval='1m'
+    )
+
+# Get list of all available market sectors that are available
+reponse = token_terminal.get_market_sectors()
+
+# Get list of all metrics
+reponse = token_terminal.get_all_metrics()
+
+# To retrieve metric aggregations for multiple projects.
+project_ids = ['aave', 'uniswap']
+reponse = token_terminal.get_projects_metric_aggregations(project_ids=project_ids)
+```
+-------
+#### Donate & Help maintain the library
+
+[![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
+
+-------
```

