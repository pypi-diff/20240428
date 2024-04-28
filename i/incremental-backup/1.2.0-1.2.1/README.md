# Comparing `tmp/incremental_backup-1.2.0.tar.gz` & `tmp/incremental_backup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incremental_backup-1.2.0.tar", last modified: Wed Apr 10 11:19:28 2024, max compression
+gzip compressed data, was "incremental_backup-1.2.1.tar", last modified: Sun Apr 28 03:05:10 2024, max compression
```

## Comparing `incremental_backup-1.2.0.tar` & `incremental_backup-1.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.978950 incremental_backup-1.2.0/incremental_backup/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/_utility/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/_utility/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/backup/sum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/command/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/incremental_backup/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/complete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/meta/start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/prune.py
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/incremental_backup/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/incremental_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 11:19:28.000000 incremental_backup-1.2.0/incremental_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:19:28.986950 incremental_backup-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:19:28.982950 incremental_backup-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)    26292 2024-04-10 11:19:24.000000 incremental_backup-1.2.0/test/test_restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.123024 incremental_backup-1.2.1/incremental_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.123024 incremental_backup-1.2.1/incremental_backup/_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/_utility/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/_utility/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.123024 incremental_backup-1.2.1/incremental_backup/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/backup/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12692 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/backup/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/backup/sum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.123024 incremental_backup-1.2.1/incremental_backup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/incremental_backup/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/command/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/incremental_backup/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/meta/complete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/meta/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/meta/start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/incremental_backup/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/incremental_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 03:05:10.000000 incremental_backup-1.2.1/incremental_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-28 03:05:10.000000 incremental_backup-1.2.1/incremental_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 03:05:10.000000 incremental_backup-1.2.1/incremental_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-28 03:05:10.000000 incremental_backup-1.2.1/incremental_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:05:10.127024 incremental_backup-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/test/test_path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/test/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27594 2024-04-28 03:05:05.000000 incremental_backup-1.2.1/test/test_restore.py
```

### Comparing `incremental_backup-1.2.0/LICENCE.txt` & `incremental_backup-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.2.0/PKG-INFO` & `incremental_backup-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,74 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.2.0
+Version: 1.2.1
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
-# Incremental Backup Tool (MK 2)
+# Incremental Backup Tool
 
-by Reece Jones
+**An easy-to-use, no fluff incremental file backup application.**
 
-## Purpose
+## Features
 
-Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
-There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.
-
-Thus, I created this tool. Some of its design goals are:
-
-- free, open source
-- as simple as possible (no installation, no GUI, no fluff)
-- robust
-- fast
-- efficient
-- transparent backup format
-
-This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
-Please see [ChangesFromOriginal.md](ChangesFromOriginal.md) for details.  
-If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
-
-## Disclaimer
-
-This application is intended for low-risk personal use.
-I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
+- **Efficient backup** - copies and stores only changed files.
+- **Simple backup format** - data is stored as plain files, metadata is JSON.
+- **No configuration** - all the tool needs to know is where the data is, and where to put the backups.
+- **Focus on failure** - designed with failure in mind to keep your data intact.
+- **CLI and API usage**
 
 ## Requirements
 
-General usage:
-
 - Windows or Linux system
 - Python 3.9 or newer
 
-Development:
-
-- Pytest (any recent version should do)
+## Usage
 
-## Application Structure
+**Create a backup:**
 
-Important files and directories:
+```
+python -m incremental_backup backup /path/to/back/up /safe/backup/location
+```
 
-- `incremental_backup/` - The Python package.
-  - `backup/` - High-level backup functionality.
-  - `cli/` - Command line interface functionality (see also the _Usage_ section).
-  - `meta/` - Functionality related to backup metadata and structure.
-  - `__main__.py` - Entrypoint for using the command line interface via the package name.
-  - `restore.py` - Backup restoration functionality.
-- `test/` - Test code. Each directory/file corresponds to the module in `incremental_backup/` it tests.
+This will back up files from `/path/to/back/up` into `/safe/backup/location`.
 
-The `incremental_backup` Python package contains all application functionality and can be easily used in a library-like manner.
-Additionally, this package doubles as the application entrypoint.
+Run the same command again to do subsequent backups - it's that easy! Backups in `/safe/backup/location` will be automatically read to determine what needs to be copied.
 
-## Usage
+For details, see [docs/BackupUsage.md](./docs/BackupUsage.md).
 
-The Python package is executable via a command line interface.
-The interface uses multiple "commands" for different functionality.
-Usage is as follows:
+**Restore files:**
 
 ```
-python3 -m incremental_backup <command> <command_args>
+python -m incremental_backup restore /safe/backup/location /restore/to/here
 ```
 
-(You may have to adjust the Python command based on your system configuration.)
+This restores the backed up files from `/safe/backup/location` into `/restore/to/here`.
 
-Commands:
+For details, see [docs/RestoreUsage.md](./docs/RestoreUsage.md).
 
-- `backup` - Creates a new backup. See [BackupUsage.md](BackupUsage.md) for details.
-- `restore` - Restores files from backups. See [RestoreUsage.md](RestoreUsage.md) for details.
-
-To start using this application, you probably want to have a look at [BackupUsage.md](BackupUsage.md).
+## Disclaimer
 
-### Program Exit Codes
+This application is intended for low-risk personal use.
+I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
 
-- 0 - The operation completed successfully, possibly with some warnings (i.e. nonfatal errors).
-- 1 - The command line arguments are invalid.
-- 2 - The operation could not be completed due to a runtime error (typically would be a file I/O error).
-- -1 - The operation was aborted due to a programmer error - sorry in advance.
+## Development and Contributing
 
-## Running Tests
+For details on developing or otherwise contributing to the project, please see [CONTRIBUTING.md](./CONTRIBUTING.md).
 
-With your working directory as the project root directory:
+## Background
 
-```
-python3 -m pytest
-```
+Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
+There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.  
+Thus, I created this tool, and aimed for it to be as simple, open, and robust as possible.
 
-This runs a suite of unit and integration tests.
+This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
+Please see [docs/ChangesFromOriginal.md](./docs/ChangesFromOriginal.md) for details.  
+If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
```

### Comparing `incremental_backup-1.2.0/README.md` & `incremental_backup-1.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,59 @@
-# Incremental Backup Tool (MK 2)
+# Incremental Backup Tool
 
-by Reece Jones
+**An easy-to-use, no fluff incremental file backup application.**
 
-## Purpose
+## Features
 
-Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
-There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.
-
-Thus, I created this tool. Some of its design goals are:
-
-- free, open source
-- as simple as possible (no installation, no GUI, no fluff)
-- robust
-- fast
-- efficient
-- transparent backup format
-
-This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
-Please see [ChangesFromOriginal.md](ChangesFromOriginal.md) for details.  
-If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
-
-## Disclaimer
-
-This application is intended for low-risk personal use.
-I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
+- **Efficient backup** - copies and stores only changed files.
+- **Simple backup format** - data is stored as plain files, metadata is JSON.
+- **No configuration** - all the tool needs to know is where the data is, and where to put the backups.
+- **Focus on failure** - designed with failure in mind to keep your data intact.
+- **CLI and API usage**
 
 ## Requirements
 
-General usage:
-
 - Windows or Linux system
 - Python 3.9 or newer
 
-Development:
-
-- Pytest (any recent version should do)
+## Usage
 
-## Application Structure
+**Create a backup:**
 
-Important files and directories:
+```
+python -m incremental_backup backup /path/to/back/up /safe/backup/location
+```
 
-- `incremental_backup/` - The Python package.
-  - `backup/` - High-level backup functionality.
-  - `cli/` - Command line interface functionality (see also the _Usage_ section).
-  - `meta/` - Functionality related to backup metadata and structure.
-  - `__main__.py` - Entrypoint for using the command line interface via the package name.
-  - `restore.py` - Backup restoration functionality.
-- `test/` - Test code. Each directory/file corresponds to the module in `incremental_backup/` it tests.
+This will back up files from `/path/to/back/up` into `/safe/backup/location`.
 
-The `incremental_backup` Python package contains all application functionality and can be easily used in a library-like manner.
-Additionally, this package doubles as the application entrypoint.
+Run the same command again to do subsequent backups - it's that easy! Backups in `/safe/backup/location` will be automatically read to determine what needs to be copied.
 
-## Usage
+For details, see [docs/BackupUsage.md](./docs/BackupUsage.md).
 
-The Python package is executable via a command line interface.
-The interface uses multiple "commands" for different functionality.
-Usage is as follows:
+**Restore files:**
 
 ```
-python3 -m incremental_backup <command> <command_args>
+python -m incremental_backup restore /safe/backup/location /restore/to/here
 ```
 
-(You may have to adjust the Python command based on your system configuration.)
+This restores the backed up files from `/safe/backup/location` into `/restore/to/here`.
 
-Commands:
+For details, see [docs/RestoreUsage.md](./docs/RestoreUsage.md).
 
-- `backup` - Creates a new backup. See [BackupUsage.md](BackupUsage.md) for details.
-- `restore` - Restores files from backups. See [RestoreUsage.md](RestoreUsage.md) for details.
-
-To start using this application, you probably want to have a look at [BackupUsage.md](BackupUsage.md).
+## Disclaimer
 
-### Program Exit Codes
+This application is intended for low-risk personal use.
+I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
 
-- 0 - The operation completed successfully, possibly with some warnings (i.e. nonfatal errors).
-- 1 - The command line arguments are invalid.
-- 2 - The operation could not be completed due to a runtime error (typically would be a file I/O error).
-- -1 - The operation was aborted due to a programmer error - sorry in advance.
+## Development and Contributing
 
-## Running Tests
+For details on developing or otherwise contributing to the project, please see [CONTRIBUTING.md](./CONTRIBUTING.md).
 
-With your working directory as the project root directory:
+## Background
 
-```
-python3 -m pytest
-```
+Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
+There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.  
+Thus, I created this tool, and aimed for it to be as simple, open, and robust as possible.
 
-This runs a suite of unit and integration tests.
+This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
+Please see [docs/ChangesFromOriginal.md](./docs/ChangesFromOriginal.md) for details.  
+If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
```

### Comparing `incremental_backup-1.2.0/incremental_backup/backup/backup.py` & `incremental_backup-1.2.1/incremental_backup/backup/backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Callable, Iterable, Optional, overload, Sequence
+from typing import Callable, Iterable, Optional, Sequence, overload
 
-from incremental_backup.backup.filesystem import scan_filesystem, ScanFilesystemCallbacks
-from incremental_backup.backup.plan import BackupPlan, execute_backup_plan, ExecuteBackupPlanCallbacks, \
-    ExecuteBackupPlanResults
+from incremental_backup._utility import StrPath
+from incremental_backup.backup.filesystem import (
+    ScanFilesystemCallbacks,
+    scan_filesystem,
+)
+from incremental_backup.backup.plan import (
+    BackupPlan,
+    ExecuteBackupPlanCallbacks,
+    ExecuteBackupPlanResults,
+    execute_backup_plan,
+)
 from incremental_backup.backup.sum import BackupSum
-from incremental_backup.meta import BackupCompleteInfo, BackupDirectoryCreationError, BackupManifest, \
-    BackupMetadata, BackupStartInfo, COMPLETE_INFO_FILENAME, create_new_backup_directory, \
-    DATA_DIRECTORY_NAME, MANIFEST_FILENAME, read_backups, ReadBackupsCallbacks, START_INFO_FILENAME, \
-    write_backup_complete_info_file, write_backup_manifest_file, write_backup_start_info_file
+from incremental_backup.meta import (
+    COMPLETE_INFO_FILENAME,
+    DATA_DIRECTORY_NAME,
+    MANIFEST_FILENAME,
+    START_INFO_FILENAME,
+    BackupCompleteInfo,
+    BackupDirectoryCreationError,
+    BackupManifest,
+    BackupMetadata,
+    BackupStartInfo,
+    ReadBackupsCallbacks,
+    create_new_backup_directory,
+    read_backups,
+    write_backup_complete_info_file,
+    write_backup_manifest_file,
+    write_backup_start_info_file,
+)
 from incremental_backup.path_exclude import PathExcludePattern
-from incremental_backup._utility import StrPath
 
-
-__all__ = [
-    'BackupCallbacks',
-    'BackupError',
-    'BackupResults',
-    'perform_backup'
-]
+__all__ = ["BackupCallbacks", "BackupError", "BackupResults", "perform_backup"]
 
 
 @dataclass(frozen=True)
 class BackupResults:
     """Return results of `perform_backup()`."""
 
     backup_path: Path
@@ -73,62 +87,83 @@
 
     on_write_complete_info_error: Callable[[Path, OSError], None] = lambda path, error: None
     """Called when writing the backup completion information file fails.
         First argument is the path to the file, second argument is the raised exception."""
 
 
 @overload
-def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
-                   callbacks: BackupCallbacks = BackupCallbacks()) -> BackupResults:
-    ...
+def perform_backup(
+    source_directory: StrPath,
+    target_directory: StrPath,
+    exclude_patterns: Iterable[PathExcludePattern],
+    callbacks: BackupCallbacks = BackupCallbacks(),
+) -> BackupResults: ...
+
 
 @overload
-def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
-                   callbacks: BackupCallbacks = BackupCallbacks(), skip_empty: bool = False) -> Optional[BackupResults]:
-    ...
-
-# TODO: clean up this interface. Have an "options" object argument rather than overloads
-def perform_backup(source_directory: StrPath, target_directory: StrPath, exclude_patterns: Iterable[PathExcludePattern],
-                   callbacks: BackupCallbacks = BackupCallbacks(), skip_empty: bool = False) -> Optional[BackupResults]:
+def perform_backup(
+    source_directory: StrPath,
+    target_directory: StrPath,
+    exclude_patterns: Iterable[PathExcludePattern],
+    callbacks: BackupCallbacks = BackupCallbacks(),
+    skip_empty: bool = False,
+) -> Optional[BackupResults]: ...
+
+
+# TODO: (breaking) clean up this interface. Have an "options" object argument rather than overloads
+def perform_backup(
+    source_directory: StrPath,
+    target_directory: StrPath,
+    exclude_patterns: Iterable[PathExcludePattern],
+    callbacks: BackupCallbacks = BackupCallbacks(),
+    skip_empty: bool = False,
+) -> Optional[BackupResults]:
     """Performs the entire operation of creating a new backup, including creating the backup directory, copying files,
-        and saving metadata.
+    and saving metadata.
 
-        :param source_directory: Directory to back up.
-        :param target_directory: Directory to create the new backup in, and where any previous backups are read from.
-            Need not exist.
-        :param exclude_patterns: Patterns to match paths which will be excluded from the backup.
-        :param callbacks: Callbacks for certain events during execution. See `BackupCallbacks`.
-        :param skip_empty: Only perform the backup if there are file changes to record.
-        :return: Metadata and summary information for the backup operation. None if the backup was skipped.
-        :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
-            `BackupError`.
+    :param source_directory: Directory to back up.
+    :param target_directory: Directory to create the new backup in, and where any previous backups are read from.
+        Need not exist.
+    :param exclude_patterns: Patterns to match paths which will be excluded from the backup.
+    :param callbacks: Callbacks for certain events during execution. See `BackupCallbacks`.
+    :param skip_empty: Only perform the backup if there are file changes to record.
+    :return: Metadata and summary information for the backup operation. None if the backup was skipped.
+    :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
+        `BackupError`.
     """
 
-    return _BackupOperation(source_directory, target_directory, exclude_patterns, skip_empty, callbacks).perform_backup()
+    return _BackupOperation(
+        source_directory, target_directory, exclude_patterns, skip_empty, callbacks
+    ).perform_backup()
 
 
 class _BackupOperation:
     """Implementation of the backup creation operation."""
 
-    def __init__(self, source_directory: StrPath, target_directory: StrPath,
-                 exclude_patterns: Iterable[PathExcludePattern], skip_empty: bool,
-                 callbacks: BackupCallbacks = BackupCallbacks()) -> None:
+    def __init__(
+        self,
+        source_directory: StrPath,
+        target_directory: StrPath,
+        exclude_patterns: Iterable[PathExcludePattern],
+        skip_empty: bool,
+        callbacks: BackupCallbacks = BackupCallbacks(),
+    ) -> None:
         self.source_directory = Path(source_directory)
         self.target_directory = Path(target_directory)
         self.exclude_patterns = tuple(exclude_patterns)
         self.skip_empty = skip_empty
         self.callbacks = callbacks
 
         self._init_working_state()
 
     def perform_backup(self) -> Optional[BackupResults]:
         """Creates a new backup.
 
-            :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
-                `BackupError`.
+        :except BackupError: If an error occurs that prevents the backup operation from creating a valid backup. See
+            `BackupError`.
         """
 
         self._init_working_state()
 
         self._validate_source_directory()
         self._validate_target_directory()
 
@@ -153,96 +188,108 @@
         complete_info = self._create_complete_info()
 
         self.callbacks.on_before_save_metadata()
         self._save_manifest(backup_path, execute_results.manifest)
         self._save_complete_info(backup_path, complete_info)
 
         return BackupResults(
-            backup_path, start_info, execute_results.manifest, complete_info, execute_results.files_copied,
-            execute_results.files_removed)
+            backup_path,
+            start_info,
+            execute_results.manifest,
+            complete_info,
+            execute_results.files_copied,
+            execute_results.files_removed,
+        )
 
     def _init_working_state(self) -> None:
         """Initialises various shared data used by and operated on by the methods in this class."""
 
         self.paths_skipped = False
 
     def _validate_source_directory(self) -> None:
         """Validates the backup source directory.
-            Should mostly prevent other parts of the backup operation from failing strangely for invalid inputs.
+        Should mostly prevent other parts of the backup operation from failing strangely for invalid inputs.
 
-            :except BackupError: If the source directory is not an accessible directory.
+        :except BackupError: If the source directory is not an accessible directory.
         """
 
         try:
             if not self.source_directory.exists():
-                raise BackupError('Source directory not found')
+                raise BackupError("Source directory not found")
             if not self.source_directory.is_dir():
-                raise BackupError('Source directory is not a directory')
+                raise BackupError("Source directory is not a directory")
         except OSError as e:
-            raise BackupError(f'Failed to query source directory: {e}') from e
+            raise BackupError(f"Failed to query source directory: {e}") from e
 
     def _validate_target_directory(self) -> None:
         """Validates the backup target directory.
-            Should mostly prevent other parts of the backup operation from failing strangely for invalid inputs.
+        Should mostly prevent other parts of the backup operation from failing strangely for invalid inputs.
 
-            :except BackupError: If the target directory is inaccessible, or exists and is not a directory.
+        :except BackupError: If the target directory is inaccessible, or exists and is not a directory.
         """
 
         try:
             if self.target_directory.exists() and not self.target_directory.is_dir():
-                raise BackupError('Target directory is not a directory')
+                raise BackupError("Target directory is not a directory")
         except OSError as e:
-            raise BackupError(f'Failed to query target directory: {e}') from e
+            raise BackupError(f"Failed to query target directory: {e}") from e
 
     def _read_previous_backups(self) -> Sequence[BackupMetadata]:
         """Reads existing backups' metadata from the backup target directory.
 
-            If any backup's metadata cannot be read, skips that backup.
+        If any backup's metadata cannot be read, skips that backup.
 
-            :except BackupError: If the target directory cannot be enumerated.
+        :except BackupError: If the target directory cannot be enumerated.
         """
 
         self.callbacks.on_before_read_previous_backups()
 
         try:
             if not self.target_directory.exists():
                 backups = []
             else:
                 backups = read_backups(self.target_directory, self.callbacks.read_backups)
         except OSError as e:
-            raise BackupError(f'Failed to enumerate target directory: {e}') from e
+            raise BackupError(f"Failed to enumerate target directory: {e}") from e
         backups = tuple(backups)
 
         self.callbacks.on_after_read_previous_backups(backups)
 
         return backups
 
     def _initialise_backup(self, start_time: datetime) -> tuple[Path, Path, BackupStartInfo]:
         """Creates the backup directory and start info file.
 
-            :return: Tuple of (backup_path, data_path, start_info).
-            :except BackupError: If a fatal error occurs.
+        :return: Tuple of (backup_path, data_path, start_info).
+        :except BackupError: If a fatal error occurs.
         """
 
         self.callbacks.on_before_initialise_backup()
         backup_path = self._create_backup_directory()
         data_path = self._create_data_directory(backup_path)
         start_info = self._create_and_write_start_info(backup_path, start_time)
         return backup_path, data_path, start_info
 
     @staticmethod
     def _is_backup_plan_empty(backup_plan: BackupPlan) -> bool:
         root = backup_plan.root
-        return not (root.copied_files or root.removed_files or root.removed_directories or root.subdirectories
-            or root.contains_copied_files or root.contains_removed_items or root.removed_directory_file_count)
+        return not (
+            root.copied_files
+            or root.removed_files
+            or root.removed_directories
+            or root.subdirectories
+            or root.contains_copied_files
+            or root.contains_removed_items
+            or root.removed_directory_file_count
+        )
 
     def _create_backup_directory(self) -> Path:
         """Creates a new backup directory within the target directory.
 
-            :except BackupError: If the directory could not be created.
+        :except BackupError: If the directory could not be created.
         """
 
         try:
             backup_name = create_new_backup_directory(self.target_directory)
         except BackupDirectoryCreationError as e:
             raise BackupError(str(e)) from e
 
@@ -252,38 +299,38 @@
 
         return backup_path
 
     @staticmethod
     def _create_data_directory(backup_path: Path, /) -> Path:
         """Creates the backup data directory (directory which contains the copied files).
 
-            :return: Path to the created directory.
-            :except BackupError: If the directory could not be created.
+        :return: Path to the created directory.
+        :except BackupError: If the directory could not be created.
         """
 
         path = backup_path / DATA_DIRECTORY_NAME
         try:
             path.mkdir(parents=True, exist_ok=False)
         except OSError as e:
-            raise BackupError(f'Failed to create backup data directory: {e}') from e
+            raise BackupError(f"Failed to create backup data directory: {e}") from e
         return path
 
     @staticmethod
     def _create_and_write_start_info(backup_path: Path, start_time: datetime) -> BackupStartInfo:
         """Creates and writes the backup start information to file within the backup directory.
 
-            :except BackupError: If the file could not be written to.
+        :except BackupError: If the file could not be written to.
         """
 
         start_info = BackupStartInfo(start_time)
         file_path = backup_path / START_INFO_FILENAME
         try:
             write_backup_start_info_file(file_path, start_info)
         except OSError as e:
-            raise BackupError(f'Failed to write backup start information file: {e}') from e
+            raise BackupError(f"Failed to write backup start information file: {e}") from e
         return start_info
 
     def _compute_backup_plan(self, backup_sum: BackupSum) -> BackupPlan:
         """Scans the source directory and generates the backup plan."""
 
         self.callbacks.on_before_scan_source()
 
@@ -294,56 +341,60 @@
 
     def _back_up_files(self, destination_path: StrPath, backup_plan: BackupPlan) -> ExecuteBackupPlanResults:
         """Backs up files from the source directory to the backup directory according to the backup plan."""
 
         self.callbacks.on_before_copy_files()
 
         execute_results = execute_backup_plan(
-            backup_plan, self.source_directory, destination_path, self.callbacks.execute_plan)
+            backup_plan,
+            self.source_directory,
+            destination_path,
+            self.callbacks.execute_plan,
+        )
 
         self.paths_skipped = self.paths_skipped or execute_results.paths_skipped
 
         return execute_results
 
     def _create_complete_info(self) -> BackupCompleteInfo:
         return BackupCompleteInfo(datetime.now(timezone.utc), self.paths_skipped)
 
     @staticmethod
     def _save_manifest(backup_path: Path, manifest: BackupManifest) -> None:
         """Writes the backup manifest to file within the backup directory.
 
-            :except BackupError: If the file could not be written to.
+        :except BackupError: If the file could not be written to.
         """
 
         file_path = backup_path / MANIFEST_FILENAME
         try:
             write_backup_manifest_file(file_path, manifest)
         except OSError as e:
-            raise BackupError(f'Failed to write backup manifest file: {e}') from e
+            raise BackupError(f"Failed to write backup manifest file: {e}") from e
 
     def _save_complete_info(self, backup_path: Path, complete_info: BackupCompleteInfo) -> None:
         """Writes the backup completion information to file within the backup directory.
 
-            It is not a fatal error if this operation fails, since the completion information is not required by the
-            application at this time."""
+        It is not a fatal error if this operation fails, since the completion information is not required by the
+        application at this time."""
 
         file_path = backup_path / COMPLETE_INFO_FILENAME
         try:
             write_backup_complete_info_file(file_path, complete_info)
         except OSError as e:
             # Not fatal since the completion info isn't currently used by the software.
             self.callbacks.on_write_complete_info_error(file_path, e)
 
 
 class BackupError(Exception):
     """Raised when creating a backup fails such that a valid backup cannot be produced.
 
-        Some cases where this exception is raised:
-         - The source directory cannot be accessed at all.
-         - A new backup directory couldn't be created.
-         - Writing the backup start information file failed.
-         - Writing the backup manifest file failed.
+    Some cases where this exception is raised:
+     - The source directory cannot be accessed at all.
+     - A new backup directory couldn't be created.
+     - Writing the backup start information file failed.
+     - Writing the backup manifest file failed.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
         self.message = message
```

### Comparing `incremental_backup-1.2.0/incremental_backup/backup/filesystem.py` & `incremental_backup-1.2.1/incremental_backup/backup/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
+import os.path
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from functools import partial
-import os.path
 from pathlib import Path
 from typing import Callable, Iterable
 
-from incremental_backup.path_exclude import PathExcludePattern, is_path_excluded
 from incremental_backup._utility import StrPath
-
+from incremental_backup.path_exclude import PathExcludePattern, is_path_excluded
 
 __all__ = [
-    'Directory',
-    'File',
-    'scan_filesystem',
-    'ScanFilesystemCallbacks',
-    'ScanFilesystemResults'
+    "Directory",
+    "File",
+    "scan_filesystem",
+    "ScanFilesystemCallbacks",
+    "ScanFilesystemResults",
 ]
 
 
 @dataclass
 class File:
     name: str
     last_modified: datetime
 
 
 @dataclass
 class Directory:
     name: str
     files: list[File] = field(default_factory=list)
-    subdirectories: list['Directory'] = field(default_factory=list)
+    subdirectories: list["Directory"] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class ScanFilesystemCallbacks:
     """Callbacks for events that occur during `scan_filesystem()`."""
 
     on_exclude: Callable[[Path], None] = lambda path: None
@@ -55,48 +54,52 @@
     """Root of the tree representation of the filesystem (the root itself represents the directory requested to be
         scanned)."""
 
     paths_skipped: bool
     """Indicates if any paths were skipped due to I/O errors (does not include paths matched by exclude patterns)."""
 
 
-def scan_filesystem(path: StrPath, /, exclude_patterns: Iterable[PathExcludePattern],
-                    callbacks: ScanFilesystemCallbacks = ScanFilesystemCallbacks()) -> ScanFilesystemResults:
+def scan_filesystem(
+    path: StrPath,
+    /,
+    exclude_patterns: Iterable[PathExcludePattern],
+    callbacks: ScanFilesystemCallbacks = ScanFilesystemCallbacks(),
+) -> ScanFilesystemResults:
     """Produces a tree representation of the filesystem at a given directory.
 
-        If any paths cannot be accessed for any reason, they will be skipped and excluded from the constructed tree.
+    If any paths cannot be accessed for any reason, they will be skipped and excluded from the constructed tree.
 
-        :param path: The path of the directory to scan.
-        :param exclude_patterns: Compiled exclude patterns. If a directory or file matches any of these, it and its
-            descendents are not included in the scan.
-        :param callbacks: Callbacks for certain events during scanning. See `ScanFilesystemCallbacks`.
+    :param path: The path of the directory to scan.
+    :param exclude_patterns: Compiled exclude patterns. If a directory or file matches any of these, it and its
+        descendents are not included in the scan.
+    :param callbacks: Callbacks for certain events during scanning. See `ScanFilesystemCallbacks`.
     """
 
     path = Path(path)
 
     paths_skipped = False
-    root = Directory('')
+    root = Directory("")
     search_stack: list[Callable[[], None]] = []
     path_segments: list[str] = []
     tree_node_stack = [root]
     is_root = True
 
     def pop_path_segment() -> None:
         del path_segments[-1]
 
     def pop_tree_node() -> None:
         del tree_node_stack[-1]
 
     def visit_directory(search_directory: Path, /) -> None:
         if is_root:
-            directory_path = '/'
+            directory_path = "/"
         else:
             path_segments.append(os.path.normcase(search_directory.name))
             search_stack.append(pop_path_segment)
-            directory_path = '/' + '/'.join(path_segments) + '/'
+            directory_path = "/" + "/".join(path_segments) + "/"
 
         if is_path_excluded(directory_path, exclude_patterns):
             (callbacks.on_exclude)(search_directory)
         else:
             if is_root:
                 tree_node = root
             else:
```

### Comparing `incremental_backup-1.2.0/incremental_backup/backup/plan.py` & `incremental_backup-1.2.1/incremental_backup/backup/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
+import shutil
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
-import shutil
 from typing import Callable, Optional
 
+from incremental_backup._utility import StrPath, path_name_equal
 from incremental_backup.backup import filesystem
 from incremental_backup.backup.sum import BackupSum
 from incremental_backup.meta import BackupManifest
-from incremental_backup._utility import path_name_equal, StrPath
-
 
 __all__ = [
-    'BackupPlan',
-    'execute_backup_plan',
-    'ExecuteBackupPlanCallbacks',
-    'ExecuteBackupPlanResults'
+    "BackupPlan",
+    "execute_backup_plan",
+    "ExecuteBackupPlanCallbacks",
+    "ExecuteBackupPlanResults",
 ]
 
 
 @dataclass
 class BackupPlan:
     """The data required to perform a backup operation.
-        Describes which files are to be copied, as well as information for creating the backup manifest."""
+    Describes which files are to be copied, as well as information for creating the backup manifest."""
 
     @dataclass
     class Directory:
         name: str
         copied_files: list[str] = field(default_factory=list)
         removed_files: list[str] = field(default_factory=list)
         removed_directories: list[str] = field(default_factory=list)
-        subdirectories: list['BackupPlan.Directory'] = field(default_factory=list)
+        subdirectories: list["BackupPlan.Directory"] = field(default_factory=list)
         contains_copied_files: bool = False
         """Indicates if this directory or any of its descendents contain any copied files."""
         contains_removed_items: bool = False
         """Indicates if this directory or any of its descendents contain any removed files or removed directories."""
         removed_directory_file_count: int = 0
         """The total number of files previously contained in the removed subdirectories."""
 
-    root: Directory = field(default_factory=lambda: BackupPlan.Directory(''))
+    root: Directory = field(default_factory=lambda: BackupPlan.Directory(""))
 
     @classmethod
-    def new(cls, source_tree: filesystem.Directory, backup_sum: BackupSum) -> 'BackupPlan':
+    def new(cls, source_tree: filesystem.Directory, backup_sum: BackupSum) -> "BackupPlan":
         """Constructs a backup plan from the backup source directory state and previous backup sum."""
 
         plan = cls()
         plan_directories = [plan.root]
 
         search_stack: list[Callable[[], None]] = []
         backup_sum_stack: list[Optional[BackupSum.Directory]] = [backup_sum.root]
@@ -70,43 +69,58 @@
                 search_stack.append(pop_plan_node)
                 plan_directories.append(plan_directory)
 
                 if backup_sum_stack[-1] is None:
                     backup_sum_directory = None
                 else:
                     backup_sum_directory = next(
-                        (d for d in backup_sum_stack[-1].subdirectories
-                         if path_name_equal(d.name, search_directory.name)), None)
+                        (
+                            d
+                            for d in backup_sum_stack[-1].subdirectories
+                            if path_name_equal(d.name, search_directory.name)
+                        ),
+                        None,
+                    )
                 backup_sum_stack.append(backup_sum_directory)
                 search_stack.append(pop_backup_sum_node)
 
             if backup_sum_directory is None:
                 # Nothing backed up here so far, only possibility is new files to back up.
                 plan_directory.copied_files.extend(f.name for f in search_directory.files)
             else:
                 # Something backed up here before, could have new files, modified files, removed files, removed
                 # subdirectories.
 
                 for current_file in search_directory.files:
                     backed_up_file = next(
-                        (f for f in backup_sum_directory.files if path_name_equal(f.name, current_file.name)), None)
+                        (f for f in backup_sum_directory.files if path_name_equal(f.name, current_file.name)),
+                        None,
+                    )
                     # File never backed up or modified since last backup.
-                    if (backed_up_file is None
-                            or current_file.last_modified > backed_up_file.last_backup.start_info.start_time):
+                    if (
+                        backed_up_file is None
+                        or current_file.last_modified > backed_up_file.last_backup.start_info.start_time
+                    ):
                         plan_directory.copied_files.append(current_file.name)
 
                 plan_directory.removed_files.extend(
-                    f.name for f in backup_sum_directory.files
-                    if not any(path_name_equal(f.name, f2.name) for f2 in search_directory.files))
-
-                removed_directories = \
-                    [d for d in backup_sum_directory.subdirectories
-                     if not any(path_name_equal(d.name, d2.name) for d2 in search_directory.subdirectories)]
+                    f.name
+                    for f in backup_sum_directory.files
+                    if not any(path_name_equal(f.name, f2.name) for f2 in search_directory.files)
+                )
+
+                removed_directories = [
+                    d
+                    for d in backup_sum_directory.subdirectories
+                    if not any(path_name_equal(d.name, d2.name) for d2 in search_directory.subdirectories)
+                ]
                 plan_directory.removed_directories.extend(d.name for d in removed_directories)
-                plan_directory.removed_directory_file_count = sum(d.count_contained_files() for d in removed_directories)
+                plan_directory.removed_directory_file_count = sum(
+                    d.count_contained_files() for d in removed_directories
+                )
 
             # Need to use partial instead of lambda to avoid name rebinding issues.
             search_stack.extend(partial(visit_directory, d) for d in reversed(search_directory.subdirectories))
 
         search_stack.append(partial(visit_directory, source_tree))
         while search_stack:
             search_stack.pop()()
@@ -148,31 +162,34 @@
 
     on_copy_error: Callable[[Path, Path, OSError], None] = lambda src, dest, error: None
     """Called when an error is raised copying a file.
         First argument is the source path, second argument is the destination path, third argument is the raised
         exception."""
 
 
-def execute_backup_plan(backup_plan: BackupPlan, source_directory: StrPath, destination_directory: StrPath,
-                        callbacks: ExecuteBackupPlanCallbacks = ExecuteBackupPlanCallbacks()) \
-        -> ExecuteBackupPlanResults:
+def execute_backup_plan(
+    backup_plan: BackupPlan,
+    source_directory: StrPath,
+    destination_directory: StrPath,
+    callbacks: ExecuteBackupPlanCallbacks = ExecuteBackupPlanCallbacks(),
+) -> ExecuteBackupPlanResults:
     """Enacts a backup plan, copying files and creating the backup manifest.
 
-        If a file cannot be backup up (i.e. copied), it is ignored and excluded from the manifest.
+    If a file cannot be backup up (i.e. copied), it is ignored and excluded from the manifest.
 
-        If a directory cannot be created, no files will be backed up into it or its (planned) child directories.
-        Any files planned to be backed up within it will not be copied and will be excluded from the manifest.
-        However, any removed files or directories within it will still be recorded in the manifest.
-
-        :param backup_plan: The backup plan to enact. Should be based off `source_directory`, otherwise the results will
-            be nonsense.
-        :param source_directory: The backup source directory; where files are copied from.
-        :param destination_directory: The location to copy files to. Need not exist. This directory itself represents
-            the backup source directory.
-        :param callbacks: Callbacks for certain events during execution. See `ExecuteBackupPlanCallbacks`.
+    If a directory cannot be created, no files will be backed up into it or its (planned) child directories.
+    Any files planned to be backed up within it will not be copied and will be excluded from the manifest.
+    However, any removed files or directories within it will still be recorded in the manifest.
+
+    :param backup_plan: The backup plan to enact. Should be based off `source_directory`, otherwise the results will
+        be nonsense.
+    :param source_directory: The backup source directory; where files are copied from.
+    :param destination_directory: The location to copy files to. Need not exist. This directory itself represents
+        the backup source directory.
+    :param callbacks: Callbacks for certain events during execution. See `ExecuteBackupPlanCallbacks`.
     """
 
     manifest = BackupManifest()
     paths_skipped = False
     files_copied = 0
     files_removed = 0
     search_stack: list[Callable[[], None]] = []
@@ -224,16 +241,17 @@
                     else:
                         copied_files.append(file)
                         files_copied += 1
 
         # Keep searching through child directories if:
         #   a) destination directory was created successfully, or
         #   b) destination directory creation failed, but there are still removed items to be recorded in the manifest.
-        children_to_visit = [d for d in reversed(search_directory.subdirectories)
-                             if not mkdir_failed or d.contains_removed_items]
+        children_to_visit = [
+            d for d in reversed(search_directory.subdirectories) if not mkdir_failed or d.contains_removed_items
+        ]
 
         # Only need to create and fill in the manifest entry if there is anything to put in it. I.e. if there are copied
         # files or removed files/directories to be recorded, or child entries. This may not always be true if creating
         # the destination directory failed.
         if copied_files or search_directory.removed_files or search_directory.removed_directories or children_to_visit:
             if is_root:
                 manifest_directory = manifest.root
```

### Comparing `incremental_backup-1.2.0/incremental_backup/backup/sum.py` & `incremental_backup-1.2.1/incremental_backup/backup/sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 from dataclasses import dataclass, field
 from typing import Iterable, Union
 
-from incremental_backup.meta import BackupManifest, BackupMetadata
 from incremental_backup._utility import path_name_equal
+from incremental_backup.meta import BackupManifest, BackupMetadata
 
-
-__all__ = [
-    'BackupSum'
-]
+__all__ = ["BackupSum"]
 
 
 @dataclass
 class BackupSum:
     """Represents the result of applying a sequence of backups.
-        That is, reconstructs the state of the source directory given backup data.
+    That is, reconstructs the state of the source directory given backup data.
     """
 
     @dataclass
     class File:
         name: str
 
         last_backup: BackupMetadata
         """The metadata of the last backup which copied this file."""
 
     @dataclass
     class Directory:
         name: str
-        files: list['BackupSum.File'] = field(default_factory=list)
-        subdirectories: list['BackupSum.Directory'] = field(default_factory=list)
+        files: list["BackupSum.File"] = field(default_factory=list)
+        subdirectories: list["BackupSum.Directory"] = field(default_factory=list)
 
         def count_contained_files(self) -> int:
             """Calculates the total number of files contained in this directory and all its descendents."""
 
             count = 0
             search_stack: list[BackupSum.Directory] = [self]
             while search_stack:
                 search_directory = search_stack.pop()
                 count += len(search_directory.files)
                 search_stack.extend(search_directory.subdirectories)
             return count
 
-    root: Directory = field(default_factory=lambda: BackupSum.Directory(''))
+    root: Directory = field(default_factory=lambda: BackupSum.Directory(""))
     """The root of the reconstructed file/directory structure.
         This object represents the backup source directory.
     """
 
     @classmethod
-    def from_backups(cls, backups: Iterable[BackupMetadata], /) -> 'BackupSum':
+    def from_backups(cls, backups: Iterable[BackupMetadata], /) -> "BackupSum":
         """Constructs a backup sum from previous backup metadata.
 
-            :param backups: 0 or more backups to sum. Should all be for the same source directory, or the results will
-                be meaningless.
+        :param backups: 0 or more backups to sum. Should all be for the same source directory, or the results will
+            be meaningless.
         """
 
         backup_sum = cls()
 
         backups_sorted = sorted(backups, key=lambda backup: backup.start_info.start_time)
 
         # list of all directories. Parent will always occur before child in list.
@@ -68,36 +65,41 @@
                 search_directory = search_stack.pop()
                 if search_directory is None:
                     del sum_stack[-1]
                 else:
                     if not is_root:
                         sum_directory = next(
                             (d for d in sum_stack[-1].subdirectories if path_name_equal(d.name, search_directory.name)),
-                            None)
+                            None,
+                        )
                         if sum_directory is None:
                             sum_directory = BackupSum.Directory(search_directory.name)
                             sum_stack[-1].subdirectories.append(sum_directory)
                             directories.append(sum_directory)
                         sum_stack.append(sum_directory)
 
                     for copied_file in search_directory.copied_files:
                         prev_file = next(
-                            (f for f in sum_stack[-1].files if path_name_equal(f.name, copied_file)), None)
+                            (f for f in sum_stack[-1].files if path_name_equal(f.name, copied_file)),
+                            None,
+                        )
                         if prev_file is None:
                             sum_stack[-1].files.append(BackupSum.File(copied_file, backup))
                         else:
                             prev_file.last_backup = backup
 
                     for removed_file in search_directory.removed_files:
-                        sum_stack[-1].files = \
-                            [f for f in sum_stack[-1].files if not path_name_equal(f.name, removed_file)]
+                        sum_stack[-1].files = [
+                            f for f in sum_stack[-1].files if not path_name_equal(f.name, removed_file)
+                        ]
 
                     for removed_directory in search_directory.removed_directories:
-                        sum_stack[-1].subdirectories = \
-                            [d for d in sum_stack[-1].subdirectories if not path_name_equal(d.name, removed_directory)]
+                        sum_stack[-1].subdirectories = [
+                            d for d in sum_stack[-1].subdirectories if not path_name_equal(d.name, removed_directory)
+                        ]
 
                     search_stack.append(None)
                     search_stack.extend(reversed(search_directory.subdirectories))
                 is_root = False
 
         # Calculate if each directory has nonempty descendents has and remove empty directories.
         # Empty = contains nothing or only directories.
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/backup.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,121 +1,145 @@
 import argparse
 from pathlib import Path
 from typing import Optional, Sequence
 
-from incremental_backup.backup import BackupCallbacks, BackupError, BackupResults, ExecuteBackupPlanCallbacks, \
-    perform_backup, ScanFilesystemCallbacks
+from incremental_backup._utility import print_warning
+from incremental_backup.backup import (
+    BackupCallbacks,
+    BackupError,
+    BackupResults,
+    ExecuteBackupPlanCallbacks,
+    ScanFilesystemCallbacks,
+    perform_backup,
+)
 from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.exception import CommandRuntimeError
 from incremental_backup.meta import ReadBackupsCallbacks
 from incremental_backup.path_exclude import PathExcludePattern
-from incremental_backup._utility import print_warning
 
-
-__all__ = [
-    'BackupCommand'
-]
+__all__ = ["BackupCommand"]
 
 
 class BackupCommand(Command):
     """The program command which creates new backups."""
 
-    COMMAND_STRING = 'backup'
+    COMMAND_STRING = "backup"
 
     @staticmethod
     def add_arg_subparser(subparser, /) -> None:
         """Adds the argparse subparser for the backup command."""
 
         parser = subparser.add_parser(
-            BackupCommand.COMMAND_STRING, description='Creates a new backup.', help='Creates a new backup.')
-        parser.add_argument('source_dir', type=Path, help='Directory to back up.')
-        parser.add_argument('target_dir', type=Path, help='Directory to back up into.')
+            BackupCommand.COMMAND_STRING,
+            description="Creates a new backup.",
+            help="Creates a new backup.",
+        )
+        parser.add_argument("source_dir", type=Path, help="Directory to back up.")
+        parser.add_argument("target_dir", type=Path, help="Directory to back up into.")
         parser.add_argument(
-            '--exclude', nargs='+', type=PathExcludePattern, required=False, help='Path patterns to exclude.')
-        parser.add_argument('--skip-empty', action='store_true', default=False,
-            help='Only back up if there are file changes to record.')
+            "--exclude",
+            nargs="+",
+            type=PathExcludePattern,
+            required=False,
+            help="Path patterns to exclude.",
+        )
+        parser.add_argument(
+            "--skip-empty",
+            action="store_true",
+            default=False,
+            help="Only back up if there are file changes to record.",
+        )
 
     def __init__(self, arguments: argparse.Namespace, /) -> None:
         """
-            :param arguments: The parsed command line arguments object acquired from argparse.
+        :param arguments: The parsed command line arguments object acquired from argparse.
         """
 
         super().__init__(arguments)
         self.source_path: Path = arguments.source_dir
         self.target_path: Path = arguments.target_dir
         self.exclude_patterns: Sequence[PathExcludePattern] = arguments.exclude or ()
         self.skip_empty: bool = arguments.skip_empty
 
     def run(self) -> None:
         """Executes the backup command.
 
