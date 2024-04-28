# Comparing `tmp/colorful_logging-0.6.tar.gz` & `tmp/colorful_logging-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_logging-0.6.tar", last modified: Sun Apr 28 07:30:30 2024, max compression
+gzip compressed data, was "colorful_logging-0.7.tar", last modified: Sun Apr 28 07:38:30 2024, max compression
```

## Comparing `colorful_logging-0.6.tar` & `colorful_logging-0.7.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:30:30.732294 colorful_logging-0.6/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1811 2024-04-28 07:30:30.732294 colorful_logging-0.6/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1023 2024-04-28 07:29:43.000000 colorful_logging-0.6/README.md
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:30:30.732294 colorful_logging-0.6/colorful_logging.egg-info/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1811 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      178 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:30:30.000000 colorful_logging-0.6/colorful_logging.egg-info/top_level.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:30:30.732294 colorful_logging-0.6/setup.cfg
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1081 2024-04-28 07:30:21.000000 colorful_logging-0.6/setup.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:38:30.402250 colorful_logging-0.7/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1864 2024-04-28 07:38:30.402250 colorful_logging-0.7/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1076 2024-04-28 07:36:59.000000 colorful_logging-0.7/README.md
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:38:30.402250 colorful_logging-0.7/colorful_logging/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 06:42:56.000000 colorful_logging-0.7/colorful_logging/__init__.py
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     5410 2024-04-28 07:23:22.000000 colorful_logging-0.7/colorful_logging/colorful_logging.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:38:30.402250 colorful_logging-0.7/colorful_logging.egg-info/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1864 2024-04-28 07:38:30.000000 colorful_logging-0.7/colorful_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      244 2024-04-28 07:38:30.000000 colorful_logging-0.7/colorful_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:38:30.000000 colorful_logging-0.7/colorful_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       17 2024-04-28 07:38:30.000000 colorful_logging-0.7/colorful_logging.egg-info/top_level.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:38:30.402250 colorful_logging-0.7/setup.cfg
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1086 2024-04-28 07:38:09.000000 colorful_logging-0.7/setup.py
```

### Comparing `colorful_logging-0.6/PKG-INFO` & `colorful_logging-0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful_logging
-Version: 0.6
+Version: 0.7
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # This is just a simple library to print colorful using sys.stderr to write.
 
 ```python
-from colorful_logging import color_print
+from colorful_logging.colorful_logging import color_print
 
 # color_print(
 # text: str = your text
 # color: str = 'red', 'blue', ...
 # fmt: bool = True or False
 # lvl: str -> it's just a simple naming when using the "fmt=True"
 # )
@@ -44,27 +44,29 @@
 
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
+
 ```python
-from colorful_logging import get_color
+from colorful_logging.colorful_logging import get_color
 
 c = get_color("dark blue")
 r = get_color("reset")
 
 text = f"hello {c}Ali{r}"
 print(text)
 ```
 
 ## You can also colorize you object:
+
 ```python
-from colorful_logging import colorize
+from colorful_logging.colorful_logging import colorize
 
 p = Person(name="ali", age=18)
 
 colorized_elem = colorize("pink", p)
 
 print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.6/README.md` & `colorful_logging-0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This is just a simple library to print colorful using sys.stderr to write.
 
 ```python
-from colorful_logging import color_print
+from colorful_logging.colorful_logging import color_print
 
 # color_print(
 # text: str = your text
 # color: str = 'red', 'blue', ...
 # fmt: bool = True or False
 # lvl: str -> it's just a simple naming when using the "fmt=True"
 # )
@@ -23,27 +23,29 @@
 
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
+
 ```python
-from colorful_logging import get_color
+from colorful_logging.colorful_logging import get_color
 
 c = get_color("dark blue")
 r = get_color("reset")
 
 text = f"hello {c}Ali{r}"
 print(text)
 ```
 
 ## You can also colorize you object:
+
 ```python
-from colorful_logging import colorize
+from colorful_logging.colorful_logging import colorize
 
 p = Person(name="ali", age=18)
 
 colorized_elem = colorize("pink", p)
 
 print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.6/colorful_logging.egg-info/PKG-INFO` & `colorful_logging-0.7/colorful_logging.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logging
-Version: 0.6
+Version: 0.7
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # This is just a simple library to print colorful using sys.stderr to write.
 
 ```python
-from colorful_logging import color_print
+from colorful_logging.colorful_logging import color_print
 
 # color_print(
 # text: str = your text
 # color: str = 'red', 'blue', ...
 # fmt: bool = True or False
 # lvl: str -> it's just a simple naming when using the "fmt=True"
 # )
@@ -44,27 +44,29 @@
 
 
 # here also you can use it without formatting the line: 
 color_print('ali is good', 'bold')
 ```
 
 ## To get specific color:
+
 ```python
-from colorful_logging import get_color
+from colorful_logging.colorful_logging import get_color
 
 c = get_color("dark blue")
 r = get_color("reset")
 
 text = f"hello {c}Ali{r}"
 print(text)
 ```
 
 ## You can also colorize you object:
+
 ```python
-from colorful_logging import colorize
+from colorful_logging.colorful_logging import colorize
 
 p = Person(name="ali", age=18)
 
 colorized_elem = colorize("pink", p)
 
 print(f"hello {colorized_elem}")
 ```
```

### Comparing `colorful_logging-0.6/setup.py` & `colorful_logging-0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 long_description = ""
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='colorful_logging',
-    version='0.6',
-    packages=find_packages(),
+    version='0.7',
+    packages=['colorful_logging'],
     install_requires=[],
     url='https://github.com/zamoosh/colorful_logging',
     author='zamoosh',
     author_email='moyi.pary@gmail.com',
     description='A library to print colorful',
     long_description_content_type="text/markdown",
     long_description=long_description,
```

