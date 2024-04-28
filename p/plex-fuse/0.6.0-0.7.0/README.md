# Comparing `tmp/plex-fuse-0.6.0.tar.gz` & `tmp/plex_fuse-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-fuse-0.6.0.tar", last modified: Wed Apr 10 13:44:37 2024, max compression
+gzip compressed data, was "plex_fuse-0.7.0.tar", last modified: Sun Apr 28 18:14:37 2024, max compression
```

## Comparing `plex-fuse-0.6.0.tar` & `plex_fuse-0.7.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/plex_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 13:44:37.000000 plex-fuse-0.6.0/plex_fuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.271532 plex-fuse-0.6.0/plexfuse/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/CacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/CachedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/DelayedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/FileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/HttpCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/cache/UserDictCacheControl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/control/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/control/ControlListener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/FsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexFS.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/PlexFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/Timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/fs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.275532 plex-fuse-0.6.0/plexfuse/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/ChunkedFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/Control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/Playable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/PlexVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/plexfuse/vfs/entry/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/AttrEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/ControlEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/ControlSockEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/DirEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/EpisodeEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/LibraryEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/MovieEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/PathEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/PlexMatchEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SeasonEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/plexfuse/vfs/entry/SubtitleEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:44:37.279532 plex-fuse-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_chunk_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_chunk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_file_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_file_copy_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 13:44:30.000000 plex-fuse-0.6.0/tests/test_socket_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.775156 plex_fuse-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-28 18:14:37.775156 plex_fuse-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.775156 plex_fuse-0.7.0/plex_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 18:14:37.000000 plex_fuse-0.7.0/plex_fuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.767156 plex_fuse-0.7.0/plexfuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/TimeoutLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.767156 plex_fuse-0.7.0/plexfuse/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/CacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/CachedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/DelayedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/FileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/HttpCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/cache/UserDictCacheControl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.767156 plex_fuse-0.7.0/plexfuse/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/control/Control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/control/ControlListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/control/ControlVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.771156 plex_fuse-0.7.0/plexfuse/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/FsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/PlexDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/PlexFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/PlexFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/Timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/fs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.771156 plex_fuse-0.7.0/plexfuse/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/plex/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.771156 plex_fuse-0.7.0/plexfuse/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/ChunkedFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/Playable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/PlexVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.771156 plex_fuse-0.7.0/plexfuse/vfs/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/AttrEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/ControlSockEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/DirEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/EpisodeEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/LibraryEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/MovieEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/PathEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/PlexMatchEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/SeasonEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/SectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/SubtitleEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/plexfuse/vfs/entry/SymlinkEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:14:37.775156 plex_fuse-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:14:37.775156 plex_fuse-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_chunk_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_chunk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_file_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_file_copy_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_socket_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-28 18:14:30.000000 plex_fuse-0.7.0/tests/test_timeout_lock.py
```

### Comparing `plex-fuse-0.6.0/LICENSE` & `plex_fuse-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/PKG-INFO` & `plex_fuse-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.6.0
+Version: 0.7.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex-fuse-0.6.0/README.md` & `plex_fuse-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plex_fuse.egg-info/PKG-INFO` & `plex_fuse-0.7.0/plex_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.6.0
+Version: 0.7.0
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex-fuse-0.6.0/plex_fuse.egg-info/SOURCES.txt` & `plex_fuse-0.7.0/plex_fuse.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,50 +3,53 @@
 pyproject.toml
 plex_fuse.egg-info/PKG-INFO
 plex_fuse.egg-info/SOURCES.txt
 plex_fuse.egg-info/dependency_links.txt
 plex_fuse.egg-info/entry_points.txt
 plex_fuse.egg-info/requires.txt
 plex_fuse.egg-info/top_level.txt
+plexfuse/TimeoutLock.py
 plexfuse/__main__.py
 plexfuse/__version__.py
 plexfuse/normalize.py
 plexfuse/cache/CacheControl.py
 plexfuse/cache/CachedPropertyCacheControl.py
 plexfuse/cache/DelayedPropertyCacheControl.py
 plexfuse/cache/FileCache.py
 plexfuse/cache/HttpCache.py
 plexfuse/cache/UserDictCacheControl.py
+plexfuse/control/Control.py
 plexfuse/control/ControlListener.py
