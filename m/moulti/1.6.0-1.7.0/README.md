# Comparing `tmp/moulti-1.6.0.tar.gz` & `tmp/moulti-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moulti-1.6.0.tar", last modified: Thu Apr 18 14:41:10 2024, max compression
+gzip compressed data, was "moulti-1.7.0.tar", last modified: Sun Apr 28 13:17:18 2024, max compression
```

## Comparing `moulti-1.6.0.tar` & `moulti-1.7.0.tar`

### file list

```diff
@@ -1,53 +1,62 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.6.0/LICENSE
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4241 2024-04-18 14:41:10.850919 moulti-1.6.0/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3252 2024-04-18 01:55:09.000000 moulti-1.6.0/README.md
--rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.6.0/pyproject.toml
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-18 14:41:10.850919 moulti-1.6.0/setup.cfg
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1497 2024-04-18 14:38:53.000000 moulti-1.6.0/setup.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.846919 moulti-1.6.0/src/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.846919 moulti-1.6.0/src/moulti/
--rw-r--r--   0 xavier    (1000) xavier    (1000)       76 2024-04-18 14:38:56.000000 moulti-1.6.0/src/moulti/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.6.0/src/moulti/__main__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.6.0/src/moulti/ansi.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    21830 2024-04-17 16:17:33.000000 moulti-1.6.0/src/moulti/app.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7395 2024-04-15 23:17:12.000000 moulti-1.6.0/src/moulti/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/helpers.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.6.0/src/moulti/precli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.6.0/src/moulti/protocol.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/
--rw-r--r--   0 xavier    (1000) xavier    (1000)      165 2024-02-16 23:41:25.000000 moulti-1.6.0/src/moulti/widgets/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/abstractquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      600 2024-02-16 15:33:17.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2785 2024-03-12 15:58:46.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/abstractstep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1123 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6555 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/buttonquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.6.0/src/moulti/widgets/cli.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/inputquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/cli.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-03-11 11:06:29.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.6.0/src/moulti/widgets/moulticonsole.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.6.0/src/moulti/widgets/moultilog.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.6.0/src/moulti/widgets/quitdialog.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/step/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.6.0/src/moulti/widgets/step/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4541 2024-02-24 00:23:06.000000 moulti-1.6.0/src/moulti/widgets/step/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7225 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/step/tui.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/stepcontainer.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.6.0/src/moulti/widgets/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.6.0/src/moulti/widgets/vertscroll.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti.egg-info/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4241 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/PKG-INFO
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1274 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/SOURCES.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/dependency_links.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       46 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/entry_points.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       36 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/requires.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/top_level.txt
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.7.0/LICENSE
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4347 2024-04-28 13:17:18.692666 moulti-1.7.0/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3358 2024-04-20 17:36:22.000000 moulti-1.7.0/README.md
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.7.0/pyproject.toml
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-28 13:17:18.692666 moulti-1.7.0/setup.cfg
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1605 2024-04-28 13:14:18.000000 moulti-1.7.0/setup.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.688666 moulti-1.7.0/src/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.688666 moulti-1.7.0/src/moulti/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       76 2024-04-28 13:14:28.000000 moulti-1.7.0/src/moulti/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.7.0/src/moulti/__main__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.7.0/src/moulti/ansi.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    25720 2024-04-28 13:13:58.000000 moulti-1.7.0/src/moulti/app.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2841 2024-04-20 13:43:17.000000 moulti-1.7.0/src/moulti/askpass.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7826 2024-04-24 21:40:25.000000 moulti-1.7.0/src/moulti/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.7.0/src/moulti/helpers.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.7.0/src/moulti/precli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.7.0/src/moulti/protocol.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      177 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/abstractquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2024-04-23 18:32:39.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2794 2024-04-23 17:32:01.000000 moulti-1.7.0/src/moulti/widgets/abstractquestion/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/abstractstep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      699 2024-04-23 18:32:38.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4594 2024-04-23 21:17:23.000000 moulti-1.7.0/src/moulti/widgets/abstractstep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/buttonquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.7.0/src/moulti/widgets/buttonquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.7.0/src/moulti/widgets/cli.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/collapsiblestep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 17:16:59.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 18:32:37.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2805 2024-04-24 21:39:15.000000 moulti-1.7.0/src/moulti/widgets/collapsiblestep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/divider/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/divider/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1614 2024-04-23 20:39:30.000000 moulti-1.7.0/src/moulti/widgets/divider/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      813 2024-04-24 21:40:25.000000 moulti-1.7.0/src/moulti/widgets/divider/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/inputquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/cli.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-04-23 21:17:23.000000 moulti-1.7.0/src/moulti/widgets/inputquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.7.0/src/moulti/widgets/moulticonsole.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.7.0/src/moulti/widgets/moultilog.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.7.0/src/moulti/widgets/quitdialog.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti/widgets/step/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.7.0/src/moulti/widgets/step/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4550 2024-04-23 20:13:13.000000 moulti-1.7.0/src/moulti/widgets/step/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7353 2024-04-28 00:47:55.000000 moulti-1.7.0/src/moulti/widgets/step/tui.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.7.0/src/moulti/widgets/stepcontainer.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.7.0/src/moulti/widgets/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.7.0/src/moulti/widgets/vertscroll.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-28 13:17:18.692666 moulti-1.7.0/src/moulti.egg-info/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4347 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/PKG-INFO
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1534 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/SOURCES.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/dependency_links.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       83 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/entry_points.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       36 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/requires.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-04-28 13:17:18.000000 moulti-1.7.0/src/moulti.egg-info/top_level.txt
```

### Comparing `moulti-1.6.0/LICENSE` & `moulti-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/PKG-INFO` & `moulti-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.6.0
+Version: 1.7.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
 Classifier: Environment :: Console :: Curses
