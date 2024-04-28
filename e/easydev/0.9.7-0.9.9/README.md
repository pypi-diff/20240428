# Comparing `tmp/easydev-0.9.7.tar.gz` & `tmp/easydev-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easydev-0.9.7.tar", last modified: Mon Nov 30 20:14:29 2015, max compression
+gzip compressed data, was "dist/easydev-0.9.9.tar", last modified: Tue Jan 12 21:23:11 2016, max compression
```

## Comparing `easydev-0.9.7.tar` & `easydev-0.9.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       54 2014-08-18 07:57:06.000000 easydev-0.9.7/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3620 2015-11-30 20:10:19.000000 easydev-0.9.7/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2456 2014-08-18 07:57:06.000000 easydev-0.9.7/share/copybutton.js
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/themes/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/themes/standard/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3740 2014-09-05 09:25:10.000000 easydev-0.9.7/share/themes/standard/layout.html
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/themes/standard/static/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      897 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/static/warning.jpg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      430 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/static/bgtop.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14130 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/static/software.css_t
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      434 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/static/bgfooter.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      623 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/google_footer.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      515 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/indexsidebar.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       64 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/index.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      481 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/standard/theme.conf
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      257 2014-12-10 09:39:24.000000 easydev-0.9.7/share/themes/standard/google_head.html
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/themes/cno/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4426 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/layout.html
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/share/themes/cno/static/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      897 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/static/warning.jpg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      430 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/static/bgtop.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14149 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/static/software.css_t
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      434 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/static/bgfooter.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      623 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/google_footer.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      515 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/indexsidebar.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       64 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/index.html
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      481 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/theme.conf
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2014-08-18 07:57:06.000000 easydev-0.9.7/share/themes/cno/google_head.html
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      148 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_dependencies.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      644 2014-08-30 08:42:50.000000 easydev-0.9.7/test/test_decorators.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      488 2015-06-18 07:33:06.000000 easydev-0.9.7/test/test_easytest.py
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)      239 2015-11-03 14:52:38.000000 easydev-0.9.7/test/test_browse.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2497 2015-09-10 09:29:05.000000 easydev-0.9.7/test/test_config.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      609 2015-10-16 08:18:01.000000 easydev-0.9.7/test/test_progressbar.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      570 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_multicore.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      422 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_copybutton.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      707 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_paths.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      333 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_package.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      741 2015-11-12 20:46:00.000000 easydev-0.9.7/test/test_codecs.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       89 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_setuptools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2015-06-19 13:21:24.000000 easydev-0.9.7/test/test_lsf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2015-01-05 13:42:47.000000 easydev-0.9.7/test/test_multigit.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2877 2015-01-05 14:16:32.000000 easydev-0.9.7/test/test_tools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      363 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_console.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      454 2015-10-16 07:28:34.000000 easydev-0.9.7/test/test_url.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       83 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_doc.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      572 2015-11-12 20:46:00.000000 easydev-0.9.7/test/test_misc.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      234 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_cnolab_sphinx.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      456 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_logging_tools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2255 2014-08-18 07:57:06.000000 easydev-0.9.7/test/test_multisetup.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4105 2015-11-30 20:14:29.000000 easydev-0.9.7/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2707 2015-11-20 11:18:56.000000 easydev-0.9.7/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      325 2015-11-30 20:14:29.000000 easydev-0.9.7/setup.cfg
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/src/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/src/easydev/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3278 2014-09-10 08:34:27.000000 easydev-0.9.7/src/easydev/console.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     7647 2015-11-30 20:09:52.000000 easydev-0.9.7/src/easydev/tools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1539 2014-09-10 08:39:03.000000 easydev-0.9.7/src/easydev/sphinx_themes.py
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     6253 2015-01-05 14:43:54.000000 easydev-0.9.7/src/easydev/multigit.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5363 2015-11-21 12:44:05.000000 easydev-0.9.7/src/easydev/progressbar.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1458 2015-08-24 14:42:41.000000 easydev-0.9.7/src/easydev/misc.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2988 2014-09-10 08:38:13.000000 easydev-0.9.7/src/easydev/logging_tools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4646 2014-09-10 08:35:14.000000 easydev-0.9.7/src/easydev/copybutton.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13062 2014-12-10 13:14:04.000000 easydev-0.9.7/src/easydev/package.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1721 2015-11-20 11:51:23.000000 easydev-0.9.7/src/easydev/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      908 2014-09-10 08:36:36.000000 easydev-0.9.7/src/easydev/dependencies.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1006 2015-01-26 10:23:43.000000 easydev-0.9.7/src/easydev/doc.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13020 2014-12-10 14:06:30.000000 easydev-0.9.7/src/easydev/multisetup.py
--rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)     6109 2015-11-20 11:42:51.000000 easydev-0.9.7/src/easydev/browser.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4466 2015-10-19 17:07:35.000000 easydev-0.9.7/src/easydev/multicore.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1213 2015-11-12 20:46:00.000000 easydev-0.9.7/src/easydev/url.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2819 2015-09-10 09:52:07.000000 easydev-0.9.7/src/easydev/lsf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3092 2014-09-10 08:37:35.000000 easydev-0.9.7/src/easydev/easytest.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13329 2015-09-10 09:28:13.000000 easydev-0.9.7/src/easydev/config_tools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5273 2014-09-10 08:36:11.000000 easydev-0.9.7/src/easydev/decorators.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2597 2014-12-08 09:39:41.000000 easydev-0.9.7/src/easydev/codecs.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2014-09-10 08:38:45.000000 easydev-0.9.7/src/easydev/setuptools.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4183 2015-10-16 07:53:54.000000 easydev-0.9.7/src/easydev/paths.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2015-11-30 20:14:29.000000 easydev-0.9.7/src/easydev.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       20 2015-11-30 20:14:28.000000 easydev-0.9.7/src/easydev.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        8 2015-11-30 20:14:28.000000 easydev-0.9.7/src/easydev.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2024 2015-11-30 20:14:29.000000 easydev-0.9.7/src/easydev.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      170 2015-11-30 20:14:28.000000 easydev-0.9.7/src/easydev.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4105 2015-11-30 20:14:28.000000 easydev-0.9.7/src/easydev.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2015-11-30 20:14:28.000000 easydev-0.9.7/src/easydev.egg-info/dependency_links.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       54 2014-08-18 07:57:06.000000 easydev-0.9.9/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3550 2016-01-12 21:20:54.000000 easydev-0.9.9/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2456 2014-08-18 07:57:06.000000 easydev-0.9.9/share/copybutton.js
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/themes/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/themes/standard/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3740 2014-09-05 09:25:10.000000 easydev-0.9.9/share/themes/standard/layout.html
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/themes/standard/static/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      897 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/static/warning.jpg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      430 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/static/bgtop.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14130 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/static/software.css_t
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      434 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/static/bgfooter.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      623 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/google_footer.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      515 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/indexsidebar.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       64 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/index.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      481 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/standard/theme.conf
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      257 2014-12-10 09:39:24.000000 easydev-0.9.9/share/themes/standard/google_head.html
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/themes/cno/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4426 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/layout.html
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/share/themes/cno/static/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      897 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/static/warning.jpg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      430 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/static/bgtop.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14149 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/static/software.css_t
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      434 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/static/bgfooter.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      623 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/google_footer.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      515 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/indexsidebar.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       64 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/index.html
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      481 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/theme.conf
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2014-08-18 07:57:06.000000 easydev-0.9.9/share/themes/cno/google_head.html
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/test/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      148 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_dependencies.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      644 2014-08-30 08:42:50.000000 easydev-0.9.9/test/test_decorators.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      488 2015-06-18 07:33:06.000000 easydev-0.9.9/test/test_easytest.py
+-rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)      239 2015-11-03 14:52:38.000000 easydev-0.9.9/test/test_browse.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2497 2015-09-10 09:29:05.000000 easydev-0.9.9/test/test_config.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      609 2015-10-16 08:18:01.000000 easydev-0.9.9/test/test_progressbar.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      570 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_multicore.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      422 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_copybutton.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      707 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_paths.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      333 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_package.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      741 2015-11-12 20:46:00.000000 easydev-0.9.9/test/test_codecs.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       89 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_setuptools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      169 2015-06-19 13:21:24.000000 easydev-0.9.9/test/test_lsf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2015-01-05 13:42:47.000000 easydev-0.9.9/test/test_multigit.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2877 2015-01-05 14:16:32.000000 easydev-0.9.9/test/test_tools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      363 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_console.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      454 2015-10-16 07:28:34.000000 easydev-0.9.9/test/test_url.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       83 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_doc.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      572 2015-11-12 20:46:00.000000 easydev-0.9.9/test/test_misc.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      234 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_cnolab_sphinx.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      456 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_logging_tools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2255 2014-08-18 07:57:06.000000 easydev-0.9.9/test/test_multisetup.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4105 2016-01-12 21:23:11.000000 easydev-0.9.9/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2707 2015-11-20 11:18:56.000000 easydev-0.9.9/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      325 2016-01-12 21:23:11.000000 easydev-0.9.9/setup.cfg
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/src/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3278 2014-09-10 08:34:27.000000 easydev-0.9.9/src/easydev/console.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     7647 2015-11-30 20:09:52.000000 easydev-0.9.9/src/easydev/tools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1539 2014-09-10 08:39:03.000000 easydev-0.9.9/src/easydev/sphinx_themes.py
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     6253 2015-01-05 14:43:54.000000 easydev-0.9.9/src/easydev/multigit.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    23573 2016-01-12 21:13:47.000000 easydev-0.9.9/src/easydev/appdirs.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5363 2015-11-21 12:44:05.000000 easydev-0.9.9/src/easydev/progressbar.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1458 2015-08-24 14:42:41.000000 easydev-0.9.9/src/easydev/misc.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2988 2014-09-10 08:38:13.000000 easydev-0.9.9/src/easydev/logging_tools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4646 2014-09-10 08:35:14.000000 easydev-0.9.9/src/easydev/copybutton.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13062 2014-12-10 13:14:04.000000 easydev-0.9.9/src/easydev/package.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1721 2015-11-20 11:51:23.000000 easydev-0.9.9/src/easydev/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      908 2014-09-10 08:36:36.000000 easydev-0.9.9/src/easydev/dependencies.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1006 2015-01-26 10:23:43.000000 easydev-0.9.9/src/easydev/doc.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13020 2014-12-10 14:06:30.000000 easydev-0.9.9/src/easydev/multisetup.py
+-rw-r--r--   0 cokelaer  (1000) cokelaer  (1000)     6109 2015-11-20 11:42:51.000000 easydev-0.9.9/src/easydev/browser.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4466 2015-10-19 17:07:35.000000 easydev-0.9.9/src/easydev/multicore.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1213 2015-11-12 20:46:00.000000 easydev-0.9.9/src/easydev/url.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2819 2015-09-10 09:52:07.000000 easydev-0.9.9/src/easydev/lsf.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3092 2014-09-10 08:37:35.000000 easydev-0.9.9/src/easydev/easytest.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13342 2016-01-12 21:21:58.000000 easydev-0.9.9/src/easydev/config_tools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5273 2014-09-10 08:36:11.000000 easydev-0.9.9/src/easydev/decorators.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2597 2014-12-08 09:39:41.000000 easydev-0.9.9/src/easydev/codecs.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2014-09-10 08:38:45.000000 easydev-0.9.9/src/easydev/setuptools.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4183 2015-10-16 07:53:54.000000 easydev-0.9.9/src/easydev/paths.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        8 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/top_level.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2013 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      170 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4105 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2016-01-12 21:23:11.000000 easydev-0.9.9/src/easydev.egg-info/dependency_links.txt
```

### Comparing `easydev-0.9.7/setup.py` & `easydev-0.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import os
 from setuptools import setup, find_packages
 import glob
 
 _MAJOR               = 0
 _MINOR               = 9
