# Comparing `tmp/cobib-4.5.0.tar.gz` & `tmp/cobib-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-4.5.0.tar", last modified: Sun Mar 17 15:42:24 2024, max compression
+gzip compressed data, was "cobib-5.0.0.tar", last modified: Sun Apr 28 12:09:56 2024, max compression
```

## Comparing `cobib-4.5.0.tar` & `cobib-5.0.0.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.412373 cobib-4.5.0/
--rw-r--r--   0 max       (1000) max       (1000)    40390 2024-03-17 15:41:03.000000 cobib-4.5.0/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-4.5.0/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-4.5.0/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)    49657 2024-03-17 15:42:24.412373 cobib-4.5.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     7835 2024-03-03 19:36:55.000000 cobib-4.5.0/README.md
--rw-r--r--   0 max       (1000) max       (1000)    36069 2024-03-17 15:41:24.000000 cobib-4.5.0/cobib.1
--rw-r--r--   0 max       (1000) max       (1000)     2915 2024-03-03 19:36:55.000000 cobib-4.5.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-4.5.0/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-03-17 15:42:24.412373 cobib-4.5.0/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.389040 cobib-4.5.0/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.395707 cobib-4.5.0/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2024-03-17 15:41:15.000000 cobib-4.5.0/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      648 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.399040 cobib-4.5.0/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)      996 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    20578 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     8652 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     4857 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     8923 2024-02-03 16:57:42.000000 cobib-4.5.0/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     7688 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     3144 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/git.py
--rw-r--r--   0 max       (1000) max       (1000)     7489 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4772 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)    14711 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/commands/list_.py
--rw-r--r--   0 max       (1000) max       (1000)    21356 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)    10533 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     4802 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)    19667 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/review.py
--rw-r--r--   0 max       (1000) max       (1000)    11729 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     2411 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     5499 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/commands/undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.399040 cobib-4.5.0/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-4.5.0/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    38956 2024-01-22 06:23:25.000000 cobib-4.5.0/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)    11469 2023-12-12 08:31:55.000000 cobib-4.5.0/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.402373 cobib-4.5.0/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-4.5.0/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4135 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/database/author.py
--rw-r--r--   0 max       (1000) max       (1000)    16846 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    24383 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.402373 cobib-4.5.0/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3115 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    12844 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.402373 cobib-4.5.0/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5224 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-4.5.0/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.405707 cobib-4.5.0/src/cobib/ui/
--rw-r--r--   0 max       (1000) max       (1000)      611 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/ui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4322 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/ui/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.409040 cobib-4.5.0/src/cobib/ui/components/
--rw-r--r--   0 max       (1000) max       (1000)     1105 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/ui/components/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1471 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/ui/components/argument_parser.py
--rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/ui/components/entry_view.py
--rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/ui/components/help_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/ui/components/input_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/ui/components/list_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-4.5.0/src/cobib/ui/components/log_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/ui/components/logging_handler.py
--rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-4.5.0/src/cobib/ui/components/main_content.py
--rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/ui/components/motion_key.py
--rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/ui/components/preset_filter_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/ui/components/search_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/ui/components/selection_filter.py
--rw-r--r--   0 max       (1000) max       (1000)     1842 2024-03-17 15:35:47.000000 cobib-4.5.0/src/cobib/ui/shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)    20862 2024-02-03 17:15:14.000000 cobib-4.5.0/src/cobib/ui/tui.py
--rw-r--r--   0 max       (1000) max       (1000)     4303 2023-08-26 11:05:01.000000 cobib-4.5.0/src/cobib/ui/ui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.412373 cobib-4.5.0/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/utils/context.py
--rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-4.5.0/src/cobib/utils/diff_renderer.py
--rw-r--r--   0 max       (1000) max       (1000)     7469 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-4.5.0/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/utils/progress.py
--rw-r--r--   0 max       (1000) max       (1000)     8994 2024-01-21 19:11:03.000000 cobib-4.5.0/src/cobib/utils/prompt.py
--rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-4.5.0/src/cobib/utils/rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)     8892 2024-03-17 15:35:41.000000 cobib-4.5.0/src/cobib/utils/shell_helper.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.412373 cobib-4.5.0/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    49657 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2340 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       47 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)      135 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2024-03-17 15:42:24.000000 cobib-4.5.0/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-03-17 15:42:24.412373 cobib-4.5.0/tests/
--rw-r--r--   0 max       (1000) max       (1000)     4300 2024-03-03 19:36:49.000000 cobib-4.5.0/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.750714 cobib-5.0.0/
+-rw-r--r--   0 max       (1000) max       (1000)    41947 2024-04-28 12:08:28.000000 cobib-5.0.0/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-01-18 21:03:08.000000 cobib-5.0.0/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-5.0.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)    51364 2024-04-28 12:09:56.750714 cobib-5.0.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     8035 2024-03-17 16:27:49.000000 cobib-5.0.0/README.md
+-rw-r--r--   0 max       (1000) max       (1000)    35143 2024-04-28 12:07:47.000000 cobib-5.0.0/cobib.1
+-rw-r--r--   0 max       (1000) max       (1000)     4580 2024-04-28 11:19:47.000000 cobib-5.0.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)      135 2024-02-03 16:58:09.000000 cobib-5.0.0/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-28 12:09:56.750714 cobib-5.0.0/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.724048 cobib-5.0.0/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.730714 cobib-5.0.0/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2024-04-28 12:07:29.000000 cobib-5.0.0/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      445 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.737381 cobib-5.0.0/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)     1108 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    23338 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7015 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     4633 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     8699 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7477 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     3179 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/git.py
+-rw-r--r--   0 max       (1000) max       (1000)     7264 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4548 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)     4607 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/lint.py
+-rw-r--r--   0 max       (1000) max       (1000)    14510 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    21161 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    10356 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4578 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)    19498 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/review.py
+-rw-r--r--   0 max       (1000) max       (1000)    11513 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2211 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5275 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/undo.py
+-rw-r--r--   0 max       (1000) max       (1000)     2578 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/commands/unify_labels.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1302 2023-11-12 10:49:04.000000 cobib-5.0.0/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1521 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/config/command.py
+-rw-r--r--   0 max       (1000) max       (1000)    42596 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    31459 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)    11469 2023-12-12 08:31:55.000000 cobib-5.0.0/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)     1413 2023-11-13 21:18:22.000000 cobib-5.0.0/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4164 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/database/author.py
+-rw-r--r--   0 max       (1000) max       (1000)    18110 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    24383 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.740714 cobib-5.0.0/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3051 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12895 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.744047 cobib-5.0.0/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5317 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2034 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     3522 2023-11-12 10:49:04.000000 cobib-5.0.0/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3815 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4731 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3593 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3852 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.744047 cobib-5.0.0/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      236 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4094 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)     1043 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1911 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/components/entry_points.py
+-rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     3287 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/help_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2566 2024-01-14 16:13:13.000000 cobib-5.0.0/src/cobib/ui/components/input_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     4649 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/list_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1564 2024-01-14 16:13:13.000000 cobib-5.0.0/src/cobib/ui/components/log_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2257 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/ui/components/logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)     2891 2023-12-11 20:47:52.000000 cobib-5.0.0/src/cobib/ui/components/main_content.py
+-rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/ui/components/motion_key.py
+-rw-r--r--   0 max       (1000) max       (1000)     2731 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/preset_filter_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     3908 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/search_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1373 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)    21173 2024-03-17 16:27:49.000000 cobib-5.0.0/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4311 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      460 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/utils/context.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-5.0.0/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     7574 2024-04-28 11:21:44.000000 cobib-5.0.0/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4615 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     4776 2023-12-17 17:15:09.000000 cobib-5.0.0/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     2998 2024-01-21 19:11:03.000000 cobib-5.0.0/src/cobib/utils/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     9017 2024-04-28 11:19:47.000000 cobib-5.0.0/src/cobib/utils/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)     1860 2023-08-27 11:42:15.000000 cobib-5.0.0/src/cobib/utils/rel_path.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.750714 cobib-5.0.0/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    51364 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2366 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1151 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      135 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2024-04-28 12:09:56.000000 cobib-5.0.0/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-28 12:09:56.747381 cobib-5.0.0/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     4314 2024-04-28 11:19:47.000000 cobib-5.0.0/tests/test_main.py
```

### Comparing `cobib-4.5.0/CHANGELOG.md` & `cobib-5.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,48 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.0] - 2024-04-28
+
+Pypi: https://pypi.org/project/cobib/5.0.0/
+
+### Added
+
+- the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
+  - (DEV) a dummy plugin show-casing these extensions
+
+### Changed
+- the entire `shell_helper` module has been replaced as follows (!139):
+  - the following deprecated helper methods were removed without replacement:
+    - `_list_commands`
+    - `_list_filters`
+    - `_list_labels`
+  - the following secondary commands have been refactored:
+    - `_lint_database` is now `cobib.commands.lint.LintCommand`
+    - `_unify_labels` is now `cobib.commands.unify_labels.UnifyLabelsCommand`
+    - `_example_config` is now `cobib.config.command.ExampleConfigCommand`
+- the interactive disambiguation mechanism during the `add` command now handles
+  multiple matching related entries (#121,!168)
+  - this includes the ability to `cancel` the disambiguation and entry addition
+
+### Removed
+
+- the previously deprecated `console` attribute of all commands has been removed (!139)
+- the previously deprecated `prompt` attribute of all commands has been removed (!139)
+- the `cobib.ui.shell_helper` and `cobib.utils.shell_helper` modules have been removed (!139)
+- the previously deprecated `--update` argument of the `add` command (!168)
+- the previously deprecated `--skip-existing` argument of the `add` command (!168)
+- the previously deprecated `LabelSuffix.CAPTIAL` attribute (!168)
+- Python 3.8 is no longer supported (!173)
+
+
 ## [4.5.0] - 2024-03-17
 
 Pypi: https://pypi.org/project/cobib/4.5.0/
 
 ### Added
 - the new `cobib.utils.context.get_active_app` method which returns any running
   textual App and replaces the need for the `cobib.utils.prompt.Prompt.console`
@@ -954,15 +988,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.5.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/tags/v4.0.0
```

### Comparing `cobib-4.5.0/LICENSE.txt` & `cobib-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/PKG-INFO` & `cobib-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.5.0
+Version: 5.0.0
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Changelog, https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md
 Keywords: reference-manager,citation-manager,bibliography,cli,tui,command-line,terminal,console,bibtex,doi,arxiv,isbn
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: bibtexparser
 Requires-Dist: lxml
 Requires-Dist: pylatexenc
 Requires-Dist: requests
@@ -255,14 +254,21 @@
 
 You may also specify a different config file at runtime by using the `-c` or `--config` command line argument or by specifying a custom path in the `COBIB_CONFIG` environment variable.
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
+## Plugins
+
+coBib supports the implementation of plugins!
+You can find an example plugin in [this folder](./plugin) or read the docs of
+`cobib_dummy` (when viewing the hosted documentation online).
+
+
 ## Documentation
 
 coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
@@ -301,14 +307,48 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.0] - 2024-04-28
+
+Pypi: https://pypi.org/project/cobib/5.0.0/
+
+### Added
+
+- the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
+  - (DEV) a dummy plugin show-casing these extensions
+
+### Changed
+- the entire `shell_helper` module has been replaced as follows (!139):
+  - the following deprecated helper methods were removed without replacement:
+    - `_list_commands`
+    - `_list_filters`
+    - `_list_labels`
+  - the following secondary commands have been refactored:
+    - `_lint_database` is now `cobib.commands.lint.LintCommand`
+    - `_unify_labels` is now `cobib.commands.unify_labels.UnifyLabelsCommand`
+    - `_example_config` is now `cobib.config.command.ExampleConfigCommand`
+- the interactive disambiguation mechanism during the `add` command now handles
+  multiple matching related entries (#121,!168)
+  - this includes the ability to `cancel` the disambiguation and entry addition
+
+### Removed
+
+- the previously deprecated `console` attribute of all commands has been removed (!139)
+- the previously deprecated `prompt` attribute of all commands has been removed (!139)
+- the `cobib.ui.shell_helper` and `cobib.utils.shell_helper` modules have been removed (!139)
+- the previously deprecated `--update` argument of the `add` command (!168)
+- the previously deprecated `--skip-existing` argument of the `add` command (!168)
+- the previously deprecated `LabelSuffix.CAPTIAL` attribute (!168)
+- Python 3.8 is no longer supported (!173)
+
+
 ## [4.5.0] - 2024-03-17
 
 Pypi: https://pypi.org/project/cobib/4.5.0/
 
 ### Added
 - the new `cobib.utils.context.get_active_app` method which returns any running
   textual App and replaces the need for the `cobib.utils.prompt.Prompt.console`
@@ -1252,15 +1292,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.5.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/tags/v4.0.0
```

### Comparing `cobib-4.5.0/README.md` & `cobib-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,21 @@
 
 You may also specify a different config file at runtime by using the `-c` or `--config` command line argument or by specifying a custom path in the `COBIB_CONFIG` environment variable.
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
+## Plugins
+
+coBib supports the implementation of plugins!
+You can find an example plugin in [this folder](./plugin) or read the docs of
+`cobib_dummy` (when viewing the hosted documentation online).
+
+
 ## Documentation
 
 coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
```

### Comparing `cobib-4.5.0/cobib.1` & `cobib-5.0.0/cobib.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2024-03-17 v4.5.0
+.TH COBIB 1 2024-04-28 v5.0.0
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
@@ -524,14 +524,32 @@
 Provide a custom Zotero user ID. If this is a publicly accessible library, no
 API key is required. Otherwise you must also use the following argument.
 .PP
 .in +12n
 .BR \-\-api-key " "\fI<API\ key>\fR
 .in +8n
 Provide a custom Zotero API key.
+.TP
+.B cobib lint
+Lints the database file for potential points of formatting improvements.
+.PP
+.in +8n
+.BR \-f ", " \-\-format
+.in +4n
+If you provide this option, coBib will automatically format your database to
+resolve all found lint messages.
+.TP
+.B cobib unify_labels
+Updates all entry labels in your database to follow the default naming pattern.
+.PP
+.in +8n
+.BR \-a ", " \-\-apply
+.in +4n
+If you provide this option, coBib will actually apply the updates rather than
+preview them in dry-mode.
 .SH FILTERS
 In order to limit the output of the \fIlist\fR, \fImodify\fR, \fIsearch\fR, and
 \fIexport\fR commands you can apply additional filters via keyword arguments.
 Their availability depends on your database since they are added to the argument
 parser at runtime.
 However, you can find a full list for your specific case with \fIcobib list
 \-\-help\fR.
@@ -651,15 +669,15 @@
 Opens a small window providing help for the key bindings.
 .SH CONFIGURATION
 Since version 3.0, coBib can be configured directly via \fIPython\fR. To do so,
 you must place the configuration file at \fI$HOME/.config/cobib/config.py\fR.
 If you don't have a configuration file yet, you can get started by copying the
 well-documented example configuration to the right location via:
 .in +4n
-    \fIcobib _example_config > ~/.config/cobib/config.py\fR
+    \fIcobib example_config > ~/.config/cobib/config.py\fR
 .in -4n
 If you do have an old configuration file (prior to v3.0) and would like some
 guidance on how to migrate it, please read this short blog post of mine:
 https://mrossinek.gitlab.io/programming/cobibs-new-configuration/
 .PP
 Since v3.5, coBib also respects the \fICOBIB_CONFIG\fR environment variable.
 With this you can either specify a custom path to your configuration file or
@@ -920,60 +938,14 @@
 .BR EVENTS
 .TP
 Since v3.3.0 coBib comes with a number of subscribable events. Their
 configuration is detailed in the online documentation,
 https://cobib.gitlab.io/cobib/cobib/config/event.html, and will not be
 repeated here.
 .PP
-.SH SHELL UTILITIES
-In addition to the \fISUBCOMMANDS\fR coBib also provides some "meta"-commands
-for varying purposes.
-.TP
-.B cobib _example_config
-Prints the example configuration.
-This is \fIDEPRECATED\fR and will be available as \fIexample_config\fR starting
-from coBib v5.0
-You can do the following to get started with a custom configuration:
-.in +4n
-    \fIcobib _example_config > ~/.config/cobib/config.py\fR
-.TP
-.B cobib _lint_database
-Lints the database file for potential points of formatting improvements.
-This is \fIDEPRECATED\fR and will be available as \fIlint\fR starting from
-coBib v5.0
-.PP
-.in +8n
-.BR \-f ", " \-\-format
-.in +4n
-If you provide this option, coBib will automatically format your database to
-resolve all found lint messages.
-.TP
-.B cobib _unify_labels
-Updates all entry labels in your database to follow the default naming pattern.
-This is \fIDEPRECATED\fR and will be available as \fIlint\fR starting from
-coBib v5.0
-.PP
-.in +8n
-.BR \-a ", " \-\-apply
-.in +4n
-If you provide this option, coBib will actually apply the updates rather than
-preview them in dry-mode.
-.TP
-.B cobib _list_commands
-Lists all available \fISUBCOMMANDS\fR.
-This is \fIDEPRECATED\fR without replacement.
-.TP
-.B cobib _list_labels
-Lists all labels in your database.
-This is \fIDEPRECATED\fR without replacement.
-.TP
-.B cobib _list_filters
-Lists all available filters.
-This is \fIDEPRECATED\fR without replacement.
-.PP
 .SH ENVIRONMENT
 .TP
 .IR $EDITOR
 Specifies the editor program to use for the \fBedit\fR command.
 .SH FILES
 .TP
 .IR $HOME/.config/cobib/config.ini
```

### Comparing `cobib-4.5.0/src/cobib/commands/__init__.py` & `cobib-5.0.0/src/cobib/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from .add import AddCommand as AddCommand
 from .delete import DeleteCommand as DeleteCommand
 from .edit import EditCommand as EditCommand
 from .export import ExportCommand as ExportCommand
 from .git import GitCommand as GitCommand
 from .import_ import ImportCommand as ImportCommand
 from .init import InitCommand as InitCommand
+from .lint import LintCommand as LintCommand
 from .list_ import ListCommand as ListCommand
 from .modify import ModifyCommand as ModifyCommand
 from .open import OpenCommand as OpenCommand
 from .redo import RedoCommand as RedoCommand
 from .review import ReviewCommand as ReviewCommand
 from .search import SearchCommand as SearchCommand
 from .show import ShowCommand as ShowCommand
 from .undo import UndoCommand as UndoCommand
+from .unify_labels import UnifyLabelsCommand as UnifyLabelsCommand
```

### Comparing `cobib-4.5.0/src/cobib/commands/add.py` & `cobib-5.0.0/src/cobib/commands/add.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,89 +82,105 @@
 cobib add --skip-download --arxiv <some arXiv ID>
 ```
 While the next command will always attempt the automatic download:
 ```
 cobib add --force-download --arxiv <some arXiv ID>
 ```
 
+#### Label Disambiguation
+
 Since v4.0.0 coBib will ask you what to do when encountering a conflict at runtime. That means, when
 a label already exists in your database, you have various choices how to handle it:
 
 1. you can `keep` the existing entry and skip the addition of the new one.
    .. note::
-      This is equivalent to the old `--skip-existing` argument (added in v3.3.0) which is now
-      deprecated and will be removed in a future version.
+      This is equivalent to the old `--skip-existing` argument (added in v3.3.0; deprecated in
+      v4.0.0; removed in v5.0.0).
 
 2. you can `replace` the existing entry.
 
 3. you can `update` the existing entry.
-   ```
-   cobib add --doi <some DOI> --disambiguation update --label <some existing label>```
 
    This will take the existing entry and combine it with all new information found in the freshly
    added entry. Existing fields will be overwritten. If you have an automatically downloaded file
    associated with this entry, that will also be overwritten.
    This feature is especially useful if you want to update an entry which you previously added from
    the arXiv with its newly published version.
    .. note::
-      This is equivalent to the `--update` argument (added in v3.3.0) which is now deprecated and
-      will be removed in a future version.
+      This is equivalent to the `--update` argument (added in v3.3.0; deprecated in v4.0.0; removed
+      in v5.0.0).
 
 4. you can `disambiguate` the entries. This will be done based on the
    `cobib.config.config.DatabaseFormatConfig.label_suffix` setting. It defaults to appending `_a`,
    `_b`, etc. to the label in order to differentiate (disambiguate) it from the already existing
    one.
 
 When running into such a case, coBib will generate a side-by-side comparison of the existing and new
-entry and give you the choice of how to proceed. The default choice is to *cancel* the addition
-(i.e. `keep`) in order to prevent data loss.
+entry and give you the choice of how to proceed. The default choice is to `keep` the existing entry
+in order to prevent data loss.
+
+Since v5.0.0 coBib also handles multiple existing entries that are related to the new one via their
+disambiguation suffix. This means, that the interactive prompt above will loop over all existing
+entries and ask you how to handle them.
+- Answering with `update` or `replace` will immediately apply to the currently compared entry and
+  end the iteration.
+- Answering `keep` will leave the current entry unchanged and proceed to the next.
+- Answering `cancel` will immediately stop the iteration and abort the process of adding this new
+  entry.
+- Answering `disambiguate` will immdetiately stop the iteration and add this new entry under a newly
+  disambiguated label.
+
+.. note::
+   If you `keep` all existing entries, this will automatically trigger the `disambiguate` mode for
+   adding the new entry.
 
 If you already know that you will run into this case, you can bypass the prompt via the
 `--disambiguation` argument and provide the intended answer ahead of time, for example like so:
 ```
 cobib add --doi <some DOI> --disambiguation replace --label <some existing label>
 ```
 
+.. note::
+   If you do this in a scenario where multiple related entries already exist, the provided answer
+   will **ONLY** apply to the exactly matching label.
+
 ### TUI
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `a` key which will drop you into the prompt where you can type out a
 normal command-line command:
 ```
 :add <arguments go here>
 ```
 """
 
 from __future__ import annotations
 
 import argparse
 import asyncio
-import inspect
 import logging
 from collections import OrderedDict
 from collections.abc import Callable
 from functools import wraps
 from typing import ClassVar
 
-from rich.console import Console
 from rich.prompt import InvalidResponse, PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
-from cobib import parsers
-from cobib.config import Event, config
+from cobib.config import Event, LabelSuffix, config
 from cobib.database import Database, Entry
 from cobib.parsers import BibtexParser
 from cobib.parsers.base_parser import Parser
+from cobib.ui.components.entry_points import entry_points
 from cobib.utils.diff_renderer import Differ
 from cobib.utils.file_downloader import FileDownloader
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 from cobib.utils.prompt import Prompt
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 from .edit import EditCommand
 from .modify import evaluate_as_f_string
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
@@ -178,47 +194,45 @@
           occur.
         * `-f`, `--file`: one or multiple files to associate with this entry. This data will be
           stored in the `cobib.database.Entry.file` property.
         * `-p`, `--path`: the path to store the downloaded associated file in. This can be used to
           overwrite the `cobib.config.config.FileDownloaderConfig.default_location`.
         * `--skip-download`: skips the automatic download of an associated file.
         * `--force-download`: forces the automatic download of an associated file.
-        * `--skip-existing`: **DEPRECATED** use `--disambiguation keep` instead!
-        * `-u`, `--update`: **DEPRECATED** use `--disambiguation update` instead!
         * in addition to the options above, a *mutually exclusive group* of keyword arguments for
           all available `cobib.parsers` are registered at runtime. Please check the output of
           `cobib add --help` for the exact list.
         * any *positional* arguments (i.e. those, not preceded by a keyword) are interpreted as tags
           and will be stored in the `cobib.database.Entry.tags` property.
     """
 
     name = "add"
 
-    _avail_parsers: ClassVar[dict[str, Callable[[], Parser]]] = {
-        cls.name: cls for _, cls in inspect.getmembers(parsers) if inspect.isclass(cls)
+    _avail_parsers: ClassVar[dict[str, tuple[Callable[[], Parser], bool]]] = {
+        cls.name: (cls.load(), builtin) for (cls, builtin) in entry_points("cobib.parsers")
     }
-    """The available parsers."""
+    """The available parsers. The values are a tuple of the parser `entry_point` and a boolean
+    indicating whether it is built-in (`True`) or from an external source (`False`). In the former
+    case, the parser will attempt to provide a short-hand argument option, for example `-b` for
+    `--bibtex`."""
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.new_entries: dict[str, Entry] = OrderedDict()
         """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were added by
         this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="add", description="Add subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="add", description="Add subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("-l", "--label", type=str, help="the label for the new database entry")
         parser.add_argument(
             "-f",
             "--file",
             type=str,
             nargs="+",
             action="extend",
@@ -241,75 +255,45 @@
         skip_download_group.add_argument(
             "--force-download",
             dest="skip_download",
             action="store_false",
             default=None,
             help="force the automatic download of an associated file",
         )
-        parser.add_argument(
-            "--skip-existing",
-            action="store_true",
-            help="DEPRECATED: use '--disambiguation keep' instead!",
-        )
-        parser.add_argument(
-            "-u",
-            "--update",
-            action="store_true",
-            help="DEPRECATED: use '--disambiguation update' instead!",
-        )
         group_add = parser.add_mutually_exclusive_group()
-        for name in cls._avail_parsers.keys():
-            try:
-                group_add.add_argument(
-                    f"-{name[0]}", f"--{name}", type=str, help=f"{name} object identifier"
-                )
-            except argparse.ArgumentError:
+        for name, (_, short_hand) in cls._avail_parsers.items():
+            help_text = f"{name} object identifier"
+            if short_hand:
                 try:
-                    group_add.add_argument(f"--{name}", type=str, help=f"{name} object identifier")
-                except argparse.ArgumentError:
+                    group_add.add_argument(f"-{name[0]}", f"--{name}", type=str, help=help_text)
                     continue
+                except argparse.ArgumentError:
+                    pass
+            try:
+                group_add.add_argument(f"--{name}", type=str, help=help_text)
+            except argparse.ArgumentError:
+                LOGGER.error(f"Could not setup the {name} parser argument for the add command.")
+
         parser.add_argument(
             "tags",
             nargs=argparse.REMAINDER,
             help="A list of space-separated tags to associate with this entry."
             "\nYou can use quotes to specify tags with spaces in them.",
         )
 
         cls.argparser = parser
 
-    @classmethod
-    def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
-        largs = super()._parse_args(args)
-
-        if largs.skip_existing:
-            msg = (
-                "The '--skip-existing' argument of the 'add' command is deprecated! "
-                "Instead you should use '--disambiguation keep'."
-            )
-            LOGGER.warning(msg)
-            largs.disambiguation = "keep"
-
-        if largs.update:
-            msg = (
-                "The '--update' argument of the 'add' command is deprecated! "
-                "Instead you should use '--disambiguation update'."
-            )
-            LOGGER.warning(msg)
-            largs.disambiguation = "update"
-
-        return largs
-
     @override
-    async def execute(self) -> None:  # type: ignore[override]  # noqa: PLR0912
+    async def execute(self) -> None:  # type: ignore[override]  # noqa: PLR0912,PLR0915
         LOGGER.debug("Starting Add command.")
 
         Event.PreAddCommand.fire(self)
 
         edit_entries = False
-        for name, cls in AddCommand._avail_parsers.items():
+        for name, (cls, _) in AddCommand._avail_parsers.items():
             string = getattr(self.largs, name, None)
             if string is None:
                 continue
             LOGGER.debug("Adding entries from %s: '%s'.", name, string)
             self.new_entries = cls().parse(string)
             break
         else:
@@ -381,60 +365,113 @@
                     )
                     LOGGER.warning(msg)
                     continue
                 # in all other cases, we enter an interactive prompt to let the user decide how
                 # to proceed
                 msg = f"You tried to add a new entry '{lbl}' which already exists!"
                 LOGGER.warning(msg)
-                res = self.largs.disambiguation
-                # if the user provided the reply at runtime using the --disambiguation argument, the
-                # following condition is not met
-                if res is None:
-                    parser = BibtexParser()
-                    left = parser.dump(bib[lbl])
-                    right = parser.dump(entry)
-                    diff = Differ(left, right)
-                    diff.compute()
-                    table = diff.render("bibtex")
-
-                    prompt_text = "How would you like to handle this conflict?"
-                    choices = ["keep", "replace", "update", "disambiguate", "help"]
-                    default = "keep"
-
-                    res = await Prompt.ask(
-                        prompt_text,
-                        choices=choices,
-                        default=default,
-                        pre_prompt_message=table,
-                        process_response_wrapper=self._wrap_prompt_process_response,
+
+                # finding related entries in the database
+                direct, indirect = bib.find_related_labels(lbl)
+                if len(indirect) > 0:
+                    separator, enumerator = config.database.format.label_suffix
+                    trimmed_lbl, _ = LabelSuffix.trim_label(lbl, separator, enumerator)
+                    msg = (
+                        f"Found some indirectly related entries to '{lbl}': {indirect}.\n"
+                        "You can use the review command to inspect these like so:\n"
+                        f"cobib review -- ++label {trimmed_lbl}"
                     )
+                    LOGGER.warning(msg)
+
+                # get the --disambiguation argument (which will be `None` by default)
+                res = self.largs.disambiguation
+
+                parser = BibtexParser()
 
-                if res == "update":
-                    msg = f"Updating the already existing entry '{lbl}' with the new data."
-                    LOGGER.info(msg)
-                    entry.merge(bib[lbl], ours=True)
-                    overwrite_file = True
-                elif res == "disambiguate":
+                # the first label that we would like to check is the current one
+                direct_lbl = lbl
+                direct.remove(lbl)
+                # the remaining ones will be iterated later
+                direct_iter = iter(direct)
+
+                # we loop until we reach the `disambiguate` answer (which implies the end) or we
+                # break out manually below
+                while res != "disambiguate":
+                    if res is None:
+                        # if the user did not provide an answer via the input arguments, this
+                        # renders an interactive prompt for them
+                        left = parser.dump(bib[direct_lbl])
+                        right = parser.dump(entry)
+                        diff = Differ(left, right)
+                        diff.compute()
+                        table = diff.render("bibtex")
+
+                        prompt_text = "How would you like to handle this conflict?"
+                        choices = ["keep", "replace", "update", "cancel", "disambiguate", "help"]
+                        default = "keep"
+
+                        res = await Prompt.ask(
+                            prompt_text,
+                            choices=choices,
+                            default=default,
+                            pre_prompt_message=table,
+                            process_response_wrapper=self._wrap_prompt_process_response,
+                        )
+
+                    if res == "update":
+                        msg = (
+                            f"Updating the already existing entry '{direct_lbl}' with the new data."
+                        )
+                        LOGGER.info(msg)
+                        entry.merge(bib[direct_lbl], ours=True)
+                        self._rename_added_entry(entry, direct_lbl)
+                        overwrite_file = True
+                        break
+
+                    elif res == "replace":
+                        msg = (
+                            f"Overwriting the already existing entry '{direct_lbl}' with the new "
+                            "data."
+                        )
+                        LOGGER.info(msg)
+                        self._rename_added_entry(entry, direct_lbl)
+                        overwrite_file = True
+                        break
+
+                    elif res == "disambiguate":
+                        msg = "Skipping all other related entries and disambiguating the new one."
+                        LOGGER.info(msg)
+                        break
+
+                    elif res == "keep":
+                        res = None
+                        msg = f"Keeping the already existing entry '{direct_lbl}'."
+                        LOGGER.info(msg)
+
+                    elif res == "cancel":  # pragma: no branch
+                        msg = f"Cancelling the addition of the new entry '{lbl}'."
+                        LOGGER.warning(msg)
+                        return
+
+                    try:
+                        direct_lbl = next(direct_iter)
+                    except StopIteration:
+                        res = "disambiguate"
+                        msg = "No more related entries, triggering label disambiguation."
+                        LOGGER.info(msg)
+                        break
+
+                if res == "disambiguate":
                     msg = (
                         "The label will be disambiguated based on the configuration option: "
                         "config.database.format.label_suffix"
                     )
                     LOGGER.warning(msg)
                     new_label = bib.disambiguate_label(lbl, entry)
-                    entry.label = new_label
-                    self.new_entries[new_label] = entry
-                    self.new_entries.pop(lbl)
-                elif res == "replace":
-                    msg = f"Overwriting the already existing entry '{lbl}' with the new data."
-                    LOGGER.info(msg)
-                elif res == "keep":
-                    msg = f"Skipping addition of the already existing entry '{lbl}'."
-                    LOGGER.info(msg)
-                    self.new_entries.pop(lbl)
-                    continue
+                    self._rename_added_entry(entry, new_label)
 
             # download associated file (if requested)
             if "_download" in entry.data.keys():
                 if skip_download:
                     entry.data.pop("_download")
                 else:
                     task = asyncio.create_task(
@@ -462,14 +499,27 @@
 
         self.git()
 
         for label in self.new_entries:
             msg = f"'{label}' was added to the database."
             LOGGER.log(35, msg)
 
+    def _rename_added_entry(self, entry: Entry, new_label: str) -> None:
+        """Renames the provided entry to the new provided label.
+
+        Args:
+            entry: the entry to be renamed.
+            new_label: its new label.
+        """
+        old_label = entry.label
+        if old_label != new_label:
+            entry.label = new_label
+            self.new_entries[new_label] = entry
+            self.new_entries.pop(old_label)
+
     @staticmethod
     def _wrap_prompt_process_response(
         func: Callable[[PromptBase[PromptType], str], PromptType],
     ) -> Callable[[PromptBase[PromptType], str], PromptType]:
         """A method to wrap a `PromptBase.process_response` method.
 
         This method wraps a `PromptBase.process_response` method in order to handle a user's request
@@ -491,13 +541,14 @@
                 LOGGER.debug("User requested help.")
                 raise InvalidResponse(
                     "[yellow]A conflict between an existing (left) and newly added entry (right) "
                     "occurred. These are your options:\n"
                     "  'keep' the existing entry and discard the new addition (default)\n"
                     "  'replace' the existing entry with the new one\n"
                     "  'update' the existing entry with the new data\n"
+                    "  'cancel' the addition of this new entry\n"
                     "  'disambiguate' the new entry from the existing one by adding a label suffix"
                 )
 
             return return_value
 
         return process_response
```

### Comparing `cobib-4.5.0/src/cobib/commands/base_command.py` & `cobib-5.0.0/src/cobib/commands/base_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 import json
 import logging
 import os
 import shlex
 import sys
 from abc import ABC, abstractmethod
 
-from rich.console import Console, ConsoleRenderable
-from rich.prompt import Prompt, PromptBase, PromptType
-from textual.app import App
+from rich.console import ConsoleRenderable
 from textual.widget import Widget
 
 from cobib.config import Event, config
-from cobib.ui.components import ArgumentParser as ArgumentParser  # noqa: PLC0414
 from cobib.utils.rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class Command(ABC):
@@ -29,72 +26,43 @@
     This interface should be implemented by all concrete command implementations.
     """
 
     name = "base"
     """The commands `name` is used to extract the available commands for the command-line interface.
     """
 
-    argparser: ArgumentParser
+    argparser: argparse.ArgumentParser
     """Every command has its own `argparse.ArgumentParser` which is used to parse the arguments
     provided to the command. This is done no matter how the command is executed, whether
     programmatically via Python, from the command-line or any other UI."""
 
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
+    def __init__(self, *args: str) -> None:
         """Initializes a command instance.
 
         Args:
             *args: the sequence of additional command arguments. These will be passed on to the
                 `argparser` of this command for further parsing.
-            console: a command may be in need of printing something for the user during its
-                execution (and before its final result rendering). If so, it should use the `print`
-                method of this console object.
-            prompt: a command may be in need of prompting the user for an input. If so, it will use
-                this prompt kind. It is important that this is respected, as different UIs may
-                inject specific prompt classes to implement different runtime behavior.
         """
         self.args: tuple[str, ...] = args
         """The raw provided command arguments."""
 
         self.largs: argparse.Namespace = self.__class__._parse_args(args)
         """The parsed (local) arguments."""
 
-        if console is not None:
-            LOGGER.log(
-                45,
-                "The `console` argument to all the commands is DEPRECATED since it no longer has "
-                "any effect.",
-            )
-        self.console: Console | App[None] = console if console is not None else Console()
-        """DEPRECATED The object via which to print output to the user during runtime execution."""
-
-        if prompt is not None:
-            LOGGER.log(
-                45,
-                "The `prompt` argument to all the commands is DEPRECATED since it no longer has "
-                "any effect.",
-            )
-        self.prompt: type[PromptBase[PromptType]] = prompt if prompt is not None else Prompt
-        """DEPRECATED The object via which to prompt the user for input during runtime execution."""
-
     @classmethod
     @abstractmethod
     def init_argparser(cls) -> None:
         """Initializes this command's `argparse.ArgumentParser`.
 
         This method needs to be overwritten by every subclass and handles the registration of all
         available command arguments.
         """
 
     @classmethod
-    def _get_argparser(cls) -> ArgumentParser:
+    def _get_argparser(cls) -> argparse.ArgumentParser:
         """Returns this command's `argparse.ArgumentParser`.
 
         The reason for having this method is to handle the parser initialization such that it only
         needs to be done once.
 
         Returns:
             This command's initialized `argparser` object.
```

### Comparing `cobib-4.5.0/src/cobib/commands/delete.py` & `cobib-5.0.0/src/cobib/commands/delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,28 +25,26 @@
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `d` key.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import os
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.prompt import Confirm
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class DeleteCommand(Command):
     """The Delete Command.
@@ -59,29 +57,26 @@
         * `--no-preserve-files`: does NOT skip the deletion of any associated files. This overwrites
           the `cobib.config.config.DeleteCommandConfig.preserve_files` setting.
     """
 
     name = "delete"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.deleted_entries: set[str] = set()
         """A set of labels which were deleted by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="delete", description="Delete subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="delete", description="Delete subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("labels", type=str, nargs="+", help="labels of the entries")
         preserve_files_group = parser.add_mutually_exclusive_group()
         preserve_files_group.add_argument(
             "--preserve-files",
             action="store_true",
             default=None,
             help="do not delete associated files",
```

### Comparing `cobib-4.5.0/src/cobib/commands/edit.py` & `cobib-5.0.0/src/cobib/commands/edit.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,31 +43,29 @@
 ```
 :edit --add <new label>
 ```
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import os
 import tempfile
 from pathlib import Path
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.parsers.yaml import YAMLParser
 from cobib.utils.context import get_active_app
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class EditCommand(Command):
     """The Edit Command.
@@ -85,29 +83,26 @@
           manually rename the entry label during editing. This overwrites the
           `cobib.config.config.EditCommandConfig.preserve_files` setting.
     """
 
     name = "edit"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.new_entry: Entry
         """A `cobib.database.Entry` instance edited by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="edit", description="Edit subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="edit", description="Edit subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("label", type=str, help="label of the entry")
         parser.add_argument(
             "-a",
             "--add",
             action="store_true",
             help="if specified, will add a new entry for unknown labels",
         )
```

### Comparing `cobib-4.5.0/src/cobib/commands/export.py` & `cobib-5.0.0/src/cobib/commands/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,26 +59,23 @@
 
 from __future__ import annotations
 
 import argparse
 import logging
 from zipfile import ZipFile
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Database, Entry
 from cobib.parsers.bibtex import BibtexParser
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ExportCommand(Command):
@@ -98,29 +95,26 @@
         * in addition to the above, you can add `filters` to specify a subset of your
           database for exporting. For more information refer to `cobib.commands.list_`.
     """
 
     name = "export"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.exported_entries: list[Entry] = []
         """A list of `cobib.database.Entry` objects which were exported by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="export", description="Export subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="export", description="Export subcommand parser.", exit_on_error=True
+        )
         parser.add_argument(
             "-b", "--bibtex", type=argparse.FileType("a"), help="BibLaTeX output file"
         )
         parser.add_argument("-z", "--zip", type=argparse.FileType("a"), help="zip output file")
         parser.add_argument(
             "-s",
             "--selection",
@@ -182,15 +176,15 @@
                     )
                 entry_str = bibtex_parser.dump(entry)
                 self.largs.bibtex.write(entry_str)
             if self.largs.zip is not None:
                 if "file" in entry.data.keys() and entry.file is not None:
                     files = entry.file
                     if not isinstance(files, list):
