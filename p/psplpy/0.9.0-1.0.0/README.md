# Comparing `tmp/psplpy-0.9.0.tar.gz` & `tmp/psplpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "psplpy-1.0.0.tar", last modified: Sun Apr 28 07:57:08 2024, max compression
```

## Comparing `psplpy-0.9.0.tar` & `psplpy-1.0.0.tar`

### file list

```diff
@@ -1,74 +1,33 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 psplpy-0.9.0/requirements.txt
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/__init__.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/autogui_util.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/command_wrapper.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/data_access.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/data_process.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/dllmain.cpp
--rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/file_util.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/gui_util.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/image_util.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/interact_util.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/linux.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/ocr_util.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/other.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/other_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/setting.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/time_it.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/time_util.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/timing.py
--rw-r--r--   0        0        0   123261 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/data/icon.png
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/data/time_it_template.txt
--rw-r--r--   0        0        0    59392 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/lib/PyDll.dll
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/__init__.py
--rw-r--r--   0        0        0    11134 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/auto_wechat.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/deprecated.rar
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/linux.py
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/my_notepad.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/scripts/upload_pypi_project.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/README.md
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/test.webp
--rw-r--r--   0        0        0    49167 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/test_ref.ppm
--rwxr-xr-x   0        0        0   771584 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/anim_diff.exe
--rwxr-xr-x   0        0        0   879104 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/anim_dump.exe
--rwxr-xr-x   0        0        0   725504 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/cwebp.exe
--rwxr-xr-x   0        0        0   492544 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/dwebp.exe
--rw-r--r--   0        0        0   229376 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/freeglut.dll
--rwxr-xr-x   0        0        0   720896 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/get_disto.exe
--rwxr-xr-x   0        0        0   791552 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/gif2webp.exe
--rwxr-xr-x   0        0        0   746496 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/img2webp.exe
--rwxr-xr-x   0        0        0   486912 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/vwebp.exe
--rwxr-xr-x   0        0        0   223232 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/webp_quality.exe
--rwxr-xr-x   0        0        0   307200 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/webpinfo.exe
--rwxr-xr-x   0        0        0   238592 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/bin/webpmux.exe
--rw-r--r--   0        0        0    13839 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/doc/api.md
--rw-r--r--   0        0        0    18611 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/doc/tools.md
--rw-r--r--   0        0        0    24285 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/decode.h
--rw-r--r--   0        0        0    15966 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/demux.h
--rw-r--r--   0        0        0    28562 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/encode.h
--rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/mux.h
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/mux_types.h
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/include/webp/types.h
--rw-r--r--   0        0        0  1704890 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/lib/libwebp.lib
--rw-r--r--   0        0        0    41276 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/lib/libwebpdemux.lib
--rw-r--r--   0        0        0   120972 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/libwebp-1.3.1-windows-x64/lib/libwebpmux.lib
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/AdbWinApi.dll
--rw-r--r--   0        0        0    62976 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/AdbWinUsbApi.dll
--rw-r--r--   0        0        0  1073895 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/NOTICE.txt
--rwxr-xr-x   0        0        0  5938176 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/adb.exe
--rwxr-xr-x   0        0        0   241664 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/dmtracedump.exe
--rwxr-xr-x   0        0        0   430592 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/etc1tool.exe
--rwxr-xr-x   0        0        0  1830912 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/fastboot.exe
--rwxr-xr-x   0        0        0    44032 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/hprof-conv.exe
--rw-r--r--   0        0        0   231594 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/libwinpthread-1.dll
--rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/make_f2fs.exe
--rwxr-xr-x   0        0        0   466944 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/make_f2fs_casefold.exe
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/mke2fs.conf
--rwxr-xr-x   0        0        0   745472 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/mke2fs.exe
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/source.properties
--rwxr-xr-x   0        0        0  1330176 2020-02-02 00:00:00.000000 psplpy-0.9.0/psplpy/tools/platform-tools/sqlite3.exe
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 psplpy-0.9.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 psplpy-0.9.0/LICENSE
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 psplpy-0.9.0/README.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 psplpy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 psplpy-0.9.0/PKG-INFO
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-04-28 07:57:08.930115 psplpy-1.0.0/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      213 2024-04-10 09:07:19.000000 psplpy-1.0.0/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy/
+-rw-r--r--   0 a         (1000) a         (1000)       80 2024-04-17 20:36:31.000000 psplpy-1.0.0/psplpy/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2339 2024-04-17 19:45:37.000000 psplpy-1.0.0/psplpy/concurrency_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     3939 2024-04-28 07:48:09.000000 psplpy-1.0.0/psplpy/dynamic_compose.py
+-rw-r--r--   0 a         (1000) a         (1000)      932 2024-04-19 21:14:36.000000 psplpy-1.0.0/psplpy/file_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)    16862 2024-04-28 05:12:45.000000 psplpy-1.0.0/psplpy/image_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     3579 2024-04-17 20:36:31.000000 psplpy-1.0.0/psplpy/middleware_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     3317 2024-04-18 00:34:49.000000 psplpy-1.0.0/psplpy/network_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)      959 2024-04-19 18:40:32.000000 psplpy-1.0.0/psplpy/other_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy/scripts/
+-rw-r--r--   0 a         (1000) a         (1000)     4316 2024-04-10 23:12:10.000000 psplpy-1.0.0/psplpy/scripts/block_jetbrains.py
+-rw-r--r--   0 a         (1000) a         (1000)     1194 2024-04-09 23:43:54.000000 psplpy-1.0.0/psplpy/scripts/upload_pypi_project.py
+-rw-r--r--   0 a         (1000) a         (1000)     8500 2024-04-17 20:51:44.000000 psplpy-1.0.0/psplpy/serialization_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/psplpy.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      681 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)        7 2024-04-28 07:57:08.000000 psplpy-1.0.0/psplpy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)      423 2024-04-13 20:00:29.000000 psplpy-1.0.0/pyproject.toml
+-rw-r--r--   0 a         (1000) a         (1000)       38 2024-04-28 07:57:08.930115 psplpy-1.0.0/setup.cfg
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-04-28 07:57:08.930115 psplpy-1.0.0/tests/
+-rw-r--r--   0 a         (1000) a         (1000)      909 2024-04-28 06:49:06.000000 psplpy-1.0.0/tests/test.py
+-rw-r--r--   0 a         (1000) a         (1000)      873 2024-04-17 19:47:51.000000 psplpy-1.0.0/tests/test_concurrency_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)      912 2024-04-28 07:36:54.000000 psplpy-1.0.0/tests/test_dynamic_compose.py
+-rw-r--r--   0 a         (1000) a         (1000)      464 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_file_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     4448 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_image_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     3001 2024-04-10 22:24:54.000000 psplpy-1.0.0/tests/test_middleware_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     1653 2024-04-19 02:14:39.000000 psplpy-1.0.0/tests/test_network_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)      478 2024-04-19 21:19:24.000000 psplpy-1.0.0/tests/test_other_utils.py
+-rw-r--r--   0 a         (1000) a         (1000)     5480 2024-04-17 21:08:14.000000 psplpy-1.0.0/tests/test_serialization_utils.py
```

### Comparing `psplpy-0.9.0/PKG-INFO` & `psplpy-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 0.9.0
+Version: 1.0.0
 Summary: The Personal Study Purposes Library of PYthon.
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PSPLPY
 
 The **P**ersonal **S**tudy **P**urposes **L**ibrary of **PY**thon.
 
 It's only a python library for personal study purposes.
 
 If you find any problem, you can contact me at
-https://github.com/y-09/psplpy
+https://github.com/y-09/psplpy
```

