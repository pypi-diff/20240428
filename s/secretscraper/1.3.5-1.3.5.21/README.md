# Comparing `tmp/secretscraper-1.3.5.tar.gz` & `tmp/secretscraper-1.3.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.5.tar", max compression
+gzip compressed data, was "secretscraper-1.3.5.21.tar", max compression
```

## Comparing `secretscraper-1.3.5.tar` & `secretscraper-1.3.5.21.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5/LICENSE
--rw-r--r--   0        0        0     6931 2024-04-28 10:36:36.702155 secretscraper-1.3.5/README.md
--rw-r--r--   0        0        0     1561 2024-04-28 10:17:34.707725 secretscraper-1.3.5/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-28 10:17:34.697611 secretscraper-1.3.5/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-28 08:01:35.923498 secretscraper-1.3.5/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13239 2024-04-28 09:47:53.979495 secretscraper-1.3.5/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5/src/secretscraper/exception.py
--rw-r--r--   0        0        0    13716 2024-04-28 10:04:29.006701 secretscraper-1.3.5/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5/src/secretscraper/log.py
--rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2049 2024-04-28 09:59:40.730737 secretscraper-1.3.5/src/secretscraper/util.py
--rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 secretscraper-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5.21/LICENSE
+-rw-r--r--   0        0        0     8045 2024-04-28 15:15:35.500487 secretscraper-1.3.5.21/README.md
+-rw-r--r--   0        0        0     1564 2024-04-28 14:48:27.584726 secretscraper-1.3.5.21/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-28 14:48:27.582340 secretscraper-1.3.5.21/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5.21/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5.21/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.5.21/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5.21/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.5.21/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5.21/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5.21/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.5.21/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5.21/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5.21/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5.21/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5.21/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5.21/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5.21/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.5.21/src/secretscraper/util.py
+-rw-r--r--   0        0        0     8983 1970-01-01 00:00:00.000000 secretscraper-1.3.5.21/PKG-INFO
```

### Comparing `secretscraper-1.3.5/LICENSE` & `secretscraper-1.3.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/README.md` & `secretscraper-1.3.5.21/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
 
 ## Overview
 
-SecretScraper is a web scraper tool that can crawl through target websites, scrape from response and extract secret
-information via regular expression.
+SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
+data via regular expression.
 
-## Feature
 
-- Web crawler: scrape through target url and extract all extending urls, roll around through new links until depth or
-  page number exceeds the limitation
+## Feature
+- Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
@@ -48,14 +47,16 @@
 http://scrapeme.live/1
 http://scrapeme.live/2
 http://scrapeme.live/3
 http://scrapeme.live/4
 http://scrapeme.live/1
 ```
 A sample output:
+<img width="1125" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/00dd2053-7b9a-4ef3-a2b2-8c168e8ec0ee">
+
 ```text
 > secretscraper -u http://127.0.0.1:8888
 Target urls num: 1
 Max depth: 1, Max page num: 1000
 Output file: /Users/padishah/Documents/Files/Python_WorkSpace/secretscraper/src/secretscraper/crawler.log
 Target URLs: http://127.0.0.1:8888
 
@@ -110,21 +111,23 @@
                                2(thorough) for max_depth=2, default 1
   --max-page INTEGER           Max page number to crawl, default 100000
   --max-depth INTEGER          Max depth to crawl, default 1
   -o, --outfile FILE           Output result to specified file
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
-                               http://127.0.0.1:7890
+                               socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
+  --detail                     Show detailed result
   -l, --local PATH             Local file or directory, scan local
                                file/directory recursively
   --help                       Show this message and exit.
+
 ```
 
 ### Advanced Usage
 
 #### Thorough Crawl
 
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
@@ -165,14 +168,31 @@
 follow_redirects: false
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
+urlFind:
+  - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
+  - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+  - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
+  - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
+  - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+jsFind:
+  - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+  - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
+  - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+dangerousPath:
+  - logout
+  - update
+  - remove
+  - insert
+  - delete
+
 rules:
   - name: Swagger
     regex: \b[\w/]+?((swagger-ui.html)|(\"swagger\":)|(Swagger UI)|(swaggerUi)|(swaggerVersion))\b
     loaded: true
   - name: ID Card
     regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3}\$)|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
     loaded: true
@@ -204,29 +224,31 @@
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
 - [ ] Add regex doc reference
-- [ ] Generate configuration file
+- [x] Generate configuration file
+- [x] Detect dangerous paths and avoid requesting them
 - [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
   - Prettify output, add `--detail` option
   - Generate default configuration to settings.yml
+  - Avoid requesting dangerous paths
 
 ## 2024.4.28 Version 1.3.2
 - **New Features**
   - Extract links via regex
 
 ## 2024.4.26 Version 1.3.1
 - **New Features**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `secretscraper-1.3.5/pyproject.toml` & `secretscraper-1.3.5.21/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.5"
