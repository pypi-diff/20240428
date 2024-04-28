# Comparing `tmp/wcommon-1.6.0.tar.gz` & `tmp/wcommon-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.6.0.tar", last modified: Tue Jan  2 07:50:10 2024, max compression
+gzip compressed data, was "wcommon-1.6.1.tar", last modified: Sun Apr 28 09:52:12 2024, max compression
```

## Comparing `wcommon-1.6.0.tar` & `wcommon-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-01-02 07:50:10.607187 wcommon-1.6.0/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2024-01-02 07:50:10.606891 wcommon-1.6.0/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.6.0/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2024-01-02 07:50:10.607364 wcommon-1.6.0/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2024-01-02 06:28:49.000000 wcommon-1.6.0/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-01-02 07:50:10.603489 wcommon-1.6.0/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    30696 2024-01-02 07:49:23.000000 wcommon-1.6.0/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-01-02 07:50:10.606354 wcommon-1.6.0/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2024-01-02 07:50:10.000000 wcommon-1.6.0/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2024-01-02 07:50:10.000000 wcommon-1.6.0/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2024-01-02 07:50:10.000000 wcommon-1.6.0/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2024-01-02 07:50:10.000000 wcommon-1.6.0/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2024-01-02 07:50:10.000000 wcommon-1.6.0/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.283061 wcommon-1.6.1/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1776 2024-04-28 09:52:12.281528 wcommon-1.6.1/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1382 2024-04-28 09:51:36.000000 wcommon-1.6.1/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2024-04-28 09:52:12.283478 wcommon-1.6.1/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2024-01-26 07:38:05.000000 wcommon-1.6.1/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.268898 wcommon-1.6.1/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    31043 2024-01-26 07:37:04.000000 wcommon-1.6.1/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.279104 wcommon-1.6.1/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1776 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.6.0/PKG-INFO` & `wcommon-1.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.6.0
+Version: 1.6.1
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # This is my common Python tool classes.
+# Main page is https://pypi.org/project/wcommon/ .
 
 
 ### /data/apps/public/conf.ini content like:
 ```
 [mysql]
 host=example.com
 port=3306
```

### Comparing `wcommon-1.6.0/README.md` & `wcommon-1.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This is my common Python tool classes.
+# Main page is https://pypi.org/project/wcommon/ .
 
 
 ### /data/apps/public/conf.ini content like:
 ```
 [mysql]
 host=example.com
 port=3306
```

### Comparing `wcommon-1.6.0/setup.py` & `wcommon-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.6.0",
+    version="1.6.1",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.6.0/wcommon/__init__.py` & `wcommon-1.6.1/wcommon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -924,7 +924,16 @@
         """
         return self.post(action, data)
 
     def post(self, action, data=None):
         data1 = self._transfer_data(data)
         return requests.post(url="{}{}".format(self.urlPrefix, action), auth=(self.username, self.password),
                              headers=self.headers, data=data1)
+
+    def update(self,index_name,doc_id,data):
+        """
+        :param index_name : 索引的名称
+        :param doc_id : 文档的id
+        :param data: 格式为{'id': '332214', 'price': '10', 'sort': '5', 'is_use': '3'}
+        :return:
+        """
+        return self.post("/{}/_update/{}".format(index_name, doc_id), data={"doc": data})
```

### Comparing `wcommon-1.6.0/wcommon.egg-info/PKG-INFO` & `wcommon-1.6.1/wcommon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.6.0
+Version: 1.6.1
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # This is my common Python tool classes.
+# Main page is https://pypi.org/project/wcommon/ .
 
 
 ### /data/apps/public/conf.ini content like:
 ```
 [mysql]
 host=example.com
 port=3306
```