-                        files = [files]
+                        files = [files]  # type: ignore[unreachable]
                     for file in files:
                         path = RelPath(file).path
                         LOGGER.debug(
                             'Adding "%s" associated with "%s" to the zip file.', path, entry.label
                         )
                         self.largs.zip.write(path, path.name)
```

### Comparing `cobib-4.5.0/src/cobib/commands/git.py` & `cobib-5.0.0/src/cobib/commands/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 import subprocess
 
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class GitCommand(Command):
     """The Git Command.
@@ -72,15 +72,17 @@
     """
 
     name = "git"
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="git", description="Git subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="git", description="Git subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("git_args", nargs=argparse.REMAINDER, help="the arguments to git")
         cls.argparser = parser
 
     @override
     @classmethod
     def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
         largs = super()._parse_args(())
```

### Comparing `cobib-4.5.0/src/cobib/commands/import_.py` & `cobib-5.0.0/src/cobib/commands/import_.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,30 +53,26 @@
 :import <arguments go here>
 ```
 """
 
 from __future__ import annotations
 
 import argparse
-import inspect
 import logging
 from collections import OrderedDict
 from typing import Any, Callable, ClassVar
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
-from cobib import importers
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.importers.base_importer import Importer
+from cobib.ui.components.entry_points import entry_points
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ImportCommand(Command):
     """The ImportCommand.
@@ -93,35 +89,32 @@
           `cobib import --zotero -- --help`.
     """
 
     name = "import"
 
     # NOTE: the Callable type is unable to express the complex signature of the Importer class
     _avail_importers: ClassVar[dict[str, Callable[[Any], Importer]]] = {
-        cls.name: cls for _, cls in inspect.getmembers(importers) if inspect.isclass(cls)
+        cls.name: cls.load() for (cls, _) in entry_points("cobib.importers")
     }
     """The available importers."""
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.new_entries: dict[str, Entry] = OrderedDict()
         """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were imported
         by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="import", description="Import subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="import", description="Import subcommand parser.", exit_on_error=True
+        )
         skip_download_group = parser.add_mutually_exclusive_group()
         skip_download_group.add_argument(
             "--skip-download",
             action="store_true",
             default=None,
             help="skip the automatic download of encountered PDF attachments",
         )
@@ -134,15 +127,15 @@
         )
         parser.add_argument(
             "importer_arguments",
             nargs="*",
             help="You can pass additional arguments to the chosen importer. To ensure this works as"
             " expected you should add the pseudo-argument '--' before the remaining arguments.",
         )
-        group_import = parser.add_mutually_exclusive_group()
+        group_import = parser.add_mutually_exclusive_group(required=True)
         for name in cls._avail_importers.keys():
             try:
                 group_import.add_argument(f"--{name}", action="store_true", help=f"{name} importer")
             except argparse.ArgumentError:
                 continue
         cls.argparser = parser
```

