# Comparing `tmp/adbutils-2.4.1.tar.gz` & `tmp/adbutils-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.4.1.tar", last modified: Wed Apr 17 02:58:57 2024, max compression
+gzip compressed data, was "adbutils-2.5.0.tar", last modified: Sun Apr 28 11:05:58 2024, max compression
```

## Comparing `adbutils-2.4.1.tar` & `adbutils-2.5.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.824798 adbutils-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 02:58:51.000000 adbutils-2.4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.816798 adbutils-2.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 02:58:51.000000 adbutils-2.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-17 02:58:51.000000 adbutils-2.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 02:58:51.000000 adbutils-2.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-17 02:58:51.000000 adbutils-2.4.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 02:58:57.000000 adbutils-2.4.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-17 02:58:57.000000 adbutils-2.4.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 02:58:51.000000 adbutils-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 02:58:57.824798 adbutils-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-17 02:58:51.000000 adbutils-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-17 02:58:51.000000 adbutils-2.4.1/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 02:58:57.000000 adbutils-2.4.1/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.816798 adbutils-2.4.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-17 02:58:51.000000 adbutils-2.4.1/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-17 02:58:51.000000 adbutils-2.4.1/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 02:58:51.000000 adbutils-2.4.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.820798 adbutils-2.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-17 02:58:51.000000 adbutils-2.4.1/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 02:58:51.000000 adbutils-2.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 02:58:51.000000 adbutils-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 02:58:57.824798 adbutils-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 02:58:51.000000 adbutils-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.824798 adbutils-2.4.1/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-17 02:58:51.000000 adbutils-2.4.1/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:57.824798 adbutils-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-17 02:58:51.000000 adbutils-2.4.1/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-17 02:58:51.000000 adbutils-2.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 02:58:51.000000 adbutils-2.4.1/tests/test_adb_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-28 11:05:51.000000 adbutils-2.5.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 11:05:51.000000 adbutils-2.5.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-28 11:05:51.000000 adbutils-2.5.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 11:05:58.000000 adbutils-2.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-28 11:05:58.000000 adbutils-2.5.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 11:05:51.000000 adbutils-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-28 11:05:58.076576 adbutils-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-28 11:05:51.000000 adbutils-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-28 11:05:51.000000 adbutils-2.5.0/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 11:05:58.000000 adbutils-2.5.0/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.072576 adbutils-2.5.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-28 11:05:51.000000 adbutils-2.5.0/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-28 11:05:51.000000 adbutils-2.5.0/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-28 11:05:51.000000 adbutils-2.5.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 11:05:51.000000 adbutils-2.5.0/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 11:05:51.000000 adbutils-2.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 11:05:51.000000 adbutils-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-28 11:05:58.076576 adbutils-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-28 11:05:51.000000 adbutils-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-28 11:05:51.000000 adbutils-2.5.0/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:05:58.076576 adbutils-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 11:05:51.000000 adbutils-2.5.0/tests/test_adb_server.py
```

### Comparing `adbutils-2.4.1/.coveragerc` & `adbutils-2.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/.github/workflows/main.yml` & `adbutils-2.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/.github/workflows/publish-to-pypi.yml` & `adbutils-2.5.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/.travis.yml` & `adbutils-2.5.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/LICENSE` & `adbutils-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/PKG-INFO` & `adbutils-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.4.1
+Version: 2.5.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.4.1/README.md` & `adbutils-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/__init__.py` & `adbutils-2.5.0/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/__main__.py` & `adbutils-2.5.0/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/_adb.py` & `adbutils-2.5.0/adbutils/_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/_deprecated.py` & `adbutils-2.5.0/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/_device.py` & `adbutils-2.5.0/adbutils/_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/_proto.py` & `adbutils-2.5.0/adbutils/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/_utils.py` & `adbutils-2.5.0/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/errors.py` & `adbutils-2.5.0/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/install.py` & `adbutils-2.5.0/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/pidcat.py` & `adbutils-2.5.0/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/screenrecord.py` & `adbutils-2.5.0/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils/screenshot.py` & `adbutils-2.5.0/adbutils/screenshot.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,30 +38,42 @@
     def framebuffer(self) -> Image.Image:
         pass
 
 class ScreenshotExtesion(AbstractDevice):
     def __init__(self):
         self.__framebuffer_ok = True
 
