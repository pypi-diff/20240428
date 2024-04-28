# Comparing `tmp/secretscraper-1.3.4.tar.gz` & `tmp/secretscraper-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.4.tar", max compression
+gzip compressed data, was "secretscraper-1.3.5.tar", max compression
```

## Comparing `secretscraper-1.3.4.tar` & `secretscraper-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.4/LICENSE
--rw-r--r--   0        0        0     6848 2024-04-28 06:27:58.884906 secretscraper-1.3.4/README.md
--rw-r--r--   0        0        0     1529 2024-04-28 06:44:05.257369 secretscraper-1.3.4/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-28 06:44:05.260383 secretscraper-1.3.4/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     4277 2024-04-28 06:26:30.968337 secretscraper-1.3.4/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.4/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2442 2024-04-28 03:25:18.536550 secretscraper-1.3.4/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.4/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.4/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.4/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.4/src/secretscraper/exception.py
--rw-r--r--   0        0        0    12276 2024-04-28 06:26:30.980493 secretscraper-1.3.4/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.4/src/secretscraper/filter.py
--rw-r--r--   0        0        0     5861 2024-04-28 06:26:30.984899 secretscraper-1.3.4/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.4/src/secretscraper/log.py
--rw-r--r--   0        0        0     6919 2024-04-28 05:14:28.249196 secretscraper-1.3.4/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.4/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4316 2024-04-28 05:20:02.448324 secretscraper-1.3.4/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     1368 2024-04-28 05:40:42.876681 secretscraper-1.3.4/src/secretscraper/util.py
--rw-r--r--   0        0        0     7776 1970-01-01 00:00:00.000000 secretscraper-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5/LICENSE
+-rw-r--r--   0        0        0     6931 2024-04-28 10:36:36.702155 secretscraper-1.3.5/README.md
+-rw-r--r--   0        0        0     1561 2024-04-28 10:17:34.707725 secretscraper-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-28 10:17:34.697611 secretscraper-1.3.5/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2442 2024-04-28 08:01:35.923498 secretscraper-1.3.5/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13239 2024-04-28 09:47:53.979495 secretscraper-1.3.5/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    13716 2024-04-28 10:04:29.006701 secretscraper-1.3.5/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2049 2024-04-28 09:59:40.730737 secretscraper-1.3.5/src/secretscraper/util.py
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 secretscraper-1.3.5/PKG-INFO
```

### Comparing `secretscraper-1.3.4/LICENSE` & `secretscraper-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/README.md` & `secretscraper-1.3.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
-- Platform: MaxOS or Ubuntu, no support for Windows temporarily(due to [hyperscan](https://pypi.org/project/hyperscan/) is employed in this project).
-- Python Version: 3.11
+- Platform: Test on MaxOS, Ubuntu and Windows.
+- Python Version >= 3.11
 
 ## Usage
 
 ### Install
 
 ```bash
 pip install secretscraper
@@ -203,24 +203,31 @@
 
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
-- [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
 - [ ] Generate configuration file
+- [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.28 Version 1.3.5
+- **New Features**
+  - Support windows
+  - Optimize crawler
+  - Prettify output, add `--detail` option
+  - Generate default configuration to settings.yml
+
 ## 2024.4.28 Version 1.3.2
 - **New Features**
   - Extract links via regex
 
 ## 2024.4.26 Version 1.3.1
 - **New Features**
   - [x] Support scan local files
```

### Comparing `secretscraper-1.3.4/pyproject.toml` & `secretscraper-1.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.4"
+version = "1.3.5"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
@@ -16,15 +16,15 @@
 click = "^8.1.3"
 hyperscan = [
     { version = "^0.7.7", platform = "darwin" },
     { version = "^0.7.7", platform = "linux" }
 ]
 bs4 = "^0.0.2"
 aiohttp = "^3.9.4"
-httpx = "^0.27.0"
+httpx = {extras = ["socks"], version = "^0.27.0"}
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
```

### Comparing `secretscraper-1.3.4/src/secretscraper/config/__init__.py` & `secretscraper-1.3.5/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/config/settings.yml` & `secretscraper-1.3.5/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/coroutinue.py` & `secretscraper-1.3.5/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/crawler.py` & `secretscraper-1.3.5/src/secretscraper/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,25 +218,27 @@
         is_html = False
         try:
             content_type = response.headers['content-type']
         except KeyError:
             content_type = ""
         if content_type.startswith("text"):
             is_text_like = True
-            if content_type.strip() == "text/html":
+            if content_type.strip().startswith("text/html"):
                 is_html = True
         elif content_type.startswith("application"):
             if content_type.endswith(
                 "octet-stream"
             ) or content_type.endswith("pdf"):
                 is_text_like = False
             else:
                 is_text_like = True
 
-        if not is_text_like:
+        if not is_text_like or not is_html:  # or not is_html just process html
+            return
+        if response.status_code != 200:  # just process normal response
             return
 
         if self.max_depth <= 0 or url_node.depth + 1 <= self.max_depth:
             # avoid enqueue urls with excessive depth
             # for non-html response, just record, no visit
             is_extending = True
         else:
@@ -294,14 +296,16 @@
             logger.error(f"Timeout while fetching {url}")
         except httpx.ConnectError as e:
             logger.error(f"Connection error for {url}: {e}")
         except httpx.InvalidURL as e:
             logger.error(f"Invalid URL for {url}: {e}")
         except httpx.TimeoutException as e:
             logger.error(f"Timeout while fetching {url} ")
+        except httpx.ReadError as e:
+            logger.debug(f"Read error for {url}: {e}") # trigger when keyboard interrupt
         except KeyboardInterrupt:
             pass  # ignore
         except Exception as e:
             logger.error(f"Unexpected error: {e.__class__} while fetching {url}")
         return response
 
     async def clean(self):
```

### Comparing `secretscraper-1.3.4/src/secretscraper/entity.py` & `secretscraper-1.3.5/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/exception.py` & `secretscraper-1.3.5/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/facade.py` & `secretscraper-1.3.5/src/secretscraper/facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import copy
 import functools
 import logging
 import pathlib
 import traceback
 import typing
 import warnings
+from urllib.parse import urlparse
 from collections import namedtuple
 
 import click
 import dynaconf
 
 from .crawler import Crawler
 from .exception import FacadeException, FileScannerException
 from .filter import (ChainedURLFilter, DomainBlackListURLFilter,
                      DomainWhiteListURLFilter)
 from .handler import get_regex_handler
 from .output_formatter import Formatter
 from .scanner import FileScanner
 from .urlparser import URLParser, RegexURLParser
-from .util import Range, read_rules_from_setting
+from .util import Range, read_rules_from_setting, to_host_port
 
 logger = logging.getLogger(__name__)
 
 warnings.filterwarnings("ignore")  # ignore all warnings
 
 
 def print_func(f: typing.IO, func: typing.Callable, content: str, **kwargs) -> None:
@@ -69,14 +70,15 @@
         self.custom_settings = custom_settings
         self.formatter = Formatter()
         self.hide_regex: bool = False
         self.outfile = pathlib.Path(__file__).parent / "crawler.log"
         self.print_func = print_func
         self.debug: bool = False
         self.follow_redirects: bool = False
+        self.detail_output: bool = False
         self.crawler: Crawler = self.create_crawler()
 
     def start(self):
         """Start the crawler and output"""
         with self.outfile.open("w") as f:
             try:
 
@@ -84,25 +86,46 @@
                 print_func_colorful(f,
                                     self.print_func,
                                     f"Target URLs: {', '.join(self.crawler.start_urls)}",
                                     bold=True,
                                     blink=True,
                                     )
                 self.crawler.start()
-
-                # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
-                self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
-
-                self.formatter.output_found_domains(list(self.crawler.found_urls), True)
-
-                if not self.hide_regex:
-                    print_func_colorful(f, self.print_func,
-                                        f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
-                                        )
-                print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
+                if self.detail_output:
+                    # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
+                    self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
+
+                    if not self.hide_regex:
+                        print_func_colorful(f, self.print_func,
+                                            f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
+                                            )
+                    print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
+                    self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+                else:
+                    # tidy output
+                    # URLs per domain
+                    domains = set()
+                    for url in self.crawler.start_urls:
+                        try:
+                            obj = urlparse(url)
+                            domain, _ = to_host_port(obj.netloc)
+                            if len(domain) > 0:
+                                domains.add(domain.strip())
+                        except:
+                            pass
+                    self.formatter.output_url_per_domain(domains, self.crawler.url_dict)
+                    # JS per domain
+                    self.formatter.output_url_per_domain(domains, self.crawler.js_dict, "JS")
+                    # Domains
+                    self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+                    # Secrets
+                    if not self.hide_regex:
+                        print_func_colorful(f, self.print_func,
+                                            f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
+                                            )
             except KeyboardInterrupt:
                 self.print_func("\nExiting...")
                 self.crawler.close_all()
             except Exception as e:
                 self.print_func(f"Unexpected error: {e}.\nExiting...")
                 self.crawler.close_all()
                 # raise FacadeException from e
@@ -150,15 +173,15 @@
             with url_file.open("r") as f:
                 lines = f.readlines()
                 for line in lines:
                     if len(line.strip()) == 0:
                         continue
                     start_urls.add(line.strip())
         if url is not None:
-            start_urls.add(url)
+            start_urls.add(url.strip())
         print_config(f"Target urls num: {len(start_urls)}")
 
         # Specify mode
         mode: typing.Optional[int] = self.custom_settings.get("mode", None)
         if mode is not None:
             mode = int(mode)
             if mode == 1:
@@ -233,15 +256,19 @@
         rules: dict[str, str] = read_rules_from_setting(self.settings)
         handler = get_regex_handler(rules)
 
         # Read url/js regex
         rules: list[str] = self.settings.get("urlFind")
         rules.extend(self.settings.get("jsFind"))
         rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
-        parser = RegexURLParser(get_regex_handler(rules_dict))
+        parser = RegexURLParser(get_regex_handler(rules_dict, type_="regex"))
+
+        # Detailed output
+        if self.custom_settings.get("detail", False) is True:
+            self.detail_output = True
 
         crawler = Crawler(
             start_urls=list(start_urls),
             url_filter=urlfilter,
             # parser=URLParser(),
             parser=parser,
             handler=handler,
```

### Comparing `secretscraper-1.3.4/src/secretscraper/filter.py` & `secretscraper-1.3.5/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/handler.py` & `secretscraper-1.3.5/src/secretscraper/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -150,13 +150,21 @@
         results: list[Secret] = list()
         if result is not None:
             secret = Secret(type="HTML Element", data=result)
             results.append(secret)
         return results
 
 
-def get_regex_handler(rules: dict[str, str], *args, **kwargs) -> Handler:
+def get_regex_handler(rules: dict[str, str], type_: str = "", *args, **kwargs) -> Handler:
     """Return regex handler on current platform"""
-    if sys.platform.startswith("win"):
-        return ReRegexHandler(rules, *args, **kwargs)
+    if len(type_) == 0:
+        if sys.platform.startswith("win"):
+            return ReRegexHandler(rules, *args, **kwargs)
+        else:
+            return HyperscanRegexHandler(rules, *args, **kwargs)
     else:
-        return HyperscanRegexHandler(rules, *args, **kwargs)
+        if type == "regex":
+            return ReRegexHandler(rules, *args, **kwargs)
+        elif type == "hyperscan":
+            return HyperscanRegexHandler(rules, *args, **kwargs)
+        else:
+            return ReRegexHandler(rules, *args, **kwargs)
```

### Comparing `secretscraper-1.3.4/src/secretscraper/log.py` & `secretscraper-1.3.5/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/output_formatter.py` & `secretscraper-1.3.5/src/secretscraper/output_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 import sys
 import typing
 
 import click
 
 from .entity import URL, Secret, URLNode
-from .util import Range
+from .util import Range, to_host_port
 
 
 class Formatter:
     """Colorful output for terminal and non-colorful output for out-file"""
 
     def __init__(
         self,
@@ -46,14 +46,19 @@
             return click.style(status, fg="red")
 
     def format_normal_result(self, content: str) -> str:
         return click.style(content, fg="bright_blue")
 
     def filter(self, url: URLNode) -> bool:
         """Determine whether a url should be displayed"""
+        try:
+            if int(url.response_status) == 404:  # filter 404 by default
+                return False
+        except ValueError:
+            pass
         if self._allowed_status is None:
             return True
         for status_range in self._allowed_status:
             try:
                 if status_range.start <= int(url.response_status) < status_range.end:
                     continue
                 else:
@@ -65,20 +70,20 @@
     def output_found_domains(
         self, found_urls: typing.Iterable[URLNode], is_print: bool = False
     ) -> str:
         """Output the found domains"""
         if not is_print:
             urls = {str(url.url_object.netloc) for url in found_urls}
             found_urls_str = "\n".join(urls)
-            result = f"{len(urls)} Domains:\n{found_urls_str}\n"
+            result = f"\n{len(urls)} Domains:\n{found_urls_str}\n"
             return result
         else:
             urls = {str(url.url_object.netloc) for url in found_urls}
             found_urls_str = "\n".join(urls)
-            result = f"{len(urls)} Domains:\n{found_urls_str}\n"
+            result = f"\n{len(urls)} Domains:\n{found_urls_str}\n"
             click.echo(f"{len(urls)} Domains:")
             click.echo(self.format_normal_result(f"{found_urls_str}"))
             click.echo("")
             return result
 
     def output_url_hierarchy(
         self, url_dict: dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
@@ -112,14 +117,44 @@
                     f"\n{len(url_set)} URLs from {base.url} ["
                     + self.format_colorful_status(base.response_status)
                     + f"] (depth:{base.depth}):\n{urls_str}"
                 )
 
             return url_hierarchy
 
+    def output_url_per_domain(
+        self, domains: set[str], url_dict: dict[URLNode, typing.Iterable[URLNode]], url_type: str = "URL"
+    ) -> str:
+        """Output the URLs for differenct domains"""
+        url_hierarchy = ""
+        domain_secrets: dict[str, list[URLNode]] = dict()
+        for base, urls in url_dict.items():
+            domain, _ = to_host_port(base.url_object.netloc)
+            if domain not in domains:
+                domain = "Other"
+            if domain not in domain_secrets:
+                domain_secrets[domain] = list()
+            domain_secrets[domain].extend(list(urls))
+        for domain, urls in domain_secrets.items():
+            if urls is None or len(urls) == 0:
+                continue
+            url_set = {
+                self.format_normal_result(f"{str(url.url)}")
+                + " ["
+                + self.format_colorful_status(url.response_status)
+                + "]"
+                for url in urls
+                if self.filter(url)
+            }
+            urls_str = "\n".join(url_set)
+            url_hierarchy += f"\n{len(url_set)} {url_type} from {domain}:\n{urls_str}\n"
+        click.echo(url_hierarchy)
+
+        return url_hierarchy
+
     def output_js(
         self, js_dict: dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
     ) -> str:
         """Output the url hierarchy"""
         if is_print:
             js_str = ""
             for base, urls in js_dict.items():
@@ -159,15 +194,15 @@
             return "No secrets found.\n"
         for url, secrets in url_secrets.items():
             if secrets is not None and len(list(secrets)) > 0:
                 secret_set = {
                     f"{str(secret.type)}: {str(secret.data)}" for secret in secrets
                 }
                 secrets_str = "\n".join(secret_set)
-                url_secrets_str += f"\n{len(secret_set)} Secrets found in {url.url} {str(url.response_status)}:\n{secrets_str}\n"
+                url_secrets_str += f"\n{len(secret_set)} Secrets found in {url.url} [{self.format_colorful_status(str(url.response_status))}]:\n{secrets_str}\n"
         return url_secrets_str
 
     def output_local_scan_secrets(self, path_secrets: dict[pathlib.Path, typing.Iterable[Secret]]) -> str:
         """Display all secrets found in local file"""
         if len(path_secrets) == 0:
             click.echo("No secrets found.\n")
         result = ""
```

### Comparing `secretscraper-1.3.4/src/secretscraper/scanner.py` & `secretscraper-1.3.5/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.4/src/secretscraper/urlparser.py` & `secretscraper-1.3.5/src/secretscraper/urlparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Set
 from urllib.parse import ParseResult, urlparse
 
 from bs4 import BeautifulSoup
 
 from .handler import Handler
 from .entity import URL, URLNode, Secret
-from .util import is_static_resource
+from .util import is_static_resource, sanitize_url
 
 
 class URLParser:
     """Extract URL nodes in HTML"""
 
     def __init__(self):
         pass
@@ -52,16 +52,20 @@
                     hrefs.add(href)
             except KeyError:
                 pass
 
         for href in hrefs:
             if href is not None:
                 url_obj = urlparse(href)
+
                 if is_static_resource(url_obj.path):
                     continue
+                href = sanitize_url(href)
+                if len(href) == 0:
+                    continue
                 if (
                     len(url_obj.scheme) > 0
                     and url_obj.netloc is not None
                     and len(url_obj.netloc) > 0
                 ):
                     # a full url
                     node = URLNode(
@@ -108,14 +112,17 @@
             link = link.data
             if len(link) == 0:
                 continue
             obj = urlparse(link)
             # ignore static resource
             if is_static_resource(obj.path):
                 continue
+            link = sanitize_url(link)
+            if len(link) == 0:
+                continue
             url_obj = URL(
                 scheme=base_url.url_object.scheme if obj.scheme == "" or obj.scheme not in (
                     "http", "https") else obj.scheme,
                 netloc=base_url.url_object.netloc if obj.netloc == "" else obj.netloc,
                 path=obj.path,
                 params=obj.params,
                 query=obj.query,
```

### Comparing `secretscraper-1.3.4/src/secretscraper/util.py` & `secretscraper-1.3.5/src/secretscraper/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Common utility functions."""
 
 from collections import namedtuple
+import re
+from urllib.parse import urlparse
 
 from dynaconf import LazySettings
 
 from .exception import SecretScraperException
 
 Range = namedtuple("Range", ["start", "end"])
 
@@ -29,22 +31,45 @@
             f"Exception occur when reading rules from setting: {e}"
         ) from e
     return rules_dict
 
 
 def is_static_resource(path: str) -> bool:
     """Check whether a path is a static resource"""
-    exts = ['.png', '.jpg', '.jpeg', '.gif', '.css', '.ico']
+    exts = ['.png', '.jpg', '.jpeg', '.gif', '.css', '.ico', ".dtd", '.svg']
     for ext in exts:
         if path.endswith(ext):
             return True
     return False
 
 
 def to_host_port(netloc: str) -> tuple[str, str]:
     """Convert netloc to host and port"""
     r = netloc.split(":")
     if len(r) == 1:
         return r[0], ""
     if len(r) == 2:
         return r[0].strip(), r[1].strip()
     return '', ''
+
+
+def sanitize_url(url: str) -> str:
+    """Remove invalid characters in url
+    Return emtpy string if url is invalid
+    """
+    url = url.replace(" ", "") \
+        .replace("\\/", "/") \
+        .replace("%3A", ":") \
+        .replace("%2F", "/")
+    # remove url that does not contain any word
+    m = re.search("[a-zA-Z0-9]+", url)
+    if m is None:
+        return ""
+    if url.strip().startswith("javascript"):
+        return ""
+    try:
+        obj = urlparse(url)
+        if obj.netloc.startswith("127.0.0.1") or obj.netloc.startswith("localhost"):
+            return ""
+    except:
+        pass
+    return url
```

### Comparing `secretscraper-1.3.4/PKG-INFO` & `secretscraper-1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.4
+Version: 1.3.5
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: httpx[socks] (>=0.27.0,<0.28.0)
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "darwin"
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "linux"
 Description-Content-Type: text/markdown
 
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
@@ -36,16 +36,16 @@
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
-- Platform: MaxOS or Ubuntu, no support for Windows temporarily(due to [hyperscan](https://pypi.org/project/hyperscan/) is employed in this project).
-- Python Version: 3.11
+- Platform: Test on MaxOS, Ubuntu and Windows.
+- Python Version >= 3.11
 
 ## Usage
 
 ### Install
 
 ```bash
 pip install secretscraper
@@ -225,24 +225,31 @@
 
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
-- [ ] Support url-finder output format, add `--tree` option
 - [ ] Add regex doc reference
 - [ ] Generate configuration file
+- [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.28 Version 1.3.5
+- **New Features**
+  - Support windows
+  - Optimize crawler
+  - Prettify output, add `--detail` option
+  - Generate default configuration to settings.yml
+
 ## 2024.4.28 Version 1.3.2
 - **New Features**
   - Extract links via regex
 
 ## 2024.4.26 Version 1.3.1
 - **New Features**
   - [x] Support scan local files
```

