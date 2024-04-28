# Comparing `tmp/pyslth-0.1.6.tar.gz` & `tmp/pyslth-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.1.6.tar", last modified: Sat Apr 27 20:11:58 2024, max compression
+gzip compressed data, was "pyslth-0.1.7.tar", last modified: Sun Apr 28 00:52:03 2024, max compression
```

## Comparing `pyslth-0.1.6.tar` & `pyslth-0.1.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.820749 pyslth-0.1.6/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.6/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-27 20:11:58.820542 pyslth-0.1.6/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.788526 pyslth-0.1.6/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-27 20:11:58.000000 pyslth-0.1.6/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1723 2024-04-27 20:11:58.000000 pyslth-0.1.6/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-27 20:11:58.000000 pyslth-0.1.6/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-27 20:11:58.000000 pyslth-0.1.6/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-27 20:11:58.000000 pyslth-0.1.6/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.6/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-27 20:11:58.820808 pyslth-0.1.6/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-27 20:11:23.000000 pyslth-0.1.6/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.794551 pyslth-0.1.6/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.6/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.6/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.795265 pyslth-0.1.6/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.6/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.6/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20236 2024-04-27 15:13:10.000000 pyslth-0.1.6/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.6/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.6/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.795613 pyslth-0.1.6/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.799045 pyslth-0.1.6/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.6/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.6/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.801797 pyslth-0.1.6/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.6/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.6/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.6/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.6/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.6/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.6/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.6/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.802271 pyslth-0.1.6/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.6/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.6/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.6/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.802600 pyslth-0.1.6/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.803816 pyslth-0.1.6/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.806165 pyslth-0.1.6/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.6/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.6/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.808058 pyslth-0.1.6/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.6/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.6/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.6/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.6/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.819966 pyslth-0.1.6/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-27 19:03:35.000000 pyslth-0.1.6/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    80435 2024-04-27 19:03:35.000000 pyslth-0.1.6/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-27 19:03:35.000000 pyslth-0.1.6/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/slth.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.6/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.6/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-27 20:11:58.820183 pyslth-0.1.6/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     1499 2024-04-27 19:06:07.000000 pyslth-0.1.6/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.6/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.6/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.6/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2264 2024-04-27 19:07:43.000000 pyslth-0.1.6/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.809836 pyslth-0.1.7/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.7/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 00:52:03.809620 pyslth-0.1.7/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.779087 pyslth-0.1.7/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1723 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.7/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-28 00:52:03.809897 pyslth-0.1.7/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-28 00:50:05.000000 pyslth-0.1.7/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.785715 pyslth-0.1.7/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.7/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.7/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.788911 pyslth-0.1.7/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.7/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.7/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.1.7/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.7/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.7/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.789462 pyslth-0.1.7/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.790126 pyslth-0.1.7/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.7/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.7/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.792663 pyslth-0.1.7/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.7/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.7/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.7/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.1.7/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.7/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.7/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.7/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.793164 pyslth-0.1.7/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.7/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.7/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.7/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.793492 pyslth-0.1.7/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.794764 pyslth-0.1.7/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.797074 pyslth-0.1.7/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.7/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.7/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.799185 pyslth-0.1.7/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.7/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.7/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.7/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.7/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.808821 pyslth-0.1.7/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    79731 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.809330 pyslth-0.1.7/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.1.7/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.7/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.7/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.7/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.1.7/slth/views.py
```

### Comparing `pyslth-0.1.6/PKG-INFO` & `pyslth-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.6
+Version: 0.1.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.6/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.7/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.6
+Version: 0.1.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.6/pyslth.egg-info/SOURCES.txt` & `pyslth-0.1.7/pyslth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,12 +51,12 @@
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
 slth/static/js/lib.min.js
 slth/static/js/peerjs.min.js
 slth/static/js/qrcode.min.js
 slth/static/js/react-trigger-change.js
 slth/static/js/react.min.js
-slth/static/js/service-worker.js
 slth/static/js/slth.js
 slth/static/js/vanilla-masker.js
 slth/static/js/vanilla-masker.min.js
-slth/templates/index.html
+slth/templates/index.html
+slth/templates/service-worker.js
```

### Comparing `pyslth-0.1.6/setup.py` & `pyslth-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.1.6/slth/__init__.py` & `pyslth-0.1.7/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/components.py` & `pyslth-0.1.7/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/db/models.py` & `pyslth-0.1.7/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/endpoints.py` & `pyslth-0.1.7/slth/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 from django.views.decorators.csrf import csrf_exempt
 from .factory import FormFactory
 from .forms import LoginForm, ModelForm, Form, SendPushNotificationForm, EditProfileForm
 from .serializer import serialize, Serializer
 from .components import Application as Application_, Navbar, Menu, Footer, Response, Boxes, IconSet
 from .exceptions import JsonResponseException
 from .utils import build_url, append_url
