# Comparing `tmp/oscb-1.0.0.tar.gz` & `tmp/oscb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.0.0.tar", last modified: Wed Apr 24 14:34:03 2024, max compression
+gzip compressed data, was "oscb-1.0.6.tar", last modified: Sun Apr 28 01:03:20 2024, max compression
```

## Comparing `oscb-1.0.0.tar` & `oscb-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:34:03.776629 oscb-1.0.0/
--rw-rw-rw-   0        0        0      652 2024-04-24 14:34:03.775629 oscb-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 14:34:03.751588 oscb-1.0.0/oscb/
--rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.0/oscb/__init__.py
--rw-rw-rw-   0        0        0      650 2024-04-23 21:02:52.000000 oscb-1.0.0/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:34:03.774642 oscb-1.0.0/oscb.egg-info/
--rw-rw-rw-   0        0        0      652 2024-04-24 14:34:03.000000 oscb-1.0.0/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-24 14:34:03.000000 oscb-1.0.0/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:34:03.000000 oscb-1.0.0/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-24 14:34:03.000000 oscb-1.0.0/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 14:34:03.000000 oscb-1.0.0/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:34:03.776629 oscb-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1839 2024-04-23 21:19:30.000000 oscb-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.209242 oscb-1.0.6/
+-rw-rw-rw-   0        0        0      650 2024-04-28 01:03:20.209242 oscb-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.187679 oscb-1.0.6/oscb/
+-rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.0.6/oscb/__init__.py
+-rw-rw-rw-   0        0        0      650 2024-04-28 01:02:11.000000 oscb-1.0.6/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-28 01:03:20.206941 oscb-1.0.6/oscb.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 01:03:20.000000 oscb-1.0.6/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 01:03:20.209242 oscb-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1735 2024-04-28 01:02:44.000000 oscb-1.0.6/setup.py
```

### Comparing `oscb-1.0.0/PKG-INFO` & `oscb-1.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.0
-Summary: oscb
-Home-page: https://github.com/cirisjl/Machine-learning-development-environment-for-single-cell-sequencing-data-analyses.git
-Author: OSCB Team
-Author-email: 
-License: MIT
-Keywords: pytorch,graph machine learning,graph representation learning,graph neural networks
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
+Version: 1.0.6
+Summary: Description of your package
+Home-page: https://github.com/your_username/oscb
+Author: Your Name
+Author-email: your.email@example.com
+Keywords: sample setuptools development
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `oscb-1.0.0/oscb/version.py` & `oscb-1.0.6/oscb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.0.0'
+__version__ = '1.0.6'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.0.0/oscb.egg-info/PKG-INFO` & `oscb-1.0.6/oscb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.0.0
-Summary: oscb
-Home-page: https://github.com/cirisjl/Machine-learning-development-environment-for-single-cell-sequencing-data-analyses.git
-Author: OSCB Team
-Author-email: 
-License: MIT
-Keywords: pytorch,graph machine learning,graph representation learning,graph neural networks
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
+Version: 1.0.6
+Summary: Description of your package
+Home-page: https://github.com/your_username/oscb
+Author: Your Name
+Author-email: your.email@example.com
+Keywords: sample setuptools development
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `oscb-1.0.0/setup.py` & `oscb-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,41 +16,42 @@
 readme_path = path.join(here, 'README.md')
 try:
     with open(readme_path, encoding='utf-8') as f:
         long_description = f.read()
 except FileNotFoundError:
     print(f"README.md not found at '{readme_path}'. No long description provided.")
 
-package_data_list = []
 
-setup(name='oscb',
-      version=__version__,
-      description='oscb',
-      url='https://github.com/cirisjl/Machine-learning-development-environment-for-single-cell-sequencing-data-analyses.git',
-      author='OSCB Team',
-      author_email='',
-      keywords=['pytorch', 'graph machine learning', 'graph representation learning', 'graph neural networks'],
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      install_requires = [
+setup(
+    name='oscb',
+    version='1.0.6',
+    description='Description of your package',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/your_username/oscb',
+    author='Your Name',
+    author_email='your.email@example.com',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+    ],
+    keywords='sample setuptools development',
+    packages=find_packages(),
+    python_requires='>=3.6, <4',
+    install_requires=[
         'torch>=1.6.0',
         'numpy>=1.16.0',
         'tqdm>=4.29.0',
         'scikit-learn>=0.20.0',
         'pandas>=0.24.0',
         'six>=1.12.0',
         'urllib3>=1.24.0',
         'outdated>=0.2.0',
         'joblib>=1.3.2'
-      ],
-      license='MIT',
-      packages=find_packages(exclude=['dataset', 'examples', 'docs']),
-      package_data={'oscb': package_data_list},
-      include_package_data=True,
-      classifiers=[
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'Intended Audience :: Science/Research',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'License :: OSI Approved :: MIT License',
     ],
-)
+    package_data={'oscb': ['data/*.csv']},  # Add your package data here if any
+)
```

