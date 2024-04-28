# Comparing `tmp/hustmirror_cli-1.1.2b0.tar.gz` & `tmp/hustmirror_cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hustmirror_cli-1.1.2b0.tar", last modified: Mon Apr 22 08:15:54 2024, max compression
+gzip compressed data, was "hustmirror_cli-1.1.3.tar", last modified: Sun Apr 28 07:19:02 2024, max compression
```

## Comparing `hustmirror_cli-1.1.2b0.tar` & `hustmirror_cli-1.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-22 08:15:39.355380 hustmirror_cli-1.1.2b0/LICENSE
--rw-r--r--   0        0        0       17 2024-04-22 08:15:39.355380 hustmirror_cli-1.1.2b0/README.md
--rw-r--r--   0        0        0      471 2024-04-22 08:15:54.763552 hustmirror_cli-1.1.2b0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 08:15:39.355380 hustmirror_cli-1.1.2b0/src/hustmirror_cli/__init__.py
--rw-r--r--   0        0        0      242 1970-01-01 00:00:00.000000 hustmirror_cli-1.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/README.md
+-rw-r--r--   0        0        0      470 2024-04-28 07:19:02.827945 hustmirror_cli-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/src/hustmirror_cli/__init__.py
+-rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 hustmirror_cli-1.1.3/PKG-INFO
```

### Comparing `hustmirror_cli-1.1.2b0/LICENSE` & `hustmirror_cli-1.1.3/LICENSE`

 * *Files identical despite different names*

