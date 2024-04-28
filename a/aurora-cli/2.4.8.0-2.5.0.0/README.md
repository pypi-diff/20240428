# Comparing `tmp/aurora-cli-2.4.8.0.tar.gz` & `tmp/aurora_cli-2.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora-cli-2.4.8.0.tar", last modified: Fri Mar 29 16:18:44 2024, max compression
+gzip compressed data, was "aurora_cli-2.5.0.0.tar", last modified: Sun Apr 28 08:52:00 2024, max compression
```

## Comparing `aurora-cli-2.4.8.0.tar` & `aurora_cli-2.5.0.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.330637 aurora-cli-2.4.8.0/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/LICENSE
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/README.md
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1719 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/__main__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_device.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-03-29 12:18:36.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_emulator.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6003 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_emulator_vm.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3478 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/common.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-03-29 12:15:42.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4015 2024-03-16 18:49:53.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4844 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_build.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5954 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4115 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-03-16 20:49:23.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_icon.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_plugins.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    22873 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-03-29 11:55:51.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_available.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_clear.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-03-29 11:54:28.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_install.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_installed.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_package.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_remove.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_sign.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_targets.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_validate.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8005 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-03-29 11:56:02.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/group_sdk.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/support/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7080 2024-03-29 12:00:52.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/conf.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1051 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/dependency.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1979 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/dependency_required.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/download.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7232 2024-03-29 12:36:35.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/helper.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/output.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-03-29 12:34:19.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/sdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-03-16 15:04:33.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/ssh.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    17448 2024-03-29 13:47:50.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/texts.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-03-29 12:15:42.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/vbox.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-03-29 13:03:53.000000 aurora-cli-2.4.8.0/aurora_cli/src/support/versions.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-29 16:18:44.326637 aurora-cli-2.4.8.0/aurora_cli.egg-info/
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2623 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/entry_points.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/requires.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-03-29 16:18:44.000000 aurora-cli-2.4.8.0/aurora_cli.egg-info/top_level.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-03-29 16:18:44.330637 aurora-cli-2.4.8.0/setup.cfg
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-03-29 12:00:52.000000 aurora-cli-2.4.8.0/setup.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.700296 aurora_cli-2.5.0.0/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/LICENSE
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-04-28 08:52:00.700296 aurora_cli-2.5.0.0/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/README.md
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.687296 aurora_cli-2.5.0.0/aurora_cli/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2177 2024-04-27 19:07:23.000000 aurora_cli-2.5.0.0/aurora_cli/__main__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.688296 aurora_cli-2.5.0.0/aurora_cli/src/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.688296 aurora_cli-2.5.0.0/aurora_cli/src/features/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.689296 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_device.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_emulator.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6158 2024-04-28 08:28:43.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_emulator_vm.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.689296 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3478 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/common.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.690297 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4015 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4846 2024-04-27 18:39:23.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_build.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7031 2024-04-28 08:29:49.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4115 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.690297 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    24329 2024-04-28 08:29:49.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.693296 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_available.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_install.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_package.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.694296 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8046 2024-04-27 19:17:13.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.695296 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/group_sdk.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.696296 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.699296 aurora_cli-2.5.0.0/aurora_cli/src/support/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.699296 aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7080 2024-04-28 08:46:15.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/conf.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1051 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/dependency.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1979 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/dependency_required.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/download.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7232 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/helper.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/output.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/sdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/ssh.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    17448 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/texts.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/vbox.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-04-27 18:28:50.000000 aurora_cli-2.5.0.0/aurora_cli/src/support/versions.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 08:52:00.699296 aurora_cli-2.5.0.0/aurora_cli.egg-info/
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2623 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/requires.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-04-28 08:52:00.000000 aurora_cli-2.5.0.0/aurora_cli.egg-info/top_level.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-04-28 08:52:00.700296 aurora_cli-2.5.0.0/setup.cfg
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-04-28 08:46:15.000000 aurora_cli-2.5.0.0/setup.py
```

### Comparing `aurora-cli-2.4.8.0/LICENSE` & `aurora_cli-2.5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/PKG-INFO` & `aurora_cli-2.5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.4.8.0
+Version: 2.5.0.0
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora-cli-2.4.8.0/README.md` & `aurora_cli-2.5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/__main__.py` & `aurora_cli-2.5.0.0/aurora_cli/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,24 @@
 
 
 @click.group(invoke_without_command=True)
 @click.version_option(version=Conf.get_app_version(), prog_name=Conf.get_app_name())
 @click.option('--conf', '-c', default=None, help='Specify config path.', type=click.STRING, required=False)
 @click.pass_context
 def main(ctx: {}, conf: {}):