-_MICRO               = 7
+_MICRO               = 9
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {'Cokelaer':('Thomas Cokelaer','cokelaer@ebi.ac.uk')},
     'version': version,
     'license' : 'GPL',
@@ -68,17 +68,15 @@
     download_url     = metainfo['download_url'],
     classifiers      = metainfo['classifiers'],
 
     # package installation
     package_dir = {'':'src'},
     packages = ['easydev'],
 
-    install_requires = ['ordereddict', 'appdirs'],
-
-    # ordereddict is for python2.6 and below
+    install_requires = [],
 
     # somehow, the google_head.html is found in themes/standard and themese/cno
     # directories thanks to the contents of datafiles variable but the ones from
     # themes/standard directory are not copied inside the distribution ?
     # using the MANIFEST.in solve the issue. However, data_files=datafiles is
     # still required for python setup.py install or pip install to copy the
     # share directory in the proper place. sure there will be a neat solution
```

### Comparing `easydev-0.9.7/share/copybutton.js` & `easydev-0.9.9/share/copybutton.js`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/standard/layout.html` & `easydev-0.9.9/share/themes/standard/layout.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/standard/static/warning.jpg` & `easydev-0.9.9/share/themes/standard/static/warning.jpg`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/standard/static/software.css_t` & `easydev-0.9.9/share/themes/standard/static/software.css_t`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/standard/google_footer.html` & `easydev-0.9.9/share/themes/standard/google_footer.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/standard/indexsidebar.html` & `easydev-0.9.9/share/themes/standard/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/cno/layout.html` & `easydev-0.9.9/share/themes/cno/layout.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/cno/static/warning.jpg` & `easydev-0.9.9/share/themes/cno/static/warning.jpg`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/cno/static/software.css_t` & `easydev-0.9.9/share/themes/cno/static/software.css_t`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/cno/google_footer.html` & `easydev-0.9.9/share/themes/cno/google_footer.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/share/themes/cno/indexsidebar.html` & `easydev-0.9.9/share/themes/cno/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_decorators.py` & `easydev-0.9.9/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_config.py` & `easydev-0.9.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_progressbar.py` & `easydev-0.9.9/test/test_progressbar.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_multicore.py` & `easydev-0.9.9/test/test_multicore.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_paths.py` & `easydev-0.9.9/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_codecs.py` & `easydev-0.9.9/test/test_codecs.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_tools.py` & `easydev-0.9.9/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_misc.py` & `easydev-0.9.9/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/test/test_multisetup.py` & `easydev-0.9.9/test/test_multisetup.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/PKG-INFO` & `easydev-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: easydev
-Version: 0.9.7
+Version: 0.9.9
 Summary: Common utilities to ease the development of Python packages
 Home-page: ['http://packages.python.org/easydev/']
 Author: Thomas Cokelaer
 Author-email: cokelaer@ebi.ac.uk
 License: GPL
 Download-URL: ['http://pypi.python.org/pypi/easydev']
 Description: easydev
```

