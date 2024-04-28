# Comparing `tmp/pydolarvenezuela-1.5.0.tar.gz` & `tmp/pydolarvenezuela-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.0.tar", last modified: Sat Apr 27 00:35:27 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.1.tar", last modified: Sun Apr 28 16:04:46 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.0.tar` & `pydolarvenezuela-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:27.096863 pydolarvenezuela-1.5.0/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     7269 2024-04-27 00:35:27.036554 pydolarvenezuela-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4878 2024-04-26 19:43:36.000000 pydolarvenezuela-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.686303 pydolarvenezuela-1.5.0/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2723 2024-04-27 00:34:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.729503 pydolarvenezuela-1.5.0/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.733494 pydolarvenezuela-1.5.0/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.748395 pydolarvenezuela-1.5.0/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.798509 pydolarvenezuela-1.5.0/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      318 2024-04-26 04:57:25.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      716 2024-04-25 23:43:03.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.935924 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     4914 2024-04-27 00:30:35.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:26.950354 pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:35:27.024552 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7269 2024-04-27 00:35:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2024-04-27 00:35:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 00:35:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-27 00:35:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 00:35:26.000000 pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-27 00:34:12.000000 pydolarvenezuela-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 00:35:27.097863 pydolarvenezuela-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-27 00:34:18.000000 pydolarvenezuela-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.640573 pydolarvenezuela-1.5.1/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     7209 2024-04-28 16:04:46.635504 pydolarvenezuela-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4818 2024-04-28 12:19:05.000000 pydolarvenezuela-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.513172 pydolarvenezuela-1.5.1/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2712 2024-04-28 16:02:13.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.546367 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.546367 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.563226 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.581247 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 11:38:43.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.611897 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5149 2024-04-28 15:09:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     1846 2024-04-28 12:10:50.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2315 2024-04-28 12:10:54.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1037 2024-04-28 12:10:58.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.618121 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.632505 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7209 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-28 16:02:26.000000 pydolarvenezuela-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 16:04:46.640573 pydolarvenezuela-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-28 16:02:19.000000 pydolarvenezuela-1.5.1/setup.py
```

### Comparing `pydolarvenezuela-1.5.0/LICENSE` & `pydolarvenezuela-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.0/PKG-INFO` & `pydolarvenezuela-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.0
+Version: 1.5.1
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -49,40 +49,38 @@
 pyDolarVenezuela es una librería de Python que te brinda la posibilidad de obtener los valores del dólar en distintos monitores en Venezuela, así como las tasas de cambio proporcionadas por el Banco Central de Venezuela. Esta librería consulta diversas páginas web que ofrecen información actualizada sobre el valor del dólar:
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| iVenezuela | https://www.ivenezuela.travel/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-| Dpedidos | https://dpedidos.com/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-
+| Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
 
 ## Uso
 Debes importar el módulo `pages`, donde encontrarás una variedad de atributos que contienen información sobre una página específica de la que deseas obtener los datos. Adicionalmente deberás importar la clase `Monitor`, cuyos parámetros será la página que deseas utilizar y la moneda en la que se expresarán los precios (`USD`, `EUR`).
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
 pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
 
 ```python
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor, Redis
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 
 # Defecto
 db = Redis(
     host='localhost',
     port=6379
 )
 
@@ -115,15 +113,15 @@
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 # Obtener los valores de todos los monitores
 valores_dolar = monitor.get_value_monitors()
```

