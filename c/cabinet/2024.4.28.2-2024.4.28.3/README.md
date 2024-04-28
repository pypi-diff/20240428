# Comparing `tmp/cabinet-2024.4.28.2.tar.gz` & `tmp/cabinet-2024.4.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.28.2.tar", last modified: Sun Apr 28 18:04:48 2024, max compression
+gzip compressed data, was "cabinet-2024.4.28.3.tar", last modified: Sun Apr 28 18:47:53 2024, max compression
```

## Comparing `cabinet-2024.4.28.2.tar` & `cabinet-2024.4.28.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.28.2/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.28.2/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37940 2024-04-28 18:04:10.000000 cabinet-2024.4.28.2/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.28.2/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.28.2/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.4.28.2/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:04:48.580899 cabinet-2024.4.28.2/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 18:04:48.000000 cabinet-2024.4.28.2/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:47:53.545892 cabinet-2024.4.28.3/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.28.3/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:47:53.545892 cabinet-2024.4.28.3/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.28.3/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.28.3/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 18:47:53.545892 cabinet-2024.4.28.3/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:47:53.541892 cabinet-2024.4.28.3/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:47:53.545892 cabinet-2024.4.28.3/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.28.3/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.28.3/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38470 2024-04-28 18:34:24.000000 cabinet-2024.4.28.3/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.28.3/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.28.3/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.4.28.3/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 18:47:53.545892 cabinet-2024.4.28.3/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 18:47:53.000000 cabinet-2024.4.28.3/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 18:47:53.000000 cabinet-2024.4.28.3/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 18:47:53.000000 cabinet-2024.4.28.3/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 18:47:53.000000 cabinet-2024.4.28.3/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 18:47:53.000000 cabinet-2024.4.28.3/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.28.2/LICENSE` & `cabinet-2024.4.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.2/PKG-INFO` & `cabinet-2024.4.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.28.2
+Version: 2024.4.28.3
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.28.2/README.md` & `cabinet-2024.4.28.3/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.2/setup.cfg` & `cabinet-2024.4.28.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.28.2
+version = 2024.04.28.3
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.28.2/src/cabinet/cabinet.py` & `cabinet-2024.4.28.3/src/cabinet/cabinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -823,54 +823,65 @@
             return content.split('\n')
         except FileNotFoundError as error:
             if not ignore_not_found:
                 self.log(f"get_file_as_array: {error}", level="error")
             return None
 
     def write_file(self, file_name: str, path_file: str = '',
-                   content: Optional[str] = None, append: bool = False,
-                   is_quiet: bool = False) -> bool:
+                content: Optional[str] = None, append: bool = False,
+                is_quiet: bool = False) -> bool:
         """
-        writes a file to the specified path, creating necessary subfolders.
-        resolves aliases in paths.
+        Writes a file to the specified path, creating necessary subfolders.
+        Resolves aliases in paths.
 
-        args:
+        Args:
             file_name (str): the name of the file to write.
             path_file (str, optional): the directory path for the file.
-                uses default log path if empty.
-                use 'notes' for cabinet -> path -> notes
+                Uses default log path if empty.
+                Use 'notes' for cabinet -> path -> notes
             content (str, optional): the content to write to the file.
-                creates an empty file if none.
+                Creates an empty file if none.
             append (bool, optional): set to true to append to the file instead of overwriting.
-                defaults to false.
+                Defaults to false.
             is_quiet (bool, optional): set to true to suppress status messages.
-                defaults to false.
+                Defaults to false.
 
-        returns:
-            true if the file was successfully written, false otherwise.
+        Returns:
+            True if the file was successfully written, False otherwise.
         """
         try:
-            # handle default file path and notes alias
+            # Handle default file path and notes alias
             if not path_file:
                 path_file = helpers.resolve_path(self.path_log or '~/.cabinet/log')
             elif path_file == "notes":
                 path_notes: str = self.get('path', 'notes', return_type=str) or ''
                 path_file = helpers.resolve_path(path_notes or self.path_log or '~/.cabinet/notes')
 
-            # create directory if it does not exist
+            # Create directory if it does not exist
             os.makedirs(path_file, exist_ok=True)
 
-            # write content to file
+            # Full path to the file
+            full_path = os.path.join(path_file, file_name)
+
+            # Check if appending and the file exists and is not empty
+            if append and os.path.exists(full_path) and os.path.getsize(full_path) > 0:
+                with open(full_path, 'r+', encoding="utf8") as file:
+                    file.seek(0, os.SEEK_END)  # Move to the end of file
+                    file.seek(file.tell() - 1, os.SEEK_SET)  # Move back one character
+                    if file.read(1) != '\n':
+                        content = '\n' + (content or "")
+
+            # Write content to file
             mode = 'a+' if append else 'w'
-            with open(os.path.join(path_file, file_name), mode, encoding="utf8") as file:
+            with open(full_path, mode, encoding="utf8") as file:
                 file.write(content or "")
 
-            # optionally print status message
+            # Optionally print status message
             if not is_quiet:
-                print(f"wrote to '{os.path.join(path_file, file_name)}'")
+                print(f"Wrote to '{full_path}'")
 
             return True
         except (OSError, IOError) as error:
             self.log(f"write_file: {error}", level="error")
             return False
 
     def export(self):
```

### Comparing `cabinet-2024.4.28.2/src/cabinet/constants.py` & `cabinet-2024.4.28.3/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.2/src/cabinet/mail.py` & `cabinet-2024.4.28.3/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.28.2/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.28.3/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.28.2
+Version: 2024.4.28.3
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

