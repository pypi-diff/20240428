# Comparing `tmp/length_nest_pro_mq-0.0.3.tar.gz` & `tmp/length_nest_pro_mq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "length_nest_pro_mq-0.0.3.tar", last modified: Sun Apr 28 13:45:25 2024, max compression
+gzip compressed data, was "length_nest_pro_mq-0.0.4.tar", last modified: Sun Apr 28 14:17:26 2024, max compression
```

## Comparing `length_nest_pro_mq-0.0.3.tar` & `length_nest_pro_mq-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:45:25.840446 length_nest_pro_mq-0.0.3/
--rw-rw-rw-   0        0        0      343 2024-04-28 13:45:25.838473 length_nest_pro_mq-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 13:45:25.836462 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/
--rw-rw-rw-   0        0        0      343 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:45:25.000000 length_nest_pro_mq-0.0.3/length_nest_pro_MQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 13:45:25.841444 length_nest_pro_mq-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-04-28 13:45:08.000000 length_nest_pro_mq-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:17:26.747597 length_nest_pro_mq-0.0.4/
+-rw-rw-rw-   0        0        0      343 2024-04-28 14:17:26.745605 length_nest_pro_mq-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 14:17:26.721664 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/
+-rw-rw-rw-   0        0        0       37 2024-04-28 12:04:54.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/__init__.py
+-rw-rw-rw-   0        0        0    10331 2024-04-27 07:27:35.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/column_sort.py
+-rw-rw-rw-   0        0        0     2425 2024-04-27 07:27:35.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/day_based_rot_file_handler.py
+-rw-rw-rw-   0        0        0     7684 2024-04-28 12:41:45.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/main.py
+-rw-rw-rw-   0        0        0    66082 2024-04-28 12:05:52.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/nest_calculation_new.py
+-rw-rw-rw-   0        0        0     1898 2024-04-28 12:17:05.000000 length_nest_pro_mq-0.0.4/length-nest-pro-MQ/rabbitmq_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:17:26.744643 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-04-28 14:17:26.000000 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-04-28 14:17:26.000000 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 14:17:26.000000 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-28 14:17:26.000000 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-28 14:17:26.000000 length_nest_pro_mq-0.0.4/length_nest_pro_MQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 14:17:26.748594 length_nest_pro_mq-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      811 2024-04-28 14:17:20.000000 length_nest_pro_mq-0.0.4/setup.py
```

### Comparing `length_nest_pro_mq-0.0.3/setup.py` & `length_nest_pro_mq-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="length-nest-pro-MQ",
-    version='0.0.3',
+    version='0.0.4',
     author="Niels Bos",
     author_email="nielsb00@gmail.com",
     description="length_nest_pro_MQ",
     long_description="Adapted version of length_nest_pro, enhanced with message queue",
     packages=find_packages(),
+    package_data={'spam': ['data.txt']},
     install_requires=['numpy', 'wheel', 'setuptools', 'pika'],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=["rabbit mq", "length nest pro"]
 
 )
```

