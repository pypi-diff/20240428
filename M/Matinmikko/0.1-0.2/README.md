# Comparing `tmp/Matinmikko-0.1.tar.gz` & `tmp/Matinmikko-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Matinmikko-0.1.tar", last modified: Sun Apr 28 08:49:48 2024, max compression
+gzip compressed data, was "Matinmikko-0.2.tar", last modified: Sun Apr 28 09:07:22 2024, max compression
```

## Comparing `Matinmikko-0.1.tar` & `Matinmikko-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:49:48.902092 Matinmikko-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-28 08:49:48.828474 Matinmikko-0.1/Matinmikko/
--rw-rw-rw-   0        0        0       25 2024-04-28 08:13:43.000000 Matinmikko-0.1/Matinmikko/__init__.py
--rw-rw-rw-   0        0        0       35 2024-04-28 08:13:38.000000 Matinmikko-0.1/Matinmikko/main.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:49:48.897090 Matinmikko-0.1/Matinmikko.egg-info/
--rw-rw-rw-   0        0        0       55 2024-04-28 08:49:48.000000 Matinmikko-0.1/Matinmikko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-28 08:49:48.000000 Matinmikko-0.1/Matinmikko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:49:48.000000 Matinmikko-0.1/Matinmikko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-28 08:49:48.000000 Matinmikko-0.1/Matinmikko.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-04-28 08:49:48.000000 Matinmikko-0.1/Matinmikko.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       55 2024-04-28 08:49:48.901086 Matinmikko-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       27 2024-04-28 08:16:28.000000 Matinmikko-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 08:49:48.903087 Matinmikko-0.1/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-04-28 08:46:12.000000 Matinmikko-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:07:22.177140 Matinmikko-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-28 09:07:22.144533 Matinmikko-0.2/Matinmikko/
+-rw-rw-rw-   0        0        0       25 2024-04-28 08:13:43.000000 Matinmikko-0.2/Matinmikko/__init__.py
+-rw-rw-rw-   0        0        0       35 2024-04-28 08:13:38.000000 Matinmikko-0.2/Matinmikko/main.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:07:22.170613 Matinmikko-0.2/Matinmikko.egg-info/
+-rw-rw-rw-   0        0        0      127 2024-04-28 09:07:21.000000 Matinmikko-0.2/Matinmikko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-28 09:07:22.000000 Matinmikko-0.2/Matinmikko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:07:21.000000 Matinmikko-0.2/Matinmikko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-28 09:07:21.000000 Matinmikko-0.2/Matinmikko.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-04-28 09:07:21.000000 Matinmikko-0.2/Matinmikko.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      127 2024-04-28 09:07:22.175143 Matinmikko-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2024-04-28 08:16:28.000000 Matinmikko-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:07:22.178150 Matinmikko-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      424 2024-04-28 09:07:08.000000 Matinmikko-0.2/setup.py
```

