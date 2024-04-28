# Comparing `tmp/cabinet-2024.4.25.1.tar.gz` & `tmp/cabinet-2024.4.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.25.1.tar", last modified: Fri Apr 26 06:21:58 2024, max compression
+gzip compressed data, was "cabinet-2024.4.27.1.tar", last modified: Sun Apr 28 04:01:40 2024, max compression
```

## Comparing `cabinet-2024.4.25.1.tar` & `cabinet-2024.4.27.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.25.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.671914 cabinet-2024.4.25.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37937 2024-04-26 06:03:05.000000 cabinet-2024.4.25.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.25.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-26 04:02:59.000000 cabinet-2024.4.25.1/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4894 2024-04-16 03:19:05.000000 cabinet-2024.4.25.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.27.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37996 2024-04-28 04:00:13.000000 cabinet-2024.4.27.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.27.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-26 04:02:59.000000 cabinet-2024.4.27.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4894 2024-04-16 03:19:05.000000 cabinet-2024.4.27.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.25.1/LICENSE` & `cabinet-2024.4.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.25.1/PKG-INFO` & `cabinet-2024.4.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.25.1
+Version: 2024.4.27.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.25.1/README.md` & `cabinet-2024.4.27.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.25.1/setup.cfg` & `cabinet-2024.4.27.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.25.1
+version = 2024.04.27.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.25.1/src/cabinet/cabinet.py` & `cabinet-2024.4.27.1/src/cabinet/cabinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=too-many-lines
+
 """
 Cabinet provides a simple interface for storing and retrieving data in a centralized location.
 
 It includes a variety of utility methods for managing files, logging, and managing configurations.
 
 Usage:
     ```
@@ -271,15 +273,16 @@
             sys.exit(-1)
         except pymongo.errors.ConfigurationError as error:
             print(ERROR_MONGODB_DNS)
             print(error)
             sys.exit(-1)
 
 
-        path_log = helpers.resolve_path(self.get('path', 'log', returnType=str) or '~/.cabinet/log')
+        path_log = helpers.resolve_path(self.get('path', 'log', return_type=str) \
+            or '~/.cabinet/log')
         path_log_slash = os.path.join(path_log, '')
 
         # Create the directory if it doesn't exist
         if not os.path.exists(path_log_slash):
             os.makedirs(path_log_slash)
 
         self.path_log = path_log_slash
@@ -563,32 +566,32 @@
         if is_print:
             print(f"Modified {result.modified_count} item(s)")
             print(
                 f"{' -> '.join(attribute[:-1])} set to {value}\n")
 
         return value
 
-    T = TypeVar('T', bound=Any)  # Generic type variable for returnType
+    T = TypeVar('T', bound=Any)  # Generic type variable for return_type
     def get(self, *attributes, warn_missing: bool = False, is_print: bool = False,
-            no_cache: bool = False, returnType: Optional[Type[T]] = None) -> Optional[T]:
+            no_cache: bool = False, return_type: Optional[Type[T]] = None) -> Optional[T]:
         """
             Returns a property or properties from MongoDB based on the input attributes,
             using a cache file to improve performance.
 
             Args:
                 *attributes (str): A sequence of strings representing nested attributes.
                 warn_missing (bool, optional): Whether to warn if an attribute is missing.
                 is_print (bool, optional): Whether to print the return value.
                 no_cache (bool, optional): Whether to force a fresh MongoDB call.
-                returnType (Type[T], optional): The expected return type of the result.
+                return_type (Type[T], optional): The expected return type of the result.
                     Defaults to object, which includes any type.
 
             Returns:
                 The value of the attribute if it exists in the cache or MongoDB,
-                cast to returnType, otherwise None.
+                cast to return_type, otherwise None.
 
             Usage:
                 get('person', 'tyler', 'salary')  # Returns the value of person -> tyler -> salary
             """
 
         path_cache_file = f"{self.path_config_dir}/cache.json"
         cache_update_needed = no_cache
@@ -639,23 +642,23 @@
 
             if is_print:
                 print(result)
 
             if is_print:
                 print(result)
 
-            # Handle returnType if specified
-            if returnType is not None:
+            # Handle return_type if specified
+            if return_type is not None:
                 try:
-                    return returnType(result)
+                    return return_type(result)
                 except (ValueError, TypeError) as e:
-                    self.log(f"Error casting result to {returnType}: {str(e)}", level="error")
+                    self.log(f"Error casting result to {return_type}: {str(e)}", level="error")
                     return None
             else:
-                return result  # Return as is if no specific returnType is needed
+                return result  # Return as is if no specific return_type is needed
 
         if warn_missing:
             self.log("No document found in cache or MongoDB", level="warn")
         return None
 
     def remove(self, *attribute, is_print: bool = False):
         """
@@ -849,15 +852,15 @@
             true if the file was successfully written, false otherwise.
         """
         try:
             # handle default file path and notes alias
             if not path_file:
                 path_file = helpers.resolve_path(self.path_log or '~/.cabinet/log')
             elif path_file == "notes":
-                path_notes: str = self.get('path', 'notes', returnType=str) or ''
+                path_notes: str = self.get('path', 'notes', return_type=str) or ''
                 path_file = helpers.resolve_path(path_notes or self.path_log or '~/.cabinet/notes')
 
             # create directory if it does not exist
             os.makedirs(path_file, exist_ok=True)
 
             # write content to file
             mode = 'a+' if append else 'w'
```

### Comparing `cabinet-2024.4.25.1/src/cabinet/constants.py` & `cabinet-2024.4.27.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.25.1/src/cabinet/mail.py` & `cabinet-2024.4.27.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.25.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.27.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.25.1
+Version: 2024.4.27.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