@@ -54,14 +54,15 @@
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
+- an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.6.0/README.md` & `moulti-1.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
+- an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.6.0/pyproject.toml` & `moulti-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/setup.py` & `moulti-1.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 short_description += 'lines emitted by your scripts to visual, collapsible blocks called steps.'
 
 with open('README.md', 'r') as readme:
 	long_description = readme.read()
 
 setup(
 	name='moulti',
-	version='1.6.0',
+	version='1.7.0',
 	description=short_description,
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Xavier G.',
 	author_email='xavier.moulti@kindwolf.org',
 	url='https://github.com/xavierog/moulti',
 	packages=[
 		'moulti',
 		'moulti.widgets',
 		'moulti.widgets.abstractstep',
+		'moulti.widgets.divider',
+		'moulti.widgets.collapsiblestep',
 		'moulti.widgets.step',
 		'moulti.widgets.abstractquestion',
 		'moulti.widgets.buttonquestion',
 		'moulti.widgets.inputquestion',
 	],
 	classifiers=[
 		'Environment :: Console :: Curses',
@@ -39,11 +41,12 @@
 	],
 	license='MIT',
 	keywords=['cli', 'tui', 'curses', 'terminal', 'multiplex', 'script', 'output', 'steps', 'textual', 'collapsible'],
 	package_dir={'': 'src'},
 	install_requires=['textual>=0.53', 'pyperclip', 'argcomplete'],
 	entry_points={
 		'console_scripts': [
-			'moulti = moulti.precli:main'
+			'moulti = moulti.precli:main',
+			'moulti-askpass = moulti.askpass:main',
 		]
 	},
 )
```

### Comparing `moulti-1.6.0/src/moulti/ansi.py` & `moulti-1.7.0/src/moulti/ansi.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/app.py` & `moulti-1.7.0/src/moulti/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import json
 import time
 import asyncio
 import datetime
 import selectors
+import subprocess
 from concurrent.futures import ThreadPoolExecutor
-from typing import Any, Callable, Iterator
+from queue import Queue
+from typing import Any, Callable, Iterator, cast
 from socket import socket as Socket
+from shutil import which
 from time import time_ns, localtime, strftime
 from threading import get_ident, Lock
 from rich.markup import MarkupError
 from textual import work
 from textual.app import App, ComposeResult
 from textual.dom import BadIdentifier
 from textual.widgets import Footer, Label, ProgressBar
@@ -21,40 +24,66 @@
 from .protocol import PRINTABLE_MOULTI_SOCKET, clean_socket, current_instance
 from .protocol import moulti_listen, get_unix_credentials, send_json_message
 from .protocol import MoultiConnectionClosedException, MoultiProtocolException, Message, FDs
 from .protocol import MoultiTLVReader, data_to_message, getraddr
 from .widgets.tui import MoultiWidgets
 from .widgets.stepcontainer import StepContainer
 from .widgets.abstractstep.tui import AbstractStep
+from .widgets.collapsiblestep.tui import CollapsibleStep
+from .widgets.step.tui import Step
 from .widgets.moulticonsole import MoultiConsole
 from .widgets.quitdialog import QuitDialog
 
+
+MOULTI_RUN_OUTPUT_STEP_ID = 'moulti_run_output'
+
 def timestamp() -> str:
 	timestamp_ns = time_ns()
 	timestamp_s = timestamp_ns//10**9
 	ns = timestamp_ns - timestamp_s * 10**9
 	ms = ns // 10**6
 	timestr = strftime('%FT%T', localtime(timestamp_s))
 	timestr = f'{timestr}.{ms:03d} '
 	return timestr
 
+def run_environment(_command: list[str], copy: bool = True) -> dict[str, str]:
+	"""
+	Return environment variables set by "Moulti run <command>".
+	"""
+	environment = os.environ.copy() if copy else {}
+
+	environment['MOULTI_RUN'] = 'moulti'
+	environment['MOULTI_SOCKET_PATH'] = PRINTABLE_MOULTI_SOCKET
+	environment['MOULTI_INSTANCE_PID'] = str(os.getpid())
+
+	if 'SSH_ASKPASS' not in os.environ:
+		environment['SSH_ASKPASS'] = 'moulti-askpass'
+		environment['SSH_ASKPASS_REQUIRE'] = 'force'
+
+	if 'SUDO_ASKPASS' not in os.environ:
+		# sudo requires an absolute path:
+		if moulti_askpass_abspath := which('moulti-askpass'):
+			environment['SUDO_ASKPASS'] = moulti_askpass_abspath
+
+	return environment
+
 class MoultiMessageException(Exception):
 	pass
 
 class Moulti(App):
 	"""
 	moulti is a Terminal User Interface (TUI) meant to display multiple outputs.
 	It is visually similar to https://github.com/dankilman/multiplex but unlike
 	it, moulti does not do anything until instructed to.
 	"""
 	BINDINGS = [
 		("s", "save", "Save"),
 		("n", "toggle_console", "Console"),
-		("x", "expand_all", "Expand all"),
-		("o", "collapse_all", "Collapse all"),
+		("x", "collapse_all(False)", "Expand all"),
+		("o", "collapse_all(True)", "Collapse all"),
 		("d", "toggle_dark", "Dark/Light"),
 		("q", "quit", "Quit"),
 	]
 	# Disable Textual's command palette; it may come back if Moulti ends up with too many commands though:
 	ENABLE_COMMAND_PALETTE = False
 
 	def __init__(self, command: list[str]|None = None):