### Comparing `cobib-4.5.0/src/cobib/commands/init.py` & `cobib-5.0.0/src/cobib/commands/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,28 +23,26 @@
 .. warning::
    You can**not** run this command from the TUI, because the database must have already been
    initialized *before* you can start the TUI in the first place.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import os
 import sys
 from pathlib import Path
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class InitCommand(Command):
     """The Init Command.
@@ -53,33 +51,30 @@
 
         * `-g`, `--git`: initializes the git-integration.
     """
 
     name = "init"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.file: Path
         """The path to the database file."""
 
         self.root: Path
         """The parent directory where the database file resides. This is where the git repository
         gets initialized (if the git integration was enabled)."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="init", description="Init subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="init", description="Init subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("-g", "--git", action="store_true", help="initialize git repository")
         cls.argparser = parser
 
     @override
     def execute(self) -> None:
         LOGGER.debug("Starting Init command.")
```

### Comparing `cobib-4.5.0/src/cobib/commands/list_.py` & `cobib-5.0.0/src/cobib/commands/list_.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,26 +99,24 @@
 
 import argparse
 import logging
 from collections import defaultdict
 from copy import copy
 from typing import Any
 
-from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase, PromptType
+from rich.console import ConsoleRenderable
 from rich.table import Table
 from rich.text import Text
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.ui.components import ListView
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ListCommand(Command):
     """The List Command.
