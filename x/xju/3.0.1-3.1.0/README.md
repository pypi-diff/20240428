# Comparing `tmp/xju-3.0.1.tar.gz` & `tmp/xju-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-3.0.1.tar", last modified: Tue Mar 26 11:09:47 2024, max compression
+gzip compressed data, was "xju-3.1.0.tar", last modified: Sun Apr 28 04:38:12 2024, max compression
```

## Comparing `xju-3.0.1.tar` & `xju-3.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.922296 xju-3.0.1/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2024-03-26 11:09:47.000000 xju-3.0.1/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)    10326 2024-03-26 11:09:47.922296 xju-3.0.1/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     8790 2024-03-26 11:09:47.000000 xju-3.0.1/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2024-03-26 11:09:47.000000 xju-3.0.1/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-03-26 11:09:47.922296 xju-3.0.1/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.914296 xju-3.0.1/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.918296 xju-3.0.1/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-3.0.1/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-3.0.1/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.922296 xju-3.0.1/src/xju/cmc/
--rwxr-xr-x   0 xju       (1001) xju       (1001)     9796 2023-11-19 01:52:13.000000 xju-3.0.1/src/xju/cmc/AsyncDict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-3.0.1/src/xju/cmc/AsyncOpt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-3.0.1/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-11-26 07:06:55.000000 xju-3.0.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-3.0.1/src/xju/cmc/Dict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-3.0.1/src/xju/cmc/Opt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1459 2024-03-19 10:15:57.000000 xju-3.0.1/src/xju/cmc/Process.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-3.0.1/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    45419 2024-03-09 04:40:58.000000 xju-3.0.1/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     8548 2024-03-09 07:44:30.000000 xju-3.0.1/src/xju/cmc/async_cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-3.0.1/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14897 2024-03-09 07:13:47.000000 xju-3.0.1/src/xju/cmc/cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4475 2024-03-01 12:12:32.000000 xju-3.0.1/src/xju/cmc/delay_cancellation.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.922296 xju-3.0.1/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-3.0.1/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-3.0.1/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-3.0.1/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-3.0.1/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-3.0.1/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-3.0.1/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-3.0.1/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18361 2024-03-19 08:42:32.000000 xju-3.0.1/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-3.0.1/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-3.0.1/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-3.0.1/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-3.0.1/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-3.0.1/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-3.0.1/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7377 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju/cmc_mypy_plugin.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2024-02-04 01:38:20.000000 xju-3.0.1/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-3.0.1/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    79481 2024-03-01 12:17:56.000000 xju-3.0.1/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    44126 2024-03-26 10:57:35.000000 xju-3.0.1/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     9347 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju/json_codec_mypy_plugin.py
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-3.0.1/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-3.0.1/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1352 2024-03-01 12:17:56.000000 xju-3.0.1/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-3.0.1/src/xju/misc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    25757 2023-11-19 01:52:13.000000 xju-3.0.1/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    13294 2023-11-19 01:52:13.000000 xju-3.0.1/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-3.0.1/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-3.0.1/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-3.0.1/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-3.0.1/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-3.0.1/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-3.0.1/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3403 2023-10-03 21:35:57.000000 xju-3.0.1/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2762 2023-10-03 21:39:56.000000 xju-3.0.1/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7647 2024-03-19 08:36:54.000000 xju-3.0.1/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6010 2024-03-19 08:44:56.000000 xju-3.0.1/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-26 11:09:47.922296 xju-3.0.1/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)    10326 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1508 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-03-26 11:09:47.000000 xju-3.0.1/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.941629 xju-3.1.0/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2024-04-28 04:38:11.000000 xju-3.1.0/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)    10434 2024-04-28 04:38:12.941629 xju-3.1.0/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     8898 2024-04-28 04:38:11.000000 xju-3.1.0/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2024-04-28 04:38:11.000000 xju-3.1.0/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-04-28 04:38:12.941629 xju-3.1.0/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.933629 xju-3.1.0/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.937629 xju-3.1.0/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-3.1.0/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-3.1.0/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.941629 xju-3.1.0/src/xju/cmc/
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     9796 2023-11-19 01:52:13.000000 xju-3.1.0/src/xju/cmc/AsyncDict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-3.1.0/src/xju/cmc/AsyncOpt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-3.1.0/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-11-26 07:06:55.000000 xju-3.1.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-3.1.0/src/xju/cmc/Dict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-3.1.0/src/xju/cmc/Opt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1459 2024-03-19 10:15:57.000000 xju-3.1.0/src/xju/cmc/Process.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-3.1.0/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    45419 2024-03-09 04:40:58.000000 xju-3.1.0/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8548 2024-03-09 07:44:30.000000 xju-3.1.0/src/xju/cmc/async_cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-3.1.0/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14897 2024-03-09 07:13:47.000000 xju-3.1.0/src/xju/cmc/cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4475 2024-03-01 12:12:32.000000 xju-3.1.0/src/xju/cmc/delay_cancellation.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.941629 xju-3.1.0/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-3.1.0/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-3.1.0/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-3.1.0/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-3.1.0/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-3.1.0/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-3.1.0/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-3.1.0/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18361 2024-03-19 08:42:32.000000 xju-3.1.0/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-3.1.0/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-3.1.0/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-3.1.0/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-3.1.0/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-3.1.0/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-3.1.0/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7377 2024-04-28 04:38:11.000000 xju-3.1.0/src/xju/cmc_mypy_plugin.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2024-02-04 01:38:20.000000 xju-3.1.0/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-3.1.0/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    80520 2024-04-28 04:07:50.000000 xju-3.1.0/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    44759 2024-04-28 03:45:21.000000 xju-3.1.0/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     9347 2024-04-28 04:38:11.000000 xju-3.1.0/src/xju/json_codec_mypy_plugin.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-3.1.0/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-3.1.0/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1352 2024-03-01 12:17:56.000000 xju-3.1.0/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-3.1.0/src/xju/misc.py.test
+-r--r--r--   0 xju       (1001) xju       (1001)    26466 2024-04-28 03:38:30.000000 xju-3.1.0/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    13529 2024-04-28 03:38:21.000000 xju-3.1.0/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-3.1.0/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-3.1.0/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2024-04-28 00:35:48.000000 xju-3.1.0/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2024-04-28 00:35:48.000000 xju-3.1.0/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:11.000000 xju-3.1.0/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-3.1.0/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-3.1.0/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3403 2023-10-03 21:35:57.000000 xju-3.1.0/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2762 2023-10-03 21:39:56.000000 xju-3.1.0/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7647 2024-03-19 08:36:54.000000 xju-3.1.0/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6010 2024-03-19 08:44:56.000000 xju-3.1.0/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-04-28 04:38:12.941629 xju-3.1.0/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)    10434 2024-04-28 04:38:12.000000 xju-3.1.0/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1508 2024-04-28 04:38:12.000000 xju-3.1.0/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-04-28 04:38:12.000000 xju-3.1.0/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-04-28 04:38:12.000000 xju-3.1.0/src/xju.egg-info/top_level.txt
```

### Comparing `xju-3.0.1/MIT-LICENCE` & `xju-3.1.0/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/PKG-INFO` & `xju-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 3.0.1
+Version: 3.1.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -195,14 +195,16 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.1.0 add validity pattern support to xju.newtype.Str
+- 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
 - 2.0.3 add xju.cmc_mypy_plugin, no need for xju.cmc.AsyncCM/CM when using async_cmclass/cmclass decorator
 - 2.0.2 add xju.cmc.delay_cancellation
 - 2.0.2 add bytes support to xju.json_codec