@@ -139,30 +168,101 @@
 		self.logconsole(f'known widgets: {widget_list}')
 		self.network_loop()
 
 	def network_loop_is_ready(self) -> None:
 		if self.init_command is not None:
 			self.exec(self.init_command)
 
+	def output_policy(self) -> bool|None:
+		"""
+		`moulti run` launches an arbitrary command. In an ideal world, this command should not output anything on
+		stdout/stderr. In practice, this method returns:
+		- None if Moulti should ignore stdout/stderr (default)
+		- False if Moulti should discard stdout/stderr
+		- True if Moulti should harvest stdout/stderr and append it to the "moulti_run_output" step
+		"""
+		policy = None
+		if value := os.environ.get('MOULTI_RUN_OUTPUT'):
+			if value == 'discard':
+				policy = False
+			elif value == 'harvest':
+				policy = True
+		return policy
+
+	def output_policy_popen_args(self) -> dict[str, Any]:
+		"""
+		Return the adequate subprocess.Popen() arguments for `moulti run` based on output_policy().
+		"""
+		policy = self.output_policy()
+		if policy is None: # default/ignore
+			return {'stdout': None, 'stderr': None}
+		if policy: # harvest
+			return {
+				'stdout': subprocess.PIPE,
+				'stderr': subprocess.STDOUT,
+				'text': True,
+				'encoding': 'utf-8',
+				'errors': 'surrogateescape',
+			}
+		# discard:
+		return {'stdout': subprocess.DEVNULL, 'stderr': subprocess.DEVNULL}
+
+	def output_policy_step(self) -> Step:
+		"""
+		Return the step that should display unexpected stdout/stderr lines harvested by `moulti run`.
+		"""
+		step = self.step_from_message({'id': MOULTI_RUN_OUTPUT_STEP_ID})
+		if step is not None:
+			return cast(Step, step)
+		# This should not fail since the id is valid and reserved:
+		step = Step(id=MOULTI_RUN_OUTPUT_STEP_ID, collapsed=False)
+		call = (self.steps_container.add_step, step)
+		self.call_from_thread(call_all, [call])
+		return step
+
+	def output_policy_pass(self, step: Step, filedesc: Any, initial_data: str) -> None:
+		"""
+		Set up the queue and threads necessary to display unexpected stdout/stderr lines harvested by `moulti run`.
+		"""
+		# This method is very similar to Step.cli_action_pass().
+		queue: Queue = Queue()
+		# Helper functions:
+		def reply(**_kwargs: Any) -> None:
+			pass
+		def debug(line: str) -> None:
+			self.logconsole(f'exec: {line}')
+		helpers = {'file_descriptors': [filedesc], 'debug': debug, 'reply': reply}
+		step.append_from_queue(queue, helpers)
+		queue.put_nowait(initial_data)
+		step.append_from_file_descriptor_to_queue(queue, {}, helpers)
+
 	@work(thread=True)
 	def exec(self, command: list[str]) -> None:
+		"""
+		Launch the given command with the assumption it is meant to drive the current Moulti instance.
+		This method is the heart of `moulti run`.
+		"""
 		worker = get_current_worker()
-		import subprocess # pylint: disable=import-outside-toplevel
 		try:
 			self.init_command_running = True
-			environment = os.environ.copy()
-			environment['MOULTI_RUN'] = 'moulti'
-			environment['MOULTI_SOCKET_PATH'] = PRINTABLE_MOULTI_SOCKET
-			environment['MOULTI_INSTANCE_PID'] = str(os.getpid())
 			self.logconsole(f'exec: about to run {command}')
+			popen_args: dict[str, Any] = {'env': run_environment(command), 'stdin': subprocess.DEVNULL}
 			# Not using 'with' because that waits for the process to exit; pylint: disable=consider-using-with
-			process = subprocess.Popen(command, env=environment, stdin=subprocess.DEVNULL)
+			process = subprocess.Popen(command, **popen_args, **self.output_policy_popen_args())
 			self.logconsole(f'exec: {command} launched with PID {process.pid}')
 			returncode = None
+			watch_output = bool(self.output_policy())
 			while not worker.is_cancelled:
+				if watch_output: # Harvest stdout/stderr lines
+					# If the child process outputs anything, pass it to a special step:
+					assert process.stdout is not None # for mypy
+					if (data := process.stdout.read(1)) and (step := self.output_policy_step()):
+						self.output_policy_pass(step, process.stdout, data)
+						# We no longer need to watch output in this loop:
+						watch_output = False
 				returncode = process.poll() # non-blocking wait(), e.g. wait4(process.pid, result_addr, WNOHANG, NULL)
 				if returncode is not None:
 					self.init_command_running = False
 					self.logconsole(f'exec: {command} exited with return code {returncode}')
 					break
 				time.sleep(0.5)
 			if returncode is None:
@@ -199,23 +299,18 @@
 			if worker and not worker.is_cancelled:
 				self.call_from_thread(self.end_user_console.write, line)
 
 	def action_toggle_console(self) -> None:
 		"""Toggle the console."""
 		self.end_user_console.toggle_class('hidden')
 
-	def action_expand_all(self) -> None:
-		"""Expand all steps."""
-		for step in self.all_steps():
-			step.collapsible.collapsed = False
-
-	def action_collapse_all(self) -> None:
+	def action_collapse_all(self, collapsed: bool = True) -> None:
 		"""Collapse all steps."""
