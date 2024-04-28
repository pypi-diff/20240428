# Comparing `tmp/zcbot-io-sdk-0.0.2.tar.gz` & `tmp/zcbot-io-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcbot-io-sdk-0.0.2.tar", last modified: Thu Apr 25 05:58:53 2024, max compression
+gzip compressed data, was "zcbot-io-sdk-0.0.3.tar", last modified: Sun Apr 28 02:34:35 2024, max compression
```

## Comparing `zcbot-io-sdk-0.0.2.tar` & `zcbot-io-sdk-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.018966 zcbot-io-sdk-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-03-15 02:17:02.000000 zcbot-io-sdk-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      363 2024-04-25 05:58:53.018966 zcbot-io-sdk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      123 2024-04-24 08:53:04.000000 zcbot-io-sdk-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-25 05:58:53.018966 zcbot-io-sdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      574 2024-04-25 05:52:21.000000 zcbot-io-sdk-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.007965 zcbot-io-sdk-0.0.2/test/
--rw-rw-rw-   0        0        0     2224 2024-04-24 09:07:11.000000 zcbot-io-sdk-0.0.2/test/test_jd.py
--rw-rw-rw-   0        0        0      936 2024-04-25 03:23:26.000000 zcbot-io-sdk-0.0.2/test/test_jslink.py
--rw-rw-rw-   0        0        0      550 2024-04-25 02:43:04.000000 zcbot-io-sdk-0.0.2/test/test_suning.py
--rw-rw-rw-   0        0        0     2511 2024-04-25 02:43:59.000000 zcbot-io-sdk-0.0.2/test/test_tmall.py
--rw-rw-rw-   0        0        0      409 2024-04-25 03:22:28.000000 zcbot-io-sdk-0.0.2/test/test_zcgov.py
--rw-rw-rw-   0        0        0      588 2024-04-25 02:49:13.000000 zcbot-io-sdk-0.0.2/test/test_zkh.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.008965 zcbot-io-sdk-0.0.2/zcbot_io_sdk/
--rw-rw-rw-   0        0        0       19 2024-04-24 07:42:37.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.015965 zcbot-io-sdk-0.0.2/zcbot_io_sdk/images/
--rw-rw-rw-   0        0        0       19 2024-04-24 07:43:02.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk/images/__init__.py
--rw-rw-rw-   0        0        0     4260 2024-04-25 05:52:21.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk/images/processor.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.017965 zcbot-io-sdk-0.0.2/zcbot_io_sdk/utils/
--rw-rw-rw-   0        0        0       19 2024-04-24 07:51:30.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     1808 2024-04-25 05:55:27.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk/utils/b64.py
-drwxrwxrwx   0        0        0        0 2024-04-25 05:58:53.012965 zcbot-io-sdk-0.0.2/zcbot_io_sdk.egg-info/
--rw-rw-rw-   0        0        0      363 2024-04-25 05:58:52.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-04-25 05:58:52.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 05:58:52.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 05:58:52.000000 zcbot-io-sdk-0.0.2/zcbot_io_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.739849 zcbot-io-sdk-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-03-15 02:17:02.000000 zcbot-io-sdk-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      363 2024-04-28 02:34:35.739849 zcbot-io-sdk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-04-24 08:53:04.000000 zcbot-io-sdk-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-28 02:34:35.739849 zcbot-io-sdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      574 2024-04-28 02:24:14.000000 zcbot-io-sdk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.729849 zcbot-io-sdk-0.0.3/test/
+-rw-rw-rw-   0        0        0     2224 2024-04-24 09:07:11.000000 zcbot-io-sdk-0.0.3/test/test_jd.py
+-rw-rw-rw-   0        0        0      936 2024-04-25 03:23:26.000000 zcbot-io-sdk-0.0.3/test/test_jslink.py
+-rw-rw-rw-   0        0        0      550 2024-04-25 02:43:04.000000 zcbot-io-sdk-0.0.3/test/test_suning.py
+-rw-rw-rw-   0        0        0     2511 2024-04-25 02:43:59.000000 zcbot-io-sdk-0.0.3/test/test_tmall.py
+-rw-rw-rw-   0        0        0      409 2024-04-25 03:22:28.000000 zcbot-io-sdk-0.0.3/test/test_zcgov.py
+-rw-rw-rw-   0        0        0      588 2024-04-25 02:49:13.000000 zcbot-io-sdk-0.0.3/test/test_zkh.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.730848 zcbot-io-sdk-0.0.3/zcbot_io_sdk/
+-rw-rw-rw-   0        0        0       19 2024-04-24 07:42:37.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.736849 zcbot-io-sdk-0.0.3/zcbot_io_sdk/images/
+-rw-rw-rw-   0        0        0       19 2024-04-24 07:43:02.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk/images/__init__.py
+-rw-rw-rw-   0        0        0     4260 2024-04-25 05:52:21.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk/images/processor.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.738849 zcbot-io-sdk-0.0.3/zcbot_io_sdk/utils/
+-rw-rw-rw-   0        0        0       19 2024-04-24 07:51:30.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     1810 2024-04-28 02:22:36.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk/utils/b64.py
+drwxrwxrwx   0        0        0        0 2024-04-28 02:34:35.734848 zcbot-io-sdk-0.0.3/zcbot_io_sdk.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-04-28 02:34:35.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-04-28 02:34:35.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 02:34:35.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 02:34:35.000000 zcbot-io-sdk-0.0.3/zcbot_io_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-io-sdk-0.0.2/setup.py` & `zcbot-io-sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-io-sdk',
-      version='0.0.2',
+      version='0.0.3',
       description='zcbot io sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=[],
       python_requires='>=3.7',
```

### Comparing `zcbot-io-sdk-0.0.2/test/test_jd.py` & `zcbot-io-sdk-0.0.3/test/test_jd.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/test/test_jslink.py` & `zcbot-io-sdk-0.0.3/test/test_jslink.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/test/test_suning.py` & `zcbot-io-sdk-0.0.3/test/test_suning.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/test/test_tmall.py` & `zcbot-io-sdk-0.0.3/test/test_tmall.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/test/test_zkh.py` & `zcbot-io-sdk-0.0.3/test/test_zkh.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/zcbot_io_sdk/images/processor.py` & `zcbot-io-sdk-0.0.3/zcbot_io_sdk/images/processor.py`

 * *Files identical despite different names*

### Comparing `zcbot-io-sdk-0.0.2/zcbot_io_sdk/utils/b64.py` & `zcbot-io-sdk-0.0.3/zcbot_io_sdk/utils/b64.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
             return 'http://' + url.strip()
         return url.strip()
     except ValueError:
         return url.strip()
 
 
 def encode_single_img(img_path: str, plat_code: str = "common") -> str:
-    base_url = f"https://io.zcbot.cn/wmc/image/{plat_code}/?src_url="
+    base_url = f"https://io.zcbot.cn/images/wmc/{plat_code}/?src_url="
     return base_url + encode(fill_link(img_path).encode())
 
 
 def encode_plat_code_img(img_list: List[str], plat_code) -> List[str]:
     if not img_list:
         return img_list
     temp = []
-    base_url = f"https://io.zcbot.cn/wmc/image/{plat_code}/?src_url="
+    base_url = f"https://io.zcbot.cn/images/wmc/{plat_code}/?src_url="
     for img in img_list:
         img_type = mime.guess_type(img)[0]
         if img_type == "image/gif":
             continue
         temp.append(base_url + encode(fill_link(img).encode()))
 
     return temp
```

