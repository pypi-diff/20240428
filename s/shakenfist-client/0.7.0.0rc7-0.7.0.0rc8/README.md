# Comparing `tmp/shakenfist-client-0.7.0.0rc7.tar.gz` & `tmp/shakenfist-client-0.7.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-client-0.7.0.0rc7.tar", last modified: Mon Sep 11 10:12:01 2023, max compression
+gzip compressed data, was "shakenfist-client-0.7.0.0rc8.tar", last modified: Sun Apr 28 03:26:20 2024, max compression
```

## Comparing `shakenfist-client-0.7.0.0rc7.tar` & `shakenfist-client-0.7.0.0rc8.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.328906 shakenfist-client-0.7.0.0rc7/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.316906 shakenfist-client-0.7.0.0rc7/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.320906 shakenfist-client-0.7.0.0rc7/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1048 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/configure-tests.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8972 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8981 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8987 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9337 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1306 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-09-11 10:12:01.328906 shakenfist-client-0.7.0.0rc7/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.324906 shakenfist-client-0.7.0.0rc7/ansible/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10729 2022-11-20 01:06:18.000000 shakenfist-client-0.7.0.0rc7/ansible/sf_instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3994 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc7/ansible/sf_network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc7/ansible/sf_snapshot.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      398 2023-09-11 10:11:25.000000 shakenfist-client-0.7.0.0rc7/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2023-09-11 10:12:01.332906 shakenfist-client-0.7.0.0rc7/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1372 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.324906 shakenfist-client-0.7.0.0rc7/shakenfist_client/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    38802 2023-09-11 10:11:25.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/apiclient.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.328906 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/admin.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    13862 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/artifact.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/backup.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7843 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/blob.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    29220 2023-09-11 10:11:25.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3249 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/interface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/label.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8896 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/namespace.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8294 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7475 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/node.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4222 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/main.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.328906 shakenfist-client-0.7.0.0rc7/shakenfist_client/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15322 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/tests/test_client_apiclient.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5829 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client/util.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.324906 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1476 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      129 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2023-09-11 10:12:01.000000 shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-09-11 10:12:01.328906 shakenfist-client-0.7.0.0rc7/tools/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc7/tools/buffer.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc7/tools/clone_with_depends.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc7/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc7/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.892466 shakenfist-client-0.7.0.0rc8/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.880466 shakenfist-client-0.7.0.0rc8/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.884466 shakenfist-client-0.7.0.0rc8/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8978 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/.github/workflows/ansible-module-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7892 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7898 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7898 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-ubuntu-2204-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1094 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2024-04-28 03:26:20.892466 shakenfist-client-0.7.0.0rc8/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.884466 shakenfist-client-0.7.0.0rc8/ansible/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      128 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/ansible/sf_instance
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      128 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/ansible/sf_namespace
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      127 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/ansible/sf_network
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc8/ansible/sf_snapshot.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      429 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2024-04-28 03:26:20.892466 shakenfist-client-0.7.0.0rc8/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1406 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.884466 shakenfist-client-0.7.0.0rc8/shakenfist_client/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    42740 2024-04-28 03:25:53.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/apiclient.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.888466 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/admin.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    19707 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/ansible.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13862 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/artifact.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/backup.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7843 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/blob.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    30645 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3249 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/interface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    20147 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/k3s.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/label.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8896 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/namespace.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10542 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8531 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/node.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4376 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/main.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.892466 shakenfist-client-0.7.0.0rc8/shakenfist_client/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15344 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/tests/test_client_apiclient.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5758 2024-03-29 00:25:05.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client/util.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.888466 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1540 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      136 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2024-04-28 03:26:20.000000 shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-28 03:26:20.892466 shakenfist-client-0.7.0.0rc8/tools/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc8/tools/buffer.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc8/tools/clone_with_depends.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc8/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc8/tox.ini
```

### Comparing `shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-debian-10-localhost.yml` & `shakenfist-client-0.7.0.0rc8/.github/workflows/ansible-module-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-name: Test debian-10-localhost
+name: Ansible module testing
 
 on:
   push:
     branches:
       - develop
       - v*-releases
   pull_request:
     branches:
       - develop
       - v*-releases
 
 jobs:
-  debian-10-localhost:
+  ansible-modules:
     runs-on: self-hosted
-    timeout-minutes: 120
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
       cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
@@ -40,27 +39,30 @@
           python3 ${GITHUB_WORKSPACE}/client-python/tools/clone_with_depends.py
 
       - name: Build infrastructure
         run: |
           cd ${GITHUB_WORKSPACE}/shakenfist
           ansible-playbook -i /home/debian/ansible-hosts \
               --extra-vars "identifier=${SHAKENFIST_NAMESPACE} source_path=${GITHUB_WORKSPACE} \
-              base_image=sf://label/ci-images/debian-10 base_image_user=debian" \
-              deploy/ansible/ci-topology-localhost.yml
+              base_image=sf://label/ci-images/debian-11 base_image_user=debian" \
+              deploy/ansible/ci-topology-slim-primary.yml
 
-      - name: Log github actions buffering status
+      - name: Copy CI tools to primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           cd ${GITHUB_WORKSPACE}/shakenfist
           scp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              tools/buffer.py debian@$primary:buffer.py
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              debian@$primary python3 buffer.py
+              -o UserKnownHostsFile=/dev/null -rp tools \
+              debian@$primary:.
+
+      - name: Log github actions buffering status
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} python3 tools/buffer.py
 
       - name: Run getsf installer on primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               debian@$primary /tmp/getsf-wrapper
@@ -73,15 +75,15 @@
 
       - name: Wait for API to start answering
         run: |
           set +e
 
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary 'sudo chmod ugo+r /etc/sf/sfrc /etc/sf/shakenfist.json /var/log/syslog'
+              debian@$primary 'sudo chmod ugo+r /etc/sf/* /var/log/syslog'
 
           count=0
           while [ $count -lt 60 ]
           do
             ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary '. /etc/sf/sfrc; sf-client instance list'
             if [ $? == 0 ]; then
@@ -106,39 +108,27 @@
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload debian-11 /srv/ci/debian:11 --shared'
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload cirros /srv/ci/cirros --shared'
 
-      - name: Create a base level of activity in the cluster
-        run: |
-          . ${GITHUB_WORKSPACE}/ci-environment.sh
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary \
-              'echo "==== sfrc ===="; cat /etc/sf/sfrc; echo "==== end sfrc ===="'
-          echo ""
-          echo ""
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary \
-              '. /etc/sf/sfrc; for i in `seq 100`; do sf-client --async=continue network create background-$i 10.$i.0.0/24 > /dev/null; echo -n "."; done'
-          echo ""
-
-      - name: Run functional tests
+      - name: Run ansible module tests
+        timeout-minutes: 120
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               $source_path/shakenfist \
               debian@$primary:shakenfist
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=3"
+              debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; bash ansiblemoduletests.sh"
 
       - name: Check logs
-        if: ${{ ! cancelled() }}
+        if: always()
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
                 -o UserKnownHostsFile=/dev/null \
                 debian@$primary sudo chmod ugo+r /var/log/syslog
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
@@ -151,25 +141,41 @@
           etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
           echo "This CI run created $etcd_conns etcd connections."
           if [ $etcd_conns -gt 5000 ]; then
             echo "FAILURE: Too many etcd clients!"
             failures=1
           fi
 
+          echo
+          sigterms=`grep -c "Sent SIGTERM to " ${GITHUB_WORKSPACE}/syslog || true`
+          echo "This CI run sent $sigterms SIGTERM signals while shutting down."
+          if [ $sigterms -gt 50 ]; then
+            echo "FAILURE: Too many SIGTERMs sent!"
+            failures=1
+          fi
+
           FORBIDDEN=("Traceback (most recent call last):"
                      "ERROR sf"
+                     "ERROR gunicorn"
                      " died"
                      "Extra vxlan present"
                      "Fork support is only compatible with the epoll1 and poll polling strategies"
                      "not using configured address"
                      "Dumping thread traces"
                      "because it is leased to"
                      "not committing online upgrade"
                      "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
-                     "ConnectionFailedError")
+                     "ConnectionFailedError"
+                     "invalid JWT in Authorization header"
+                     "Libvirt Error: XML error"
+                     "Cleaning up leaked IPAM"
+                     "Cleaning up leaked vxlan"
+                     "Waiting to acquire lock"
+                     'apparmor="DENIED"'
+                     "Ignoring malformed cache entry")
           IFS=""
           for forbid in ${FORBIDDEN[*]}
           do
             if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
             then
               echo "FAILURE: Forbidden string found in logs: $forbid"
               failures=1
@@ -177,47 +183,47 @@
           done
 
           if [ $failures -gt 0 ]; then
               echo "...failures detected."
               exit 1
           fi
 
-      - name: Gather logs
-        if: ${{ ! cancelled() }}
+      - name: Check process CPU usage
+        if: always()
         run: |