-            :except CommandRuntimeError: If an error occurs such that a valid backup cannot be produced.
+        :except CommandRuntimeError: If an error occurs such that a valid backup cannot be produced.
         """
 
         self._print_config()
 
         callbacks = self._backup_callbacks()
 
         try:
             results = perform_backup(
-                self.source_path, self.target_path, self.exclude_patterns, callbacks, self.skip_empty)
+                self.source_path,
+                self.target_path,
+                self.exclude_patterns,
+                callbacks,
+                self.skip_empty,
+            )
         except BackupError as e:
             raise CommandRuntimeError(str(e)) from e
 
         self._print_results(results)
 
     @staticmethod
     def _backup_callbacks() -> BackupCallbacks:
         """Creates the callbacks for `perform_backup()`."""
 
         return BackupCallbacks(
-            on_before_read_previous_backups=lambda: print('Reading previous backups'),
+            on_before_read_previous_backups=lambda: print("Reading previous backups"),
             read_backups=ReadBackupsCallbacks(
-                on_query_entry_error=lambda path, error:
-                    print_warning(f'Failed to query entry in target directory "{path}": {error}'),
-                on_read_metadata_error=lambda path, error:
-                    print_warning(f'Failed to read metadata of previous backup {path.name}: {error}'),
+                on_query_entry_error=lambda path, error: print_warning(
+                    f'Failed to query entry in target directory "{path}": {error}'
+                ),
+                on_read_metadata_error=lambda path, error: print_warning(
+                    f"Failed to read metadata of previous backup {path.name}: {error}"
+                ),
             ),
-            on_after_read_previous_backups=lambda backups: print(f'Read {len(backups)} previous backups'),
-            on_before_initialise_backup=lambda: print('Initialising backup'),
-            on_created_backup_directory=lambda path: print(f'Backup name: {path.name}'),
-            on_before_scan_source=lambda: print('Scanning source directory'),
+            on_after_read_previous_backups=lambda backups: print(f"Read {len(backups)} previous backups"),
+            on_before_initialise_backup=lambda: print("Initialising backup"),
+            on_created_backup_directory=lambda path: print(f"Backup name: {path.name}"),
+            on_before_scan_source=lambda: print("Scanning source directory"),
             scan_source=ScanFilesystemCallbacks(
                 on_exclude=lambda path: print(f'Excluded path "{path}"'),
                 on_listdir_error=lambda path, error: print_warning(f'Failed to enumerate directory "{path}": {error}'),
-                on_metadata_error=lambda path, error: print_warning(f'Failed to get metadata of "{path}": {error}')
+                on_metadata_error=lambda path, error: print_warning(f'Failed to get metadata of "{path}": {error}'),
             ),
-            on_before_copy_files=lambda: print('Copying files'),
+            on_before_copy_files=lambda: print("Copying files"),
             execute_plan=ExecuteBackupPlanCallbacks(
                 on_mkdir_error=lambda path, error: print_warning(f'Failed to create directory "{path}": {error}'),
-                on_copy_error=lambda src, dest, error:
-                    print_warning(f'Failed to copy file "{src}" to "{dest}": {error}')
+                on_copy_error=lambda src, dest, error: print_warning(
+                    f'Failed to copy file "{src}" to "{dest}": {error}'
+                ),
+            ),
+            on_before_save_metadata=lambda: print("Saving metadata"),
+            on_write_complete_info_error=lambda path, error: print_warning(
+                f"Failed to write backup completion information file: {error}"
             ),
-            on_before_save_metadata=lambda: print('Saving metadata'),
-            on_write_complete_info_error=lambda path, error:
-                print_warning(f'Failed to write backup completion information file: {error}')
         )
 
     def _print_config(self) -> None:
         """Prints the configuration of the application to stdout."""
 
-        print(f'Source directory: {self.source_path}')
-        print(f'Target directory: {self.target_path}')
-        print('Exclude patterns:')
+        print(f"Source directory: {self.source_path}")
+        print(f"Target directory: {self.target_path}")
+        print("Exclude patterns:")
         if self.exclude_patterns:
             for pattern in self.exclude_patterns:
-                print(f'  {pattern}')
+                print(f"  {pattern}")
         else:
-            print('  <none>')
+            print("  <none>")
         if self.skip_empty:
-            print('Skip empty backup: yes')
+            print("Skip empty backup: yes")
         print()
 
     @staticmethod
     def _print_results(results: Optional[BackupResults], /) -> None:
         """Prints backup results to the console."""
 
         files_copied = results.files_copied if results else 0
         files_removed = results.files_removed if results else 0
-        print(f'+{files_copied} / -{files_removed} files')
+        print(f"+{files_copied} / -{files_removed} files")
         if results is None:
-            print('Skipping empty backup')
+            print("Skipping empty backup")
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/command.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import argparse
 from typing import ClassVar, Protocol
 
-
-__all__ = [
-    'Command'
-]
+__all__ = ["Command"]
 
 
 class Command(Protocol):
     """Contains the functionality for one "command" of the incremental backup tool.
-        A command is a specific mode of operation, i.e. backup, restore, etc. The principle is the same as Git commands,
-        e.g. "git add", "git commit".
+    A command is a specific mode of operation, i.e. backup, restore, etc. The principle is the same as Git commands,
+    e.g. "git add", "git commit".
     """
 
     COMMAND_STRING: ClassVar[str]
     """Name of the command as specified in the command line arguments."""
 
     @staticmethod
     def add_arg_subparser(subparser, /) -> None:
         """Adds the argparse subparser for the command."""
 
         raise NotImplementedError()
 
-    # TODO: pass args as a struct for backwards compatibility
+    # TODO: (breaking) pass args as a struct for backwards compatibility
     def __init__(self, arguments: argparse.Namespace, /) -> None:
         """
-            :param arguments: The parsed command line arguments object acquired from argparse.
+        :param arguments: The parsed command line arguments object acquired from argparse.
         """
 
     def run(self) -> None:
         """Executes the command."""
 
         raise NotImplementedError()
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/exception.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 from typing import Optional
 
-
-__all__ = [
-    'CommandArgumentError',
-    'CommandError',
-    'CommandRuntimeError'
-]
+__all__ = ["CommandArgumentError", "CommandError", "CommandRuntimeError"]
 
 
 class CommandError(Exception):
     """High-level, unrecoverable application error. Prefer not use this class itself, create a specific subclass.
-        This type of error probably shouldn't be caught except at the highest scope."""
+    This type of error probably shouldn't be caught except at the highest scope."""
 
     def __init__(self, message: str) -> None:
         """
-            :param message: Description of the error. This is typically printed to the console, so should be informative
-                enough for a standard user.
+        :param message: Description of the error. This is typically printed to the console, so should be informative
+            enough for a standard user.
         """
 
         super().__init__(message)
         self.message = message
 
 
 class CommandArgumentError(CommandError):
     """Indicates that command line arguments are invalid."""
 
-    # TODO: remove usage
+    # TODO: (breaking) remove usage
     def __init__(self, message: str, usage: Optional[str] = None) -> None:
         """
-            :param message: Specific description of the error.
-            :param usage: (DEPRECATED) Program usage information string to display to the user.
+        :param message: Specific description of the error.
+        :param usage: (DEPRECATED) Program usage information string to display to the user.
         """
 
         super().__init__(message)
         self.usage = usage
 
 
 class CommandRuntimeError(CommandError):
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/prune.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/prune.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,82 @@
 import argparse
 from pathlib import Path
 
+from incremental_backup._utility import print_warning
 from incremental_backup.cli.command.command import Command
-from incremental_backup.cli.command.exception import CommandArgumentError, CommandRuntimeError
+from incremental_backup.cli.command.exception import (
+    CommandArgumentError,
+    CommandRuntimeError,
+)
 from incremental_backup.meta import ReadBackupsCallbacks
-from incremental_backup.prune import BackupPrunabilityOptions, prune_backups, PruneBackupsCallbacks, \
-    PruneBackupsConfig, PruneBackupsError, PruneBackupsResults
-from incremental_backup._utility import print_warning
+from incremental_backup.prune import (
+    BackupPrunabilityOptions,
+    PruneBackupsCallbacks,
+    PruneBackupsConfig,
+    PruneBackupsError,
+    PruneBackupsResults,
+    prune_backups,
+)
 
-
-__all__ = [
-    'PruneCommand'
-]
+__all__ = ["PruneCommand"]
 
 
 class PruneCommand(Command):
     """The program command which deletes unneeded backups."""
 
-    COMMAND_STRING = 'prune'
+    COMMAND_STRING = "prune"
 
     @staticmethod
     def add_arg_subparser(subparser, /) -> None:
         """Adds the argparse subparser for the prune command."""
 
-        parser = subparser.add_parser(PruneCommand.COMMAND_STRING, description='Removes unneeded backups.',
-            help='Removes unneeded backups.')
-        parser.add_argument('backup_target_dir', type=Path, help='Directory containing backups to operate on.')
-        parser.add_argument('--commit', action='store_true', default=False,
-            help='If not specified, don\'t delete anything.')
-        prune_modes_parser = parser.add_argument_group('Prune modes')
-        prune_modes_parser.add_argument('--delete_empty', action='store_true', default=False,
-            help='Delete backups not containing any changes.')
+        parser = subparser.add_parser(
+            PruneCommand.COMMAND_STRING,
+            description="Removes unneeded backups.",
+            help="Removes unneeded backups.",
+        )
+        parser.add_argument(
+            "backup_target_dir",
+            type=Path,
+            help="Directory containing backups to operate on.",
+        )
+        parser.add_argument(
+            "--commit",
+            action="store_true",
+            default=False,
+            help="If not specified, don't delete anything.",
+        )
+        prune_modes_parser = parser.add_argument_group("Prune modes")
+        # TODO: (breaking) replace underscore with hypen in flag name
+        prune_modes_parser.add_argument(
+            "--delete_empty",
+            action="store_true",
+            default=False,
+            help="Delete backups not containing any changes.",
+        )
 
     def __init__(self, arguments: argparse.Namespace) -> None:
         """
-            :param arguments: The parsed command line arguments object acquired from argparse.
+        :param arguments: The parsed command line arguments object acquired from argparse.
 
-            :except CommandArgumentError: If the arguments are invalid.
+        :except CommandArgumentError: If the arguments are invalid.
         """
 
         super().__init__(arguments)
         self.backup_target_directory: Path = arguments.backup_target_dir
         self.commit: bool = arguments.commit
         self.delete_empty: bool = arguments.delete_empty
 
         if not self.delete_empty:
-            raise CommandArgumentError('At least one prune mode must be specified.')
+            raise CommandArgumentError("At least one prune mode must be specified.")
 
     def run(self) -> None:
         """Executes the prune command.
 
-            :except CommandRuntimeError: If an error occurs such that the prune operation cannot continue.
+        :except CommandRuntimeError: If an error occurs such that the prune operation cannot continue.
         """
 
         self._print_config()
 
         config = self._prune_backups_config()
         callbacks = self._prune_backups_callbacks()
 
@@ -64,48 +86,50 @@
             raise CommandRuntimeError(str(e)) from e
 
         self._print_results(results)
 
     def _print_config(self) -> None:
         """Prints the configuration of the application to stdout."""
 
-        print(f'Backup target directory: {self.backup_target_directory}')
+        print(f"Backup target directory: {self.backup_target_directory}")
         if not self.commit:
-            print(f'Dry run: True')
-        print('Deleting:')
+            print("Dry run: True")
+        print("Deleting:")
         if self.delete_empty:
-            print('  Empty backups')
+            print("  Empty backups")
         print()
 
     def _prune_backups_config(self) -> PruneBackupsConfig:
         return PruneBackupsConfig(
             not self.commit,
-            BackupPrunabilityOptions(prune_empty=self.delete_empty, prune_other_data=False)
+            BackupPrunabilityOptions(prune_empty=self.delete_empty, prune_other_data=False),
         )
 
     @staticmethod
     def _prune_backups_callbacks() -> PruneBackupsCallbacks:
         """Creates the callbacks for `prune_backups()`."""
 
         return PruneBackupsCallbacks(
-            on_before_read_backups=lambda: print('Reading backups'),
+            on_before_read_backups=lambda: print("Reading backups"),
             read_backups=ReadBackupsCallbacks(
-                on_query_entry_error=lambda path, error:
-                    print_warning(f'Failed to query entry in backup target directory "{path}": {error}'),
-                on_read_metadata_error=lambda path, error:
-                    print_warning(f'Failed to read metadata of backup {path.name}: {error}'),
+                on_query_entry_error=lambda path, error: print_warning(
+                    f'Failed to query entry in backup target directory "{path}": {error}'
+                ),
+                on_read_metadata_error=lambda path, error: print_warning(
+                    f"Failed to read metadata of backup {path.name}: {error}"
+                ),
             ),
-            on_after_read_backups=lambda backups: print(f'Read {len(backups)} backups'),
-            on_selected_backups=lambda backups: print(f'Pruning {len(backups)} backups'),
-            on_delete_error=lambda path, error: print_warning(f'Failed to delete backup "{path}": {error}')
+            on_after_read_backups=lambda backups: print(f"Read {len(backups)} backups"),
+            on_selected_backups=lambda backups: print(f"Pruning {len(backups)} backups"),
+            on_delete_error=lambda path, error: print_warning(f'Failed to delete backup "{path}": {error}'),
         )
 
     def _print_results(self, results: PruneBackupsResults) -> None:
         """Prints backup prune results to the console."""
 
         print()
         if not self.commit:
-            print('DRY RUN - simulated results only')
+            print("DRY RUN - simulated results only")
         backup_count = results.total_backups_removed + results.backups_remaining
         removed_percent = 100 * results.total_backups_removed / backup_count if backup_count > 0 else 0
-        print(f'Deleted {results.total_backups_removed} / {backup_count} backups ({removed_percent:.2f}%)')
-        print(f'  {results.empty_backups_removed} empty')
+        print(f"Deleted {results.total_backups_removed} / {backup_count} backups ({removed_percent:.2f}%)")
+        print(f"  {results.empty_backups_removed} empty")
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/registry.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from collections.abc import Sequence
 
-from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.backup import BackupCommand
-from incremental_backup.cli.command.restore import RestoreCommand
+from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.prune import PruneCommand
+from incremental_backup.cli.command.restore import RestoreCommand
 
-
-__all__ = [
-    'COMMAND_CLASSES',
-    'get_command_class'
-]
+__all__ = ["COMMAND_CLASSES", "get_command_class"]
 
 
-COMMAND_CLASSES: Sequence[type[Command]] = (
-    BackupCommand,
-    RestoreCommand,
-    PruneCommand
-)
+COMMAND_CLASSES: Sequence[type[Command]] = (BackupCommand, RestoreCommand, PruneCommand)
 """List of all commands recognised by the program.
     Add or remove commands here.
 """
 
 
 def get_command_class(command_string: str, /) -> type[Command]:
     """Obtains a command class from its command line string.
-    
-        :except ValueError: If the command is not found.
+
+    :except ValueError: If the command is not found.
     """
 
     for command in COMMAND_CLASSES:
         if command.COMMAND_STRING == command_string:
             return command
-    raise ValueError('Command not found')
+    raise ValueError("Command not found")
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/command/restore.py` & `incremental_backup-1.2.1/incremental_backup/cli/command/restore.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import argparse
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Union
 
+from incremental_backup._utility import print_warning
 from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.exception import CommandRuntimeError
 from incremental_backup.meta import ReadBackupsCallbacks
-from incremental_backup.restore import perform_restore, RestoreCallbacks, RestoreError, RestoreFilesCallbacks, RestoreResults
-from incremental_backup._utility import print_warning
-
+from incremental_backup.restore import (
+    RestoreCallbacks,
+    RestoreError,
+    RestoreFilesCallbacks,
+    RestoreResults,
+    perform_restore,
+)
 
-__all__ = [
-    'RestoreCommand'
-]
+__all__ = ["RestoreCommand"]
 
 
 # TODO? a command line flag to abort the restore if any backup can't be read
 
 
 class RestoreCommand(Command):
     """The program command which restores files from backups."""
 
-    COMMAND_STRING = 'restore'
+    COMMAND_STRING = "restore"
 
     @staticmethod
     def add_arg_subparser(subparser, /) -> None:
         """Adds the argparse subparser for the restore command."""
 
-        parser = subparser.add_parser(RestoreCommand.COMMAND_STRING, description='Restores files from backups.',
-                                      help='Restores files from backups.')
-        parser.add_argument('backup_target_dir', type=Path, help='Directory containing backups to restore from.')
-        parser.add_argument('destination_dir', type=Path, help='Directory to restore into.')
-        parser.add_argument('backup_or_time', type=RestoreCommand._parse_backup_name_or_time,
-                            nargs='?', help='Name or timestamp of latest backup to restore.')
+        parser = subparser.add_parser(
+            RestoreCommand.COMMAND_STRING,
+            description="Restores files from backups.",
+            help="Restores files from backups.",
+        )
+        parser.add_argument(
+            "backup_target_dir",
+            type=Path,
+            help="Directory containing backups to restore from.",
+        )
+        parser.add_argument("destination_dir", type=Path, help="Directory to restore into.")
+        parser.add_argument(
+            "backup_or_time",
+            type=RestoreCommand._parse_backup_name_or_time,
+            nargs="?",
+            help="Name or timestamp of latest backup to restore.",
+        )
 
     def __init__(self, arguments: argparse.Namespace, /) -> None:
         """
-            :param arguments: The parsed command line arguments object acquired from argparse.
+        :param arguments: The parsed command line arguments object acquired from argparse.
         """
 
         super().__init__(arguments)
         self.backup_target_directory: Path = arguments.backup_target_dir
         self.destination_directory: Path = arguments.destination_dir
         if arguments.backup_or_time is None:
             backup_name = None
@@ -53,35 +67,40 @@
             backup_time = None
         self.backup_name: Optional[str] = backup_name
         self.backup_time: Optional[datetime] = backup_time
 
     def run(self) -> None:
         """Executes the restore command.
 
-            :except CommandRuntimeError: If an error occurs such that the restore operation cannot continue.
+        :except CommandRuntimeError: If an error occurs such that the restore operation cannot continue.
         """
 
         self._print_config()
 
         callbacks = self._restore_callbacks()
 
         try:
             results = perform_restore(
-                self.backup_target_directory, self.destination_directory, self.backup_name, self.backup_time, callbacks)
+                self.backup_target_directory,
+                self.destination_directory,
+                self.backup_name,
+                self.backup_time,
+                callbacks,
+            )
         except RestoreError as e:
             raise CommandRuntimeError(str(e)) from e
 
         self._print_results(results)
 
     @staticmethod
     def _parse_backup_name_or_time(name_or_time: str, /) -> Union[str, datetime]:
         """Parses the "backup name or timestamp" command line argument.
-            Valid values are backup names (i.e. alphanumeric) and ISO-8601 timestamps.
+        Valid values are backup names (i.e. alphanumeric) and ISO-8601 timestamps.
 
-            :except ArgumentTypeError: If the value is neither a valid backup name nor timestamp.
+        :except ArgumentTypeError: If the value is neither a valid backup name nor timestamp.
         """
 
         if name_or_time.isascii() and name_or_time.isalnum() and len(name_or_time) >= 10:
             # Is probably a backup name.
             return name_or_time
 
         try:
@@ -89,50 +108,53 @@
             if time.tzinfo is None:
                 local_tz = datetime.now().astimezone().tzinfo
                 time = time.replace(tzinfo=local_tz)
             return time
         except ValueError:
             pass
 
-        raise argparse.ArgumentTypeError('Must be a backup name or ISO-8601 timestamp.')
+        raise argparse.ArgumentTypeError("Must be a backup name or ISO-8601 timestamp.")
 
     @staticmethod
     def _restore_callbacks() -> RestoreCallbacks:
         """Creates the callbacks for `perform_restore()`."""
 
         return RestoreCallbacks(
-            on_before_read_previous_backups=lambda: print('Reading previous backups'),
+            on_before_read_previous_backups=lambda: print("Reading previous backups"),
             read_backups=ReadBackupsCallbacks(
-                on_query_entry_error=lambda path, error:
-                    print_warning(f'Failed to query entry in backup target directory "{path}": {error}'),
-                on_read_metadata_error=lambda path, error:
-                    print_warning(f'Failed to read metadata of previous backup {path.name}: {error}'),
+                on_query_entry_error=lambda path, error: print_warning(
+                    f'Failed to query entry in backup target directory "{path}": {error}'
+                ),
+                on_read_metadata_error=lambda path, error: print_warning(
+                    f"Failed to read metadata of previous backup {path.name}: {error}"
+                ),
             ),
-            on_after_read_previous_backups=lambda backups: print(f'Read {len(backups)} previous backups'),
-            on_selected_backups=lambda backups: print(f'Using {len(backups)} for restore'),
-            on_before_initialise_restore=lambda: print('Initialising restoration'),
-            on_before_restore_files=lambda: print('Copying files'),
+            on_after_read_previous_backups=lambda backups: print(f"Read {len(backups)} previous backups"),
+            on_selected_backups=lambda backups: print(f"Using {len(backups)} for restore"),
+            on_before_initialise_restore=lambda: print("Initialising restoration"),
+            on_before_restore_files=lambda: print("Copying files"),
             restore_files=RestoreFilesCallbacks(
                 on_mkdir_error=lambda path, error: print_warning(f'Failed to create directory "{path}": {error}'),
-                on_copy_error=lambda src, dest, error:
-                    print_warning(f'Failed to copy file "{src}" to "{dest}": {error}')
-            )
+                on_copy_error=lambda src, dest, error: print_warning(
+                    f'Failed to copy file "{src}" to "{dest}": {error}'
+                ),
+            ),
         )
 
     def _print_config(self) -> None:
         """Prints the configuration of the application to stdout."""
 
-        print(f'Backup target directory: {self.backup_target_directory}')
-        print(f'Destination directory: {self.destination_directory}')
+        print(f"Backup target directory: {self.backup_target_directory}")
+        print(f"Destination directory: {self.destination_directory}")
         if self.backup_name is not None:
-            print(f'Restore up to backup {self.backup_name}')
+            print(f"Restore up to backup {self.backup_name}")
         elif self.backup_time is not None:
-            print(f'Restore up to {self.backup_time.isoformat()}')
+            print(f"Restore up to {self.backup_time.isoformat()}")
         else:
-            print('Restore up to latest backup')
+            print("Restore up to latest backup")
         print()
 
     @staticmethod
     def _print_results(results: RestoreResults, /) -> None:
         """Prints restore results to the console."""
 
-        print(f'Restored {results.files_restored} files')
+        print(f"Restored {results.files_restored} files")
```

### Comparing `incremental_backup-1.2.0/incremental_backup/cli/main.py` & `incremental_backup-1.2.1/incremental_backup/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 import argparse
 import sys
 from typing import NoReturn, Sequence
 
-from incremental_backup.cli.command import COMMAND_CLASSES, CommandArgumentError, CommandError, get_command_class
 from incremental_backup._utility import print_error
+from incremental_backup.cli.command import (
+    COMMAND_CLASSES,
+    CommandArgumentError,
+    CommandError,
+    get_command_class,
+)
 
-
-__all__ = [
-    'cli_entrypoint',
-    'cli_main'
-]
+__all__ = ["cli_entrypoint", "cli_main"]
 
 
 def cli_entrypoint() -> NoReturn:
     """Process-level entrypoint of the incremental backup program.
-        Collects arguments from `sys.argv`, performs all processing, then terminates the process with `sys.exit()`."""
+    Collects arguments from `sys.argv`, performs all processing, then terminates the process with `sys.exit()`."""
 
     exit_code = cli_main(sys.argv)
     sys.exit(exit_code)
 
 
 def cli_main(arguments: Sequence[str], /) -> int:
     """Intermediate entrypoint function which may be handy for testing purposes.
 
-        :param arguments: The program command line arguments.
-        :return: Process exit code.
+    :param arguments: The program command line arguments.
+    :return: Process exit code.
     """
 
     # Strip off the "program name" argument.
     arguments = arguments[1:]
 
     try:
         arg_parser = _get_argument_parser()
         parsed_arguments = arg_parser.parse_args(arguments)
         command_class = get_command_class(parsed_arguments.command)
         command_instance = command_class(parsed_arguments)
         command_instance.run()
         return EXIT_CODE_SUCCESS
     except CommandArgumentError as e:
-        if e.usage is None: # TODO: remove when usage is removed
+        if e.usage is None:  # TODO: (breaking) remove when usage is removed
             arg_parser.print_usage(sys.stderr)
         else:
             print(e.usage, file=sys.stderr)
         print()
-        print(f'{arg_parser.prog}: error: {e.message}', file=sys.stderr)
+        print(f"{arg_parser.prog}: error: {e.message}", file=sys.stderr)
         return EXIT_CODE_INVALID_ARGUMENTS
     except CommandError as e:
         print_error(str(e))
         return EXIT_CODE_GENERAL_ERROR
     except Exception as e:
-        print_error(f'Unhandled exception: {repr(e)}')
+        print_error(f"Unhandled exception: {repr(e)}")
         return EXIT_CODE_LOGIC_ERROR
 
 
 def _get_argument_parser() -> argparse.ArgumentParser:
     """Creates the command line argument parser. Adds subparsers for each command."""
 
-    arg_parser = _ArgumentParser('incremental_backup', description='Incremental backup tool.')
-    arg_subparser = arg_parser.add_subparsers(title='commands', required=True, dest='command')
+    arg_parser = _ArgumentParser("incremental_backup", description="Incremental backup tool.")
+    arg_subparser = arg_parser.add_subparsers(title="commands", required=True, dest="command")
 
     for cls in COMMAND_CLASSES:
         cls.add_arg_subparser(arg_subparser)
 
     return arg_parser
 
 
 class _ArgumentParser(argparse.ArgumentParser):
     """Custom `argparse.ArgumentParser` implementation so we can throw exceptions for invalid arguments instead of
