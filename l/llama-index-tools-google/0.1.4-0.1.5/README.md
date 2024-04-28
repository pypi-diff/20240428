# Comparing `tmp/llama_index_tools_google-0.1.4.tar.gz` & `tmp/llama_index_tools_google-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_tools_google-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_tools_google-0.1.5.tar", max compression
```

## Comparing `llama_index_tools_google-0.1.4.tar` & `llama_index_tools_google-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       39 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/README.md
--rw-r--r--   0        0        0      351 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/__init__.py
--rw-r--r--   0        0        0     7162 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/base.py
--rw-r--r--   0        0        0        0 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/__init__.py
--rw-r--r--   0        0        0     9163 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/base.py
--rw-r--r--   0        0        0        7 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/search/__init__.py
--rw-r--r--   0        0        0     1449 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/llama_index/tools/google/search/base.py
--rw-r--r--   0        0        0     1688 2024-04-26 21:20:55.299486 llama_index_tools_google-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 llama_index_tools_google-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/README.md
+-rw-r--r--   0        0        0      351 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/calendar/__init__.py
+-rw-r--r--   0        0        0     7163 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/calendar/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/gmail/__init__.py
+-rw-r--r--   0        0        0     9163 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/gmail/base.py
+-rw-r--r--   0        0        0        7 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/search/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/llama_index/tools/google/search/base.py
+-rw-r--r--   0        0        0     1688 2024-04-28 02:57:17.014759 llama_index_tools_google-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 llama_index_tools_google-0.1.5/PKG-INFO
```

### Comparing `llama_index_tools_google-0.1.4/llama_index/tools/google/calendar/base.py` & `llama_index_tools_google-0.1.5/llama_index/tools/google/calendar/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,18 @@
             attendees Optional[List[str]]: A list of email address to invite to the event
         """
         from googleapiclient.discovery import build
 
         credentials = self._get_credentials()
         service = build("calendar", "v3", credentials=credentials)
 
-        attendees_list = []
-        for attendee in attendees:
-            attendees_list.append({"email": attendee})
+        attendees_list = (
+            [{"email": attendee} for attendee in attendees] if attendees else []
+        )
+
         start_time = (
             datetime.datetime.strptime(start_datetime, "%Y-%m-%dT%H:%M:%S%z")
             .astimezone()
             .strftime("%Y-%m-%dT%H:%M:%S.%f%z")
         )
         end_time = (
             datetime.datetime.strptime(end_datetime, "%Y-%m-%dT%H:%M:%S%z")
```

### Comparing `llama_index_tools_google-0.1.4/llama_index/tools/google/gmail/base.py` & `llama_index_tools_google-0.1.5/llama_index/tools/google/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_tools_google-0.1.4/llama_index/tools/google/search/base.py` & `llama_index_tools_google-0.1.5/llama_index/tools/google/search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_tools_google-0.1.4/pyproject.toml` & `llama_index_tools_google-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 description = "llama-index tools google integration"
 exclude = ["**/BUILD"]
 keywords = ["email", "gmail"]
 license = "MIT"
 maintainers = ["ajhofmann"]
 name = "llama-index-tools-google"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 google-api-python-client = "^2.115.0"
 google-auth-httplib2 = "^0.2.0"
 google-auth-oauthlib = "^1.2.0"
```

### Comparing `llama_index_tools_google-0.1.4/PKG-INFO` & `llama_index_tools_google-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-tools-google
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index tools google integration
 License: MIT
 Keywords: email,gmail
 Author: Your Name
 Author-email: you@example.com
 Maintainer: ajhofmann
 Requires-Python: >=3.8.1,<4.0
```