@@ -146,33 +144,31 @@
           runtime based on the fields available in the database. Please refer that section or the
           output of `cobib list --help` for more information.
     """
 
     name = "list"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.entries: list[Entry] = []
         """A list of entries, filtered and sorted according to the provided command arguments."""
 
         self.columns: list[str] = []
         """A list of (key) columns to be included when rendering the results."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(
-            prog="list", description="List subcommand parser.", prefix_chars="+-"
+        parser = argparse.ArgumentParser(
+            prog="list",
+            description="List subcommand parser.",
+            prefix_chars="+-",
+            exit_on_error=True,
         )
         parser.add_argument("-s", "--sort", help="specify column along which to sort the list")
         parser.add_argument(
             "-r", "--reverse", action="store_true", help="reverses the listing order"
         )
         parser.add_argument("-l", "--limit", type=int, help="limits the number of listed entries")
         ignore_case_group = parser.add_mutually_exclusive_group()
```

### Comparing `cobib-4.5.0/src/cobib/commands/modify.py` & `cobib-5.0.0/src/cobib/commands/modify.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,32 +90,30 @@
 ```
 
 [^1]: <https://docs.python.org/3/reference/lexical_analysis.html#formatted-string-literals>
 """
 
 from __future__ import annotations
 
+import argparse
 import ast
 import logging
 from collections.abc import Callable
 from copy import copy
 from typing import Any
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
 from text_unidecode import unidecode
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.utils.logging import get_stream_handler
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ModifyCommand(Command):
@@ -146,21 +144,16 @@
         * in addition to the above, you can add `filters` to specify a subset of your database for
           exporting. For more information refer to `cobib.commands.list_`.
     """
 
     name = "modify"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.modified_entries: list[Entry] = []
         """A list of `cobib.database.Entry` objects which were modified by this command."""
 
     @staticmethod
     def field_value_pair(string: str) -> tuple[str, str]:
         """Utility method to assert the field-value pair argument type.
@@ -180,15 +173,17 @@
         # NOTE: we split only the first field off in case the value contains f-string format
         # specifications
         return (field, ":".join(value))
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="modify", description="Modify subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="modify", description="Modify subcommand parser.", exit_on_error=True
+        )
         parser.add_argument(
             "modification",
             type=ModifyCommand.field_value_pair,
             help="Modification to apply to the specified entries."
             "\nThis argument must be a string formatted as <field>:<value> where field can be any "
             "field of the entries and value can be any string which should be placed in that "
             "field. Be sure to escape this field-value pair properly, especially if the value "
@@ -439,15 +434,15 @@
     Returns:
         The evaluated AST node expression.
     """
     if locals_ is not None and "unidecode" not in locals_:
         locals_["unidecode"] = unidecode
 
     try:
-        return eval(  # type: ignore
+        return eval(  # type: ignore[no-any-return]
             compile(ast.Expression(node), filename="<string>", mode="eval"), locals_
         )
     except NameError as err:
         LOGGER.warning("You tried use an undefined variable. Falling back to an empty string.")
         LOGGER.error(err)
         return ""
 
@@ -470,15 +465,15 @@
     References:
         <https://stackoverflow.com/a/61190684>
     """
     if locals_ is not None and "unidecode" not in locals_:
         locals_["unidecode"] = unidecode
 
     result: list[str] = []
-    for part in ast.parse(f"f'''{value}'''").body[0].value.values:  # type: ignore
+    for part in ast.parse(f"f'''{value}'''").body[0].value.values:  # type: ignore[attr-defined]
         typ = type(part)
 
         if typ is ast.Constant:
             result.append(part.value)
 
         elif typ is ast.FormattedValue:
             value = evaluate_ast_node(part.value, locals_)
```

