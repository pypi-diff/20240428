# Comparing `tmp/colorful_logging-0.5.tar.gz` & `tmp/colorful_logging-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_logging-0.5.tar", last modified: Sun Apr 28 07:27:16 2024, max compression
+gzip compressed data, was "colorful_logging-0.6.tar", last modified: Sun Apr 28 07:30:30 2024, max compression
```

## Comparing `colorful_logging-0.5.tar` & `colorful_logging-0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:27:16.809104 colorful_logging-0.5/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1610 2024-04-28 07:27:16.809104 colorful_logging-0.5/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      822 2024-04-28 07:13:32.000000 colorful_logging-0.5/README.md
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:27:16.809104 colorful_logging-0.5/colorful_logging.egg-info/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1610 2024-04-28 07:27:16.000000 colorful_logging-0.5/colorful_logging.egg-info/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      178 2024-04-28 07:27:16.000000 colorful_logging-0.5/colorful_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:27:16.000000 colorful_logging-0.5/colorful_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:27:16.000000 colorful_logging-0.5/colorful_logging.egg-info/top_level.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:27:16.809104 colorful_logging-0.5/setup.cfg
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1081 2024-04-28 07:27:02.000000 colorful_logging-0.5/setup.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:30:30.732294 colorful_logging-0.6/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1811 2024-04-28 07:30:30.732294 colorful_logging-0.6/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1023 2024-04-28 07:29:43.000000 colorful_logging-0.6/README.md
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:30:30.732294 colorful_logging-0.6/colorful_logging.egg-info/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1811 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      178 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/top_level.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:30:30.732294 colorful_logging-0.6/setup.cfg
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1081 2024-04-28 07:30:21.000000 colorful_logging-0.6/setup.py
```

### Comparing `colorful_logging-0.5/PKG-INFO` & `colorful_logging-0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful_logging
-Version: 0.5
+Version: 0.6
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -45,16 +45,28 @@
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
 ```python
-from colorful_logging import _get_color_
+from colorful_logging import get_color
 
-c = _get_color_("dark blue")
-r = _get_color_("reset")
+c = get_color("dark blue")
+r = get_color("reset")
 
-text = f"hello {c}Ali{}"
+text = f"hello {c}Ali{r}"
+print(text)
+```
+
+## You can also colorize you object:
+```python
+from colorful_logging import colorize
+
+p = Person(name="ali", age=18)
+
+colorized_elem = colorize("pink", p)
+
+print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.5/README.md` & `colorful_logging-0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -24,14 +24,26 @@
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
 ```python
-from colorful_logging import _get_color_
+from colorful_logging import get_color
 
-c = _get_color_("dark blue")
-r = _get_color_("reset")
+c = get_color("dark blue")
+r = get_color("reset")
 
-text = f"hello {c}Ali{}"
+text = f"hello {c}Ali{r}"
+print(text)
+```
+
+## You can also colorize you object:
+```python
+from colorful_logging import colorize
+
+p = Person(name="ali", age=18)
+
+colorized_elem = colorize("pink", p)
+
+print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.5/colorful_logging.egg-info/PKG-INFO` & `colorful_logging-0.6/colorful_logging.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logging
-Version: 0.5
+Version: 0.6
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -45,16 +45,28 @@
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
 ```python
-from colorful_logging import _get_color_
+from colorful_logging import get_color
 
-c = _get_color_("dark blue")
-r = _get_color_("reset")
+c = get_color("dark blue")
+r = get_color("reset")
 
-text = f"hello {c}Ali{}"
+text = f"hello {c}Ali{r}"
+print(text)
+```
+
+## You can also colorize you object:
+```python
+from colorful_logging import colorize
+
+p = Person(name="ali", age=18)
+
+colorized_elem = colorize("pink", p)
+
+print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.5/setup.py` & `colorful_logging-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = ""
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='colorful_logging',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/zamoosh/colorful_logging',
     author='zamoosh',
     author_email='moyi.pary@gmail.com',
     description='A library to print colorful',
     long_description_content_type="text/markdown",
```

