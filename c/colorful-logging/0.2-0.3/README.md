# Comparing `tmp/colorful_logging-0.2.tar.gz` & `tmp/colorful_logging-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_logging-0.2.tar", last modified: Tue Feb  6 15:02:46 2024, max compression
+gzip compressed data, was "colorful_logging-0.3.tar", last modified: Sun Apr 28 07:08:12 2024, max compression
```

## Comparing `colorful_logging-0.2.tar` & `colorful_logging-0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-02-06 15:02:46.460565 colorful_logging-0.2/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      241 2024-02-06 15:02:46.460565 colorful_logging-0.2/PKG-INFO
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-02-06 15:02:46.460565 colorful_logging-0.2/colorful_logging.egg-info/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      241 2024-02-06 15:02:46.000000 colorful_logging-0.2/colorful_logging.egg-info/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      168 2024-02-06 15:02:46.000000 colorful_logging-0.2/colorful_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-02-06 15:02:46.000000 colorful_logging-0.2/colorful_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-02-06 15:02:46.000000 colorful_logging-0.2/colorful_logging.egg-info/top_level.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-02-06 15:02:46.460565 colorful_logging-0.2/setup.cfg
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      340 2024-02-06 15:02:44.000000 colorful_logging-0.2/setup.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:08:12.571385 colorful_logging-0.3/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1447 2024-04-28 07:08:12.571385 colorful_logging-0.3/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      659 2024-02-06 15:25:50.000000 colorful_logging-0.3/README.md
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:08:12.567381 colorful_logging-0.3/colorful_logging.egg-info/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1447 2024-04-28 07:08:12.000000 colorful_logging-0.3/colorful_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      178 2024-04-28 07:08:12.000000 colorful_logging-0.3/colorful_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:08:12.000000 colorful_logging-0.3/colorful_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:08:12.000000 colorful_logging-0.3/colorful_logging.egg-info/top_level.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:08:12.571385 colorful_logging-0.3/setup.cfg
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1081 2024-04-28 07:03:47.000000 colorful_logging-0.3/setup.py
```

