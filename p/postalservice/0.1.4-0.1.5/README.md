# Comparing `tmp/postalservice-0.1.4.tar.gz` & `tmp/postalservice-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postalservice-0.1.4.tar", last modified: Fri Mar 29 14:01:36 2024, max compression
+gzip compressed data, was "postalservice-0.1.5.tar", last modified: Sun Apr 28 10:17:06 2024, max compression
```

## Comparing `postalservice-0.1.4.tar` & `postalservice-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:01:36.309145 postalservice-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-29 14:01:32.000000 postalservice-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-29 14:01:36.309145 postalservice-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-29 14:01:32.000000 postalservice-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:01:36.309145 postalservice-0.1.4/postalservice/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/baseservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/frilservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/mercariservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:01:36.309145 postalservice-0.1.4/postalservice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/utils/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-29 14:01:32.000000 postalservice-0.1.4/postalservice/utils/search_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:01:36.309145 postalservice-0.1.4/postalservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-29 14:01:36.000000 postalservice-0.1.4/postalservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 14:01:36.000000 postalservice-0.1.4/postalservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 14:01:36.000000 postalservice-0.1.4/postalservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 14:01:36.000000 postalservice-0.1.4/postalservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 14:01:36.309145 postalservice-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-29 14:01:32.000000 postalservice-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:01:36.309145 postalservice-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 14:01:32.000000 postalservice-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-03-29 14:01:32.000000 postalservice-0.1.4/tests/baseservicetestclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-29 14:01:32.000000 postalservice-0.1.4/tests/test_fril.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-29 14:01:32.000000 postalservice-0.1.4/tests/test_mercari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:17:06.992088 postalservice-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-28 10:17:03.000000 postalservice-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-28 10:17:06.992088 postalservice-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-28 10:17:03.000000 postalservice-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:17:06.992088 postalservice-0.1.5/postalservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/baseservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/frilservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/mercariservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:17:06.992088 postalservice-0.1.5/postalservice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/utils/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-28 10:17:03.000000 postalservice-0.1.5/postalservice/yjpservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:17:06.992088 postalservice-0.1.5/postalservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-28 10:17:06.000000 postalservice-0.1.5/postalservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-28 10:17:06.000000 postalservice-0.1.5/postalservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:17:06.000000 postalservice-0.1.5/postalservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 10:17:06.000000 postalservice-0.1.5/postalservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:17:06.992088 postalservice-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-28 10:17:03.000000 postalservice-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:17:06.992088 postalservice-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-28 10:17:03.000000 postalservice-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-28 10:17:03.000000 postalservice-0.1.5/tests/baseservicetestclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-28 10:17:03.000000 postalservice-0.1.5/tests/test_fril.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-28 10:17:03.000000 postalservice-0.1.5/tests/test_mercari.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 10:17:03.000000 postalservice-0.1.5/tests/test_yjp.py
```

### Comparing `postalservice-0.1.4/LICENSE` & `postalservice-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `postalservice-0.1.4/PKG-INFO` & `postalservice-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: postalservice
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for second hand shopping
 Author: Aapo Montin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postal Service Python Library
 [![Mercari](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml)
 [![Fril](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml)
+[![YJP](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml)
 [![PyPI version](https://badge.fury.io/py/postalservice.svg)](https://badge.fury.io/py/postalservice)
 
 Python library for scraping second hand Japanese websites for easier access to the search results. Useful for creating datasets, notification systems, or web APIs. Targets the website API if available, or parses the HTML response.
 
 ## Features
 
 - Mercari, Fril scraping
@@ -61,11 +62,10 @@
 `BaseService` is an abstract base class that defines the interface for a service. All services implement this and therefore have all these class methods:
 
 - `get_search_results(params: dict) -> SearchResults`: Fetches data synchronously using the provided parameters, parses the response, and returns the results as SearchResults object.
 
 - `get_search_results_async(params: dict) -> SearchResults`: Fetches data asynchronously using the provided parameters, parses the response (asynchronously, if needed), and returns the results as SearchResults object. 
 
 ## todo
-- YJP support
-- Filter by brand
+- Rakuten support
 - General improvements to structure of the library
-- Support for getting intermediate/temporary results for slow sites like Fril
+- Support for multiple sizes for sites where only one size is possible to select at a time
```