```

### Comparing `xju-3.0.1/README.rst` & `xju-3.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,16 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.1.0 add validity pattern support to xju.newtype.Str
+- 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
 - 2.0.3 add xju.cmc_mypy_plugin, no need for xju.cmc.AsyncCM/CM when using async_cmclass/cmclass decorator
 - 2.0.2 add xju.cmc.delay_cancellation
 - 2.0.2 add bytes support to xju.json_codec
```

### Comparing `xju-3.0.1/pyproject.toml` & `xju-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "3.0.1"
+version = "3.1.0"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `xju-3.0.1/src/xju/assert_.py` & `xju-3.1.0/src/xju/assert_.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/assert_.py.test` & `xju-3.1.0/src/xju/assert_.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/AsyncDict.py.test` & `xju-3.1.0/src/xju/cmc/AsyncDict.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/AsyncOpt.py.test` & `xju-3.1.0/src/xju/cmc/AsyncOpt.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-3.1.0/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test` & `xju-3.1.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/Dict.py.test` & `xju-3.1.0/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/Opt.py.test` & `xju-3.1.0/src/xju/cmc/Opt.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/Process.py.test` & `xju-3.1.0/src/xju/cmc/Process.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-3.1.0/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/__init__.py` & `xju-3.1.0/src/xju/cmc/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/async_cmclass.py.test` & `xju-3.1.0/src/xju/cmc/async_cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/cmc.py.test` & `xju-3.1.0/src/xju/cmc/cmc.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/cmclass.py.test` & `xju-3.1.0/src/xju/cmc/cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/delay_cancellation.py.test` & `xju-3.1.0/src/xju/cmc/delay_cancellation.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/FileLock.py.test` & `xju-3.1.0/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/FileMode.py.test` & `xju-3.1.0/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/FilePosition.py.test` & `xju-3.1.0/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/FileReader.py.test` & `xju-3.1.0/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/FileWriter.py.test` & `xju-3.1.0/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/Pipe.py.test` & `xju-3.1.0/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-3.1.0/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/io/__init__.py` & `xju-3.1.0/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/perflog.py` & `xju-3.1.0/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/perflog.py.test` & `xju-3.1.0/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/signal.py` & `xju-3.1.0/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/signal.py.test` & `xju-3.1.0/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/tstore.py` & `xju-3.1.0/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc/tstore.py.test` & `xju-3.1.0/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmc_mypy_plugin.py` & `xju-3.1.0/src/xju/cmc_mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmd.py` & `xju-3.1.0/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/cmd.py.test` & `xju-3.1.0/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/json_codec.py` & `xju-3.1.0/src/xju/json_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -881,14 +881,20 @@
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not an str')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
         return get_type_fqn(self.t)
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        if self.t.pattern is not None:
+            return {
+                'description': self.get_type_fqn(),
+                'type': 'string',
+                'pattern': self.t.pattern.pattern
+            }
         return {
             'description': self.get_type_fqn(),
             'type': 'string'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return self.get_type_fqn()
     def typescript_as_object_key_type(self,back_refs:TypeScriptBackRefs|None) -> str:
@@ -896,42 +902,53 @@
     def ensure_typescript_defs(self, namespace) -> None:
         typescript_fqn=[TypeScriptUQN(_) for _ in self.get_type_fqn().split('.')]
         target_namespace=namespace.get_namespace_of(typescript_fqn)
         typescript_type_name=typescript_fqn[-1]
         if typescript_type_name not in target_namespace.defs:
             target_namespace.defs[typescript_type_name]=TypeScriptSourceCode(
                 f"type {typescript_type_name} = string;")
+            as_a=self.get_typescript_asa(TypeScriptSourceCode("v"),
+                                         TypeScriptNamespace({}),
+                                         None)
             target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
                 f"function asInstanceOf{typescript_type_name}(v: any): {typescript_type_name}\n"
                 f"{{\n"
-                f"    try{{\n"
-                f"        if (typeof v !== 'string' /* {self.get_type_fqn()} */) throw new Error(`${{v}} is a ${{typeof v}}`);\n"
-                f"        return v;\n"
-                f"    }}\n"
-                f"    catch(e:any){{\n"
-                f"        throw new Error(`${{v}} is not a {typescript_type_name} because ${{e}}`);\n"
-                f"    }}\n"
+                f"    return {as_a};\n"
                 f"}}")
+            is_a=self.get_typescript_isa(TypeScriptSourceCode("v"),
+                                         TypeScriptNamespace({}),
+                                         None)
             target_namespace.defs[TypeScriptUQN(f'isInstanceOf{typescript_type_name}')]=TypeScriptSourceCode(
-                f"function isInstanceOf{typescript_type_name}(v:any): v is string\n"
+                f"function isInstanceOf{typescript_type_name}(v:any): v is string /* {self.get_type_fqn()} */\n"
                 f"{{\n"
-                f"    return typeof v === 'string' /* {self.get_type_fqn()} */;\n"
+                f"    return {is_a};\n"
                 f"}}")
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        if self.t.pattern is not None:
+            return TypeScriptSourceCode(
+                f"(typeof ({expression}) == 'string' /* {self.get_type_fqn()} */ &&\n"
+                f"(new RegExp({self.t.pattern.pattern!r})).exec({expression})!==null)")
         return TypeScriptSourceCode(
-            f"(typeof ({expression}) == 'string')")
+            f"(typeof ({expression}) == 'string') /* {self.get_type_fqn()} */")
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
+        if self.t.pattern is not None:
+            return TypeScriptSourceCode(
+                f"((v: any): {tt} => {{\n"
+                f"    if (typeof v !== 'string' /* {self.get_type_fqn()} */) throw new Error(`${{v}} is not a {self.get_type_fqn()} i.e. a string, it is a ${{typeof v}}`);\n"
+                f"    if ((new RegExp({self.t.pattern.pattern!r})).exec({expression})===null) throw new Error(`${{v}} does not match pattern `+{self.t.pattern.pattern!r});\n"
+                f"    return v as {tt};\n"
+                f"}})({expression})")
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{\n"
             f"    if (typeof v !== 'string' /* {self.get_type_fqn()} */) throw new Error(`${{v}} is not a {self.get_type_fqn()} i.e. a string, it is a ${{typeof v}}`);\n"
             f"    return v as {tt};\n"
             f"}})({expression})")
     pass
 
@@ -1148,15 +1165,15 @@
         self.attr_codecs=attr_codecs
         if issubclass(t,CustomClassCodec):
             self.custom_codec=t
         pass
     def encode(self,x,_:None|Callable[[Any],JsonType]) -> JsonType:
         'encode {x} as a {self.t}'
         try:
-            if type(x) is not self.t:
+            if not isinstance(x, self.t):
                 xt=type(x)
                 raise Exception(f'{x!r} (of type {xt}) is not a {self.t}')
             if self.custom_codec is not None:
                 return self.custom_codec.xju_json_codec_encode(x)
             def back_ref(x:Any) -> JsonType:
                 return self.encode(x,None)
             result={}
```

