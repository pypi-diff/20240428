# Comparing `tmp/numimage-0.0.1.tar.gz` & `tmp/numimage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numimage-0.0.1.tar", last modified: Sun Apr 28 06:38:11 2024, max compression
+gzip compressed data, was "numimage-0.0.2.tar", last modified: Sun Apr 28 06:48:37 2024, max compression
```

## Comparing `numimage-0.0.1.tar` & `numimage-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:38:11.412504 numimage-0.0.1/
--rw-rw-rw-   0        0        0     1073 2020-03-05 23:01:44.000000 numimage-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2940 2024-04-28 06:38:11.412504 numimage-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2024-04-28 06:37:33.000000 numimage-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 06:38:11.405527 numimage-0.0.1/numimage/
--rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.1/numimage/__init__.py
--rw-rw-rw-   0        0        0     5546 2024-04-28 06:31:49.000000 numimage-0.0.1/numimage/geometry.py
--rw-rw-rw-   0        0        0      142 2024-04-26 09:14:23.000000 numimage-0.0.1/numimage/math_h.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:38:11.411507 numimage-0.0.1/numimage.egg-info/
--rw-rw-rw-   0        0        0     2940 2024-04-28 06:38:11.000000 numimage-0.0.1/numimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-28 06:38:11.000000 numimage-0.0.1/numimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:38:11.000000 numimage-0.0.1/numimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 06:38:11.000000 numimage-0.0.1/numimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 06:38:11.000000 numimage-0.0.1/numimage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:38:11.413501 numimage-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2024 2024-04-28 06:37:02.000000 numimage-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:38:11.411507 numimage-0.0.1/string_h/
--rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.1/string_h/__init__.py
--rw-rw-rw-   0        0        0       48 2020-03-05 23:01:44.000000 numimage-0.0.1/string_h/reverse.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:48:37.858426 numimage-0.0.2/
+-rw-rw-rw-   0        0        0     1073 2020-03-05 23:01:44.000000 numimage-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3022 2024-04-28 06:48:37.858426 numimage-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2024-04-28 06:37:33.000000 numimage-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 06:48:37.846466 numimage-0.0.2/numimage/
+-rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.2/numimage/__init__.py
+-rw-rw-rw-   0        0        0     5546 2024-04-28 06:31:49.000000 numimage-0.0.2/numimage/geometry.py
+-rw-rw-rw-   0        0        0      142 2024-04-26 09:14:23.000000 numimage-0.0.2/numimage/math_h.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:48:37.857429 numimage-0.0.2/numimage.egg-info/
+-rw-rw-rw-   0        0        0     3022 2024-04-28 06:48:37.000000 numimage-0.0.2/numimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-28 06:48:37.000000 numimage-0.0.2/numimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:48:37.000000 numimage-0.0.2/numimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-28 06:48:37.000000 numimage-0.0.2/numimage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 06:48:37.000000 numimage-0.0.2/numimage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:48:37.858426 numimage-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2064 2024-04-28 06:48:32.000000 numimage-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:48:37.857429 numimage-0.0.2/string_h/
+-rw-rw-rw-   0        0        0        0 2020-03-05 23:01:44.000000 numimage-0.0.2/string_h/__init__.py
+-rw-rw-rw-   0        0        0       48 2020-03-05 23:01:44.000000 numimage-0.0.2/string_h/reverse.py
```

### Comparing `numimage-0.0.1/LICENSE.txt` & `numimage-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numimage-0.0.1/PKG-INFO` & `numimage-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numimage
-Version: 0.0.1
+Version: 0.0.2
 Summary: 验证打包功能的测试包, 请勿下载
 Home-page: https://github.com/JackyFuHk/numimage
 Author: JackyFu
 Author-email: 343651570@qq.com
 License: MIT
 Keywords: jacky package demo
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,17 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pytest
+Requires-Dist: torch==2.0.1
+Requires-Dist: torchvision
+Requires-Dist: svg.path
 
 # 韩灵稚打包测试
 Hanlingzhi's Package PyPi Demo
 ##工程结构说明
 <pre>
 .
 ├── LICENSE.txt    	// 证书文件
```

### Comparing `numimage-0.0.1/README.md` & `numimage-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `numimage-0.0.1/numimage/geometry.py` & `numimage-0.0.2/numimage/geometry.py`

 * *Files identical despite different names*

### Comparing `numimage-0.0.1/numimage.egg-info/PKG-INFO` & `numimage-0.0.2/numimage.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numimage
-Version: 0.0.1
+Version: 0.0.2
 Summary: 验证打包功能的测试包, 请勿下载
 Home-page: https://github.com/JackyFuHk/numimage
 Author: JackyFu
 Author-email: 343651570@qq.com
 License: MIT
 Keywords: jacky package demo
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,17 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pytest
+Requires-Dist: torch==2.0.1
+Requires-Dist: torchvision
+Requires-Dist: svg.path
 
 # 韩灵稚打包测试
 Hanlingzhi's Package PyPi Demo
 ##工程结构说明
 <pre>
 .
 ├── LICENSE.txt    	// 证书文件
```

### Comparing `numimage-0.0.1/setup.py` & `numimage-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包名
     name="numimage",
     # 版本(也可以用日期表示 2020.3.1 这样每次提交不需要在改版本)
-    version="0.0.1",
+    version="0.0.2",
     # 作者
     author="JackyFu",
     # 作者邮箱
     author_email="343651570@qq.com",
     # 包的说明(这个要正规,会展示出来, 列表页灰色横幅可见)
     description="验证打包功能的测试包, 请勿下载",
     # 项目描述
@@ -50,11 +50,11 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         "Operating System :: OS Independent",
     ],
     # 包依赖
-    install_requires=['pytest'],
+    install_requires=['pytest','torch==2.0.1','torchvision','svg.path'],
     # python版本依赖
     python_requires='>=3.6',
 )
```