-        exiting the process."""
+    exiting the process."""
 
     def error(self, message: str) -> NoReturn:
         raise CommandArgumentError(message)
 
 
 # Process exit codes.
 EXIT_CODE_SUCCESS = 0
```

### Comparing `incremental_backup-1.2.0/incremental_backup/meta/complete_info.py` & `incremental_backup-1.2.1/incremental_backup/meta/complete_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
+import json
 from dataclasses import dataclass
 from datetime import datetime
-import json
-from typing import Any, cast, NoReturn, Optional
+from typing import Any, NoReturn, Optional, cast
 
 from incremental_backup._utility import StrPath
 
-
 __all__ = [
-    'BackupCompleteInfo',
-    'BackupCompleteInfoParseError',
-    'deserialise_backup_complete_info',
-    'read_backup_complete_info_file',
-    'serialise_backup_complete_info',
-    'write_backup_complete_info_file'
+    "BackupCompleteInfo",
+    "BackupCompleteInfoParseError",
+    "deserialise_backup_complete_info",
+    "read_backup_complete_info_file",
+    "serialise_backup_complete_info",
+    "write_backup_complete_info_file",
 ]
 
 
 @dataclass(frozen=True)
 class BackupCompleteInfo:
     """Information pertaining to the completion of a backup operation."""
 
@@ -27,86 +26,86 @@
     """Indicates if any paths were skipped due to filesystem errors (does NOT include explicitly excluded paths)."""
 
 
 def serialise_backup_complete_info(value: BackupCompleteInfo, /) -> str:
     """Writes backup completion information to a string."""
 
     json_data = {
-        'end_time': value.end_time.isoformat(),
-        'paths_skipped': value.paths_skipped
+        "end_time": value.end_time.isoformat(),
+        "paths_skipped": value.paths_skipped,
     }
     return json.dumps(json_data, indent=4, ensure_ascii=False)
 
 
 def write_backup_complete_info_file(path: StrPath, value: BackupCompleteInfo, /) -> None:
     """Writes backup completion information to file.
 
-        :except OSError: If the file could not be written to.
+    :except OSError: If the file could not be written to.
     """
 
-    with open(path, 'w', encoding='utf8') as file:
+    with open(path, "w", encoding="utf8") as file:
         file.write(serialise_backup_complete_info(value))
 
 
 def deserialise_backup_complete_info(string: str, /) -> BackupCompleteInfo:
     """Reads backup completion information from a string.
 
-        :except BackupCompleteInfoParseError: If the string is not valid backup completion information.
+    :except BackupCompleteInfoParseError: If the string is not valid backup completion information.
     """
 
     def parse_error(reason: str, e: Optional[Exception] = None, /) -> NoReturn:
         if e is None:
             raise BackupCompleteInfoParseError(reason)
         else:
             raise BackupCompleteInfoParseError(reason) from e
 
     try:
         json_data = json.loads(string)
     except json.JSONDecodeError as e:
         parse_error(str(e), e)
 
     if not isinstance(json_data, dict):
-        parse_error('Expected an object')
+        parse_error("Expected an object")
     json_data = cast(dict[Any, Any], json_data)
 
-    fields = {'end_time', 'paths_skipped'}
+    fields = {"end_time", "paths_skipped"}
     if set(json_data.keys()) != fields:
-        parse_error(f'Expected fields {fields}')
+        parse_error(f"Expected fields {fields}")
 
     try:
-        end_time = datetime.fromisoformat(json_data['end_time'])
+        end_time = datetime.fromisoformat(json_data["end_time"])
     except (TypeError, ValueError) as e:
         parse_error('Field "end_time" must be an ISO-8601 date string', e)
 
-    if not isinstance(json_data['paths_skipped'], bool):
+    if not isinstance(json_data["paths_skipped"], bool):
         parse_error('Field "paths_skipped" must be a boolean')
-    paths_skipped = json_data['paths_skipped']
+    paths_skipped = json_data["paths_skipped"]
 
     return BackupCompleteInfo(end_time, paths_skipped)
 
 
 def read_backup_complete_info_file(path: StrPath, /) -> BackupCompleteInfo:
     """Reads backup completion information from file.
 
-        :except OSError: If the file could not be read.
-        :except BackupCompleteInfoParseError: If the file is not valid backup completion information.
+    :except OSError: If the file could not be read.
+    :except BackupCompleteInfoParseError: If the file is not valid backup completion information.
     """
 
     try:
-        with open(path, 'r', encoding='utf8') as file:
+        with open(path, "r", encoding="utf8") as file:
             return deserialise_backup_complete_info(file.read())
     except BackupCompleteInfoParseError as e:
         # TODO: may be nicer to raise from the cause of e
         raise BackupCompleteInfoParseError(e.reason, str(path)) from e
 
 
 class BackupCompleteInfoParseError(Exception):
     """Raised when a backup completion information file cannot be parsed due to invalid format."""
 
     def __init__(self, reason: str, file_path: Optional[str] = None) -> None:
         if file_path is None:
-            message = f'Failed to parse backup start info: {reason}'
+            message = f"Failed to parse backup start info: {reason}"
         else:
             message = f'Failed to parse backup start info file "{file_path}": {reason}'
         super().__init__(message)
         self.reason = reason
         self.file_path = file_path
```

### Comparing `incremental_backup-1.2.0/incremental_backup/meta/manifest.py` & `incremental_backup-1.2.1/incremental_backup/meta/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-from dataclasses import dataclass, field
 import json
-from typing import Any, cast, Iterator, NoReturn, Optional, Union
-
-from incremental_backup._utility import path_name_equal, StrPath
+from dataclasses import dataclass, field
+from typing import Any, Iterator, NoReturn, Optional, Union, cast
 
+from incremental_backup._utility import StrPath, path_name_equal
 
 __all__ = [
-    'BackupManifest',
-    'BackupManifestParseError',
-    'deserialise_backup_manifest',
-    'read_backup_manifest_file',
-    'serialise_backup_manifest',
-    'write_backup_manifest_file'
+    "BackupManifest",
+    "BackupManifestParseError",
+    "deserialise_backup_manifest",
+    "read_backup_manifest_file",
+    "serialise_backup_manifest",
+    "write_backup_manifest_file",
 ]
 
 
 @dataclass
 class BackupManifest:
     """Lists the files and directories copied and removed (compared to the previous backup).
-        The data is represented in a tree structure like a filesystem.
+    The data is represented in a tree structure like a filesystem.
     """
 
     @dataclass
     class Directory:
         name: str
         copied_files: list[str] = field(default_factory=list)
         removed_files: list[str] = field(default_factory=list)
         removed_directories: list[str] = field(default_factory=list)
-        subdirectories: list['BackupManifest.Directory'] = field(default_factory=list)
+        subdirectories: list["BackupManifest.Directory"] = field(default_factory=list)
 
-    root: Directory = field(default_factory=lambda: BackupManifest.Directory(''))
+    root: Directory = field(default_factory=lambda: BackupManifest.Directory(""))
     """The root of the manifest tree. This object represents the backup source directory."""
 
 
 def serialise_backup_manifest(value: BackupManifest, /) -> str:
     """Writes a backup manifest to a string."""
 
     def search(manifest: BackupManifest, /) -> Iterator[Optional[BackupManifest.Directory]]:
@@ -41,131 +40,132 @@
         while stack:
             node = stack.pop()
             yield node
             if node is not None:
                 stack.append(None)
                 stack.extend(reversed(node.subdirectories))
 
-    def compress_backtracks(nodes: Iterator[Optional[BackupManifest.Directory]], /) \
-            -> Iterator[Union[BackupManifest.Directory, int]]:
+    def compress_backtracks(
+        nodes: Iterator[Optional[BackupManifest.Directory]], /
+    ) -> Iterator[Union[BackupManifest.Directory, int]]:
         backtrack_count = 0
         for node in nodes:
             if node is None:
                 backtrack_count += 1
             else:
                 if backtrack_count > 0:
                     yield backtrack_count
                     backtrack_count = 0
                 yield node
         # Also trims trailing backtracks since they are not required.
 
     def node_to_object(node: Union[BackupManifest.Directory, int], /) -> Union[dict[str, Union[str, list[str]]], str]:
         if isinstance(node, int):
-            return f'^{node}'
+            return f"^{node}"
         else:
-            obj: dict[str, Union[str, list[str]]] = {'n': node.name}
+            obj: dict[str, Union[str, list[str]]] = {"n": node.name}
             if node.copied_files:
-                obj['cf'] = node.copied_files
+                obj["cf"] = node.copied_files
             if node.removed_files:
-                obj['rf'] = node.removed_files
+                obj["rf"] = node.removed_files
             if node.removed_directories:
-                obj['rd'] = node.removed_directories
+                obj["rd"] = node.removed_directories
             return obj
 
     nodes = list(compress_backtracks(search(value)))
     json_data = [node_to_object(node) for node in nodes]
 
     return json.dumps(json_data, indent=0, ensure_ascii=False)
 
 
 def write_backup_manifest_file(path: StrPath, value: BackupManifest, /) -> None:
     """Writes a backup manifest to file.
 
-        :except OSError: If the file could not be written to.
+    :except OSError: If the file could not be written to.
     """
 
-    with open(path, 'w', encoding='utf8') as file:
+    with open(path, "w", encoding="utf8") as file:
         file.write(serialise_backup_manifest(value))
 
 
 def deserialise_backup_manifest(string: str, /) -> BackupManifest:
     """Reads a backup manifest from a string.
 
-        :except BackupManifestParseError: If the string is not a valid backup manifest.
+    :except BackupManifestParseError: If the string is not a valid backup manifest.
     """
 
     def parse_error(reason: str, e: Optional[Exception] = None, /) -> NoReturn:
         if e is None:
             raise BackupManifestParseError(reason)
         else:
             raise BackupManifestParseError(reason) from e
 
     def parse_directory_entry(entry: dict[Any, Any], entry_num: int, /) -> tuple[str, list[str], list[str], list[str]]:
         try:
-            name = entry.pop('n')
+            name = entry.pop("n")
         except KeyError as e:
             # Can allow the name to be missing for the source directory, it's not used anyway.
             if entry_num == 1:
-                name = ''
+                name = ""
             else:
                 parse_error(f'Entry {entry_num}: missing required field "n"', e)
         if not isinstance(name, str):
             parse_error(f'Entry {entry_num}: field "n" must be a string')
 
-        copied_files = entry.pop('cf', [])
+        copied_files = entry.pop("cf", [])
         if not isinstance(copied_files, list) or not all(isinstance(f, str) for f in copied_files):
             parse_error(f'Entry {entry_num}: field "cf" must be a list of strings')
         copied_files = cast(list[str], copied_files)
 
-        removed_files = entry.pop('rf', [])
+        removed_files = entry.pop("rf", [])
         if not isinstance(removed_files, list) or not all(isinstance(f, str) for f in removed_files):
             parse_error(f'Entry {entry_num}: field "rf" must be a list of strings')
         removed_files = cast(list[str], removed_files)
 
-        removed_directories = entry.pop('rd', [])
+        removed_directories = entry.pop("rd", [])
         if not isinstance(removed_directories, list) or not all(isinstance(f, str) for f in removed_directories):
             parse_error(f'Entry {entry_num}: field "rd" must be a list of strings')
         removed_directories = cast(list[str], removed_directories)
 
         if extra_fields := list(entry.keys()):
-            parse_error(f'Entry {entry_num}: invalid fields {extra_fields}')
+            parse_error(f"Entry {entry_num}: invalid fields {extra_fields}")
 
         return name, copied_files, removed_files, removed_directories
 
     def parse_backtrack(entry: str, entry_num: int, /) -> int:
-        if not entry.startswith('^'):
+        if not entry.startswith("^"):
             parse_error(f'Entry: {entry_num}: invalid value, backtrack must be in form "^n"')
 
         try:
             backtracks = int(entry[1:])
         except ValueError:
             pass
         else:
             if backtracks >= 1:
                 return backtracks
-        parse_error(f'Entry {entry_num}: invalid backtrack amount, must be positive integer')
+        parse_error(f"Entry {entry_num}: invalid backtrack amount, must be positive integer")
 
     try:
         json_data = json.loads(string)
     except json.JSONDecodeError as e:
         parse_error(str(e), e)
 
     if not isinstance(json_data, list):
-        parse_error('Expected a list')
+        parse_error("Expected a list")
     json_data = cast(list[Any], json_data)
 
     backup_manifest = BackupManifest()
     directory_stack: list[BackupManifest.Directory] = []
     for entry_num, entry in enumerate(json_data, 1):
         if isinstance(entry, str):
             backtracks = parse_backtrack(entry, entry_num)
 
             # Backtrack to parent directory.
             if len(directory_stack) <= backtracks:
-                parse_error(f'Entry {entry_num}: cannot backtrack past backup source directory')
+                parse_error(f"Entry {entry_num}: cannot backtrack past backup source directory")
             del directory_stack[-backtracks:]
         elif isinstance(entry, dict):
             entry = cast(dict[Any, Any], entry)
             # Directory entry.
 
             name, copied_files, removed_files, removed_directories = parse_directory_entry(entry, entry_num)
 
@@ -175,53 +175,56 @@
                 directory.copied_files = copied_files
                 directory.removed_files = removed_files
                 directory.removed_directories = removed_directories
             else:
                 # Not root directory.
 
                 # We explicitly allow re-entering a directory. It shouldn't occur in practice, though.
-                directory = next((d for d in directory_stack[-1].subdirectories if path_name_equal(d.name, name)), None)
+                directory = next(
+                    (d for d in directory_stack[-1].subdirectories if path_name_equal(d.name, name)),
+                    None,
+                )
                 if directory is None:
                     # We haven't entered this directory yet, need to create it.
                     directory = BackupManifest.Directory(name, copied_files, removed_files, removed_directories)
                     directory_stack[-1].subdirectories.append(directory)
                 else:
                     # Already entered this directory, need to update it.
 
                     # Technically we should check if these have already been added, but I don't think it will cause any
                     # issues, and checking would cost performance.
                     directory.copied_files.extend(copied_files)
                     directory.removed_files.extend(removed_files)
                     directory.removed_directories.extend(removed_directories)
             directory_stack.append(directory)
         else:
-            parse_error(f'Entry {entry_num}: invalid value, expected object or string')
+            parse_error(f"Entry {entry_num}: invalid value, expected object or string")
 
     return backup_manifest
 
 
 def read_backup_manifest_file(path: StrPath, /) -> BackupManifest:
     """Reads a backup manifest from file.
 
-        :except OSError: If the file could not be read.
-        :except BackupManifestParseError: If the file is not a valid backup manifest.
+    :except OSError: If the file could not be read.
+    :except BackupManifestParseError: If the file is not a valid backup manifest.
     """
 
     try:
-        with open(path, 'r', encoding='utf8') as file:
+        with open(path, "r", encoding="utf8") as file:
             return deserialise_backup_manifest(file.read())
     except BackupManifestParseError as e:
         # TODO: may be nicer to raise from the cause of e
         raise BackupManifestParseError(e.reason, str(path)) from e
 
 
 class BackupManifestParseError(Exception):
     """Raised when a backup manifest file cannot be parsed due to invalid format."""
 
     def __init__(self, reason: str, file_path: Optional[str] = None) -> None:
         if file_path is None:
-            message = f'Failed to parse backup manifest: {reason}'
+            message = f"Failed to parse backup manifest: {reason}"
         else:
             message = f'Failed to parse backup manifest file "{file_path}": {reason}'
         super().__init__(message)
         self.reason = reason
         self.file_path = file_path
```

### Comparing `incremental_backup-1.2.0/incremental_backup/meta/meta.py` & `incremental_backup-1.2.1/incremental_backup/meta/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,102 @@
 from dataclasses import dataclass
 from pathlib import Path
 from random import Random
 from typing import Callable, Union
 
-from incremental_backup.meta.manifest import BackupManifest, BackupManifestParseError, read_backup_manifest_file
-from incremental_backup.meta.start_info import BackupStartInfo, BackupStartInfoParseError, read_backup_start_info_file
 from incremental_backup._utility import StrPath
-
+from incremental_backup.meta.manifest import (
+    BackupManifest,
+    BackupManifestParseError,
+    read_backup_manifest_file,
+)
+from incremental_backup.meta.start_info import (
+    BackupStartInfo,
+    BackupStartInfoParseError,
+    read_backup_start_info_file,
+)
 
 __all__ = [
-    'BACKUP_DIRECTORY_CREATION_RETRIES',
-    'BACKUP_NAME_LENGTH',
-    'BackupDirectoryCreationError',
-    'BackupMetadata',
-    'COMPLETE_INFO_FILENAME',
-    'create_new_backup_directory',
-    'DATA_DIRECTORY_NAME',
-    'generate_backup_name',
-    'check_if_probably_backup',
-    'MANIFEST_FILENAME',
-    'read_backup_metadata',
-    'read_backups',
-    'ReadBackupsCallbacks',
-    'START_INFO_FILENAME'
+    "BACKUP_DIRECTORY_CREATION_RETRIES",
+    "BACKUP_NAME_LENGTH",
+    "BackupDirectoryCreationError",
+    "BackupMetadata",
+    "COMPLETE_INFO_FILENAME",
+    "create_new_backup_directory",
+    "DATA_DIRECTORY_NAME",
+    "generate_backup_name",
+    "check_if_probably_backup",
+    "MANIFEST_FILENAME",
+    "read_backup_metadata",
+    "read_backups",
+    "ReadBackupsCallbacks",
+    "START_INFO_FILENAME",
 ]
 
 
-MANIFEST_FILENAME = 'manifest.json'
+MANIFEST_FILENAME = "manifest.json"
 """The name of the backup manifest file within a backup directory."""
 
-START_INFO_FILENAME = 'start.json'
+START_INFO_FILENAME = "start.json"
 """The name of the backup start information file within a backup directory."""
 
-COMPLETE_INFO_FILENAME = 'completion.json'
+COMPLETE_INFO_FILENAME = "completion.json"
 """The name of the backup completion information file within a backup directory."""
 
-DATA_DIRECTORY_NAME = 'data'
+DATA_DIRECTORY_NAME = "data"
 """The name of the backup data directory within a backup directory."""
 
 
 def check_if_probably_backup(directory: StrPath, /) -> bool:
     """Checks if a directory is likely to be a backup directory.
 
-        If the directory is a valid backup, and is accessible, then this function will return `True`.
-        If the directory is not a valid backup, then this function will probably return `False`, but may return `True`.
+    If the directory is a valid backup, and is accessible, then this function will return `True`.
+    If the directory is not a valid backup, then this function will probably return `False`, but may return `True`.
 
-        :except OSError: If querying the directory or its contents failed (excluding if the directory or its expected
-            contents don't exist).
+    :except OSError: If querying the directory or its contents failed (excluding if the directory or its expected
+        contents don't exist).
     """
 
     directory = Path(directory)
 
     start_info_path = directory / START_INFO_FILENAME
     manifest_path = directory / MANIFEST_FILENAME
     # Do not check for exact length of backup name, in case we change it in the future.
     # Also check name properties first to avoid hitting the filesystem if possible.
     name = directory.name
-    return (len(name) >= 10 and name.isascii() and name.isalnum() and directory.is_dir() and start_info_path.is_file()
-            and manifest_path.is_file())
+    return (
+        len(name) >= 10
+        and name.isascii()
+        and name.isalnum()
+        and directory.is_dir()
+        and start_info_path.is_file()
+        and manifest_path.is_file()
+    )
 
 
 @dataclass(frozen=True)
 class BackupMetadata:
     """All useful metadata for a backup."""
 
     name: str
     start_info: BackupStartInfo
     manifest: BackupManifest
 
     # Backup completion information is not here because it is currently not read by the application.
 
 
-# TODO: should refactor and simplify exceptions. Don't need so fine grained.
+# TODO: (breaking) should refactor and simplify exceptions. Don't need so fine grained.
+
 
 def read_backup_metadata(backup_directory: StrPath, /) -> BackupMetadata:
     """Reads the metadata of a backup, i.e. the name, start information, and manifest.
 
-        :except OSError: If a metadata file could not be read.
-        :except BackupStartInfoParseError: If the backup start information file could not be parsed.
-        :except BackupManifestParseError: If the backup manifest file could not be parsed.
+    :except OSError: If a metadata file could not be read.
+    :except BackupStartInfoParseError: If the backup start information file could not be parsed.
+    :except BackupManifestParseError: If the backup manifest file could not be parsed.
     """
 
     backup_directory = Path(backup_directory)
     name = backup_directory.name
     start_info = read_backup_start_info_file(backup_directory / START_INFO_FILENAME)
     manifest = read_backup_manifest_file(backup_directory / MANIFEST_FILENAME)
     return BackupMetadata(name, start_info, manifest)
@@ -90,41 +104,48 @@
 
 @dataclass(frozen=True)
 class ReadBackupsCallbacks:
     on_query_entry_error: Callable[[Path, OSError], None] = lambda path, error: None
     """Called when querying an entry in the target directory fails.
         First argument is the path to the file/directory, second argument is the raised exception."""
 
-    on_read_metadata_error: Callable[[Path, Union[OSError, BackupStartInfoParseError, BackupManifestParseError]], None] \
-        = lambda path, error: None
+    on_read_metadata_error: Callable[
+        [Path, Union[OSError, BackupStartInfoParseError, BackupManifestParseError]],
+        None,
+    ] = lambda path, error: None
     """Called when reading the metadata of a backup fails.
         First argument is the path of the backup, second argument is the raised exception."""
 
 
-def read_backups(directory: StrPath, /, callbacks: ReadBackupsCallbacks = ReadBackupsCallbacks()) \
-        -> list[BackupMetadata]:
+def read_backups(
+    directory: StrPath, /, callbacks: ReadBackupsCallbacks = ReadBackupsCallbacks()
+) -> list[BackupMetadata]:
     """Reads all backups present in a directory.
 
-        If a backup is not valid or cannot be read, it is skipped.
+    If a backup is not valid or cannot be read, it is skipped.
 
-        :except OSError: If the directory cannot be accessed.
+    :except OSError: If the directory cannot be accessed.
     """
 
     directory = Path(directory)
 
     entries = list(directory.iterdir())
 
     backups: list[BackupMetadata] = []
     for entry in entries:
         # Try to just read the backup metadata first, because check_if_probably_backup() is quite slow. That way we only
         # pay the cost of check_if_probably_backup() if a directory is not backup, which is unlikely to occur in typical
         # usage.
         try:
             metadata = read_backup_metadata(entry)
-        except (OSError, BackupStartInfoParseError, BackupManifestParseError) as read_error:
+        except (
+            OSError,
+            BackupStartInfoParseError,
+            BackupManifestParseError,
+        ) as read_error:
             # Could be: a valid backup and a filesystem error occurred, or a backup with malformed metadata, or
             # something that's not a backup at all.
             try:
                 if check_if_probably_backup(entry):
                     (callbacks.on_read_metadata_error)(entry, read_error)
                 # If the entry doesn't look like a backup at all then just ignore it.
             except OSError as query_error:
@@ -137,33 +158,33 @@
 
 BACKUP_NAME_LENGTH = 16
 """The length of a backup directory name."""
 
 
 def generate_backup_name(random_gen: Random = Random(), /) -> str:
     """Generates a (very likely) unique name for a backup.
-        The name has length `BACKUP_NAME_LENGTH` and consists of only lowercase ASCII alphabetic characters and digits.
+    The name has length `BACKUP_NAME_LENGTH` and consists of only lowercase ASCII alphabetic characters and digits.
     """
 
