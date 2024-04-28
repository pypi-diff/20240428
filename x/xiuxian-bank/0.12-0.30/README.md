# Comparing `tmp/xiuxian_bank-0.12.tar.gz` & `tmp/xiuxian_bank-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian_bank-0.12.tar", last modified: Thu Apr 25 01:38:24 2024, max compression
+gzip compressed data, was "xiuxian_bank-0.30.tar", last modified: Sun Apr 28 20:05:03 2024, max compression
```

## Comparing `xiuxian_bank-0.12.tar` & `xiuxian_bank-0.30.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:38:24.182659 xiuxian_bank-0.12/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:38:24.182659 xiuxian_bank-0.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 01:38:24.182659 xiuxian_bank-0.12/setup.cfg
--rw-rw-rw-   0        0        0      490 2024-04-25 00:03:51.000000 xiuxian_bank-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:38:24.181658 xiuxian_bank-0.12/xiuxian_bank.egg-info/
--rw-rw-rw-   0        0        0      251 2024-04-25 01:38:24.000000 xiuxian_bank-0.12/xiuxian_bank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-25 01:38:24.000000 xiuxian_bank-0.12/xiuxian_bank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:38:24.000000 xiuxian_bank-0.12/xiuxian_bank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:38:24.000000 xiuxian_bank-0.12/xiuxian_bank.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:03.104609 xiuxian_bank-0.30/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:03.103618 xiuxian_bank-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:05:03.104609 xiuxian_bank-0.30/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-28 20:03:16.000000 xiuxian_bank-0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:03.095621 xiuxian_bank-0.30/xiuxian_bank/
+-rw-rw-rw-   0        0        0    10525 2024-04-28 19:39:42.000000 xiuxian_bank-0.30/xiuxian_bank/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-04-22 01:25:08.000000 xiuxian_bank-0.30/xiuxian_bank/bankconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:05:03.102618 xiuxian_bank-0.30/xiuxian_bank.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-04-28 20:05:03.000000 xiuxian_bank-0.30/xiuxian_bank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-28 20:05:03.000000 xiuxian_bank-0.30/xiuxian_bank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:05:03.000000 xiuxian_bank-0.30/xiuxian_bank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:05:03.000000 xiuxian_bank-0.30/xiuxian_bank.egg-info/top_level.txt
```

