# Comparing `tmp/cabinet-2024.4.27.1.tar.gz` & `tmp/cabinet-2024.4.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.27.1.tar", last modified: Sun Apr 28 04:01:40 2024, max compression
+gzip compressed data, was "cabinet-2024.4.28.1.tar", last modified: Sun Apr 28 07:01:43 2024, max compression
```

## Comparing `cabinet-2024.4.27.1.tar` & `cabinet-2024.4.28.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.27.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.27.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37996 2024-04-28 04:00:13.000000 cabinet-2024.4.27.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.27.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-26 04:02:59.000000 cabinet-2024.4.27.1/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4894 2024-04-16 03:19:05.000000 cabinet-2024.4.27.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 04:01:40.425106 cabinet-2024.4.27.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 04:01:40.000000 cabinet-2024.4.27.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.28.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.28.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37996 2024-04-28 06:57:49.000000 cabinet-2024.4.28.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.28.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.28.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 07:01:09.000000 cabinet-2024.4.28.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 07:01:43.110950 cabinet-2024.4.28.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-28 07:01:43.000000 cabinet-2024.4.28.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.27.1/LICENSE` & `cabinet-2024.4.28.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.27.1/PKG-INFO` & `cabinet-2024.4.28.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.27.1
+Version: 2024.4.28.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.27.1/README.md` & `cabinet-2024.4.28.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.27.1/setup.cfg` & `cabinet-2024.4.28.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.27.1
+version = 2024.04.28.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.27.1/src/cabinet/cabinet.py` & `cabinet-2024.4.28.1/src/cabinet/cabinet.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.27.1/src/cabinet/constants.py` & `cabinet-2024.4.28.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.27.1/src/cabinet/mail.py` & `cabinet-2024.4.28.1/src/cabinet/mail.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 """
 
 import smtplib
 from urllib.parse import unquote
 import sys
 import pwd
 import os
+import subprocess
+import shlex
+from typing import List
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 import cabinet
 
 class Mail:
     """
     Provides functionality for sending email using SMTP and MIMEText.
@@ -134,11 +137,47 @@
                     is_quiet=is_quiet)
 
         except smtplib.SMTPAuthenticationError as err:
             self.cab.log(
                 f"Could not log into {self.username}; set this with Cabinet.\n\n{err}",
                 level="error")
 
+    def send_in_background(self, subject: str, body: str, to_addr: str = '') -> None:
+        """
+        Sends an email in the background to allow scripts to complete without waiting.
+
+        Args:
+            subject (str): The subject line of the email.
+            body (str): The main content of the email.
+            to_addr (str, optional): The recipient's email address.
+                If not provided, defaults to the first address in the cabinet -> email -> to
+
+        Returns:
+            None
+        """
+        # Fetch default to_addr if not provided
+        if not to_addr:
+            cab_to: List[str] = self.cab.get("email", "to", return_type=list) or []
+            to_addr = cab_to[0] if cab_to else ''
+            if not to_addr:
+                self.cab.log("No email address to send_in_background", level="error")
+                return  # Exit if there is no address to send to
+
+        # Sanitize and prepare arguments to avoid shell injection and handle internal single quotes
+        subject = shlex.quote(subject)
+        body = shlex.quote(body)
+        to_addr = shlex.quote(to_addr)
+
+        # Prepare the command string with proper quoting
+        command = f"cabinet --mail -s {subject} -b {body}"
+        if to_addr:
+            command += f" --to {to_addr}"
+
+        # Schedule the command to run immediately using 'at'
+        schedule_command = f'echo {command} | at now'
+        subprocess.Popen(schedule_command, shell=True,
+                        stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
 
 if __name__ == "__main__":
     if len(sys.argv) == 1:
         print("Usage: cabinet --mail -s <subject> -b <body> --to <to, optional>")
```

### Comparing `cabinet-2024.4.27.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.28.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.27.1
+Version: 2024.4.28.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