+version = "1.3.5.21"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.5/src/secretscraper/cmdline.py` & `secretscraper-1.3.5.21/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/config/__init__.py` & `secretscraper-1.3.5.21/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/config/settings.yml` & `secretscraper-1.3.5.21/src/secretscraper/config/settings.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,23 @@
 urlFind:
   - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
   - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
   - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
   - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
   - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
 jsFind:
-    - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
-    - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
-    - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+  - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+  - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
+  - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+dangerousPath:
+  - logout
+  - update
+  - remove
+  - insert
+  - delete
 
 rules:
   - name: Swagger
     regex: \b[\w/]+?((swagger-ui.html)|(\"swagger\":)|(Swagger UI)|(swaggerUi)|(swaggerVersion))\b
     loaded: true
   - name: ID Card
     regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3}\$)|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
```

### Comparing `secretscraper-1.3.5/src/secretscraper/coroutinue.py` & `secretscraper-1.3.5.21/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/crawler.py` & `secretscraper-1.3.5.21/src/secretscraper/crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The facade interfaces to integrate crawler, filter, and handler"""
 
 import asyncio
 import logging
 import queue
+import re
 import threading
 import traceback
 import typing
 from typing import Set
 from urllib.parse import urlparse
 
 import aiohttp
@@ -44,14 +45,15 @@
         num_workers: int = 100,
         proxy: str = None,
         headers: dict = None,
         verbose: bool = False,
         timeout: float = 5,
         debug: bool = False,
         follow_redirects: bool = False,
+        dangerous_paths: list[str] = None,
     ):
         """
 
         :param start_urls: urls to start crawl from
         # :param client: aiohttp client
         :param url_filter: determine whether a url should be crawled
         :param parser: extract child url nodes from html
@@ -59,15 +61,17 @@
         # :param allowed_status: filter response status. None for no filter
         :param max_page_num: max number of urls to crawl, 0 for no limit
         :param max_depth: max url depth, should greater than 0
         :param num_workers: worker number of the async pool
         :param proxy: http proxy
         :param verbose: whether to print exception detail
         :param timeout: timeout for aiohttp request
+        :param dangerous_paths: dangerous paths to evade
         """
+        self.dangerous_paths = dangerous_paths
         self.proxy = proxy
         self.start_urls = start_urls
         # self.client = client
         self.filter = url_filter
         self.parser = parser
         self.handler = handler
         self.max_page_num = max_page_num
@@ -165,18 +169,31 @@
         except asyncio.CancelledError:
             pass
         except Exception as e:
             raise CrawlerException("Unexpected Exception") from e
         finally:
             await self.clean()
 
+    def is_evade(self, url: URLNode) -> bool:
+        """Check whether url should be evaded"""
+        if self.dangerous_paths is not None:
+            path = url.url_object.path
+            if len(
+                [path for p in self.dangerous_paths if re.search(f"{p}", path.strip(), re.IGNORECASE)]
+            ) > 0:
+                return True
+        return False
+
     async def process_one(self, url_node: URLNode):
         """Fetch, extract url children and execute handler on result"""
         if self.max_page_num > 0 and self.total_page >= self.max_page_num:
             return
+        if self.is_evade(url_node):
+            logger.debug(f"Evading {url_node}")
+            return
         logger.debug(f"Processing {url_node.url}")
         self.total_page += 1
         response = await self.fetch(url_node.url)
         if response is not None:  # and response.status == 200
             url_node.response_status = str(response.status_code)
 
             response_text: str = response.text
@@ -297,15 +314,15 @@
         except httpx.ConnectError as e:
             logger.error(f"Connection error for {url}: {e}")
         except httpx.InvalidURL as e:
             logger.error(f"Invalid URL for {url}: {e}")
         except httpx.TimeoutException as e:
             logger.error(f"Timeout while fetching {url} ")
         except httpx.ReadError as e:
-            logger.debug(f"Read error for {url}: {e}") # trigger when keyboard interrupt
+            logger.debug(f"Read error for {url}: {e}")  # trigger when keyboard interrupt
         except KeyboardInterrupt:
             pass  # ignore
         except Exception as e:
             logger.error(f"Unexpected error: {e.__class__} while fetching {url}")
         return response
 
     async def clean(self):
```

### Comparing `secretscraper-1.3.5/src/secretscraper/entity.py` & `secretscraper-1.3.5.21/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/exception.py` & `secretscraper-1.3.5.21/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/facade.py` & `secretscraper-1.3.5.21/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,19 @@
         rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
         parser = RegexURLParser(get_regex_handler(rules_dict, type_="regex"))
 
         # Detailed output
         if self.custom_settings.get("detail", False) is True:
             self.detail_output = True
 
+        # Dangerous paths
+        dangerous_paths: list[str] = list()
+        if self.settings.get("dangerousPath", None) is not None:
+            dangerous_paths.extend(set(self.settings("dangerousPath")))
+
         crawler = Crawler(
             start_urls=list(start_urls),
             url_filter=urlfilter,
             # parser=URLParser(),
             parser=parser,
             handler=handler,
             max_page_num=self.settings.get("max_page_num"),
@@ -277,14 +282,15 @@
             num_workers=self.settings.get("workers_num"),
             proxy=self.settings.get("proxy"),
             headers=headers,
             verbose=self.settings.get("verbose"),
             timeout=self.settings.get("timeout"),
             debug=self.debug,
             follow_redirects=self.settings["follow_redirects"],
+            dangerous_paths = dangerous_paths
         )
         return crawler
 
 
 class FileScannerFacade:
     """Facade for local file scanner"""
```

### Comparing `secretscraper-1.3.5/src/secretscraper/filter.py` & `secretscraper-1.3.5.21/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/handler.py` & `secretscraper-1.3.5.21/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/log.py` & `secretscraper-1.3.5.21/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/output_formatter.py` & `secretscraper-1.3.5.21/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/scanner.py` & `secretscraper-1.3.5.21/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/urlparser.py` & `secretscraper-1.3.5.21/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5/src/secretscraper/util.py` & `secretscraper-1.3.5.21/src/secretscraper/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from collections import namedtuple
 import re
 from urllib.parse import urlparse
 
 from dynaconf import LazySettings
 
+from .entity import URL
 from .exception import SecretScraperException
 
 Range = namedtuple("Range", ["start", "end"])
 
 
 def read_rules_from_setting(settings: LazySettings) -> dict[str, str]:
     """Read rules from settings
