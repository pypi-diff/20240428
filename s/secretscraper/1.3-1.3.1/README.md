# Comparing `tmp/secretscraper-1.3.tar.gz` & `tmp/secretscraper-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.tar", max compression
+gzip compressed data, was "secretscraper-1.3.1.tar", max compression
```

## Comparing `secretscraper-1.3.tar` & `secretscraper-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3/LICENSE
--rw-r--r--   0        0        0     6489 2024-04-26 08:06:31.965119 secretscraper-1.3/README.md
--rw-r--r--   0        0        0     1436 2024-04-26 08:18:01.049146 secretscraper-1.3/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-26 08:18:01.043859 secretscraper-1.3/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-26 07:57:48.575721 secretscraper-1.3/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-16 11:30:07.208957 secretscraper-1.3/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3/src/secretscraper/exception.py
--rw-r--r--   0        0        0    11771 2024-04-26 08:03:45.874327 secretscraper-1.3/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2093 2024-04-15 07:08:56.960583 secretscraper-1.3/src/secretscraper/filter.py
--rw-r--r--   0        0        0     4817 2024-04-15 07:08:56.998319 secretscraper-1.3/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3/src/secretscraper/log.py
--rw-r--r--   0        0        0     6802 2024-04-26 08:02:37.301072 secretscraper-1.3/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     2645 2024-04-15 07:08:56.999973 secretscraper-1.3/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0      873 2024-04-16 10:31:30.742064 secretscraper-1.3/src/secretscraper/util.py
--rw-r--r--   0        0        0     7461 1970-01-01 00:00:00.000000 secretscraper-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6737 2024-04-28 02:57:57.773811 secretscraper-1.3.1/README.md
+-rw-r--r--   0        0        0     1438 2024-04-28 02:57:57.779725 secretscraper-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-28 02:57:57.783810 secretscraper-1.3.1/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-26 07:57:48.575721 secretscraper-1.3.1/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.1/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-16 11:30:07.208957 secretscraper-1.3.1/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.1/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    12962 2024-04-16 12:29:17.184270 secretscraper-1.3.1/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.1/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.1/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    11777 2024-04-28 02:53:58.636401 secretscraper-1.3.1/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2093 2024-04-15 07:08:56.960583 secretscraper-1.3.1/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     4817 2024-04-15 07:08:56.998319 secretscraper-1.3.1/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.1/src/secretscraper/log.py
+-rw-r--r--   0        0        0     6802 2024-04-26 08:02:37.301072 secretscraper-1.3.1/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.1/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     2645 2024-04-15 07:08:56.999973 secretscraper-1.3.1/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0      873 2024-04-16 10:31:30.742064 secretscraper-1.3.1/src/secretscraper/util.py
+-rw-r--r--   0        0        0     7711 1970-01-01 00:00:00.000000 secretscraper-1.3.1/PKG-INFO
```

### Comparing `secretscraper-1.3/LICENSE` & `secretscraper-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/README.md` & `secretscraper-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -205,8 +205,21 @@
 
 ---
 
 # TODO
 - [x] Scan local file
 - [ ] Support windows
 - [ ] Support headless browser
-- [ ] Extract links additionally via regex
+- [ ] Extract links via regex
+- [ ] Support url-finder output format, add `--tree` option
+- [ ] Add regex doc reference
+
+---
+
+# Change Log
+## 2024.4.26 Version 1.3
+- **New Features**
+  - [x] Support scan local files
+
+## 2024.4.15
+- [x] Add status to url result
+- [x] All crawler test passed
```

### Comparing `secretscraper-1.3/pyproject.toml` & `secretscraper-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3"
+version = "1.3.1"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3/src/secretscraper/cmdline.py` & `secretscraper-1.3.1/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/config/__init__.py` & `secretscraper-1.3.1/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/config/settings.yml` & `secretscraper-1.3.1/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/coroutinue.py` & `secretscraper-1.3.1/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/crawler.py` & `secretscraper-1.3.1/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/entity.py` & `secretscraper-1.3.1/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/exception.py` & `secretscraper-1.3.1/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/facade.py` & `secretscraper-1.3.1/src/secretscraper/facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,18 +91,18 @@
 
                 # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
                 self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
 
                 self.formatter.output_found_domains(list(self.crawler.found_urls), True)
 
                 if not self.hide_regex:
-                    print_func_colorful(self.print_func,
+                    print_func_colorful(f, self.print_func,
                                         f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
                                         )
-                print_func_colorful(self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
+                print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
             except KeyboardInterrupt:
                 self.print_func("\nExiting...")
                 self.crawler.close_all()
             except Exception as e:
                 self.print_func(f"Unexpected error: {e}.\nExiting...")
                 self.crawler.close_all()
                 # raise FacadeException from e
```

### Comparing `secretscraper-1.3/src/secretscraper/filter.py` & `secretscraper-1.3.1/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/handler.py` & `secretscraper-1.3.1/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/log.py` & `secretscraper-1.3.1/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/output_formatter.py` & `secretscraper-1.3.1/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/scanner.py` & `secretscraper-1.3.1/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/urlparser.py` & `secretscraper-1.3.1/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/src/secretscraper/util.py` & `secretscraper-1.3.1/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3/PKG-INFO` & `secretscraper-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3
+Version: 1.3.1
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -229,9 +229,22 @@
 
 ---
 
 # TODO
 - [x] Scan local file
 - [ ] Support windows
 - [ ] Support headless browser
-- [ ] Extract links additionally via regex
+- [ ] Extract links via regex
+- [ ] Support url-finder output format, add `--tree` option
+- [ ] Add regex doc reference
+
+---
+
+# Change Log
+## 2024.4.26 Version 1.3
+- **New Features**
+  - [x] Support scan local files
+
+## 2024.4.15
+- [x] Add status to url result
+- [x] All crawler test passed
```

