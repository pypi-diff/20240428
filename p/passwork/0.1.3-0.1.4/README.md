# Comparing `tmp/passwork-0.1.3.tar.gz` & `tmp/passwork-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwork-0.1.3.tar", last modified: Sat Apr 27 14:05:13 2024, max compression
+gzip compressed data, was "passwork-0.1.4.tar", last modified: Sun Apr 28 14:42:29 2024, max compression
```

## Comparing `passwork-0.1.3.tar` & `passwork-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734683 passwork-0.1.3/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1065 2024-04-23 15:05:31.000000 passwork-0.1.3/LICENSE
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-27 14:05:13.734626 passwork-0.1.3/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     5814 2024-04-23 15:05:31.000000 passwork-0.1.3/README.md
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.730125 passwork-0.1.3/passwork/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       42 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/main.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.732142 passwork-0.1.3/passwork/password_crud/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      168 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2908 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/add_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      799 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/delete_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2121 2024-04-27 14:02:55.000000 passwork-0.1.3/passwork/password_crud/get_inbox_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2248 2024-04-27 12:13:16.000000 passwork-0.1.3/passwork/password_crud/get_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1658 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/password_crud/search_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     8159 2024-04-27 13:34:55.000000 passwork-0.1.3/passwork/passwork_api.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.732944 passwork-0.1.3/passwork/rest_modules/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1056 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/rest_modules/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4646 2024-04-27 12:34:52.000000 passwork-0.1.3/passwork/rest_modules/passwords.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1808 2024-04-27 13:02:05.000000 passwork-0.1.3/passwork/rest_modules/users.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      431 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/rest_modules/vaults.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1362 2024-04-27 13:22:16.000000 passwork-0.1.3/passwork/session_options.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734119 passwork-0.1.3/passwork/utils/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      116 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3954 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/base32.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3200 2024-04-23 15:05:31.000000 passwork-0.1.3/passwork/utils/crypto_file.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4679 2024-04-27 13:36:30.000000 passwork-0.1.3/passwork/utils/crypto_interface.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3552 2024-04-27 12:57:05.000000 passwork-0.1.3/passwork/utils/passwork_utils.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-27 14:05:13.734374 passwork-0.1.3/passwork.egg-info/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      810 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/SOURCES.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        1 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/dependency_links.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       52 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/requires.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        9 2024-04-27 14:05:13.000000 passwork-0.1.3/passwork.egg-info/top_level.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       38 2024-04-27 14:05:13.734910 passwork-0.1.3/setup.cfg
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      638 2024-04-27 14:05:07.000000 passwork-0.1.3/setup.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700727 passwork-0.1.4/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1065 2024-04-23 15:05:31.000000 passwork-0.1.4/LICENSE
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-28 14:42:29.700672 passwork-0.1.4/PKG-INFO
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     5814 2024-04-23 15:05:31.000000 passwork-0.1.4/README.md
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.696071 passwork-0.1.4/passwork/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       42 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/main.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.697903 passwork-0.1.4/passwork/password_crud/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      219 2024-04-28 14:39:47.000000 passwork-0.1.4/passwork/password_crud/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2908 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/add_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      799 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/delete_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2121 2024-04-27 14:02:55.000000 passwork-0.1.4/passwork/password_crud/get_inbox_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2248 2024-04-27 12:13:16.000000 passwork-0.1.4/passwork/password_crud/get_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1658 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/search_password.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     8159 2024-04-27 13:34:55.000000 passwork-0.1.4/passwork/passwork_api.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.698899 passwork-0.1.4/passwork/rest_modules/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1056 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/rest_modules/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4646 2024-04-27 12:34:52.000000 passwork-0.1.4/passwork/rest_modules/passwords.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1808 2024-04-27 13:02:05.000000 passwork-0.1.4/passwork/rest_modules/users.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      431 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/rest_modules/vaults.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1362 2024-04-27 13:22:16.000000 passwork-0.1.4/passwork/session_options.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700179 passwork-0.1.4/passwork/utils/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      116 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/__init__.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3954 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/base32.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3200 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/crypto_file.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4679 2024-04-27 13:36:30.000000 passwork-0.1.4/passwork/utils/crypto_interface.py
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3552 2024-04-27 12:57:05.000000 passwork-0.1.4/passwork/utils/passwork_utils.py
+drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700456 passwork-0.1.4/passwork.egg-info/
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/PKG-INFO
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      810 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/SOURCES.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        1 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/dependency_links.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       52 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/requires.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        9 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/top_level.txt
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       38 2024-04-28 14:42:29.700941 passwork-0.1.4/setup.cfg
+-rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      638 2024-04-28 14:39:47.000000 passwork-0.1.4/setup.py
```

### Comparing `passwork-0.1.3/LICENSE` & `passwork-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/PKG-INFO` & `passwork-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwork
-Version: 0.1.3
+Version: 0.1.4
 Summary: Passwork connector
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `passwork-0.1.3/README.md` & `passwork-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/password_crud/add_password.py` & `passwork-0.1.4/passwork/password_crud/add_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/password_crud/delete_password.py` & `passwork-0.1.4/passwork/password_crud/delete_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/password_crud/get_inbox_password.py` & `passwork-0.1.4/passwork/password_crud/get_inbox_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/password_crud/get_password.py` & `passwork-0.1.4/passwork/password_crud/get_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/password_crud/search_password.py` & `passwork-0.1.4/passwork/password_crud/search_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/passwork_api.py` & `passwork-0.1.4/passwork/passwork_api.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/rest_modules/__init__.py` & `passwork-0.1.4/passwork/rest_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/rest_modules/passwords.py` & `passwork-0.1.4/passwork/rest_modules/passwords.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/rest_modules/users.py` & `passwork-0.1.4/passwork/rest_modules/users.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/session_options.py` & `passwork-0.1.4/passwork/session_options.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/utils/base32.py` & `passwork-0.1.4/passwork/utils/base32.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/utils/crypto_file.py` & `passwork-0.1.4/passwork/utils/crypto_file.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/utils/crypto_interface.py` & `passwork-0.1.4/passwork/utils/crypto_interface.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork/utils/passwork_utils.py` & `passwork-0.1.4/passwork/utils/passwork_utils.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/passwork.egg-info/PKG-INFO` & `passwork-0.1.4/passwork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passwork
-Version: 0.1.3
+Version: 0.1.4
 Summary: Passwork connector
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `passwork-0.1.3/passwork.egg-info/SOURCES.txt` & `passwork-0.1.4/passwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `passwork-0.1.3/setup.py` & `passwork-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='passwork',
-    version='0.1.3',
+    version='0.1.4',
     description='Passwork connector',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'requests>=2.31.0',
         'cryptography>=42.0.5',
```