+plexfuse/control/ControlVFS.py
 plexfuse/fs/FsOptions.py
 plexfuse/fs/PlexDirectory.py
 plexfuse/fs/PlexFS.py
 plexfuse/fs/PlexFile.py
 plexfuse/fs/RefCountedDict.py
 plexfuse/fs/Timestampable.py
 plexfuse/fs/main.py
 plexfuse/plex/Monitor.py
 plexfuse/plex/PlexApi.py
 plexfuse/plex/types.py
 plexfuse/vfs/ChunkedFile.py
-plexfuse/vfs/Control.py
 plexfuse/vfs/Playable.py
 plexfuse/vfs/PlexVFS.py
 plexfuse/vfs/entry/AttrEntry.py
-plexfuse/vfs/entry/ControlEntry.py
 plexfuse/vfs/entry/ControlSockEntry.py
 plexfuse/vfs/entry/DirEntry.py
 plexfuse/vfs/entry/EpisodeEntry.py
 plexfuse/vfs/entry/FileEntry.py
 plexfuse/vfs/entry/LibraryEntry.py
 plexfuse/vfs/entry/MovieEntry.py
 plexfuse/vfs/entry/PathEntry.py
 plexfuse/vfs/entry/PlexMatchEntry.py
 plexfuse/vfs/entry/SeasonEntry.py
 plexfuse/vfs/entry/SectionEntry.py
 plexfuse/vfs/entry/SubtitleEntry.py
+plexfuse/vfs/entry/SymlinkEntry.py
 tests/test_RefCountedDict.py
 tests/test_chunk_calc.py
 tests/test_chunk_read.py
 tests/test_file_copy.py
 tests/test_file_copy_partial.py
-tests/test_socket_control.py
+tests/test_socket_control.py
+tests/test_timeout_lock.py
```

### Comparing `plex-fuse-0.6.0/plexfuse/cache/CacheControl.py` & `plex_fuse-0.7.0/plexfuse/cache/CacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/cache/CachedPropertyCacheControl.py` & `plex_fuse-0.7.0/plexfuse/cache/CachedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/cache/DelayedPropertyCacheControl.py` & `plex_fuse-0.7.0/plexfuse/cache/DelayedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/cache/FileCache.py` & `plex_fuse-0.7.0/plexfuse/cache/FileCache.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/cache/HttpCache.py` & `plex_fuse-0.7.0/plexfuse/cache/HttpCache.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/cache/UserDictCacheControl.py` & `plex_fuse-0.7.0/plexfuse/cache/UserDictCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/control/ControlListener.py` & `plex_fuse-0.7.0/plexfuse/control/ControlListener.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import os.path
 import socket
 from threading import Thread
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from plexfuse.vfs.Control import Control
+    from plexfuse.control.Control import Control
 
 
 class ControlListener:
     def __init__(self, path: str, control: Control):
         self.path = path
         self.control = control
         self.thread = None
```

### Comparing `plex-fuse-0.6.0/plexfuse/fs/PlexFS.py` & `plex_fuse-0.7.0/plexfuse/fs/PlexFS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import errno
 from functools import cache, cached_property
 from pathlib import Path
-from threading import Lock
 
 import fuse
 
+from plexfuse.control.Control import Control
 from plexfuse.control.ControlListener import ControlListener
 from plexfuse.fs.FsOptions import FsOptions
 from plexfuse.fs.PlexDirectory import PlexDirectory
 from plexfuse.fs.PlexFile import PlexFile
 from plexfuse.fs.RefCountedDict import RefCountedDict
 from plexfuse.normalize import normalize
 from plexfuse.plex.Monitor import Monitor
 from plexfuse.plex.PlexApi import PlexApi
+from plexfuse.TimeoutLock import TimeoutLock
 from plexfuse.vfs.entry.DirEntry import DirEntry
 from plexfuse.vfs.PlexVFS import PlexVFS
 
 
 class PlexFS(fuse.Fuse):
     control: ControlListener | None
     monitor: Monitor | None
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.options = FsOptions()
         self.control = None
         self.monitor = None
         self.file_map = RefCountedDict()
-        self.iolock = Lock()
+        self.iolock = TimeoutLock(60)
 
     @cached_property
     def plex(self):
         return PlexApi()
 
     @cached_property
     def vfs(self):
-        return PlexVFS(self.plex, self, self.options.control_path)
+        return PlexVFS(self.plex, self.options.control_path)
 
     def fsinit(self):
         # "cache_path" property doesn't get always initialized from options:
         # https://github.com/libfuse/python-fuse/issues/61#issuecomment-1902472620
         cache_path = self.options.cache_path if self.options.cache_path else PlexApi.CACHE_PATH
         PlexApi.CACHE_PATH = Path(cache_path).absolute()
         PlexApi.HTTP_CACHE = self.options.http_cache
         print(f"fsinit: CACHE_PATH={PlexApi.CACHE_PATH}")
         print(f"fsinit: HTTP_CACHE={PlexApi.HTTP_CACHE}")
         print(f"fsinit: control_path={self.options.control_path}")
         print(f"fsinit: listen_events={self.options.listen_events}")
         if self.options.control_path:
-            self.control = ControlListener(self.options.control_path, self.vfs.control).start()
+            control = Control(self.plex, self, self.vfs)
+            self.control = ControlListener(self.options.control_path, control).start()
         if self.options.listen_events:
             self.monitor = Monitor(self.plex).start()
 
     def fsdestroy(self):
         if self.control:
             self.control.stop()
```

### Comparing `plex-fuse-0.6.0/plexfuse/fs/RefCountedDict.py` & `plex_fuse-0.7.0/plexfuse/fs/RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/fs/main.py` & `plex_fuse-0.7.0/plexfuse/fs/main.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/plex/Monitor.py` & `plex_fuse-0.7.0/plexfuse/plex/Monitor.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/plex/PlexApi.py` & `plex_fuse-0.7.0/plexfuse/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/ChunkedFile.py` & `plex_fuse-0.7.0/plexfuse/vfs/ChunkedFile.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/Playable.py` & `plex_fuse-0.7.0/plexfuse/vfs/Playable.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/PlexVFS.py` & `plex_fuse-0.7.0/plexfuse/vfs/PlexVFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 from collections import UserDict
 from typing import TYPE_CHECKING
 
+from plexfuse.control.ControlVFS import ControlVFS
 from plexfuse.vfs.ChunkedFile import ChunkedFile
-from plexfuse.vfs.Control import Control
 from plexfuse.vfs.entry.DirEntry import DirEntry
 from plexfuse.vfs.entry.FileEntry import FileEntry
 from plexfuse.vfs.entry.PlexMatchEntry import PlexMatchEntry
 from plexfuse.vfs.entry.SubtitleEntry import SubtitleEntry
 
 if TYPE_CHECKING:
-    from plexfuse.fs.PlexFS import PlexFS
     from plexfuse.plex.PlexApi import PlexApi
 
 
 class PlexVFS(UserDict):
     SUBTITLE_EXT = (".srt", ".vtt")
 
-    def __init__(self, plex: PlexApi, plexfs: PlexFS, control_path: str = None):
+    def __init__(self, plex: PlexApi, control_path: str = None):
         super().__init__()
         self.plex = plex
         self.reader = ChunkedFile(plex)
-        self.control = Control(plex, plexfs, self, control_path)
+        self.control = ControlVFS(control_path)
 
     def __missing__(self, path: str):
         entry = self.resolve(path)
         if entry is None:
             raise KeyError(path)
 
         self[path] = entry
```

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/entry/FileEntry.py` & `plex_fuse-0.7.0/plexfuse/vfs/entry/FileEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/entry/LibraryEntry.py` & `plex_fuse-0.7.0/plexfuse/vfs/entry/LibraryEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/entry/PlexMatchEntry.py` & `plex_fuse-0.7.0/plexfuse/vfs/entry/PlexMatchEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/entry/SectionEntry.py` & `plex_fuse-0.7.0/plexfuse/vfs/entry/SectionEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/plexfuse/vfs/entry/SubtitleEntry.py` & `plex_fuse-0.7.0/plexfuse/vfs/entry/SubtitleEntry.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/pyproject.toml` & `plex_fuse-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/tests/test_RefCountedDict.py` & `plex_fuse-0.7.0/tests/test_RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/tests/test_chunk_calc.py` & `plex_fuse-0.7.0/tests/test_chunk_calc.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/tests/test_chunk_read.py` & `plex_fuse-0.7.0/tests/test_chunk_read.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/tests/test_file_copy_partial.py` & `plex_fuse-0.7.0/tests/test_file_copy_partial.py`

 * *Files identical despite different names*

### Comparing `plex-fuse-0.6.0/tests/test_socket_control.py` & `plex_fuse-0.7.0/tests/test_socket_control.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from time import sleep
 
+from plexfuse.control.Control import Control
 from plexfuse.control.ControlListener import ControlListener
 from plexfuse.fs.PlexFS import PlexFS
 from plexfuse.plex.PlexApi import PlexApi
-from plexfuse.vfs.Control import Control
 from plexfuse.vfs.PlexVFS import PlexVFS
 
 
 def test_socket_control():
     p = PlexApi()
     fs = PlexFS()
     vfs = PlexVFS(p, fs)
```

