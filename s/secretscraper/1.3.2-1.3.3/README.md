# Comparing `tmp/secretscraper-1.3.2.tar.gz` & `tmp/secretscraper-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.2.tar", max compression
+gzip compressed data, was "secretscraper-1.3.3.tar", max compression
```

## Comparing `secretscraper-1.3.2.tar` & `secretscraper-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.2/LICENSE
--rw-r--r--   0        0        0     6848 2024-04-28 06:09:06.202652 secretscraper-1.3.2/README.md
--rw-r--r--   0        0        0     1438 2024-04-28 05:22:20.977269 secretscraper-1.3.2/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-28 05:22:11.471379 secretscraper-1.3.2/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     4333 2024-04-28 06:03:46.871130 secretscraper-1.3.2/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.2/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-28 03:25:18.536550 secretscraper-1.3.2/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.2/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.2/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.2/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.2/src/secretscraper/exception.py
--rw-r--r--   0        0        0    12301 2024-04-28 05:11:46.059038 secretscraper-1.3.2/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.2/src/secretscraper/filter.py
--rw-r--r--   0        0        0     5241 2024-04-28 04:44:33.112445 secretscraper-1.3.2/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.2/src/secretscraper/log.py
--rw-r--r--   0        0        0     6919 2024-04-28 05:14:28.249196 secretscraper-1.3.2/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.2/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4316 2024-04-28 05:20:02.448324 secretscraper-1.3.2/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     1368 2024-04-28 05:40:42.876681 secretscraper-1.3.2/src/secretscraper/util.py
--rw-r--r--   0        0        0     7822 1970-01-01 00:00:00.000000 secretscraper-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.3/LICENSE
+-rw-r--r--   0        0        0     6848 2024-04-28 06:27:58.884906 secretscraper-1.3.3/README.md
+-rw-r--r--   0        0        0     1529 2024-04-28 06:28:17.915587 secretscraper-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-28 06:28:17.926857 secretscraper-1.3.3/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     4277 2024-04-28 06:26:30.968337 secretscraper-1.3.3/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.3/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2442 2024-04-28 03:25:18.536550 secretscraper-1.3.3/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.3/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.3/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.3/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.3/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    12276 2024-04-28 06:26:30.980493 secretscraper-1.3.3/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.3/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     5861 2024-04-28 06:26:30.984899 secretscraper-1.3.3/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.3/src/secretscraper/log.py
+-rw-r--r--   0        0        0     6919 2024-04-28 05:14:28.249196 secretscraper-1.3.3/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.3/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4316 2024-04-28 05:20:02.448324 secretscraper-1.3.3/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     1368 2024-04-28 05:40:42.876681 secretscraper-1.3.3/src/secretscraper/util.py
+-rw-r--r--   0        0        0     7917 1970-01-01 00:00:00.000000 secretscraper-1.3.3/PKG-INFO
```

### Comparing `secretscraper-1.3.2/LICENSE` & `secretscraper-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/README.md` & `secretscraper-1.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -202,19 +202,19 @@
     loaded: true
 
 ```
 
 ---
 
 # TODO
-- [ ] Support windows
 - [ ] Support headless browser
 - [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
 - [ ] Generate configuration file
+- [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
 ## 2024.4.28 Version 1.3.2
```

### Comparing `secretscraper-1.3.2/pyproject.toml` & `secretscraper-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.2"
+version = "1.3.3"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
@@ -12,15 +12,18 @@
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
 dynaconf = "^3.1.12"
 click = "^8.1.3"
 pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
-hyperscan = "^0.7.7"
+hyperscan = [
+    { version = "^0.7.7", platform = "darwin" },
+    { version = "^0.7.7", platform = "linux" }
+]
 bs4 = "^0.0.2"
 aiohttp = "^3.9.4"
 pytest-cov = "^5.0.0"
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
```

### Comparing `secretscraper-1.3.2/src/secretscraper/cmdline.py` & `secretscraper-1.3.3/src/secretscraper/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from click import Context
 from dynaconf.base import Settings
 
 from secretscraper import __version__
 from secretscraper.config import settings
 from secretscraper.exception import FacadeException
 from secretscraper.facade import CrawlerFacade, FileScannerFacade
-from secretscraper.handler import HyperscanRegexHandler
 from secretscraper.log import init_log
 
 facade_settings = settings  # for unit test
 facade_obj = None
 
 
 # @click.group(invoke_without_command=True)
```

### Comparing `secretscraper-1.3.2/src/secretscraper/config/__init__.py` & `secretscraper-1.3.3/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/config/settings.yml` & `secretscraper-1.3.3/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/coroutinue.py` & `secretscraper-1.3.3/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/crawler.py` & `secretscraper-1.3.3/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/entity.py` & `secretscraper-1.3.3/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/exception.py` & `secretscraper-1.3.3/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/facade.py` & `secretscraper-1.3.3/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import click
 import dynaconf
 
 from .crawler import Crawler
 from .exception import FacadeException, FileScannerException
 from .filter import (ChainedURLFilter, DomainBlackListURLFilter,
                      DomainWhiteListURLFilter)
