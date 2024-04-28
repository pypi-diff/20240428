# Comparing `tmp/secretscraper-1.3.1.tar.gz` & `tmp/secretscraper-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.1.tar", max compression
+gzip compressed data, was "secretscraper-1.3.2.tar", max compression
```

## Comparing `secretscraper-1.3.1.tar` & `secretscraper-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.1/LICENSE
--rw-r--r--   0        0        0     6737 2024-04-28 02:57:57.773811 secretscraper-1.3.1/README.md
--rw-r--r--   0        0        0     1438 2024-04-28 02:57:57.779725 secretscraper-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-28 02:57:57.783810 secretscraper-1.3.1/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-26 07:57:48.575721 secretscraper-1.3.1/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.1/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-16 11:30:07.208957 secretscraper-1.3.1/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.1/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.1/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.1/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.1/src/secretscraper/exception.py
--rw-r--r--   0        0        0    11777 2024-04-28 02:53:58.636401 secretscraper-1.3.1/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2093 2024-04-15 07:08:56.960583 secretscraper-1.3.1/src/secretscraper/filter.py
--rw-r--r--   0        0        0     4817 2024-04-15 07:08:56.998319 secretscraper-1.3.1/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.1/src/secretscraper/log.py
--rw-r--r--   0        0        0     6802 2024-04-26 08:02:37.301072 secretscraper-1.3.1/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.1/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     2645 2024-04-15 07:08:56.999973 secretscraper-1.3.1/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0      873 2024-04-16 10:31:30.742064 secretscraper-1.3.1/src/secretscraper/util.py
--rw-r--r--   0        0        0     7711 1970-01-01 00:00:00.000000 secretscraper-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.2/LICENSE
+-rw-r--r--   0        0        0     6848 2024-04-28 06:09:06.202652 secretscraper-1.3.2/README.md
+-rw-r--r--   0        0        0     1438 2024-04-28 05:22:20.977269 secretscraper-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-28 05:22:11.471379 secretscraper-1.3.2/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     4333 2024-04-28 06:03:46.871130 secretscraper-1.3.2/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.2/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2442 2024-04-28 03:25:18.536550 secretscraper-1.3.2/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.2/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.2/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.2/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.2/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    12301 2024-04-28 05:11:46.059038 secretscraper-1.3.2/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.2/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     5241 2024-04-28 04:44:33.112445 secretscraper-1.3.2/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.2/src/secretscraper/log.py
+-rw-r--r--   0        0        0     6919 2024-04-28 05:14:28.249196 secretscraper-1.3.2/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.2/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4316 2024-04-28 05:20:02.448324 secretscraper-1.3.2/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     1368 2024-04-28 05:40:42.876681 secretscraper-1.3.2/src/secretscraper/util.py
+-rw-r--r--   0        0        0     7822 1970-01-01 00:00:00.000000 secretscraper-1.3.2/PKG-INFO
```

### Comparing `secretscraper-1.3.1/LICENSE` & `secretscraper-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/README.md` & `secretscraper-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -202,24 +202,29 @@
     loaded: true
 
 ```
 
 ---
 
 # TODO
-- [x] Scan local file
 - [ ] Support windows
 - [ ] Support headless browser
-- [ ] Extract links via regex
 - [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
+- [ ] Generate configuration file
+- [x] Scan local file
+- [x] Extract links via regex
 
 ---
 
 # Change Log
-## 2024.4.26 Version 1.3
+## 2024.4.28 Version 1.3.2
+- **New Features**
+  - Extract links via regex
+
+## 2024.4.26 Version 1.3.1
 - **New Features**
   - [x] Support scan local files
 
 ## 2024.4.15
 - [x] Add status to url result
 - [x] All crawler test passed
```

### Comparing `secretscraper-1.3.1/pyproject.toml` & `secretscraper-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.1"
+version = "1.3.2"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.1/src/secretscraper/cmdline.py` & `secretscraper-1.3.2/src/secretscraper/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 @click.option(
     "-x",
     "--proxy",
     help="Set proxy, e.g. http://127.0.0.1:8080, http://127.0.0.1:7890",
     type=click.STRING,
 )
 @click.option("-H", "--hide-regex", help="Hide regex search result", is_flag=True)
