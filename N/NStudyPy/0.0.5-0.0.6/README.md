# Comparing `tmp/nstudypy-0.0.5.tar.gz` & `tmp/nstudypy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstudypy-0.0.5.tar", last modified: Fri Apr 26 04:52:28 2024, max compression
+gzip compressed data, was "nstudypy-0.0.6.tar", last modified: Sun Apr 28 06:58:34 2024, max compression
```

## Comparing `nstudypy-0.0.5.tar` & `nstudypy-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:52:28.748260 nstudypy-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 04:52:19.000000 nstudypy-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-26 04:52:28.748260 nstudypy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 04:52:19.000000 nstudypy-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 04:52:19.000000 nstudypy-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 04:52:19.000000 nstudypy-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:52:28.748260 nstudypy-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:52:28.744260 nstudypy-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:52:28.748260 nstudypy-0.0.5/src/NStudyPy/
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/PyDate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/PyPDF.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/PyShape.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/PyString.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/PyTools.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 04:52:19.000000 nstudypy-0.0.5/src/NStudyPy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:52:28.748260 nstudypy-0.0.5/src/NStudyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-26 04:52:28.000000 nstudypy-0.0.5/src/NStudyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-26 04:52:28.000000 nstudypy-0.0.5/src/NStudyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:52:28.000000 nstudypy-0.0.5/src/NStudyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 04:52:28.000000 nstudypy-0.0.5/src/NStudyPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 04:52:28.000000 nstudypy-0.0.5/src/NStudyPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:34.494128 nstudypy-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 06:58:23.000000 nstudypy-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-28 06:58:34.494128 nstudypy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-28 06:58:23.000000 nstudypy-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-28 06:58:23.000000 nstudypy-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 06:58:23.000000 nstudypy-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 06:58:34.494128 nstudypy-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:34.490128 nstudypy-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:34.490128 nstudypy-0.0.6/src/NStudyPy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyPDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyShape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/PyWeb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-28 06:58:23.000000 nstudypy-0.0.6/src/NStudyPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:58:34.494128 nstudypy-0.0.6/src/NStudyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-28 06:58:34.000000 nstudypy-0.0.6/src/NStudyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 06:58:34.000000 nstudypy-0.0.6/src/NStudyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:58:34.000000 nstudypy-0.0.6/src/NStudyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-28 06:58:34.000000 nstudypy-0.0.6/src/NStudyPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 06:58:34.000000 nstudypy-0.0.6/src/NStudyPy.egg-info/top_level.txt
```

### Comparing `nstudypy-0.0.5/LICENSE` & `nstudypy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.5/PKG-INFO` & `nstudypy-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NStudyPy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A NStudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
 Maintainer: Jack Li contributors
 Project-URL: Homepage, https://nstudy.org
 Project-URL: Documentation, https://hub.nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NStudyPy/issues
 Keywords: NStudyPy,tools
@@ -27,15 +27,19 @@
 ## 使用方法
 ```bash
 pip install -U NStudyPy -i https://pypi.org/simple
 ```
 
 ## 版本更新历史
 
-## version 0.0.4
+## version 0.0.6
+- 添加 `PyWeb` `PyFile` 工具
+- 更新 `PyString` `PyTools` 工具
+
+## version 0.0.5
 - 添加 `PyDate` `PyPDF` 工具
 - 更新 `PyString` `PyTools` 工具
 
 ## version 0.0.4
 - Python 升级到 3.9+
 - 添加 `PyShape` `PyString` 工具
```

### Comparing `nstudypy-0.0.5/pyproject.toml` & `nstudypy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.5/src/NStudyPy/PyDate.py` & `nstudypy-0.0.6/src/NStudyPy/PyDate.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,8 +49,16 @@
 def to_date(date_string: str, date_format: str = DATE_FORMAT_YYYY_MM_DD) -> datetime:
     """
     字符串转日期
     :param date_string:
     :param date_format: 见 get_date date_format
     :return:
     """
-    return datetime.strptime(date_string, date_format)
+    return datetime.strptime(date_string, date_format)
+
+
+def get_now() -> datetime:
+    """
+    获取当前时间
+    :return:
+    """
+    return datetime.now()
```

### Comparing `nstudypy-0.0.5/src/NStudyPy/PyPDF.py` & `nstudypy-0.0.6/src/NStudyPy/PyPDF.py`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.5/src/NStudyPy/PyShape.py` & `nstudypy-0.0.6/src/NStudyPy/PyShape.py`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.5/src/NStudyPy.egg-info/PKG-INFO` & `nstudypy-0.0.6/src/NStudyPy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NStudyPy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A NStudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
 Maintainer: Jack Li contributors
 Project-URL: Homepage, https://nstudy.org
 Project-URL: Documentation, https://hub.nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NStudyPy/issues
 Keywords: NStudyPy,tools
@@ -27,15 +27,19 @@
 ## 使用方法
 ```bash
 pip install -U NStudyPy -i https://pypi.org/simple
 ```
 
 ## 版本更新历史
 
-## version 0.0.4
+## version 0.0.6
+- 添加 `PyWeb` `PyFile` 工具
+- 更新 `PyString` `PyTools` 工具
+
+## version 0.0.5
 - 添加 `PyDate` `PyPDF` 工具
 - 更新 `PyString` `PyTools` 工具
 
 ## version 0.0.4
 - Python 升级到 3.9+
 - 添加 `PyShape` `PyString` 工具
```