### Comparing `pydolarvenezuela-1.5.0/README.md` & `pydolarvenezuela-1.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,38 @@
 pyDolarVenezuela es una librería de Python que te brinda la posibilidad de obtener los valores del dólar en distintos monitores en Venezuela, así como las tasas de cambio proporcionadas por el Banco Central de Venezuela. Esta librería consulta diversas páginas web que ofrecen información actualizada sobre el valor del dólar:
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| iVenezuela | https://www.ivenezuela.travel/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-| Dpedidos | https://dpedidos.com/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-
+| Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
 
 ## Uso
 Debes importar el módulo `pages`, donde encontrarás una variedad de atributos que contienen información sobre una página específica de la que deseas obtener los datos. Adicionalmente deberás importar la clase `Monitor`, cuyos parámetros será la página que deseas utilizar y la moneda en la que se expresarán los precios (`USD`, `EUR`).
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
 pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
 
 ```python
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor, Redis
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 
 # Defecto
 db = Redis(
     host='localhost',
     port=6379
 )
 
@@ -69,15 +67,15 @@
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 # Obtener los valores de todos los monitores
 valores_dolar = monitor.get_value_monitors()
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from typing import Literal
 from colorama import Fore
 
 from . import network
-from .models.pages import Monitor as Page
+from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.0'
+version = '1.5.1'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,136 @@
 import json
+from typing import Any
 from .bcv import BCV
 from .criptodolar import CriptoDolar
 from .exchangemonitor import ExchangeMonitor
-from .ivenezuela import iVenezuela
-from .dpedidos import Dpedidos
+from .italcambio import Italcambio
 
 from ..data.redis import Cache
 from ..models.database import Redis
-from ..models.pages import Monitor
-from ..pages import BCV as B, CriptoDolar as C, Dpedidos as D, ExchangeMonitor as E, iVenezuela as I 
-
-monitor_classes = {
-    'usd': {
-        B.name: BCV,
-        C.name: CriptoDolar,
-        E.name: ExchangeMonitor,
-        D.name: Dpedidos,
-        I.name: iVenezuela
+from ..models.pages import Page
+from ..pages import BCV as B, CriptoDolar as C, ExchangeMonitor as E, Italcambio as I
+from ..utils import currencies_list
+
+monitor_classes = [
+    {
+        B.name: {
+            'currency': B.currencies,
+            'provider': BCV
+        }
+    },
+    {
+        C.name: {
+            'currency': C.currencies,
+            'provider': CriptoDolar
+        }
     },
-    'eur': {
-        B.name: BCV,
-        C.name: CriptoDolar,
-        E.name: ExchangeMonitor
+    {
+        E.name: {
+            'currency': E.currencies,
+            'provider': ExchangeMonitor
+        }
+    },
+    {
+        I.name: {
+            'currency': I.currencies,
+            'provider': Italcambio
+        }
     }
-}
+]
 
-def select_monitor(provider: Monitor, db: Redis, **kwargs):
+def select_monitor(provider: Page, db: Redis, **kwargs):
+    global data
+        
     currency = kwargs.get('currency')
     monitor_code = kwargs.get('monitor_code')
     name_property = kwargs.get('name_property')
     prettify = kwargs.get('prettify', False)
 
-    if currency not in ['usd', 'eur']:
-        raise ValueError(f"The currency type must be 'usd' or 'eur', not {currency}")
+    if currency not in currencies_list:
+        raise ValueError(f"The currency type must be 'usd', 'eur'..., not {currency}")
+
+    def _get_values_specifics():
+        if not monitor_code:
+            return data
+        
+        try:
+            monitor_data = data[monitor_code.lower()]
+            if name_property:
+                if name_property == 'last_update' and provider.name == B.name:
+                    return data[name_property]
+                value = monitor_data[name_property]
+                return f'Bs. {value}' if prettify and name_property == 'price' else value
+            return monitor_data
+        except KeyError:
+            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
+
+    def _update_item(existing_data_dict: dict, i: Any, last_data: dict):
+        if existing_data_dict[i]['price'] != last_data[i]['price']:
+            price = existing_data_dict[i]['price']
+            new_price = last_data[i]['price']
+            change  = round(float(new_price - price), 2)
+            percent = float(f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}'.replace('-', ' '))
+            symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
+            color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
+            last_update = last_data[i].get('last_update', None)
+            change = float(str(change).replace('-', ' '))
+
+            if not last_update:
+                existing_data_dict[i].update({
+                    'price': new_price,
+                    'change': change,
+                    'percent': percent,
+                    'color': color,
+                    'symbol': symbol,
+                    'last_update': last_update
+                })
+            else:
+                existing_data_dict[i].update({
+                    'price': new_price,
+                    'change': change,
+                    'percent': percent,
+                    'color': color,
+                    'symbol': symbol,
+                })
 
     try:
-        monitor_class = monitor_classes.get(currency).get(provider.name)
+        monitor_class = None
+
+        for monitor in monitor_classes:
+            if monitor.get(provider.name) and currency in monitor.get(provider.name)['currency']:
+                monitor_class = monitor[provider.name]['provider']
+
         if monitor_class is not None:
+            data = monitor_class(url=provider.provider, currency=currency).get_values()
             if db is not None:
-                response = monitor_class(provider.provider, currency).get_values()
-
                 key = f'{currency}:{provider.name}'
                 cache = Cache(db)
 
                 existing_data = cache.get_data(key)
 
                 if not existing_data:
-                    cache.set_data(key, json.dumps(response), db.ttl)
-                else:
-                    existing_data_dict: dict[str, dict] = json.loads(existing_data)
-                    for name in existing_data_dict:
-                        if not name == 'last_update':
-                            if name in existing_data_dict and name in response:
-                                if existing_data_dict[name]['price'] != response[name]['price']:
-                                    price = existing_data_dict[name]['price']
-                                    new_price = response[name]['price']
-                                    change  = round(float(new_price - price), 2)
-                                    percent = f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}%'
-                                    symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
-                                    color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
-                                    last_update = None if provider.name == B.name else response[name]['last_update']
-
-                                    if not provider.name == B.name:
-                                        existing_data_dict[name].update({
-                                            'price': new_price,
-                                            'change': change,
-                                            'percent': percent,
-                                            'color': color,
-                                            'symbol': symbol,
-                                            'last_update': last_update
-                                        })
-                                    else:
-                                        existing_data_dict[name].update({
-                                            'price': new_price,
-                                            'change': change,
-                                            'percent': percent,
-                                            'color': color,
-                                            'symbol': symbol,
-                                        })
-                
+                    cache.set_data(key, json.dumps(data), db.ttl)
+
+                existing_data_dict = json.loads(cache.get_data(key))
+                for name in existing_data_dict:
+                    if not name == 'last_update' and not name == 'banks':
+                        if name in existing_data_dict and name in data:
+                            _update_item(existing_data_dict, name, data)
+                    else:
+                        if name == 'banks' and name in data:
+                            for i in range(len(existing_data_dict[name])):
+                                _update_item(existing_data_dict[name], i, data[name])
+                        elif name == 'last_update':
+                            existing_data_dict[name] = data[name]
+                            
                 cache.set_data(key, json.dumps(existing_data_dict), db.ttl)
-                existing_data_dict: dict[str, dict] = json.loads(
+                data = json.loads(
                     cache.get_data(key)
                 )
 
-                if not monitor_code:
-                    return existing_data_dict
-                
-                try:
-                    monitor_data = existing_data_dict[monitor_code.lower()]
-                    if name_property:
-                        value = monitor_data[name_property]
-                        return f'Bs. {value}' if prettify and name_property == 'price' else value
-                    return monitor_data
-                except KeyError:
-                    raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
-
-            return monitor_class(provider.provider, currency).get_values(
-                monitor_code=monitor_code,
-                name_property=name_property, 
-                prettify=prettify
-            )
+                return _get_values_specifics()
+            return _get_values_specifics()
         else:
             raise ValueError("Provider not supported")
     except Exception as e:
         raise e
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/bcv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-import requests
 from bs4 import BeautifulSoup
 
+from ..network import requests, get
 from ..utils import currencies
 
 requests.packages.urllib3.disable_warnings()
 
 def _get_rate_by_id(tag_id: str, soup: BeautifulSoup):
     return float(soup.find(id=tag_id).find("strong").text.strip().replace(',', '.'))
 
 def _get_time(soup: BeautifulSoup):
     date = soup.find("span", "date-display-single").get('content')
     return date.split('T')[0].replace('-', '/')
 
 class BCV:
-    def __init__(self, url: str, currency: str) -> None:
-        response      = requests.get(url, verify=False)
-        response.raise_for_status()
-
-        self.soup     = BeautifulSoup(response.content, 'html.parser')
-        self.currency = currency
+    def __init__(self, url: str, **kwargs) -> None:
+        response = get(f'{url}tasas-informativas-sistema-bancario', verify=False)
+        self.soup = BeautifulSoup(response, 'html.parser')
 
     def _load(self) -> None:
+        self.rates = {}
         section_tipo_de_cambio_oficial = self.soup.find("div", "view-tipo-de-cambio-oficial-del-bcv")
+        section_sistema_bancario = self.soup.find("div", "table-responsive")
 
-        self.rates = {}
+        banks = []
+        for bank in section_sistema_bancario.find('tbody').find_all('tr'):
+            title = str(bank.find('td', 'views-field views-field-views-conditional').text).strip()
+
+            if title not in [bank['title'] for bank in banks]:
+                price = float(str(bank.find('td', 'views-field views-field-field-tasa-venta').text).replace(',', '.'))
+
+                banks.append({
+                    'title': title,
+                    'price_old': price,
+                    'price': round(price, 2),
+                    'last_update': str(bank.find('td', 'views-field views-field-field-fecha-del-indicador').text).strip().replace('-', '/')
+                })
+            self.rates['banks'] = banks
+        
         self.rates['last_update'] = _get_time(section_tipo_de_cambio_oficial)
 
         for code, values in currencies.items():
             self.rates[code] = {
                 "title": values['name'],
                 "price": round(_get_rate_by_id(values['id'], section_tipo_de_cambio_oficial), 2),
                 "price_old": _get_rate_by_id(values['id'], section_tipo_de_cambio_oficial)
             }
 
-    def get_values(self, **kwargs):
-        currency_code = kwargs.get('monitor_code')
-        name_property = kwargs.get('name_property')
-        prettify = kwargs.get('prettify', False)
-        
+    def get_values(self):
         self._load()
-
-        if not currency_code:
-            return self.rates
-        
-        try:
-            monitor_data = self.rates[currency_code.lower()]
-            if name_property:
-                if name_property == 'last_update':
-                    return self.rates['last_update']
-                value = monitor_data[name_property]
-                return f'Bs. {value}' if prettify and name_property == 'price' else value
-            return monitor_data
-        except KeyError:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
+        return self.rates
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/criptodolar.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         if monitor_name in ['Dólar Monitor', 'Euro Monitor']:
             return 'EnParaleloVzla'
         else:
             return monitor_name.split(' ')[1]
     return monitor_name
 
 class CriptoDolar:
-    def __init__(self, url: str, currency: str) -> None:
+    def __init__(self, url: str, currency: str, **kwargs) -> None:
         response           = (network.get(url + "coins/latest", {'type': 'bolivar', 'base': 'usd'}) if currency == 'usd'
                               else network.get(url + "coins/latest", {'type': 'bolivar', 'base': 'eur'}))
         self.json_response = json.loads(response)
         self.currency = currency
     
     def _load(self):
         self.data = {}
@@ -34,25 +34,10 @@
                     'price_old': monitor['priceOld'],
                     'type': 'bank' if monitor['type'] == 'bancove' else 'monitor',
                     'last_update': time.get_time_standard(monitor['updatedAt']),
                 }
 
                 self.data[_convert_specific_format(data['title'])] = data
     
-    def get_values(self, **kwargs):
-        monitor_code = kwargs.get('monitor_code')
-        name_property = kwargs.get('name_property')
-        prettify = kwargs.get('prettify', False)
-        
+    def get_values(self):
         self._load()
-
-        if not monitor_code:
-            return self.data
-        
-        try:
-            monitor_data = self.data[monitor_code.lower()]
-            if name_property:
-                value = monitor_data[name_property]
-                return f'Bs. {value}' if prettify and name_property == 'price' else value
-            return monitor_data
-        except KeyError:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
+        return self.data
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from bs4 import BeautifulSoup
-
 from .. import network
 from ..tools import time
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
 def _get_values_monitors(soup: BeautifulSoup):
     return [value for value in soup]
 
 class ExchangeMonitor:
-    def __init__(self, url: str, currency: str) -> None:
+    def __init__(self, url: str, currency: str, **kwargs) -> None:
         response = (network.curl(url + "dolar-venezuela") if currency == 'usd'
                     else network.curl(url + "dolar-venezuela/EUR"))
         self.soup = BeautifulSoup(response, "html.parser")
     
     def _load(self):
         section_dolar_venezuela = self.soup.find_all("div", "col-xs-12 col-sm-6 col-md-4 col-tabla")
         _scraping_monitors = _get_values_monitors(section_dolar_venezuela)
@@ -47,25 +46,10 @@
                 'change': change,
                 'color': color,
                 'symbol': symbol
             }
 
             self.data[_convert_specific_format(name)] = data
     
-    def get_values(self, **kwargs):
-        monitor_code = kwargs.get('monitor_code')
-        name_property = kwargs.get('name_property')
-        prettify = kwargs.get('prettify', False)
-        
+    def get_values(self):
         self._load()
-
-        if not monitor_code:
-            return self.data
-        
-        try:
-            monitor_data = self.data[monitor_code.lower()]
-            if name_property:
-                value = monitor_data[name_property]
-                return f'Bs. {value}' if prettify and name_property == 'price' else value
-            return monitor_data
-        except KeyError:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
+        return self.data
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.0
+Version: 1.5.1
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -49,40 +49,38 @@
 pyDolarVenezuela es una librería de Python que te brinda la posibilidad de obtener los valores del dólar en distintos monitores en Venezuela, así como las tasas de cambio proporcionadas por el Banco Central de Venezuela. Esta librería consulta diversas páginas web que ofrecen información actualizada sobre el valor del dólar:
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| iVenezuela | https://www.ivenezuela.travel/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-| Dpedidos | https://dpedidos.com/ | ![Inactive](https://img.shields.io/badge/Inactivo-red) |
-
+| Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
 
 ## Uso
 Debes importar el módulo `pages`, donde encontrarás una variedad de atributos que contienen información sobre una página específica de la que deseas obtener los datos. Adicionalmente deberás importar la clase `Monitor`, cuyos parámetros será la página que deseas utilizar y la moneda en la que se expresarán los precios (`USD`, `EUR`).
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
 pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
 
 ```python
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor, Redis
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 
 # Defecto
 db = Redis(
     host='localhost',
     port=6379
 )
 
@@ -115,15 +113,15 @@
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 # Obtener los valores de todos los monitores
 valores_dolar = monitor.get_value_monitors()
```

### Comparing `pydolarvenezuela-1.5.0/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,13 +17,12 @@
 pyDolarVenezuela/data/redis.py
 pyDolarVenezuela/models/__init__.py
 pyDolarVenezuela/models/database.py
 pyDolarVenezuela/models/pages.py
 pyDolarVenezuela/provider/__init__.py
 pyDolarVenezuela/provider/bcv.py
 pyDolarVenezuela/provider/criptodolar.py
-pyDolarVenezuela/provider/dpedidos.py
 pyDolarVenezuela/provider/exchangemonitor.py
-pyDolarVenezuela/provider/ivenezuela.py
+pyDolarVenezuela/provider/italcambio.py
 pyDolarVenezuela/tools/__init__.py
 pyDolarVenezuela/tools/calculator.py
 pyDolarVenezuela/tools/time.py
```

### Comparing `pydolarvenezuela-1.5.0/pyproject.toml` & `pydolarvenezuela-1.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.0"
+version = "1.5.1"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.0/setup.py` & `pydolarvenezuela-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.0'
+VERSION = '1.5.1'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

