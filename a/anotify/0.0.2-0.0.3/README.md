# Comparing `tmp/anotify-0.0.2.tar.gz` & `tmp/anotify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.0.2.tar", last modified: Fri Apr 26 13:34:26 2024, max compression
+gzip compressed data, was "anotify-0.0.3.tar", last modified: Sun Apr 28 06:23:26 2024, max compression
```

## Comparing `anotify-0.0.2.tar` & `anotify-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 13:34:26.154750 anotify-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-26 13:34:26.145988 anotify-0.0.2/ANotify/
--rw-rw-rw-   0        0        0      677 2024-04-26 11:54:00.000000 anotify-0.0.2/ANotify/Nanpush.py
--rw-rw-rw-   0        0        0     2719 2024-04-26 11:56:48.000000 anotify-0.0.2/ANotify/Nemail.py
--rw-rw-rw-   0        0        0      429 2024-04-26 11:57:17.000000 anotify-0.0.2/ANotify/Niyuu.py
--rw-rw-rw-   0        0        0     1610 2024-04-26 11:58:03.000000 anotify-0.0.2/ANotify/Npushplus.py
--rw-rw-rw-   0        0        0      814 2024-04-26 11:58:18.000000 anotify-0.0.2/ANotify/Nserverchan.py
--rw-rw-rw-   0        0        0     6307 2024-04-26 12:01:18.000000 anotify-0.0.2/ANotify/Nwecom.py
--rw-rw-rw-   0        0        0      888 2024-04-26 13:05:21.000000 anotify-0.0.2/ANotify/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-26 12:33:33.000000 anotify-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2652 2024-04-26 13:34:26.152990 anotify-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2202 2024-04-26 13:30:03.000000 anotify-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 13:34:26.152990 anotify-0.0.2/anotify.egg-info/
--rw-rw-rw-   0        0        0     2652 2024-04-26 13:34:25.000000 anotify-0.0.2/anotify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-04-26 13:34:26.000000 anotify-0.0.2/anotify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 13:34:25.000000 anotify-0.0.2/anotify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 13:34:25.000000 anotify-0.0.2/anotify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 13:34:25.000000 anotify-0.0.2/anotify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 13:34:26.154750 anotify-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-04-26 13:34:24.000000 anotify-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.057036 anotify-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.040988 anotify-0.0.3/ANotify/
+-rw-rw-rw-   0        0        0      677 2024-04-26 11:54:00.000000 anotify-0.0.3/ANotify/Nanpush.py
+-rw-rw-rw-   0        0        0     2719 2024-04-26 11:56:48.000000 anotify-0.0.3/ANotify/Nemail.py
+-rw-rw-rw-   0        0        0      429 2024-04-26 11:57:17.000000 anotify-0.0.3/ANotify/Niyuu.py
+-rw-rw-rw-   0        0        0     1610 2024-04-26 11:58:03.000000 anotify-0.0.3/ANotify/Npushplus.py
+-rw-rw-rw-   0        0        0      750 2024-04-28 06:22:25.000000 anotify-0.0.3/ANotify/Nserverchan.py
+-rw-rw-rw-   0        0        0     6307 2024-04-26 12:01:18.000000 anotify-0.0.3/ANotify/Nwecom.py
+-rw-rw-rw-   0        0        0      888 2024-04-26 13:05:21.000000 anotify-0.0.3/ANotify/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-26 12:33:33.000000 anotify-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2652 2024-04-28 06:23:26.056035 anotify-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2024-04-26 13:30:03.000000 anotify-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.055036 anotify-0.0.3/anotify.egg-info/
+-rw-rw-rw-   0        0        0     2652 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:23:26.057036 anotify-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-04-28 06:23:18.000000 anotify-0.0.3/setup.py
```

### Comparing `anotify-0.0.2/ANotify/Nanpush.py` & `anotify-0.0.3/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/ANotify/Nemail.py` & `anotify-0.0.3/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/ANotify/Npushplus.py` & `anotify-0.0.3/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/ANotify/Nserverchan.py` & `anotify-0.0.3/ANotify/Nserverchan.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         """
 
         data = {
             "text": msg_title,
             "desp": msg_text,
         }
 
-        request_url = f"{self.base_url}?title={msg_title}&desp={msg_text}"
-
-        response = requests.get(request_url)
+        response = requests.post(self.base_url, data=data)
         response.raise_for_status()
         return response.json()
 
 if __name__ == "__main__":
     TOKEN = ''
     print(ServerChanNotify(TOKEN).send_msg("测试标题", "测试正文"))
```

### Comparing `anotify-0.0.2/ANotify/Nwecom.py` & `anotify-0.0.3/ANotify/Nwecom.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/ANotify/__init__.py` & `anotify-0.0.3/ANotify/__init__.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/LICENSE` & `anotify-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/PKG-INFO` & `anotify-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.2 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.3 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.25.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
```

### Comparing `anotify-0.0.2/README.md` & `anotify-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `anotify-0.0.2/anotify.egg-info/PKG-INFO` & `anotify-0.0.3/anotify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.2 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.3 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.25.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
```

### Comparing `anotify-0.0.2/setup.py` & `anotify-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         'requests>=2.25.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
     description='Send notifications by multiple channels.',
```