-@click.option("-F", "--follow-redirects", help="Follow redirects", is_flag=True, default=False)
+@click.option("-F", "--follow-redirects", help="Follow redirects", is_flag=True)
 @click.option("-u", "--url", help="Target url", type=click.STRING)
 @click.option("-l", "--local", help="Local file or directory, scan local file/directory recursively ",
               type=click.Path(exists=True, file_okay=True, dir_okay=True, path_type=pathlib.Path))
 def main(**options):
     """Main commands"""
     if options["version"]:
         click.echo(__version__)
```

### Comparing `secretscraper-1.3.1/src/secretscraper/config/__init__.py` & `secretscraper-1.3.2/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/coroutinue.py` & `secretscraper-1.3.2/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/crawler.py` & `secretscraper-1.3.2/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/entity.py` & `secretscraper-1.3.2/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/exception.py` & `secretscraper-1.3.2/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/facade.py` & `secretscraper-1.3.2/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import click
 import dynaconf
 
 from .crawler import Crawler
 from .exception import FacadeException, FileScannerException
 from .filter import (ChainedURLFilter, DomainBlackListURLFilter,
                      DomainWhiteListURLFilter)
-from .handler import HyperscanRegexHandler
+from .handler import HyperscanRegexHandler, ReRegexHandler
 from .output_formatter import Formatter
 from .scanner import FileScanner
-from .urlparser import URLParser
+from .urlparser import URLParser, RegexURLParser
 from .util import Range, read_rules_from_setting
 
 logger = logging.getLogger(__name__)
 
 warnings.filterwarnings("ignore")  # ignore all warnings
 
 
@@ -192,18 +192,22 @@
             for status_ex in status.split(","):
                 status_ex = status_ex.strip()
                 if status_ex.__contains__("-"):
                     min_status = status_ex.split("-")[0]
                     max_status = status_ex.split("-")[1]
                     if min_status >= max_status:
                         raise FacadeException(f"Invalid status range: {status_ex}")
+                    if allowed_status is None:
+                        allowed_status = list()
                     allowed_status.append(
                         Range(start=int(min_status), end=int(max_status) + 1)
                     )
                 else:
+                    if allowed_status is None:
+                        allowed_status = list()
                     allowed_status.append(
                         Range(start=int(status_ex), end=int(status_ex) + 1)
                     )
         self.formatter._allowed_status = allowed_status
 
         # UA and Headers
         headers = self.settings.get("headers")
@@ -225,18 +229,25 @@
         if verbose is not None:
             self.settings["verbose"] = verbose
 
         # Read rules from config file
         rules: dict[str, str] = read_rules_from_setting(self.settings)
         handler = HyperscanRegexHandler(rules)
 