-		for step in self.all_steps():
-			step.collapsible.collapsed = True
+		for step in self.steps_container.query('CollapsibleStep').results(CollapsibleStep):
+			step.collapsible.collapsed = collapsed
 
 	async def action_quit(self) -> None:
 		"""Quit Moulti."""
 		if self.init_command is not None and self.init_command_running:
 			message = 'The command passed to "moulti run" is still running.'
 			self.push_screen(QuitDialog(message))
 			return
@@ -324,14 +419,18 @@
 				action = str(message.get('action'))
 				# add/update/delete actions are considered common/standard and are thus handled here:
 				if action == 'add':
 					if step:
 						raise MoultiMessageException(f'id {message.get("id")} already in use')
 					if 'id' not in message:
 						raise MoultiMessageException('missing id')
+					# Users may create the 'moulti_run_output' step but it MUST be a step, not a question or a divider:
+					if message['id'] == MOULTI_RUN_OUTPUT_STEP_ID and message['command'] != 'step':
+						err = f'{MOULTI_RUN_OUTPUT_STEP_ID} is a reserved id that must be assigned to a step'
+						raise MoultiMessageException(err)
 					calls.append((self.steps_container.add_step, command_class(**message)))
 				else:
 					# All other actions require an existing step:
 					if not step:
 						raise MoultiMessageException(f'unknown id: {message.get("id")}')
 					if not isinstance(step, command_class):
 						raise MoultiMessageException(f'{message.get("id")} is not a {command}')
```

### Comparing `moulti-1.6.0/src/moulti/cli.py` & `moulti-1.7.0/src/moulti/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 from .helpers import pint, float_str, send_to_moulti_and_handle_reply
 from .protocol import send_to_moulti, PRINTABLE_MOULTI_SOCKET
 from .protocol import moulti_connect, send_json_message, recv_json_message
 from .widgets.cli import add_cli_arguments
 
 def init(args: dict) -> None:
 	"""Start a new Moulti instance."""
+
+	# Handle --print-env:
+	if args.pop('print_env', False):
+		from .app import run_environment # pylint: disable=import-outside-toplevel
+		environment_variables = run_environment(args['command'], False)
+		for name, value in environment_variables.items():
+			print(f'{name}={value}')
+		sys.exit(0)
+
 	from .app import main as init_moulti # pylint: disable=import-outside-toplevel
 	init_moulti(**args)
 
 def wait(verbose: bool = False, delay: int = 500, max_attempts: int = 0) -> None:
 	"""Wait until the Moulti instance is available.
 	Args:
 		verbose: if True, output the reason why each connection attempt failed
@@ -102,14 +111,15 @@
 	# moulti init
 	init_parser = subparsers.add_parser('init', help='Start a new Moulti instance.')
 	init_parser.set_defaults(func=init)
 
 	# moulti run
 	run_parser = subparsers.add_parser('run', help='Start a new Moulti instance and run a command')
 	run_parser.set_defaults(func=init)
+	run_parser.add_argument('--print-env', action='store_true', default=False, help='print environment variables set by Moulti and exit')
 	run_parser.add_argument('command', type=str, nargs='+', help='command to run along with its arguments')
 
 	# moulti wait
 	wait_parser = subparsers.add_parser('wait', help='Wait until the Moulti instance is available.')
 	wait_parser.set_defaults(func=wait)
 	wait_parser.add_argument('--verbose', '-v', action='store_true', help='if True, output the reason why each connection attempt failed')
 	wait_parser.add_argument('--delay', '-d', type=pint, default=500, help='number of milliseconds between two connection attempts')
```

### Comparing `moulti-1.6.0/src/moulti/helpers.py` & `moulti-1.7.0/src/moulti/helpers.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/precli.py` & `moulti-1.7.0/src/moulti/precli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/protocol.py` & `moulti-1.7.0/src/moulti/protocol.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/abstractquestion/cli.py` & `moulti-1.7.0/src/moulti/widgets/abstractquestion/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from moulti.helpers import Args, handle_reply
 from moulti.protocol import send_to_moulti
-from ..abstractstep.cli import add_abstractstep_options
+from ..collapsiblestep.cli import add_collapsiblestep_options
 
 def add_abstractquestion_options(parser: ArgumentParser, none: bool = False) -> None:
-	add_abstractstep_options(parser, none)
+	add_collapsiblestep_options(parser, none)
 	parser.add_argument('--text', '-t', type=str, default=None if none else '', help='Question text')
 
 def question_get_answer(args: Args) -> None:
 	reply = send_to_moulti(args)
 	assert reply is not None
 	answer = reply.get('answer')
 	if answer is not None:
```

### Comparing `moulti-1.6.0/src/moulti/widgets/abstractquestion/tui.py` & `moulti-1.7.0/src/moulti/widgets/abstractquestion/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any
 from textual import work
 from textual.app import ComposeResult
 from textual.message import Message
 from textual.widget import Widget
 from textual.widgets import Static
-from ..abstractstep.tui import AbstractStep
+from ..collapsiblestep.tui import CollapsibleStep
 
-class AbstractQuestion(AbstractStep):
+class AbstractQuestion(CollapsibleStep):
 	"""
 	This widget represents an interactive question in a script, program or process.
 	"""
 	def __init__(self, id: str, **kwargs: str|int|bool): # pylint: disable=redefined-builtin
 		self.question_label = Static('', classes='question_text')
 		self.answer: str|None = None
 		self.waiting: list[Any] = []
```

### Comparing `moulti-1.6.0/src/moulti/widgets/abstractstep/cli.py` & `moulti-1.7.0/src/moulti/widgets/collapsiblestep/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from argparse import ArgumentParser, BooleanOptionalAction
-from moulti.helpers import bool_or_int
+from ..abstractstep.cli import add_abstractstep_options
 
-def add_abstractstep_options(parser: ArgumentParser, none: bool = False) -> None:
+def add_collapsiblestep_options(parser: ArgumentParser, none: bool = False) -> None:
 	"""Options common to step add (with actual default values) and step update (with None default values)."""
-	parser.add_argument('--title', type=str, default=None, help='step title, always visible')
+	add_abstractstep_options(parser, none)
+	parser.add_argument('--collapsed', action=BooleanOptionalAction, default=None if none else False, help='whether to collapse the step')
 	parser.add_argument('--top-text', '-tt', type=str, default=None if none else '', help='line of text displayed above the content')
 	parser.add_argument('--bottom-text', '-bt', type=str, default=None if none else '', help='line of text displayed below the content')
-	parser.add_argument('--classes', '-c', type=str, default=None if none else 'standard', help='step class (color): standard, error, warning, success')
-	parser.add_argument('--collapsed', action=BooleanOptionalAction, default=None if none else False, help='whether to collapse the step')
-	parser.add_argument('--scroll-on-activity', type=bool_or_int, default=None if none else False, help='whether to scroll to this step upon activity', metavar='{true,false,...,-2,-1,0,1,2,...}')
```

### Comparing `moulti-1.6.0/src/moulti/widgets/abstractstep/tui.py` & `moulti-1.7.0/src/moulti/widgets/step/tui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,209 @@
-import json
-from operator import attrgetter
+import os
+from queue import Queue
 from typing import Any, Callable
-from pyperclip import copy # type: ignore
-from rich.errors import MarkupError
+from textual import work
 from textual.app import ComposeResult
-from textual.events import Click
-from textual.message import Message
-from textual.widgets import Static, Collapsible
+from textual.worker import get_current_worker
+from rich.text import Text
+from ..collapsiblestep.tui import CollapsibleStep
+from ..moultilog import MoultiLog
 
-class AbstractStep(Static):
+ANSI_ESCAPE_SEQUENCE = '\x1b'
+
+class Step(CollapsibleStep):
 	"""