### Comparing `cobib-4.5.0/src/cobib/commands/open.py` & `cobib-5.0.0/src/cobib/commands/open.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,35 +45,34 @@
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `o` key.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import os
 import subprocess
 import warnings
 from collections import defaultdict
 from collections.abc import Callable
 from functools import wraps
 from urllib.parse import ParseResult, urlparse
 
-from rich.console import Console
 from rich.prompt import InvalidResponse, PromptBase, PromptType
 from rich.text import Text
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.prompt import Prompt
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class OpenCommand(Command):
     """The Open Command.
@@ -83,29 +82,26 @@
         * `labels`: one (or multiple) labels of the entries to be opened.
         * `-f`, `--field`: specifies the field to be opened, bypassing the interactive prompt.
     """
 
     name = "open"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.opened_entries: set[str] = set()
         """The set of labels corresponding to the entries which were opened by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="open", description="Open subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="open", description="Open subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("labels", type=str, nargs="+", help="labels of the entries")
         parser.add_argument(
             "-f",
             "--field",
             type=str,
             choices=["all", *config.commands.open.fields],
             help="which field to open in case multiple are found",
```

### Comparing `cobib-4.5.0/src/cobib/commands/redo.py` & `cobib-5.0.0/src/cobib/commands/redo.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,61 +17,56 @@
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `r` key.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import subprocess
 import sys
 from pathlib import Path
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class RedoCommand(Command):
     """The Redo Command.
 
     This command does not parse any additional arguments.
     """
 
     name = "redo"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.root: Path
         """The path to the root of the git repository tracking the database."""
 
         self.sha: str
         """The git commit SHA which was reverted by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="redo", description="Redo subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="redo", description="Redo subcommand parser.", exit_on_error=True
+        )
         cls.argparser = parser
 
     @override
     def execute(self) -> None:
         git_tracked = config.database.git
         if not git_tracked:
             msg = (
```

### Comparing `cobib-4.5.0/src/cobib/commands/review.py` & `cobib-5.0.0/src/cobib/commands/review.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,28 +103,27 @@
 import json
 import logging
 import subprocess
 from collections.abc import Callable
 from functools import wraps
 from typing import cast
 
-from rich.console import Console, Group
+from rich.console import Group
 from rich.prompt import InvalidResponse, PromptBase, PromptType
 from rich.syntax import Syntax
 from rich.text import Text
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.parsers import YAMLParser
 from cobib.utils.prompt import Prompt
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 from .edit import EditCommand
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
@@ -149,35 +148,32 @@
         * in addition to the above, you can add `filters` to specify a subset of your
           database for reviewing. For more information refer to `cobib.commands.list_`.
     """
 
     name = "review"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         if self.largs.done is None:
             # NOTE: we cannot make the default of the `done` argument an empty list because this
             # would remain the same list across multiple runs of the review command within the same
             # session.
             self.largs.done = []
 
         self.reviewed_entries: list[Entry] = []
         """A list of `cobib.database.Entry` objects which were marked as `done` by this review."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="review", description="Review subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="review", description="Review subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("field", type=str, nargs="*", help="the field(s) to review")
         parser.add_argument(
             "-c",
             "--context",
             action="store_true",
             help="When specified, the full entries will be previewed even if selected fields have "
             "been provided. This disables the interactive `context` action by always enabling it.",
```

### Comparing `cobib-4.5.0/src/cobib/commands/search.py` & `cobib-5.0.0/src/cobib/commands/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,25 @@
 
 from __future__ import annotations
 
 import argparse
 import asyncio
 import logging
 
-from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase, PromptType
+from rich.console import ConsoleRenderable
 from rich.text import Text
 from rich.tree import Tree
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Entry
 from cobib.ui.components import SearchView
 from cobib.utils.progress import Progress
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class SearchCommand(Command):
@@ -109,21 +107,16 @@
         * in addition to the above, you can add `filters` to narrow the search down to a subset of
           your database. For more information refer to `cobib.commands.list_`.
     """
 
     name = "search"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.entries: list[Entry] = []
         """A filtered list of entries searched over by this command."""
 
         self.matches: list[list[list[str]]] = []
         """The search matches detected by this command. This is a nested list of the following
         structure: the first list level iterates over the entries; the second list level iterates
@@ -132,15 +125,17 @@
 
         self.hits: int = 0
         """The number of search hits detected by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="search", description="Search subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="search", description="Search subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("query", type=str, nargs="+", help="text to search for")
         ignore_case_group = parser.add_mutually_exclusive_group()
         ignore_case_group.add_argument(
             "-i",
             "--ignore-case",
             action="store_true",
             default=None,
```

### Comparing `cobib-4.5.0/src/cobib/commands/show.py` & `cobib-5.0.0/src/cobib/commands/show.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `ENTER` key.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 
-from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase, PromptType
+from rich.console import ConsoleRenderable
 from rich.syntax import Syntax
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.parsers.bibtex import BibtexParser
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ShowCommand(Command):
     """The Show Command.
@@ -38,29 +37,26 @@
 
         * `label`: the label of the entry to be shown.
     """
 
     name = "show"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.entry_str: str = ""
         """The string-formatted `cobib.database.Entry` shown by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="show", description="Show subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="show", description="Show subcommand parser.", exit_on_error=True
+        )
         parser.add_argument("label", type=str, help="label of the entry")
         cls.argparser = parser
 
     @override
     def execute(self) -> None:
         LOGGER.debug("Starting Show command.")
```

### Comparing `cobib-4.5.0/src/cobib/commands/undo.py` & `cobib-5.0.0/src/cobib/commands/undo.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,27 @@
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `u` key.
 """
 
 from __future__ import annotations
 
+import argparse
 import logging
 import subprocess
 import sys
 from pathlib import Path
 
-from rich.console import Console
-from rich.prompt import PromptBase, PromptType
-from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
-from .base_command import ArgumentParser, Command
+from .base_command import Command
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class UndoCommand(Command):
     """The Undo Command.
@@ -53,32 +51,29 @@
         * `-f`, `--force`: if specified, this will also revert changes which have *not* been
           auto-committed by coBib.
     """
 
     name = "undo"
 
     @override
-    def __init__(
-        self,
-        *args: str,
-        console: Console | App[None] | None = None,
-        prompt: type[PromptBase[PromptType]] | None = None,
-    ) -> None:
-        super().__init__(*args, console=console, prompt=prompt)
+    def __init__(self, *args: str) -> None:
+        super().__init__(*args)
 
         self.root: Path
         """The path to the root of the git repository tracking the database."""
 
         self.sha: str
         """The git commit SHA which was reverted by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="undo", description="Undo subcommand parser.")
+        parser = argparse.ArgumentParser(
+            prog="undo", description="Undo subcommand parser.", exit_on_error=True
+        )
         parser.add_argument(
             "-f", "--force", action="store_true", help="allow undoing non auto-committed changes"
         )
         cls.argparser = parser
 
     @override
     def execute(self) -> None:
```

### Comparing `cobib-4.5.0/src/cobib/config/__init__.py` & `cobib-5.0.0/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/config/config.py` & `cobib-5.0.0/src/cobib/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import io
 import logging
 import os
 import sys
 from abc import abstractmethod
 from collections.abc import Callable
 from dataclasses import MISSING, dataclass, field, fields
-from enum import Enum, EnumMeta, auto
+from enum import Enum, auto
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, NamedTuple, TextIO
+from typing import TYPE_CHECKING, NamedTuple, TextIO
 
 from rich.style import Style
 from rich.theme import Theme
 from typing_extensions import override
 
 from cobib.utils.rel_path import RelPath
 
@@ -506,50 +506,139 @@
         self.list_.validate()
         self.modify.validate()
         self.open.validate()
         self.search.validate()
         self.show.validate()
 
 
-class _DeprecateOnAccess(EnumMeta):
-    """A metaclass to add deprecation warnings to deprecated Enum values upon access."""
-
-    @override
-    def __getattribute__(cls, name: str) -> Any:
-        if name == "CAPTIAL":
-            LOGGER.log(
-                45,
-                "The LabelSuffix.CAPTIAL value is deprecated! Please switch to the correctly "
-                "spelled LabelSuffix.CAPITAL instead.",
-            )
-        return super().__getattribute__(name)
-
-    @override
-    def __getitem__(cls, name: str) -> Any:
-        if name == "CAPTIAL":
-            LOGGER.log(
-                45,
-                "The LabelSuffix.CAPTIAL value is deprecated! Please switch to the correctly "
-                "spelled LabelSuffix.CAPITAL instead.",
-            )
-        return super().__getitem__(name)
-
-
-class LabelSuffix(Enum, metaclass=_DeprecateOnAccess):
+class LabelSuffix(Enum):
     """Suffixes to disambiguate `cobib.database.Entry` labels."""
 
     ALPHA = lambda count: chr(96 + count)
     """Enumerates with lowercase roman letters: `a-z`."""
     CAPITAL = lambda count: chr(64 + count)
     """Enumerates with uppercase roman letters: `A-Z`."""
 
     NUMERIC = lambda count: str(count)
     """Enumerates with arabic numbers: `1, 2, ...`."""
