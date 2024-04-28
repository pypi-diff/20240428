# Comparing `tmp/numpyds-0.2.tar.gz` & `tmp/numpyds-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyds-0.2.tar", last modified: Sun Apr 28 14:37:45 2024, max compression
+gzip compressed data, was "numpyds-1.2.tar", last modified: Sun Apr 28 14:44:38 2024, max compression
```

## Comparing `numpyds-0.2.tar` & `numpyds-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 14:37:45.650876 numpyds-0.2/
--rw-rw-rw-   0        0        0      132 2024-04-28 14:37:45.648708 numpyds-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 14:37:45.622514 numpyds-0.2/numpyds/
--rw-rw-rw-   0        0        0     3329 2024-04-28 14:36:08.000000 numpyds-0.2/numpyds/__init__.py
--rw-rw-rw-   0        0        0    15540 2024-04-28 14:33:44.000000 numpyds-0.2/numpyds/main.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:37:45.647666 numpyds-0.2/numpyds.egg-info/
--rw-rw-rw-   0        0        0      132 2024-04-28 14:37:45.000000 numpyds-0.2/numpyds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-04-28 14:37:45.000000 numpyds-0.2/numpyds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 14:37:45.000000 numpyds-0.2/numpyds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 14:37:45.000000 numpyds-0.2/numpyds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-28 14:37:45.000000 numpyds-0.2/numpyds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 14:37:45.650876 numpyds-0.2/setup.cfg
--rw-rw-rw-   0        0        0      238 2024-04-28 14:37:35.000000 numpyds-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:44:38.589752 numpyds-1.2/
+-rw-rw-rw-   0        0        0      132 2024-04-28 14:44:38.589752 numpyds-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 14:44:38.571096 numpyds-1.2/numpyds/
+-rw-rw-rw-   0        0        0    18877 2024-04-28 14:43:34.000000 numpyds-1.2/numpyds/__init__.py
+-rw-rw-rw-   0        0        0    15540 2024-04-28 14:33:44.000000 numpyds-1.2/numpyds/main.py
+drwxrwxrwx   0        0        0        0 2024-04-28 14:44:38.588320 numpyds-1.2/numpyds.egg-info/
+-rw-rw-rw-   0        0        0      132 2024-04-28 14:44:38.000000 numpyds-1.2/numpyds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-04-28 14:44:38.000000 numpyds-1.2/numpyds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 14:44:38.000000 numpyds-1.2/numpyds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 14:44:38.000000 numpyds-1.2/numpyds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-28 14:44:38.000000 numpyds-1.2/numpyds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 14:44:38.589752 numpyds-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      238 2024-04-28 14:43:53.000000 numpyds-1.2/setup.py
```

### Comparing `numpyds-0.2/numpyds/main.py` & `numpyds-1.2/numpyds/main.py`

 * *Files identical despite different names*