### Comparing `postalservice-0.1.4/README.md` & `postalservice-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Postal Service Python Library
 [![Mercari](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml)
 [![Fril](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml)
+[![YJP](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml)
 [![PyPI version](https://badge.fury.io/py/postalservice.svg)](https://badge.fury.io/py/postalservice)
 
 Python library for scraping second hand Japanese websites for easier access to the search results. Useful for creating datasets, notification systems, or web APIs. Targets the website API if available, or parses the HTML response.
 
 ## Features
 
 - Mercari, Fril scraping
@@ -53,11 +54,10 @@
 `BaseService` is an abstract base class that defines the interface for a service. All services implement this and therefore have all these class methods:
 
 - `get_search_results(params: dict) -> SearchResults`: Fetches data synchronously using the provided parameters, parses the response, and returns the results as SearchResults object.
 
 - `get_search_results_async(params: dict) -> SearchResults`: Fetches data asynchronously using the provided parameters, parses the response (asynchronously, if needed), and returns the results as SearchResults object. 
 
 ## todo
-- YJP support
-- Filter by brand
+- Rakuten support
 - General improvements to structure of the library
-- Support for getting intermediate/temporary results for slow sites like Fril
+- Support for multiple sizes for sites where only one size is possible to select at a time
```

### Comparing `postalservice-0.1.4/postalservice/baseservice.py` & `postalservice-0.1.5/postalservice/baseservice.py`

 * *Files identical despite different names*

### Comparing `postalservice-0.1.4/postalservice/frilservice.py` & `postalservice-0.1.5/postalservice/frilservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,14 @@
     "goa": "321",
     "FULLCOUNT": "2651",
     "WHITESVILLE": "9493",
     "WAREHOUSE": "4290",
     "takahiro miyashita the soloist": "8964",
 }
 
-CATEGORIES_MAP = {
-    "tops": 526,
-    "outerwear": 539,
-    "pants": 562,
-    "shoes": 572,
-    "bags": 580,
-    "hats": 598,
-    "accessories": 614,
-    "jewelry": 606,
-}
-
 
 class FrilService(BaseService):
 
     async def fetch_data_async(self, params: dict) -> httpx.Response:
         self.item_count = params.get("item_count", 36)
         url = self.get_search_params(params)
         res = await fetch_async(url)
@@ -166,15 +155,8 @@
         brands = params.get("brand")
         if "brand" in params and brands is not None and len(brands) > 0:
             if brands[0] not in BRANDS_MAP:
                 raise ValueError(f"Brand {brands[0]} is not supported")
             brand_id = BRANDS_MAP[brands[0]]
             url += f"&brand_id={brand_id}"
 
-        categories = params.get("category")
-        if "category" in params and categories is not None and len(categories) > 0:
-            if categories[0] not in CATEGORIES_MAP:
-                raise ValueError(f"Category {categories[0]} is not supported")
-            category_id = CATEGORIES_MAP[categories[0]]
-            url += f"&category_id={category_id}"
-
         return url
```

### Comparing `postalservice-0.1.4/postalservice/mercariservice.py` & `postalservice-0.1.5/postalservice/mercariservice.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     "XS": "154",
     "S": "2",
     "M": "3",
     "L": "4",
     "XL": "5",
     "XXL": "155",
 }
-
-BRANDS_MAP = {
+BREANS_MAP = {
     "JUNYA WATANABE": "1623",
     "JUNYA WATANABE MAN": "15429",
     "BLACK COMME des GARCONS": "1624",
     "COMME des GARCONS HOMME": "7319",
     "COMME des GARCONS HOMME DEUX": "7320",
     "COMME des GARCONS SHIRT": "7321",
     "JUNYA WATANABE COMME des GARCONS": "7389",
@@ -35,25 +34,14 @@
     "goa": "542",
     "FULLCOUNT": "5602",
     "WHITESVILLE": "8689",
     "WAREHOUSE": "281",
     "takahiro miyashita the soloist": "14631",
 }
 
-CATEGORIES_MAP = {
-    "tops": "30",
-    "outerwear": "31",
-    "pants": "32",
-    "shoes": "33",
-    "bags": "34",
-    "hats": "36",
-    "accessories": "38",
-    "jewelry": "37",
-}
-
 
 class MercariService(BaseService):
 
     def generate_payload_and_headers(self, params: dict):
         if not isinstance(params, dict):
             raise TypeError("params must be a dict")
 
@@ -68,26 +56,20 @@
 
         if size is not None:
             mapped_size = SIZE_MAP.get(size)
         else:
             mapped_size = None
 
         brands = params.get("brand")
+        print("brands raw")
+        print(brands)
         if brands is None:
             brands = []
         else:
-            brands = [BRANDS_MAP.get(brand) for brand in brands]
-
-        categories_str = params.get("category")
-        if categories_str is not None:
-            categories_ids = [
-                CATEGORIES_MAP.get(category) for category in categories_str
-            ]
-        else:
-            categories_ids = []
+            brands = [BREANS_MAP.get(brand) for brand in brands]
 
         url = "https://api.mercari.jp/v2/entities:search"
         searchSessionId = "".join(random.choice(CHARACTERS) for i in range(32))
         payload = {
             "userId": "",
             "pageSize": item_count,
             "pageToken": page_token,
@@ -97,15 +79,15 @@
             "searchCondition": {
                 "keyword": keyword,
                 "excludeKeyword": "",
                 "sort": "SORT_CREATED_TIME",
                 "order": "ORDER_DESC",
                 "status": ["STATUS_ON_SALE"],
                 "sizeId": [mapped_size],
-                "categoryId": categories_ids,
+                "categoryId": [],
                 "brandId": brands,
                 "sellerId": [],
                 "priceMin": 0,
                 "priceMax": 0,
                 "itemConditionId": [],
                 "shippingPayerId": [],
                 "shippingFromArea": [],
```

### Comparing `postalservice-0.1.4/postalservice/utils/network_utils.py` & `postalservice-0.1.5/postalservice/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `postalservice-0.1.4/postalservice/utils/search_utils.py` & `postalservice-0.1.5/postalservice/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `postalservice-0.1.4/postalservice.egg-info/PKG-INFO` & `postalservice-0.1.5/postalservice.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: postalservice
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for second hand shopping
 Author: Aapo Montin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postal Service Python Library
 [![Mercari](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/mercari_tests.yml)
 [![Fril](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/fril_tests.yml)
+[![YJP](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml/badge.svg)](https://github.com/apmnt/postalservice_python/actions/workflows/yjp_tests.yml)
 [![PyPI version](https://badge.fury.io/py/postalservice.svg)](https://badge.fury.io/py/postalservice)
 
 Python library for scraping second hand Japanese websites for easier access to the search results. Useful for creating datasets, notification systems, or web APIs. Targets the website API if available, or parses the HTML response.
 
 ## Features
 
 - Mercari, Fril scraping
@@ -61,11 +62,10 @@
 `BaseService` is an abstract base class that defines the interface for a service. All services implement this and therefore have all these class methods:
 
 - `get_search_results(params: dict) -> SearchResults`: Fetches data synchronously using the provided parameters, parses the response, and returns the results as SearchResults object.
 
 - `get_search_results_async(params: dict) -> SearchResults`: Fetches data asynchronously using the provided parameters, parses the response (asynchronously, if needed), and returns the results as SearchResults object. 
 
 ## todo
-- YJP support
-- Filter by brand
+- Rakuten support
 - General improvements to structure of the library
-- Support for getting intermediate/temporary results for slow sites like Fril
+- Support for multiple sizes for sites where only one size is possible to select at a time
```

### Comparing `postalservice-0.1.4/tests/baseservicetestclass.py` & `postalservice-0.1.5/tests/baseservicetestclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,18 +130,7 @@
         print(sparams.get_dict())
         searchresults = self.service.get_search_results(sparams.get_dict())
         print(searchresults.to_json())
         # Loop through the items and assert the brand is comme des garcons
         for i in range(searchresults.count()):
             self.logger.info(searchresults.get(i)["brand"])
             self.assertTrue("JUNYA WATANABE" in searchresults.get(i)["brand"])
-
-    def test_search_by_category(self):
-        sparams = SearchParams("comme des garcons", category=["accessories"])
-        print(sparams.get_dict())
-        searchresults = asyncio.run(
-            self.service.get_search_results_async(sparams.get_dict())
-        )
-        print(searchresults.to_json())
-        # Loop through the items and assert the category is shirts (manually)
-        for i in range(searchresults.count()):
-            self.logger.info(searchresults.get(i))
```