-    CAPTIAL = lambda count: chr(64 + count)
-    """**Deprecated!** This is a deprecated mistyped name of `LabelSuffix.CAPITAL`."""
+
+    @staticmethod
+    def reverse(type_: LabelSuffix, suffix: str) -> int:
+        """Reverses a label suffix enumerator from a suffix to its integer value.
+
+        Args:
+            type_: the `LabelSuffix` enumerator.
+            suffix: the suffix to reverse.
+
+        Returns:
+            The integer value of the reversed suffix.
+
+        Raises:
+            ValueError: if a non-numeric suffix is longer than 1 character.
+            ValueError: if an alphabetic suffix did not fall within the alphabet.
+            ValueError: if an invalid suffix of some other form is provided.
+        """
+        # TODO: once Python 3.10 becomes the default, change this to a match statement
+
+        if type_ == LabelSuffix.NUMERIC:
+            return int(suffix)
+
+        if len(suffix) > 1:
+            raise ValueError("A non-numeric suffix may not be longer than a single character.")
+
+        if type_ in {LabelSuffix.ALPHA, LabelSuffix.CAPITAL}:
+            # we can convert both of these cases in the same way by using base 36 for `int()`
+            ret = int(suffix, 36) - 9
+            if ret < 0:
+                raise ValueError(
+                    f"'{suffix}' is not a valid alphabetic suffix because its ANSI value falls "
+                    "outside of the alphabetic range, yielding a negative value."
+                )
+            return ret
+
+        raise ValueError(f"'{suffix}' is not a valid suffix.")
+
+    @staticmethod
+    def suffix_type(suffix: str) -> LabelSuffix | None:
+        """Determines the enumerator type for a given suffix.
+
+        Args:
+            suffix: the suffix whose enumerator type to determine.
+
+        Returns:
+            An optional enumerator type. If the suffix was invalid, `None` will be returned.
+        """
+        if not suffix.isascii():
+            # if the input contains a non-ASCII character, it cannot be a label suffix
+            return None
+
+        try:
+            # test if the suffix is numeric by attempting to convert it to a base-10 integer
+            _ = int(suffix)
+        except ValueError:
+            # first ensure that we have only alphabetic characters left
+            if not suffix.isalpha():
+                # this is important, because for example "hello123" will pass `islower()` because
+                # all of the cased characters are indeed lower-cased
+                return None
+
+            if suffix.islower():
+                return LabelSuffix.ALPHA
+            if suffix.isupper():
+                return LabelSuffix.CAPITAL
+        else:
+            return LabelSuffix.NUMERIC
+
+        # the provided suffix did not match any of the builtin enumerators
+        return None
+
+    @staticmethod
+    def trim_label(label: str, separator: str, type_: LabelSuffix) -> tuple[str, int]:
+        """Trims the provided label based on the separator and suffix type.
+
+        Args:
+            label: the label whose suffix to trim.
+            separator: the separator character between the actual label and the suffix.
+            type_: the `LabelSuffix` enumerator.
+
+        Returns:
+            The pair of the trimmed label and numeric value of its original suffix.
+        """
+        # initialize the counter of the suffix
+        suffix_value = 0
+
+        # try split the suffix from the label using the provided separator
+        *pieces, suffix = label.split(separator)
+
+        if pieces:
+            # piece together the left-over raw label without its suffix
+            raw_label = separator.join(pieces)
+            # determine the suffix type of this label
+            suffix_type = LabelSuffix.suffix_type(suffix)
+
+            if suffix_type is not None and suffix_type != type_:
+                # if it does not match the expected suffix type, ignore it
+                LOGGER.info(
+                    f"The suffix type encountered on '{label}' does not match the configured one. "
+                    "Assuming that this is intentional and therefore ignoring this as a suffix."
+                )
+                raw_label = label
+            else:
+                try:
+                    # try to obtain the suffix value by reversing it
+                    suffix_value = LabelSuffix.reverse(type_, suffix)
+                except ValueError:
+                    # if this fails, reset the raw label and assume that this was not an actual
+                    # disambiguation suffix
+                    raw_label = label
+        else:
+            # the original split did not yield any pieces so the `suffix` is the actual `raw_label`
+            raw_label = suffix
+
+        return (raw_label, suffix_value)
 
 
 class AuthorFormat(Enum):
     """Storage formats for the `author` information."""
 
     YAML = auto()
     """Stores the list of authors as a YAML list, separating out the first and last names as well as
@@ -973,15 +1062,15 @@
         if spec is None:
             LOGGER.error(
                 "The config at %s could not be interpreted as a Python module.", configpath
             )
             sys.exit(1)
         else:
             cfg = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(cfg)  # type: ignore
+            spec.loader.exec_module(cfg)  # type: ignore[union-attr]
 
         try:
             # validate config
             config.validate()
         except RuntimeError as exc:
             LOGGER.error(exc)
             sys.exit(1)
```

### Comparing `cobib-4.5.0/src/cobib/config/event.py` & `cobib-5.0.0/src/cobib/config/event.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/config/example.py` & `cobib-5.0.0/src/cobib/config/example.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/database/__init__.py` & `cobib-5.0.0/src/cobib/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/database/author.py` & `cobib-5.0.0/src/cobib/database/author.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
             last = parts[-1]
             first = parts[0]
             particle = None
             for part in parts[1:-1]:
                 if part[0].islower():
                     if particle:
-                        particle += " " + part
+                        particle += " " + part  # type: ignore[unreachable]
                     else:
                         particle = part
                 else:
                     first += " " + part
 
             return Author(first, last, particle=particle)
```

### Comparing `cobib-4.5.0/src/cobib/database/database.py` & `cobib-5.0.0/src/cobib/database/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,26 @@
 
 import logging
 import pickle
 import re
 import sys
 from collections import OrderedDict
 from pathlib import Path
-from typing import TYPE_CHECKING, ClassVar, cast
+from typing import ClassVar, cast
 
-from cobib.config import config
+from cobib.config import LabelSuffix, config
 from cobib.utils.rel_path import RelPath
 
-if TYPE_CHECKING:
-    import cobib.database
+from .entry import Entry
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
-# TODO: once Python 3.9 becomes the default, OrderedDict can be properly sub-typed
-class Database(OrderedDict):  # type: ignore
+class Database(OrderedDict[str, Entry]):
     """coBib's Database class is a runtime interface to the plain-test YAML file.
 
     This class is a *singleton*.
     Thus, accessing `cobib.database.Database` will always yield the identical instance at runtime.
     This ensures data consistency during all operations on the database.
     """
 
@@ -58,15 +56,15 @@
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._unsaved_entries = {}
         if not cls._read:
             cls.read(bypass_cache=bypass_cache)
         return cls._instance
 
-    def update(self, new_entries: dict[str, cobib.database.Entry]) -> None:  # type: ignore
+    def update(self, new_entries: dict[str, Entry]) -> None:  # type: ignore[explicit-override,override]
         """Updates the database with the given dictionary of entries.
 
         This function wraps `OrderedDict.update` and adds the labels of the changed entries to the
         dictionary of unsaved entries (`Database._unsaved_entries`). This will minimize IO access by
         only actually writing the unsaved entries in batches.
 
         Args:
@@ -74,28 +72,28 @@
                 database.
         """
         for label in new_entries.keys():
             LOGGER.debug("Updating entry %s", label)
             Database._unsaved_entries[label] = label
         super().update(new_entries)
 
-    def pop(self, label: str) -> cobib.database.Entry:  # type: ignore
+    def pop(self, label: str) -> Entry:  # type: ignore[explicit-override,override]
         """Pops the entry pointed to by the given label.
 
         This function wraps `OrderedDict.pop` and adds the removed labels to the unsaved entries
         (`Database._unsaved_entries`). This will minimize IO access by only actually writing the
         unsaved entries in batches.
 
         Args:
             label: the label of the entry to be removed.
 
         Returns:
             The entry pointed to by the given label.
         """
-        entry: cobib.database.Entry = super().pop(label)
+        entry: Entry = super().pop(label)
         LOGGER.debug("Removing entry: %s", label)
         Database._unsaved_entries[label] = None
         return entry
 
     def rename(self, old_label: str, new_label: str) -> None:
         """Renames an entry label.
 
@@ -110,15 +108,15 @@
         Database._unsaved_entries[old_label] = new_label
         if new_label != old_label:
             # NOTE: this is not technically needed but the rename method is exploited during
             # database linting with "fake" renames in order to register entries for re-writing
             # during saving
             super().pop(old_label)
 
-    def disambiguate_label(self, label: str, entry: cobib.database.Entry) -> str:
+    def disambiguate_label(self, label: str, entry: Entry) -> str:
         """Disambiguate a given label to ensure it becomes unique.
 
         This function ensures that a label is unique by appending a configurable suffix to a label
         if it is already present in the database at runtime.
 
         Args:
             label: the label which to disambiguate.
@@ -155,14 +153,44 @@
                 "you are running a disambiguation of the label '%s'. You may want to check whether "
                 "these two entries are related and (if so) edit or merge them manually. For more "
                 "information see also: https://gitlab.com/cobib/cobib/-/issues/121",
                 new_label,
                 label,
             )
 
+    def find_related_labels(self, label: str) -> tuple[set[str], set[str]]:
+        """Finds related labels to the provided one.
+
+        Args:
+            label: the original label for which to find related ones.
+
+        Returns:
+            A pair of sets of strings. The first set contains directly related labels, i.e. ones
+            which match the provided label exactly, modulo the value of their suffix based on
+            `config.database.format.label_suffix`. The second set contains indirectly related
+            labels, i.e. ones which also start with the same text as the original label but do not
+            have a matching suffix.
+        """
+        separator, enumerator = config.database.format.label_suffix
+        trimmed_label, _ = LabelSuffix.trim_label(label, separator, enumerator)
+
+        directly_related_labels = set()
+        indirectly_related_labels = set()
+        for existing_label in self.keys():
+            if not existing_label.startswith(trimmed_label):
+                continue
+
+            raw_label, _ = LabelSuffix.trim_label(existing_label, separator, enumerator)
+            if raw_label == trimmed_label:
+                directly_related_labels.add(existing_label)
+            else:
+                indirectly_related_labels.add(existing_label)
+
+        return directly_related_labels, indirectly_related_labels
+
     @classmethod
     def reset(cls) -> None:
         """Resets the database.
 
         This clears the contents of the singleton instance and resets the `_read` class attribute.
         """
         if cls._instance is not None:
@@ -269,15 +297,15 @@
                     continue
             except AttributeError:
                 pass
             if overwrite and line.startswith("..."):
                 LOGGER.debug('Reached end of entry "%s".', cur_label)
                 overwrite = False
 
-                new_label = cls._unsaved_entries.pop(cur_label)
+                new_label = cast(str, cls._unsaved_entries.pop(cur_label))
                 entry = _instance.get(new_label, None)
                 if entry:
                     LOGGER.debug('Writing modified entry "%s".', new_label)
                     entry_str = entry.save(parser=yml)
                     buffer.append("\n".join(entry_str.split("\n")[1:]))
                 else:
                     # Entry has been deleted. Pop the previous `---` line.
```

### Comparing `cobib-4.5.0/src/cobib/database/entry.py` & `cobib-5.0.0/src/cobib/database/entry.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/importers/base_importer.py` & `cobib-5.0.0/src/cobib/importers/base_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import argparse
 import logging
 import sys
 from abc import ABC, abstractmethod
 
 from cobib.database import Entry
-from cobib.ui.components import ArgumentParser as ArgumentParser  # noqa: PLC0414
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class Importer(ABC):
     """The Importer interface.
@@ -20,15 +19,15 @@
     This interface should be implemented by all concrete importer implementations.
     """
 
     name = "base"
     """The importers `name` is used to register itself as an input argument to the
     `cobib.commands.import_.ImportCommand`."""
 
-    argparser: ArgumentParser
+    argparser: argparse.ArgumentParser
     """Every importer has its own `argparse.ArgumentParser` which is used to parse the arguments
     provided to it."""
 
     def __init__(self, *args: str, skip_download: bool = False) -> None:
         """Initializes an importer instance.
 
         Args:
@@ -53,15 +52,15 @@
         """Initializes this importer's `argparse.ArgumentParser`.
 
         This method needs to be overwritten by every subclass and handles the registration of all
         available importer arguments.
         """
 
     @classmethod
-    def _get_argparser(cls) -> ArgumentParser:
+    def _get_argparser(cls) -> argparse.ArgumentParser:
         """Returns this importer's `argparse.ArgumentParser`.
 
         The reason for having this method is to handle the parser initialization such that it only
         needs to be done once.
 
         Returns:
             This importer's initialized `argparser` object.
```

### Comparing `cobib-4.5.0/src/cobib/importers/zotero.py` & `cobib-5.0.0/src/cobib/importers/zotero.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ```
 
 [1]: https://www.zotero.org/
 """
 
 from __future__ import annotations
 
+import argparse
 import json
 import logging
 import os
 import subprocess
 import sys
 
 import requests
@@ -53,15 +54,15 @@
 
 from cobib.config import Event, config
 from cobib.database import Entry
 from cobib.parsers import BibtexParser
 from cobib.utils.file_downloader import FileDownloader
 from cobib.utils.rel_path import RelPath
 
-from .base_importer import ArgumentParser, Importer
+from .base_importer import Importer
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class ZoteroImporter(Importer):
     """The Zotero Importer.
@@ -105,15 +106,17 @@
 
         self.imported_entries: list[Entry] = []
         """A list of `cobib.database.Entry` objects which were imported by this importer."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
-        parser = ArgumentParser(prog="zotero", description="Zotero migration parser.")
+        parser = argparse.ArgumentParser(
+            prog="zotero", description="Zotero migration parser.", exit_on_error=True
+        )
         parser.add_argument(
             "--no-cache", action="store_true", help="disable use of cached OAuth tokens"
         )
         parser.add_argument(
             "--api-key", type=str, help="the user-specific Zotero API key for the coBib application"
         )
         parser.add_argument("--user-id", type=str, help="the Zotero user ID used for API calls")
```

### Comparing `cobib-4.5.0/src/cobib/parsers/__init__.py` & `cobib-5.0.0/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/arxiv.py` & `cobib-5.0.0/src/cobib/parsers/arxiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,24 +65,24 @@
             if page.encoding is None:
                 page.encoding = "utf-8"
         except requests.exceptions.RequestException as err:
             LOGGER.error("An Exception occurred while trying to query the arXiv ID: %s.", arxiv_id)
             LOGGER.error(err)
             return OrderedDict()
         xml = BeautifulSoup(page.text, features="xml")
-        if xml.feed.entry.title.contents[0] == "Error":
+        if xml.feed.entry.title.contents[0] == "Error":  # type: ignore[union-attr]
             msg = (
-                "The arXiv API returned the following error: " + xml.feed.entry.summary.contents[0]
+                "The arXiv API returned the following error: " + xml.feed.entry.summary.contents[0]  # type: ignore[operator,union-attr]
             )
             LOGGER.warning(msg)
             return OrderedDict()
         label = ""
         entry: dict[str, Any] = {}
         entry["archivePrefix"] = "arXiv"