### Comparing `xju-3.0.1/src/xju/json_codec.py.test` & `xju-3.1.0/src/xju/json_codec.py.test`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,17 @@
 
 # dict with specific value type, keys can be str...
 Assert(codec(dict[str,int]).decode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
 Assert(codec(dict[str,int]).encode({'fred':5, 'jock': 9}))=={'fred':5, 'jock':9}
 
 #... or xju.newtype.Str or anything that with str encoding
 class SurnameTag:pass
-class Surname(xju.newtype.Str[SurnameTag]):pass
+class Surname(xju.newtype.Str[SurnameTag]):
+    pattern=re.compile(r'^\S*$')  # disallow whitespace
+    pass
 
 Assert(codec(dict[Surname,int]).encode({Surname('fred'):5, Surname('jock'): 9}))=={'fred':5, 'jock':9}
 Assert(codec(dict[Surname,int]).decode({'fred':5, 'jock':9}))=={Surname('fred'):5, Surname('jock'): 9}
 
 # ... must be given a dict...
 try:
     x=codec(dict).decode(7)
@@ -500,14 +502,21 @@
         'a',
         'b',
         'street',
         'suburb',
         'postcode',
         'unit']
 
+# ... base class codec can encode subclass (but, obviously, cannot decode to subclass)
+Assert(codec(Address).encode(
+    UnitAddress(
+        'fred',17,Street('alba'),Suburb('bocca'),Postcode(3365),unit=Unit('17a'))))==codec(
+            Address).encode(
+                Address(Street('alba'),Suburb('bocca'),Postcode(3365)))
+       
 # custom class encoding by implementing CustomClassCodec protocol, for example
 # to support encoding of external types with control over their json representation
 class IpV4Addr(ipaddress.IPv4Address):
     __xju_json_codec=codec(str)
 
     @staticmethod
     def xju_json_codec_encode(x:object) -> JsonType:
