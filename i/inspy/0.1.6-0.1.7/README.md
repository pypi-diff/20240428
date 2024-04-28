# Comparing `tmp/inspy-0.1.6.tar.gz` & `tmp/inspy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inspy-0.1.6.tar", last modified: Tue Apr 16 07:01:19 2024, max compression
+gzip compressed data, was "dist\inspy-0.1.7.tar", last modified: Sun Apr 28 09:38:54 2024, max compression
```

## Comparing `inspy-0.1.6.tar` & `inspy-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/
--rw-rw-rw-   0        0        0     1086 2024-03-29 02:52:46.000000 inspy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       22 2024-03-29 10:16:21.000000 inspy-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1386 2024-04-16 07:01:19.000000 inspy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-01 06:20:14.000000 inspy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/inspy.egg-info/
--rw-rw-rw-   0        0        0     1386 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 07:01:18.000000 inspy-0.1.6/inspy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 07:01:19.000000 inspy-0.1.6/piinspy/
--rw-rw-rw-   0        0        0     2429 2024-03-29 02:56:18.000000 inspy-0.1.6/piinspy/__init__.py
--rw-rw-rw-   0        0        0     2135 2024-04-16 06:49:45.000000 inspy-0.1.6/piinspy/ins.json
--rw-rw-rw-   0        0        0    10166 2024-03-28 09:53:58.000000 inspy-0.1.6/piinspy/ins_class.py
--rw-rw-rw-   0        0        0     1159 2024-03-28 10:09:09.000000 inspy-0.1.6/piinspy/ins_function.py
--rw-rw-rw-   0        0        0      920 2024-03-29 02:36:10.000000 inspy-0.1.6/piinspy/insconst.py
--rw-rw-rw-   0        0        0      904 2024-03-29 02:57:10.000000 inspy-0.1.6/piinspy/log.py
--rw-rw-rw-   0        0        0       77 2023-11-20 02:03:46.000000 inspy-0.1.6/piinspy/package.json
--rw-rw-rw-   0        0        0       42 2024-04-16 07:01:19.000000 inspy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1493 2024-04-16 07:01:07.000000 inspy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:38:54.000000 inspy-0.1.7/
+-rw-rw-rw-   0        0        0     1086 2024-03-29 02:52:46.000000 inspy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       22 2024-03-29 10:16:21.000000 inspy-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1386 2024-04-28 09:38:54.000000 inspy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-04-01 06:20:14.000000 inspy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/
+-rw-rw-rw-   0        0        0     1386 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 09:38:54.000000 inspy-0.1.7/inspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:38:54.000000 inspy-0.1.7/piinspy/
+-rw-rw-rw-   0        0        0     2429 2024-03-29 02:56:18.000000 inspy-0.1.7/piinspy/__init__.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 06:49:45.000000 inspy-0.1.7/piinspy/ins.json
+-rw-rw-rw-   0        0        0    10252 2024-04-28 09:36:59.000000 inspy-0.1.7/piinspy/ins_class.py
+-rw-rw-rw-   0        0        0     1159 2024-03-28 10:09:09.000000 inspy-0.1.7/piinspy/ins_function.py
+-rw-rw-rw-   0        0        0      920 2024-03-29 02:36:10.000000 inspy-0.1.7/piinspy/insconst.py
+-rw-rw-rw-   0        0        0      904 2024-03-29 02:57:10.000000 inspy-0.1.7/piinspy/log.py
+-rw-rw-rw-   0        0        0       77 2023-11-20 02:03:46.000000 inspy-0.1.7/piinspy/package.json
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:38:54.000000 inspy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-04-28 09:38:33.000000 inspy-0.1.7/setup.py
```

### Comparing `inspy-0.1.6/LICENSE` & `inspy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/PKG-INFO` & `inspy-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy
-Version: 0.1.6
+Version: 0.1.7
 Summary: scan and control for instrument that support SCPI COMMAND added 34461A
 Home-page: https://github.com/AceWalTer/inspy
 Author: Yafei Wang
 Author-email: yafei.wang@pisemi.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inspy-0.1.6/README.md` & `inspy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/inspy.egg-info/PKG-INFO` & `inspy-0.1.7/inspy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy
-Version: 0.1.6
+Version: 0.1.7
 Summary: scan and control for instrument that support SCPI COMMAND added 34461A
 Home-page: https://github.com/AceWalTer/inspy
 Author: Yafei Wang
 Author-email: yafei.wang@pisemi.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inspy-0.1.6/piinspy/__init__.py` & `inspy-0.1.7/piinspy/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/piinspy/ins.json` & `inspy-0.1.7/piinspy/ins.json`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/piinspy/ins_class.py` & `inspy-0.1.7/piinspy/ins_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     @Version: 1.0 \n
     @Description : None \n
     @Create Time: 2023/12/27 13:41 \n
 """
 import time
 from functools import wraps
 from .ins_function import *
+from log import *
 
 
 class PiIns:
     """ err: means error type
             0: no error
             1: connect error
         index: means the index of the ins if there is more than one instruments of the same type
@@ -33,14 +34,16 @@
             self.ins = prm.open_resource(self.pInsID)
             self.ins.timeout = 5000
         except Exception as e:
             print(self.pInsID, self.pInsName, e)
             self.err = 1
         if self.err == 0:
             self.command = register_function(self.pInsType, self.pInsName)
+        else:
+            log_print("ERROR", "fail to register")
 
     def __str__(self):
         return self.pInsType + " " + self.pInsName + " " + self.pInsID + " " + str(self.index)
 
     def write_cmd(self, pStr):
         print(self.ins.write(pStr))
```

### Comparing `inspy-0.1.6/piinspy/ins_function.py` & `inspy-0.1.7/piinspy/ins_function.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/piinspy/insconst.py` & `inspy-0.1.7/piinspy/insconst.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/piinspy/log.py` & `inspy-0.1.7/piinspy/log.py`

 * *Files identical despite different names*

### Comparing `inspy-0.1.6/setup.py` & `inspy-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     @Description: None \n
     @Create Time: 2024/3/29 11:16 \n
 """
 from setuptools import setup, find_packages
 
 setup(
     name='inspy',  # 包名
-    version='0.1.6',  # 包的版本
+    version='0.1.7',  # 包的版本
     author='Yafei Wang',  # 作者名字
     author_email='yafei.wang@pisemi.com',  # 作者邮箱
     description='scan and control for instrument that support SCPI COMMAND added 34461A',  # 简短描述
     long_description=open('README.md').read(),  # 长描述，通常是README
     long_description_content_type='text/markdown',  # 长描述的类型，这里是markdown
     url='https://github.com/AceWalTer/inspy',  # 项目主页
     packages=find_packages(),  # 自动找到项目中的所有包
```