-from .handler import HyperscanRegexHandler, ReRegexHandler
+from .handler import get_regex_handler
 from .output_formatter import Formatter
 from .scanner import FileScanner
 from .urlparser import URLParser, RegexURLParser
 from .util import Range, read_rules_from_setting
 
 logger = logging.getLogger(__name__)
 
@@ -227,21 +227,21 @@
         # Verbose
         verbose: typing.Optional[bool] = self.custom_settings.get("verbose", None)
         if verbose is not None:
             self.settings["verbose"] = verbose
 
         # Read rules from config file
         rules: dict[str, str] = read_rules_from_setting(self.settings)
-        handler = HyperscanRegexHandler(rules)
+        handler = get_regex_handler(rules)
 
         # Read url/js regex
         rules: list[str] = self.settings.get("urlFind")
         rules.extend(self.settings.get("jsFind"))
         rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
-        parser = RegexURLParser(ReRegexHandler(rules_dict))
+        parser = RegexURLParser(get_regex_handler(rules_dict))
 
         crawler = Crawler(
             start_urls=list(start_urls),
             url_filter=urlfilter,
             # parser=URLParser(),
             parser=parser,
             handler=handler,
@@ -308,15 +308,15 @@
         )
         if outfile is not None:
             self.outfile = outfile
         print_config(f"Output file: {self.outfile}")
 
         # Read rules from config file
         rules: dict[str, str] = read_rules_from_setting(self.settings)
-        handler = HyperscanRegexHandler(rules)
+        handler = get_regex_handler(rules)
 
         # Get all files from directory
         base: typing.Optional[pathlib.Path] = self.custom_settings.get('local', None)
         if base is None:
             raise FacadeException(f"Internal error: No base directory")
         targets: list[pathlib.Path] = list()
         if base.is_file():