+    """
+The application allows you to install tools for working with the Aurora OS and simplifies working with them.
+More details about the tools can be found on the documentation page:
+
+Flutter SDK  https://omprussia.gitlab.io/flutter/flutter
+Aurora SDK   https://developer.auroraos.ru/doc/software_development/sdk
+Platform SDK https://developer.auroraos.ru/doc/software_development/psdk
+
+This is a third party tool written by enthusiasts!
+    """
     ctx.obj = Conf(conf)
     if not ctx.invoked_subcommand:
         print(ctx.get_help())
 
 
 main.add_command(group_sdk)
 main.add_command(group_psdk)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_device.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_device.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_emulator.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_emulator.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/devices/group_emulator_vm.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/devices/group_emulator_vm.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 
 import click
 
 from aurora_cli.src.support.dependency_required import check_dependency_ffmpeg
 from aurora_cli.src.support.helper import gen_file_name, get_path_file
 from aurora_cli.src.support.output import VerboseType, echo_stdout, echo_stderr
+from aurora_cli.src.support.sdk import find_folder_sdk
 from aurora_cli.src.support.texts import AppTexts
 from aurora_cli.src.support.vbox import vm_search_emulator_aurora, vb_manage_command, vm_check_is_run
 
 
 @click.group(name='start', invoke_without_command=True)
 @click.pass_context
 @click.option('-v', '--verbose', is_flag=True, help='Detailed output')
@@ -53,15 +54,15 @@
     emulator_name = vm_search_emulator_aurora(VerboseType.none)
 
     if vm_check_is_run(emulator_name):
         # Screenshot path directory
         screenshot_dir = Path.home() / 'Pictures' / 'Screenshots'
 
         # Create is not exist
-        if screenshot_dir.is_dir():
+        if not screenshot_dir.is_dir():
             screenshot_dir.mkdir(parents=True, exist_ok=True)
 
         # Screenshot name
         screenshot_name = gen_file_name('Screenshot_from_', 'png')
 
         # Screenshot path
         screenshot_path = screenshot_dir / screenshot_name
@@ -89,14 +90,17 @@
 @click.group(name='recording', invoke_without_command=True)
 @click.pass_context
 @click.option('-c', '--convert', is_flag=True, help='Convert video to mp4')
 @click.option('-v', '--verbose', is_flag=True, help='Detailed output')
 def emulator_recording(ctx: {}, convert: bool, verbose: bool):
     """Recording video from emulator."""
 
+    workdir = ctx.obj.get_workdir()
+    sdk_path = find_folder_sdk(workdir)
+
     # Required ffmpeg dependency for convert
     if convert:
         check_dependency_ffmpeg()
 
     emulator_name = vm_search_emulator_aurora(VerboseType.none)
 
     # Check verbose
