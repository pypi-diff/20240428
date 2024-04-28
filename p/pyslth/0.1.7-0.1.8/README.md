# Comparing `tmp/pyslth-0.1.7.tar.gz` & `tmp/pyslth-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.1.7.tar", last modified: Sun Apr 28 00:52:03 2024, max compression
+gzip compressed data, was "pyslth-0.1.8.tar", last modified: Sun Apr 28 01:11:18 2024, max compression
```

## Comparing `pyslth-0.1.7.tar` & `pyslth-0.1.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.809836 pyslth-0.1.7/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.7/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 00:52:03.809620 pyslth-0.1.7/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.779087 pyslth-0.1.7/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1723 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-28 00:52:03.000000 pyslth-0.1.7/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.7/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-28 00:52:03.809897 pyslth-0.1.7/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-28 00:50:05.000000 pyslth-0.1.7/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.785715 pyslth-0.1.7/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.7/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.7/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.788911 pyslth-0.1.7/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.7/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.7/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.1.7/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.7/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.7/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.789462 pyslth-0.1.7/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.790126 pyslth-0.1.7/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.7/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.7/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.792663 pyslth-0.1.7/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.7/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.7/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.7/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.1.7/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.7/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.7/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.7/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.793164 pyslth-0.1.7/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.7/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.7/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.7/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.793492 pyslth-0.1.7/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.794764 pyslth-0.1.7/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.797074 pyslth-0.1.7/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.7/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.7/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.799185 pyslth-0.1.7/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.7/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.7/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.7/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.7/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.808821 pyslth-0.1.7/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    79731 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-28 00:51:36.000000 pyslth-0.1.7/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/slth.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.7/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 00:52:03.809330 pyslth-0.1.7/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.1.7/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.7/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.7/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.7/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.7/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.1.7/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.060392 pyslth-0.1.8/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.8/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 01:11:18.060179 pyslth-0.1.8/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.030859 pyslth-0.1.8/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1723 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.8/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-28 01:11:18.060455 pyslth-0.1.8/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-28 01:10:54.000000 pyslth-0.1.8/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.036938 pyslth-0.1.8/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.8/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.8/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.037568 pyslth-0.1.8/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.8/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.8/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.1.8/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.8/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.8/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.037922 pyslth-0.1.8/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.038644 pyslth-0.1.8/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.8/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.8/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.040874 pyslth-0.1.8/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.8/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.8/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.8/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.1.8/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.8/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.8/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.8/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.041377 pyslth-0.1.8/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.8/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.8/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.8/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.041686 pyslth-0.1.8/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.042949 pyslth-0.1.8/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.049536 pyslth-0.1.8/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.8/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.8/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.051591 pyslth-0.1.8/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.8/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.8/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.8/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.8/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.059409 pyslth-0.1.8/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    79781 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.059888 pyslth-0.1.8/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.1.8/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.8/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.8/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.8/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.1.8/slth/views.py
```

### Comparing `pyslth-0.1.7/PKG-INFO` & `pyslth-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.7
+Version: 0.1.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.7/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.8/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.7
+Version: 0.1.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.7/pyslth.egg-info/SOURCES.txt` & `pyslth-0.1.8/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/setup.py` & `pyslth-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.1.7/slth/__init__.py` & `pyslth-0.1.8/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/components.py` & `pyslth-0.1.8/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/db/models.py` & `pyslth-0.1.8/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/endpoints.py` & `pyslth-0.1.8/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/factory.py` & `pyslth-0.1.8/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/forms.py` & `pyslth-0.1.8/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/management/commands/integration_test.py` & `pyslth-0.1.8/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/management/commands/sync.py` & `pyslth-0.1.8/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/migrations/0001_initial.py` & `pyslth-0.1.8/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.8/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/models.py` & `pyslth-0.1.8/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/permissions.py` & `pyslth-0.1.8/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/queryset.py` & `pyslth-0.1.8/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/roles.py` & `pyslth-0.1.8/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/selenium/__init__.py` & `pyslth-0.1.8/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/selenium/browser.py` & `pyslth-0.1.8/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/serializer.py` & `pyslth-0.1.8/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/fontawesome.min.css` & `pyslth-0.1.8/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/fonts/Eina02-Bold.f8011405.ttf` & `pyslth-0.1.8/slth/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/fonts/Eina02-Regular.2e682693.ttf` & `pyslth-0.1.8/slth/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `pyslth-0.1.8/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.1.8/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/slth.css` & `pyslth-0.1.8/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/css/solid.min.css` & `pyslth-0.1.8/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/images/logo.png` & `pyslth-0.1.8/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/images/logo.svg` & `pyslth-0.1.8/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/images/user.png` & `pyslth-0.1.8/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/echarts.min.js` & `pyslth-0.1.8/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/index.min.js` & `pyslth-0.1.8/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/lib.min.js` & `pyslth-0.1.8/slth/static/js/lib.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3822,14 +3822,14 @@
             window.application.content = r, re.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     })
 };
 window.load = function(e) {
-    e.indexOf(window.origin) >= 0 ? (e != document.location.href && window.history.pushState({
+    e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
     }, "", e), q("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
 y.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.1.7/slth/static/js/peerjs.min.js` & `pyslth-0.1.8/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/qrcode.min.js` & `pyslth-0.1.8/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/react-trigger-change.js` & `pyslth-0.1.8/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/react.min.js` & `pyslth-0.1.8/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/vanilla-masker.js` & `pyslth-0.1.8/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/static/js/vanilla-masker.min.js` & `pyslth-0.1.8/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/statistics.py` & `pyslth-0.1.8/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/templates/index.html` & `pyslth-0.1.8/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/templates/service-worker.js` & `pyslth-0.1.8/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/tests.py` & `pyslth-0.1.8/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/urls.py` & `pyslth-0.1.8/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/utils.py` & `pyslth-0.1.8/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.7/slth/views.py` & `pyslth-0.1.8/slth/views.py`

 * *Files identical despite different names*