### Comparing `easydev-0.9.7/README.rst` & `easydev-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/console.py` & `easydev-0.9.9/src/easydev/console.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/tools.py` & `easydev-0.9.9/src/easydev/tools.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/sphinx_themes.py` & `easydev-0.9.9/src/easydev/sphinx_themes.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/multigit.py` & `easydev-0.9.9/src/easydev/multigit.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/progressbar.py` & `easydev-0.9.9/src/easydev/progressbar.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/misc.py` & `easydev-0.9.9/src/easydev/misc.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/logging_tools.py` & `easydev-0.9.9/src/easydev/logging_tools.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/copybutton.py` & `easydev-0.9.9/src/easydev/copybutton.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/package.py` & `easydev-0.9.9/src/easydev/package.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/__init__.py` & `easydev-0.9.9/src/easydev/__init__.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/dependencies.py` & `easydev-0.9.9/src/easydev/dependencies.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/doc.py` & `easydev-0.9.9/src/easydev/doc.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/multisetup.py` & `easydev-0.9.9/src/easydev/multisetup.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/browser.py` & `easydev-0.9.9/src/easydev/browser.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/multicore.py` & `easydev-0.9.9/src/easydev/multicore.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/url.py` & `easydev-0.9.9/src/easydev/url.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/lsf.py` & `easydev-0.9.9/src/easydev/lsf.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/easytest.py` & `easydev-0.9.9/src/easydev/easytest.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/config_tools.py` & `easydev-0.9.9/src/easydev/config_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
 
 class CustomConfig(object):
     """Base class to manipulate a config directory"""
 
     def __init__(self, name, verbose=False):
         self.verbose = verbose