-          set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              debian@$primary '. /etc/sf/sfrc; sf-client node cpuhogs'
 
-          cd ${GITHUB_WORKSPACE}
-          rm -rf artifacts bundle
-          mkdir -p artifacts bundle
+      - name: Fetch and tweak inventory
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              debian@$primary:/etc/sf/inventory.yaml /srv/github/
+          sed -i 's|/root/.ssh|/home/debian/.ssh|g' /srv/github/inventory.yaml
 
-          echo "=============================="
-          for node in $nodes
-          do
-            echo "=== $node ==="
-            safe_node=$(echo $node | tr "-" "_")
+          echo "====="
+          cat /srv/github/inventory.yaml
 
-            ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                debian@${!safe_node} sudo /srv/shakenfist/venv/bin/clingwrap gather \
-                --target /srv/shakenfist/venv/share/clingwrap/shakenfist-ci-failure.cwd --output /tmp/$node.zip
-            scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                debian@${!safe_node}:/tmp/$node.zip bundle/
-
-            mkdir -p bundle/$node
-
-            # We ignore the exit code of unzip, as it will return 1 if a warning is
-            # emitted during expansion, even though expansion worked correctly. For
-            # example stripping a leading / from paths.
-            unzip -q bundle/$node.zip -d bundle/$node/ || true
-            rm bundle/$node.zip
-          done
+      - name: Gather logs
+        if: always()
+        run: |
+          set -x
 