-    chars = 'abcdefghijklmnopqrstuvwxyz0123456789'
-    name = ''.join(random_gen.choices(chars, k=BACKUP_NAME_LENGTH))
+    chars = "abcdefghijklmnopqrstuvwxyz0123456789"
+    name = "".join(random_gen.choices(chars, k=BACKUP_NAME_LENGTH))
     return name
 
 
 BACKUP_DIRECTORY_CREATION_RETRIES = 20
 """The number of times to retry creating a new backup directory before failing."""
 
 
 def create_new_backup_directory(target_directory: StrPath, /) -> str:
     """Creates a new backup directory in the given directory (which may not necessarily exist).
-        Will try up to `BACKUP_DIRECTORY_CREATION_RETRIES` to create a new directory before failing.
+    Will try up to `BACKUP_DIRECTORY_CREATION_RETRIES` to create a new directory before failing.
 
-        :return: Name of the new backup directory.
-        :except BackupDirectoryCreationError: If the directory could not be created (due to filesystem errors or name
-            conflicts) within the required number of retries.
+    :return: Name of the new backup directory.
+    :except BackupDirectoryCreationError: If the directory could not be created (due to filesystem errors or name
+        conflicts) within the required number of retries.
     """
 
     retries = BACKUP_DIRECTORY_CREATION_RETRIES
     while True:
         name = generate_backup_name()
         path = Path(target_directory, name)
         try:
@@ -177,9 +198,9 @@
             return name
 
 
 class BackupDirectoryCreationError(Exception):
     """Raised when creating a backup directory fails due to filesystem errors or name conflicts."""
 
     def __init__(self, reason: str) -> None:
-        super().__init__(f'Failed to create backup directory: {reason}')
+        super().__init__(f"Failed to create backup directory: {reason}")
         self.reason = reason
```

### Comparing `incremental_backup-1.2.0/incremental_backup/meta/start_info.py` & `incremental_backup-1.2.1/incremental_backup/meta/start_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,104 +1,101 @@
+import json
 from dataclasses import dataclass
 from datetime import datetime
-import json
-from typing import Any, cast, NoReturn, Optional
+from typing import Any, NoReturn, Optional, cast
 
 from incremental_backup._utility import StrPath
 
-
 __all__ = [
-    'BackupStartInfo',
-    'BackupStartInfoParseError',
-    'deserialise_backup_start_info',
-    'read_backup_start_info_file',
-    'serialise_backup_start_info',
-    'write_backup_start_info_file'
+    "BackupStartInfo",
+    "BackupStartInfoParseError",
+    "deserialise_backup_start_info",
+    "read_backup_start_info_file",
+    "serialise_backup_start_info",
+    "write_backup_start_info_file",
 ]
 
 
 @dataclass(frozen=True)
 class BackupStartInfo:
     """Information pertaining to the start of a backup operation."""
 
     start_time: datetime
     """The UTC time at which the backup operated started (just before any files were copied)."""
 
 
 def serialise_backup_start_info(value: BackupStartInfo, /) -> str:
     """Writes backup start information to a string."""
 
-    json_data = {
-        'start_time': value.start_time.isoformat()
-    }
+    json_data = {"start_time": value.start_time.isoformat()}
     return json.dumps(json_data, indent=4, ensure_ascii=False)
 
 
 def write_backup_start_info_file(path: StrPath, value: BackupStartInfo, /) -> None:
     """Writes backup start information to file.
 
-        :except OSError: If the file could not be written to.
+    :except OSError: If the file could not be written to.
     """
 
-    with open(path, 'w', encoding='utf8') as file:
+    with open(path, "w", encoding="utf8") as file:
         file.write(serialise_backup_start_info(value))
 
 
 def deserialise_backup_start_info(string: str) -> BackupStartInfo:
     """Reads backup start information from a string.
 
-        :except BackupStartInfoParseError: If the string is not valid backup start information.
+    :except BackupStartInfoParseError: If the string is not valid backup start information.
     """
 
     def parse_error(reason: str, e: Optional[Exception] = None, /) -> NoReturn:
         if e is None:
             raise BackupStartInfoParseError(reason)
         else:
             raise BackupStartInfoParseError(reason) from e
 
     try:
         json_data = json.loads(string)
     except json.JSONDecodeError as e:
         parse_error(str(e), e)
 
     if not isinstance(json_data, dict):
-        parse_error('Expected an object')
+        parse_error("Expected an object")
     json_data = cast(dict[Any, Any], json_data)
 
-    fields = {'start_time'}
+    fields = {"start_time"}
     if set(json_data.keys()) != fields:
-        parse_error(f'Expected fields {fields}')
+        parse_error(f"Expected fields {fields}")
 
     try:
-        start_time = datetime.fromisoformat(json_data['start_time'])
+        start_time = datetime.fromisoformat(json_data["start_time"])
     except (TypeError, ValueError) as e:
         parse_error('Field "start_time" must be an ISO-8601 date string', e)
 
     return BackupStartInfo(start_time)
 
 
 def read_backup_start_info_file(path: StrPath, /) -> BackupStartInfo:
     """Reads backup start information from file.
 
-        :except OSError: If the file could not be read.
-        :except BackupStartInfoParseError: If the file is not valid backup start information.
+    :except OSError: If the file could not be read.
+    :except BackupStartInfoParseError: If the file is not valid backup start information.
     """
 
     try:
-        with open(path, 'r', encoding='utf8') as file:
+        with open(path, "r", encoding="utf8") as file:
             return deserialise_backup_start_info(file.read())
     except BackupStartInfoParseError as e:
         # TODO: may be nicer to raise from the cause of e
         raise BackupStartInfoParseError(e.reason, str(path)) from e
 
 
 class BackupStartInfoParseError(Exception):
     """Raised when a backup start information file cannot be parsed due to invalid format."""
 
     def __init__(self, reason: str, file_path: Optional[str] = None) -> None:
         if file_path is None:
-            message = f'Failed to parse backup start info: {reason}'
+            message = f"Failed to parse backup start info: {reason}"
         else:
             message = f'Failed to parse backup start info file "{file_path}": {reason}'
         super().__init__(message)
         self.reason = reason
         self.file_path = file_path
```

### Comparing `incremental_backup-1.2.0/incremental_backup/path_exclude.py` & `incremental_backup-1.2.1/incremental_backup/path_exclude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import re
 from typing import Iterable
 
-
-__all__ = [
-    'PathExcludePattern',
-    'is_path_excluded'
-]
+__all__ = ["PathExcludePattern", "is_path_excluded"]
 
 
 class PathExcludePattern:
     def __init__(self, pattern: str, /) -> None:
         self.pattern = self._compile_pattern(pattern)
 
     def matches(self, path: str, /) -> bool:
@@ -22,14 +18,14 @@
     def __str__(self) -> str:
         return self.pattern.pattern
 
 
 def is_path_excluded(path: str, exclude_patterns: Iterable[PathExcludePattern], /) -> bool:
     """Checks if a path is matched by any path exclude pattern.
 
-        :param path: The path in question. Should be an absolute POSIX-style path, where the root is the backup source
-            directory. Paths that are directories should end in a forward slash ('/'). Paths that are files should not
-            end in a forward slash. Path components should be normalised with `os.path.normcase()`.
-        :param exclude_patterns: Compiled path exclude patterns, from `compile_exclude_pattern()`.
+    :param path: The path in question. Should be an absolute POSIX-style path, where the root is the backup source
+        directory. Paths that are directories should end in a forward slash ('/'). Paths that are files should not
+        end in a forward slash. Path components should be normalised with `os.path.normcase()`.
+    :param exclude_patterns: Compiled path exclude patterns, from `compile_exclude_pattern()`.
     """
 
     return any(pattern.matches(path) for pattern in exclude_patterns)
```

### Comparing `incremental_backup-1.2.0/incremental_backup/prune.py` & `incremental_backup-1.2.1/incremental_backup/prune.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,96 @@
+import shutil
 from collections.abc import Sequence
 from dataclasses import dataclass
 from pathlib import Path
-import shutil
 from typing import Any, Callable
 
-from incremental_backup.meta import BackupMetadata, COMPLETE_INFO_FILENAME, DATA_DIRECTORY_NAME, MANIFEST_FILENAME, \
-    read_backups, ReadBackupsCallbacks, START_INFO_FILENAME
 from incremental_backup._utility import StrPath
-
+from incremental_backup.meta import (
+    COMPLETE_INFO_FILENAME,
+    DATA_DIRECTORY_NAME,
+    MANIFEST_FILENAME,
+    START_INFO_FILENAME,
+    BackupMetadata,
+    ReadBackupsCallbacks,
+    read_backups,
+)
 
 __all__ = [
-    'BackupPrunabilityOptions',
-    'is_backup_prunable',
-    'prune_backups',
-    'PruneBackupsCallbacks',
-    'PruneBackupsError',
-    'PruneBackupsResults'
+    "BackupPrunabilityOptions",
+    "is_backup_prunable",
+    "prune_backups",
+    "PruneBackupsCallbacks",
+    "PruneBackupsError",
+    "PruneBackupsResults",
 ]
 
 
 @dataclass
 class BackupPrunabilityOptions:
     """Options for deciding what backups may be pruned."""
 
     prune_empty: bool
     """If true, backups containing no copied or removed files are eligible for deletion."""
 
     prune_other_data: bool
     """If true, allow deleting backups containing files not recognised by this application."""
 
 
-def is_backup_prunable(backup_path: StrPath, backup_metadata: BackupMetadata, options: BackupPrunabilityOptions, /) \
-        -> bool:
+def is_backup_prunable(
+    backup_path: StrPath,
+    backup_metadata: BackupMetadata,
+    options: BackupPrunabilityOptions,
+    /,
+) -> bool:
     """Checks if a backup is useless and can be deleted.
-    
-        :except OSError: If querying the backup contents failed.
+
+    :except OSError: If querying the backup contents failed.
     """
 
     backup_path = Path(backup_path)
 
     def is_backup_empty() -> bool:
         manifest_root = backup_metadata.manifest.root
-        manifest_nonempty = (manifest_root.copied_files or manifest_root.removed_files
-            or manifest_root.removed_directories or manifest_root.subdirectories)
+        manifest_nonempty = (
+            manifest_root.copied_files
+            or manifest_root.removed_files
+            or manifest_root.removed_directories
+            or manifest_root.subdirectories
+        )
         if manifest_nonempty:
             return False
 
         data_dir = backup_path / DATA_DIRECTORY_NAME
         # Can raise OSError
         data_nonempty = len(list(data_dir.iterdir())) > 0
         if data_nonempty:
             return False
-    
+
         return True
 
     def backup_contains_other_data() -> bool:
         # Can raise OSError
         backup_contents = {entry.name for entry in backup_path.iterdir()}
-        expected_contents = {START_INFO_FILENAME, MANIFEST_FILENAME, COMPLETE_INFO_FILENAME, DATA_DIRECTORY_NAME}
+        expected_contents = {
+            START_INFO_FILENAME,
+            MANIFEST_FILENAME,
+            COMPLETE_INFO_FILENAME,
+            DATA_DIRECTORY_NAME,
+        }
         return backup_contents != expected_contents
 
     prunable = False
     if options.prune_empty and is_backup_empty():
         prunable = True
-    
+
     if prunable and (not options.prune_other_data) and backup_contains_other_data():
         # If there is other data than just the backup, don't delete.
         prunable = False
-    
+
     return prunable
 
 
 @dataclass
 class PruneBackupsConfig:
     dry_run: bool
     """If true, simulate the prune operation without modifying the filesystem."""
@@ -111,34 +130,37 @@
     total_backups_removed: int
     """Total number of backups removed."""
 
     backups_remaining: int
     """The number of valid backups not removed."""
 
 
-def prune_backups(backup_target_directory: StrPath, config: PruneBackupsConfig,
-        callbacks: PruneBackupsCallbacks = PruneBackupsCallbacks()) -> PruneBackupsResults:
+def prune_backups(
+    backup_target_directory: StrPath,
+    config: PruneBackupsConfig,
+    callbacks: PruneBackupsCallbacks = PruneBackupsCallbacks(),
+) -> PruneBackupsResults:
     """Deletes backups which are not useful.
-    
-        :param backup_target_directory: The directory containing the backups which are being examined. I.e. the
-            "target directory" from the backup creation operation.
-        :param config: Options to tune what and how backups are pruned.
-        :param callbacks: Callbacks for certain events during execution. See `PruneBackupsCallbacks`.
-        :return: Summary information for the prune operation.
-        :except PruneBackupsError: If an error occurs that prevents the prune operation from completing.
+
+    :param backup_target_directory: The directory containing the backups which are being examined. I.e. the
+        "target directory" from the backup creation operation.
+    :param config: Options to tune what and how backups are pruned.
+    :param callbacks: Callbacks for certain events during execution. See `PruneBackupsCallbacks`.
+    :return: Summary information for the prune operation.
+    :except PruneBackupsError: If an error occurs that prevents the prune operation from completing.
     """
 
     backup_target_directory = Path(backup_target_directory)
 
     callbacks.on_before_read_backups()
 
     try:
         backups = read_backups(backup_target_directory, callbacks.read_backups)
     except OSError as e:
-        raise PruneBackupsError(f'Failed to query backup target directory: {e}') from e
+        raise PruneBackupsError(f"Failed to query backup target directory: {e}") from e
     callbacks.on_after_read_backups(tuple(backups))
 
     prunable_backups: list[BackupMetadata] = []
     for backup in backups:
         backup_path = backup_target_directory / backup.name
         try:
             is_prunable = is_backup_prunable(backup_path, backup, config.prunability_options)
@@ -164,18 +186,18 @@
 
             try:
                 shutil.rmtree(backup_path, ignore_errors=False, onerror=on_rmtree_error)
             except OSError as e:
                 # Unclear if exceptions can still occur when onerror is provided.
                 callbacks.on_delete_error(backup_path, e)
                 success = False
-        
+
         if success:
             empty_backups_removed += 1
-    
+
     total_backups_removed = empty_backups_removed
     backups_remaining = len(backups) - total_backups_removed
     return PruneBackupsResults(empty_backups_removed, total_backups_removed, backups_remaining)
 
 
 class PruneBackupsError(Exception):
     def __init__(self, message: str) -> None:
```

### Comparing `incremental_backup-1.2.0/incremental_backup/restore.py` & `incremental_backup-1.2.1/incremental_backup/restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+import shutil
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
 from pathlib import Path
-import shutil
 from typing import Callable, Optional, Sequence
 
-from incremental_backup.backup import BackupSum
-from incremental_backup.meta import BackupMetadata, DATA_DIRECTORY_NAME, read_backups, ReadBackupsCallbacks
 from incremental_backup._utility import StrPath
-
+from incremental_backup.backup import BackupSum
+from incremental_backup.meta import (
+    DATA_DIRECTORY_NAME,
+    BackupMetadata,
+    ReadBackupsCallbacks,
+    read_backups,
+)
 
 __all__ = [
-    'perform_restore',
-    'restore_files',
-    'RestoreError',
-    'RestoreFilesCallbacks',
-    'RestoreFilesResults',
-    'RestoreCallbacks',
-    'RestoreResults'
+    "perform_restore",
+    "restore_files",
+    "RestoreError",
+    "RestoreFilesCallbacks",
+    "RestoreFilesResults",
+    "RestoreCallbacks",
+    "RestoreResults",
 ]
 
 
 @dataclass(frozen=True)
 class RestoreFilesResults:
     """Return results of `restore_files()`."""
 
@@ -39,23 +43,27 @@
 
     on_copy_error: Callable[[Path, Path, OSError], None] = lambda src, dest, error: None
     """Called when an error is raised copying a file.
         First argument is the source path, second argument is the destination path, third argument is the raised
         exception."""
 
 
-def restore_files(backup_target_directory: StrPath, backup_sum: BackupSum, destination_directory: StrPath,
-                  callbacks: RestoreFilesCallbacks = RestoreFilesCallbacks()) -> RestoreFilesResults:
+def restore_files(
+    backup_target_directory: StrPath,
+    backup_sum: BackupSum,
+    destination_directory: StrPath,
+    callbacks: RestoreFilesCallbacks = RestoreFilesCallbacks(),
+) -> RestoreFilesResults:
     """Restores files and directories from backups to a new location.
 
-        :param backup_target_directory: The directory containing the backups which are being restored. I.e. the
-            "target directory" from the backup creation operation.
-        :param backup_sum: Sum of backups to restore files from.
-        :param destination_directory: Directory where files will be restored to. Need not exist.
-        :param callbacks: Callbacks for certain events during execution. See `RestoreFilesCallbacks`.
+    :param backup_target_directory: The directory containing the backups which are being restored. I.e. the
+        "target directory" from the backup creation operation.
+    :param backup_sum: Sum of backups to restore files from.
+    :param destination_directory: Directory where files will be restored to. Need not exist.
+    :param callbacks: Callbacks for certain events during execution. See `RestoreFilesCallbacks`.
     """
 
     paths_skipped = False
     files_restored = 0
     search_stack: list[Callable[[], None]] = []
     path_segments: list[str] = []
     is_root = True
@@ -80,15 +88,19 @@
             paths_skipped = True
 
             (callbacks.on_mkdir_error)(directory_path, e)
         else:
             for file in search_directory.files:
                 relative_file_path = relative_directory_path / file.name
                 source_file_path = Path(
-                    backup_target_directory, file.last_backup.name, DATA_DIRECTORY_NAME, relative_file_path)
+                    backup_target_directory,
+                    file.last_backup.name,
+                    DATA_DIRECTORY_NAME,
+                    relative_file_path,
+                )
                 destination_file_path = destination_directory / relative_file_path
 
                 try:
                     shutil.copy2(source_file_path, destination_file_path)
                 except OSError as e:
                     paths_skipped = True
 
@@ -139,60 +151,74 @@
     on_before_restore_files: Callable[[], None] = lambda: None
     """Called just before copying files to the destination."""
 
     restore_files: RestoreFilesCallbacks = RestoreFilesCallbacks()
     """Callbacks for `restore_files()`."""
 
 
-def perform_restore(backup_target_directory: StrPath, destination_directory: StrPath,
-                    backup_name: Optional[str] = None, backup_time: Optional[datetime] = None,
-                    callbacks: RestoreCallbacks = RestoreCallbacks()) -> RestoreResults:
+def perform_restore(
+    backup_target_directory: StrPath,
+    destination_directory: StrPath,
+    backup_name: Optional[str] = None,
+    backup_time: Optional[datetime] = None,
+    callbacks: RestoreCallbacks = RestoreCallbacks(),
+) -> RestoreResults:
     """Restores files and directories from existing backups.
 
-        :param backup_target_directory: The directory containing the backups which are being restored. I.e. the
-            "target directory" from the backup creation operation.
-        :param destination_directory: Directory where files will be restored to. Need not exist.
-        :param backup_name: If specified, only backups up to and including this backup (chronologically) will be used to
-            restore files. Cannot be specified if `backup_time` is also specified.
-        :param backup_time: If specified, only backups up to and including this time will be used to restore files.
-            Cannot be specified if `backup_name` is also specified.
-        :param callbacks: Callbacks for certain events during execution. See `RestoreCallbacks`.
-        :return: Summary information for the restore operation.
-        :except ValueError: If both `backup_name` and `backup_time` are not `None`.
-        :except RestoreError: If an error occurs that prevents the restore operation from completing. See `RestoreError`.
+    :param backup_target_directory: The directory containing the backups which are being restored. I.e. the
+        "target directory" from the backup creation operation.
+    :param destination_directory: Directory where files will be restored to. Need not exist.
+    :param backup_name: If specified, only backups up to and including this backup (chronologically) will be used to
+        restore files. Cannot be specified if `backup_time` is also specified.
+    :param backup_time: If specified, only backups up to and including this time will be used to restore files.
+        Cannot be specified if `backup_name` is also specified.
+    :param callbacks: Callbacks for certain events during execution. See `RestoreCallbacks`.
+    :return: Summary information for the restore operation.
+    :except ValueError: If both `backup_name` and `backup_time` are not `None`.
+    :except RestoreError: If an error occurs that prevents the restore operation from completing. See `RestoreError`.
     """
 
     return _RestoreOperation(
-        backup_target_directory, destination_directory, backup_name, backup_time, callbacks).perform_restore()
+        backup_target_directory,
+        destination_directory,
+        backup_name,
+        backup_time,
+        callbacks,
+    ).perform_restore()
 
 
 class _RestoreOperation:
     """Implementation of the backup restore operation."""
 
-    def __init__(self, backup_target_directory: StrPath, destination_directory: StrPath,
-                 backup_name: Optional[str] = None, backup_time: Optional[datetime] = None,
-                 callbacks: RestoreCallbacks = RestoreCallbacks()) -> None:
+    def __init__(
+        self,
+        backup_target_directory: StrPath,
+        destination_directory: StrPath,
+        backup_name: Optional[str] = None,
+        backup_time: Optional[datetime] = None,
+        callbacks: RestoreCallbacks = RestoreCallbacks(),
+    ) -> None:
         """
-            :except ValueError: If both `backup_name` and `backup_time` are not `None`.
+        :except ValueError: If both `backup_name` and `backup_time` are not `None`.
         """
 
         if backup_name is not None and backup_time is not None:
-            raise ValueError('backup_name and backup_time should not both be specified.')
+            raise ValueError("backup_name and backup_time should not both be specified.")
 
         self.backup_name = backup_name
         self.backup_time = backup_time
         self.backup_target_directory = Path(backup_target_directory)
         self.destination_directory = Path(destination_directory)
         self.callbacks = callbacks
 
     def perform_restore(self) -> RestoreResults:
         """Restores files from the specified backups.
 
-            :except RestoreError: If an error occurs that prevents the restore operation from completing. See
-                `RestoreError`.
+        :except RestoreError: If an error occurs that prevents the restore operation from completing. See
+            `RestoreError`.
         """
 
         self._validate_backup_target_directory()
         self._validate_destination_directory()
 
         previous_backups = self._read_previous_backups()
         selected_backups = self._select_backups_to_restore(previous_backups)
@@ -203,78 +229,78 @@
 
         results = self._restore_files(backup_sum)
 
         return results
 
     def _validate_backup_target_directory(self) -> None:
         """Validates the backup target directory.
-            Should mostly prevent other parts of the restore operation from failing strangely for invalid inputs.
+        Should mostly prevent other parts of the restore operation from failing strangely for invalid inputs.
 
-            :except Restore: If the backup target directory is not an accessible directory.
+        :except Restore: If the backup target directory is not an accessible directory.
         """
 
         try:
             if not self.backup_target_directory.exists():
-                raise RestoreError(f'Backup target directory not found')
+                raise RestoreError("Backup target directory not found")
             if not self.backup_target_directory.is_dir():
-                raise RestoreError(f'Backup target directory is not a directory')
+                raise RestoreError("Backup target directory is not a directory")
         except OSError as e:
-            raise RestoreError(f'Failed to query backup target directory: {e}') from e
+            raise RestoreError(f"Failed to query backup target directory: {e}") from e
 
     def _validate_destination_directory(self) -> None:
         """Validates the restore destination directory.
-            Should mostly prevent other parts of the restore operation from failing strangely for invalid inputs.
+        Should mostly prevent other parts of the restore operation from failing strangely for invalid inputs.
 
-            :except RestoreError: If the destination directory is inaccessible, or exists and is not an empty directory.
+        :except RestoreError: If the destination directory is inaccessible, or exists and is not an empty directory.
         """
 
         try:
             if self.destination_directory.exists():
                 if self.destination_directory.is_dir() and tuple(self.destination_directory.iterdir()):