-	This is the base class for all components end users may wish to add to Moulti.
+	This widget represents a step in a script, program or process.
+	Visually speaking, it is essentially a collapsible text area surrounded
+	with optional text lines.
 	"""
 
-	class StepActivity(Message):
-		def __init__(self, step: 'AbstractStep', *args: Any, **kwargs: Any):
-			self.step = step
-			super().__init__(*args, **kwargs)
-
-	def __init__(self, id: str, **kwargs: Any): # pylint: disable=redefined-builtin
-		self.collapsible = Collapsible(title=id)
-		self.top_label = Static('', classes='top_text')
-		self.bottom_label = Static('', classes='bottom_text')
-
-		self.top_text = ''
-		self.bottom_text = ''
-
-		# This attribute is meant to prevent deletion of a step while content
-		# is being appended to it:
-		self.prevent_deletion = 0
+	BINDINGS = [
+		("c", "to_clipboard(False)", "Copy"),
+		("w", "to_clipboard(True)", "With colors"),
+	]
 
-		self.scroll_on_activity: bool|int = False
+	def __init__(self, id: str, **kwargs: str|int|bool): # pylint: disable=redefined-builtin
+		self.log_widget = MoultiLog(highlight=False)
 
-		self.check_properties(kwargs)
-		self.init_kwargs = kwargs
+		self.min_height = 1
+		self.max_height = 25
 
-		step_classes = str(kwargs.get('classes', ''))
-		super().__init__(id='step_' + id, classes=step_classes)
+		super().__init__(id=id, **kwargs)
 
-	def subcompose(self) -> ComposeResult:
-		return []
+		self.color = ''
 
-	def compose(self) -> ComposeResult:
-		with self.collapsible:
-			yield self.top_label
-			yield from self.subcompose()
-			yield self.bottom_label
-
-	def on_mount(self) -> None:
-		self.query_one('CollapsibleTitle').tooltip = f'Step id: {self.title_from_id()}'
-		self.update_properties(self.init_kwargs)
-
-	async def on_click(self, _: Click) -> None:
-		"""
-		Steps are meant to be focusable but it is actually the CollapsibleTitle that holds the focus.
-		"""
-		self.query_one('CollapsibleTitle').focus()
-
-	def title_from_id(self) -> str:
-		self_id = str(self.id)
-		if '_' not in self_id:
-			return self_id
-		return self_id.split('_', 1)[1]
-
-	def index(self) -> int:
-		if self.parent is not None:
-			return sorted(self.parent.children, key=attrgetter('sort_order')).index(self) + 1
-		return -1
-
-	def check_markup(self, value: str|int|bool) -> None:
-		value = str(value)
-		text = self.render_str(value)
-		# Extra check to work around https://github.com/Textualize/textual/issues/4248:
-		for span in text.spans:
-			if hasattr(span.style, 'meta') and span.style.meta.get('@click') == ():
-				raise MarkupError('problematic @click tag')
-
-	def check_markup_dict(self, check_dict: dict[str, str|int|bool], *keys: str) -> None:
-		for key in keys:
-			if key in check_dict:
-				self.check_markup(check_dict[key])
+	def cli_action_append(self, kwargs: dict[str, Any], helpers: dict[str, Any]) -> tuple:
+		if 'text' not in kwargs:
+			helpers['reply'](done=False, error='missing text for append operation')
+			return ()
+		return self.append, '\n'.join(kwargs['text'])
 
-	def check_properties(self, kwargs: dict[str, str|int|bool]) -> None:
-		self.check_markup_dict(kwargs, 'title', 'top_text', 'bottom_text')
+	def cli_action_clear(self, _kwargs: dict[str, str|int|bool], _helpers: dict[str, Any]) -> tuple:
+		return self.clear, # pylint: disable=trailing-comma-tuple
+
+	def subcompose(self) -> ComposeResult:
+		yield self.log_widget
 
 	def update_properties(self, kwargs: dict[str, str|int|bool]) -> None:
-		if 'classes' in kwargs:
-			self.set_classes(str(kwargs['classes']))
-		if 'title' in kwargs:
-			self.collapsible.title = str(kwargs['title']) if kwargs['title'] else self.title_from_id()
-		if 'collapsed' in kwargs:
-			self.collapsible.collapsed = bool(kwargs['collapsed'])
-		if 'top_text' in kwargs:
-			self.top_text = str(kwargs['top_text'])
-			self.top_label.update(self.top_text)
-		self.top_label.styles.display = 'block' if self.top_text else 'none'
-		if 'bottom_text' in kwargs:
-			self.bottom_text = str(kwargs['bottom_text'])
-			self.bottom_label.update(self.bottom_text)
-		self.bottom_label.styles.display = 'block' if self.bottom_text else 'none'
-		if 'scroll_on_activity' in kwargs:
-			scroll_on_activity = kwargs['scroll_on_activity']
-			if isinstance(scroll_on_activity, int):
-				self.scroll_on_activity = scroll_on_activity
-			else:
-				self.scroll_on_activity = bool(scroll_on_activity)
+		super().update_properties(kwargs)
+		if 'text' in kwargs:
+			self.clear()
+			self.append(str(kwargs['text']))
+		if 'min_height' in kwargs:
+			self.min_height = int(kwargs['min_height'])
+		if 'max_height' in kwargs:
+			self.max_height = int(kwargs['max_height'])
+		self.log_widget.styles.min_height = self.min_height
+		self.log_widget.styles.max_height = self.max_height if self.max_height > 0 else None
 
 	def export_properties(self) -> dict[str, Any]:
-		prop: dict[str, Any] = {}
-		prop['id'] = self.title_from_id()
-		prop['classes'] = ' '.join(self.classes)
-		prop['title'] = self.collapsible.title
-		prop['collapsed'] = self.collapsible.collapsed
-		prop['top_text'] = self.top_text
-		prop['bottom_text'] = self.bottom_text
-		prop['scroll_on_activity'] = self.scroll_on_activity
+		prop = super().export_properties()
+		prop['min_height'] = self.min_height
+		prop['max_height'] = self.max_height
 		return prop
 
 	def save(self, opener: Callable[[str, int], int], filename: str, extra_properties: dict[str, Any]) -> None:
-		properties = {**extra_properties, **self.export_properties()}
-		with open(filename + '.properties.json', 'w', encoding='utf-8', opener=opener) as properties_filedesc:
-			json.dump(properties, properties_filedesc, indent=4)
-			properties_filedesc.write('\n')
-
-	def notify_copy_to_clipboard(self, result: bool, explanation: str) -> None:
-		step_index = self.index()
-		title = f'Step #{step_index} copied!' if result else f'Failed to copy step #{step_index}'
-		if explanation:
-			message = explanation
-		elif result:
-			message = f'Step #{step_index} copied to clipboard'
-		else:
-			message = f'Could not copy step #{step_index} to clipboard'
-		self.app.notify(message, title=title, severity='information' if result else 'error')
-
-	@staticmethod
-	def copy_to_clipboard(func: Callable) -> Callable:
-		def wrapper(self: AbstractStep, *args: Any, **kwargs: Any) -> None:
-			try:
-				result, data, explanation = func(self, *args, **kwargs)
-				if result:
-					copy(data)
-			except Exception as exc:
-				result, explanation = False, str(exc)
-			self.notify_copy_to_clipboard(result, explanation)
-		return wrapper
-
-	def activity(self) -> None:
-		msg = AbstractStep.StepActivity(self)
-		self.call_after_refresh(self.post_message, msg)
-
-	DEFAULT_COLORS = """
-	$step_default: $primary;
-	$step_success: ansi_bright_green;
-	$step_warning: orange;
-	$step_error: tomato;
-	"""
-	DEFAULT_CSS = DEFAULT_COLORS + """
-	AbstractStep {
-		/* If we do not specify "auto" here, each step will take 100% of the viewport: */
-		height: auto;
-		background: $step_default;
-		border-left: blank;
-		color: auto;
-		&.success { background: $step_success; }
-		&.warning { background: $step_warning; }
-		&.error { background: $step_error; }
-		/* Compact design: no padding, no margins, no borders: */
-		& Collapsible {
-			/* Inherit the parent background instead of altering it via $boost: */
-			background: initial;
-			padding: 0;
-			margin: 0;
-			border: none;
-		}
-		& CollapsibleTitle {
-			padding: 0;
-			width: 100%;
+		super().save(opener, filename, extra_properties)
+		filename = filename + '.contents.log'
+		with open(filename, 'w', encoding='utf-8', errors='surrogateescape', opener=opener) as contents_filedesc:
+			self.log_widget.to_file(contents_filedesc)
+
+	@CollapsibleStep.copy_to_clipboard
+	def action_to_clipboard(self, keep_styles: bool = True) -> tuple[bool, str, str]:
+		lines = list(self.log_widget.to_lines(keep_styles))
+		lines_count = len(lines)
+		lines.append('') # add an extra \n
+		data = '\n'.join(lines)
+		return True, data, f'copied {lines_count} lines, {len(data)} characters to clipboard'
+
+	def clear(self) -> None:
+		self.log_widget.clear()
+		self.color = ''
+
+	def append(self, text: str) -> None:
+		# RichLog does not handle partial lines and thus always adds a trailing \n; therefore, we must strip one (and
+		# only one) trailing \n, if present:
+		if text and text[-1] == '\n':
+			text = text[:-1]
+		# If necessary, prepend the ANSI escape code for the color inherited from the last line:
+		if self.color:
+			text = self.color + text
+		# Deal with colored text; the text_to_write variable is made necessary by mypy.
+		text_to_write: str | Text = text
+		if ANSI_ESCAPE_SEQUENCE in text:
+			# Convert text and an extra character from ANSI to Rich Text
+			text_to_write = Text.from_ansi(text + '_')
+			# The extra character reflects the color the next line should inherit:
+			self.color = Step.last_character_color(text_to_write)
+			# Strip the extra character:
+			text_to_write.right_crop(1)
+		self.log_widget.write(text_to_write)
+		self.activity()
+
+	@classmethod
+	def last_character_color(cls, text: Text) -> str:
+		# If the last span (if any) covers the last character...
+		if text.spans and text.spans[-1].end == len(text):
+			# ... return the ANSI escape code for its color:
+			style = text.spans[-1].style
+			assert not isinstance(style, str) # prevent calling render() on str
+			return style.render('_').split('_')[0]
+		return ''
+
+	def cli_action_pass(self, kwargs: dict[str, str|int|bool], helpers: dict[str, Any]) -> tuple:
+		if not helpers['file_descriptors']:
+			helpers['reply'](done=False, error='missing file descriptor for pass operation')
+			return ()
+		# Set up a queue between two workers:
+		# - one that reads data from the file descriptor and replies to the client;
+		# - one that appends lines to the step.
+		queue: Queue = Queue()
+		self.append_from_queue(queue, helpers)
+		self.append_from_file_descriptor_to_queue(queue, kwargs, helpers)
+		return ()
+
+	@work(thread=True)
+	async def append_from_file_descriptor_to_queue(
+		self,
+		queue: Queue,
+		kwargs: dict[str, Any],
+		helpers: dict[str, Any],
+	) -> None:
+		current_worker = get_current_worker()
+		error = None
+		try:
+			file_desc = helpers['file_descriptors'][0]
+			# Read lines from the given file descriptor:
+			if isinstance(file_desc, int):
+				actual_file_desc = os.fdopen(file_desc, encoding='utf-8', errors='surrogateescape')
+			else:
+				actual_file_desc = file_desc
+			with actual_file_desc as text_io:
+				# Syscall-wise, Python will read(fd, buffer, count) where count = max(8192, read_size) - read_bytes.
+				# But it will NOT return anything unless it has reached the hinted read size.
+				# Out of the box, Moulti should strive to display lines as soon as possible, hence the default value of
+				# 1. It remains possible to specify a larger value, e.g. when one knows there are going to be many
+				# lines over a short timespan, e.g. "find / -ls".
+				read_size = int(kwargs.get('read_size', 1))
+				while data := text_io.read(read_size):
+					if current_worker.is_cancelled:
+						break
+					queue.put_nowait(data)
+				queue.put_nowait(None)
+		except Exception as exc:
+			error = str(exc)
+			helpers['debug'](f'pass: {error}')
+		helpers['reply'](done=error is None, error=error)
+
+	@work(thread=True)
+	async def append_from_queue(self, queue: Queue, helpers: dict[str, Any]) -> None:
+		current_worker = get_current_worker()
+		self.prevent_deletion += 1
+		try:
+			buffer = []
+			while True:
+				if current_worker.is_cancelled:
+					break
+				data = queue.get()
+				if data is not None:
+					# Buffer data to avoid queuing partial lines as, down the
+					# line, RichLog.write() only handles complete lines:
+					# look for the position of \n from the end of the string :
+					eol = data.rfind('\n')
+					if eol == -1: # no \n found, buffer the whole string:
+						buffer.append(data)
+					else:
+						before = data[:eol]
+						after = data[eol+1:]
+						buffer.append(before)
+						self.app.call_from_thread(self.append, ''.join(buffer))
+						buffer.clear()
+						if after:
+							buffer.append(after)
+				else:
+					# Reached EOF: flush buffer and signal EOF:
+					if buffer:
+						self.app.call_from_thread(self.append, ''.join(buffer))
+					break
+		except Exception as exc:
+			helpers['debug'](f'append_from_queue: {exc}')
+		finally:
+			self.prevent_deletion -= 1
+
+	DEFAULT_CSS = CollapsibleStep.DEFAULT_CSS + """
+	Step {
+		& MoultiLog {
+			scrollbar-corner-color: $step_default;
 		}
-		& CollapsibleTitle:focus {
-			background: initial;
+		&.success {
+			& MoultiLog { scrollbar-corner-color: $step_success; }
 		}
-		& CollapsibleTitle:hover {
-			background: $foreground 80%;
+		&.warning {
+			& MoultiLog { scrollbar-corner-color: $step_warning; }
 		}
-		/* Collapsible contents: */
-		& Contents {
-			/* Leave some space on each side of the contents: */
-			padding-left: 2 !important;
-			padding-right: 1 !important;
+		&.error {
+			& MoultiLog { scrollbar-corner-color: $step_error; }
 		}
 	}
-	AbstractStep:focus, AbstractStep:focus-within {
-		border-left: thick $accent-lighten-3;
-	}
 	"""
+MoultiWidgetClass = Step
```

### Comparing `moulti-1.6.0/src/moulti/widgets/buttonquestion/cli.py` & `moulti-1.7.0/src/moulti/widgets/buttonquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/buttonquestion/tui.py` & `moulti-1.7.0/src/moulti/widgets/buttonquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/inputquestion/cli.py` & `moulti-1.7.0/src/moulti/widgets/inputquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/inputquestion/tui.py` & `moulti-1.7.0/src/moulti/widgets/inputquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/moulticonsole.py` & `moulti-1.7.0/src/moulti/widgets/moulticonsole.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/moultilog.py` & `moulti-1.7.0/src/moulti/widgets/moultilog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/quitdialog.py` & `moulti-1.7.0/src/moulti/widgets/quitdialog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/step/cli.py` & `moulti-1.7.0/src/moulti/widgets/step/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from argparse import ArgumentParser, _SubParsersAction
 from moulti.helpers import Args, pint, handle_reply
 from moulti.helpers import send_to_moulti_and_handle_reply, send_no_none_to_moulti_and_handle_reply
 from moulti.protocol import moulti_connect, send_json_message, recv_json_message
-from ..abstractstep.cli import add_abstractstep_options
+from ..collapsiblestep.cli import add_collapsiblestep_options
 
 COMMAND = 'step'
 
 def add_cli_arguments(subparsers: _SubParsersAction) -> None:
 	# moulti step:
 	step_parser = subparsers.add_parser(COMMAND, help='Create and manage steps shown by Moulti.')
 	step_subparsers = step_parser.add_subparsers(required=True)
@@ -50,15 +50,15 @@
 	pass_parser.set_defaults(func=pass_stdin)
 	pass_parser.add_argument('id', type=str, help='unique identifier')
 	pass_parser.add_argument('--append', '--no-clear', '-a', dest='append', action='store_true', help='do not clear the target step')
 	pass_parser.add_argument('--read-size', '-rs', dest='read_size', type=pint, default=1, help='read size')
 
 def add_step_options(parser: ArgumentParser, none: bool = False) -> None:
 	"""Options common to step add (with actual default values) and step update (with None default values)."""
-	add_abstractstep_options(parser, none)
+	add_collapsiblestep_options(parser, none)
 	parser.add_argument('--text', '-t', type=str, default=None if none else '', help='content')
 	parser.add_argument('--min-height', '-mh', type=pint, default=None if none else  1, help='minimum content height')
 	parser.add_argument('--max-height', '-Mh', type=pint, default=None if none else 25, help='maximum content height; 0 to disable')
 
 def pass_stdin(args: Args) -> None:
 	"""Pass the stdin file descriptor to Moulti and inject everything read from it into a given step."""
 	moulti_socket = moulti_connect()
```

### Comparing `moulti-1.6.0/src/moulti/widgets/stepcontainer.py` & `moulti-1.7.0/src/moulti/widgets/stepcontainer.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti/widgets/tui.py` & `moulti-1.7.0/src/moulti/widgets/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.6.0/src/moulti.egg-info/PKG-INFO` & `moulti-1.7.0/src/moulti.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.6.0
+Version: 1.7.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
 Classifier: Environment :: Console :: Curses
@@ -54,14 +54,15 @@
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
 Moulti also features:
 - a **progress bar**: [documentation](Documentation.md#progress-bar)
 - programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
+- an askpass helper named `moulti-askpass`: [documentation](Documentation.md#moulti-run-dealing-with-ssh)
 
 When it comes to look and feel, Moulti can be customised:
 
 - through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
```

### Comparing `moulti-1.6.0/src/moulti.egg-info/SOURCES.txt` & `moulti-1.7.0/src/moulti.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 src/moulti/__init__.py
 src/moulti/__main__.py
 src/moulti/ansi.py
 src/moulti/app.py
+src/moulti/askpass.py
 src/moulti/cli.py
 src/moulti/helpers.py
 src/moulti/precli.py
 src/moulti/protocol.py
 src/moulti.egg-info/PKG-INFO
 src/moulti.egg-info/SOURCES.txt
 src/moulti.egg-info/dependency_links.txt
@@ -29,13 +30,19 @@
 src/moulti/widgets/abstractquestion/tui.py
 src/moulti/widgets/abstractstep/__init__.py
 src/moulti/widgets/abstractstep/cli.py
 src/moulti/widgets/abstractstep/tui.py
 src/moulti/widgets/buttonquestion/__init__.py
 src/moulti/widgets/buttonquestion/cli.py
 src/moulti/widgets/buttonquestion/tui.py
+src/moulti/widgets/collapsiblestep/__init__.py
+src/moulti/widgets/collapsiblestep/cli.py
+src/moulti/widgets/collapsiblestep/tui.py
+src/moulti/widgets/divider/__init__.py
+src/moulti/widgets/divider/cli.py
+src/moulti/widgets/divider/tui.py
 src/moulti/widgets/inputquestion/__init__.py
 src/moulti/widgets/inputquestion/cli.py
 src/moulti/widgets/inputquestion/tui.py
 src/moulti/widgets/step/__init__.py
 src/moulti/widgets/step/cli.py
 src/moulti/widgets/step/tui.py
```

