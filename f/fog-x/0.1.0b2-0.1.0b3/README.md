# Comparing `tmp/fog_x-0.1.0b2.tar.gz` & `tmp/fog_x-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fog_x-0.1.0b2.tar", last modified: Wed Apr 24 07:40:43 2024, max compression
+gzip compressed data, was "fog_x-0.1.0b3.tar", last modified: Sun Apr 28 08:29:31 2024, max compression
```

## Comparing `fog_x-0.1.0b2.tar` & `fog_x-0.1.0b3.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.264227 fog_x-0.1.0b2/
--rw-r--r--   0 kych     (1000610) users    (1000001)      380 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/Containerfile
--rw-r--r--   0 kych     (1000610) users    (1000001)      229 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/HISTORY.md
--rw-r--r--   0 kych     (1000610) users    (1000001)    12926 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/LICENSE
--rw-r--r--   0 kych     (1000610) users    (1000001)       81 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/MANIFEST.in
--rw-r--r--   0 kych     (1000610) users    (1000001)     4027 2024-04-24 07:40:43.264227 fog_x-0.1.0b2/PKG-INFO
--rw-r--r--   0 kych     (1000610) users    (1000001)     3002 2024-04-24 07:38:28.000000 fog_x-0.1.0b2/README.md
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.248227 fog_x-0.1.0b2/fog_x/
--rw-r--r--   0 kych     (1000610) users    (1000001)       13 2024-04-24 07:40:40.000000 fog_x-0.1.0b2/fog_x/VERSION
--rw-r--r--   0 kych     (1000610) users    (1000001)      367 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/__init__.py
--rw-r--r--   0 kych     (1000610) users    (1000001)      136 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/__main__.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.252227 fog_x-0.1.0b2/fog_x/__pycache__/
--rw-r--r--   0 kych     (1000610) users    (1000001)      541 2024-04-24 02:18:00.000000 fog_x-0.1.0b2/fog_x/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)      539 2024-04-24 03:51:49.000000 fog_x-0.1.0b2/fog_x/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)    16408 2024-04-24 02:21:58.000000 fog_x-0.1.0b2/fog_x/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)    16385 2024-04-24 03:52:12.000000 fog_x-0.1.0b2/fog_x/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3635 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/__pycache__/episode.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3608 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/__pycache__/episode.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     4309 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/__pycache__/feature.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     4305 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/__pycache__/feature.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)      734 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/cli.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.256227 fog_x-0.1.0b2/fog_x/database/
--rw-r--r--   0 kych     (1000610) users    (1000001)      383 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/database/__init__.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.260227 fog_x-0.1.0b2/fog_x/database/__pycache__/
--rw-r--r--   0 kych     (1000610) users    (1000001)      440 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)      438 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     5183 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/db_connector.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     5177 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/db_connector.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     7038 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/db_manager.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     7004 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/db_manager.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     6519 2024-04-24 02:21:59.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/polars_connector.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     6594 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/polars_connector.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3851 2024-04-24 02:18:01.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3894 2024-04-24 03:51:50.000000 fog_x-0.1.0b2/fog_x/database/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     6405 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/database/db_connector.py
--rw-r--r--   0 kych     (1000610) users    (1000001)    12943 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/database/db_manager.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     8199 2024-04-24 02:21:00.000000 fog_x-0.1.0b2/fog_x/database/polars_connector.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     5944 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/database/utils.py
--rw-r--r--   0 kych     (1000610) users    (1000001)    24743 2024-04-24 03:52:10.000000 fog_x-0.1.0b2/fog_x/dataset.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     3466 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/episode.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     5261 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/feature.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.260227 fog_x-0.1.0b2/fog_x/rlds/
--rw-r--r--   0 kych     (1000610) users    (1000001)       29 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/rlds/__init__.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.260227 fog_x-0.1.0b2/fog_x/rlds/__pycache__/
--rw-r--r--   0 kych     (1000610) users    (1000001)      172 2024-04-24 02:18:02.000000 fog_x-0.1.0b2/fog_x/rlds/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3201 2024-04-24 02:18:02.000000 fog_x-0.1.0b2/fog_x/rlds/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 kych     (1000610) users    (1000001)     3320 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/rlds/utils.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     6599 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/rlds/writer.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.260227 fog_x-0.1.0b2/fog_x/storage/
--rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/storage/__init__.py
--rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/fog_x/storage/storage.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.264227 fog_x-0.1.0b2/fog_x.egg-info/
--rw-r--r--   0 kych     (1000610) users    (1000001)     4027 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/PKG-INFO
--rw-r--r--   0 kych     (1000610) users    (1000001)     1633 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/SOURCES.txt
--rw-r--r--   0 kych     (1000610) users    (1000001)        1 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/dependency_links.txt
--rw-r--r--   0 kych     (1000610) users    (1000001)       46 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/entry_points.txt
--rw-r--r--   0 kych     (1000610) users    (1000001)      220 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/requires.txt
--rw-r--r--   0 kych     (1000610) users    (1000001)        6 2024-04-24 07:40:43.000000 fog_x-0.1.0b2/fog_x.egg-info/top_level.txt
--rw-r--r--   0 kych     (1000610) users    (1000001)       38 2024-04-24 07:40:43.264227 fog_x-0.1.0b2/setup.cfg
--rw-r--r--   0 kych     (1000610) users    (1000001)     1294 2024-04-24 07:38:58.000000 fog_x-0.1.0b2/setup.py
-drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-24 07:40:43.260227 fog_x-0.1.0b2/tests/
--rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/tests/__init__.py
--rw-r--r--   0 kych     (1000610) users    (1000001)      398 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/tests/conftest.py
--rw-r--r--   0 kych     (1000610) users    (1000001)     2347 2024-04-24 00:35:07.000000 fog_x-0.1.0b2/tests/test_base.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.313152 fog_x-0.1.0b3/
+-rw-r--r--   0 kych     (1000610) users    (1000001)      380 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/Containerfile
+-rw-r--r--   0 kych     (1000610) users    (1000001)      229 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/HISTORY.md
+-rw-r--r--   0 kych     (1000610) users    (1000001)    12926 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/LICENSE
+-rw-r--r--   0 kych     (1000610) users    (1000001)       81 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/MANIFEST.in
+-rw-r--r--   0 kych     (1000610) users    (1000001)    19069 2024-04-28 08:29:31.309152 fog_x-0.1.0b3/PKG-INFO
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3002 2024-04-24 07:38:28.000000 fog_x-0.1.0b3/README.md
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.301152 fog_x-0.1.0b3/fog_x/
+-rw-r--r--   0 kych     (1000610) users    (1000001)       13 2024-04-28 08:19:34.000000 fog_x-0.1.0b3/fog_x/VERSION
+-rw-r--r--   0 kych     (1000610) users    (1000001)      367 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/__init__.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)      136 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/__main__.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.301152 fog_x-0.1.0b3/fog_x/__pycache__/
+-rw-r--r--   0 kych     (1000610) users    (1000001)      541 2024-04-24 02:18:00.000000 fog_x-0.1.0b3/fog_x/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)      539 2024-04-24 03:51:49.000000 fog_x-0.1.0b3/fog_x/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)    16408 2024-04-24 02:21:58.000000 fog_x-0.1.0b3/fog_x/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)    16385 2024-04-24 03:52:12.000000 fog_x-0.1.0b3/fog_x/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3635 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/__pycache__/episode.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3608 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/__pycache__/episode.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     4309 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/__pycache__/feature.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     4305 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/__pycache__/feature.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)      734 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/cli.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.305152 fog_x-0.1.0b3/fog_x/database/
+-rw-r--r--   0 kych     (1000610) users    (1000001)      383 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/database/__init__.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.305152 fog_x-0.1.0b3/fog_x/database/__pycache__/
+-rw-r--r--   0 kych     (1000610) users    (1000001)      440 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)      438 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     5183 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/db_connector.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     5177 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/db_connector.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     7038 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/db_manager.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     7004 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/db_manager.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     6519 2024-04-24 02:21:59.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/polars_connector.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     6594 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/polars_connector.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3851 2024-04-24 02:18:01.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3894 2024-04-24 03:51:50.000000 fog_x-0.1.0b3/fog_x/database/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     6405 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/database/db_connector.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)    12943 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/database/db_manager.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     8199 2024-04-24 02:21:00.000000 fog_x-0.1.0b3/fog_x/database/polars_connector.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     5944 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/database/utils.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)    24743 2024-04-24 03:52:10.000000 fog_x-0.1.0b3/fog_x/dataset.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3466 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/episode.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     5261 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/feature.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.305152 fog_x-0.1.0b3/fog_x/rlds/
+-rw-r--r--   0 kych     (1000610) users    (1000001)       29 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/rlds/__init__.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.305152 fog_x-0.1.0b3/fog_x/rlds/__pycache__/
+-rw-r--r--   0 kych     (1000610) users    (1000001)      172 2024-04-24 02:18:02.000000 fog_x-0.1.0b3/fog_x/rlds/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3201 2024-04-24 02:18:02.000000 fog_x-0.1.0b3/fog_x/rlds/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 kych     (1000610) users    (1000001)     3320 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/rlds/utils.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     6599 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/rlds/writer.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.309152 fog_x-0.1.0b3/fog_x/storage/
+-rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/storage/__init__.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/fog_x/storage/storage.py
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.309152 fog_x-0.1.0b3/fog_x.egg-info/
+-rw-r--r--   0 kych     (1000610) users    (1000001)    19069 2024-04-28 08:29:31.000000 fog_x-0.1.0b3/fog_x.egg-info/PKG-INFO
+-rw-r--r--   0 kych     (1000610) users    (1000001)     1607 2024-04-28 08:29:31.000000 fog_x-0.1.0b3/fog_x.egg-info/SOURCES.txt
+-rw-r--r--   0 kych     (1000610) users    (1000001)        1 2024-04-28 08:29:31.000000 fog_x-0.1.0b3/fog_x.egg-info/dependency_links.txt
+-rw-r--r--   0 kych     (1000610) users    (1000001)      262 2024-04-28 08:29:31.000000 fog_x-0.1.0b3/fog_x.egg-info/requires.txt
+-rw-r--r--   0 kych     (1000610) users    (1000001)        6 2024-04-28 08:29:31.000000 fog_x-0.1.0b3/fog_x.egg-info/top_level.txt
+-rw-r--r--   0 kych     (1000610) users    (1000001)      895 2024-04-28 08:27:49.000000 fog_x-0.1.0b3/pyproject.toml
+-rw-r--r--   0 kych     (1000610) users    (1000001)       38 2024-04-28 08:29:31.313152 fog_x-0.1.0b3/setup.cfg
+drwxr-xr-x   0 kych     (1000610) users    (1000001)        0 2024-04-28 08:29:31.309152 fog_x-0.1.0b3/tests/
+-rw-r--r--   0 kych     (1000610) users    (1000001)        0 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/tests/__init__.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)      398 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/tests/conftest.py
+-rw-r--r--   0 kych     (1000610) users    (1000001)     2347 2024-04-24 00:35:07.000000 fog_x-0.1.0b3/tests/test_base.py
```

### Comparing `fog_x-0.1.0b2/LICENSE` & `fog_x-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/README.md` & `fog_x-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/__init__.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/__init__.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/dataset.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/dataset.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/dataset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/episode.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/episode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/episode.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/episode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/feature.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/feature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/__pycache__/feature.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/__pycache__/feature.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/cli.py` & `fog_x-0.1.0b3/fog_x/cli.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/db_connector.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/db_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/db_connector.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/db_connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/db_manager.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/db_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/db_manager.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/db_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/polars_connector.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/polars_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/polars_connector.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/polars_connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/utils.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/__pycache__/utils.cpython-39.pyc` & `fog_x-0.1.0b3/fog_x/database/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/db_connector.py` & `fog_x-0.1.0b3/fog_x/database/db_connector.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/db_manager.py` & `fog_x-0.1.0b3/fog_x/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/polars_connector.py` & `fog_x-0.1.0b3/fog_x/database/polars_connector.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/database/utils.py` & `fog_x-0.1.0b3/fog_x/database/utils.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/dataset.py` & `fog_x-0.1.0b3/fog_x/dataset.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/episode.py` & `fog_x-0.1.0b3/fog_x/episode.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/feature.py` & `fog_x-0.1.0b3/fog_x/feature.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/rlds/__pycache__/utils.cpython-310.pyc` & `fog_x-0.1.0b3/fog_x/rlds/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/rlds/utils.py` & `fog_x-0.1.0b3/fog_x/rlds/utils.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x/rlds/writer.py` & `fog_x-0.1.0b3/fog_x/rlds/writer.py`

 * *Files identical despite different names*

### Comparing `fog_x-0.1.0b2/fog_x.egg-info/SOURCES.txt` & `fog_x-0.1.0b3/fog_x.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Containerfile
 HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 fog_x/VERSION
 fog_x/__init__.py
 fog_x/__main__.py
 fog_x/cli.py
 fog_x/dataset.py
 fog_x/episode.py
 fog_x/feature.py
 fog_x.egg-info/PKG-INFO
 fog_x.egg-info/SOURCES.txt
 fog_x.egg-info/dependency_links.txt
-fog_x.egg-info/entry_points.txt
 fog_x.egg-info/requires.txt
 fog_x.egg-info/top_level.txt
 fog_x/__pycache__/__init__.cpython-310.pyc
 fog_x/__pycache__/__init__.cpython-39.pyc
 fog_x/__pycache__/dataset.cpython-310.pyc
 fog_x/__pycache__/dataset.cpython-39.pyc
 fog_x/__pycache__/episode.cpython-310.pyc
```

### Comparing `fog_x-0.1.0b2/tests/test_base.py` & `fog_x-0.1.0b3/tests/test_base.py`

 * *Files identical despite different names*