@@ -815,14 +824,16 @@
 
 Assert(AnyJsonCodecImpl().get_json_schema({},None))== {'oneOf': [{'type': 'null'}, {'type': 'boolean'}, {'type': 'object'}, {'type': 'array'}, {'type': 'number'}, {'type': 'string'}]}
 
 Assert(codec(AgeInYears).get_json_schema())=={'description': 'AgeInYears', 'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Street).get_json_schema())=={'description': 'Street', 'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
+Assert(codec(Surname).get_json_schema())=={'description': 'Surname', 'type': 'string', 'pattern': r'^\S*$', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
+
 Assert(codec(Metres).get_json_schema())=={'description': 'Metres', 'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Literal['fred']).get_json_schema())=={'type': 'string', 'enum': ['fred'], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 Assert(codec(Literal[7,8]).get_json_schema())=={'oneOf': [{'type': 'number', 'enum': [7]}, {'type': 'number', 'enum': [8]}], '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema', 'definitions': {}}
 Assert(codec(Literal[False]).get_json_schema())=={'type': 'boolean', 'enum': [False], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 Assert(codec(O).get_json_schema())=={'oneOf': [{'type': 'string', 'enum': ['fred']}, {'type': 'integer', 'enum': [7]}], '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema', 'definitions': {}}
```

### Comparing `xju-3.0.1/src/xju/json_codec_mypy_plugin.py` & `xju-3.1.0/src/xju/json_codec_mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/jsonschema.py` & `xju-3.1.0/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/jsonschema.py.test` & `xju-3.1.0/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/misc.py` & `xju-3.1.0/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/misc.py.test` & `xju-3.1.0/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/newtype.py` & `xju-3.1.0/src/xju/newtype.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 #
 #  class HoursTag:pass
 #  class Hours(Int[HoursTag]):pass
 #
 # ... note do not use 'Hours=Int[HoursTag]' because that is an alias to a generic and
 # therefore has not run-time presence and therefore cannot be used with isinstance.
 #
+from re import Pattern
 from typing import Iterable,Sized,Container,Collection,Reversible,Protocol,Type,overload,TypeVar
 from typing import Generic,Tuple,Mapping,Optional,List,Literal,Union,Any,Self,Never
 from types import NotImplementedType
+from xju.xn import in_function_context
 
 Tag=TypeVar('Tag',covariant=True)
 
 class Int(Generic[Tag]):
     __value:int
 
     def __init__(self, value:int):
@@ -410,16 +412,30 @@
         return self.value().as_integer_ratio()
 
     pass
 
 
 class Str(Generic[Tag]):
     __value:str
+
+    # class may specify pattern for valid values to match
+    # match is "entirely" i.e. re.Pattern.search
+    # note this must be a class attribute (not overrided by an instance value)
+    pattern: Pattern | None = None
+
     def __init__(self, value:str):
-        self.__value=value
+        "initialise {self.__class__.__name__} to value {value!r}"
+        try:
+            self.__value=value
+            if self.__class__.pattern is not None:
+                if not self.__class__.pattern.search(value):
+                    raise Exception(
+                        f"{value!r} does not match regular expression {self.__class__.pattern.pattern!r}")
+        except Exception:
+            raise in_function_context(Str.__init__,vars())
         pass
 
     def value(self)->str:
         return self.__value
 
     # note the following type: ignore is to get the desired behaviour from mypy --strict-equality
     # (as at mypy 1.3.0) i.e. forbid comparison of Int[XTag] and Int[YTag], noting:
```

### Comparing `xju-3.0.1/src/xju/newtype.py.test` & `xju-3.1.0/src/xju/newtype.py.test`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,30 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 from sys import path
 from os.path import dirname
 if path[0]==dirname(__file__): path.pop(0)
 
+import re
+
 from xju.newtype import Str,Int,Float,Bool
 from xju.assert_ import Assert
 from xju.xn import readable_repr
 
 from typing import Dict,cast
 from math import trunc,ceil,floor
 
 class FirstNameType:pass
 class LastNameType:pass
 
 class FirstName(Str[FirstNameType]):pass
-class LastName(Str[LastNameType]):pass
+class LastName(Str[LastNameType]):
+    pattern=re.compile(r'^\S*$')  # disallow whitespace
+    pass
 
 def full_name(first_name:FirstName,last_name:LastName)->str:
     return f'{first_name} {last_name}'
 
 def f(x:FirstName)->FirstName:
     return x
 
@@ -410,14 +414,21 @@
 y:list[LastName|Weight|Hours] = [ LastName('fred'), Weight(7.8), Hours(9) ]
 
 Assert(LastName('jock') not in y)==True
 Assert(Hours(2) not in y)==True
 Assert(Weight(2.1) not in y)==True
 
 
+try:
+    LastName('St Cloud')
+except Exception as e:
+    Assert(str(e)).contains(r"'St Cloud' does not match regular expression '^\\S*$'")
+else:
+    assert False
+
 
 # Bool[X]
 
 class EnabledTag: pass
 class IsRedTag: pass
 
 class Enabled(Bool[EnabledTag]):pass
```

### Comparing `xju-3.0.1/src/xju/patch.py` & `xju-3.1.0/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/patch.py.test` & `xju-3.1.0/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/pq.py` & `xju-3.1.0/src/xju/pq.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/pq.py.test` & `xju-3.1.0/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/rfc2616.py` & `xju-3.1.0/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/rfc2616.py.test` & `xju-3.1.0/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/time.py` & `xju-3.1.0/src/xju/time.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/time.py.test` & `xju-3.1.0/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/xn.py` & `xju-3.1.0/src/xju/xn.py`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju/xn.py.test` & `xju-3.1.0/src/xju/xn.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.0.1/src/xju.egg-info/PKG-INFO` & `xju-3.1.0/src/xju.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 3.0.1
+Version: 3.1.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -195,14 +195,16 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.1.0 add validity pattern support to xju.newtype.Str
+- 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
 - 2.0.3 add xju.cmc_mypy_plugin, no need for xju.cmc.AsyncCM/CM when using async_cmclass/cmclass decorator
 - 2.0.2 add xju.cmc.delay_cancellation
 - 2.0.2 add bytes support to xju.json_codec
```

### Comparing `xju-3.0.1/src/xju.egg-info/SOURCES.txt` & `xju-3.1.0/src/xju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

