# Comparing `tmp/pydmt-0.3.8.tar.gz` & `tmp/pydmt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmt-0.3.8.tar", last modified: Sat Apr  6 12:36:27 2024, max compression
+gzip compressed data, was "pydmt-0.3.9.tar", last modified: Sat Apr  6 12:38:55 2024, max compression
```

## Comparing `pydmt-0.3.8.tar` & `pydmt-0.3.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.818407 pydmt-0.3.8/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2024-04-06 12:36:12.000000 pydmt-0.3.8/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:36:27.818407 pydmt-0.3.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      396 2024-04-06 12:36:12.000000 pydmt-0.3.8/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt/api/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/api/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.3.8/pydmt/api/builder.py
--rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.3.8/pydmt/api/copy.py
--rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.3.8/pydmt/api/fail.py
--rw-r--r--   0 mark      (1000) mark      (1000)      613 2023-05-01 12:24:57.000000 pydmt-0.3.8/pydmt/api/feature.py
--rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.3.8/pydmt/api/one_source_one_target.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt/builders/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/builders/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.3.8/pydmt/builders/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      498 2023-11-13 15:29:48.000000 pydmt-0.3.8/pydmt/builders/gem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      396 2023-12-29 14:25:09.000000 pydmt-0.3.8/pydmt/builders/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.3.8/pydmt/builders/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.3.8/pydmt/builders/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1893 2024-04-06 12:30:31.000000 pydmt-0.3.8/pydmt/builders/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.3.8/pydmt/builders/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2728 2024-04-06 12:35:38.000000 pydmt-0.3.8/pydmt/builders/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.3.8/pydmt/builders/yaml.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3284 2024-01-10 12:06:23.000000 pydmt-0.3.8/pydmt/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt/core/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/core/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.3.8/pydmt/core/cache.py
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.3.8/pydmt/core/graph.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.3.8/pydmt/core/pydmt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/core/tempdir.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt/features/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/features/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.3.8/pydmt/features/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      370 2023-11-13 08:36:09.000000 pydmt-0.3.8/pydmt/features/gem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.3.8/pydmt/features/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-05-01 12:22:39.000000 pydmt-0.3.8/pydmt/features/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.3.8/pydmt/features/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.3.8/pydmt/features/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.3.8/pydmt/features/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)      455 2023-12-29 15:12:48.000000 pydmt-0.3.8/pydmt/features/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1010 2023-05-01 12:25:10.000000 pydmt-0.3.8/pydmt/features/yaml.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.818407 pydmt-0.3.8/pydmt/helpers/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.3.8/pydmt/helpers/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.3.8/pydmt/helpers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      135 2023-05-02 19:24:19.000000 pydmt-0.3.8/pydmt/helpers/composites.py
--rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.3.8/pydmt/helpers/deb.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.3.8/pydmt/helpers/deb_python_package.py
--rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.3.8/pydmt/helpers/files.py
--rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.3.8/pydmt/helpers/general.py
--rw-r--r--   0 mark      (1000) mark      (1000)      785 2023-05-02 19:24:19.000000 pydmt-0.3.8/pydmt/helpers/git.py
--rw-r--r--   0 mark      (1000) mark      (1000)      212 2023-04-28 19:49:07.000000 pydmt-0.3.8/pydmt/helpers/github.py
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.3.8/pydmt/helpers/messages.py
--rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.3.8/pydmt/helpers/misc.py
--rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.3.8/pydmt/helpers/pkgs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.3.8/pydmt/helpers/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4782 2023-04-28 19:46:14.000000 pydmt-0.3.8/pydmt/helpers/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)      818 2023-10-10 18:09:54.000000 pydmt-0.3.8/pydmt/helpers/signature.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.3.8/pydmt/helpers/snipplets.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1360 2023-11-16 04:41:39.000000 pydmt-0.3.8/pydmt/helpers/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5395 2024-01-10 12:03:31.000000 pydmt-0.3.8/pydmt/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      174 2024-04-06 12:36:12.000000 pydmt-0.3.8/pydmt/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.818407 pydmt-0.3.8/pydmt/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.8/pydmt/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.3.8/pydmt/utils/digest.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.3.8/pydmt/utils/digester.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.3.8/pydmt/utils/filesystem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2023-11-16 04:41:08.000000 pydmt-0.3.8/pydmt/utils/importlib.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.3.8/pydmt/utils/logging.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.3.8/pydmt/utils/php.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2470 2024-04-06 12:20:29.000000 pydmt-0.3.8/pydmt/utils/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.3.8/pydmt/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:36:27.814407 pydmt-0.3.8/pydmt.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     1615 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       42 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       77 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-06 12:36:27.000000 pydmt-0.3.8/pydmt.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2024-04-06 12:36:27.818407 pydmt-0.3.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1760 2024-04-06 12:36:12.000000 pydmt-0.3.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2024-04-06 12:38:44.000000 pydmt-0.3.9/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:38:55.407053 pydmt-0.3.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      396 2024-04-06 12:38:44.000000 pydmt-0.3.9/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.403053 pydmt-0.3.9/pydmt/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/__init__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.403053 pydmt-0.3.9/pydmt/api/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/api/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.3.9/pydmt/api/builder.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.3.9/pydmt/api/copy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.3.9/pydmt/api/fail.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2023-05-01 12:24:57.000000 pydmt-0.3.9/pydmt/api/feature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.3.9/pydmt/api/one_source_one_target.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/pydmt/builders/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/builders/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.3.9/pydmt/builders/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      498 2023-11-13 15:29:48.000000 pydmt-0.3.9/pydmt/builders/gem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      396 2023-12-29 14:25:09.000000 pydmt-0.3.9/pydmt/builders/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.3.9/pydmt/builders/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.3.9/pydmt/builders/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1930 2024-04-06 12:37:55.000000 pydmt-0.3.9/pydmt/builders/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.3.9/pydmt/builders/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2806 2024-04-06 12:38:22.000000 pydmt-0.3.9/pydmt/builders/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.3.9/pydmt/builders/yaml.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3284 2024-01-10 12:06:23.000000 pydmt-0.3.9/pydmt/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/pydmt/core/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/core/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.3.9/pydmt/core/cache.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.3.9/pydmt/core/graph.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.3.9/pydmt/core/pydmt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/core/tempdir.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/pydmt/features/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/features/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.3.9/pydmt/features/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      370 2023-11-13 08:36:09.000000 pydmt-0.3.9/pydmt/features/gem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.3.9/pydmt/features/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-05-01 12:22:39.000000 pydmt-0.3.9/pydmt/features/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.3.9/pydmt/features/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.3.9/pydmt/features/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.3.9/pydmt/features/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      455 2023-12-29 15:12:48.000000 pydmt-0.3.9/pydmt/features/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1010 2023-05-01 12:25:10.000000 pydmt-0.3.9/pydmt/features/yaml.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/pydmt/helpers/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.3.9/pydmt/helpers/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.3.9/pydmt/helpers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      135 2023-05-02 19:24:19.000000 pydmt-0.3.9/pydmt/helpers/composites.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.3.9/pydmt/helpers/deb.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.3.9/pydmt/helpers/deb_python_package.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.3.9/pydmt/helpers/files.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.3.9/pydmt/helpers/general.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      785 2023-05-02 19:24:19.000000 pydmt-0.3.9/pydmt/helpers/git.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      212 2023-04-28 19:49:07.000000 pydmt-0.3.9/pydmt/helpers/github.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.3.9/pydmt/helpers/messages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.3.9/pydmt/helpers/misc.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.3.9/pydmt/helpers/pkgs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.3.9/pydmt/helpers/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4782 2023-04-28 19:46:14.000000 pydmt-0.3.9/pydmt/helpers/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      818 2023-10-10 18:09:54.000000 pydmt-0.3.9/pydmt/helpers/signature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.3.9/pydmt/helpers/snipplets.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1360 2023-11-16 04:41:39.000000 pydmt-0.3.9/pydmt/helpers/urls.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5395 2024-01-10 12:03:31.000000 pydmt-0.3.9/pydmt/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      174 2024-04-06 12:38:44.000000 pydmt-0.3.9/pydmt/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.407053 pydmt-0.3.9/pydmt/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.9/pydmt/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.3.9/pydmt/utils/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.3.9/pydmt/utils/digester.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.3.9/pydmt/utils/filesystem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2023-11-16 04:41:08.000000 pydmt-0.3.9/pydmt/utils/importlib.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.3.9/pydmt/utils/logging.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.3.9/pydmt/utils/php.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2470 2024-04-06 12:20:29.000000 pydmt-0.3.9/pydmt/utils/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.3.9/pydmt/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:38:55.403053 pydmt-0.3.9/pydmt.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     1615 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       77 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-06 12:38:55.000000 pydmt-0.3.9/pydmt.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2024-04-06 12:38:55.411053 pydmt-0.3.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1760 2024-04-06 12:38:44.000000 pydmt-0.3.9/setup.py
```

### Comparing `pydmt-0.3.8/LICENSE` & `pydmt-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/PKG-INFO` & `pydmt-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -42,10 +42,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.3.8
+version: 0.3.9
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024
```

### Comparing `pydmt-0.3.8/pydmt/api/builder.py` & `pydmt-0.3.9/pydmt/api/builder.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/api/feature.py` & `pydmt-0.3.9/pydmt/api/feature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/api/one_source_one_target.py` & `pydmt-0.3.9/pydmt/api/one_source_one_target.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/builders/apt.py` & `pydmt-0.3.9/pydmt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/builders/mako.py` & `pydmt-0.3.9/pydmt/builders/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/builders/reqs.py` & `pydmt-0.3.9/pydmt/builders/reqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         Because importing python.py may fail because of prereqs that python.py
         needs. In this case the user specifies these prereqs in bootstrap.py
         """
         if os.path.isfile(REQUIREMENTS):
             args = get_install_args()
             args.extend(["-r", REQUIREMENTS])
             check_call(args)
+            mkdir_touch(self.target)
             return
         args = get_install_args()
         packs = collect_bootstrap_reqs()
         if packs:
             args.extend(packs)
             check_call(args)
         args = get_install_args()
```

### Comparing `pydmt-0.3.8/pydmt/builders/sphinx.py` & `pydmt-0.3.9/pydmt/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/builders/venv.py` & `pydmt-0.3.9/pydmt/builders/venv.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
     def build(self) -> None:
         if ConfigVenv.incremental and os.path.isdir(TARGET_FOLDER):
             if os.path.isfile(REQUIREMENTS):
                 args = get_install_args()
                 args.extend(["-r", REQUIREMENTS])
                 check_call(args)
+                mkdir_touch(self.target)
                 return
             # now install regular packages (we only run the install if there are packages to install)
             packs = collect_reqs(add_dev=ConfigVenv.add_dev)
             if packs:
                 args = get_install_args()
                 args.extend(packs)
                 check_call_ve(args)
@@ -63,14 +64,15 @@
                 "pip",
             ]
             check_call_ve(args)
         if os.path.isfile(REQUIREMENTS):
             args = get_install_args()
             args.extend(["-r", REQUIREMENTS])
             check_call(args)
+            mkdir_touch(self.target)
             return
         # install bootstrap packages so that we could read config/* files
         packs = collect_bootstrap_reqs()
         if packs:
             args = get_install_args()
             args.extend(packs)
             check_call_ve(args)
```

### Comparing `pydmt-0.3.8/pydmt/builders/yaml.py` & `pydmt-0.3.9/pydmt/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/configs.py` & `pydmt-0.3.9/pydmt/configs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/core/cache.py` & `pydmt-0.3.9/pydmt/core/cache.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/core/pydmt.py` & `pydmt-0.3.9/pydmt/core/pydmt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/features/apt.py` & `pydmt-0.3.9/pydmt/features/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/features/mako.py` & `pydmt-0.3.9/pydmt/features/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/features/yaml.py` & `pydmt-0.3.9/pydmt/features/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/apt.py` & `pydmt-0.3.9/pydmt/helpers/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/deb.py` & `pydmt-0.3.9/pydmt/helpers/deb.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/deb_python_package.py` & `pydmt-0.3.9/pydmt/helpers/deb_python_package.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/git.py` & `pydmt-0.3.9/pydmt/helpers/git.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/python.py` & `pydmt-0.3.9/pydmt/helpers/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/signature.py` & `pydmt-0.3.9/pydmt/helpers/signature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/snipplets.py` & `pydmt-0.3.9/pydmt/helpers/snipplets.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/helpers/urls.py` & `pydmt-0.3.9/pydmt/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/main.py` & `pydmt-0.3.9/pydmt/main.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/utils/digest.py` & `pydmt-0.3.9/pydmt/utils/digest.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/utils/digester.py` & `pydmt-0.3.9/pydmt/utils/digester.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/utils/filesystem.py` & `pydmt-0.3.9/pydmt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/utils/python.py` & `pydmt-0.3.9/pydmt/utils/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt/utils/subprocess.py` & `pydmt-0.3.9/pydmt/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/pydmt.egg-info/PKG-INFO` & `pydmt-0.3.9/pydmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -42,10 +42,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.3.8
+version: 0.3.9
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024
```

### Comparing `pydmt-0.3.8/pydmt.egg-info/SOURCES.txt` & `pydmt-0.3.9/pydmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.8/setup.py` & `pydmt-0.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.rst") as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydmt",
-    version="0.3.8",
+    version="0.3.9",
     packages=[
         "pydmt",
         "pydmt.api",
         "pydmt.builders",
         "pydmt.core",
         "pydmt.features",
         "pydmt.helpers",
```

