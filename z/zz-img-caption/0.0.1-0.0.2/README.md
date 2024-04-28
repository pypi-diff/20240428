# Comparing `tmp/zz-img-caption-0.0.1.tar.gz` & `tmp/zz-img-caption-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zz-img-caption-0.0.1.tar", last modified: Sun Apr 28 09:20:13 2024, max compression
+gzip compressed data, was "zz-img-caption-0.0.2.tar", last modified: Sun Apr 28 09:36:40 2024, max compression
```

## Comparing `zz-img-caption-0.0.1.tar` & `zz-img-caption-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 09:20:13.047244 zz-img-caption-0.0.1/
--rw-rw-rw-   0        0        0      907 2024-04-28 09:20:13.047244 zz-img-caption-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 09:20:13.041737 zz-img-caption-0.0.1/caption/
--rw-rw-rw-   0        0        0        0 2024-04-28 06:23:48.000000 zz-img-caption-0.0.1/caption/__init__.py
--rw-rw-rw-   0        0        0     4614 2024-04-28 06:29:20.000000 zz-img-caption-0.0.1/caption/caption_engine.py
--rw-rw-rw-   0        0        0     6020 2024-04-28 09:14:30.000000 zz-img-caption-0.0.1/caption/cli_main.py
--rw-rw-rw-   0        0        0     1631 2024-04-28 08:46:02.000000 zz-img-caption-0.0.1/caption/cli_parser.py
--rw-rw-rw-   0        0        0      212 2024-04-28 09:18:56.000000 zz-img-caption-0.0.1/caption/manifest.json
--rw-rw-rw-   0        0        0      704 2024-04-28 07:00:01.000000 zz-img-caption-0.0.1/caption/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-28 09:20:13.047244 zz-img-caption-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1638 2024-04-28 08:44:49.000000 zz-img-caption-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 09:20:13.046246 zz-img-caption-0.0.1/zz_img_caption.egg-info/
--rw-rw-rw-   0        0        0      907 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 09:20:13.000000 zz-img-caption-0.0.1/zz_img_caption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 09:36:40.075454 zz-img-caption-0.0.2/
+-rw-rw-rw-   0        0        0     3993 2024-04-28 09:36:40.075454 zz-img-caption-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 09:36:40.065443 zz-img-caption-0.0.2/caption/
+-rw-rw-rw-   0        0        0        0 2024-04-28 06:23:48.000000 zz-img-caption-0.0.2/caption/__init__.py
+-rw-rw-rw-   0        0        0     4614 2024-04-28 06:29:20.000000 zz-img-caption-0.0.2/caption/caption_engine.py
+-rw-rw-rw-   0        0        0     6020 2024-04-28 09:14:30.000000 zz-img-caption-0.0.2/caption/cli_main.py
+-rw-rw-rw-   0        0        0     1631 2024-04-28 08:46:02.000000 zz-img-caption-0.0.2/caption/cli_parser.py
+-rw-rw-rw-   0        0        0      212 2024-04-28 09:36:23.000000 zz-img-caption-0.0.2/caption/manifest.json
+-rw-rw-rw-   0        0        0      704 2024-04-28 07:00:01.000000 zz-img-caption-0.0.2/caption/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 09:36:40.075454 zz-img-caption-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2024-04-28 08:44:49.000000 zz-img-caption-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 09:36:40.075454 zz-img-caption-0.0.2/zz_img_caption.egg-info/
+-rw-rw-rw-   0        0        0     3993 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 09:36:40.000000 zz-img-caption-0.0.2/zz_img_caption.egg-info/top_level.txt
```

### Comparing `zz-img-caption-0.0.1/caption/caption_engine.py` & `zz-img-caption-0.0.2/caption/caption_engine.py`

 * *Files identical despite different names*

### Comparing `zz-img-caption-0.0.1/caption/cli_main.py` & `zz-img-caption-0.0.2/caption/cli_main.py`

 * *Files identical despite different names*

### Comparing `zz-img-caption-0.0.1/caption/cli_parser.py` & `zz-img-caption-0.0.2/caption/cli_parser.py`

 * *Files identical despite different names*

### Comparing `zz-img-caption-0.0.1/caption/utils.py` & `zz-img-caption-0.0.2/caption/utils.py`

 * *Files identical despite different names*

### Comparing `zz-img-caption-0.0.1/setup.py` & `zz-img-caption-0.0.2/setup.py`

 * *Files identical despite different names*