-        import appdirs
+        from easydev import appdirs
         self.appdirs = appdirs.AppDirs(name)
 
     def init(self):
         sdir = self.appdirs.user_config_dir
         self._get_and_create(sdir)
 
     def _get_config_dir(self):
```

### Comparing `easydev-0.9.7/src/easydev/decorators.py` & `easydev-0.9.9/src/easydev/decorators.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/codecs.py` & `easydev-0.9.9/src/easydev/codecs.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/setuptools.py` & `easydev-0.9.9/src/easydev/setuptools.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev/paths.py` & `easydev-0.9.9/src/easydev/paths.py`

 * *Files identical despite different names*

### Comparing `easydev-0.9.7/src/easydev.egg-info/SOURCES.txt` & `easydev-0.9.9/src/easydev.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 share/themes/standard/layout.html
 share/themes/standard/theme.conf
 share/themes/standard/static/bgfooter.png
 share/themes/standard/static/bgtop.png
 share/themes/standard/static/software.css_t
 share/themes/standard/static/warning.jpg
 src/easydev/__init__.py
+src/easydev/appdirs.py
 src/easydev/browser.py
 src/easydev/codecs.py
 src/easydev/config_tools.py
 src/easydev/console.py
 src/easydev/copybutton.py
 src/easydev/decorators.py
 src/easydev/dependencies.py
@@ -46,15 +47,14 @@
 src/easydev/sphinx_themes.py
 src/easydev/tools.py
 src/easydev/url.py
 src/easydev.egg-info/PKG-INFO
 src/easydev.egg-info/SOURCES.txt
 src/easydev.egg-info/dependency_links.txt
 src/easydev.egg-info/entry_points.txt
-src/easydev.egg-info/requires.txt
 src/easydev.egg-info/top_level.txt
 test/test_browse.py
 test/test_cnolab_sphinx.py
 test/test_codecs.py
 test/test_config.py
 test/test_console.py
 test/test_copybutton.py
```

### Comparing `easydev-0.9.7/src/easydev.egg-info/PKG-INFO` & `easydev-0.9.9/src/easydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: easydev
-Version: 0.9.7
+Version: 0.9.9
 Summary: Common utilities to ease the development of Python packages
 Home-page: ['http://packages.python.org/easydev/']
 Author: Thomas Cokelaer
 Author-email: cokelaer@ebi.ac.uk
 License: GPL
 Download-URL: ['http://pypi.python.org/pypi/easydev']
 Description: easydev
```

