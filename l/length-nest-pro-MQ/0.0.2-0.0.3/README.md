# Comparing `tmp/length_nest_pro_MQ-0.0.2.tar.gz` & `tmp/length_nest_pro_mq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "length_nest_pro_MQ-0.0.2.tar", last modified: Mon Apr 15 19:44:32 2024, max compression
+gzip compressed data, was "length_nest_pro_mq-0.0.3.tar", last modified: Sun Apr 28 13:45:25 2024, max compression
```

## Comparing `length_nest_pro_MQ-0.0.2.tar` & `length_nest_pro_mq-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 19:44:32.603241 length_nest_pro_MQ-0.0.2/
--rw-rw-rw-   0        0        0    35823 2024-02-15 16:11:23.000000 length_nest_pro_MQ-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-15 19:44:32.586434 length_nest_pro_MQ-0.0.2/LengthNestProMQ/
--rw-rw-rw-   0        0        0        0 2024-04-15 13:48:44.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/__init__.py
--rw-rw-rw-   0        0        0    10331 2024-03-11 13:47:55.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/column_sort.py
--rw-rw-rw-   0        0        0     2425 2024-03-18 11:28:24.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/day_based_rot_file_handler.py
--rw-rw-rw-   0        0        0     7314 2024-04-15 19:39:25.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/main.py
--rw-rw-rw-   0        0        0    66083 2024-03-11 15:07:58.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/nest_calculation_new.py
--rw-rw-rw-   0        0        0     2026 2024-04-15 19:38:57.000000 length_nest_pro_MQ-0.0.2/LengthNestProMQ/rabbitmq_manager.py
--rw-rw-rw-   0        0        0      386 2024-04-15 19:44:32.602241 length_nest_pro_MQ-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2024-03-30 10:05:36.000000 length_nest_pro_MQ-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 19:44:32.600278 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-15 19:44:32.000000 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-15 19:44:32.000000 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 19:44:32.000000 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-15 19:44:32.000000 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 19:44:32.000000 length_nest_pro_MQ-0.0.2/length_nest_pro_MQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      671 2024-04-15 18:19:59.000000 length_nest_pro_MQ-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 19:44:32.603241 length_nest_pro_MQ-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-04-15 19:43:41.000000 length_nest_pro_MQ-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:45:25.840446 length_nest_pro_mq-0.0.3/
+-rw-rw-rw-   0        0        0      343 2024-04-28 13:45:25.838473 length_nest_pro_mq-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 13:45:25.836462 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:45:25.841444 length_nest_pro_mq-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-04-28 13:45:08.000000 length_nest_pro_mq-0.0.3/setup.py
```

### Comparing `length_nest_pro_MQ-0.0.2/setup.py` & `length_nest_pro_mq-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
-DESCRIPTION = 'length_nest_pro_MQ'
-LONG_DESCRIPTION = 'An adapted version of the length nest pro, enriched with a message queue connection'
+VERSION = '0.0.1'
+DESCRIPTION = 'My first Python package'
+LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
-    name="length_nest_pro_MQ",
-    version=VERSION,
+    name="length-nest-pro-MQ",
+    version='0.0.3',
     author="Niels Bos",
     author_email="nielsb00@gmail.com",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    description="length_nest_pro_MQ",
+    long_description="Adapted version of length_nest_pro, enhanced with message queue",
     packages=find_packages(),
-    install_requires=[
-        "numpy",
-        "wheel",
-        "setuptools",
-        "pika"
-    ],  # add any additional packages that
+    install_requires=['numpy', 'wheel', 'setuptools', 'pika'],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
-    keywords=['rabbit mq', 'length nest pro'],
-    classifiers=[
-    ]
+    keywords=["rabbit mq", "length nest pro"]
+
 )
```

