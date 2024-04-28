# Comparing `tmp/pytigon-gui-0.240302.tar.gz` & `tmp/pytigon-gui-0.240428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-gui-0.240302.tar", last modified: Sat Mar  2 14:25:48 2024, max compression
+gzip compressed data, was "pytigon-gui-0.240428.tar", last modified: Sun Apr 28 17:14:13 2024, max compression
```

## Comparing `pytigon-gui-0.240302.tar` & `pytigon-gui-0.240428.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.672830 pytigon-gui-0.240302/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/LICENSE
--rw-r--r--   0 sch       (1000) sch       (1000)     1256 2024-03-02 14:25:48.672830 pytigon-gui-0.240302/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       13 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.664830 pytigon-gui-0.240302/pytigon_gui/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/__init__.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.664830 pytigon-gui-0.240302/pytigon_gui/guictrl/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8763 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/basectrl.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.664830 pytigon-gui-0.240302/pytigon_gui/guictrl/button/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/button/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3421 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/button/toolbarbutton.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    72521 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/ctrl.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.668830 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    29337 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/grid.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8655 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridpanel.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10888 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_base.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    15506 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_from_html_table.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    15999 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_from_proxy.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6772 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/popupcelleditors.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8379 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/renderers.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6564 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/grid/tabproxy.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.668830 pytigon-gui-0.240302/pytigon_gui/guictrl/popup/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/popup/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9819 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/popup/popuphtml.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    11505 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/popup/select2.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25501 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guictrl/tag.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.668830 pytigon-gui-0.240302/pytigon_gui/guiframe/
--rw-rw-r--   0 sch       (1000) sch       (1000)     1104 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    44711 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/appframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4204 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/baseframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3551 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/browserframe.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    44314 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/form.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2137 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/manager.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8187 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/notebook.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    18048 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/notebookpage.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19288 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guiframe/page.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.668830 pytigon-gui-0.240302/pytigon_gui/guilib/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2441 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/events.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3320 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/httperror.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9834 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/image.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2490 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/logindialog.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3934 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/pytigon_install.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2182 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/signal.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4967 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/threadwindow.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4321 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1653 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/guilib/websocket.py
--rwxrwxr-x   0 sch       (1000) sch       (1000)    47471 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/pytigon.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.672830 pytigon-gui-0.240302/pytigon_gui/toolbar/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14182 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/basetoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5910 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/generictoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2498 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/menubar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16934 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/moderntoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4498 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/standardtoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25006 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/standardtoolbarbuttons.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10675 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/toolbar/treetoolbar.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6692 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/pytigon_gui/wxauto.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-03-02 14:25:48.672830 pytigon-gui-0.240302/pytigon_gui.egg-info/
--rw-r--r--   0 sch       (1000) sch       (1000)     1256 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)     1935 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       46 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/entry_points.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       79 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       12 2024-03-02 14:25:48.000000 pytigon-gui-0.240302/pytigon_gui.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       80 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/requirements.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-03-02 14:25:48.672830 pytigon-gui-0.240302/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     1917 2024-03-02 14:22:06.000000 pytigon-gui-0.240302/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.956836 pytigon-gui-0.240428/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/LICENSE
+-rw-r--r--   0 sch       (1000) sch       (1000)     1256 2024-04-28 17:14:13.956836 pytigon-gui-0.240428/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       13 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.944836 pytigon-gui-0.240428/pytigon_gui/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/__init__.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.948836 pytigon-gui-0.240428/pytigon_gui/guictrl/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8763 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/basectrl.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.948836 pytigon-gui-0.240428/pytigon_gui/guictrl/button/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/button/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3421 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/button/toolbarbutton.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    72521 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/ctrl.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.948836 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    29337 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/grid.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8655 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridpanel.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10888 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_base.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    15506 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_from_html_table.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    15999 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_from_proxy.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6772 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/popupcelleditors.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8379 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/renderers.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6564 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/grid/tabproxy.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.948836 pytigon-gui-0.240428/pytigon_gui/guictrl/popup/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/popup/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9819 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/popup/popuphtml.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    11505 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/popup/select2.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25501 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guictrl/tag.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.952836 pytigon-gui-0.240428/pytigon_gui/guiframe/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1104 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    44711 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/appframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4204 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/baseframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3551 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/browserframe.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    44314 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/form.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2137 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/manager.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8187 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/notebook.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    18048 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/notebookpage.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19288 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guiframe/page.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.952836 pytigon-gui-0.240428/pytigon_gui/guilib/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2441 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/events.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3320 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/httperror.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9834 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/image.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2490 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/logindialog.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3934 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/pytigon_install.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2182 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/signal.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4967 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/threadwindow.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4321 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1653 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/guilib/websocket.py
+-rwxrwxr-x   0 sch       (1000) sch       (1000)    47471 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/pytigon.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.956836 pytigon-gui-0.240428/pytigon_gui/toolbar/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14182 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/basetoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5910 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/generictoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2498 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/menubar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16934 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/moderntoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4498 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/standardtoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25006 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/standardtoolbarbuttons.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10675 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/toolbar/treetoolbar.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6692 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/pytigon_gui/wxauto.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:14:13.956836 pytigon-gui-0.240428/pytigon_gui.egg-info/
+-rw-r--r--   0 sch       (1000) sch       (1000)     1256 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1935 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       46 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       79 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       12 2024-04-28 17:14:13.000000 pytigon-gui-0.240428/pytigon_gui.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       80 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/requirements.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-04-28 17:14:13.956836 pytigon-gui-0.240428/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1917 2024-04-28 17:09:49.000000 pytigon-gui-0.240428/setup.py
```

### Comparing `pytigon-gui-0.240302/LICENSE` & `pytigon-gui-0.240428/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/PKG-INFO` & `pytigon-gui-0.240428/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-gui
-Version: 0.240302
+Version: 0.240428
 Summary: Pytigon GUI
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pytigon-gui-0.240302/pytigon_gui/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/basectrl.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/basectrl.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/button/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/button/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/button/toolbarbutton.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/button/toolbarbutton.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/ctrl.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/ctrl.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/grid.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/grid.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridpanel.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridpanel.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_base.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_base.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_from_html_table.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_from_html_table.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/gridtable_from_proxy.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/gridtable_from_proxy.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/popupcelleditors.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/popupcelleditors.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/renderers.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/renderers.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/grid/tabproxy.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/grid/tabproxy.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/popup/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/popup/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/popup/popuphtml.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/popup/popuphtml.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/popup/select2.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/popup/select2.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guictrl/tag.py` & `pytigon-gui-0.240428/pytigon_gui/guictrl/tag.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/appframe.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/appframe.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/baseframe.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/baseframe.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/browserframe.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/browserframe.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/form.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/form.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/manager.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/manager.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/notebook.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/notebook.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/notebookpage.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/notebookpage.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guiframe/page.py` & `pytigon-gui-0.240428/pytigon_gui/guiframe/page.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/events.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/events.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/httperror.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/httperror.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/image.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/image.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/logindialog.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/logindialog.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/pytigon_install.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/pytigon_install.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/signal.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/signal.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/threadwindow.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/threadwindow.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/tools.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/guilib/websocket.py` & `pytigon-gui-0.240428/pytigon_gui/guilib/websocket.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/pytigon.py` & `pytigon-gui-0.240428/pytigon_gui/pytigon.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/__init__.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/basetoolbar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/basetoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/generictoolbar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/generictoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/menubar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/menubar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/moderntoolbar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/moderntoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/standardtoolbar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/standardtoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/standardtoolbarbuttons.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/standardtoolbarbuttons.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/toolbar/treetoolbar.py` & `pytigon-gui-0.240428/pytigon_gui/toolbar/treetoolbar.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui/wxauto.py` & `pytigon-gui-0.240428/pytigon_gui/wxauto.py`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/pytigon_gui.egg-info/PKG-INFO` & `pytigon-gui-0.240428/pytigon_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-gui
-Version: 0.240302
+Version: 0.240428
 Summary: Pytigon GUI
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pytigon-gui-0.240302/pytigon_gui.egg-info/SOURCES.txt` & `pytigon-gui-0.240428/pytigon_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytigon-gui-0.240302/setup.py` & `pytigon-gui-0.240428/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     tmp = f.read().strip().split("\n")
     install_requires = [pos for pos in tmp if "://" not in pos]
     dependency_links = [pos for pos in tmp if "://" in pos]
 
 
 setup(
     name="pytigon-gui",
-    version="0.240302",
+    version="0.240428",
     description="Pytigon GUI",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={"": extra_files},
     install_requires=install_requires,
```