-from .models import PushSubscription, Profile
+from .models import PushSubscription, Profile, User
 from slth.queryset import QuerySet
 from slth import APPLICATON, ENDPOINTS
-from django.contrib.auth.models import User
 
 
 import slth
 
 
 T = TypeVar("T")
 
@@ -431,15 +430,19 @@
 class Users(ListEndpoint[User]):
 
     class Meta:
         modal = False
         verbose_name = 'Usuários'
 
     def get(self):
-        return super().get().fields('username', 'email', 'is_superuser').actions('sendpushnotification')
+        return (
+            super().get()
+            .fields('username', 'email', 'is_superuser')
+            .actions('add', 'view', 'edit', 'delete', 'sendpushnotification')
+        )
 
 class Dashboard(Endpoint):
     class Meta:
         verbose_name = ''
         
     def get(self):
         if self.request.user.is_authenticated:
```

### Comparing `pyslth-0.1.6/slth/factory.py` & `pyslth-0.1.7/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/forms.py` & `pyslth-0.1.7/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/management/commands/integration_test.py` & `pyslth-0.1.7/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/management/commands/sync.py` & `pyslth-0.1.7/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/migrations/0001_initial.py` & `pyslth-0.1.7/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.7/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/models.py` & `pyslth-0.1.7/slth/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import binascii
-from .db import models
+from .db import models, meta
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
-
+from django.contrib.auth.models import User
 from django.apps import apps
 from datetime import datetime
 from django.utils.html import strip_tags
 from django.core.mail import EmailMultiAlternatives
+from slth import APPLICATON
 
 
 class RoleQuerySet(models.QuerySet):
 
     def contains(self, *names):
         _names = getattr(self, '_names', None)
         if _names is None:
@@ -49,19 +50,20 @@
         verbose_name = 'Papel'
         verbose_name_plural = 'Papéis'
 
     def __str__(self):
         return self.get_description()
 
     def get_verbose_name(self):
-        return self.name
+        return APPLICATON['groups'].get(self.name, self.name)
 
     def get_scope_value(self):
         return apps.get_model(self.model).objects.get(pk=self.value) if self.model else None
 
+    @meta('Descrição')
     def get_description(self):
         scope_value = self.get_scope_value()
         return '{} - {}'.format(self.get_verbose_name(), scope_value) if scope_value else self.get_verbose_name()
 
 
 class EmailManager(models.Manager):
     def all(self):
@@ -151,7 +153,37 @@
     def save(self, *args, **kwargs):
         if not self.key:
             self.key = binascii.hexlify(os.urandom(20)).decode()
         return super().save(*args, **kwargs)
 
     def __str__(self):
         return self.key
