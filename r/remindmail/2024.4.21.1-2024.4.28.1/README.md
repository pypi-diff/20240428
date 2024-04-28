# Comparing `tmp/remindmail-2024.4.21.1.tar.gz` & `tmp/remindmail-2024.4.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.21.1.tar", last modified: Sun Apr 21 20:02:04 2024, max compression
+gzip compressed data, was "remindmail-2024.4.28.1.tar", last modified: Sun Apr 28 18:43:01 2024, max compression
```

## Comparing `remindmail-2024.4.21.1.tar` & `remindmail-2024.4.28.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.21.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.292281 remindmail-2024.4.21.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.292281 remindmail-2024.4.21.1/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.21.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.21.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.21.1/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-18 05:46:42.000000 remindmail-2024.4.21.1/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-21 20:00:16.000000 remindmail-2024.4.21.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23904 2024-04-16 04:37:39.000000 remindmail-2024.4.21.1/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.21.1/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-21 20:02:04.296281 remindmail-2024.4.21.1/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-21 20:02:04.000000 remindmail-2024.4.21.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:43:01.495804 remindmail-2024.4.28.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.28.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-28 18:43:01.495804 remindmail-2024.4.28.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.28.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.28.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-28 18:43:01.495804 remindmail-2024.4.28.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:43:01.491805 remindmail-2024.4.28.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:43:01.491805 remindmail-2024.4.28.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.28.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.28.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.28.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-28 18:42:14.000000 remindmail-2024.4.28.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-28 18:42:11.000000 remindmail-2024.4.28.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23904 2024-04-16 04:37:39.000000 remindmail-2024.4.28.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.28.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:43:01.495804 remindmail-2024.4.28.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-28 18:43:01.000000 remindmail-2024.4.28.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-28 18:43:01.000000 remindmail-2024.4.28.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 18:43:01.000000 remindmail-2024.4.28.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-28 18:43:01.000000 remindmail-2024.4.28.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-28 18:43:01.000000 remindmail-2024.4.28.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.21.1/LICENSE.md` & `remindmail-2024.4.28.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/PKG-INFO` & `remindmail-2024.4.28.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.21.1
+Version: 2024.4.28.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.21.1/README.md` & `remindmail-2024.4.28.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/setup.cfg` & `remindmail-2024.4.28.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.21.1
+version = 2024.04.28.1
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.21.1/src/remind/__main__.py` & `remindmail-2024.4.28.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/src/remind/error_handler.py` & `remindmail-2024.4.28.1/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/src/remind/query_manager.py` & `remindmail-2024.4.28.1/src/remind/query_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         input_str = input_str.replace("every week", "every sunday")
 
         now = datetime.now()
         start_date = now + timedelta(days=1)
 
         # handle edge case where time between midnight and 4am
         if now.hour < 4:
-            start_date += timedelta(days=1)
+            start_date -= timedelta(days=1)
 
         key: ReminderKeyType | None = None
         value = ''
         frequency = None
         modifiers = 'd'
 
         # parse input_str
```

### Comparing `remindmail-2024.4.21.1/src/remind/reminder.py` & `remindmail-2024.4.28.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/src/remind/reminder_confirmation.py` & `remindmail-2024.4.28.1/src/remind/reminder_confirmation.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/src/remind/reminder_manager.py` & `remindmail-2024.4.28.1/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.21.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.28.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.21.1
+Version: 2024.4.28.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

