# Comparing `tmp/dazbo_commons-0.1.1.tar.gz` & `tmp/dazbo_commons-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dazbo_commons-0.1.1.tar", last modified: Sun Apr 28 14:54:11 2024, max compression
+gzip compressed data, was "dazbo_commons-0.1.2.tar", last modified: Sun Apr 28 15:41:01 2024, max compression
```

## Comparing `dazbo_commons-0.1.1.tar` & `dazbo_commons-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 14:54:11.367034 dazbo_commons-0.1.1/
--rw-rw-rw-   0        0        0     1078 2023-08-13 12:35:48.000000 dazbo_commons-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      757 2024-04-28 14:54:11.365022 dazbo_commons-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2410 2024-04-28 14:49:15.000000 dazbo_commons-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 14:54:11.368020 dazbo_commons-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-04-28 14:52:51.000000 dazbo_commons-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:54:11.323812 dazbo_commons-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 14:54:11.335316 dazbo_commons-0.1.1/src/dazbo_commons/
--rw-rw-rw-   0        0        0      210 2024-04-28 13:46:13.000000 dazbo_commons-0.1.1/src/dazbo_commons/__init__.py
--rw-rw-rw-   0        0        0     4272 2024-04-28 13:46:01.000000 dazbo_commons-0.1.1/src/dazbo_commons/colored_logging.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:54:11.363013 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/
--rw-rw-rw-   0        0        0      757 2024-04-28 14:54:11.000000 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-28 14:54:11.000000 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 14:54:11.000000 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-28 14:54:11.000000 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-28 14:54:11.000000 dazbo_commons-0.1.1/src/dazbo_commons.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 14:54:11.359670 dazbo_commons-0.1.1/tests/
--rw-rw-rw-   0        0        0     2916 2024-04-28 14:05:12.000000 dazbo_commons-0.1.1/tests/test_colored_logging.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.486826 dazbo_commons-0.1.2/
+-rw-rw-rw-   0        0        0     1099 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      782 2024-04-28 15:41:01.485826 dazbo_commons-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2619 2024-04-28 15:09:58.000000 dazbo_commons-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 15:41:01.486826 dazbo_commons-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      981 2024-04-28 15:39:58.000000 dazbo_commons-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.466828 dazbo_commons-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.473827 dazbo_commons-0.1.2/src/dazbo_commons/
+-rw-rw-rw-   0        0        0      210 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/src/dazbo_commons/__init__.py
+-rw-rw-rw-   0        0        0     4272 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/src/dazbo_commons/colored_logging.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.484826 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/
+-rw-rw-rw-   0        0        0      782 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.482828 dazbo_commons-0.1.2/tests/
+-rw-rw-rw-   0        0        0     2916 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/tests/test_colored_logging.py
```

### Comparing `dazbo_commons-0.1.1/LICENSE` & `dazbo_commons-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Derailed-Dash (Dazbo)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Derailed-Dash (Dazbo)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dazbo_commons-0.1.1/PKG-INFO` & `dazbo_commons-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dazbo_commons
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handy utility code, such as coloured logging.
 Home-page: https://github.com/derailed-dash/dazbo-commons-py
 Author: Darren Lester
 Author-email: derailed.dash@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorama
 Provides-Extra: dev
 Requires-Dist: pytest>=5.4; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 See the README in the project repo
```

### Comparing `dazbo_commons-0.1.1/README.md` & `dazbo_commons-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 ├── setup.cfg
 ├── LICENSE
 └── requirements.txt
 ```
 
 ## To Install and Use
 
+You can simply install the package from [PyPi](https://pypi.org/project/dazbo-commons/). There's no need to clone this repo.
+
 ```bash
 pip install dazbo-commons
 ```
 
-In your Python code, include this `import`:
+Then, in your Python code, include this `import`:
 
 ```python
 import dazbo_commons as dc
 ```
 
 ## Coloured Logging Module
 
@@ -83,32 +85,31 @@
 4. Install packages for actually creating the build. (If nto already included in `requirements.txt`):
 
 ```bash
 py -m pip install twine
 py -m pip install --upgrade build
 ```
 
-5. Build the package.
+5. Make any required updates to the `setup.py` file. E.g. the `version` attribute.
+
+6. Build the package.
 
 ```bash
 py -m build
 ```
 
 This generates a `dist` folder in your project folder.
 
-6. Upload the package to [PyPi](https://pypi.org/). 
+7. Upload the package to [PyPi](https://pypi.org/). 
 
 Notes:
 - You'll need to create a free account, if you haven't done so already.
 - You'll need to generate an API token in _Account Settings_, for uploading to the API.
+- You may want to delete any previous builds.
 
 ```bash
 py -m twine upload dist/*
 ```
 
 You'll be prompted for your API token. In my experience, when doing this from a terminal inside VS Code, Ctrl-V doesn't work here. So I use Paste from the menu, and this works.
 
-4. Deactivate the virtual environment. E.g.
-
-```bash
-deactivate
-```
+And we're done!
```

### Comparing `dazbo_commons-0.1.1/setup.py` & `dazbo_commons-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dazbo_commons',
-    version='0.1.1',
+    version='0.1.2',
     author='Darren Lester',
     author_email='derailed.dash@gmail.com',
     description='Handy utility code, such as coloured logging.',
     long_description='See the README in the project repo',
     long_description_content_type='text/markdown',
     url='https://github.com/derailed-dash/dazbo-commons-py',
     package_dir={'': 'src'},
@@ -16,15 +16,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
     python_requires='>=3.7',
     install_requires=[
-        # list of required packages
+        'colorama',
     ],
     extras_require={
         'dev': [
             'pytest>=5.4',
             'check-manifest',
             'twine',
         ],
```

### Comparing `dazbo_commons-0.1.1/src/dazbo_commons/colored_logging.py` & `dazbo_commons-0.1.2/src/dazbo_commons/colored_logging.py`

 * *Files identical despite different names*

### Comparing `dazbo_commons-0.1.1/src/dazbo_commons.egg-info/PKG-INFO` & `dazbo_commons-0.1.2/src/dazbo_commons.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dazbo_commons
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handy utility code, such as coloured logging.
 Home-page: https://github.com/derailed-dash/dazbo-commons-py
 Author: Darren Lester
 Author-email: derailed.dash@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorama
 Provides-Extra: dev
 Requires-Dist: pytest>=5.4; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 See the README in the project repo
```

### Comparing `dazbo_commons-0.1.1/tests/test_colored_logging.py` & `dazbo_commons-0.1.2/tests/test_colored_logging.py`

 * *Files identical despite different names*