+    
+class User(User):
+    class Meta:
+        icon = 'users'
+        proxy = True
+        verbose_name = 'Usuário'
+        verbose_name_plural = 'Usuários'
+
+    def formfactory(self):
+        return (
+            super().formfactory()
+            .fieldset('Dados Gerais', (('first_name', 'last_name'), 'email'))
+            .fieldset('Dados de Acesso', (('is_superuser', 'is_active'),))
+        )
+    
+    def serializer(self):
+        return (
+            super().serializer()
+            .fieldset('Dados Gerais', (('first_name', 'last_name'), 'email'))
+            .fieldset('Dados de Acesso', (('is_superuser', 'is_active'),))
+            .queryset('Notificação', 'get_push_subscriptions')
+            .queryset('Papéis', 'get_roles')
+        )
+    
+    def get_push_subscriptions(self):
+        return self.pushsubscription_set.fields('device')
+    
+    def get_roles(self):
+        return Role.objects.filter(username=self.username).fields('get_description')
+
```

### Comparing `pyslth-0.1.6/slth/permissions.py` & `pyslth-0.1.7/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/queryset.py` & `pyslth-0.1.7/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/roles.py` & `pyslth-0.1.7/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/selenium/__init__.py` & `pyslth-0.1.7/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/selenium/browser.py` & `pyslth-0.1.7/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/serializer.py` & `pyslth-0.1.7/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/fontawesome.min.css` & `pyslth-0.1.7/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/fonts/Eina02-Bold.f8011405.ttf` & `pyslth-0.1.7/slth/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/fonts/Eina02-Regular.2e682693.ttf` & `pyslth-0.1.7/slth/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `pyslth-0.1.7/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.1.7/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/slth.css` & `pyslth-0.1.7/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/css/solid.min.css` & `pyslth-0.1.7/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/images/logo.png` & `pyslth-0.1.7/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/images/logo.svg` & `pyslth-0.1.7/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/images/user.png` & `pyslth-0.1.7/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/echarts.min.js` & `pyslth-0.1.7/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/index.min.js` & `pyslth-0.1.7/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/lib.min.js` & `pyslth-0.1.7/slth/static/js/lib.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     j as t,
-    c as P,
+    c as H,
     r as S
 } from "./react.min.js";
 
 function k(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
@@ -42,15 +42,15 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function b(e) {
+function w(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
@@ -68,15 +68,15 @@
         };
         return e.primary && (a.backgroundColor = "#1351b4", a.color = "white"), e.default && (a.color = "#1351b4", a.border = "solid 1px #1351b4"), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(b, {
+            children: t.jsx(w, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const Te = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
@@ -90,28 +90,28 @@
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 10
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(b, {
+            children: [t.jsx(w, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
 function Q(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), P.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
+    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -144,29 +144,29 @@
     return n()
 }
 
 function Ie(e) {
     return ge(e.data)
 }
 
-function I(e) {
+function A(e) {
     return e.replace("/app/", "/api/")
 }
 
 function F(e) {
     return e.replace("/api/", "/app/")
 }
 
 function q(e, n, a, r) {
     const c = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
     c && (i.Authorization = "Token " + c);
-    const l = I(n);
+    const l = A(n);
     var d = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
     r && (d.body = r);
     var o = null,
@@ -192,41 +192,41 @@
 function ge(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
     }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = F(e.redirect)) : e.message && Q(e.message)
 }
 
 function xe() {
-    document.querySelector(".layer") == null && P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ae, {}))
+    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Be, {}))
 }
 
 function ye(e, n) {
     fe(), xe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Be, {
-        url: I(e)
+    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ae, {
+        url: A(e)
     }))
 }
 
 function De(e) {
-    fe(), xe(), P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Le, {
-        url: I(e)
+    fe(), xe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Le, {
+        url: A(e)
     }))
 }
 
 function U(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function Ae(e) {
+function Be(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
@@ -238,35 +238,35 @@
         onClick: function() {
             U()
         },
         style: n
     })
 }
 
-function Be(e) {
+function Ae(e) {
     const [n, a] = S.useState(null), [r, c] = S.useState(0);
     S.useEffect(() => {
-        i(I(e.url)), document.querySelector(".layer").style.display = "block"
+        i(A(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(o) {
-        q("GET", I(o), function(h) {
+        q("GET", A(o), function(h) {
             a(h), c(r + 1)
         })
     }
 
     function l() {
         const o = {
             textAlign: "right",
             cursor: "pointer"
         };
         if (n) return t.jsxs("div", {
             children: [t.jsx("div", {
                 style: o,
-                children: t.jsx(b, {
+                children: t.jsx(w, {
                     icon: "x",
                     onClick: () => U()
                 })
             }), t.jsx(y, {
                 data: n
             })]
         })
@@ -304,57 +304,57 @@
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: c,
-                children: t.jsx(b, {
+                children: t.jsx(w, {
                     icon: "x",
                     onClick: () => U()
                 })
             }), t.jsx("iframe", {
-                src: I(e.url),
+                src: A(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
     }
     return a()
 }
 
-function Oe() {
+function Ne() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function A({
+function D({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: c,
     primary: i,
     compact: l,
     spin: d
 }) {
     function o() {
-        return a ? l || !r ? t.jsx(b, {
+        return a ? l || !r ? t.jsx(w, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Ee, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(b, {
+            }), t.jsx(w, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
@@ -380,27 +380,27 @@
             },
             children: o()
         })
     }
     return h()
 }
 
-function N(e) {
+function O(e) {
     const n = e.id || Math.random(),
         [a, r] = S.useState(e.data.name);
 
     function c(d) {
         d.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(d)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name ? t.jsx(b, {
+        return e.data.icon ? e.compact || !e.data.name ? t.jsx(w, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(b, {
+            children: [t.jsx(w, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
@@ -468,27 +468,27 @@
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(d => t.jsx("li", {
                     style: l,
-                    children: t.jsx(N, {
+                    children: t.jsx(O, {
                         data: d,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
     return c()
 }
-const Ne = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
+const Oe = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     V = {
         padding: 15,
         border: "solid 1px #CCC",
         borderRadius: 5
     };
 
 function te(e) {
@@ -545,57 +545,57 @@
     if (e) {
         for (var n = 0; n < e.hide.length; n++) Re(e.hide[n]);
         for (var n = 0; n < e.show.length; n++) _e(e.show[n]);
         for (var a in e.set) Fe(a, e.set[a])
     }
 }
 
-function Pe(e) {
+function He(e) {
     function n() {
         const a = {
             color: "#155bcb",
             backgroundColor: "#d4e5ff",
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(b, {
+                children: [t.jsx(w, {
                     icon: "circle-check",
                     style: {
                         color: "#155bcb",
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function He(e) {
+function Pe(e) {
     function n() {
         const a = {
             color: "white",
             display: "none",
             backgroundColor: "#e52207",
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
-            children: [t.jsx(b, {
+            children: [t.jsx(w, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -629,25 +629,25 @@
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
             style: d,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
-            }), e.data.action && t.jsx(N, {
+            }), e.data.action && t.jsx(O, {
                 data: e.data.action,
                 style: {
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Ne.indexOf(e.data.type) >= 0 ? t.jsx(ce, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Oe.indexOf(e.data.type) >= 0 ? t.jsx(ce, {
             data: e.data
         }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ue, {
             data: e.data
         }) : t.jsx(ne, {
             data: e.data
         }) : t.jsx(Ve, {
             data: e.data
@@ -666,15 +666,15 @@
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
     function c() {
         return t.jsx("div", {
-            children: t.jsx(He, {
+            children: t.jsx(Pe, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function i() {
         return e.data.help_text && t.jsx(We, {
@@ -731,21 +731,21 @@
             let o = l.target.files[0];
             var d = new FileReader;
             d.onload = function(h) {
                 if (te(o.name)) {
                     const v = "display" + a;
                     var s = document.createElement("img");
                     s.id = l.target.id + "img", s.style.width = "200px", s.style.display = "block", s.style.margin = "auto", s.style.marginTop = "20px", s.onload = function(j) {
-                        const D = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
+                        const I = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
                         var C = document.createElement("canvas");
                         const M = C.getContext("2d");
                         C.height = C.width * (s.height / s.width);
                         const E = document.createElement("canvas"),
-                            H = E.getContext("2d");
-                        E.width = s.width * D, E.height = s.height * D, H.drawImage(s, 0, 0, E.width, E.height), M.drawImage(E, 0, 0, E.width * D, E.height * D, 0, 0, C.width, C.height), E.toBlob(function(g) {
+                            P = E.getContext("2d");
+                        E.width = s.width * I, E.height = s.height * I, P.drawImage(s, 0, 0, E.width, E.height), M.drawImage(E, 0, 0, E.width * I, E.height * I, 0, 0, C.width, C.height), E.toBlob(function(g) {
                             const f = new DataTransfer;
                             f.items.add(new File([g], o.name)), l.target.files = f.files
                         });
                         var u = document.getElementById(v);
                         u == null ? (u = document.createElement("div"), u.id = v) : u.removeChild(u.childNodes[0]), u.appendChild(s), l.target.parentNode.appendChild(u)
                     }, s.src = h.target.result
                 }
@@ -773,15 +773,15 @@
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10
                     },
                     children: [t.jsx("div", {
                         style: h,
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
                                 color: "#1351b4"
                             }
                         })
                     }), t.jsxs("div", {
@@ -802,15 +802,15 @@
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
                             children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(s => "." + s).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: h,
-                        children: t.jsx(A, {
+                        children: t.jsx(D, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: l,
@@ -881,34 +881,34 @@
                     cursor: "pointer",
                     marginRight: 5
                 },
                 p = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [u == null && n.map((w, L) => t.jsxs("div", {
+                children: [u == null && n.map((b, L) => t.jsxs("div", {
                     style: g,
                     children: [t.jsx("span", {
                         onClick: () => E(L),
                         style: f,
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "trash-can",
                             style: p
                         })
-                    }), w.value]
-                }, Math.random())), u != null && Array.from(u.options).map((w, L) => t.jsxs("div", {
+                    }), b.value]
+                }, Math.random())), u != null && Array.from(u.options).map((b, L) => t.jsxs("div", {
                     style: g,
                     children: [t.jsx("span", {
                         onClick: () => E(L),
                         style: f,
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "trash-can",
                             style: p
                         })
-                    }), w.innerHTML]
+                    }), b.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function m(u) {
         o([])
@@ -945,22 +945,22 @@
         const f = document.getElementById(r);
         if (f) {
             let T = null,
                 _ = f,
                 W = null;
             for (; !W && (_ = _.parentElement) instanceof HTMLElement;) _.matches("dialog") && (W = _);
             T = W;
-            const O = f.getBoundingClientRect();
-            var p = O.top + O.height,
-                w = O.left;
+            const N = f.getBoundingClientRect();
+            var p = N.top + N.height,
+                b = N.left;
             if (T) {
                 const J = T.getBoundingClientRect();
-                p = p - J.top, w = w - J.left
-            } else p += window.scrollY, w += window.scrollX;
-            g.width = O.width, g.top = p, g.left = w
+                p = p - J.top, b = b - J.left
+            } else p += window.scrollY, b += window.scrollX;
+            g.width = N.width, g.top = p, g.left = b
         }
         const L = {
                 cursor: "pointer",
                 padding: 10
             },
             Z = !c && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
@@ -975,15 +975,15 @@
                 onChange: C,
                 onMouseLeave: j,
                 onBlur: j,
                 defaultValue: Z,
                 style: u
             }), d && i && t.jsxs("ul", {
                 style: g,
-                onMouseLeave: D,
+                onMouseLeave: I,
                 onMouseEnter: function(T) {
                     h = !0
                 },
                 children: [d.length == 0 && t.jsx("li", {
                     style: L,
                     children: "Nenhuma opção encontrada."
                 }), d.map(T => t.jsx("li", {
@@ -995,19 +995,19 @@
                 }, Math.random()))]
             })]
         })
     }
 
     function j(u) {
         h = !1, setTimeout(function() {
-            D(u)
+            I(u)
         }, 250)
     }
 
-    function D(u) {
+    function I(u) {
         const g = document.getElementById(a),
             f = document.getElementById(r);
         c || g.options.length > 0 && f.value != g.options[0].innerHTML && (g.innerHTML = "", f.value = "", l(!1)), u.target.tagName == "UL" ? l(!1) : h || l(!1)
     }
 
     function C(u) {
         const g = e.data.choices.indexOf("?") < 0 ? "?" : "&";
@@ -1024,20 +1024,20 @@
 
     function E(u) {
         const g = document.getElementById(a);
         var f = Array.from(g.options);
         g.innerHTML = f.slice(0, u).concat(f.slice(u + 1)).map(p => `<option selected value="${p.value}">${p.innerHTML}</option>`).join(""), o([])
     }
 
-    function H() {
+    function P() {
         return t.jsxs(t.Fragment, {
             children: [s(), x(), v()]
         })
     }
-    return H()
+    return P()
 }
 
 function Ge(e) {
     function n() {
         var a = {
             ...V
         };
@@ -1177,21 +1177,21 @@
     function c() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(ie, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(D, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(A, {
+                }), t.jsx(D, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => i(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
@@ -1254,21 +1254,21 @@
                 data: s
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(D, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => i(),
                     id: "extra-add-" + x + "-",
                     display: m
-                }), t.jsx(A, {
+                }), t.jsx(D, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => l(x),
                     display: "inline"
                 })]
             })]
         }, Math.random())
@@ -1295,15 +1295,15 @@
             m.name = m.name.replace("__n__", "__" + n + "__")
         }), s.fields[0].value = 0) : s.fieldsets.map(function(m) {
             m.fields.map(function(x) {
                 x.map(function(v) {
                     v.name = v.name.replace("__n__", "__" + n + "__")
                 }), x[0].value = 0
             })
-        }), P.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(c, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(c, 100)
     }
 
     function l(s) {
         const m = e.data.template,
             v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + s + "__"),
             j = document.querySelector("input[name=" + v + "]");
         parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + s + "-" + a).style.display = "none", c()
@@ -1317,15 +1317,15 @@
     function o() {
         return t.jsx("div", {
             id: "info-" + a,
             children: t.jsx(ie, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(A, {
+                children: t.jsx(D, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
@@ -1409,15 +1409,15 @@
         return t.jsx("h1", {
             style: s,
             children: e.data.title
         })
     }
 
     function r() {
-        return e.data.info && t.jsx(Pe, {
+        return e.data.info && t.jsx(He, {
             data: {
                 text: e.data.info
             }
         })
     }
 
     function c() {
@@ -1440,20 +1440,20 @@
 
     function l() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(A, {
+            children: [t.jsx(D, {
                 onClick: o,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(A, {
+            }), t.jsx(D, {
                 onClick: h,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
@@ -1485,23 +1485,23 @@
     }
 
     function h(s) {
         s.preventDefault();
         var m = document.getElementById(n),
             x = new FormData(m);
         q("POST", e.data.url, function(j) {
-            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return U(), Oe(), ge(j);
-            var D = j.text;
+            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return U(), Ne(), ge(j);
+            var I = j.text;
             console.log(j), Object.keys(j.errors).map(function(C) {
-                if (C == "__all__") D = j.errors[C];
+                if (C == "__all__") I = j.errors[C];
                 else {
                     const M = m.querySelector("#" + C + "_error");
                     M.querySelector("span").innerHTML = j.errors[C], M.style.display = "block"
                 }
-            }), Q(D, !0)
+            }), Q(I, !0)
         }, x)
     }
     return d()
 }
 
 function G(e) {
     if (e === null || e === "") return "-";
@@ -1666,15 +1666,15 @@
     function o(u, g, f) {
         const p = document.getElementById("form-" + e.data.id);
         p.querySelector("input[name=" + n.calendar.field + "__day]").value = u || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = g || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = f || "", M()
     }
 
     function h() {
         if (n.calendar) {
-            const w = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+            const b = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
                 L = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 Z = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
@@ -1700,15 +1700,15 @@
                     display: "block",
                     width: 30,
                     height: 30,
                     margin: "auto",
                     cursor: "pointer",
                     lineHeight: "2rem"
                 },
-                O = {
+                N = {
                     padding: 10,
                     textAlign: "center"
                 },
                 J = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
@@ -1746,15 +1746,15 @@
                             style: {
                                 margin: 0
                             },
                             children: [L[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
                             className: T,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(b, {
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(w, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => o(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
@@ -1767,15 +1767,15 @@
                             onClick: () => o(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
                     style: Z,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
-                            children: w.map(ee => t.jsx("th", {
+                            children: b.map(ee => t.jsx("th", {
                                 children: ee
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
                         children: u.map(ee => t.jsx("tr", {
                             children: ee.map(B => t.jsxs("td", {
                                 style: _,
@@ -1784,27 +1784,27 @@
                                     children: B.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
                                         children: B.date
                                     }) : B.date + B.today
                                 }), B.total && t.jsx("div", {
-                                    style: O,
+                                    style: N,
                                     onClick: () => o(B.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
                                         style: W,
                                         children: t.jsx("span", {
                                             style: {
                                                 textDecoration: B.selected ? "underline" : "normal"
                                             },
                                             children: B.total
                                         })
                                     })
                                 }), !B.total && t.jsx("div", {
-                                    style: O,
+                                    style: N,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
             })
@@ -1847,15 +1847,15 @@
                 style: f,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center",
                         textAlign: "right"
                     },
                     children: u.actions.map(function(p) {
-                        return t.jsx(N, {
+                        return t.jsx(O, {
                             data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
@@ -1868,15 +1868,15 @@
             }), t.jsx("td", {
                 style: f,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
                     children: u.actions.map(function(p) {
-                        return t.jsx(N, {
+                        return t.jsx(O, {
                             data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
@@ -1916,16 +1916,16 @@
         const f = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
         f.value = u, M()
     }
 
     function j() {
         const u = document.getElementById("form-" + e.data.id);
         if (u) {
-            const w = u.querySelector("input[name=page]");
-            w && (w.value = n.pagination.page.current)
+            const b = u.querySelector("input[name=page]");
+            b && (b.value = n.pagination.page.current)
         }
         const g = {
                 display: "flex",
                 justifyContent: "space-between",
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
@@ -1947,17 +1947,17 @@
                 children: [t.jsxs("div", {
                     style: f,
                     children: ["Exibir", t.jsx("select", {
                         style: p,
                         name: "page_size",
                         onChange: () => v(1),
                         value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(w) {
+                        children: n.pagination.page.sizes.map(function(b) {
                             return t.jsx("option", {
-                                children: w
+                                children: b
                             }, Math.random())
                         })
                     })]
                 }), t.jsx("div", {
                     style: f,
                     children: "|"
                 }), t.jsxs("div", {
@@ -1976,45 +1976,45 @@
                         style: {
                             width: 30,
                             marginLeft: 10,
                             marginRight: 10,
                             height: "2rem",
                             textAlign: "center"
                         },
-                        onKeyDown: function(w) {
-                            w.key == "Enter" && (w.preventDefault(), v(w.target.value < 0 ? 1 : Math.min(w.target.value, n.pagination.page.total)))
+                        onKeyDown: function(b) {
+                            b.key == "Enter" && (b.preventDefault(), v(b.target.value < 0 ? 1 : Math.min(b.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
                         style: f,
                         children: "|"
-                    }), n.pagination.page.previous && t.jsx(A, {
+                    }), n.pagination.page.previous && t.jsx(D, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
                         onClick: () => v(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(A, {
+                    }), n.pagination.page.next && t.jsx(D, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
                         onClick: () => v(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function D() {
+    function I() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(u) {
-                return t.jsx(N, {
+                return t.jsx(O, {
                     data: u,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
@@ -2034,34 +2034,34 @@
                 children: [t.jsxs(X, {
                     width: 250,
                     children: [g && t.jsx("div", {
                         style: u,
                         children: t.jsx(Y, {
                             data: p
                         })
-                    }), f && n.filters.map(function(w) {
-                        return w.type != "hidden" && t.jsx("div", {
+                    }), f && n.filters.map(function(b) {
+                        return b.type != "hidden" && t.jsx("div", {
                             style: u,
                             children: t.jsx(Y, {
-                                data: w
+                                data: b
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         style: u,
-                        children: t.jsx(A, {
+                        children: t.jsx(D, {
                             onClick: M,
                             label: "Filtrar",
                             default: !0
                         })
                     })]
-                }), f && n.filters.map(function(w) {
-                    return w.type == "hidden" && t.jsx("div", {
+                }), f && n.filters.map(function(b) {
+                    return b.type == "hidden" && t.jsx("div", {
                         style: u,
                         children: t.jsx(Y, {
-                            data: w
+                            data: b
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
@@ -2086,19 +2086,19 @@
                                 data: g
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [D(), l(), C(), h(), x(), j()]
+            children: [I(), l(), C(), h(), x(), j()]
         })
     }
 
-    function H() {
+    function P() {
         window[e.data.id] = () => M();
         const u = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
@@ -2112,29 +2112,29 @@
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
                 }), c(), E()]
             })
         })
     }
-    return H()
+    return P()
 }
 
 function ae(e) {
     function n() {
         return e.data.url ? t.jsx(Qe, {
             data: e.data
-        }) : t.jsx(we, {
+        }) : t.jsx(be, {
             data: e.data
         })
     }
     return n()
 }
 
-function we(e) {
+function be(e) {
     function n() {
         const a = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsxs("div", {
@@ -2157,29 +2157,29 @@
         })
     }
 
     function i() {
         return window[n] = () => c(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: t.jsx(we, {
+            children: t.jsx(be, {
                 data: a,
                 width: 100
             })
         })
     }
     return i()
 }
 
 function Ke(e) {
     const n = Math.random(),
         [a, r] = S.useState(e.data);
 
     function c() {
-        return t.jsx(be, {
+        return t.jsx(we, {
             data: a
         })
     }
 
     function i() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
@@ -2235,15 +2235,15 @@
     }
 
     function l() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
             children: a.map(function(d) {
-                return t.jsx(N, {
+                return t.jsx(O, {
                     data: d,
                     default: !0
                 }, Math.random())
             })
         })
     }
     return l()
@@ -2269,15 +2269,15 @@
                 data: e.data
             })]
         })
     }
     return n()
 }
 
-function be(e) {
+function we(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
                 alignItems: "baseline"
             },
             r = {
@@ -2288,15 +2288,15 @@
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
                 "data-label": k(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(c) {
-                    return t.jsx(N, {
+                    return t.jsx(O, {
                         data: c,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
@@ -2324,15 +2324,15 @@
         })
     }
     return r()
 }
 
 function nt(e) {
     function n() {
-        return t.jsx(be, {
+        return t.jsx(we, {
             data: e.data
         })
     }
 
     function a() {
         const c = {
             backgroundColor: "white"
@@ -3057,27 +3057,27 @@
             onClick: n,
             children: t.jsxs(z, {
                 href: i.url,
                 dataLabel: k(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [l == 0 && t.jsx(b, {
+                children: [l == 0 && t.jsx(w, {
                     icon: i.icon || "dot-circle",
                     style: o
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: d,
             "data-label": k(i.label),
-            children: [l == 0 && t.jsx(b, {
+            children: [l == 0 && t.jsx(w, {
                 icon: i.icon || "dot-circle",
                 style: o
-            }), i.label, t.jsx(b, {
+            }), i.label, t.jsx(w, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
@@ -3127,39 +3127,41 @@
             h = new Uint8Array(o.length);
         for (let s = 0; s < o.length; ++s) h[s] = o.charCodeAt(s);
         return h
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
-            const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
-            i.pushManager.subscribe({
-                userVisibleOnly: !0,
-                applicationServerKey: l
-            }).then(function(d) {
-                if (console.log(d), n = JSON.stringify(d), console.log(n), d) {
-                    alert("Notificação ativada com sucesso.");
-                    var o = new FormData;
-                    o.append("subscription", n), q("POST", "/api/pushsubscribe/", function(h) {
-                        console.log(h)
-                    }, o)
-                } else {
-                    alert("Problema ao ativar notificações.");
-                    return
-                }
-            }).catch(function(d) {
-                alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", d)
-            })
+            if (i) {
+                const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
+                i.pushManager.subscribe({
+                    userVisibleOnly: !0,
+                    applicationServerKey: l
+                }).then(function(d) {
+                    if (console.log(d), n = JSON.stringify(d), console.log(n), d) {
+                        alert("Notificação ativada com sucesso.");
+                        var o = new FormData;
+                        o.append("subscription", n), q("POST", "/api/pushsubscribe/", function(h) {
+                            console.log(h)
+                        }, o)
+                    } else {
+                        alert("Problema ao ativar notificações.");
+                        return
+                    }
+                }).catch(function(d) {
+                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", d)
+                })
+            } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
     function c() {
-        return t.jsx(b, {
+        return t.jsx(w, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
@@ -3182,15 +3184,15 @@
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function wt(e) {
+function bt(e) {
     S.useEffect(() => {
         const o = localStorage.getItem("message");
         o && (localStorage.removeItem("message"), Q(o)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h.style.display = window.innerWidth < 800 ? "none" : "block"
         })
     }, []);
@@ -3219,15 +3221,15 @@
             };
         return e.data.navbar ? t.jsxs("div", {
             style: o,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [t.jsx(b, {
+                children: [t.jsx(w, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3251,15 +3253,15 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
@@ -3268,27 +3270,27 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && t.jsx(ve, {
                     data: h,
                     style: {
                         padding: 10
@@ -3361,15 +3363,15 @@
                 children: [c(), i()]
             })]
         })
     }
     return d()
 }
 
-function bt(e) {
+function wt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
@@ -3403,15 +3405,15 @@
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function St(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(b, {
+        return e.data.icon ? i.done ? t.jsx(w, {
             style: {
                 marginTop: 12
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -3591,15 +3593,15 @@
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(l => t.jsxs(z, {
                     href: l.url,
                     style: r,
                     dataLabel: l.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(b, {
+                        children: t.jsx(w, {
                             style: c,
                             icon: l.icon
                         })
                     }), t.jsx("div", {
                         style: i,
                         children: l.label
                     })]
@@ -3631,15 +3633,15 @@
 }
 
 function qt(e) {
     function n() {
         return e.data.url ? t.jsx(z, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(b, {
+            children: e.data.icon ? t.jsx(w, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
@@ -3676,29 +3678,29 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function At(e) {
+function Bt(e) {
     function n() {
         return t.jsx(X, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
                 children: t.jsx(y, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Bt(e) {
+function At(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -3723,15 +3725,15 @@
 }
 y.register = function(e, n) {
     Se[e] = n
 };
 y.render = function(e) {
     re = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-y.register("counter", e => t.jsx(Bt, {
+y.register("counter", e => t.jsx(At, {
     data: e
 }));
 y.register("form", e => t.jsx(Ye, {
     data: e
 }));
 y.register("queryset", e => t.jsx(Xe, {
     data: e
@@ -3753,15 +3755,15 @@
 }));
 y.register("statistics", e => t.jsx(gt, {
     data: e
 }));
 y.register("image", e => t.jsx(jt, {
     data: e
 }));
-y.register("banner", e => t.jsx(bt, {
+y.register("banner", e => t.jsx(wt, {
     data: e
 }));
 y.register("map", e => t.jsx(kt, {
     data: e
 }));
 y.register("steps", e => t.jsx(St, {
     data: e
@@ -3792,70 +3794,42 @@
 }));
 y.register("file_viewer", e => t.jsx(It, {
     data: e
 }));
 y.register("response", e => t.jsx(Ie, {
     data: e
 }));
-y.register("application", e => t.jsx(wt, {
+y.register("application", e => t.jsx(bt, {
     data: e
 }));
 y.register("iconset", e => t.jsx(Me, {
     data: e
 }));
-y.register("grid", e => t.jsx(At, {
+y.register("grid", e => t.jsx(Bt, {
     data: e
 }));
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), me ? (window.application = JSON.parse(me), window.configure(), q("GET", I(e), function(n) {
+    }, "", e), me ? (window.application = JSON.parse(me), q("GET", A(e), function(n) {
         window.application.content = n, re.render(t.jsx(y, {
             data: window.application
         }, Math.random()))
     })) : q("GET", Lt, function(a) {
-        window.application = a, window.configure(), localStorage.setItem("application", JSON.stringify(window.application)), q("GET", I(e), function(r) {
+        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(r) {
             window.application.content = r, re.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     })
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 ? (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), q("GET", I(e), function(n) {
+    }, "", e), q("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-window.configure = function() {
-    const e = window.application.icon || "/static/images/logo.png";
-    [{
-        rel: "manifest",
-        href: I("/api/manifest/")
-    }, {
-        rel: "icon",
-        type: "image/png",
-        href: I(e)
-    }, {
-        rel: "apple-touch-icon",
-        sizes: "128x128",
-        href: I(e)
-    }, {
-        rel: "icon",
-        sizes: "192x192",
-        href: I(e)
-    }].forEach(function(n) {
-        const a = document.createElement("link");
-        Object.keys(n).forEach(r => a.setAttribute(r, n[r])), document.querySelector("head").appendChild(a)
-    }), "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.register("/static/js/service-worker.js", {
-        type: "module"
-    }).then(function(n) {
-        console.log("Service worker registered!")
-    }).catch(function(n) {
-        console.error("Service worker error:", n)
-    }) : console.log("Push messaging is not supported!")
-};
-y.render(P.createRoot(document.getElementById("root")));
+y.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.1.6/slth/static/js/peerjs.min.js` & `pyslth-0.1.7/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/qrcode.min.js` & `pyslth-0.1.7/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/react-trigger-change.js` & `pyslth-0.1.7/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/react.min.js` & `pyslth-0.1.7/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/service-worker.js` & `pyslth-0.1.7/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/vanilla-masker.js` & `pyslth-0.1.7/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/static/js/vanilla-masker.min.js` & `pyslth-0.1.7/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/statistics.py` & `pyslth-0.1.7/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/tests.py` & `pyslth-0.1.7/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/urls.py` & `pyslth-0.1.7/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/utils.py` & `pyslth-0.1.7/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.6/slth/views.py` & `pyslth-0.1.7/slth/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 from django.conf import settings
 from .models import Token
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .exceptions import JsonResponseException
 from .serializer import serialize
 from .utils import build_url
-
+from slth import APPLICATON
 from django.shortcuts import render
 
 def index(request, path=None):
     vite = not socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect_ex(('127.0.0.1',5173))
-    return render(request, 'index.html', dict(vite=vite))
+    return render(request, 'index.html', dict(vite=vite, application=APPLICATON))
+
+def service_worker(request):
+    return render(request, 'service-worker.js', content_type='text/javascript')
 
 @csrf_exempt
 def dispatcher(request, **kwargs):
     if request.method == 'OPTIONS':
         return ApiResponse({})
     else:
         if(1 and 'application' not in request.path and 'test' not in sys.argv): import time; time.sleep(0)
```