@@ -142,15 +146,15 @@
         vb_manage_command(
             ['controlvm', emulator_name, 'recording', 'off'],
             VerboseType.none if verbose == VerboseType.short else verbose,
         )
 
         default_path = Path(
             get_path_file(
-                '~/AuroraOS/emulator/{name}/{name}/{name}-screen0.webm'.format(name=emulator_name)
+                '{sdk_path}/emulator/{name}/{name}/{name}-screen0.webm'.format(sdk_path=sdk_path, name=emulator_name)
             )
         )
 
         if not default_path.is_file():
             echo_stderr(AppTexts.file_not_found(str(default_path)))
             exit(1)
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/common.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/common.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/devices/impl/utils.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/devices/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_build.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
   # Change output
   exec 5>&1
 
   # Build aurora application
   output=$($FLUTTER build aurora --target-platform aurora-$PLATFORM --$VERSION | tee /dev/fd/5)
 
   # Get path to rmp
-  listRPMs=$(echo "$output" | grep "│" | tr -d "\n" | sed 's/│//g' | sed 's/ //g' | sed 's/\.\//;/g')
+  listRPMs=$(echo "$output" | grep "│" | tr -d "\n" | sed 's/│//g' | sed 's/ //g' | sed 's/\\.\\//;/g')
 
   # Get package name
   for item in $(echo "$listRPMs" | tr ";" "\n")
   do
     if [ -n "$item" ] && [[ $item != *"-debug"* ]]; then
       package=$(basename "$item" | cut -d '-' -f1)
       break
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,38 @@
 """
 import os
 from pathlib import Path
 from threading import Timer
 
 import click
 
-from aurora_cli.src.features.devices.impl.utils import device_ssh_select
+from aurora_cli.src.features.devices.impl.utils import device_ssh_select, emulator_ssh_select
 from aurora_cli.src.features.flutter.impl.utils import get_spec_keys, DART_VSCODE_DATA, \
-    CUSTOM_DEVICE_CODE_DATA, get_list_flutter_installed
+    CUSTOM_DEVICE_CODE_DATA, get_list_flutter_installed, CUSTOM_DEVICE_CODE_DATA_VM
 from aurora_cli.src.support.dependency import check_dependency_vscode_plugin
 from aurora_cli.src.support.dependency_required import check_dependency_vscode
 from aurora_cli.src.support.helper import pc_command, find_path_file, prompt_index
 from aurora_cli.src.support.output import VerboseType, echo_stdout, echo_stderr
+from aurora_cli.src.support.sdk import find_folder_sdk
 from aurora_cli.src.support.ssh import ssh_client_exec_command
 from aurora_cli.src.support.texts import AppTexts
 
 
 @click.group(name='dart', invoke_without_command=True)
 @click.pass_context
 @click.option('-i', '--index', type=click.INT, help='Specify index device')
+@click.option('-e', '--emulator', is_flag=True, default=False, help="Run on emulator")
 @click.option('-y', '--yes', is_flag=True, help='All yes confirm')
 @click.option('-v', '--verbose', is_flag=True, help='Detailed output')
-def group_flutter_debug_dart(ctx: {}, index: int, yes: bool, verbose: bool):
+def group_flutter_debug_dart(ctx: {}, index: int, emulator: bool, yes: bool, verbose: bool):
     """Project configure and run on device for dart debug or hot reload."""
 
+    workdir = ctx.obj.get_workdir()
+    sdk_path = find_folder_sdk(workdir)
+
     # Required dependency
     check_dependency_vscode()
 
     # Required flutter
     versions = get_list_flutter_installed()
     if not versions:
         echo_stderr(AppTexts.flutter_not_found())
@@ -83,16 +88,20 @@
     # Enable custom device in flutter
     pc_command([
         flutter,
         'config',
         '--enable-custom-devices',
     ], VerboseType.none)
 
-    # Get device client
-    client, data = device_ssh_select(ctx, index)
+    if emulator:
+        client = emulator_ssh_select(workdir=workdir)
+        device_ip = '127.0.0.1'
+    else:
+        client, data = device_ssh_select(ctx, index)
+        device_ip = data['ip']
 
     # Get path to launch.json
     vscode_dir = Path(f'{os.getcwd()}/.vscode')
     vscode_dir.mkdir(parents=True, exist_ok=True)
     launch = Path(f'{vscode_dir}/launch.json')
 
     # Confirm rewrite file
@@ -110,34 +119,52 @@
         if not click.confirm(AppTexts.debug_configure_confirm('custom_devices.json')):
             exit(0)
 
     def rewrite_configs(url: str, ip: str):
         # Create custom_devices.json
         custom_devices.unlink(missing_ok=True)
         with open(custom_devices, 'w') as file:
-            print(CUSTOM_DEVICE_CODE_DATA.format(
-                ip=ip,
-                package=package_name,
-            ), file=file)
+            if emulator:
+                print(CUSTOM_DEVICE_CODE_DATA_VM.format(
+                    ip=ip,
+                    package=package_name,
+                    sdk_path=sdk_path
+                ), file=file)
+            else:
+                print(CUSTOM_DEVICE_CODE_DATA.format(
+                    ip=ip,
+                    package=package_name,
+                ), file=file)
         # Create launch.json
         launch.unlink(missing_ok=True)
         with open(launch, 'w') as f:
             print(DART_VSCODE_DATA.format(
                 vm_service_uri=url,
                 main_path=('example/lib/main.dart' if 'example' in str(application) and str(
                     application) != os.getcwd() else 'lib/main.dart')
             ), file=f)
 
     def ssh_nfl(port: int):
-        pc_command([
-            'ssh',
-            '-NfL',
-            '{port}:127.0.0.1:{port}'.format(port=port),
-            'defaultuser@{ip}'.format(ip=data['ip'])
-        ], VerboseType.verbose)
+        if emulator:
+            pc_command([
+                'ssh',
+                '-i',
+                '{sdk_path}/vmshare/ssh/private_keys/sdk'.format(sdk_path=sdk_path),
+                '-NfL',
+                '{port}:127.0.0.1:{port}'.format(port=port),
+                'defaultuser@{ip}'.format(ip=device_ip),
+                '-p2223'
+            ], VerboseType.verbose)
+        else:
+            pc_command([
+                'ssh',
+                '-NfL',
+                '{port}:127.0.0.1:{port}'.format(port=port),
+                'defaultuser@{ip}'.format(ip=device_ip),
+            ], VerboseType.verbose)
 
     # Loading 10 second link from app
     def exit_not_debug_run():
         echo_stderr(AppTexts.debug_error_launch_debug_app())
         os._exit(1)
 
     # Run timer
@@ -146,15 +173,15 @@
 
     def update_launch(line: str, _: int):
         if '-bash' in line:
             echo_stderr(AppTexts.debug_error_launch_bin())
             exit(1)
         if 'listening on ' in line:
             url = line.split('listening on ')[1]
-            rewrite_configs(url, data['ip'])
+            rewrite_configs(url, device_ip)
             ssh_nfl(int(url.split('/')[2].split(':')[1]))
             debug_check_run.cancel()
 
     # Exec command
     execute = '/usr/bin/{}'.format(package_name)
 
     # Execute command
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_icon.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/group_flutter_plugins.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/flutter/impl/utils.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/flutter/impl/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,14 +103,80 @@
       ],
       "forwardPortSuccessRegex": "Port forwarding success",
       "screenshot": null
     }}
   ]
 }}'''
 
+CUSTOM_DEVICE_CODE_DATA_VM = r'''{{
+  "custom-devices": [
+    {{
+      "id": "aurora",
+      "label": "Aurora",
+      "sdkNameAndVersion": "5.0",
+      "platform": null,
+      "enabled": true,
+      "ping": [
+        "ping",
+        "-c",
+        "1",
+        "-w",
+        "1",
+        "{ip}"
+      ],
+      "pingSuccessRegex": null,
+      "postBuild": null,
+      "install": [
+        "scp",
+        "-r",
+        "-o",
+        "BatchMode=yes",
+        "${{localPath}}",
+        "defaultuser@{ip}:/tmp/${{appName}}"
+      ],
+      "uninstall": [
+        "ssh",
+        "-i",
+        "{sdk_path}/vmshare/ssh/private_keys/sdk",
+        "-p2223",
+        "-o",
+        "BatchMode=yes",
+        "defaultuser@{ip}",
+        "rm -rf \"/tmp/${{appName}}\""
+      ],
+      "runDebug": [
+        "ssh",
+        "-i",
+        "{sdk_path}/vmshare/ssh/private_keys/sdk",
+        "-p2223",
+        "-o",
+        "BatchMode=yes",
+        "defaultuser@{ip}",
+        "/usr/bin/{package}"
+      ],
+      "forwardPort": [
+        "ssh",
+        "-i",
+        "{sdk_path}/vmshare/ssh/private_keys/sdk",
+        "-p2223",
+        "-o",
+        "BatchMode=yes",
+        "-o",
+        "ExitOnForwardFailure=yes",
+        "-L",
+        "127.0.0.1:${{hostPort}}:127.0.0.1:${{devicePort}}",
+        "defaultuser@{ip}",
+        "echo 'Port forwarding success'; read"
+      ],
+      "forwardPortSuccessRegex": "Port forwarding success",
+      "screenshot": null
+    }}
+  ]
+}}'''
+
 PLUGINS_OUTPUT_HTML = '''
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>Plugins info</title>
     <link rel="preconnect" href="https://fonts.googleapis.com">
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_available.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_available.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_clear.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_install.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_install.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_installed.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_package.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_package.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_remove.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_sign.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_targets.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/group_psdk_validate.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/psdk/impl/utils.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/psdk/impl/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
     return None
 
 
 # Find archive Platform SDK
 def get_url_psdk_archives(version: str) -> []:
     url_folder = get_url_sdk_folder(version)
+    if not url_folder:
+        return []
     response = get_request(url_folder)
     result = []
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, 'html.parser')
         for item in soup.findAll('a'):
             text = item.text
             if 'md5sum' not in text and 'Aurora_OS' in text and '-pu' not in text:
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/group_sdk.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/group_sdk.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/features/sdk/impl/utils.py` & `aurora_cli-2.5.0.0/aurora_cli/src/features/sdk/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/conf.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from aurora_cli.src.support.helper import get_path_file, get_request
 from aurora_cli.src.support.output import echo_stdout, VerboseType, echo_stderr
 from aurora_cli.src.support.texts import AppTexts
 
 # Data versions
 APP_NAME = 'aurora-cli'
-APP_VERSION = '2.4.8'
+APP_VERSION = '2.5.0'
 
 # Default path config
 PATH_CONF = '~/.aurora-cli/configuration.yaml'
 
 # Temp folder
 PATH_TEMP = '~/.aurora-cli/temp'
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/dependency.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/dependency.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/dependency_required.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/dependency_required.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/download.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/download.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/helper.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/helper.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/output.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/output.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/sdk.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/sdk.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/ssh.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/ssh.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/texts.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/texts.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/vbox.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/vbox.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli/src/support/versions.py` & `aurora_cli-2.5.0.0/aurora_cli/src/support/versions.py`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/aurora_cli.egg-info/PKG-INFO` & `aurora_cli-2.5.0.0/aurora_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.4.8.0
+Version: 2.5.0.0
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora-cli-2.4.8.0/aurora_cli.egg-info/SOURCES.txt` & `aurora_cli-2.5.0.0/aurora_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aurora-cli-2.4.8.0/setup.py` & `aurora_cli-2.5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 """
 
 setuptools.setup(
     name='aurora-cli',
-    version='2.4.8.0',
+    version='2.5.0.0',
     author='Vitaliy Zarubin',
     author_email='keygenqt@gmail.com',
     description='An application that simplifies the life of an application developer for the Aurora OS.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/keygenqt/aurora-cli",
     packages=setuptools.find_packages(exclude=['*tests.*', '*tests']),
```