-        for key in xml.feed.entry.findChildren(recursive=False):
+        for key in xml.feed.entry.findChildren(recursive=False):  # type: ignore[union-attr]
             if "doi" in key.name:
                 entry["doi"] = str(key.contents[0])
             elif key.name == "id":
                 entry["arxivid"] = str(key.contents[0]).replace("http://arxiv.org/abs/", "")
                 entry["eprint"] = str(key.contents[0])
             elif key.name == "primary_category":
                 entry["primaryClass"] = str(key.attrs["term"])
```

### Comparing `cobib-4.5.0/src/cobib/parsers/base_parser.py` & `cobib-5.0.0/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/bibtex.py` & `cobib-5.0.0/src/cobib/parsers/bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/doi.py` & `cobib-5.0.0/src/cobib/parsers/doi.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/isbn.py` & `cobib-5.0.0/src/cobib/parsers/isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/url.py` & `cobib-5.0.0/src/cobib/parsers/url.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/parsers/yaml.py` & `cobib-5.0.0/src/cobib/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/cli.py` & `cobib-5.0.0/src/cobib/ui/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 This class provides the main entry point to coBib. It exposes all the commands implemented in
 `cobib.commands` to the end-user and leverages [`rich`](https://github.com/textualize/rich) to
 produce beautiful output.
 """
 
 import argparse
 import asyncio
-import inspect
 import logging
 import sys
 from inspect import iscoroutinefunction
 from typing import Any
 
 from rich.console import Console
 from typing_extensions import override
 
-from cobib import __version__, commands
+from cobib import __version__
 from cobib.config import config
-from cobib.database import Database
+from cobib.ui.components.entry_points import entry_points
 from cobib.ui.tui import TUI
 from cobib.ui.ui import UI
 from cobib.utils.logging import print_changelog
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
@@ -37,19 +36,23 @@
         is omitted, the `cobib.ui.tui.TUI` gets started.
     """
 
     @override
     def add_extra_parser_arguments(self) -> None:
         self.parser.add_argument("--version", action="version", version=f"%(prog)s v{__version__}")
 
-        subcommands = [cls.name for _, cls in inspect.getmembers(commands) if inspect.isclass(cls)]
         self.parser.add_argument(
-            "command", help="subcommand to be called", choices=subcommands, nargs="?"
+            "command",
+            help="the subcommand to be run",
+            choices=sorted([cls.name for (cls, _) in entry_points("cobib.commands")]),
+            nargs="?",
+        )
+        self.parser.add_argument(
+            "args", nargs=argparse.REMAINDER, help="any arguments passed on to the subcommand"
         )
-        self.parser.add_argument("args", nargs=argparse.REMAINDER)
 
     @override
     def parse_args(self) -> argparse.Namespace:
         arguments = super().parse_args()
         if arguments.command is not None:
             sys_args = list(sys.argv)
             subcmd_args = sys_args[sys_args.index(arguments.command) + 1 :]
@@ -67,16 +70,15 @@
     @override
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.init_argument_parser(
             prog="coBib",
             description=(
-                "Cobib input arguments.\nIf no arguments are given, the TUI will start as a "
-                "default."
+                "coBib input arguments.\nIf no subcommand is given, the TUI will be started."
             ),
         )
 
     @override
     async def run(self) -> None:  # type: ignore[override]
         arguments = self.parse_args()
 
@@ -84,31 +86,24 @@
 
         if not arguments.porcelain:
             # print latest changelog
             changelog = print_changelog(__version__, config.logging.version)
             if changelog is not None:
                 console.print(changelog)
 
-        if arguments.command == "init":
-            # the database file may not exist yet, thus we ensure to execute the command before
-            # trying to read the database file
-            subcmd = getattr(commands, "InitCommand")(*arguments.args)
-            subcmd.execute()
-            return
-
-        # initialize database
-        Database()
-
         if not arguments.command:
             task = asyncio.create_task(TUI().run_async())  # type: ignore[abstract]
             await task
             # the following is required for the asynchronous TUI to quit properly
             sys.exit()
         else:
-            subcmd = getattr(commands, arguments.command.title() + "Command")(*arguments.args)
+            (cls,) = [
+                cls for (cls, _) in entry_points("cobib.commands") if cls.name == arguments.command
+            ]
+            subcmd = cls.load()(*arguments.args)
             if iscoroutinefunction(subcmd.execute):
                 await subcmd.execute()
             else:
                 subcmd.execute()
             if arguments.porcelain:
                 output = subcmd.render_porcelain()
                 for line in output:
```

### Comparing `cobib-4.5.0/src/cobib/ui/components/__init__.py` & `cobib-5.0.0/src/cobib/ui/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
    This module makes no API stability guarantees! With the `cobib.ui.tui.TUI` being based on
    [`textual`](https://textual.textualize.io/) which is still in very early stages of its
    development, breaking API changes in this module might be released as part of coBib's feature
    releases. You have been warned.
 """
 
-from .argument_parser import ArgumentParser as ArgumentParser
 from .entry_view import EntryView as EntryView
 from .help_screen import HelpScreen as HelpScreen
 from .input_screen import InputScreen as InputScreen
 from .list_view import ListView as ListView
 from .log_screen import LogScreen as LogScreen
 from .logging_handler import LoggingHandler as LoggingHandler
 from .main_content import MainContent as MainContent
```

### Comparing `cobib-4.5.0/src/cobib/ui/components/entry_view.py` & `cobib-5.0.0/src/cobib/ui/components/entry_view.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/help_screen.py` & `cobib-5.0.0/src/cobib/ui/components/help_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/input_screen.py` & `cobib-5.0.0/src/cobib/ui/components/input_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/list_view.py` & `cobib-5.0.0/src/cobib/ui/components/list_view.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/log_screen.py` & `cobib-5.0.0/src/cobib/ui/components/log_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/logging_handler.py` & `cobib-5.0.0/src/cobib/ui/components/logging_handler.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/main_content.py` & `cobib-5.0.0/src/cobib/ui/components/main_content.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/motion_key.py` & `cobib-5.0.0/src/cobib/ui/components/motion_key.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/preset_filter_screen.py` & `cobib-5.0.0/src/cobib/ui/components/preset_filter_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/search_view.py` & `cobib-5.0.0/src/cobib/ui/components/search_view.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/components/selection_filter.py` & `cobib-5.0.0/src/cobib/ui/components/selection_filter.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/ui/tui.py` & `cobib-5.0.0/src/cobib/ui/tui.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 import asyncio
 import io
 import logging
 import shlex
 from collections.abc import Awaitable, Callable, Coroutine
 from contextlib import redirect_stderr, redirect_stdout
 from inspect import iscoroutinefunction
-from typing import Any, ClassVar, cast
+from typing import TYPE_CHECKING, Any, ClassVar, cast
 
 from textual.app import App, ComposeResult
 from textual.binding import Binding
 from textual.keys import Keys
 from textual.logging import TextualHandler
 from textual.screen import Screen
 from textual.widgets import Footer, Header, Input, Static
 from typing_extensions import override
 
-from cobib import commands
 from cobib.config import config
 from cobib.database import Database
 from cobib.ui.components import (
     EntryView,
     HelpScreen,
     InputScreen,
     ListView,
@@ -42,17 +41,21 @@
     LogScreen,
     MainContent,
     MotionKey,
     PresetFilterScreen,
     SearchView,
     SelectionFilter,
 )
-from cobib.ui.ui import UI
 from cobib.utils.prompt import Confirm
 
+from .ui import UI
+
+if TYPE_CHECKING:
+    from cobib import commands
+
 LOGGER = logging.getLogger(__name__)
 
 
 # NOTE: pylint and mypy are unable to understand that the `App` interface actually implements `run`
 
 
 class TUI(UI, App[None]):  # type: ignore[misc]
@@ -374,26 +377,30 @@
         """Edits the current entry.
 
         Suspension of the App is handled directly by the edit command using
         `cobib.utils.context.get_active_app`.
         """
         main = self.query_one(MainContent)
         label = main.get_current_label()
+        from cobib import commands
+
         commands.EditCommand(label).execute()
 
     def _show_entry(self, command: commands.ShowCommand | None = None) -> None:
         """Renders the entry currently under the cursor in the `EntryView` widget.
 
         Args:
             command: the `cobib.commands.show.ShowCommand` to execute. If this is `None`, a new
                 instance will be constructed to show the entry at the current cursor location.
         """
         if command is None:
             main = self.query_one(MainContent)
             label = main.get_current_label()
+            from cobib import commands
+
             command = commands.ShowCommand(label)
         command.execute()
         entry = self.query_one(EntryView)
         static = entry.query_one(Static)
         static.update(
             command.render_rich(
                 background_color=entry.background_colors[1].rich_color.name,
@@ -403,14 +410,16 @@
     def _jump_to_entry(self, command: list[str]) -> None:
         """Jumps the cursor in the current view to the entry provided by the command arguments.
 
         Args:
             command: the list of command arguments to be passed to the
                 `cobib.commands.show.ShowCommand`.
         """
+        from cobib import commands
+
         show_cmd = commands.ShowCommand(*command)
         label = show_cmd.largs.label
         main = self.query_one(MainContent)
         try:
             main.jump_to_label(label)
         except KeyError:
             if label in Database():
@@ -421,14 +430,16 @@
                 LOGGER.info(msg)
         self._show_entry(show_cmd)
 
     async def _update_table(self) -> None:
         """Updates the list of entries displayed in the `MainContent`."""
         main = self.screen_stack[0].query_one(MainContent)
         old_table = main.query_one(ListView)
+        from cobib import commands
+
         command = commands.ListCommand(*self._list_args)
         command.execute()
         table = command.render_textual()
         await main.replace_widget(table)
         table.focus()
         if old_table is not None:
             table.cursor_coordinate = old_table.cursor_coordinate
@@ -440,14 +451,16 @@
     async def _update_tree(self, command: list[str]) -> None:
         """Updates the tree of search results displayed in the `MainContent`.
 
         Args:
             command: the list of command arguments to be passed to the
                 `cobib.commands.search.SearchCommand`.
         """
+        from cobib import commands
+
         subcmd = commands.SearchCommand(*command)
         await subcmd.execute()
         tree = subcmd.render_textual()
         main = self.query_one(MainContent)
         await main.replace_widget(tree)
         tree.focus()
         self.refresh(layout=True)
@@ -492,14 +505,16 @@
             if command[0].lower() == "list":
                 self._list_args = command[1:]
                 await self._update_table()
             elif command[0].lower() == "search":
                 await self._update_tree(command[1:])
             elif command[0].lower() == "edit":
                 with self.suspend():
+                    from cobib import commands
+
                     commands.EditCommand(*command[1:]).execute()
             else:
                 self._run_command(command)
 
     @staticmethod
     async def _async_done_callback(
         task: Awaitable[None], async_callback: Callable[[], Coroutine[Any, Any, None]]
@@ -521,14 +536,16 @@
 
         Args:
             command: a list of strings consisting of the command keyword and its arguments.
         """
         with redirect_stdout(io.StringIO()) as stdout:
             with redirect_stderr(io.StringIO()) as stderr:
                 try:
+                    from cobib import commands
+
                     subcmd = getattr(commands, command[0].title() + "Command")(*command[1:])
 
                     if not iscoroutinefunction(subcmd.execute):
                         subcmd.execute()
                     else:
                         # FIXME: in these cases, stdout and stderr cannot be captured
```

### Comparing `cobib-4.5.0/src/cobib/ui/ui.py` & `cobib-5.0.0/src/cobib/ui/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import argparse
 import logging
 from abc import abstractmethod
 from typing import Any
 
 from cobib.config import config
-from cobib.ui.components import ArgumentParser
 from cobib.utils.logging import get_file_handler, get_stream_handler
 
 LOGGER = logging.getLogger(__name__)
 """@private module logger."""
 
 
 class UI:
@@ -25,15 +24,15 @@
         * `-v`, `--verbose`: increase the logging verbosity for every time this argument is given.
         * `-p`, `--porcelain`: switches the output to porcelain mode.
         * `-l`, `--logfile`: provides the path to an alternative logging file, overwriting the
             `cobib.config.config.LoggingConfig.logfile` setting.
         * `-c`, `--config`: provides the path to an alternative configuration file.
     """
 
-    parser: ArgumentParser
+    parser: argparse.ArgumentParser
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initializes a UI object.
 
         The function signature is left purposefully vague to allow arbitrarily complex UI subclasses
         built on top of this.
 
@@ -57,15 +56,15 @@
         This method needs to called by a subclass manually (preferably) during its `__init__`. The
         keyword arguments can be used to add additional information to the `ArgumentParser`, which
         can be used to inject information into the `--help` output.
 
         Args:
             **kwargs: arbitrary keyword arguments passed on to the `ArgumentParser` constructor.
         """
-        self.parser = ArgumentParser(**kwargs)
+        self.parser = argparse.ArgumentParser(exit_on_error=True, **kwargs)
         self.parser.add_argument("-v", "--verbose", action="count", default=0)
         self.parser.add_argument(
             "-p",
             "--porcelain",
             action="store_true",
             help="switches the output to porcelain mode (meant for parsing/testing)",
         )
@@ -76,15 +75,16 @@
             "-c", "--config", type=argparse.FileType("r"), help="Alternative config file"
         )
         self.add_extra_parser_arguments()
 
     def add_extra_parser_arguments(self) -> None:
         """A hook to register additional command-line arguments.
 
-        Subclasses can overwrite this method to add additional arguments to the `ArgumentParser`.
+        Subclasses can overwrite this method to add additional arguments to the
+        `argparse.ArgumentParser`.
         This method is internally called during `init_argument_parser`.
         """
 
     def parse_args(self) -> argparse.Namespace:
         """Parses the provided command-line arguments.
 
         This method does not take any arguments because it directly gathers them from the
```

### Comparing `cobib-4.5.0/src/cobib/utils/diff_renderer.py` & `cobib-5.0.0/src/cobib/utils/diff_renderer.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/utils/file_downloader.py` & `cobib-5.0.0/src/cobib/utils/file_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,26 @@
         return cls._instance
 
     _PDF_MARKER = bytes("%PDF", "utf-8")
     """A marker which the downloaded file's beginning is checked against, to determine that it is
     indeed a PDF file."""
 
     @staticmethod
-    def _assert_pdf(content: bytes) -> bool:
+    def _assert_pdf(url: str, content: bytes) -> bool:
         """Asserts that the `content` starts with the `_PDF_MARKER`.
 
         Args:
+            url: the URL from which the content was downloaded.
             content: the string of bytes to check.
 
         Returns:
             Whether the `content` matches.
         """
         if not content.startswith(FileDownloader._PDF_MARKER):
-            LOGGER.warning("The URL did not provide a PDF file. Aborting download!")
+            LOGGER.warning(f"The URL '{url}' did not provide a PDF file. Aborting download!")
             return False
         return True
 
     @staticmethod
     def _unlink(path: RelPath) -> None:
         """Remove a file and ignore any error.
 
@@ -113,16 +114,16 @@
         url = FileDownloader._map_url(url)
 
         with open(path.path, "wb") as file:
             LOGGER.info("Downloading %s to %s", url, path)
 
             try:
                 response = requests.get(url, timeout=10, stream=True, headers=headers)
-                total_length = response.headers.get("content-length", None)
-                total_length = int(total_length) if total_length is not None else None
+                total_length_str = response.headers.get("content-length", None)
+                total_length = int(total_length_str) if total_length_str is not None else None
             except requests.exceptions.RequestException as err:
                 msg = f"An Exception occurred while downloading the file located at {url}"
                 LOGGER.warning(msg)
                 LOGGER.error(err)
                 FileDownloader._recover(path, backup)
                 return None
 
@@ -137,22 +138,22 @@
                 await optional_awaitable
 
             task = progress_bar.add_task("Downloading...", total=total_length)
 
             accumulated_length = 0
 
             if total_length is None:
-                if not FileDownloader._assert_pdf(response.content):
+                if not FileDownloader._assert_pdf(url, response.content):
                     FileDownloader._recover(path, backup)
                     progress_bar.stop()
                     return None
                 file.write(response.content)
             else:
                 for data in response.iter_content(chunk_size=4096):
-                    if accumulated_length == 0 and not FileDownloader._assert_pdf(data):
+                    if accumulated_length == 0 and not FileDownloader._assert_pdf(url, data):
                         FileDownloader._recover(path, backup)
                         progress_bar.stop()
                         return None
                     accumulated_length += len(data)
                     progress_bar.advance(task, len(data))
                     await asyncio.sleep(0)
                     file.write(data)
```

### Comparing `cobib-4.5.0/src/cobib/utils/journal_abbreviations.py` & `cobib-5.0.0/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/utils/logging.py` & `cobib-5.0.0/src/cobib/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/utils/progress.py` & `cobib-5.0.0/src/cobib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib/utils/prompt.py` & `cobib-5.0.0/src/cobib/utils/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,20 +161,20 @@
 
     @staticmethod
     def _wrap_process_response(
         func: Callable[[PromptBase[bool], str], bool],
     ) -> Callable[[PromptBase[bool], str], bool]:
         @wraps(func)
         def process_response(prompt: PromptBase[bool], value: str) -> bool:
-            return_value: bool = func(prompt, value)
+            return_value = func(prompt, value)
 
             if isinstance(return_value, bool):
                 return return_value
 
-            if cast(str, return_value).strip().lower() == "y":
+            if cast(str, return_value).strip().lower() == "y":  # type: ignore[unreachable]
                 return True
 
             if cast(str, return_value).strip().lower() == "n":
                 return False
 
             raise InvalidResponse("You may only provide 'y' or 'n' as a valid response.")
```

### Comparing `cobib-4.5.0/src/cobib/utils/rel_path.py` & `cobib-5.0.0/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-4.5.0/src/cobib.egg-info/PKG-INFO` & `cobib-5.0.0/src/cobib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.5.0
+Version: 5.0.0
 Summary: Console Bibliography
 Author-email: Max Rossmannek <max@rossmannek.de>
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/cobib/cobib
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Project-URL: Repository, https://gitlab.com/cobib/cobib
 Project-URL: Issues, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Changelog, https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md
 Keywords: reference-manager,citation-manager,bibliography,cli,tui,command-line,terminal,console,bibtex,doi,arxiv,isbn
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: bibtexparser
 Requires-Dist: lxml
 Requires-Dist: pylatexenc
 Requires-Dist: requests
@@ -255,14 +254,21 @@
 
 You may also specify a different config file at runtime by using the `-c` or `--config` command line argument or by specifying a custom path in the `COBIB_CONFIG` environment variable.
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
+## Plugins
+
+coBib supports the implementation of plugins!
+You can find an example plugin in [this folder](./plugin) or read the docs of
+`cobib_dummy` (when viewing the hosted documentation online).
+
+
 ## Documentation
 
 coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
@@ -301,14 +307,48 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [5.0.0] - 2024-04-28
+
+Pypi: https://pypi.org/project/cobib/5.0.0/
+
+### Added
+
+- the ability to add custom `commands`, `importers`, and `parsers` through entry points (#135, !139)
+  - (DEV) a dummy plugin show-casing these extensions
+
+### Changed
+- the entire `shell_helper` module has been replaced as follows (!139):
+  - the following deprecated helper methods were removed without replacement:
+    - `_list_commands`
+    - `_list_filters`
+    - `_list_labels`
+  - the following secondary commands have been refactored:
+    - `_lint_database` is now `cobib.commands.lint.LintCommand`
+    - `_unify_labels` is now `cobib.commands.unify_labels.UnifyLabelsCommand`
+    - `_example_config` is now `cobib.config.command.ExampleConfigCommand`
+- the interactive disambiguation mechanism during the `add` command now handles
+  multiple matching related entries (#121,!168)
+  - this includes the ability to `cancel` the disambiguation and entry addition
+
+### Removed
+
+- the previously deprecated `console` attribute of all commands has been removed (!139)
+- the previously deprecated `prompt` attribute of all commands has been removed (!139)
+- the `cobib.ui.shell_helper` and `cobib.utils.shell_helper` modules have been removed (!139)
+- the previously deprecated `--update` argument of the `add` command (!168)
+- the previously deprecated `--skip-existing` argument of the `add` command (!168)
+- the previously deprecated `LabelSuffix.CAPTIAL` attribute (!168)
+- Python 3.8 is no longer supported (!173)
+
+
 ## [4.5.0] - 2024-03-17
 
 Pypi: https://pypi.org/project/cobib/4.5.0/
 
 ### Added
 - the new `cobib.utils.context.get_active_app` method which returns any running
   textual App and replaces the need for the `cobib.utils.prompt.Prompt.console`
@@ -1252,15 +1292,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.5.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v5.0.0...master
+[5.0.0]: https://gitlab.com/cobib/cobib/-/tags/v5.0.0
 [4.5.0]: https://gitlab.com/cobib/cobib/-/tags/v4.5.0
 [4.4.0]: https://gitlab.com/cobib/cobib/-/tags/v4.4.0
 [4.3.1]: https://gitlab.com/cobib/cobib/-/tags/v4.3.1
 [4.3.0]: https://gitlab.com/cobib/cobib/-/tags/v4.3.0
 [4.2.0]: https://gitlab.com/cobib/cobib/-/tags/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/tags/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/tags/v4.0.0
```

### Comparing `cobib-4.5.0/src/cobib.egg-info/SOURCES.txt` & `cobib-5.0.0/src/cobib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 src/cobib/commands/base_command.py
 src/cobib/commands/delete.py
 src/cobib/commands/edit.py
 src/cobib/commands/export.py
 src/cobib/commands/git.py
 src/cobib/commands/import_.py
 src/cobib/commands/init.py
+src/cobib/commands/lint.py
 src/cobib/commands/list_.py
 src/cobib/commands/modify.py
 src/cobib/commands/open.py
 src/cobib/commands/redo.py
 src/cobib/commands/review.py
 src/cobib/commands/search.py
 src/cobib/commands/show.py
 src/cobib/commands/undo.py
+src/cobib/commands/unify_labels.py
 src/cobib/config/__init__.py
+src/cobib/config/command.py
 src/cobib/config/config.py
 src/cobib/config/event.py
 src/cobib/config/example.py
 src/cobib/database/__init__.py
 src/cobib/database/author.py
 src/cobib/database/database.py
 src/cobib/database/entry.py
@@ -48,19 +51,18 @@
 src/cobib/parsers/bibtex.py
 src/cobib/parsers/doi.py
 src/cobib/parsers/isbn.py
 src/cobib/parsers/url.py
 src/cobib/parsers/yaml.py
 src/cobib/ui/__init__.py
 src/cobib/ui/cli.py
-src/cobib/ui/shell_helper.py
 src/cobib/ui/tui.py
 src/cobib/ui/ui.py
 src/cobib/ui/components/__init__.py
-src/cobib/ui/components/argument_parser.py
+src/cobib/ui/components/entry_points.py
 src/cobib/ui/components/entry_view.py
 src/cobib/ui/components/help_screen.py
 src/cobib/ui/components/input_screen.py
 src/cobib/ui/components/list_view.py
 src/cobib/ui/components/log_screen.py
 src/cobib/ui/components/logging_handler.py
 src/cobib/ui/components/main_content.py
@@ -73,9 +75,8 @@
 src/cobib/utils/diff_renderer.py
 src/cobib/utils/file_downloader.py
 src/cobib/utils/journal_abbreviations.py
 src/cobib/utils/logging.py
 src/cobib/utils/progress.py
 src/cobib/utils/prompt.py
 src/cobib/utils/rel_path.py
-src/cobib/utils/shell_helper.py
 tests/test_main.py
```

### Comparing `cobib-4.5.0/tests/test_main.py` & `cobib-5.0.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             args: the list of values with which to monkeypatch `sys.argv`.
         """
         logfile = str(Path(tempfile.gettempdir()) / "cobib_test_logging.log")
         # we choose the open command as an arbitrary choice which has minimal side effects
         await self.run_module(monkeypatch, "main", ["cobib", "-l", logfile, *args])
         try:
             assert isinstance(logging.getLogger().handlers[-1], logging.FileHandler)
-            assert logging.getLogger().handlers[-1].baseFilename == logfile  # type: ignore
+            assert logging.getLogger().handlers[-1].baseFilename == logfile  # type: ignore[attr-defined]
         finally:
             os.remove(logfile)
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "args",
         [
```

