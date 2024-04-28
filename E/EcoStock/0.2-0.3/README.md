# Comparing `tmp/EcoStock-0.2.tar.gz` & `tmp/EcoStock-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.2.tar", last modified: Sat Apr 27 17:33:54 2024, max compression
+gzip compressed data, was "EcoStock-0.3.tar", last modified: Sun Apr 28 10:32:28 2024, max compression
```

## Comparing `EcoStock-0.2.tar` & `EcoStock-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.925283 EcoStock-0.2/
-drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.920299 EcoStock-0.2/EcoStock/
--rw-rw-rw-   0        0        0      869 2024-04-27 17:05:18.000000 EcoStock-0.2/EcoStock/__init__.py
--rw-rw-rw-   0        0        0     8646 2024-04-27 16:48:18.000000 EcoStock-0.2/EcoStock/api.py
--rw-rw-rw-   0        0        0    13738 2024-04-27 16:45:22.000000 EcoStock-0.2/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.924318 EcoStock-0.2/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-20 17:30:30.000000 EcoStock-0.2/LICENSE.md
--rw-rw-rw-   0        0        0     1737 2024-04-27 17:33:54.925283 EcoStock-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-23 14:39:00.000000 EcoStock-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 17:33:54.925283 EcoStock-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-04-27 17:04:08.000000 EcoStock-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.381217 EcoStock-0.3/
+drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.365621 EcoStock-0.3/EcoStock/
+-rw-rw-rw-   0        0        0      854 2024-04-28 10:30:11.000000 EcoStock-0.3/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0     8646 2024-04-27 16:48:18.000000 EcoStock-0.3/EcoStock/api.py
+-rw-rw-rw-   0        0        0    12900 2024-04-28 10:29:49.000000 EcoStock-0.3/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.381217 EcoStock-0.3/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1737 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-20 17:30:30.000000 EcoStock-0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1737 2024-04-28 10:32:28.381217 EcoStock-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2024-04-23 14:39:00.000000 EcoStock-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 10:32:28.381217 EcoStock-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2024-04-28 10:27:54.000000 EcoStock-0.3/setup.py
```

### Comparing `EcoStock-0.2/EcoStock/__init__.py` & `EcoStock-0.3/EcoStock/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 """
 Economic-Finance Correlation Package
 
 A Python package for investigating the correlation between economic and financial data.
 """
 
-__version__ = "0.2"
+__version__ = "0.3"
 
 from .api import app
 from .functions import (
     get_stock_data,
     plot_candlestick,
     moving_avg_stock_data,
     get_world_bank_data,
     plot_correlation,
     plot_bollinger_bands,
-    get_news,
     plot_indicator_for_countries,
     compare_indicators_countries
 )
 
 
 # Questo file fornisce una breve descrizione del pacchetto e definisce la versione. 
 # Infine, importa tutte le funzioni dal modulo functions.py in modo che siano disponibili quando importi il tuo pacchetto.
```

### Comparing `EcoStock-0.2/EcoStock/api.py` & `EcoStock-0.3/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `EcoStock-0.2/EcoStock/functions.py` & `EcoStock-0.3/EcoStock/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -260,44 +260,14 @@
 
     # Set the title of the chart to 'Bollinger Bands for {ticker}'
     fig.update_layout(title='Bollinger Bands for {}'.format(ticker))
 
     # Display the chart
     fig.show()
 
-# Get news data from GNews API
-def get_news(symbol):
-    # GNews API
-    api_key = '3dcc9727bfb88289097e7dee864baae4'
-
-    # URL of GNews's search function
-    url = f'https://gnews.io/api/v4/search?q={symbol}&token={api_key}'
-
-    try:
-        # Send a GET request to the API
-        response = requests.get(url)
-
-        # Raise an exception if the request was unsuccessful
-        response.raise_for_status()
-    except requests.exceptions.HTTPError as http_err:
-        print(f'HTTP error occurred: {http_err}')
-        return None
-    except Exception as err:
-        print(f'Other error occurred: {err}')
-        return None
-
-    # Parse the JSON response
-    try:
-        data = response.json()
-    except ValueError:
-        print('Error parsing JSON response')
-        return None
-
-    return data
-
 # Plotting indicator data for multiple countries
 def plot_indicator_for_countries(indicator, countries, start_date, end_date):
     """
     Plot an economic indicator for several countries.
 
     Parameters:
     indicator (str): The indicator of interest.
```

### Comparing `EcoStock-0.2/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.3/EcoStock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.2
+Version: 0.3
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.2/LICENSE.md` & `EcoStock-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.2/PKG-INFO` & `EcoStock-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.2
+Version: 0.3
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.2/README.md` & `EcoStock-0.3/README.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.2/setup.py` & `EcoStock-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.2',
+    version='0.3',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
```