-    def screenshot(self) -> Image.Image:
+    def screenshot(self, display_id: Optional[int] = None) -> Image.Image:
         """ Take a screenshot and return PIL.Image.Image object
-        If capture failed, return a black image
+        Args:
+            display_id: int, default None, see "dumpsys SurfaceFlinger --display-id" for valid display IDs
+        
+        Returns:
+            PIL.Image.Image object, If capture failed, return a black image
         """
         try:
-            pil_image = self.__screencap()
+            pil_image = self.__screencap(display_id)
             if pil_image.mode == "RGBA":
                 pil_image = pil_image.convert("RGB")
             return pil_image
         except UnidentifiedImageError as e:
             wsize = self.window_size()
             return Image.new("RGB", wsize, (0, 0, 0))
     
-    def __screencap(self) -> Image.Image:
-        if self.__framebuffer_ok:
-            try:
-                return self.framebuffer()
-            except NotImplementedError:
-                self.__framebuffer_ok = False
-            except UnidentifiedImageError as e:
-                logger.warning("framebuffer error: %s", e)
-        png_bytes = self.shell('screencap -p', encoding=None)
+    def __screencap(self, display_id: int = None) -> Image.Image:
+        """ Take a screenshot and return PIL.Image.Image object
+        """
+        # framebuffer is not stable, so we disable it
+        # MemoryError may occur when using framebuffer
+        
+        # if self.__framebuffer_ok and display_id is None:
+        #     try:
+        #         return self.framebuffer()
+        #     except NotImplementedError:
+        #         self.__framebuffer_ok = False
+        #     except UnidentifiedImageError as e:
+        #         logger.warning("framebuffer error: %s", e)
+        cmdargs = ['screencap', '-p']
+        if display_id is not None:
+            cmdargs.extend(['-d', str(display_id)])
+        png_bytes = self.shell(cmdargs, encoding=None)
         return Image.open(io.BytesIO(png_bytes))
```

### Comparing `adbutils-2.4.1/adbutils/shell.py` & `adbutils-2.5.0/adbutils/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,27 +148,31 @@
             sx = int(sx * w) if is_percent(sx) else sx
             sy = int(sy * h) if is_percent(sy) else sy
             ex = int(ex * w) if is_percent(ex) else ex
             ey = int(ey * h) if is_percent(ey) else ey
         x1, y1, x2, y2 = map(str, [sx, sy, ex, ey])
         self.shell(["input", "swipe", x1, y1, x2, y2, str(int(duration * 1000))])
 
-    def click(self, x, y) -> None:
+    def click(self, x, y, display_id: Optional[int] = None) -> None:
         """
         simulate android tap
 
         Args:
             x, y: int
+            display_id: int, default None, see "dumpsys SurfaceFlinger --display-id" for valid display IDs
         """
         if any(map(is_percent, [x, y])):
             w, h = self.window_size()
             x = int(x * w) if is_percent(x) else x
             y = int(y * h) if is_percent(y) else y
         x, y = map(str, [x, y])
-        self.shell(["input", "tap", x, y])
+        cmdargs = ["input"]
+        if display_id is not None:
+            cmdargs.extend(['-d', str(display_id)])
+        self.shell(cmdargs + ["tap", x, y])
 
     def send_keys(self, text: str):
         """
         Type a given text
 
         Args:
             text: text to be type
```

### Comparing `adbutils-2.4.1/adbutils/sync.py` & `adbutils-2.5.0/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/adbutils.egg-info/PKG-INFO` & `adbutils-2.5.0/adbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.4.1
+Version: 2.5.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.4.1/adbutils.egg-info/SOURCES.txt` & `adbutils-2.5.0/adbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/assets/images/pidcat.png` & `adbutils-2.5.0/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/build_wheel.py` & `adbutils-2.5.0/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/examples/reset-offline.py` & `adbutils-2.5.0/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/setup.cfg` & `adbutils-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/conftest.py` & `adbutils-2.5.0/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/test_adb.py` & `adbutils-2.5.0/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/test_deprecated.py` & `adbutils-2.5.0/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/test_device.py` & `adbutils-2.5.0/test_real_device/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/test_forward_reverse.py` & `adbutils-2.5.0/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/test_real_device/test_utils.py` & `adbutils-2.5.0/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/tests/adb_server.py` & `adbutils-2.5.0/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.4.1/tests/conftest.py` & `adbutils-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