+        # Read url/js regex
+        rules: list[str] = self.settings.get("urlFind")
+        rules.extend(self.settings.get("jsFind"))
+        rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
+        parser = RegexURLParser(ReRegexHandler(rules_dict))
+
         crawler = Crawler(
             start_urls=list(start_urls),
             url_filter=urlfilter,
-            parser=URLParser(),
+            # parser=URLParser(),
+            parser=parser,
             handler=handler,
             max_page_num=self.settings.get("max_page_num"),
             max_depth=self.settings.get("max_depth"),
             num_workers=self.settings.get("workers_num"),
             proxy=self.settings.get("proxy"),
             headers=headers,
             verbose=self.settings.get("verbose"),
```

### Comparing `secretscraper-1.3.1/src/secretscraper/filter.py` & `secretscraper-1.3.2/src/secretscraper/filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """URL filters that determine whether or not a URL should be crawled"""
 
 import fnmatch
 from typing import List, Protocol, Set
 
 from secretscraper.entity import URL, URLNode
+from secretscraper.util import to_host_port
 
 
 class URLFilter(Protocol):
     """Base interface for URL filters"""
 
     def doFilter(self, url: URL) -> bool:
         """Whether a URL should be crawled"""
@@ -23,15 +24,15 @@
     def doFilter(self, url: URL) -> bool:
         """Whether a url's domain is whitelisted
 
         - Support wildcards and any other Unix filename pattern.
         - Case-insensitive
 
         """
-        domain: str = url.netloc
+        domain, _ = to_host_port(url.netloc)
         match: bool = False
         for pattern in self.white_list:
             if fnmatch.fnmatch(domain, pattern):
                 match = True
                 break
         return match
 
@@ -43,15 +44,15 @@
         self.blacklist = blacklist
 
     def doFilter(self, url: URL) -> bool:
         """Whether a url's domain is blacklisted
 
         :return bool: True if url's domain is not in blacklist
         """
-        domain: str = url.netloc
+        domain, _ = to_host_port(url.netloc)
         match: bool = False
         for pattern in self.blacklist:
             if fnmatch.fnmatch(domain, pattern):
                 match = True
                 break
         return not match
```

### Comparing `secretscraper-1.3.1/src/secretscraper/handler.py` & `secretscraper-1.3.2/src/secretscraper/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,37 +19,44 @@
 class Handler(Protocol):
     """Base class for different types of handlers"""
 
     def handle(self, text: str) -> typing.Iterable[Secret]: ...
 
 
 class ReRegexHandler(Handler):
-    """(Deprecated) Regex handler using the `re` module, simple but have lowest performance."""
+    """ Regex handler using the `re` module, simple but have lowest performance."""
 
-    def __init__(self, rules: dict[str, str]):
+    def __init__(self, rules: dict[str, str], flags: int = 0):
         """
 
         :param rules: rules dictionary with keys indicating type and values indicating the regex
         """
         self.types = list(rules.keys())
         regexes = list(rules.values())
-        self.regexes: list = list()
+        self.regexes: list[re.Pattern] = list()
         for regex in regexes:
-            self.regexes.append(re.compile(regex))
+            self.regexes.append(re.compile(regex, flags=flags | re.IGNORECASE))
 
     def handle(self, text: str) -> typing.Iterable[Secret]:
         """Extract secret data"""
         result_list: list[Secret] = list()
         for index, regex in enumerate(self.regexes):
-            match = regex.search(text)
-            if match is not None:
-                secret_data = match.group(0)
-                secret_type = self.types[index]
-                secret = Secret(type=secret_type, data=secret_data)
-                result_list.append(secret)
+            # match = regex.search(text)
+            # if match is not None:
+            #     secret_data = match.group(0)
+            #     secret_type = self.types[index]
+            #     secret = Secret(type=secret_type, data=secret_data)
+            #     result_list.append(secret)
+            matches = regex.findall(text)
+            for match in matches:
+                if match is not None:
+                    secret_data = match if type(match) is not tuple else match[0]
+                    secret_type = self.types[index]
+                    secret = Secret(type=secret_type, data=secret_data)
+                    result_list.append(secret)
         return result_list
 
 
 class HyperscanRegexHandler(Handler):
     """Regex handler using `hyperscan` module"""
 
     def __init__(
```

### Comparing `secretscraper-1.3.1/src/secretscraper/log.py` & `secretscraper-1.3.2/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/src/secretscraper/output_formatter.py` & `secretscraper-1.3.2/src/secretscraper/output_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,21 @@
         return click.style(content, fg="bright_blue")
 
     def filter(self, url: URLNode) -> bool:
         """Determine whether a url should be displayed"""
         if self._allowed_status is None:
             return True
         for status_range in self._allowed_status:
-            if status_range.start <= url.response_status < status_range.end:
-                continue
-            else:
-                return False
+            try:
+                if status_range.start <= int(url.response_status) < status_range.end:
+                    continue
+                else:
+                    return False
+            except ValueError:
+                return False  # default discard
         return True
 
     def output_found_domains(
         self, found_urls: typing.Iterable[URLNode], is_print: bool = False
     ) -> str:
         """Output the found domains"""
         if not is_print:
```

### Comparing `secretscraper-1.3.1/src/secretscraper/scanner.py` & `secretscraper-1.3.2/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.1/PKG-INFO` & `secretscraper-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.1
+Version: 1.3.2
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -226,25 +226,30 @@
     loaded: true
 
 ```
 
 ---
 
 # TODO
-- [x] Scan local file
 - [ ] Support windows
 - [ ] Support headless browser
-- [ ] Extract links via regex
 - [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
+- [ ] Generate configuration file
+- [x] Scan local file
+- [x] Extract links via regex
 
 ---
 
 # Change Log
-## 2024.4.26 Version 1.3
+## 2024.4.28 Version 1.3.2
+- **New Features**
+  - Extract links via regex
+
+## 2024.4.26 Version 1.3.1
 - **New Features**
   - [x] Support scan local files
 
 ## 2024.4.15
 - [x] Add status to url result
 - [x] All crawler test passed
```