-          zip -rq artifacts/bundle.zip bundle/*
+          # We need the ssh key in the place ansible expects it to be, which isn't
+          # true on the CI worker node.
+          cp /srv/github/id_ci /home/debian/.ssh/id_rsa
+          cp /srv/github/id_ci.pub /home/debian/.ssh/id_rsa.pub
+          chown -R debian.debian /home/debian/.ssh
+
+          ansible-playbook -i /srv/github/inventory.yaml \
+              --extra-vars "base_image_user=debian ansible_ssh_common_args='-o StrictHostKeyChecking=no'" \
+              ${GITHUB_WORKSPACE}/shakenfist/deploy/ansible/ci-gather-logs.yml
 
-      - uses: actions/upload-artifact@v3
-        if: ${{ ! cancelled() }}
+      - uses: actions/upload-artifact@v4
+        if: always()
         with:
           name: bundle.zip
           retention-days: 90
           if-no-files-found: error
-          path: ${{ github.workspace }}/artifacts/bundle.zip
+          path: /srv/github/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-debian-11-slim-primary.yml` & `shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-debian-11-slim-primary.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     branches:
       - develop
       - v*-releases
 
 jobs:
   debian-11-slim-primary:
     runs-on: self-hosted
-    timeout-minutes: 120
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
       cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
@@ -43,24 +42,27 @@
         run: |
           cd ${GITHUB_WORKSPACE}/shakenfist
           ansible-playbook -i /home/debian/ansible-hosts \
               --extra-vars "identifier=${SHAKENFIST_NAMESPACE} source_path=${GITHUB_WORKSPACE} \
               base_image=sf://label/ci-images/debian-11 base_image_user=debian" \
               deploy/ansible/ci-topology-slim-primary.yml
 
-      - name: Log github actions buffering status
+      - name: Copy CI tools to primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           cd ${GITHUB_WORKSPACE}/shakenfist
           scp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              tools/buffer.py debian@$primary:buffer.py
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              debian@$primary python3 buffer.py
+              -o UserKnownHostsFile=/dev/null -rp tools \
+              debian@$primary:.
+
+      - name: Log github actions buffering status
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} python3 tools/buffer.py
 
       - name: Run getsf installer on primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               debian@$primary /tmp/getsf-wrapper
@@ -73,15 +75,15 @@
 
       - name: Wait for API to start answering
         run: |
           set +e
 
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary 'sudo chmod ugo+r /etc/sf/sfrc /etc/sf/shakenfist.json /var/log/syslog'
+              debian@$primary 'sudo chmod ugo+r /etc/sf/* /var/log/syslog'
 
           count=0
           while [ $count -lt 60 ]
           do
             ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary '. /etc/sf/sfrc; sf-client instance list'
             if [ $? == 0 ]; then
@@ -120,104 +122,73 @@
           echo ""
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary \
               '. /etc/sf/sfrc; for i in `seq 100`; do sf-client --async=continue network create background-$i 10.$i.0.0/24 > /dev/null; echo -n "."; done'
           echo ""
 
       - name: Run functional tests
+        timeout-minutes: 120
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               $source_path/shakenfist \
               debian@$primary:shakenfist
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=5"
+              debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; set -e; stestr run --concurrency=5; stestr slowest"
 
       - name: Check logs
-        if: ${{ ! cancelled() }}
+        if: always()
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-                -o UserKnownHostsFile=/dev/null \
-                debian@$primary sudo chmod ugo+r /var/log/syslog
-          scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              debian@$primary:/var/log/syslog \
-              ${GITHUB_WORKSPACE}/syslog
-
-          failures=0
-
-          echo
-          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
-          echo "This CI run created $etcd_conns etcd connections."
-          if [ $etcd_conns -gt 5000 ]; then
-            echo "FAILURE: Too many etcd clients!"
-            failures=1
-          fi
-
-          FORBIDDEN=("Traceback (most recent call last):"
-                     "ERROR sf"
-                     " died"
-                     "Extra vxlan present"
-                     "Fork support is only compatible with the epoll1 and poll polling strategies"
-                     "not using configured address"
-                     "Dumping thread traces"
-                     "because it is leased to"
-                     "not committing online upgrade"
-                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
-                     "ConnectionFailedError")
-          IFS=""
-          for forbid in ${FORBIDDEN[*]}
-          do
-            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
-            then
-              echo "FAILURE: Forbidden string found in logs: $forbid"
-              failures=1
-            fi
-          done
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          if [ $failures -gt 0 ]; then
-              echo "...failures detected."
-              exit 1
-          fi
+      # On Ubuntu 22.04 the cleaner is rated a CPU hog because of etcd cleanup
+      # cost. That's not really something we can control, so just ignore the CPU
+      # usage of that process instead.
+      - name: Check SF process CPU usage
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              debian@$primary '. /etc/sf/sfrc; sf-client node cpuhogs --ignore sf_cleaner'
 
-      - name: Gather logs
-        if: ${{ ! cancelled() }}
+      - name: Check for reasonable data rates
+        if: always()
         run: |
-          set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          cd ${GITHUB_WORKSPACE}
-          rm -rf artifacts bundle
-          mkdir -p artifacts bundle
+      - name: Fetch and tweak inventory
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              debian@$primary:/etc/sf/inventory.yaml /srv/github/
+          sed -i 's|/root/.ssh|/home/debian/.ssh|g' /srv/github/inventory.yaml
 
-          echo "=============================="
-          for node in $nodes
-          do
-            echo "=== $node ==="
-            safe_node=$(echo $node | tr "-" "_")
+          echo "====="
+          cat /srv/github/inventory.yaml
 
-            ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                debian@${!safe_node} sudo /srv/shakenfist/venv/bin/clingwrap gather \
-                --target /srv/shakenfist/venv/share/clingwrap/shakenfist-ci-failure.cwd --output /tmp/$node.zip
-            scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                debian@${!safe_node}:/tmp/$node.zip bundle/
-
-            mkdir -p bundle/$node
-
-            # We ignore the exit code of unzip, as it will return 1 if a warning is
-            # emitted during expansion, even though expansion worked correctly. For
-            # example stripping a leading / from paths.
-            unzip -q bundle/$node.zip -d bundle/$node/ || true
-            rm bundle/$node.zip
-          done
+      - name: Gather logs
+        if: always()
+        run: |
+          set -x
 
-          zip -rq artifacts/bundle.zip bundle/*
+          # We need the ssh key in the place ansible expects it to be, which isn't
+          # true on the CI worker node.
+          cp /srv/github/id_ci /home/debian/.ssh/id_rsa
+          cp /srv/github/id_ci.pub /home/debian/.ssh/id_rsa.pub
+
+          ansible-playbook -i /srv/github/inventory.yaml \
+              --extra-vars "base_image_user=debian ansible_ssh_common_args='-o StrictHostKeyChecking=no'" \
+              ${GITHUB_WORKSPACE}/shakenfist/deploy/ansible/ci-gather-logs.yml
 
-      - uses: actions/upload-artifact@v3
-        if: ${{ ! cancelled() }}
+      - uses: actions/upload-artifact@v4
+        if: always()
         with:
           name: bundle.zip
           retention-days: 90
           if-no-files-found: error
-          path: ${{ github.workspace }}/artifacts/bundle.zip
+          path: /srv/github/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml` & `shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     branches:
       - develop
       - v*-releases
 
 jobs:
   ubuntu-2004-slim-primary:
     runs-on: self-hosted
-    timeout-minutes: 120
     concurrency:
       group: ${{ github.workflow }}-${{ github.ref }}
       cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
@@ -43,24 +42,27 @@
         run: |
           cd ${GITHUB_WORKSPACE}/shakenfist
           ansible-playbook -i /home/debian/ansible-hosts \
               --extra-vars "identifier=${SHAKENFIST_NAMESPACE} source_path=${GITHUB_WORKSPACE} \
               base_image=sf://label/ci-images/ubuntu-2004 base_image_user=ubuntu" \
               deploy/ansible/ci-topology-slim-primary.yml
 
-      - name: Log github actions buffering status
+      - name: Copy CI tools to primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           cd ${GITHUB_WORKSPACE}/shakenfist
           scp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              tools/buffer.py ubuntu@$primary:buffer.py
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              ubuntu@$primary python3 buffer.py
+              -o UserKnownHostsFile=/dev/null -rp tools \
+              ubuntu@$primary:.
+
+      - name: Log github actions buffering status
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} python3 tools/buffer.py
 
       - name: Run getsf installer on primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               ubuntu@$primary /tmp/getsf-wrapper
@@ -73,15 +75,15 @@
 
       - name: Wait for API to start answering
         run: |
           set +e
 
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              ubuntu@$primary 'sudo chmod ugo+r /etc/sf/sfrc /etc/sf/shakenfist.json /var/log/syslog'
+              ubuntu@$primary 'sudo chmod ugo+r /etc/sf/* /var/log/syslog'
 
           count=0
           while [ $count -lt 60 ]
           do
             ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               ubuntu@$primary '. /etc/sf/sfrc; sf-client instance list'
             if [ $? == 0 ]; then
@@ -120,104 +122,73 @@
           echo ""
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               ubuntu@$primary \
               '. /etc/sf/sfrc; for i in `seq 100`; do sf-client --async=continue network create background-$i 10.$i.0.0/24 > /dev/null; echo -n "."; done'
           echo ""
 
       - name: Run functional tests
+        timeout-minutes: 120
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               $source_path/shakenfist \
               ubuntu@$primary:shakenfist
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              ubuntu@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=5"
+              ubuntu@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; set -e; stestr run --concurrency=5; stestr slowest"
 
       - name: Check logs
-        if: ${{ ! cancelled() }}
+        if: always()
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-                -o UserKnownHostsFile=/dev/null \
-                ubuntu@$primary sudo chmod ugo+r /var/log/syslog
-          scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              ubuntu@$primary:/var/log/syslog \
-              ${GITHUB_WORKSPACE}/syslog
-
-          failures=0
-
-          echo
-          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
-          echo "This CI run created $etcd_conns etcd connections."
-          if [ $etcd_conns -gt 5000 ]; then
-            echo "FAILURE: Too many etcd clients!"
-            failures=1
-          fi
-
-          FORBIDDEN=("Traceback (most recent call last):"
-                     "ERROR sf"
-                     " died"
-                     "Extra vxlan present"
-                     "Fork support is only compatible with the epoll1 and poll polling strategies"
-                     "not using configured address"
-                     "Dumping thread traces"
-                     "because it is leased to"
-                     "not committing online upgrade"
-                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
-                     "ConnectionFailedError")
-          IFS=""
-          for forbid in ${FORBIDDEN[*]}
-          do
-            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
-            then
-              echo "FAILURE: Forbidden string found in logs: $forbid"
-              failures=1
-            fi
-          done
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          if [ $failures -gt 0 ]; then
-              echo "...failures detected."
-              exit 1
-          fi
+      # On Ubuntu 22.04 the cleaner is rated a CPU hog because of etcd cleanup
+      # cost. That's not really something we can control, so just ignore the CPU
+      # usage of that process instead.
+      - name: Check SF process CPU usage
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              ubuntu@$primary '. /etc/sf/sfrc; sf-client node cpuhogs --ignore sf_cleaner'
 
-      - name: Gather logs
-        if: ${{ ! cancelled() }}
+      - name: Check for reasonable data rates
+        if: always()
         run: |
-          set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          cd ${GITHUB_WORKSPACE}
-          rm -rf artifacts bundle
-          mkdir -p artifacts bundle
+      - name: Fetch and tweak inventory
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              ubuntu@$primary:/etc/sf/inventory.yaml /srv/github/
+          sed -i 's|/root/.ssh|/home/debian/.ssh|g' /srv/github/inventory.yaml
 
-          echo "=============================="
-          for node in $nodes
-          do
-            echo "=== $node ==="
-            safe_node=$(echo $node | tr "-" "_")
+          echo "====="
+          cat /srv/github/inventory.yaml
 
-            ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                ubuntu@${!safe_node} sudo /srv/shakenfist/venv/bin/clingwrap gather \
-                --target /srv/shakenfist/venv/share/clingwrap/shakenfist-ci-failure.cwd --output /tmp/$node.zip
-            scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                ubuntu@${!safe_node}:/tmp/$node.zip bundle/
-
-            mkdir -p bundle/$node
-
-            # We ignore the exit code of unzip, as it will return 1 if a warning is
-            # emitted during expansion, even though expansion worked correctly. For
-            # example stripping a leading / from paths.
-            unzip -q bundle/$node.zip -d bundle/$node/ || true
-            rm bundle/$node.zip
-          done
+      - name: Gather logs
+        if: always()
+        run: |
+          set -x
 
-          zip -rq artifacts/bundle.zip bundle/*
+          # We need the ssh key in the place ansible expects it to be, which isn't
+          # true on the CI worker node.
+          cp /srv/github/id_ci /home/debian/.ssh/id_rsa
+          cp /srv/github/id_ci.pub /home/debian/.ssh/id_rsa.pub
+
+          ansible-playbook -i /srv/github/inventory.yaml \
+              --extra-vars "base_image_user=ubuntu ansible_ssh_common_args='-o StrictHostKeyChecking=no'" \
+              ${GITHUB_WORKSPACE}/shakenfist/deploy/ansible/ci-gather-logs.yml
 
-      - uses: actions/upload-artifact@v3
-        if: ${{ ! cancelled() }}
+      - uses: actions/upload-artifact@v4
+        if: always()
         with:
           name: bundle.zip
           retention-days: 90
           if-no-files-found: error
-          path: ${{ github.workspace }}/artifacts/bundle.zip
+          path: /srv/github/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc7/.github/workflows/functional-tests.tmpl` & `shakenfist-client-0.7.0.0rc8/.github/workflows/functional-tests-ubuntu-2204-slim-primary.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-name: Test {{name}}
+name: Test ubuntu-2204-slim-primary
 
 on:
   push:
     branches:
       - develop
       - v*-releases
   pull_request:
     branches:
       - develop
       - v*-releases
 
 jobs:
-  {{name}}:
+  ubuntu-2204-slim-primary:
     runs-on: self-hosted
-    timeout-minutes: 120
     concurrency:
-      group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
+      group: ${{ github.workflow }}-${{ github.ref }}
       cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
 
     steps:
       - name: Set environment variables
         run: |
-          echo "SF_HEAD_SHA={% raw %}${{{% endraw %} github.event.pull_request.head.sha {% raw %}}}{% endraw %}" >> $GITHUB_ENV
-          echo "SF_PRIMARY_REPO=$( echo {% raw %}${{{% endraw %} github.repository {% raw %}}}{% endraw %} | cut -f 2 -d '/' )" >> $GITHUB_ENV
+          echo "SF_HEAD_SHA=${{ github.event.pull_request.head.sha }}" >> $GITHUB_ENV
+          echo "SF_PRIMARY_REPO=$( echo ${{ github.repository }} | cut -f 2 -d '/' )" >> $GITHUB_ENV
           echo "SHAKENFIST_NAMESPACE=$(hostname)" >> $GITHUB_ENV
 
       - name: Checkout client-python
         uses: actions/checkout@v3
         with:
           path: client-python
           fetch-depth: 0
@@ -40,184 +39,156 @@
           python3 ${GITHUB_WORKSPACE}/client-python/tools/clone_with_depends.py
 
       - name: Build infrastructure
         run: |
           cd ${GITHUB_WORKSPACE}/shakenfist
           ansible-playbook -i /home/debian/ansible-hosts \
               --extra-vars "identifier=${SHAKENFIST_NAMESPACE} source_path=${GITHUB_WORKSPACE} \
-              base_image={{baseimage}} base_image_user={{baseuser}}" \
-              deploy/ansible/ci-topology-{{topology}}.yml
+              base_image=sf://label/ci-images/ubuntu-2204 base_image_user=ubuntu" \
+              deploy/ansible/ci-topology-slim-primary.yml
 
-      - name: Log github actions buffering status
+      - name: Copy CI tools to primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           cd ${GITHUB_WORKSPACE}/shakenfist
           scp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              tools/buffer.py {{baseuser}}@$primary:buffer.py
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary python3 buffer.py
+              -o UserKnownHostsFile=/dev/null -rp tools \
+              ubuntu@$primary:.
+
+      - name: Log github actions buffering status
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} python3 tools/buffer.py
 
       - name: Run getsf installer on primary
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary /tmp/getsf-wrapper
+              ubuntu@$primary /tmp/getsf-wrapper
           echo ""
           echo ""
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               'sudo rm /etc/apache2/sites-enabled/*; sudo a2ensite sf-example.conf; sudo apachectl graceful'
 
       - name: Wait for API to start answering
         run: |
           set +e
 
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary 'sudo chmod ugo+r /etc/sf/sfrc /etc/sf/shakenfist.json /var/log/syslog'
+              ubuntu@$primary 'sudo chmod ugo+r /etc/sf/* /var/log/syslog'
 
           count=0
           while [ $count -lt 60 ]
           do
             ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary '. /etc/sf/sfrc; sf-client instance list'
+              ubuntu@$primary '. /etc/sf/sfrc; sf-client instance list'
             if [ $? == 0 ]; then
               exit 0
             fi
 
             count=$(( $count + 1 ))
             sleep 5
           done
 
           exit 1
 
       - name: Import cached images
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload ubuntu-1804 /srv/ci/ubuntu:18.04 --shared'
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload ubuntu-2004 /srv/ci/ubuntu:20.04 --shared'
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload debian-11 /srv/ci/debian:11 --shared'
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               '. /etc/sf/sfrc; sf-client artifact upload cirros /srv/ci/cirros --shared'
 
       - name: Create a base level of activity in the cluster
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               'echo "==== sfrc ===="; cat /etc/sf/sfrc; echo "==== end sfrc ===="'
           echo ""
           echo ""
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary \
+              ubuntu@$primary \
               '. /etc/sf/sfrc; for i in `seq 100`; do sf-client --async=continue network create background-$i 10.$i.0.0/24 > /dev/null; echo -n "."; done'
           echo ""
 
       - name: Run functional tests
+        timeout-minutes: 120
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               $source_path/shakenfist \
-              {{baseuser}}@$primary:shakenfist
+              ubuntu@$primary:shakenfist
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency={{concurrency}}"
+              ubuntu@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; set -e; stestr run --concurrency=5; stestr slowest"
 
       - name: Check logs
-        if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
+        if: always()
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
-          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-                -o UserKnownHostsFile=/dev/null \
-                {{baseuser}}@$primary sudo chmod ugo+r /var/log/syslog
-          scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
-              -o UserKnownHostsFile=/dev/null \
-              {{baseuser}}@$primary:/var/log/syslog \
-              ${GITHUB_WORKSPACE}/syslog
-
-          failures=0
-
-          echo
-          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
-          echo "This CI run created $etcd_conns etcd connections."
-          if [ $etcd_conns -gt 5000 ]; then
-            echo "FAILURE: Too many etcd clients!"
-            failures=1
-          fi
-
-          FORBIDDEN=("Traceback (most recent call last):"
-                     "ERROR sf"
-                     " died"
-                     "Extra vxlan present"
-                     "Fork support is only compatible with the epoll1 and poll polling strategies"
-                     "not using configured address"
-                     "Dumping thread traces"
-                     "because it is leased to"
-                     "not committing online upgrade"
-                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
-                     "ConnectionFailedError")
-          IFS=""
-          for forbid in ${FORBIDDEN[*]}
-          do
-            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
-            then
-              echo "FAILURE: Forbidden string found in logs: $forbid"
-              failures=1
-            fi
-          done
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          if [ $failures -gt 0 ]; then
-              echo "...failures detected."
-              exit 1
-          fi
+      # On Ubuntu 22.04 the cleaner is rated a CPU hog because of etcd cleanup
+      # cost. That's not really something we can control, so just ignore the CPU
+      # usage of that process instead.
+      - name: Check SF process CPU usage
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              ubuntu@$primary '. /etc/sf/sfrc; sf-client node cpuhogs --ignore sf_cleaner'
 
-      - name: Gather logs
-        if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
+      - name: Check for reasonable data rates
+        if: always()
         run: |
-          set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          cd ${GITHUB_WORKSPACE}/shakenfist
+          tools/run_remote ${primary} sudo /home/${baseuser}/tools/ci_event_checks.sh
 
-          cd ${GITHUB_WORKSPACE}
-          rm -rf artifacts bundle
-          mkdir -p artifacts bundle
+      - name: Fetch and tweak inventory
+        if: always()
+        run: |
+          . ${GITHUB_WORKSPACE}/ci-environment.sh
+          scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
+              ubuntu@$primary:/etc/sf/inventory.yaml /srv/github/
+          sed -i 's|/root/.ssh|/home/debian/.ssh|g' /srv/github/inventory.yaml
 
-          echo "=============================="
-          for node in $nodes
-          do
-            echo "=== $node ==="
-            safe_node=$(echo $node | tr "-" "_")
+          echo "====="
+          cat /srv/github/inventory.yaml
 
-            ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                {{baseuser}}@${!safe_node} sudo /srv/shakenfist/venv/bin/clingwrap gather \
-                --target /srv/shakenfist/venv/share/clingwrap/shakenfist-ci-failure.cwd --output /tmp/$node.zip
-            scp -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
-                {{baseuser}}@${!safe_node}:/tmp/$node.zip bundle/
-
-            mkdir -p bundle/$node
-
-            # We ignore the exit code of unzip, as it will return 1 if a warning is
-            # emitted during expansion, even though expansion worked correctly. For
-            # example stripping a leading / from paths.
-            unzip -q bundle/$node.zip -d bundle/$node/ || true
-            rm bundle/$node.zip
-          done
+      - name: Gather logs
+        if: always()
+        run: |
+          set -x
 
-          zip -rq artifacts/bundle.zip bundle/*
+          # We need the ssh key in the place ansible expects it to be, which isn't
+          # true on the CI worker node.
+          cp /srv/github/id_ci /home/debian/.ssh/id_rsa
+          cp /srv/github/id_ci.pub /home/debian/.ssh/id_rsa.pub
+
+          ansible-playbook -i /srv/github/inventory.yaml \
+              --extra-vars "base_image_user=ubuntu ansible_ssh_common_args='-o StrictHostKeyChecking=no'" \
+              ${GITHUB_WORKSPACE}/shakenfist/deploy/ansible/ci-gather-logs.yml
 
-      - uses: actions/upload-artifact@v3
-        if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
+      - uses: actions/upload-artifact@v4
+        if: always()
         with:
           name: bundle.zip
           retention-days: 90
           if-no-files-found: error
-          path: {% raw %}${{{% endraw %} github.workspace {% raw %}}}{% endraw %}/artifacts/bundle.zip
+          path: /srv/github/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc7/LICENSE` & `shakenfist-client-0.7.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/PKG-INFO` & `shakenfist-client-0.7.0.0rc8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc7
+Version: 0.7.0.0rc8
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc7/ansible/sf_network.py` & `shakenfist-client-0.7.0.0rc8/ansible/sf_snapshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,147 +6,125 @@
 import json
 
 from ansible.module_utils.basic import AnsibleModule
 
 
 DOCUMENTATION = """
 ---
-module: sf_network
-short_description: Create and delete Shaken Fist networks.
+module: sf_snapshot
+short_description: Create and delete Shaken Fist instance snapshots.
 """
 
 EXAMPLES = """
-- name: Create Shaken Fist network
-  sf_network:
-    netblock: '192.168.242.0/24'
-    name: 'mynet'
+- name: Snapshot just the primary disk a Shaken Fist instance
+  sf_snapshot:
+    instance_uuid: '9cd9ca86-0dd4-4ddd-aa28-822855ea4318'
+    state: present
   register: result
 
-- name: Delete that network
-  sf_network:
-    uuid: '1ebc5020-6cfd-4641-8f3b-175596a19de0'
-    state: absent
+- name: Snapshot all disks on a Shaken Fist instance, without blocking
+  sf_snapshot:
+    instance_uuid: '9cd9ca86-0dd4-4ddd-aa28-822855ea4318'
+    all: true
+    async: true
+    state: present
   register: result
 
-- name: Create Shaken Fist network in different namespace
-  sf_network:
-    netblock: '192.168.242.0/24'
-    name: 'mynet'
-    namespace: 'mynamespace'
+- name: Snapshot and update the "ciimage" label
+  sf_snapshot:
+    instance_uuid: '9cd9ca86-0dd4-4ddd-aa28-822855ea4318'
+    label: ciimage
+    state: present
+  register: result
 """
 
 
 def error(message):
     return True, False, {'error': message}
 
 
 def present(module):
-    for required in ['name', 'netblock']:
-        if not module.params.get(required):
-            return error('You must specify a %s when creating an instance' % required)
-
-    params = {}
-    for key in ['name', 'netblock']:
-        params[key] = module.params.get(key)
+    if not module.params.get('instance_uuid'):
+        return error('You must specify an instance_uuid when creating an instance')
+
+    params = {
+        'instance_uuid': module.params.get('instance_uuid')
+    }
+
+    extra = ''
+    if module.params.get('all', False):
+        extra += ' --all'
+    if module.params.get('label'):
+        extra += ' --label_name %s' % module.params['label']
+    if module.params.get('delete_after_label', False):
+        extra += ' --delete-snapshot-after-label'
+    params['extra'] = extra
 
     params['async_strategy'] = 'block'
     if module.params.get('async'):
         params['async_strategy'] = 'continue'
 
     cmd = ('sf-client --json --async=%(async_strategy)s '
-           'network create %(name)s %(netblock)s'
-           % params)
-    if 'namespace' in module.params and module.params['namespace']:
-        cmd += ' --namespace ' + module.params['namespace']
-
-    if 'nat' in module.params and not module.params['nat']:
-        cmd += ' --no-nat'
-    if 'dhcp' in module.params and not module.params['dhcp']:
-        cmd += ' --no-dhcp'
-
+           'instance snapshot %(instance_uuid)s %(extra)s' % params)
     rc, stdout, stderr = module.run_command(
         cmd, check_rc=False, use_unsafe_shell=True)
     if rc != 0:
         return True, False, 'Command failed: %s' % stderr
 
-    try:
-        j = json.loads(stdout)
-    except ValueError:
-        rc = -1
-        j = ('Failed to parse JSON:\n'
-             '[[command: %s]]\n'
-             '[[stdout: %s]]\n'
-             '[[stderr: %s]]'
-             % (cmd, stdout, stderr))
-
+    j = json.loads(stdout)
     if rc != 0:
         return True, False, j
-
     return False, True, j
 
 
 def absent(module):
     if not module.params.get('uuid'):
-        return error('You must specify a uuid when deleting a network')
+        return error('You must specify a uuid when deleting a snapshot')
 
-    cmd = ('sf-client --json --async=block network delete %(uuid)s' %
-           module.params)
-    if 'namespace' in module.params and module.params['namespace']:
-        cmd += ' --namespace ' + module.params['namespace']
+    cmd = ('sf-client --json --async=block artifact delete %(uuid)s'
+           % module.params)
 
     rc, stdout, stderr = module.run_command(
         cmd, check_rc=False, use_unsafe_shell=True)
     if rc != 0:
         return True, False, 'Command failed: %s' % stderr
 
-    try:
-        j = json.loads(stdout)
-    except ValueError:
-        rc = -1
-        j = ('Failed to parse JSON:\n'
-             '[[command: %s]]\n'
-             '[[stdout: %s]]\n'
-             '[[stderr: %s]]'
-             % (cmd, stdout, stderr))
-
-    if rc != 0:
-        return True, False, j
-
-    return False, True, j
+    return False, True, None
 
 
 def main():
 
     fields = {
         'uuid': {'required': False, 'type': 'str'},
-        'netblock': {'required': False, 'type': 'str'},
-        'name': {'required': False, 'type': 'str'},
-        'namespace': {'type': 'str'},
-        'nat': {'required': False, 'type': 'bool', 'default': True},
-        'dhcp': {'required': False, 'type': 'bool', 'default': True},
+        'instance_uuid': {'required': False, 'type': 'str'},
+        'all': {'required': False, 'type': 'bool'},
+        'label': {'required': False, 'type': 'str'},
+        'delete_after_label': {'required': False, 'type': 'bool'},
 
         'async': {'required': False, 'type': 'bool'},
 
         'state': {
             'default': 'present',
             'choices': ['present', 'absent'],
             'type': 'str'
         },
     }
 
     choice_map = {
         'present': present,
-        'absent': absent,
+        'absent': absent
     }
 
     module = AnsibleModule(argument_spec=fields)
     is_error, has_changed, result = choice_map.get(
         module.params['state'])(module)
 
     if not is_error:
         module.exit_json(changed=has_changed, meta=result)
     else:
-        module.fail_json(msg='Error manipulating network', meta=result)
+        module.fail_json(msg='Error manipulating artifact',
+                         params=module.params,
+                         meta=result)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shakenfist-client-0.7.0.0rc7/release.sh` & `shakenfist-client-0.7.0.0rc8/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/setup.cfg` & `shakenfist-client-0.7.0.0rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/setup.py` & `shakenfist-client-0.7.0.0rc8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     setup_requires=['pbr'],
     pbr=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     data_files=[
         (
             'share/shakenfist/ansible', [
-                'ansible/sf_instance.py',
-                'ansible/sf_network.py',
+                'ansible/sf_instance',
+                'ansible/sf_namespace',
+                'ansible/sf_network',
                 'ansible/sf_snapshot.py'
             ]
         )
     ],
 )
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/apiclient.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/apiclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,15 @@
                  async_strategy=ASYNC_BLOCK):
         global LOG
         if verbose:
             LOG.setLevel(logging.DEBUG)
         if logger:
             LOG = logger
 
+        self.most_recent_request_id = None
         self.sync_request_timeout = sync_request_timeout
 
         LOG.debug('Client initially configured with apiurl of %s for namespace %s '
                   'and async strategy %s'
                   % (base_url, namespace, async_strategy))
 
         if not suppress_configuration_lookup:
@@ -188,41 +189,52 @@
 
     def _actual_request_url(self, method, url, data=None,
                             request_body_is_binary=False,
                             response_body_is_binary=False,
                             allow_redirects=True, stream=False):
         url = self.base_url + url
 
-        h = {'Authorization': self.cached_auth,
-             'User-Agent': get_user_agent()}
+        h = {
+                'Authorization': self.cached_auth,
+                'User-Agent': get_user_agent()
+            }
         if data:
             if request_body_is_binary:
                 h['Content-Type'] = 'application/octet-stream'
             else:
                 h['Content-Type'] = 'application/json'
                 data = json.dumps(data, indent=4, sort_keys=True)
 
         start_time = time.time()
         r = requests.request(method, url, data=data, headers=h,
                              allow_redirects=allow_redirects, stream=stream)
         end_time = time.time()
 
         LOG.debug('-------------------------------------------------------')
         LOG.debug('API client requested: %s %s' % (method, url))
+        for hkey in h:
+            if hkey == 'Authorization' and h[hkey]:
+                LOG.debug('Header: Authorization = Bearer *****')
+            else:
+                LOG.debug('Header: %s = %s' % (hkey, h[hkey]))
         if data:
             if request_body_is_binary:
                 LOG.debug('Data: ...%d bytes of binary omitted...' % len(data))
             else:
                 LOG.debug('Data:\n    %s' % '\n    '.join(data.split('\n')))
         for h in r.history:
             LOG.debug('URL request history: %s --> %s %s'
                       % (h.url, h.status_code, h.headers.get('Location')))
         LOG.debug('API client response: code = %s (took %.02f seconds)'
                   % (r.status_code, (end_time - start_time)))
 
+        self.most_recent_request_id = r.headers.get('X-Request-ID')
+        for hkey in r.headers:
+            LOG.debug('Header: %s = %s' % (hkey, r.headers[hkey]))
+
         if not stream and r.text:
             if response_body_is_binary:
                 LOG.debug('Data: ...%d bytes of binary omitted...'
                           % len(r.text))
             else:
                 try:
                     LOG.debug('Data:\n    %s'
@@ -438,16 +450,24 @@
                 inst = self.get_instance(uuid)
                 if not inst or inst['state'] == 'deleted':
                     LOG.debug('Instance %s is now deleted' % uuid)
                     waiting_for.remove(uuid)
 
         return deleted
 
-    def get_instance(self, instance_ref):
-        r = self._request_url('GET', '/instances/' + instance_ref)
+    def get_instance(self, instance_ref, namespace=None):
+        if namespace and not self.check_capability('get-instance-namespace'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'lookup of instances with a specific namespace.')
+
+        data = None
+        if namespace:
+            data = {'namespace': namespace}
+        r = self._request_url('GET', '/instances/' + instance_ref, data=data)
         return r.json()
 
     def get_instance_interfaces(self, instance_ref):
         r = self._request_url('GET', '/instances/' + instance_ref +
                               '/interfaces')
         return r.json()
 
@@ -483,16 +503,15 @@
         clean_disks = []
         for d in disk:
             if 'size' in d and d['size']:
                 d['size'] = int(d['size'])
             clean_disks.append(d)
         body['disk'] = clean_disks
 
-        r = self._request_url('POST', '/instances',
-                              data=body)
+        r = self._request_url('POST', '/instances', data=body)
         i = r.json()
 
         deadline = time.time() + _calculate_async_deadline(self.async_strategy)
         while True:
             if i['state'] not in ['initial', 'creating']:
                 return i
 
@@ -553,21 +572,26 @@
         return out
 
     def get_instance_snapshots(self, instance_ref):
         r = self._request_url('GET', '/instances/' + instance_ref +
                               '/snapshot')
         return r.json()
 
-    def get_instance_agentoperations(self, instance_ref):
+    def get_instance_agentoperations(self, instance_ref, all=False):
         if not self.check_capability('instance-agentoperations'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'looking up the agent operations for an instance.')
+        if all and not self.check_capability('instance-agentoperations-all'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'looking up all agent operations for an instance.')
+
         r = self._request_url('GET', '/instances/' + instance_ref +
-                              '/agentoperation')
+                              '/agentoperations', data={'all': all})
         return r.json()
 
     def update_label(self, label_name, blob_uuid):
         r = self._request_url(
             'POST', '/label/%s' % label_name, data={'blob_uuid': blob_uuid})
         return _correct_blob_indexes(r.json())
 
@@ -741,16 +765,24 @@
         r = self._request_url('GET', '/blobs', data={'node': node})
         return r.json()
 
     def get_networks(self, all=False):
         r = self._request_url('GET', '/networks', data={'all': all})
         return r.json()
 
-    def get_network(self, network_ref):
-        r = self._request_url('GET', '/networks/' + network_ref)
+    def get_network(self, network_ref, namespace=None):
+        if namespace and not self.check_capability('get-network-namespace'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'lookup of networks with a specific namespace.')
+
+        data = None
+        if namespace:
+            data = {'namespace': namespace}
+        r = self._request_url('GET', '/networks/' + network_ref, data=data)
         return r.json()
 
     def delete_network(self, network_ref, namespace=None):
         # Why pass a namespace when you're passing an exact UUID? The idea here
         # is that it provides a consistent interface, but also a safety check
         # against overly zealous loops deleting things.
         data = None
@@ -788,16 +820,43 @@
                 LOG.debug('Deadline exceeded waiting for network to be created')
                 return n
 
             time.sleep(1)
             n = self.get_network(n['uuid'])
 
     def get_network_interfaces(self, network_ref):
-        r = self._request_url('GET', '/networks/' +
-                              network_ref + '/interfaces')
+        r = self._request_url('GET', '/networks/' + network_ref + '/interfaces')
+        return r.json()
+
+    def get_network_addresses(self, network_ref):
+        if not self.check_capability('list-addresses'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'listing network addresses.')
+
+        r = self._request_url('GET', '/networks/' + network_ref + '/addresses')
+        return r.json()
+
+    def route_network_address(self, network_ref):
+        if not self.check_capability('route-addresses'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'routing addresses.')
+
+        r = self._request_url('POST', '/networks/' + network_ref + '/route')
+        return r.json()
+
+    def unroute_network_address(self, network_ref, address):
+        if not self.check_capability('route-addresses'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'routing addresses.')
+
+        r = self._request_url(
+            'DELETE', '/networks/' + network_ref + '/route' + '/' + address)
         return r.json()
 
     def get_node(self, node):
         if not self.check_capability('node-get'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'showing a single node, try "node list" instead.')
@@ -808,14 +867,22 @@
         r = self._request_url('GET', '/nodes')
         return r.json()
 
     def delete_node(self, node):
         r = self._request_url('DELETE', '/nodes/' + node)
         return r.json()
 
+    def get_node_process_metrics(self, node):
+        if not self.check_capability('node-process-metrics'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'fetching process metrics for a node.')
+        r = self._request_url('GET', '/nodes/' + node + '/processmetrics')
+        return r.json()
+
     def get_interface(self, interface_uuid):
         r = self._request_url('GET', '/interfaces/' + interface_uuid)
         return r.json()
 
     def float_interface(self, interface_uuid):
         r = self._request_url('POST', '/interfaces/' + interface_uuid +
                               '/float')
@@ -846,43 +913,66 @@
         url = '/instances/' + instance_ref + '/consoledata'
         self._request_url('DELETE', url)
 
     def get_vdi_console_helper(self, instance_ref):
         r = self._request_url('GET', '/instances/' + instance_ref + '/vdiconsolehelper')
         return r.text
 
+    def get_screenshot(self, instance_ref):
+        if not self.check_capability('instance-screenshot'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'fetching a screenshot of an instance.')
+
+        r = self._request_url('GET', '/instances/' + instance_ref + '/screenshot')
+        return self.get_blob_data(r.json())
+
+    def _await_agentop(self, r):
+        deadline = time.time() + _calculate_async_deadline(self.async_strategy)
+        while True:
+            if r['state'] == 'complete':
+                return r
+
+            LOG.debug('Waiting for agent operation to be complete')
+            if time.time() > deadline:
+                LOG.debug('Deadline exceeded waiting for agent operation to complete')
+                return r
+
+            time.sleep(1)
+            r = self.get_agent_operation(r['uuid'])
+
     def instance_put_blob(self, instance_ref, blob_uuid, path, mode):
         if not self.check_capability('instance-put-blob'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'placing a blob on an instance.')
 
         r = self._request_url('POST', '/instances/' + instance_ref + '/agent/put',
                               data={'blob_uuid': blob_uuid, 'path': path, 'mode': mode})
-        return r.json()
+        return self._await_agentop(r.json())
 
     def instance_execute(self, instance_ref, command_line):
         if not self.check_capability('instance-execute'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'executing a command within an instance.')
 
         r = self._request_url('POST', '/instances/' + instance_ref + '/agent/execute',
                               data={'command_line': command_line})
-        return r.json()
+        return self._await_agentop(r.json())
 
     def instance_get(self, instance_ref, path):
         if not self.check_capability('instance-get'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'fetching a file from within an instance.')
 
         r = self._request_url('POST', '/instances/' + instance_ref + '/agent/get',
                               data={'path': path})
-        return r.json()
+        return self._await_agentop(r.json())
 
     def get_namespaces(self):
         r = self._request_url('GET', '/auth/namespaces')
         return r.json()
 
     def get_namespace(self, namespace):
         r = self._request_url('GET', '/auth/namespaces/' + namespace)
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/admin.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/admin.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/artifact.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/artifact.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/backup.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/backup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/blob.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/blob.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/instance.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import datetime
 import json
 import os
 from prettytable import PrettyTable
 import subprocess
 import sys
 import tempfile
-import time
 
 from shakenfist_client import apiclient, util
 
 
 @click.group(help='Instance commands')
 def instance():
     pass
@@ -124,15 +123,15 @@
         sys.exit(1)
 
     metadata = ctx.obj['CLIENT'].get_instance_metadata(i['uuid'])
     interfaces = ctx.obj['CLIENT'].get_instance_interfaces(i['uuid'])
     if include_snapshots:
         snapshots = ctx.obj['CLIENT'].get_instance_snapshots(i['uuid'])
     if include_agentoperations:
-        agentops = ctx.obj['CLIENT'].get_instance_agentoperations(i['uuid'])
+        agentops = ctx.obj['CLIENT'].get_instance_agentoperations(i['uuid'], all=True)
 
     if ctx.obj['OUTPUT'] == 'json':
         out = util.filter_dict(i, ['uuid', 'name', 'namespace', 'cpus', 'memory',
                                    'disk_spec', 'video', 'node', 'console_port',
                                    'vdi_port', 'vdi_tls_port', 'ssh_key', 'user_data',
                                    'power_state', 'state', 'uefi', 'secure_boot',
                                    'nvram_template', 'side_channels', 'agent_state'])
@@ -145,15 +144,15 @@
         if include_snapshots:
             out['snapshots'] = []
             for snap in snapshots:
                 out['snapshots'].append(util.filter_dict(
                     snap, ['uuid', 'device', 'created']))
 
         if include_agentoperations:
-            out['agentoperations'] = agentops
+            out['agent_operations'] = agentops
 
         print(json.dumps(out, indent=4, sort_keys=True))
         return
 
     if ctx.obj['OUTPUT'] == 'simple':
         format_string = '%s:%s'
     else:
@@ -173,15 +172,15 @@
     if ctx.obj['OUTPUT'] == 'pretty':
         print(format_string % ('disk spec', _pretty_dict(16, i['disk_spec'], d_space)))
     if ctx.obj['OUTPUT'] == 'pretty':
         print(format_string % ('video', _pretty_dict(16, (i['video'],), v_space)))
     print(format_string % ('node', i.get('node', '')))
     print(format_string % ('power state', i.get('power_state', '')))
     print(format_string % ('state', i.get('state', '')))
-    print(format_string % ('agent_state', i.get('agent_state', '')))
+    print(format_string % ('agent state', i.get('agent_state', '')))
     print(format_string % ('error message', i.get('error_message', '')))
 
     # NOTE(mikal): I am not sure we should expose this, but it will do
     # for now until a proxy is written.
     print(format_string % ('console port', i.get('console_port', '')))
 
     print(format_string % ('vdi port', i.get('vdi_port', '')))
@@ -246,15 +245,35 @@
             for snap in snapshots:
                 print('snapshot,%s,%s,%s'
                       % (snap['uuid'], snap['device'],
                          datetime.datetime.fromtimestamp(snap['created'])))
 
     if include_agentoperations:
         print()
-        print(agentops)
+        if ctx.obj['OUTPUT'] == 'pretty':
+            print('Agent Operations:')
+            print()
+
+            x = PrettyTable()
+            x.field_names = ['uuid', 'state', 'commands']
+            for agentop in agentops:
+                cmds = []
+                for cmd in agentop.get('commands', []):
+                    cmds.append(cmd['command'])
+                x.add_row([agentop['uuid'], agentop['state'], '; '.join(cmds)])
+            print(x)
+
+        else:
+            print('agentop,uuid,state,commands')
+            for agentop in agentops:
+                cmds = []
+                for cmd in agentop.get('commands', []):
+                    cmds.append(cmd['command'])
+                print('agentop, %s,%s,%s'
+                      % (agentop['uuid'], agentop['state'], ';'.join(cmds)))
 
 
 @instance.command(name='show', help='Show an instance')
 @click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.option('-s', '--snapshots', type=click.BOOL, is_flag=True, default=False)
 @click.option('-a', '--agentoperations', type=click.BOOL, is_flag=True, default=False)
 @click.pass_context
@@ -675,19 +694,14 @@
 
 @instance.command(name='upload', help='Upload a file to an instance')
 @click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('source', type=click.Path(exists=True))
 @click.argument('destination', type=click.Path())
 @click.pass_context
 def instance_upload(ctx, instance_ref=None, source=None, destination=None):
-    if not ctx.obj['CLIENT'].check_capability('instance-put-blob'):
-        sys.stderr.write(
-            'Unfortunately this server does not implement copying files into instances.\n')
-        sys.exit(1)
-
     if not ctx.obj['CLIENT'].check_capability('blob-search-by-hash'):
         blob = None
     else:
         # We can cheat here -- if we already have a blob in the cluster with the
         # checksum of the file we're uploading, we can skip the upload entirely and
         # just reuse that blob.
         blob = util.checksum_with_progress(ctx.obj['CLIENT'], source)
@@ -698,58 +712,74 @@
     else:
         print('Recycling existing blob')
         artifact = ctx.obj['CLIENT'].blob_artifact(
             'upload-to-%s' % instance_ref, blob['uuid'], source_url=None)
     print('Created artifact %s' % artifact['uuid'])
 
     st = os.stat(source)
-    op = ctx.obj['CLIENT'].put_instance_blob(
+    ctx.obj['CLIENT'].instance_put_blob(
             instance_ref, artifact['blob_uuid'], destination, st.st_mode)
 
-    # Wait for the copy to complete
-    while True:
-        if op['state'] == 'complete':
-            break
-        time.sleep(5)
-        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
-
-    print('Done')
-
 
 @instance.command(name='execute', help='Execute a command on an instance')
 @click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('commandline', type=click.STRING)
 @click.pass_context
 def instance_execute(ctx, instance_ref=None, commandline=None):
-    if not ctx.obj['CLIENT'].check_capability('instance-execute'):
-        sys.stderr.write(
-            'Unfortunately this server does not implement executing commands on instances.\n')
-        sys.exit(1)
-
     op = ctx.obj['CLIENT'].instance_execute(instance_ref, commandline)
 
-    # Wait for the operation to be complete
-    while True:
-        if op['state'] == 'complete':
-            break
-        time.sleep(5)
-        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
-
-    # Wait for the operation to have results
-    while True:
-        if op['results'] != {}:
-            break
-        time.sleep(5)
-        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
-
     if ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(op, indent=4, sort_keys=True))
         return
 
+    if '0' not in op.get('results', {}):
+        print('Results not available.')
+        sys.exit(1)
+
     if ctx.obj['OUTPUT'] == 'simple':
         format_string = '%s:%s'
+        joiner_template = '\n%(file)s:'
     else:
         format_string = '%-14s: %s'
+        joiner_template = '\n                '
 
-    print(format_string % ('exit code', op['return-code']))
-    print(format_string % ('stdout', op['stdout']))
-    print(format_string % ('stderr', op['stderr']))
+    print(format_string % ('exit code', op['results']['0']['return-code']))
+
+    joiner = joiner_template % {'file': 'stdout'}
+    print(format_string %
+          ('stdout', joiner.join(op['results']['0']['stdout'].split('\n'))))
+
+    joiner = joiner_template % {'file': 'stderr'}
+    print(format_string %
+          ('stderr', joiner.join(op['results']['0']['stderr'].split('\n'))))
+
+
+@instance.command(name='download', help='Download a file from an instance')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.argument('source', type=click.Path())
+@click.argument('destination', type=click.Path())
+@click.pass_context
+def instance_download(ctx, instance_ref=None, source=None, destination=None):
+    op = ctx.obj['CLIENT'].instance_get(instance_ref, source)
+    if '0' not in op.get('results', {}):
+        print('Results not available.')
+        sys.exit(1)
+
+    blob_uuid = op['results']['0'].get('content_blob')
+    if not blob_uuid:
+        print('Results did not include content')
+        sys.exit(1)
+
+    with open(destination, 'wb') as f:
+        for chunk in ctx.obj['CLIENT'].get_blob_data(blob_uuid):
+            f.write(chunk)
+
+
+@instance.command(name='screenshot',
+                  help='Download a screenshot of the console of an instance')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.argument('destination', type=click.Path())
+@click.pass_context
+def instance_screenshot(ctx, instance_ref=None, destination=None):
+    with open(destination, 'wb') as f:
+        for chunk in ctx.obj['CLIENT'].get_screenshot(instance_ref):
+            f.write(chunk)
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/interface.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/interface.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/label.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/label.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/namespace.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/namespace.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/network.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/network.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import click
 import datetime
+import ipaddress
 import json
 from prettytable import PrettyTable
 import sys
 
 
 from shakenfist_client import util
 
@@ -212,7 +213,66 @@
         for line in output.get('stdout', '').split('\n'):
             print('stdout: %s' % line)
         for line in output.get('stderr', '').split('\n'):
             print('stderr: %s' % line)
 
     elif ctx.obj['OUTPUT'] == 'json':
         print(output)
+
+
+@network.command(name='addresses', help='Display address allocations for a network')
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
+@click.pass_context
+def network_addresses(ctx, network_ref=None):
+    addresses = ctx.obj['CLIENT'].get_network_addresses(network_ref)
+    if ctx.obj['OUTPUT'] == 'json':
+        print(json.dumps(addresses, indent=4, sort_keys=True))
+        return
+
+    info_by_addr = {}
+    for addr in addresses:
+        info_by_addr[int(ipaddress.IPv4Address(addr['address']))] = addr
+
+    if ctx.obj['OUTPUT'] == 'pretty':
+        x = PrettyTable()
+        x.field_names = ['address', 'type', 'user', 'comment']
+    else:
+        print('address,type,user,comment')
+
+    for addr in sorted(info_by_addr.keys()):
+        if not info_by_addr[addr]['user']:
+            user = ''
+        elif type(info_by_addr[addr]['user']) is list:
+            user = ' '.join(info_by_addr[addr]['user'])
+        else:
+            user = info_by_addr[addr]['user']
+
+        if ctx.obj['OUTPUT'] == 'pretty':
+            x.add_row([info_by_addr[addr]['address'],
+                       info_by_addr[addr]['type'],
+                       user,
+                       info_by_addr[addr]['comment']])
+        else:
+            print('%s,%s,%s,%s'
+                  % (info_by_addr[addr]['address'],
+                     info_by_addr[addr]['type'],
+                     ' '.join(info_by_addr[addr]['user']),
+                     info_by_addr[addr]['comment']))
+
+    if ctx.obj['OUTPUT'] == 'pretty':
+        print(x)
+
+
+@network.command(name='add-routed', help='Add a routed address to the network')
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
+@click.pass_context
+def network_route(ctx, network_ref=None):
+    routed = ctx.obj['CLIENT'].route_network_address(network_ref)
+    print(routed)
+
+
+@network.command(name='delete-routed', help='Remove a routed address from the network')
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('address', type=click.STRING)
+@click.pass_context
+def network_unroute(ctx, network_ref=None, address=None):
+    ctx.obj['CLIENT'].unroute_network_address(network_ref, address)
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/commandline/node.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/commandline/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import click
 import datetime
 import json
 from prettytable import PrettyTable
 import sys
 import time
 
+from shakenfist_client.apiclient import IncapableException
 from shakenfist_client import util
 
 
 @click.group(help='Node commands')
 def node():
     pass
 
@@ -180,23 +181,42 @@
 
 
 # This command is primarily intended for a CI check to ensure we're not spinning
 # too hard in a processing loop, but it may be useful elsewhere.
 @node.command(name='cpuhogs', help='List processes consuming "too much" CPU')
 @click.option('-t', '--threshold', default=0.25,
               help='The CPU fraction above which to complain.')
+@click.option('-i', '--ignore', default='',
+              help='A comma separated list of processes to ignore')
 @click.pass_context
-def node_cpuhogs(ctx, threshold=0.25):
+def node_cpuhogs(ctx, threshold=0.25, ignore=None):
     hogs = []
+    ignore_processes = ignore.split(',')
 
     for node in ctx.obj['CLIENT'].get_nodes():
-        event = ctx.obj['CLIENT'].get_node_events(node['name'], event_type='resources', limit=1)[0]
-        for resource in event.get('extra', {}):
-            value = event['extra'][resource]
-            if resource.startswith('process_cpu_fraction_') and value > threshold:
-                hogs.append('%s on node %s has consumed %.02f of a CPU, threshold is %.02f'
-                            % (resource[len('process_cpu_fraction_'):],
-                               node['name'], value, threshold))
+        try:
+            metrics = ctx.obj['CLIENT'].get_node_process_metrics(node['name'])
+            for resource in metrics:
+                value = metrics[resource]
+                if resource.startswith('process_cpu_fraction_') and value > threshold:
+                    process = resource[len('process_cpu_fraction_'):]
+                    if process in ignore_processes:
+                        continue
+                    hogs.append('%s on node %s has consumed %.02f of a CPU, threshold is %.02f'
+                                % (process, node['name'], value, threshold))
+
+        except IncapableException:
+            # Fall back to the old way
+            event = ctx.obj['CLIENT'].get_node_events(node['name'], event_type='resources',
+                                                      limit=1)[0]
+            for resource in event.get('extra', {}):
+                value = event['extra'][resource]
+                if resource.startswith('process_cpu_fraction_') and value > threshold:
+                    process = resource[len('process_cpu_fraction_'):]
+                    if process in ignore_processes:
+                        continue
+                    hogs.append('%s on node %s has consumed %.02f of a CPU, threshold is %.02f'
+                                % (process, node['name'], value, threshold))
 
     if hogs:
         print('\n'.join(hogs))
         sys.exit(1)
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/main.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import json
 import logging
 from shakenfist_utilities import logs
 import sys
 
 from shakenfist_client import apiclient
 from shakenfist_client.commandline import admin
+from shakenfist_client.commandline import ansible
 from shakenfist_client.commandline import artifact
 from shakenfist_client.commandline import backup
 from shakenfist_client.commandline import blob
 from shakenfist_client.commandline import instance
 from shakenfist_client.commandline import interface
+from shakenfist_client.commandline import k3s
 from shakenfist_client.commandline import label
 from shakenfist_client.commandline import namespace
 from shakenfist_client.commandline import network
 from shakenfist_client.commandline import node
 
 
 LOG = logs.setup_console(__name__)
@@ -115,17 +117,19 @@
 @cli.command(name='version', help='Output the version of the client')
 @click.pass_context
 def version(ctx):
     print(apiclient.get_user_agent())
 
 
 cli.add_command(admin.admin)
+cli.add_command(ansible.ansible)
 cli.add_command(artifact.artifact)
 cli.add_command(backup.backup)
 cli.add_command(blob.blob)
 cli.add_command(instance.instance)
 cli.add_command(interface.interface)
+cli.add_command(k3s.k3s)
 cli.add_command(label.label)
 cli.add_command(namespace.namespace)
 cli.add_command(network.network)
 cli.add_command(node.node)
 cli.add_command(version)
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/tests/test_client_apiclient.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/tests/test_client_apiclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def test_get_instance(self):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
         client.get_instance('notreallyauuid')
 
         self.mock_request.assert_called_with(
-            'GET', '/instances/notreallyauuid')
+            'GET', '/instances/notreallyauuid', data=None)
 
     def test_get_instance_interfaces(self):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
         client.get_instance_interfaces('notreallyauuid')
 
         self.mock_request.assert_called_with(
@@ -291,15 +291,15 @@
 
     def test_get_network(self):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
         client.get_network('notreallyauuid')
 
         self.mock_request.assert_called_with(
-            'GET', '/networks/notreallyauuid')
+            'GET', '/networks/notreallyauuid', data=None)
 
     def test_delete_network(self):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
         client.delete_network('notreallyauuid')
 
         self.mock_request.assert_called_with(
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client/util.py` & `shakenfist-client-0.7.0.0rc8/shakenfist_client/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 def get_networks(ctx, args, incomplete):
     networks = get_client(ctx).get_networks()
     choices = [n[key] for key in ['uuid', 'name'] for n in networks]
     return [arg for arg in choices if arg.startswith(incomplete)]
 
 
-def checksum_with_progress(apiclient, source):
+def checksum_with_progress(client, source):
     st = os.stat(source)
 
     sha512_hash = hashlib.sha512()
     with open(source, 'rb') as f:
         with tqdm(total=st.st_size, unit='B', unit_scale=True,
                   desc='Calculate checksum') as pbar:
             d = f.read(4096)
@@ -97,48 +97,46 @@
                 d = f.read(4096)
                 while d:
                     sha512_hash.update(d)
                     pbar.update(len(d))
                     d = f.read(4096)
 
     print('Searching for a pre-existing blob with this hash...')
-    return apiclient.get_blob_by_sha512(sha512_hash.hexdigest())
+    return client.get_blob_by_sha512(sha512_hash.hexdigest())
 
 
-def upload_artifact_with_progress(apiclient, name, source, source_url,
+def upload_artifact_with_progress(client, name, source, source_url,
                                   namespace=None, shared=False):
     print('None found, uploading')
     buffer_size = 4096
     st = os.stat(source)
 
     # We do not use send_upload_file because we want to hook in our own
     # progress bar.
-    upload = apiclient.create_upload()
+    upload = client.create_upload()
     total = 0
     retries = 0
     with tqdm(total=st.st_size, unit='B', unit_scale=True,
               desc='Uploading %s to %s' % (upload['uuid'], upload['node'])) as pbar:
         with open(source, 'rb') as f:
             d = f.read(buffer_size)
             while d:
                 start_time = time.time()
                 try:
-                    remote_total = apiclient.send_upload(
-                        upload['uuid'], d)
+                    remote_total = client.send_upload(upload['uuid'], d)
                     retries = 0
                 except apiclient.APIException as e:
                     retries += 1
 
                     if retries > 5:
                         print('Repeated failures, aborting')
                         raise e
 
                     print('Upload error, retrying...')
-                    apiclient.truncate_upload(
-                        upload['uuid'], total)
+                    client.truncate_upload(upload['uuid'], total)
                     f.seek(total)
                     buffer_size = 4096
                     d = f.read(buffer_size)
                     continue
 
                 # We aim for each chunk to take three seconds to transfer. This is
                 # partially because of the API timeout on the other end, but also
@@ -156,10 +154,10 @@
                 if total != remote_total:
                     print('Remote side has %d, we have sent %d!' % (remote_total, total))
                     sys.exit(1)
 
                 d = f.read(buffer_size)
 
     print('Creating artifact')
-    artifact = apiclient.upload_artifact(
+    artifact = client.upload_artifact(
         name, upload['uuid'], source_url=source_url, shared=shared, namespace=namespace)
     return artifact
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/PKG-INFO` & `shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc7
+Version: 0.7.0.0rc8
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc7/shakenfist_client.egg-info/SOURCES.txt` & `shakenfist-client-0.7.0.0rc8/shakenfist_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,41 +4,43 @@
 README.md
 release.sh
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
-.github/workflows/configure-tests.py
-.github/workflows/functional-tests-debian-10-localhost.yml
+.github/workflows/ansible-module-tests.yml
 .github/workflows/functional-tests-debian-11-slim-primary.yml
 .github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
-.github/workflows/functional-tests.tmpl
+.github/workflows/functional-tests-ubuntu-2204-slim-primary.yml
 .github/workflows/python-unit-tests.yml
-ansible/sf_instance.py
-ansible/sf_network.py
+ansible/sf_instance
+ansible/sf_namespace
+ansible/sf_network
 ansible/sf_snapshot.py
 shakenfist_client/__init__.py
 shakenfist_client/apiclient.py
 shakenfist_client/main.py
 shakenfist_client/util.py
 shakenfist_client.egg-info/PKG-INFO
 shakenfist_client.egg-info/SOURCES.txt
 shakenfist_client.egg-info/dependency_links.txt
 shakenfist_client.egg-info/entry_points.txt
 shakenfist_client.egg-info/not-zip-safe
 shakenfist_client.egg-info/pbr.json
 shakenfist_client.egg-info/requires.txt
 shakenfist_client.egg-info/top_level.txt
 shakenfist_client/commandline/admin.py
+shakenfist_client/commandline/ansible.py
 shakenfist_client/commandline/artifact.py
 shakenfist_client/commandline/backup.py
 shakenfist_client/commandline/blob.py
 shakenfist_client/commandline/instance.py
 shakenfist_client/commandline/interface.py
+shakenfist_client/commandline/k3s.py
 shakenfist_client/commandline/label.py
 shakenfist_client/commandline/namespace.py
 shakenfist_client/commandline/network.py
 shakenfist_client/commandline/node.py
 shakenfist_client/tests/__init__.py
 shakenfist_client/tests/test_client_apiclient.py
 tools/buffer.py
```

### Comparing `shakenfist-client-0.7.0.0rc7/tools/clone_with_depends.py` & `shakenfist-client-0.7.0.0rc8/tools/clone_with_depends.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/tools/flake8wrap.sh` & `shakenfist-client-0.7.0.0rc8/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc7/tox.ini` & `shakenfist-client-0.7.0.0rc8/tox.ini`

 * *Files identical despite different names*

