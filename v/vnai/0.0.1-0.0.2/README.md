# Comparing `tmp/vnai-0.0.1.tar.gz` & `tmp/vnai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnai-0.0.1.tar", last modified: Fri Apr 26 16:29:35 2024, max compression
+gzip compressed data, was "vnai-0.0.2.tar", last modified: Sun Apr 28 03:45:24 2024, max compression
```

## Comparing `vnai-0.0.1.tar` & `vnai-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-26 16:29:35.808298 vnai-0.0.1/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      271 2024-04-26 16:29:35.808298 vnai-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      168 2024-04-26 16:27:45.000000 vnai-0.0.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2024-04-26 16:29:35.808298 vnai-0.0.1/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-26 16:29:35.804298 vnai-0.0.1/vnai/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2024-04-26 16:27:45.000000 vnai-0.0.1/vnai/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-26 16:29:35.808298 vnai-0.0.1/vnai.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      271 2024-04-26 16:29:35.000000 vnai-0.0.1/vnai.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      153 2024-04-26 16:29:35.000000 vnai-0.0.1/vnai.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-26 16:29:35.000000 vnai-0.0.1/vnai.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2024-04-26 16:29:35.000000 vnai-0.0.1/vnai.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-28 03:45:24.019987 vnai-0.0.2/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      568 2024-04-28 03:45:24.019987 vnai-0.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      148 2024-04-28 03:41:21.000000 vnai-0.0.2/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      563 2024-04-28 03:45:24.019987 vnai-0.0.2/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-28 03:45:24.015987 vnai-0.0.2/vnai.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      568 2024-04-28 03:45:24.000000 vnai-0.0.2/vnai.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      163 2024-04-28 03:45:24.000000 vnai-0.0.2/vnai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-28 03:45:24.000000 vnai-0.0.2/vnai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-04-28 03:45:24.000000 vnai-0.0.2/vnai.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-28 03:45:24.000000 vnai-0.0.2/vnai.egg-info/top_level.txt
```