```

### Comparing `secretscraper-1.3.2/src/secretscraper/filter.py` & `secretscraper-1.3.3/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/handler.py` & `secretscraper-1.3.3/src/secretscraper/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Handler module for extracting data from HTML pages and other text files crawled from website"""
 
 import queue
 import re
+import sys
 import typing
 from typing import Protocol
 
-import hyperscan
 from bs4 import BeautifulSoup, NavigableString, Tag
 
 from secretscraper.entity import Secret
 from secretscraper.exception import HandlerException
 
 # T = typing.TypeVar("T")
 # IterableAsyncOrSync: typing.TypeAlias = typing.Iterable[T] | typing.AsyncIterable[T]
@@ -52,82 +52,87 @@
                     secret_data = match if type(match) is not tuple else match[0]
                     secret_type = self.types[index]
                     secret = Secret(type=secret_type, data=secret_data)
                     result_list.append(secret)
         return result_list
 
 
-class HyperscanRegexHandler(Handler):
-    """Regex handler using `hyperscan` module"""
-
-    def __init__(
-        self, rules: dict[str, str], lazy_init: bool = False, hs_flag: int = 0
-    ):
-        """
-
-        :param rules: regex rules dictionary with keys indicating type and values indicating the regex
-        :param lazy_init: True for deferring the initialization to actively call the init() method, otherwise initialize immediately
-        :param hs_flag: hyperscan flag perform to every expressions
-        """
-        # self.output_queue: queue.Queue[Secret] = queue.Queue()
-        self.rules = rules
-        self._init: bool = False
-        self._hs_flag: int = (
-            hs_flag | hyperscan.HS_FLAG_SOM_LEFTMOST | hyperscan.HS_FLAG_CASELESS
-        )
-        self._db: typing.Optional[hyperscan.Database] = None
-        self.patterns: dict[int, bytes] = dict()  # pattern id => regex in bytes
-        self.types: dict[int, str] = dict()  # pattern id => type
-        if not lazy_init:
-            self.init()
-
-    def init(self):
-        """Initialize the hyperscan database."""
-        self._db = hyperscan.Database()
-        flags: list[int] = [self._hs_flag for _ in range(len(self.rules))]
-        for index, type_str in enumerate(self.rules):
-            regex = self.rules.get(type_str)
-            self.patterns[index] = regex.encode("utf-8")
-            self.types[index] = type_str
-
-        self._db.compile(
-            expressions=list(self.patterns.values()),
-            ids=list(self.patterns.keys()),
-            elements=len(self.patterns),
-            flags=flags,
-        )
-
-        self._init = True
-
-    def handle(self, text: str) -> typing.Iterable[Secret]:
-        """Extract secret data via the pre-compiled hyperscan database
-
-        This method is IO-bound.
-        """
-        if not self._init:
-            raise HandlerException("Hyperscan database is not initialized")
-
-        results: list[Secret] = list()
-
-        def on_match(
-            id: int,
-            froms: int,
-            to: int,
-            flags: int,
-            context: typing.Optional[typing.Any] = None,
-        ) -> typing.Optional[bool]:
-            match = text[froms:to]
-            type = self.types.get(id)
-            results.append(Secret(type, data=match))
-            return None
-
-        self._db.scan(
-            text.encode("utf8"), match_event_handler=on_match
-        )  # block call until all regex operation finish
-        return results
+if not sys.platform.startswith("win"):
+    # hyperscan does not support windows
+    import hyperscan
+
+
+    class HyperscanRegexHandler(Handler):
+        """Regex handler using `hyperscan` module"""
+
+        def __init__(
+            self, rules: dict[str, str], lazy_init: bool = False, hs_flag: int = 0
+        ):
+            """
+
+            :param rules: regex rules dictionary with keys indicating type and values indicating the regex
+            :param lazy_init: True for deferring the initialization to actively call the init() method, otherwise initialize immediately
+            :param hs_flag: hyperscan flag perform to every expressions
+            """
+            # self.output_queue: queue.Queue[Secret] = queue.Queue()
+            self.rules = rules
+            self._init: bool = False
+            self._hs_flag: int = (
+                hs_flag | hyperscan.HS_FLAG_SOM_LEFTMOST | hyperscan.HS_FLAG_CASELESS
+            )
+            self._db: typing.Optional[hyperscan.Database] = None
+            self.patterns: dict[int, bytes] = dict()  # pattern id => regex in bytes
+            self.types: dict[int, str] = dict()  # pattern id => type
+            if not lazy_init:
+                self.init()
+
+        def init(self):
+            """Initialize the hyperscan database."""
+            self._db = hyperscan.Database()
+            flags: list[int] = [self._hs_flag for _ in range(len(self.rules))]
+            for index, type_str in enumerate(self.rules):
+                regex = self.rules.get(type_str)
+                self.patterns[index] = regex.encode("utf-8")
+                self.types[index] = type_str
+
+            self._db.compile(
+                expressions=list(self.patterns.values()),
+                ids=list(self.patterns.keys()),
+                elements=len(self.patterns),
+                flags=flags,
+            )
+
+            self._init = True
+
+        def handle(self, text: str) -> typing.Iterable[Secret]:
+            """Extract secret data via the pre-compiled hyperscan database
+
+            This method is IO-bound.
+            """
+            if not self._init:
+                raise HandlerException("Hyperscan database is not initialized")
+
+            results: list[Secret] = list()
+
+            def on_match(
+                id: int,
+                froms: int,
+                to: int,
+                flags: int,
+                context: typing.Optional[typing.Any] = None,
+            ) -> typing.Optional[bool]:
+                match = text[froms:to]
+                type = self.types.get(id)
+                results.append(Secret(type, data=match))
+                return None
+
+            self._db.scan(
+                text.encode("utf8"), match_event_handler=on_match
+            )  # block call until all regex operation finish
+            return results
 
 
 class BSHandler(Handler):
     """BeautifulSoup handler that filter html elements on demand"""
 
     def __init__(
         self, filter_func: typing.Callable[[BeautifulSoup], list[BSResult]]
@@ -143,7 +148,15 @@
         soup = BeautifulSoup(text, "html.parser")
         result: list[BSResult] = self.filter(soup)
         results: list[Secret] = list()
         if result is not None:
             secret = Secret(type="HTML Element", data=result)
             results.append(secret)
         return results
+
+
+def get_regex_handler(rules: dict[str, str], *args, **kwargs) -> Handler:
+    """Return regex handler on current platform"""
+    if sys.platform.startswith("win"):
+        return ReRegexHandler(rules, *args, **kwargs)
+    else:
+        return HyperscanRegexHandler(rules, *args, **kwargs)
```

### Comparing `secretscraper-1.3.2/src/secretscraper/log.py` & `secretscraper-1.3.3/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/output_formatter.py` & `secretscraper-1.3.3/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/scanner.py` & `secretscraper-1.3.3/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/urlparser.py` & `secretscraper-1.3.3/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/src/secretscraper/util.py` & `secretscraper-1.3.3/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.2/PKG-INFO` & `secretscraper-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.2
+Version: 1.3.3
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: hyperscan (>=0.7.7,<0.8.0)
+Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "darwin"
+Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "linux"
 Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
 Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # SecretScraper
 
@@ -226,19 +227,19 @@
     loaded: true
 
 ```
 
 ---
 
 # TODO
-- [ ] Support windows
 - [ ] Support headless browser
 - [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
 - [ ] Generate configuration file
+- [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
 ## 2024.4.28 Version 1.3.2
```