```

### Comparing `secretscraper-1.3.5/PKG-INFO` & `secretscraper-1.3.5.21/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.5
+Version: 1.3.5.21
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,21 +22,20 @@
 
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
 
 ## Overview
 
-SecretScraper is a web scraper tool that can crawl through target websites, scrape from response and extract secret
-information via regular expression.
+SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
+data via regular expression.
 
-## Feature
 
-- Web crawler: scrape through target url and extract all extending urls, roll around through new links until depth or
-  page number exceeds the limitation
+## Feature
+- Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
@@ -70,14 +69,16 @@
 http://scrapeme.live/1
 http://scrapeme.live/2
 http://scrapeme.live/3
 http://scrapeme.live/4
 http://scrapeme.live/1
 ```
 A sample output:
+<img width="1125" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/00dd2053-7b9a-4ef3-a2b2-8c168e8ec0ee">
+
 ```text
 > secretscraper -u http://127.0.0.1:8888
 Target urls num: 1
 Max depth: 1, Max page num: 1000
 Output file: /Users/padishah/Documents/Files/Python_WorkSpace/secretscraper/src/secretscraper/crawler.log
 Target URLs: http://127.0.0.1:8888
 
@@ -132,21 +133,23 @@
                                2(thorough) for max_depth=2, default 1
   --max-page INTEGER           Max page number to crawl, default 100000
   --max-depth INTEGER          Max depth to crawl, default 1
   -o, --outfile FILE           Output result to specified file
   -s, --status TEXT            Filter response status to display, seperated by
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
-                               http://127.0.0.1:7890
+                               socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
+  --detail                     Show detailed result
   -l, --local PATH             Local file or directory, scan local
                                file/directory recursively
   --help                       Show this message and exit.
+
 ```
 
 ### Advanced Usage
 
 #### Thorough Crawl
 
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
@@ -187,14 +190,31 @@
 follow_redirects: false
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
+urlFind:
+  - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
+  - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+  - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
+  - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
+  - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+jsFind:
+  - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+  - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
+  - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+dangerousPath:
+  - logout
+  - update
+  - remove
+  - insert
+  - delete
+
 rules:
   - name: Swagger
     regex: \b[\w/]+?((swagger-ui.html)|(\"swagger\":)|(Swagger UI)|(swaggerUi)|(swaggerVersion))\b
     loaded: true
   - name: ID Card
     regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3}\$)|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
     loaded: true
@@ -226,29 +246,31 @@
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
 - [ ] Add regex doc reference
-- [ ] Generate configuration file
+- [x] Generate configuration file
+- [x] Detect dangerous paths and avoid requesting them
 - [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
   - Prettify output, add `--detail` option
   - Generate default configuration to settings.yml
+  - Avoid requesting dangerous paths
 
 ## 2024.4.28 Version 1.3.2
 - **New Features**
   - Extract links via regex
 
 ## 2024.4.26 Version 1.3.1
 - **New Features**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

