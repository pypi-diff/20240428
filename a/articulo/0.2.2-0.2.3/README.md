# Comparing `tmp/articulo-0.2.2.tar.gz` & `tmp/articulo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articulo-0.2.2.tar", max compression
+gzip compressed data, was "articulo-0.2.3.tar", max compression
```

## Comparing `articulo-0.2.2.tar` & `articulo-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    35148 2023-09-22 11:46:17.319726 articulo-0.2.2/LICENSE
--rw-r--r--   0        0        0     3582 2023-10-12 07:16:24.921623 articulo-0.2.2/README.md
--rw-r--r--   0        0        0      131 2023-09-23 11:27:12.333449 articulo-0.2.2/articulo/__init__.py
--rw-r--r--   0        0        0    11132 2024-02-17 14:39:30.170773 articulo-0.2.2/articulo/articulo.py
--rw-r--r--   0        0        0     1678 2023-10-12 07:07:07.238682 articulo-0.2.2/articulo/exceptions.py
--rw-r--r--   0        0        0      663 2024-02-17 14:41:53.692602 articulo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 articulo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-09-22 11:46:17.319726 articulo-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3582 2023-10-12 07:16:24.921623 articulo-0.2.3/README.md
+-rw-r--r--   0        0        0      131 2023-09-23 11:27:12.333449 articulo-0.2.3/articulo/__init__.py
+-rw-r--r--   0        0        0    12343 2024-04-28 18:02:49.478500 articulo-0.2.3/articulo/articulo.py
+-rw-r--r--   0        0        0      517 2024-04-28 18:03:06.651644 articulo-0.2.3/articulo/constants.py
+-rw-r--r--   0        0        0     1678 2023-10-12 07:07:07.238682 articulo-0.2.3/articulo/exceptions.py
+-rw-r--r--   0        0        0      663 2024-04-28 18:04:11.076553 articulo-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 articulo-0.2.3/PKG-INFO
```

### Comparing `articulo-0.2.2/LICENSE` & `articulo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `articulo-0.2.2/README.md` & `articulo-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `articulo-0.2.2/articulo/articulo.py` & `articulo-0.2.3/articulo/articulo.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 import re
 from functools import cached_property
 from typing import Union
 from urllib.parse import urlparse, urlunparse
 
 import validators
 import requests
-from bs4 import BeautifulSoup, NavigableString, Tag
+from bs4 import BeautifulSoup, NavigableString, Tag, Comment
 from requests import RequestException
 
+from .constants import important_content_tags, tags_to_completely_remove
 from .exceptions import (
     HTTPErrorException,
     MaxIterations,
     NoTitleException,
     NoHTMLException,
     DecodingException,
 )
@@ -153,15 +154,20 @@
 
     @cached_property
     def __content_markup(self):
         """
         Parses article HTML and returns the main article content markup using recursion.
         """
         soup = BeautifulSoup(self.__html, features="lxml")
-        return self.__look_for_best_parent(soup.body, 0)
+        raw_content = self.__look_for_best_parent(soup.body, 0)
+        if raw_content is None:
+            return raw_content
+
+        sanitized_content = self.__sanitize_content(raw_content)
+        return sanitized_content
 
     @cached_property
     def __title_element(self):
         """
         Parses article html and returns article title.
         This method assumes, that article HTML has two things:
         * title tag - as an initial title
@@ -307,14 +313,39 @@
             if isinstance(child, Tag):
                 result = self.__look_for_best_parent(child, iter_counter)
                 if result:
                     return result
 
         return None
 
+    def __sanitize_content(self, content: Tag) -> Tag:
+        """
+        Sanitizes article content from unnecessary tags.
+        """
+        self.__log("Sanitizing article content...")
+
+        # Filtering all the non-important tags.
+        for tag in content.find_all(True):  # find_all(True) will match any tag
+            if tag.decomposed:
+                continue
+            # First, we need to remove all the tags that should be completely removed
+            if tag.name in tags_to_completely_remove:
+                tag.decompose()
+            # Then, we need to unwrap all the tags that has important content
+            # but not needed by themselves
+            elif tag.name not in important_content_tags:
+                tag.unwrap()
+
+        # Removing all the comments
+        comments = content.find_all(string=lambda text: isinstance(text, Comment))
+        for comment in comments:
+            comment.extract()
+
+        return content
+
     def __get_absolute_link(self, link: str) -> str:
         """
         Makes absolute link from relative
         """
         if not validators.url(link):
             parsed_url = urlparse(self.__link)
             parsed_url = parsed_url._replace(path=link)
```

### Comparing `articulo-0.2.2/articulo/exceptions.py` & `articulo-0.2.3/articulo/exceptions.py`

 * *Files identical despite different names*

### Comparing `articulo-0.2.2/pyproject.toml` & `articulo-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "articulo"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Mikhail Ivanov <ya.ivanov-m2014v@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 lxml = "^4.9.3"
```

### Comparing `articulo-0.2.2/PKG-INFO` & `articulo-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articulo
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Mikhail Ivanov
 Author-email: ya.ivanov-m2014v@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