-                    raise RestoreError('Destination directory must be nonexistent or empty')
+                    raise RestoreError("Destination directory must be nonexistent or empty")
         except OSError as e:
-            raise RestoreError(f'Failed to query destination directory: {e}') from e
+            raise RestoreError(f"Failed to query destination directory: {e}") from e
 
     def _read_previous_backups(self) -> Sequence[BackupMetadata]:
         """Reads all existing backups' metadata from the backup target directory.
 
-            If any backup's metadata cannot be read, skips that backup.
+        If any backup's metadata cannot be read, skips that backup.
 
-            :except RestoreError: If the target directory cannot be enumerated.
+        :except RestoreError: If the target directory cannot be enumerated.
         """
 
         (self.callbacks.on_before_read_previous_backups)()
 
         try:
             backups = read_backups(self.backup_target_directory, self.callbacks.read_backups)
         except OSError as e:
-            raise RestoreError(f'Failed to enumerate backup target directory: {e}') from e
+            raise RestoreError(f"Failed to enumerate backup target directory: {e}") from e
         backups = tuple(backups)
 
         (self.callbacks.on_after_read_previous_backups)(backups)
 
         return backups
 
     def _select_backups_to_restore(self, previous_backups: Sequence[BackupMetadata], /) -> Sequence[BackupMetadata]:
         """Returns backups from `self.previous_backups` requested to restore files from, based on `self.backup_name`
-            and `self.backup_time`.
+        and `self.backup_time`.
 
-            If `backup_name` is specified, all backups whose start time is <= `backup_name`'s start time are selected.
+        If `backup_name` is specified, all backups whose start time is <= `backup_name`'s start time are selected.
 
-            If `backup_time` is specified all backups whose start time is <= `backup_time` are selected.
+        If `backup_time` is specified all backups whose start time is <= `backup_time` are selected.
 
-            If neither `backup_name` nor `backup_time` are specified, all previous backups are selected.
+        If neither `backup_name` nor `backup_time` are specified, all previous backups are selected.
 
-            :except RestoreError: If `backup_name` is specified but that backup is not found.
+        :except RestoreError: If `backup_name` is specified but that backup is not found.
         """
 
         if self.backup_name is not None:
             backup = next((b for b in previous_backups if b.name == self.backup_name), None)
             if backup is None:
-                raise RestoreError('Requested backup not found')
+                raise RestoreError("Requested backup not found")
             backup_time = backup.start_info.start_time
         else:
             backup_time = self.backup_time
         if backup_time is None:
             selected_backups = previous_backups
         else:
             selected_backups = tuple(b for b in previous_backups if b.start_info.start_time <= backup_time)
@@ -282,44 +308,48 @@
         (self.callbacks.on_selected_backups)(selected_backups)
 
         return selected_backups
 
     def _create_destination(self) -> None:
         """Creates the restore destination directory.
 
-            Not strictly necessary to do here, because it will be created anyway in `restore_files()`. But if we attempt
-            to create it here first, then we can fail with an informative error in the case the path is not accessible.
+        Not strictly necessary to do here, because it will be created anyway in `restore_files()`. But if we attempt
+        to create it here first, then we can fail with an informative error in the case the path is not accessible.
 
-            :except RestoreError: If the directory could not be created.
+        :except RestoreError: If the directory could not be created.
         """
 
         try:
             self.destination_directory.mkdir(exist_ok=True)
         except OSError as e:
-            raise RestoreError(f'Failed to create destination directory: {e}') from e
+            raise RestoreError(f"Failed to create destination directory: {e}") from e
 
     def _restore_files(self, backup_sum: BackupSum) -> RestoreResults:
         """Copies files and directories from backups specified by `backup_sum` to the destination directory.
 
-            :return: Summary information from the operation.
+        :return: Summary information from the operation.
         """
 
         (self.callbacks.on_before_restore_files)()
 
         restore_results = restore_files(
-            self.backup_target_directory, backup_sum, self.destination_directory, self.callbacks.restore_files)
+            self.backup_target_directory,
+            backup_sum,
+            self.destination_directory,
+            self.callbacks.restore_files,
+        )
 
         return RestoreResults(restore_results.files_restored, restore_results.paths_skipped)
 
 
 class RestoreError(Exception):
     """Raised when restoring files from backups fails such that the operation cannot continue.
 
-        Some cases where this exception is raised:
-         - The backup target directory can't be accessed at all.
-         - The specified backup name doesn't exist.
-         - The destination directory couldn't be created.
+    Some cases where this exception is raised:
+     - The backup target directory can't be accessed at all.
+     - The specified backup name doesn't exist.
+     - The destination directory couldn't be created.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
         self.message = message
```

### Comparing `incremental_backup-1.2.0/incremental_backup.egg-info/PKG-INFO` & `incremental_backup-1.2.1/incremental_backup.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,74 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.2.0
+Version: 1.2.1
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
-# Incremental Backup Tool (MK 2)
+# Incremental Backup Tool
 
-by Reece Jones
+**An easy-to-use, no fluff incremental file backup application.**
 
-## Purpose
+## Features
 
-Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
-There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.
-
-Thus, I created this tool. Some of its design goals are:
-
-- free, open source
-- as simple as possible (no installation, no GUI, no fluff)
-- robust
-- fast
-- efficient
-- transparent backup format
-
-This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
-Please see [ChangesFromOriginal.md](ChangesFromOriginal.md) for details.  
-If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
-
-## Disclaimer
-
-This application is intended for low-risk personal use.
-I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
+- **Efficient backup** - copies and stores only changed files.
+- **Simple backup format** - data is stored as plain files, metadata is JSON.
+- **No configuration** - all the tool needs to know is where the data is, and where to put the backups.
+- **Focus on failure** - designed with failure in mind to keep your data intact.
+- **CLI and API usage**
 
 ## Requirements
 
-General usage:
-
 - Windows or Linux system
 - Python 3.9 or newer
 
-Development:
-
-- Pytest (any recent version should do)
+## Usage
 
-## Application Structure
+**Create a backup:**
 
-Important files and directories:
+```
+python -m incremental_backup backup /path/to/back/up /safe/backup/location
+```
 
-- `incremental_backup/` - The Python package.
-  - `backup/` - High-level backup functionality.
-  - `cli/` - Command line interface functionality (see also the _Usage_ section).
-  - `meta/` - Functionality related to backup metadata and structure.
-  - `__main__.py` - Entrypoint for using the command line interface via the package name.
-  - `restore.py` - Backup restoration functionality.
-- `test/` - Test code. Each directory/file corresponds to the module in `incremental_backup/` it tests.
+This will back up files from `/path/to/back/up` into `/safe/backup/location`.
 
-The `incremental_backup` Python package contains all application functionality and can be easily used in a library-like manner.
-Additionally, this package doubles as the application entrypoint.
+Run the same command again to do subsequent backups - it's that easy! Backups in `/safe/backup/location` will be automatically read to determine what needs to be copied.
 
-## Usage
+For details, see [docs/BackupUsage.md](./docs/BackupUsage.md).
 
-The Python package is executable via a command line interface.
-The interface uses multiple "commands" for different functionality.
-Usage is as follows:
+**Restore files:**
 
 ```
-python3 -m incremental_backup <command> <command_args>
+python -m incremental_backup restore /safe/backup/location /restore/to/here
 ```
 
-(You may have to adjust the Python command based on your system configuration.)
+This restores the backed up files from `/safe/backup/location` into `/restore/to/here`.
 
-Commands:
+For details, see [docs/RestoreUsage.md](./docs/RestoreUsage.md).
 
-- `backup` - Creates a new backup. See [BackupUsage.md](BackupUsage.md) for details.
-- `restore` - Restores files from backups. See [RestoreUsage.md](RestoreUsage.md) for details.
-
-To start using this application, you probably want to have a look at [BackupUsage.md](BackupUsage.md).
+## Disclaimer
 
-### Program Exit Codes
+This application is intended for low-risk personal use.
+I have genuinely tried to make it as robust as possible, but if you use this software and lose all your data as a result, that's not my responsibility.
 
-- 0 - The operation completed successfully, possibly with some warnings (i.e. nonfatal errors).
-- 1 - The command line arguments are invalid.
-- 2 - The operation could not be completed due to a runtime error (typically would be a file I/O error).
-- -1 - The operation was aborted due to a programmer error - sorry in advance.
+## Development and Contributing
 
-## Running Tests
+For details on developing or otherwise contributing to the project, please see [CONTRIBUTING.md](./CONTRIBUTING.md).
 
-With your working directory as the project root directory:
+## Background
 
-```
-python3 -m pytest
-```
+Unlike Linux, which has awesome tools like rsync, Windows does not seem to have a good selection of free backup tools.
+There is the Windows system image backup, but that does full backups only. There is also File History, but that is janky and largely opaque.  
+Thus, I created this tool, and aimed for it to be as simple, open, and robust as possible.
 
-This runs a suite of unit and integration tests.
+This project is a successor to my initial attempts at an incremental backup tool for Windows, available [here](https://github.com/MC-DeltaT/IncrementalBackup).  
+Please see [docs/ChangesFromOriginal.md](./docs/ChangesFromOriginal.md) for details.  
+If you have used the original incremental backup tool, please note that this version is **NOT backwards compatible** with the original.
```

### Comparing `incremental_backup-1.2.0/incremental_backup.egg-info/SOURCES.txt` & `incremental_backup-1.2.1/incremental_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.2.0/test/test_path_exclude.py` & `incremental_backup-1.2.1/test/test_path_exclude.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 import re
 
 from incremental_backup.path_exclude import PathExcludePattern, is_path_excluded
 
 
 def test_path_exclude_pattern_init() -> None:
-    p1 = PathExcludePattern('')
+    p1 = PathExcludePattern("")
     assert isinstance(p1.pattern, re.Pattern)
-    assert p1.pattern.pattern == ''
+    assert p1.pattern.pattern == ""
     assert p1.pattern.flags == re.UNICODE | re.DOTALL
 
-    p2 = PathExcludePattern('/foo/bar/dir/')
+    p2 = PathExcludePattern("/foo/bar/dir/")
     assert isinstance(p2.pattern, re.Pattern)
-    assert p2.pattern.pattern == '/foo/bar/dir/'
+    assert p2.pattern.pattern == "/foo/bar/dir/"
     assert p2.pattern.flags == re.UNICODE | re.DOTALL
 
-    p3 = PathExcludePattern(r'/a/file\.txt')
+    p3 = PathExcludePattern(r"/a/file\.txt")
     assert isinstance(p3.pattern, re.Pattern)
-    assert p3.pattern.pattern == r'/a/file\.txt'
+    assert p3.pattern.pattern == r"/a/file\.txt"
     assert p3.pattern.flags == re.UNICODE | re.DOTALL
 
-    p4 = PathExcludePattern(r'.*/\.git/')
+    p4 = PathExcludePattern(r".*/\.git/")
     assert isinstance(p4.pattern, re.Pattern)
-    assert p4.pattern.pattern == r'.*/\.git/'
+    assert p4.pattern.pattern == r".*/\.git/"
     assert p4.pattern.flags == re.UNICODE | re.DOTALL
 
 
 def test_is_path_excluded_no_patterns() -> None:
-    assert not is_path_excluded('/', ())
-    assert not is_path_excluded('/foo/bar', ())
-    assert not is_path_excluded('/some/Directory/FILE', ())
-    assert not is_path_excluded('/longer/path/to/file/with/un\u1234ico\u7685de\xFA.jpg', ())
+    assert not is_path_excluded("/", ())
+    assert not is_path_excluded("/foo/bar", ())
+    assert not is_path_excluded("/some/Directory/FILE", ())
+    assert not is_path_excluded("/longer/path/to/file/with/un\u1234ico\u7685de\xfa.jpg", ())
 
 
 def test_is_path_excluded_ascii_paths() -> None:
-    patterns = ('/foo/dir_b/some_dir/', '/path/to/file', r'/path/to/file_with_ext\.jpg', r'/\$RECYCLE\.BIN/')
+    patterns = (
+        "/foo/dir_b/some_dir/",
+        "/path/to/file",
+        r"/path/to/file_with_ext\.jpg",
+        r"/\$RECYCLE\.BIN/",
+    )
     patterns = tuple(map(PathExcludePattern, patterns))
 
-    assert is_path_excluded('/foo/dir_b/some_dir/', patterns)
-    assert is_path_excluded('/path/to/file', patterns)
-    assert is_path_excluded('/path/to/file_with_ext.jpg', patterns)
-    assert is_path_excluded('/$RECYCLE.BIN/', patterns)
-    assert not is_path_excluded('/foo/dir_b/some_dir', patterns)
-    assert not is_path_excluded('/foo', patterns)
-    assert not is_path_excluded('/foo/', patterns)
-    assert not is_path_excluded('/foo/dir_b/some_dir/qux/', patterns)
-    assert not is_path_excluded('/foo/dir_b/some_dir/qux', patterns)
-    assert not is_path_excluded('/path/to/file/', patterns)
-    assert not is_path_excluded('/path/to/file_with_ext', patterns)
-    assert not is_path_excluded('/ayy', patterns)
-    assert not is_path_excluded('/a/b/c/d/e/f/', patterns)
+    assert is_path_excluded("/foo/dir_b/some_dir/", patterns)
+    assert is_path_excluded("/path/to/file", patterns)
+    assert is_path_excluded("/path/to/file_with_ext.jpg", patterns)
+    assert is_path_excluded("/$RECYCLE.BIN/", patterns)
+    assert not is_path_excluded("/foo/dir_b/some_dir", patterns)
+    assert not is_path_excluded("/foo", patterns)
+    assert not is_path_excluded("/foo/", patterns)
+    assert not is_path_excluded("/foo/dir_b/some_dir/qux/", patterns)
+    assert not is_path_excluded("/foo/dir_b/some_dir/qux", patterns)
+    assert not is_path_excluded("/path/to/file/", patterns)
+    assert not is_path_excluded("/path/to/file_with_ext", patterns)
+    assert not is_path_excluded("/ayy", patterns)
+    assert not is_path_excluded("/a/b/c/d/e/f/", patterns)
 
 
 def test_is_path_excluded_case_sensitivity() -> None:
-    patterns = ('/all/lowercase', '/ALL/UPPERCASE/', '/mixd/CASE/Path')
+    patterns = ("/all/lowercase", "/ALL/UPPERCASE/", "/mixd/CASE/Path")
     patterns = tuple(map(PathExcludePattern, patterns))
 
-    assert is_path_excluded('/all/lowercase', patterns)
-    assert is_path_excluded('/ALL/UPPERCASE/', patterns)
-    assert is_path_excluded('/mixd/CASE/Path', patterns)
-    assert not is_path_excluded('/ALL/LOWERCASE', patterns)
-    assert not is_path_excluded('/all/uppercase', patterns)
-    assert not is_path_excluded('/MIXD/case/pATH', patterns)
-    assert not is_path_excluded('/All/lowercase', patterns)
-    assert not is_path_excluded('/ALL/UPPERCASe/', patterns)
-    assert not is_path_excluded('/MIXd/CaSe/PaTH', patterns)
+    assert is_path_excluded("/all/lowercase", patterns)
+    assert is_path_excluded("/ALL/UPPERCASE/", patterns)
+    assert is_path_excluded("/mixd/CASE/Path", patterns)
+    assert not is_path_excluded("/ALL/LOWERCASE", patterns)
+    assert not is_path_excluded("/all/uppercase", patterns)
+    assert not is_path_excluded("/MIXD/case/pATH", patterns)
+    assert not is_path_excluded("/All/lowercase", patterns)
+    assert not is_path_excluded("/ALL/UPPERCASe/", patterns)
+    assert not is_path_excluded("/MIXd/CaSe/PaTH", patterns)
 
 
 def test_is_path_excluded_unicode_paths() -> None:
-    patterns = ('/dir\n/with/U\u6A72n\xDFiC\u6D42o\u5B4Dd\xFFE/', '/\u3764\u3245\u6475/qux/\u023Ffile\\.pdf',
-                '/un\xEFi\uC9F6c\u91F5ode\\.txt')
+    patterns = (
+        "/dir\n/with/U\u6a72n\xdfiC\u6d42o\u5b4dd\xffE/",
+        "/\u3764\u3245\u6475/qux/\u023ffile\\.pdf",
+        "/un\xefi\uc9f6c\u91f5ode\\.txt",
+    )
     patterns = tuple(map(PathExcludePattern, patterns))
 
-    assert is_path_excluded('/dir\n/with/U\u6A72n\xDFiC\u6D42o\u5B4Dd\xFFE/', patterns)
-    assert is_path_excluded('/\u3764\u3245\u6475/qux/\u023Ffile.pdf', patterns)
-    assert is_path_excluded('/un\xEFi\uC9F6c\u91F5ode.txt', patterns)
-    assert not is_path_excluded('/dir\n/with/U\u6A72n\xDFiC\u6D42o\u5B4Dd\xFFE', patterns)
-    assert not is_path_excluded('/dir\n/with/U\u6A72n\xDFiC\u6D42o\u5B4Dd\x00E/', patterns)
-    assert not is_path_excluded('/dir/with/U\u6A72n\xDFiC\u6D42o\u5B4Dd\xFFE/', patterns)
-    assert not is_path_excluded('/\u3764\u3245\u6475/qux/\u023Ffile.pdf/', patterns)
-    assert not is_path_excluded('/\u3764\u3245a/qux/\u023Ffile.pdf', patterns)
+    assert is_path_excluded("/dir\n/with/U\u6a72n\xdfiC\u6d42o\u5b4dd\xffE/", patterns)
+    assert is_path_excluded("/\u3764\u3245\u6475/qux/\u023ffile.pdf", patterns)
+    assert is_path_excluded("/un\xefi\uc9f6c\u91f5ode.txt", patterns)
+    assert not is_path_excluded("/dir\n/with/U\u6a72n\xdfiC\u6d42o\u5b4dd\xffE", patterns)
+    assert not is_path_excluded("/dir\n/with/U\u6a72n\xdfiC\u6d42o\u5b4dd\x00E/", patterns)
+    assert not is_path_excluded("/dir/with/U\u6a72n\xdfiC\u6d42o\u5b4dd\xffE/", patterns)
+    assert not is_path_excluded("/\u3764\u3245\u6475/qux/\u023ffile.pdf/", patterns)
+    assert not is_path_excluded("/\u3764\u3245a/qux/\u023ffile.pdf", patterns)
 
 
 def test_is_path_excluded_advanced() -> None:
-    patterns = (r'.*/\.git/', r'.*/__pycache__/')
+    patterns = (r".*/\.git/", r".*/__pycache__/")
     patterns = tuple(map(PathExcludePattern, patterns))
 
-    assert is_path_excluded('/.git/', patterns)
-    assert is_path_excluded('/my/code/project/.git/', patterns)
-    assert is_path_excluded('/__pycache__/', patterns)
-    assert is_path_excluded('/i/do/coding/__pycache__/', patterns)
-    assert is_path_excluded('/i/do/coding/__pycache__/', patterns)
-    assert not is_path_excluded('/.git', patterns)
-    assert not is_path_excluded('/.git/magic/', patterns)
-    assert not is_path_excluded('/.git/file', patterns)
-    assert not is_path_excluded('/foo.git/', patterns)
-    assert not is_path_excluded('/.git.bar/', patterns)
-    assert not is_path_excluded('/__pycache__/yeah/man/', patterns)
+    assert is_path_excluded("/.git/", patterns)
+    assert is_path_excluded("/my/code/project/.git/", patterns)
+    assert is_path_excluded("/__pycache__/", patterns)
+    assert is_path_excluded("/i/do/coding/__pycache__/", patterns)
+    assert is_path_excluded("/i/do/coding/__pycache__/", patterns)
+    assert not is_path_excluded("/.git", patterns)
+    assert not is_path_excluded("/.git/magic/", patterns)
+    assert not is_path_excluded("/.git/file", patterns)
+    assert not is_path_excluded("/foo.git/", patterns)
+    assert not is_path_excluded("/.git.bar/", patterns)
+    assert not is_path_excluded("/__pycache__/yeah/man/", patterns)
```

### Comparing `incremental_backup-1.2.0/test/test_prune.py` & `incremental_backup-1.2.1/test/test_prune.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,155 @@
 from pathlib import Path
 from typing import Any
 
 import pytest
 
 from incremental_backup.meta.meta import ReadBackupsCallbacks
-from incremental_backup.prune import BackupPrunabilityOptions, is_backup_prunable, prune_backups, PruneBackupsCallbacks, \
-    PruneBackupsConfig, PruneBackupsError, PruneBackupsResults
+from incremental_backup.prune import (
+    BackupPrunabilityOptions,
+    PruneBackupsCallbacks,
+    PruneBackupsConfig,
+    PruneBackupsError,
+    PruneBackupsResults,
+    is_backup_prunable,
+    prune_backups,
+)
 
-from helpers import AssertFilesystemUnmodified, MakeBackup, unordered_equal
+from test.helpers import AssertFilesystemUnmodified, MakeBackup, unordered_equal
 
 
 def test_is_backup_prunable_nonempty(tmpdir: Path) -> None:
     backup_path, backup_metadata = MakeBackup.valid(copied_files=True)(tmpdir)
 
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=True),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=True),
+    )
 
 
 def test_is_backup_prunable_empty(tmpdir: Path) -> None:
     backup_path, backup_metadata = MakeBackup.empty()(tmpdir)
 
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=True),
+    )
     assert is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=False),
+    )
     assert is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=True),
+    )
 
 
 def test_is_backup_prunable_removed_only(tmpdir: Path) -> None:
-    backup_path, backup_metadata = MakeBackup.valid(
-        copied_files=False, removed_files=True, removed_directories=True)(tmpdir)
+    backup_path, backup_metadata = MakeBackup.valid(copied_files=False, removed_files=True, removed_directories=True)(
+        tmpdir
+    )
 
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=True),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=True),
+    )
 
 
 def test_is_backup_prunable_other_data(tmpdir: Path) -> None:
     backup_path, backup_metadata = MakeBackup.empty()(tmpdir)
-    (backup_path / 'my_quirky_data.abc').write_text('yes')
+    (backup_path / "my_quirky_data.abc").write_text("yes")
 
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=False),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=False, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=False, prune_other_data=True),
+    )
     assert not is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=False))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=False),
+    )
     assert is_backup_prunable(
-        backup_path, backup_metadata, BackupPrunabilityOptions(prune_empty=True, prune_other_data=True))
+        backup_path,
+        backup_metadata,
+        BackupPrunabilityOptions(prune_empty=True, prune_other_data=True),
+    )
 
 
 def test_prune_backups_nonexistent_target(tmpdir: Path) -> None:
     # Backup target directory doesn't exist.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
 
     config = PruneBackupsConfig(False, BackupPrunabilityOptions(True, False))
 
     actual_callbacks: list[Any] = []
     callbacks = PruneBackupsCallbacks(
-        on_before_read_backups=lambda: actual_callbacks.append('on_before_read_backups'),
+        on_before_read_backups=lambda: actual_callbacks.append("on_before_read_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
         ),
-        on_after_read_backups=lambda backups: pytest.fail(f'Unexpected on_after_read_backups: {backups=}'),
-        on_selected_backups=lambda backups: pytest.fail(f'Unexpected on_selected_backups: {backups=}'),
-        on_delete_error=lambda path, error: pytest.fail(f'Unexpected on_delete_error: {path=} {error=}'),
+        on_after_read_backups=lambda backups: pytest.fail(f"Unexpected on_after_read_backups: {backups=}"),
+        on_selected_backups=lambda backups: pytest.fail(f"Unexpected on_selected_backups: {backups=}"),
+        on_delete_error=lambda path, error: pytest.fail(f"Unexpected on_delete_error: {path=} {error=}"),
     )
 
     with AssertFilesystemUnmodified(tmpdir):
         with pytest.raises(PruneBackupsError):
             prune_backups(target_dir, config, callbacks)
-    
-    assert actual_callbacks == [
-        'on_before_read_backups'
-    ]
+
+    assert actual_callbacks == ["on_before_read_backups"]
 
 
 def test_prune_backups_invalid_backup(tmpdir: Path) -> None:
     # Some backups have invalid metadata.
 
     backup1_path, backup1_metadata = MakeBackup.empty()(tmpdir)
     backup2_path, backup2_metadata = MakeBackup.valid()(tmpdir)
@@ -102,114 +157,125 @@
 
     config = PruneBackupsConfig(False, BackupPrunabilityOptions(True, False))
 
     # Note that since the backup is invalid, it will just be ignored without triggering any error handling.
 
     actual_callbacks: list[Any] = []
     callbacks = PruneBackupsCallbacks(
-        on_before_read_backups=lambda: actual_callbacks.append('on_before_read_backups'),
+        on_before_read_backups=lambda: actual_callbacks.append("on_before_read_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
         ),
-        on_after_read_backups=lambda backups: actual_callbacks.append(('on_after_read_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('on_selected_backups', backups)),
-        on_delete_error=lambda path, error: pytest.fail(f'Unexpected on_delete_error: {path=} {error=}'),
+        on_after_read_backups=lambda backups: actual_callbacks.append(("on_after_read_backups", backups)),
+        on_selected_backups=lambda backups: actual_callbacks.append(("on_selected_backups", backups)),
+        on_delete_error=lambda path, error: pytest.fail(f"Unexpected on_delete_error: {path=} {error=}"),
     )
 
     with AssertFilesystemUnmodified(backup2_path, backup3_path):
         results = prune_backups(tmpdir, config, callbacks)
 
     assert not backup1_path.exists()
 
     assert results == PruneBackupsResults(empty_backups_removed=1, total_backups_removed=1, backups_remaining=1)
-    
-    assert actual_callbacks[0] == 'on_before_read_backups'
-    assert actual_callbacks[1][0] == 'on_after_read_backups'
+
+    assert actual_callbacks[0] == "on_before_read_backups"
+    assert actual_callbacks[1][0] == "on_after_read_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
     assert unordered_equal(
-        (backup1_metadata.name, backup2_metadata.name), [backup.name for backup in actual_callbacks[1][1]])
-    assert actual_callbacks[2][0] == 'on_selected_backups'
+        (backup1_metadata.name, backup2_metadata.name),
+        [backup.name for backup in actual_callbacks[1][1]],
+    )
+    assert actual_callbacks[2][0] == "on_selected_backups"
     assert [backup1_metadata.name] == [backup.name for backup in actual_callbacks[2][1]]
 
 
 def test_prune_backups_delete_empty(tmpdir: Path) -> None:
     # Normal behaviour of deleting empty backups.
 
     backup1_path, backup1_metadata = MakeBackup.empty()(tmpdir)
     backup2_path, backup2_metadata = MakeBackup.valid()(tmpdir)
     backup3_path, backup3_metadata = MakeBackup.empty()(tmpdir)
 
     config = PruneBackupsConfig(False, BackupPrunabilityOptions(True, False))
 
     actual_callbacks: list[Any] = []
     callbacks = PruneBackupsCallbacks(
-        on_before_read_backups=lambda: actual_callbacks.append('on_before_read_backups'),
+        on_before_read_backups=lambda: actual_callbacks.append("on_before_read_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
         ),
-        on_after_read_backups=lambda backups: actual_callbacks.append(('on_after_read_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('on_selected_backups', backups)),
-        on_delete_error=lambda path, error: pytest.fail(f'Unexpected on_delete_error: {path=} {error=}'),
+        on_after_read_backups=lambda backups: actual_callbacks.append(("on_after_read_backups", backups)),
+        on_selected_backups=lambda backups: actual_callbacks.append(("on_selected_backups", backups)),
+        on_delete_error=lambda path, error: pytest.fail(f"Unexpected on_delete_error: {path=} {error=}"),
     )
 
     with AssertFilesystemUnmodified(backup2_path):
         results = prune_backups(tmpdir, config, callbacks)
 
     assert not backup1_path.exists()
     assert not backup3_path.exists()
 
     assert results == PruneBackupsResults(empty_backups_removed=2, total_backups_removed=2, backups_remaining=1)
-    
-    assert actual_callbacks[0] == 'on_before_read_backups'
-    assert actual_callbacks[1][0] == 'on_after_read_backups'
+
+    assert actual_callbacks[0] == "on_before_read_backups"
+    assert actual_callbacks[1][0] == "on_after_read_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
     assert unordered_equal(
         (backup1_metadata.name, backup2_metadata.name, backup3_metadata.name),
-        [backup.name for backup in actual_callbacks[1][1]])
-    assert actual_callbacks[2][0] == 'on_selected_backups'
+        [backup.name for backup in actual_callbacks[1][1]],
+    )
+    assert actual_callbacks[2][0] == "on_selected_backups"
     assert unordered_equal(
-        (backup1_metadata.name, backup3_metadata.name), [backup.name for backup in actual_callbacks[2][1]])
+        (backup1_metadata.name, backup3_metadata.name),
+        [backup.name for backup in actual_callbacks[2][1]],
+    )
 
 
 def test_prune_backups_dry_run(tmpdir: Path) -> None:
     # Normal behaviour of deleting empty backups.
 
     _, backup1_metadata = MakeBackup.empty()(tmpdir)
     _, backup2_metadata = MakeBackup.valid()(tmpdir)
     _, backup3_metadata = MakeBackup.empty()(tmpdir)
 
     config = PruneBackupsConfig(True, BackupPrunabilityOptions(True, False))
 
     actual_callbacks: list[Any] = []
     callbacks = PruneBackupsCallbacks(
-        on_before_read_backups=lambda: actual_callbacks.append('on_before_read_backups'),
+        on_before_read_backups=lambda: actual_callbacks.append("on_before_read_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
         ),
-        on_after_read_backups=lambda backups: actual_callbacks.append(('on_after_read_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('on_selected_backups', backups)),
-        on_delete_error=lambda path, error: pytest.fail(f'Unexpected on_delete_error: {path=} {error=}'),
+        on_after_read_backups=lambda backups: actual_callbacks.append(("on_after_read_backups", backups)),
+        on_selected_backups=lambda backups: actual_callbacks.append(("on_selected_backups", backups)),
+        on_delete_error=lambda path, error: pytest.fail(f"Unexpected on_delete_error: {path=} {error=}"),
     )
 
     with AssertFilesystemUnmodified(tmpdir):
         results = prune_backups(tmpdir, config, callbacks)
 
     assert results == PruneBackupsResults(empty_backups_removed=2, total_backups_removed=2, backups_remaining=1)
-    
-    assert actual_callbacks[0] == 'on_before_read_backups'
-    assert actual_callbacks[1][0] == 'on_after_read_backups'
+
+    assert actual_callbacks[0] == "on_before_read_backups"
+    assert actual_callbacks[1][0] == "on_after_read_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
     assert unordered_equal(
         (backup1_metadata.name, backup2_metadata.name, backup3_metadata.name),
-        [backup.name for backup in actual_callbacks[1][1]])
-    assert actual_callbacks[2][0] == 'on_selected_backups'
+        [backup.name for backup in actual_callbacks[1][1]],
+    )
+    assert actual_callbacks[2][0] == "on_selected_backups"
     assert unordered_equal(
-        (backup1_metadata.name, backup3_metadata.name), [backup.name for backup in actual_callbacks[2][1]])
+        (backup1_metadata.name, backup3_metadata.name),
+        [backup.name for backup in actual_callbacks[2][1]],
+    )
```

### Comparing `incremental_backup-1.2.0/test/test_restore.py` & `incremental_backup-1.2.1/test/test_restore.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 from pathlib import Path
 from typing import Any
 
 import pytest
 
 from incremental_backup.backup.sum import BackupSum
 from incremental_backup.meta.meta import BackupMetadata, ReadBackupsCallbacks
-from incremental_backup.restore import perform_restore, restore_files, RestoreCallbacks, RestoreError, \
-    RestoreFilesCallbacks, RestoreFilesResults, RestoreResults
+from incremental_backup.restore import (
+    RestoreCallbacks,
+    RestoreError,
+    RestoreFilesCallbacks,
+    RestoreFilesResults,
+    RestoreResults,
+    perform_restore,
+    restore_files,
+)
 
-from helpers import AssertFilesystemUnmodified, dir_entries, unordered_equal
+from test.helpers import AssertFilesystemUnmodified, dir_entries, unordered_equal
 
 
 def test_restore_files_empty(tmpdir: Path) -> None:
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     backup_sum = BackupSum()
 
     callbacks = RestoreFilesCallbacks(
-        on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-        on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
+        on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+        on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
     )
 
     with AssertFilesystemUnmodified(target_dir):
         actual_results = restore_files(target_dir, backup_sum, destination_dir, callbacks)
 
     expected_results = RestoreFilesResults(0, False)
     assert actual_results == expected_results
@@ -34,482 +41,574 @@
     assert destination_dir.exists()
     assert dir_entries(destination_dir) == set()
 
 
 def test_restore_files(tmpdir: Path) -> None:
     # Test with some file I/O errors.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
     # I can't be bothered filling in the rest of the metadata here, it shouldn't be used anyway.
-    backup1 = BackupMetadata('apwerfuhv4835t', None, None)
-    backup1_data_dir = target_dir / 'apwerfuhv4835t/data'
+    backup1 = BackupMetadata("apwerfuhv4835t", None, None)
+    backup1_data_dir = target_dir / "apwerfuhv4835t/data"
     backup1_data_dir.mkdir(parents=True)
-    (backup1_data_dir / 'foo.txt').write_text('some thing here')
-    (backup1_data_dir / 'dir1').mkdir()
-    (backup1_data_dir / 'dir1/dir1_file1.1').write_text('dir1_file1 text')
+    (backup1_data_dir / "foo.txt").write_text("some thing here")
+    (backup1_data_dir / "dir1").mkdir()
+    (backup1_data_dir / "dir1/dir1_file1.1").write_text("dir1_file1 text")
 
-    backup2 = BackupMetadata('sfoynbsebo8756s', None, None)
-    backup2_data_dir = target_dir / 'sfoynbsebo8756s/data'
+    backup2 = BackupMetadata("sfoynbsebo8756s", None, None)
+    backup2_data_dir = target_dir / "sfoynbsebo8756s/data"
     backup2_data_dir.mkdir(parents=True)
-    (backup2_data_dir / 'dir1').mkdir()
-    (backup2_data_dir / 'dir1/dir1_file2.png').write_text('45-jsduyfgv4 tyq73 4bt')
-    (backup2_data_dir / 'dir2').mkdir()
-    (backup2_data_dir / 'dir2/dir2_file').write_text(' < > & ~ & < >')
+    (backup2_data_dir / "dir1").mkdir()
+    (backup2_data_dir / "dir1/dir1_file2.png").write_text("45-jsduyfgv4 tyq73 4bt")
+    (backup2_data_dir / "dir2").mkdir()
+    (backup2_data_dir / "dir2/dir2_file").write_text(" < > & ~ & < >")
 
-    backup3 = BackupMetadata('dlrtioyuw3405g', None, None)
-    backup3_data_dir = target_dir / 'dlrtioyuw3405g/data'
+    backup3 = BackupMetadata("dlrtioyuw3405g", None, None)
+    backup3_data_dir = target_dir / "dlrtioyuw3405g/data"
     backup3_data_dir.mkdir(parents=True)
-    (backup3_data_dir / 'dir2/dir2\u5487\u45FE').mkdir(parents=True)
-    (backup3_data_dir / 'dir2/dir2\u5487\u45FE/the\uECF1file\u23FDyes').write_text('final file data')
+    (backup3_data_dir / "dir2/dir2\u5487\u45fe").mkdir(parents=True)
+    (backup3_data_dir / "dir2/dir2\u5487\u45fe/the\uecf1file\u23fdyes").write_text("final file data")
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
-    backup_sum = BackupSum(BackupSum.Directory('',
-        files=[BackupSum.File('foo.txt', backup1), BackupSum.File('nonexistent.file', backup2)], subdirectories=[
-            BackupSum.Directory('dir1',
-                files=[BackupSum.File('dir1_file1.1', backup1), BackupSum.File('dir1_file2.png', backup2)],
-                subdirectories=[BackupSum.Directory('mkdir_error', files=[BackupSum.File('file', backup2)])]),
-            BackupSum.Directory('dir2', files=[BackupSum.File('dir2_file', backup2)], subdirectories=[
-                BackupSum.Directory('nonexistentContents',
-                    files=[BackupSum.File('foo', backup1), BackupSum.File('bar.jpg', backup3)]),
-                BackupSum.Directory('dir2\u5487\u45FE', files=[BackupSum.File('the\uECF1file\u23FDyes', backup3)]),
-            ])
-    ]))
+    backup_sum = BackupSum(
+        BackupSum.Directory(
+            "",
+            files=[
+                BackupSum.File("foo.txt", backup1),
+                BackupSum.File("nonexistent.file", backup2),
+            ],
+            subdirectories=[
+                BackupSum.Directory(
+                    "dir1",
+                    files=[
+                        BackupSum.File("dir1_file1.1", backup1),
+                        BackupSum.File("dir1_file2.png", backup2),
+                    ],
+                    subdirectories=[BackupSum.Directory("mkdir_error", files=[BackupSum.File("file", backup2)])],
+                ),
+                BackupSum.Directory(
+                    "dir2",
+                    files=[BackupSum.File("dir2_file", backup2)],
+                    subdirectories=[
+                        BackupSum.Directory(
+                            "nonexistentContents",
+                            files=[
+                                BackupSum.File("foo", backup1),
+                                BackupSum.File("bar.jpg", backup3),
+                            ],
+                        ),
+                        BackupSum.Directory(
+                            "dir2\u5487\u45fe",
+                            files=[BackupSum.File("the\uecf1file\u23fdyes", backup3)],
+                        ),
+                    ],
+                ),
+            ],
+        )
+    )
 
     # Force mkdir error.
-    (destination_dir / 'dir1').mkdir(parents=True)
-    (destination_dir / 'dir1/mkdir_error').touch()
+    (destination_dir / "dir1").mkdir(parents=True)
+    (destination_dir / "dir1/mkdir_error").touch()
 
     mkdir_errors: list[tuple[Path, Exception]] = []
     copy_errors: list[tuple[Path, Path, Exception]] = []
     callbacks = RestoreFilesCallbacks(
         on_mkdir_error=lambda path, error: mkdir_errors.append((path, error)),
-        on_copy_error=lambda src, dest, error: copy_errors.append((src, dest, error))
+        on_copy_error=lambda src, dest, error: copy_errors.append((src, dest, error)),
     )
 
     with AssertFilesystemUnmodified(target_dir):
         actual_results = restore_files(target_dir, backup_sum, destination_dir, callbacks)
 
-    (destination_dir / 'dir1/mkdir_error').unlink(missing_ok=False)
+    (destination_dir / "dir1/mkdir_error").unlink(missing_ok=False)
 
-    assert [(p, type(e)) for p, e in mkdir_errors] == [(destination_dir / 'dir1/mkdir_error', FileExistsError)]
+    assert [(p, type(e)) for p, e in mkdir_errors] == [(destination_dir / "dir1/mkdir_error", FileExistsError)]
     assert [(s, d, type(e)) for s, d, e in copy_errors] == [
-        (target_dir / 'sfoynbsebo8756s/data/nonexistent.file', destination_dir / 'nonexistent.file', FileNotFoundError),
-        (target_dir / 'apwerfuhv4835t/data/dir2/nonexistentContents/foo', destination_dir / 'dir2/nonexistentContents/foo', FileNotFoundError),
-        (target_dir / 'dlrtioyuw3405g/data/dir2/nonexistentContents/bar.jpg', destination_dir / 'dir2/nonexistentContents/bar.jpg', FileNotFoundError),
+        (
+            target_dir / "sfoynbsebo8756s/data/nonexistent.file",
+            destination_dir / "nonexistent.file",
+            FileNotFoundError,
+        ),
+        (
+            target_dir / "apwerfuhv4835t/data/dir2/nonexistentContents/foo",
+            destination_dir / "dir2/nonexistentContents/foo",
+            FileNotFoundError,
+        ),
+        (
+            target_dir / "dlrtioyuw3405g/data/dir2/nonexistentContents/bar.jpg",
+            destination_dir / "dir2/nonexistentContents/bar.jpg",
+            FileNotFoundError,
+        ),
     ]
 
     expected_results = RestoreFilesResults(5, True)
     assert actual_results == expected_results
 
-    assert dir_entries(destination_dir) == {'foo.txt', 'dir1', 'dir2'}
-    assert (destination_dir / 'foo.txt').read_text() == 'some thing here'
-    assert dir_entries(destination_dir / 'dir1') == {'dir1_file1.1', 'dir1_file2.png'}
-    assert (destination_dir / 'dir1/dir1_file1.1').read_text() == 'dir1_file1 text'
-    assert (destination_dir / 'dir1/dir1_file2.png').read_text() == '45-jsduyfgv4 tyq73 4bt'
-    assert dir_entries(destination_dir / 'dir2') == {'dir2_file', 'dir2\u5487\u45FE', 'nonexistentContents'}
-    assert (destination_dir / 'dir2/dir2_file').read_text() == ' < > & ~ & < >'
-    assert dir_entries(destination_dir / 'dir2/dir2\u5487\u45FE') == {'the\uECF1file\u23FDyes'}
-    assert (destination_dir / 'dir2/dir2\u5487\u45FE/the\uECF1file\u23FDyes').read_text() == 'final file data'
-    assert dir_entries(destination_dir / 'dir2/nonexistentContents') == set()
+    assert dir_entries(destination_dir) == {"foo.txt", "dir1", "dir2"}
+    assert (destination_dir / "foo.txt").read_text() == "some thing here"
+    assert dir_entries(destination_dir / "dir1") == {"dir1_file1.1", "dir1_file2.png"}
+    assert (destination_dir / "dir1/dir1_file1.1").read_text() == "dir1_file1 text"
+    assert (destination_dir / "dir1/dir1_file2.png").read_text() == "45-jsduyfgv4 tyq73 4bt"
+    assert dir_entries(destination_dir / "dir2") == {
+        "dir2_file",
+        "dir2\u5487\u45fe",
+        "nonexistentContents",
+    }
+    assert (destination_dir / "dir2/dir2_file").read_text() == " < > & ~ & < >"
+    assert dir_entries(destination_dir / "dir2/dir2\u5487\u45fe") == {"the\uecf1file\u23fdyes"}
+    assert (destination_dir / "dir2/dir2\u5487\u45fe/the\uecf1file\u23fdyes").read_text() == "final file data"
+    assert dir_entries(destination_dir / "dir2/nonexistentContents") == set()
 
 
 def test_perform_restore_invalid_args(tmpdir: Path) -> None:
-    target_dir = tmpdir / 'backups'
-    destination_dir = tmpdir / 'destination'
-    backup_name = '49538tsnuefdgy'
+    target_dir = tmpdir / "backups"
+    destination_dir = tmpdir / "destination"
+    backup_name = "49538tsnuefdgy"
     backup_time = datetime(2021, 11, 15, 19, 15, 23, tzinfo=timezone.utc)
 
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: pytest.fail('Unexpected on_before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: pytest.fail("Unexpected on_before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            pytest.fail(f'Unexpected on_after_read_previous_backups: {backups=}'),
-        on_selected_backups=lambda backups: pytest.fail(f'Unexpected on_selected_backups: {backups=}'),
-        on_before_initialise_restore=lambda: pytest.fail(f'Unexpected on_before_initialise_restore'),
-        on_before_restore_files=lambda: pytest.fail(f'Unexpected on_before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: pytest.fail(
+            f"Unexpected on_after_read_previous_backups: {backups=}"
+        ),
+        on_selected_backups=lambda backups: pytest.fail(f"Unexpected on_selected_backups: {backups=}"),
+        on_before_initialise_restore=lambda: pytest.fail("Unexpected on_before_initialise_restore"),
+        on_before_restore_files=lambda: pytest.fail("Unexpected on_before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(tmpdir):
         with pytest.raises(ValueError):
             perform_restore(target_dir, destination_dir, backup_name, backup_time, callbacks)
 
 
 def test_perform_restore_nonexistent_target(tmpdir: Path) -> None:
     # Backup target directory doesn't exist.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: pytest.fail('Unexpected on_before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: pytest.fail("Unexpected on_before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            pytest.fail(f'Unexpected on_after_read_previous_backups: {backups=}'),
-        on_selected_backups=lambda backups: pytest.fail(f'Unexpected on_selected_backups: {backups=}'),
-        on_before_initialise_restore=lambda: pytest.fail(f'Unexpected on_before_initialise_restore'),
-        on_before_restore_files=lambda: pytest.fail(f'Unexpected on_before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: pytest.fail(
+            f"Unexpected on_after_read_previous_backups: {backups=}"
+        ),
+        on_selected_backups=lambda backups: pytest.fail(f"Unexpected on_selected_backups: {backups=}"),
+        on_before_initialise_restore=lambda: pytest.fail("Unexpected on_before_initialise_restore"),
+        on_before_restore_files=lambda: pytest.fail("Unexpected on_before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(tmpdir):
         with pytest.raises(RestoreError):
             perform_restore(target_dir, destination_dir, callbacks=callbacks)
 
 
 def test_perform_restore_nonempty_destination(tmpdir: Path) -> None:
     # Destination directory exists and contains files. Should not attempt to restore files.
 
-    target_dir = tmpdir / 'backups'
-    backup1_dir = target_dir / '98we45t70vwh3478tr'
+    target_dir = tmpdir / "backups"
+    backup1_dir = target_dir / "98we45t70vwh3478tr"
     backup1_dir.mkdir(parents=True)
-    (backup1_dir / 'start.json').write_text('{"start_time": "2002-11-22T05:50:12.341256+00:00"}', encoding='utf8')
-    (backup1_dir / 'manifest.json').write_text('[{"n": "", "cf": ["foo"]}]', encoding='utf8')
-    (backup1_dir / 'completion.json').write_text(
-        '{"start_time": "2002-11-22T05:50:20.495673+00:00", "paths_skipped": false}', encoding='utf8')
-    (backup1_dir / 'data').mkdir()
-    (backup1_dir / 'data/foo').write_text('Hello world!')
+    (backup1_dir / "start.json").write_text('{"start_time": "2002-11-22T05:50:12.341256+00:00"}', encoding="utf8")
+    (backup1_dir / "manifest.json").write_text('[{"n": "", "cf": ["foo"]}]', encoding="utf8")
+    (backup1_dir / "completion.json").write_text(
+        '{"start_time": "2002-11-22T05:50:20.495673+00:00", "paths_skipped": false}',
+        encoding="utf8",
+    )
+    (backup1_dir / "data").mkdir()
+    (backup1_dir / "data/foo").write_text("Hello world!")
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
     destination_dir.mkdir()
-    (destination_dir / 'foo').write_text('Do not overwrite me!')
-    (destination_dir / 'bar.txt').write_text('Nor me!')
-    (destination_dir / 'qux').mkdir()
+    (destination_dir / "foo").write_text("Do not overwrite me!")
+    (destination_dir / "bar.txt").write_text("Nor me!")
+    (destination_dir / "qux").mkdir()
 
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: pytest.fail('Unexpected on_before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: pytest.fail("Unexpected on_before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            pytest.fail(f'Unexpected on_after_read_previous_backups: {backups=}'),
-        on_selected_backups=lambda backups: pytest.fail(f'Unexpected on_selected_backups: {backups=}'),
-        on_before_initialise_restore=lambda: pytest.fail(f'Unexpected on_before_initialise_restore'),
-        on_before_restore_files=lambda: pytest.fail(f'Unexpected on_before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: pytest.fail(
+            f"Unexpected on_after_read_previous_backups: {backups=}"
+        ),
+        on_selected_backups=lambda backups: pytest.fail(f"Unexpected on_selected_backups: {backups=}"),
+        on_before_initialise_restore=lambda: pytest.fail("Unexpected on_before_initialise_restore"),
+        on_before_restore_files=lambda: pytest.fail("Unexpected on_before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(target_dir, destination_dir):
         with pytest.raises(RestoreError):
             perform_restore(target_dir, destination_dir, callbacks=callbacks)
 
 
 def test_perform_restore_nonexistent_backup(tmpdir: Path) -> None:
     # backup_name is specified but that backup doesn't exist - shouldn't restore anything.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
-    backup1_dir = target_dir / 'E49YHUDFIG'
+    backup1_dir = target_dir / "E49YHUDFIG"
     backup1_dir.mkdir()
-    (backup1_dir / 'start.json').write_text('{"start_time": "2002-11-22T05:50:12.341256+00:00"}', encoding='utf8')
-    (backup1_dir / 'manifest.json').write_text('[{"n": "", "cf": ["foo"]}]', encoding='utf8')
-    (backup1_dir / 'completion.json').write_text(
-        '{"start_time": "2002-11-22T05:50:20.495673+00:00", "paths_skipped": false}', encoding='utf8')
-    (backup1_dir / 'data').mkdir()
-    (backup1_dir / 'data/foo').write_text('Hello world!')
+    (backup1_dir / "start.json").write_text('{"start_time": "2002-11-22T05:50:12.341256+00:00"}', encoding="utf8")
+    (backup1_dir / "manifest.json").write_text('[{"n": "", "cf": ["foo"]}]', encoding="utf8")
+    (backup1_dir / "completion.json").write_text(
+        '{"start_time": "2002-11-22T05:50:20.495673+00:00", "paths_skipped": false}',
+        encoding="utf8",
+    )
+    (backup1_dir / "data").mkdir()
+    (backup1_dir / "data/foo").write_text("Hello world!")
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     callbacks = RestoreCallbacks(
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_selected_backups=lambda backups: pytest.fail(f'Unexpected on_selected_backups: {backups=}'),
-        on_before_initialise_restore=lambda: pytest.fail(f'Unexpected on_before_initialise_restore'),
-        on_before_restore_files=lambda: pytest.fail(f'Unexpected on_before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_selected_backups=lambda backups: pytest.fail(f"Unexpected on_selected_backups: {backups=}"),
+        on_before_initialise_restore=lambda: pytest.fail("Unexpected on_before_initialise_restore"),
+        on_before_restore_files=lambda: pytest.fail("Unexpected on_before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(target_dir, destination_dir):
         with pytest.raises(RestoreError):
-            perform_restore(target_dir, destination_dir, backup_name='3498tisg4o8aoe', callbacks=callbacks)
+            perform_restore(
+                target_dir,
+                destination_dir,
+                backup_name="3498tisg4o8aoe",
+                callbacks=callbacks,
+            )
 
 
 def test_perform_restore_all(tmpdir: Path) -> None:
     # Neither backup_name nor backup_time is specified, restore all backups.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
-    backup1_dir = target_dir / 'ws3e48ohitv'
+    backup1_dir = target_dir / "ws3e48ohitv"
     backup1_dir.mkdir()
-    (backup1_dir / 'start.json').write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup1_data_dir = backup1_dir / 'data'
+    (backup1_dir / "start.json").write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup1_data_dir = backup1_dir / "data"
     backup1_data_dir.mkdir()
-    (backup1_data_dir / 'foo.jpg').write_text('hello world')
-    (backup1_data_dir / 'manama').write_text('goodbye world')
-    (backup1_data_dir / 'myDir').mkdir()
-    (backup1_data_dir / 'myDir' / 'bar-qux').write_text('first content')
-    (backup1_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["foo.jpg", "manama"]},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup1_data_dir / "foo.jpg").write_text("hello world")
+    (backup1_data_dir / "manama").write_text("goodbye world")
+    (backup1_data_dir / "myDir").mkdir()
+    (backup1_data_dir / "myDir" / "bar-qux").write_text("first content")
+    (backup1_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["foo.jpg", "manama"]},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup2_dir = target_dir / '9w384rapw9ssa'
+    backup2_dir = target_dir / "9w384rapw9ssa"
     backup2_dir.mkdir()
-    (backup2_dir / 'start.json').write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup2_data_dir = backup2_dir / 'data'
+    (backup2_dir / "start.json").write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup2_data_dir = backup2_dir / "data"
     backup2_data_dir.mkdir()
-    (backup2_data_dir / 'yes.no').write_text('hello world 2')
-    (backup2_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["yes.no"]},
-            {"n": "myDir", "rf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup2_data_dir / "yes.no").write_text("hello world 2")
+    (backup2_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["yes.no"]},
+            {"n": "myDir", "rf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup3_dir = target_dir / '98P678676h9645'
+    backup3_dir = target_dir / "98P678676h9645"
     backup3_dir.mkdir()
-    (backup3_dir / 'start.json').write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding='utf8')
-    backup3_data_dir = backup3_dir / 'data'
+    (backup3_dir / "start.json").write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding="utf8")
+    backup3_data_dir = backup3_dir / "data"
     backup3_data_dir.mkdir()
-    (backup3_data_dir / 'myDir').mkdir()
-    (backup3_data_dir / 'myDir' / 'bar-qux').write_text('final content')
-    (backup3_dir / 'manifest.json').write_text(
-        '''[{"n": ""},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup3_data_dir / "myDir").mkdir()
+    (backup3_data_dir / "myDir" / "bar-qux").write_text("final content")
+    (backup3_dir / "manifest.json").write_text(
+        """[{"n": ""},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     actual_callbacks: list[Any] = []
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: actual_callbacks.append('before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: actual_callbacks.append("before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            actual_callbacks.append(('after_read_previous_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('selected_backups', backups)),
-        on_before_initialise_restore=lambda: actual_callbacks.append('before_initialise_restore'),
-        on_before_restore_files=lambda: actual_callbacks.append('before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: actual_callbacks.append(
+            ("after_read_previous_backups", backups)
+        ),
+        on_selected_backups=lambda backups: actual_callbacks.append(("selected_backups", backups)),
+        on_before_initialise_restore=lambda: actual_callbacks.append("before_initialise_restore"),
+        on_before_restore_files=lambda: actual_callbacks.append("before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(target_dir):
         actual_results = perform_restore(target_dir, destination_dir, callbacks=callbacks)
 
     assert len(actual_callbacks) == 5
-    assert actual_callbacks[0] == 'before_read_previous_backups'
-    assert actual_callbacks[1][0] == 'after_read_previous_backups'
+    assert actual_callbacks[0] == "before_read_previous_backups"
+    assert actual_callbacks[1][0] == "after_read_previous_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
-    assert unordered_equal([b.name for b in actual_callbacks[1][1]], ['ws3e48ohitv', '9w384rapw9ssa', '98P678676h9645'])
-    assert actual_callbacks[2][0] == 'selected_backups'
-    assert unordered_equal([b.name for b in actual_callbacks[2][1]], ['ws3e48ohitv', '9w384rapw9ssa', '98P678676h9645'])
-    assert actual_callbacks[3] == 'before_initialise_restore'
-    assert actual_callbacks[4] == 'before_restore_files'
+    assert unordered_equal(
+        [b.name for b in actual_callbacks[1][1]],
+        ["ws3e48ohitv", "9w384rapw9ssa", "98P678676h9645"],
+    )
+    assert actual_callbacks[2][0] == "selected_backups"
+    assert unordered_equal(
+        [b.name for b in actual_callbacks[2][1]],
+        ["ws3e48ohitv", "9w384rapw9ssa", "98P678676h9645"],
+    )
+    assert actual_callbacks[3] == "before_initialise_restore"
+    assert actual_callbacks[4] == "before_restore_files"
 
     assert actual_results == RestoreResults(4, False)
 
-    assert dir_entries(destination_dir) == {'foo.jpg', 'manama', 'yes.no', 'myDir'}
-    assert (destination_dir / 'foo.jpg').read_text() == 'hello world'
-    assert (destination_dir / 'manama').read_text() == 'goodbye world'
-    assert (destination_dir / 'yes.no').read_text() == 'hello world 2'
-    assert dir_entries(destination_dir / 'myDir') == {'bar-qux'}
-    assert (destination_dir / 'myDir' / 'bar-qux').read_text() == 'final content'
+    assert dir_entries(destination_dir) == {"foo.jpg", "manama", "yes.no", "myDir"}
+    assert (destination_dir / "foo.jpg").read_text() == "hello world"
+    assert (destination_dir / "manama").read_text() == "goodbye world"
+    assert (destination_dir / "yes.no").read_text() == "hello world 2"
+    assert dir_entries(destination_dir / "myDir") == {"bar-qux"}
+    assert (destination_dir / "myDir" / "bar-qux").read_text() == "final content"
 
 
 def test_perform_restore_name(tmpdir: Path) -> None:
     # backup_name is specified, restore up to that backup.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
-    backup1_dir = target_dir / 'ws3e48ohitv'
+    backup1_dir = target_dir / "ws3e48ohitv"
     backup1_dir.mkdir()
-    (backup1_dir / 'start.json').write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup1_data_dir = backup1_dir / 'data'
+    (backup1_dir / "start.json").write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup1_data_dir = backup1_dir / "data"
     backup1_data_dir.mkdir()
-    (backup1_data_dir / 'foo.jpg').write_text('hello world')
-    (backup1_data_dir / 'manama').write_text('goodbye world')
-    (backup1_data_dir / 'myDir').mkdir()
-    (backup1_data_dir / 'myDir' / 'bar-qux').write_text('first content')
-    (backup1_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["foo.jpg", "manama"]},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup1_data_dir / "foo.jpg").write_text("hello world")
+    (backup1_data_dir / "manama").write_text("goodbye world")
+    (backup1_data_dir / "myDir").mkdir()
+    (backup1_data_dir / "myDir" / "bar-qux").write_text("first content")
+    (backup1_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["foo.jpg", "manama"]},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup2_dir = target_dir / '9w384rapw9ssa'
+    backup2_dir = target_dir / "9w384rapw9ssa"
     backup2_dir.mkdir()
-    (backup2_dir / 'start.json').write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup2_data_dir = backup2_dir / 'data'
+    (backup2_dir / "start.json").write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup2_data_dir = backup2_dir / "data"
     backup2_data_dir.mkdir()
-    (backup2_data_dir / 'yes.no').write_text('hello world 2')
-    (backup2_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["yes.no"]},
-            {"n": "myDir", "rf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup2_data_dir / "yes.no").write_text("hello world 2")
+    (backup2_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["yes.no"]},
+            {"n": "myDir", "rf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup3_dir = target_dir / '98P678676h9645'
+    backup3_dir = target_dir / "98P678676h9645"
     backup3_dir.mkdir()
-    (backup3_dir / 'start.json').write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding='utf8')
-    backup3_data_dir = backup3_dir / 'data'
+    (backup3_dir / "start.json").write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding="utf8")
+    backup3_data_dir = backup3_dir / "data"
     backup3_data_dir.mkdir()
-    (backup3_data_dir / 'myDir').mkdir()
-    (backup3_data_dir / 'myDir' / 'bar-qux').write_text('final content')
-    (backup3_dir / 'manifest.json').write_text(
-        '''[{"n": ""},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup3_data_dir / "myDir").mkdir()
+    (backup3_data_dir / "myDir" / "bar-qux").write_text("final content")
+    (backup3_dir / "manifest.json").write_text(
+        """[{"n": ""},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     actual_callbacks: list[Any] = []
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: actual_callbacks.append('before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: actual_callbacks.append("before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            actual_callbacks.append(('after_read_previous_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('selected_backups', backups)),
-        on_before_initialise_restore=lambda: actual_callbacks.append('before_initialise_restore'),
-        on_before_restore_files=lambda: actual_callbacks.append('before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: actual_callbacks.append(
+            ("after_read_previous_backups", backups)
+        ),
+        on_selected_backups=lambda backups: actual_callbacks.append(("selected_backups", backups)),
+        on_before_initialise_restore=lambda: actual_callbacks.append("before_initialise_restore"),
+        on_before_restore_files=lambda: actual_callbacks.append("before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(target_dir):
-        actual_results = perform_restore(target_dir, destination_dir, backup_name='9w384rapw9ssa', callbacks=callbacks)
+        actual_results = perform_restore(
+            target_dir,
+            destination_dir,
+            backup_name="9w384rapw9ssa",
+            callbacks=callbacks,
+        )
 
     assert len(actual_callbacks) == 5
-    assert actual_callbacks[0] == 'before_read_previous_backups'
-    assert actual_callbacks[1][0] == 'after_read_previous_backups'
+    assert actual_callbacks[0] == "before_read_previous_backups"
+    assert actual_callbacks[1][0] == "after_read_previous_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
-    assert unordered_equal([b.name for b in actual_callbacks[1][1]], ['ws3e48ohitv', '9w384rapw9ssa', '98P678676h9645'])
-    assert actual_callbacks[2][0] == 'selected_backups'
-    assert unordered_equal([b.name for b in actual_callbacks[2][1]], ['ws3e48ohitv', '9w384rapw9ssa'])
-    assert actual_callbacks[3] == 'before_initialise_restore'
-    assert actual_callbacks[4] == 'before_restore_files'
+    assert unordered_equal(
+        [b.name for b in actual_callbacks[1][1]],
+        ["ws3e48ohitv", "9w384rapw9ssa", "98P678676h9645"],
+    )
+    assert actual_callbacks[2][0] == "selected_backups"
+    assert unordered_equal([b.name for b in actual_callbacks[2][1]], ["ws3e48ohitv", "9w384rapw9ssa"])
+    assert actual_callbacks[3] == "before_initialise_restore"
+    assert actual_callbacks[4] == "before_restore_files"
 
     assert actual_results == RestoreResults(3, False)
 
-    assert dir_entries(destination_dir) == {'foo.jpg', 'manama', 'yes.no'}
-    assert (destination_dir / 'foo.jpg').read_text() == 'hello world'
-    assert (destination_dir / 'manama').read_text() == 'goodbye world'
-    assert (destination_dir / 'yes.no').read_text() == 'hello world 2'
+    assert dir_entries(destination_dir) == {"foo.jpg", "manama", "yes.no"}
+    assert (destination_dir / "foo.jpg").read_text() == "hello world"
+    assert (destination_dir / "manama").read_text() == "goodbye world"
+    assert (destination_dir / "yes.no").read_text() == "hello world 2"
 
 
 def test_perform_restore_time(tmpdir: Path) -> None:
     # backup_time is specified, restore up to that time.
 
-    target_dir = tmpdir / 'backups'
+    target_dir = tmpdir / "backups"
     target_dir.mkdir()
 
-    backup1_dir = target_dir / 'ws3e48ohitv'
+    backup1_dir = target_dir / "ws3e48ohitv"
     backup1_dir.mkdir()
-    (backup1_dir / 'start.json').write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup1_data_dir = backup1_dir / 'data'
+    (backup1_dir / "start.json").write_text('{"start_time": "2022-03-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup1_data_dir = backup1_dir / "data"
     backup1_data_dir.mkdir()
-    (backup1_data_dir / 'foo.jpg').write_text('hello world')
-    (backup1_data_dir / 'manama').write_text('goodbye world')
-    (backup1_data_dir / 'myDir').mkdir()
-    (backup1_data_dir / 'myDir' / 'bar-qux').write_text('first content')
-    (backup1_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["foo.jpg", "manama"]},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup1_data_dir / "foo.jpg").write_text("hello world")
+    (backup1_data_dir / "manama").write_text("goodbye world")
+    (backup1_data_dir / "myDir").mkdir()
+    (backup1_data_dir / "myDir" / "bar-qux").write_text("first content")
+    (backup1_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["foo.jpg", "manama"]},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup2_dir = target_dir / '9w384rapw9ssa'
+    backup2_dir = target_dir / "9w384rapw9ssa"
     backup2_dir.mkdir()
-    (backup2_dir / 'start.json').write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding='utf8')
-    backup2_data_dir = backup2_dir / 'data'
+    (backup2_dir / "start.json").write_text('{"start_time": "2022-04-12T11:53:22.954665+00:00"}', encoding="utf8")
+    backup2_data_dir = backup2_dir / "data"
     backup2_data_dir.mkdir()
-    (backup2_data_dir / 'yes.no').write_text('hello world 2')
-    (backup2_dir / 'manifest.json').write_text(
-        '''[{"n": "", "cf": ["yes.no"]},
-            {"n": "myDir", "rf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup2_data_dir / "yes.no").write_text("hello world 2")
+    (backup2_dir / "manifest.json").write_text(
+        """[{"n": "", "cf": ["yes.no"]},
+            {"n": "myDir", "rf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    backup3_dir = target_dir / '98P678676h9645'
+    backup3_dir = target_dir / "98P678676h9645"
     backup3_dir.mkdir()
-    (backup3_dir / 'start.json').write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding='utf8')
-    backup3_data_dir = backup3_dir / 'data'
+    (backup3_dir / "start.json").write_text('{"start_time": "2022-04-25T14:50:59.430968+00:00"}', encoding="utf8")
+    backup3_data_dir = backup3_dir / "data"
     backup3_data_dir.mkdir()
-    (backup3_data_dir / 'myDir').mkdir()
-    (backup3_data_dir / 'myDir' / 'bar-qux').write_text('final content')
-    (backup3_dir / 'manifest.json').write_text(
-        '''[{"n": ""},
-            {"n": "myDir", "cf": ["bar-qux"]}]''',
-        encoding='utf8')
+    (backup3_data_dir / "myDir").mkdir()
+    (backup3_data_dir / "myDir" / "bar-qux").write_text("final content")
+    (backup3_dir / "manifest.json").write_text(
+        """[{"n": ""},
+            {"n": "myDir", "cf": ["bar-qux"]}]""",
+        encoding="utf8",
+    )
 
-    destination_dir = tmpdir / 'destination'
+    destination_dir = tmpdir / "destination"
 
     actual_callbacks: list[Any] = []
     callbacks = RestoreCallbacks(
-        on_before_read_previous_backups=lambda: actual_callbacks.append('before_read_previous_backups'),
+        on_before_read_previous_backups=lambda: actual_callbacks.append("before_read_previous_backups"),
         read_backups=ReadBackupsCallbacks(
-            on_query_entry_error=lambda path, error: pytest.fail(f'Unexpected on_query_entry_error: {path=} {error=}'),
-            on_read_metadata_error=lambda path, error:
-                pytest.fail(f'Unexpected on_read_metadata_error: {path=} {error=}')
-        ),
-        on_after_read_previous_backups=lambda backups:
-            actual_callbacks.append(('after_read_previous_backups', backups)),
-        on_selected_backups=lambda backups: actual_callbacks.append(('selected_backups', backups)),
-        on_before_initialise_restore=lambda: actual_callbacks.append('before_initialise_restore'),
-        on_before_restore_files=lambda: actual_callbacks.append('before_restore_files'),
+            on_query_entry_error=lambda path, error: pytest.fail(f"Unexpected on_query_entry_error: {path=} {error=}"),
+            on_read_metadata_error=lambda path, error: pytest.fail(
+                f"Unexpected on_read_metadata_error: {path=} {error=}"
+            ),
+        ),
+        on_after_read_previous_backups=lambda backups: actual_callbacks.append(
+            ("after_read_previous_backups", backups)
+        ),
+        on_selected_backups=lambda backups: actual_callbacks.append(("selected_backups", backups)),
+        on_before_initialise_restore=lambda: actual_callbacks.append("before_initialise_restore"),
+        on_before_restore_files=lambda: actual_callbacks.append("before_restore_files"),
         restore_files=RestoreFilesCallbacks(
-            on_mkdir_error=lambda path, error: pytest.fail(f'Unexpected on_mkdir_error: {path=} {error=}'),
-            on_copy_error=lambda src, dest, error: pytest.fail(f'Unexpected on_copy_error: {src=} {dest=} {error=}')
-        )
+            on_mkdir_error=lambda path, error: pytest.fail(f"Unexpected on_mkdir_error: {path=} {error=}"),
+            on_copy_error=lambda src, dest, error: pytest.fail(f"Unexpected on_copy_error: {src=} {dest=} {error=}"),
+        ),
     )
 
     with AssertFilesystemUnmodified(target_dir):
         actual_results = perform_restore(
-            target_dir, destination_dir, backup_time=datetime(2022, 4, 12, 11, 53, 22, 954665, tzinfo=timezone.utc),
-            callbacks=callbacks)
+            target_dir,
+            destination_dir,
+            backup_time=datetime(2022, 4, 12, 11, 53, 22, 954665, tzinfo=timezone.utc),
+            callbacks=callbacks,
+        )
 
     assert len(actual_callbacks) == 5
-    assert actual_callbacks[0] == 'before_read_previous_backups'
-    assert actual_callbacks[1][0] == 'after_read_previous_backups'
+    assert actual_callbacks[0] == "before_read_previous_backups"
+    assert actual_callbacks[1][0] == "after_read_previous_backups"
     # I can't be bothered testing that all the metadata is the same, I assume it is otherwise other things will likely
     # break anyway
-    assert unordered_equal([b.name for b in actual_callbacks[1][1]], ['ws3e48ohitv', '9w384rapw9ssa', '98P678676h9645'])
-    assert actual_callbacks[2][0] == 'selected_backups'
-    assert unordered_equal([b.name for b in actual_callbacks[2][1]], ['ws3e48ohitv', '9w384rapw9ssa'])
-    assert actual_callbacks[3] == 'before_initialise_restore'
-    assert actual_callbacks[4] == 'before_restore_files'
+    assert unordered_equal(
+        [b.name for b in actual_callbacks[1][1]],
+        ["ws3e48ohitv", "9w384rapw9ssa", "98P678676h9645"],
+    )
+    assert actual_callbacks[2][0] == "selected_backups"
+    assert unordered_equal([b.name for b in actual_callbacks[2][1]], ["ws3e48ohitv", "9w384rapw9ssa"])
+    assert actual_callbacks[3] == "before_initialise_restore"
+    assert actual_callbacks[4] == "before_restore_files"
 
     assert actual_results == RestoreResults(3, False)
 
-    assert dir_entries(destination_dir) == {'foo.jpg', 'manama', 'yes.no'}
-    assert (destination_dir / 'foo.jpg').read_text() == 'hello world'
-    assert (destination_dir / 'manama').read_text() == 'goodbye world'
-    assert (destination_dir / 'yes.no').read_text() == 'hello world 2'
+    assert dir_entries(destination_dir) == {"foo.jpg", "manama", "yes.no"}
+    assert (destination_dir / "foo.jpg").read_text() == "hello world"
+    assert (destination_dir / "manama").read_text() == "goodbye world"
+    assert (destination_dir / "yes.no").read_text() == "hello world 2"
```

