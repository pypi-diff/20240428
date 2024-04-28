# Comparing `tmp/amaproductreviews-0.0.5.tar.gz` & `tmp/amaproductreviews-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaproductreviews-0.0.5.tar", max compression
+gzip compressed data, was "amaproductreviews-0.0.6.tar", max compression
```

## Comparing `amaproductreviews-0.0.5.tar` & `amaproductreviews-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4718 2024-04-28 18:32:23.849241 amaproductreviews-0.0.5/amaproductreviews.py
--rw-r--r--   0        0        0      372 2024-04-28 19:37:46.532796 amaproductreviews-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1833 2024-04-28 19:37:06.282679 amaproductreviews-0.0.5/README.md
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 amaproductreviews-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     4718 2024-04-28 18:32:23.849241 amaproductreviews-0.0.6/amaproductreviews.py
+-rw-r--r--   0        0        0      371 2024-04-28 19:42:20.971115 amaproductreviews-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2245 2024-04-28 19:45:23.696166 amaproductreviews-0.0.6/README.md
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 amaproductreviews-0.0.6/PKG-INFO
```

### Comparing `amaproductreviews-0.0.5/amaproductreviews.py` & `amaproductreviews-0.0.6/amaproductreviews.py`

 * *Files identical despite different names*

