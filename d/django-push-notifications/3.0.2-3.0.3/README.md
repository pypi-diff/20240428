# Comparing `tmp/django-push-notifications-3.0.2.tar.gz` & `tmp/django-push-notifications-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-push-notifications-3.0.2.tar", last modified: Sun Oct 29 17:10:58 2023, max compression
+gzip compressed data, was "django-push-notifications-3.0.3.tar", last modified: Sat Apr 27 23:09:01 2024, max compression
```

## Comparing `django-push-notifications-3.0.2.tar` & `django-push-notifications-3.0.3.tar`

### file list

```diff
@@ -1,81 +1,85 @@
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:58.000463 django-push-notifications-3.0.2/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      288 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/.editorconfig
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.952462 django-push-notifications-3.0.2/.github/
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.960462 django-push-notifications-3.0.2/.github/workflows/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1021 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/.github/workflows/release.yml
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1271 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/.github/workflows/test.yml
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      193 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/.gitignore
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      415 2023-10-28 21:35:56.000000 django-push-notifications-3.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      436 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/ACKNOWLEDGEMENTS.md
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     5682 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/CHANGELOG.md
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2375 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1774 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/CONTRIBUTING.md
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1074 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/LICENSE
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)       55 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/MANIFEST.in
--rw-r--r--   0 jscarlett  (1000) jscarlett  (1000)    19279 2023-10-29 17:10:58.000463 django-push-notifications-3.0.2/PKG-INFO
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)    17717 2023-10-29 16:59:44.000000 django-push-notifications-3.0.2/README.rst
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.964462 django-push-notifications-3.0.2/django_push_notifications.egg-info/
--rw-r--r--   0 jscarlett  (1000) jscarlett  (1000)    19279 2023-10-29 17:10:57.000000 django-push-notifications-3.0.2/django_push_notifications.egg-info/PKG-INFO
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2055 2023-10-29 17:10:57.000000 django-push-notifications-3.0.2/django_push_notifications.egg-info/SOURCES.txt
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)        1 2023-10-29 17:10:57.000000 django-push-notifications-3.0.2/django_push_notifications.egg-info/dependency_links.txt
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      118 2023-10-29 17:10:57.000000 django-push-notifications-3.0.2/django_push_notifications.egg-info/requires.txt
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)       19 2023-10-29 17:10:57.000000 django-push-notifications-3.0.2/django_push_notifications.egg-info/top_level.txt
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.964462 django-push-notifications-3.0.2/docs/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2467 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/docs/APNS.rst
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     6782 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/docs/WebPush.rst
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.972463 django-push-notifications-3.0.2/push_notifications/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      224 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/__init__.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     4383 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/admin.py
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.972463 django-push-notifications-3.0.2/push_notifications/api/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/api/__init__.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     6382 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/api/rest_framework.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     5183 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/apns.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      128 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/compat.py
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.972463 django-push-notifications-3.0.2/push_notifications/conf/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      527 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/conf/__init__.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)    12804 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/conf/app.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      181 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/conf/appmodel.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1844 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/conf/base.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     5529 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/conf/legacy.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      365 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/exceptions.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     3523 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/fields.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     7319 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/gcm.py
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.976462 django-push-notifications-3.0.2/push_notifications/migrations/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2534 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0001_initial.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      444 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0002_auto_20160106_0850.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1416 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0003_wnsdevice.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      605 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0004_fcm.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1261 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0005_applicationid.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1856 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0006_webpushdevice.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1140 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0007_uniquesetting.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      616 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0008_webpush_add_edge.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      502 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/0009_alter_apnsdevice_device_id.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/migrations/__init__.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     7172 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/push_notifications/models.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2023 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/settings.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1542 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/push_notifications/webpush.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)    11319 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/push_notifications/wns.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      228 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/pyproject.toml
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1319 2023-10-29 17:10:58.000463 django-push-notifications-3.0.2/setup.cfg
--rwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)      330 2023-10-28 22:01:15.000000 django-push-notifications-3.0.2/setup.py
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.992463 django-push-notifications-3.0.2/tests/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/__init__.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2221 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/responses.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      496 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/tests/settings.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      520 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/tests/settings_unique.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     4494 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_apns_models.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     4164 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_apns_push_payload.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     7087 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_app_config.py
-drwxrwxr-x   0 jscarlett  (1000) jscarlett  (1000)        0 2023-10-29 17:10:57.996463 django-push-notifications-3.0.2/tests/test_data/
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     4248 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_data/good_revoked.pem
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     3900 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_data/good_with_passwd.pem
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1992 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_data/without_private.pem
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)      995 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_fields.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     3213 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_gcm_push_payload.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1936 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/tests/test_legacy_config.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)    19720 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_models.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     4503 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/tests/test_rest_framework.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     2945 2023-10-08 03:54:49.000000 django-push-notifications-3.0.2/tests/test_webpush.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     5330 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/test_wns.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1618 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tests/tst_unique.py
--rw-rw-r--   0 jscarlett  (1000) jscarlett  (1000)     1124 2023-10-08 01:59:40.000000 django-push-notifications-3.0.2/tox.ini
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.784536 django-push-notifications-3.0.3/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      288 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/.editorconfig
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.566884 django-push-notifications-3.0.3/.github/
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.580247 django-push-notifications-3.0.3/.github/workflows/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1021 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/.github/workflows/release.yml
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1264 2024-04-27 23:04:03.000000 django-push-notifications-3.0.3/.github/workflows/test.yml
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      193 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/.gitignore
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      415 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      436 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/ACKNOWLEDGEMENTS.md
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     5682 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/CHANGELOG.md
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2375 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1774 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/CONTRIBUTING.md
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1074 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/LICENSE
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)       55 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/MANIFEST.in
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    19312 2024-04-27 23:09:01.783784 django-push-notifications-3.0.3/PKG-INFO
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    17728 2024-04-27 23:04:03.000000 django-push-notifications-3.0.3/README.rst
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.584629 django-push-notifications-3.0.3/django_push_notifications.egg-info/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    19312 2024-04-27 23:09:01.000000 django-push-notifications-3.0.3/django_push_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2189 2024-04-27 23:09:01.000000 django-push-notifications-3.0.3/django_push_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)        1 2024-04-27 23:09:01.000000 django-push-notifications-3.0.3/django_push_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      146 2024-04-27 23:09:01.000000 django-push-notifications-3.0.3/django_push_notifications.egg-info/requires.txt
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)       19 2024-04-27 23:09:01.000000 django-push-notifications-3.0.3/django_push_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.592945 django-push-notifications-3.0.3/docs/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2467 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/docs/APNS.rst
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     3168 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/docs/FCM.rst
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     6782 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/docs/WebPush.rst
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.635687 django-push-notifications-3.0.3/push_notifications/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      224 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/__init__.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     5172 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/admin.py
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.640330 django-push-notifications-3.0.3/push_notifications/api/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)        0 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/api/__init__.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     6382 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/api/rest_framework.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     5183 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/apns.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      128 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/compat.py
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.669210 django-push-notifications-3.0.3/push_notifications/conf/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      527 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/conf/__init__.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    11662 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/conf/app.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      181 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/conf/appmodel.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1577 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/conf/base.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     4693 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/conf/legacy.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      365 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/exceptions.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     3523 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/fields.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     6271 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/gcm.py
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.700801 django-push-notifications-3.0.3/push_notifications/migrations/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2534 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0001_initial.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      444 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0002_auto_20160106_0850.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1416 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0003_wnsdevice.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      605 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0004_fcm.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1261 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0005_applicationid.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1856 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0006_webpushdevice.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1140 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0007_uniquesetting.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      616 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0008_webpush_add_edge.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      502 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/0009_alter_apnsdevice_device_id.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      732 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/migrations/0010_alter_gcmdevice_options_and_more.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)        0 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/migrations/__init__.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     7621 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/models.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1779 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/push_notifications/settings.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1542 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/webpush.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    11319 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/push_notifications/wns.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      228 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/pyproject.toml
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1307 2024-04-27 23:09:01.785924 django-push-notifications-3.0.3/setup.cfg
+-rwxr-xr-x   0 jamaalscarlett   (503) staff       (20)      332 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/setup.py
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.774855 django-push-notifications-3.0.3/tests/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)        0 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/__init__.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      314 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/responses.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      496 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/settings.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      520 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/settings_unique.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     3893 2024-04-27 23:04:03.000000 django-push-notifications-3.0.3/tests/test_admin.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     4494 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_apns_models.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     4164 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_apns_push_payload.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     5554 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/test_app_config.py
+drwxr-xr-x   0 jamaalscarlett   (503) staff       (20)        0 2024-04-27 23:09:01.781897 django-push-notifications-3.0.3/tests/test_data/
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     4248 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_data/good_revoked.pem
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     3900 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_data/good_with_passwd.pem
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1992 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_data/without_private.pem
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     3683 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/test_dict_to_message.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      995 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_fields.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2334 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/test_gcm_push_payload.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)      930 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/test_legacy_config.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)    16269 2024-04-26 01:51:31.000000 django-push-notifications-3.0.3/tests/test_models.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     4503 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_rest_framework.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     2945 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_webpush.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     5330 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/test_wns.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1618 2023-10-18 14:08:18.000000 django-push-notifications-3.0.3/tests/tst_unique.py
+-rw-r--r--   0 jamaalscarlett   (503) staff       (20)     1132 2024-04-27 23:04:03.000000 django-push-notifications-3.0.3/tox.ini
```

### Comparing `django-push-notifications-3.0.2/.github/workflows/release.yml` & `django-push-notifications-3.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/.github/workflows/test.yml` & `django-push-notifications-3.0.3/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9']
+        python-version: ['3.7', '3.8', '3.9']
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `django-push-notifications-3.0.2/CHANGELOG.md` & `django-push-notifications-3.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/CODE_OF_CONDUCT.md` & `django-push-notifications-3.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/CONTRIBUTING.md` & `django-push-notifications-3.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/LICENSE` & `django-push-notifications-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/PKG-INFO` & `django-push-notifications-3.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-push-notifications
-Version: 3.0.2
+Version: 3.0.3
 Summary: Send push notifications to mobile devices through GCM, APNS or WNS and to WebPush (Chrome, Firefox and Opera) in Django
 Home-page: https://github.com/jazzband/django-push-notifications
 Download-URL: https://github.com/jazzband/django-push-notifications/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -14,30 +14,31 @@
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=2.2
 Provides-Extra: apns
 Requires-Dist: apns2>=0.3.0; extra == "apns"
 Requires-Dist: importlib-metadata; python_version < "3.8" and extra == "apns"
 Requires-Dist: Django>=2.2; extra == "apns"
 Provides-Extra: wp
 Requires-Dist: pywebpush>=1.3.0; extra == "wp"
+Provides-Extra: fcm
+Requires-Dist: firebase-admin<6,>=5; extra == "fcm"
 
 django-push-notifications
 =========================
 
 .. image:: https://jazzband.co/static/img/badge.svg
    :target: https://jazzband.co/
    :alt: Jazzband
@@ -64,52 +65,60 @@
 FCM/GCM, APNS, WNS or WebPush devices and in the action dropdown, select "Send test message" or "Send test message in bulk", accordingly.
 Note that sending a non-bulk test message to more than one device will just iterate over the devices and send multiple
 single messages.
 UPDATE_ON_DUPLICATE_REG_ID: Transform create of an existing Device (based on registration id) into a update. See below Update of device with duplicate registration ID for more details.
 
 Dependencies
 ------------
-- Python 3.6+
+- Python 3.7+
 - Django 2.2+
 - For the API module, Django REST Framework 3.7+ is required.
 - For WebPush (WP), pywebpush 1.3.0+ is required (optional). py-vapid 1.3.0+ is required for generating the WebPush private key; however this
   step does not need to occur on the application server.
 - For Apple Push (APNS), apns2 0.3+ is required (optional).
+- For FCM, firebase-admin 5+ is required (optional).
 
 Setup
 -----
 You can install the library directly from pypi using pip:
 
 .. code-block:: shell
 
-	$ pip install django-push-notifications[WP,APNS]
+	$ pip install django-push-notifications[WP,APNS,FCM]
 
 
 Edit your settings.py file:
 
 .. code-block:: python
 
 	INSTALLED_APPS = (
 		...
 		"push_notifications"
 	)
 
+	# Import the firebase service
+	from firebase_admin import auth
+
+	# Initialize the default app (either use `GOOGLE_APPLICATION_CREDENTIALS` environment variable, or pass a firebase_admin.credentials.Certificate instance)
+	default_app = firebase_admin.initialize_app()
+
 	PUSH_NOTIFICATIONS_SETTINGS = {
-		"FCM_API_KEY": "[your api key]",
-		"GCM_API_KEY": "[your api key]",
 		"APNS_CERTIFICATE": "/path/to/your/certificate.pem",
 		"APNS_TOPIC": "com.example.push_test",
 		"WNS_PACKAGE_SECURITY_ID": "[your package security id, e.g: 'ms-app://e-3-4-6234...']",
 		"WNS_SECRET_KEY": "[your app secret key, e.g.: 'KDiejnLKDUWodsjmewuSZkk']",
 		"WP_PRIVATE_KEY": "/path/to/your/private.pem",
 		"WP_CLAIMS": {'sub': "mailto:development@example.com"}
 	}
 
 .. note::
-    If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
+	To migrate from legacy FCM APIs to HTTP v1, see `docs/FCM <https://github.com/jazzband/django-push-notifications/blob/master/docs/FCM.rst>`_.
+
+.. note::
+	If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
 
 .. note::
 	If you are planning on running your project with ``APNS_USE_SANDBOX=True``, then make sure you have set the
 	*development* certificate as your ``APNS_CERTIFICATE``. Otherwise the app will not be able to connect to the correct host. See settings_ for details.
 
 
 For more information about how to generate certificates, see `docs/APNS <https://github.com/jazzband/django-push-notifications/blob/master/docs/APNS.rst>`_.
@@ -120,15 +129,14 @@
 
 .. _settings:
 
 Settings list
 -------------
 All settings are contained in a ``PUSH_NOTIFICATIONS_SETTINGS`` dict.
 
-In order to use FCM/GCM, you are required to include ``FCM_API_KEY`` or ``GCM_API_KEY``.
 For APNS, you are required to include ``APNS_CERTIFICATE``.
 For WNS, you need both the ``WNS_PACKAGE_SECURITY_KEY`` and the ``WNS_SECRET_KEY``.
 
 **General settings**
 
 - ``USER_MODEL``: Your user model of choice. Eg. ``myapp.User``. Defaults to ``settings.AUTH_USER_MODEL``.
 - ``UPDATE_ON_DUPLICATE_REG_ID``: Transform create of an existing Device (based on registration id) into a update. See below `Update of device with duplicate registration ID`_ for more details.
@@ -142,19 +150,16 @@
 - ``APNS_TEAM_ID``: 10-character Team ID you use for developing your company’s apps for iOS.
 - ``APNS_TOPIC``: The topic of the remote notification, which is typically the bundle ID for your app. If you omit this header and your APNs certificate does not specify multiple topics, the APNs server uses the certificate’s Subject as the default topic.
 - ``APNS_USE_ALTERNATIVE_PORT``: Use port 2197 for APNS, instead of default port 443.
 - ``APNS_USE_SANDBOX``: Use 'api.development.push.apple.com', instead of default host 'api.push.apple.com'. Default value depends on ``DEBUG`` setting of your environment: if ``DEBUG`` is True and you use production certificate, you should explicitly set ``APNS_USE_SANDBOX`` to False.
 
 **FCM/GCM settings**
 
-- ``FCM_API_KEY``: Your API key for Firebase Cloud Messaging.
-- ``FCM_POST_URL``: The full url that FCM notifications will be POSTed to. Defaults to https://fcm.googleapis.com/fcm/send.
+- ``FIREBASE_APP``: Firebase app instance that is used to send the push notification. If not provided, the app will be using the default app instance that you've instantiated with ``firebase_admin.initialize_app()``.
 - ``FCM_MAX_RECIPIENTS``: The maximum amount of recipients that can be contained per bulk message. If the ``registration_ids`` list is larger than that number, multiple bulk messages will be sent. Defaults to 1000 (the maximum amount supported by FCM).
-- ``FCM_ERROR_TIMEOUT``: The timeout on FCM POSTs.
-- ``GCM_API_KEY``, ``GCM_POST_URL``, ``GCM_MAX_RECIPIENTS``, ``GCM_ERROR_TIMEOUT``: Same parameters for GCM
 
 **WNS settings**
 
 - ``WNS_PACKAGE_SECURITY_KEY``: TODO
 - ``WNS_SECRET_KEY``: TODO
 
 **WP settings**
@@ -180,14 +185,24 @@
 	device.send_message("You've got mail")
 	# If you want to customize, send an extra dict and a None message.
 	# the extras dict will be mapped into the intent extras Bundle.
 	# For dicts where all values are keys this will be sent as url parameters,
 	# but for more complex nested collections the extras dict will be sent via
 	# the bulk message api.
 	device.send_message(None, extra={"foo": "bar"})
+	device.send_message(None, extra={"foo": "bar"}, use_fcm_notifications=False) # Silent message with custom data.
+
+  # You may also pass a Firebase message object.
+	device.send_message(messaging.Message(
+		notification=messaging.Notification(
+			title='Hello World',
+			body='What a beautiful day.'
+		),
+	))
+	# If you want to use gcm.send_message directly, you will have to use messaging.Message.
 
 	device = APNSDevice.objects.get(registration_id=apns_token)
 	device.send_message("You've got mail") # Alert message may only be sent as text.
 	device.send_message(None, badge=5) # No alerts but with badge.
 	device.send_message(None, content_available=1, extra={"foo": "bar"}) # Silent message with custom data.
 	# alert with title and body.
 	device.send_message(message={"title" : "Game Request", "body" : "Bob wants to play poker"}, extra={"foo": "bar"})
@@ -248,27 +263,25 @@
 .. code-block:: python
 
 	devices.send_message(
 		"Happy name day!",
 		badge=lambda token: APNSDevice.objects.get(registration_id=token).user.get_badge()
 	)
 
-Firebase vs Google Cloud Messaging
+Firebase
 ----------------------------------
 
-``django-push-notifications`` supports both Google Cloud Messaging and Firebase Cloud Messaging (which is now the officially supported messaging platform from Google). When registering a device, you must pass the ``cloud_message_type`` parameter to set the cloud type that matches the device needs.
-This is currently defaulting to ``'GCM'``, but may change to ``'FCM'`` at some point. You are encouraged to use the `officially supported library <https://developers.google.com/cloud-messaging/faq>`_.
+``django-push-notifications`` supports Firebase Cloud Messaging v1.
 
 When using FCM, ``django-push-notifications`` will automatically use the `notification and data messages format <https://firebase.google.com/docs/cloud-messaging/concept-options#notifications_and_data_messages>`_ to be conveniently handled by Firebase devices. You may want to check the payload to see if it matches your needs, and review your notification statuses in `FCM Diagnostic console <https://support.google.com/googleplay/android-developer/answer/2663268?hl=en>`_.
 
-
 .. code-block:: python
 
 	# Create a FCM device
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
+	fcm_device = GCMDevice.objects.create(registration_id="token", user=the_user)
 
 	# Send a notification message
 	fcm_device.send_message("This is a message")
 
 	# Send a notification message with additionnal payload
 	fcm_device.send_message("This is a enriched message", extra={"title": "Notification title", "icon": "icon_ressource"})
 
@@ -280,43 +293,40 @@
 
 	# Send a notification message with options
 	fcm_device.send_message("This is a message", time_to_live=3600)
 
 	# Send a data message only
 	fcm_device.send_message(None, extra={"other": "content", "misc": "data"})
 
-You can disable this default behaviour by setting ``use_fcm_notifications`` to ``False``.
-
-.. code-block:: python
 
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
 
-	# Send a data message with classic format
-	fcm_device.send_message("This is a message", use_fcm_notifications=False)
+Behind the scenes, a `Firebase Message <https://firebase.google.com/docs/reference/admin/dotnet/class/firebase-admin/messaging/message>`_ will be created.
+You can also create this yourself and pass it to the ``send_message`` method instead.
 
 
 Sending FCM/GCM messages to topic members
 -----------------------------------------
 FCM/GCM topic messaging allows your app server to send a message to multiple devices that have opted in to a particular topic. Based on the publish/subscribe model, topic messaging supports unlimited subscriptions per app. Developers can choose any topic name that matches the regular expression, "/topics/[a-zA-Z0-9-_.~%]+".
 Note: gcm_send_bulk_message must be used when sending messages to topic subscribers, and setting the first param to any value other than None will result in a 400 Http error.
 
 .. code-block:: python
 
-	from push_notifications.gcm import send_message
+	from push_notifications.gcm import send_message, dict_to_fcm_message
 
-        # First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
-        send_message(None, {"body": "Hello members of my_topic!"}, cloud_type="FCM", to="/topics/my_topic")
+	# Create message object from dictonary. You can also directly create a messaging.Message object.
+	message = dict_to_fcm_message({"body": "Hello members of my_topic!"})
+	# First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
+	send_message(None, message, to="/topics/my_topic")
 
 Reference: `FCM Documentation <https://firebase.google.com/docs/cloud-messaging/android/topic-messaging>`_
 
 Exceptions
 ----------
 
 - ``NotificationError(Exception)``: Base exception for all notification-related errors.
-- ``gcm.GCMError(NotificationError)``: An error was returned by GCM. This is never raised when using bulk notifications.
 - ``apns.APNSError(NotificationError)``: Something went wrong upon sending APNS notifications.
 - ``apns.APNSDataOverflow(APNSError)``: The APNS payload exceeds its maximum size and cannot be sent.
 
 Django REST Framework (DRF) support
 -----------------------------------
 
 ViewSets are available for both APNS and GCM devices in two permission flavors:
```

### Comparing `django-push-notifications-3.0.2/README.rst` & `django-push-notifications-3.0.3/django_push_notifications.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: django-push-notifications
+Version: 3.0.3
+Summary: Send push notifications to mobile devices through GCM, APNS or WNS and to WebPush (Chrome, Firefox and Opera) in Django
+Home-page: https://github.com/jazzband/django-push-notifications
+Download-URL: https://github.com/jazzband/django-push-notifications/tarball/master
+Author: Jerome Leclanche
+Author-email: jerome@leclan.ch
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: System :: Networking
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Django>=2.2
+Provides-Extra: apns
+Requires-Dist: apns2>=0.3.0; extra == "apns"
+Requires-Dist: importlib-metadata; python_version < "3.8" and extra == "apns"
+Requires-Dist: Django>=2.2; extra == "apns"
+Provides-Extra: wp
+Requires-Dist: pywebpush>=1.3.0; extra == "wp"
+Provides-Extra: fcm
+Requires-Dist: firebase-admin<6,>=5; extra == "fcm"
+
 django-push-notifications
 =========================
 
 .. image:: https://jazzband.co/static/img/badge.svg
    :target: https://jazzband.co/
    :alt: Jazzband
 
@@ -27,52 +65,60 @@
 FCM/GCM, APNS, WNS or WebPush devices and in the action dropdown, select "Send test message" or "Send test message in bulk", accordingly.
 Note that sending a non-bulk test message to more than one device will just iterate over the devices and send multiple
 single messages.
 UPDATE_ON_DUPLICATE_REG_ID: Transform create of an existing Device (based on registration id) into a update. See below Update of device with duplicate registration ID for more details.
 
 Dependencies
 ------------
-- Python 3.6+
+- Python 3.7+
 - Django 2.2+
 - For the API module, Django REST Framework 3.7+ is required.
 - For WebPush (WP), pywebpush 1.3.0+ is required (optional). py-vapid 1.3.0+ is required for generating the WebPush private key; however this
   step does not need to occur on the application server.
 - For Apple Push (APNS), apns2 0.3+ is required (optional).
+- For FCM, firebase-admin 5+ is required (optional).
 
 Setup
 -----
 You can install the library directly from pypi using pip:
 
 .. code-block:: shell
 
-	$ pip install django-push-notifications[WP,APNS]
+	$ pip install django-push-notifications[WP,APNS,FCM]
 
 
 Edit your settings.py file:
 
 .. code-block:: python
 
 	INSTALLED_APPS = (
 		...
 		"push_notifications"
 	)
 
+	# Import the firebase service
+	from firebase_admin import auth
+
+	# Initialize the default app (either use `GOOGLE_APPLICATION_CREDENTIALS` environment variable, or pass a firebase_admin.credentials.Certificate instance)
+	default_app = firebase_admin.initialize_app()
+
 	PUSH_NOTIFICATIONS_SETTINGS = {
-		"FCM_API_KEY": "[your api key]",
-		"GCM_API_KEY": "[your api key]",
 		"APNS_CERTIFICATE": "/path/to/your/certificate.pem",
 		"APNS_TOPIC": "com.example.push_test",
 		"WNS_PACKAGE_SECURITY_ID": "[your package security id, e.g: 'ms-app://e-3-4-6234...']",
 		"WNS_SECRET_KEY": "[your app secret key, e.g.: 'KDiejnLKDUWodsjmewuSZkk']",
 		"WP_PRIVATE_KEY": "/path/to/your/private.pem",
 		"WP_CLAIMS": {'sub': "mailto:development@example.com"}
 	}
 
 .. note::
-    If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
+	To migrate from legacy FCM APIs to HTTP v1, see `docs/FCM <https://github.com/jazzband/django-push-notifications/blob/master/docs/FCM.rst>`_.
+
+.. note::
+	If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
 
 .. note::
 	If you are planning on running your project with ``APNS_USE_SANDBOX=True``, then make sure you have set the
 	*development* certificate as your ``APNS_CERTIFICATE``. Otherwise the app will not be able to connect to the correct host. See settings_ for details.
 
 
 For more information about how to generate certificates, see `docs/APNS <https://github.com/jazzband/django-push-notifications/blob/master/docs/APNS.rst>`_.
@@ -83,15 +129,14 @@
 
 .. _settings:
 
 Settings list
 -------------
 All settings are contained in a ``PUSH_NOTIFICATIONS_SETTINGS`` dict.
 
-In order to use FCM/GCM, you are required to include ``FCM_API_KEY`` or ``GCM_API_KEY``.
 For APNS, you are required to include ``APNS_CERTIFICATE``.
 For WNS, you need both the ``WNS_PACKAGE_SECURITY_KEY`` and the ``WNS_SECRET_KEY``.
 
 **General settings**
 
 - ``USER_MODEL``: Your user model of choice. Eg. ``myapp.User``. Defaults to ``settings.AUTH_USER_MODEL``.
 - ``UPDATE_ON_DUPLICATE_REG_ID``: Transform create of an existing Device (based on registration id) into a update. See below `Update of device with duplicate registration ID`_ for more details.
@@ -105,19 +150,16 @@
 - ``APNS_TEAM_ID``: 10-character Team ID you use for developing your company’s apps for iOS.
 - ``APNS_TOPIC``: The topic of the remote notification, which is typically the bundle ID for your app. If you omit this header and your APNs certificate does not specify multiple topics, the APNs server uses the certificate’s Subject as the default topic.
 - ``APNS_USE_ALTERNATIVE_PORT``: Use port 2197 for APNS, instead of default port 443.
 - ``APNS_USE_SANDBOX``: Use 'api.development.push.apple.com', instead of default host 'api.push.apple.com'. Default value depends on ``DEBUG`` setting of your environment: if ``DEBUG`` is True and you use production certificate, you should explicitly set ``APNS_USE_SANDBOX`` to False.
 
 **FCM/GCM settings**
 
-- ``FCM_API_KEY``: Your API key for Firebase Cloud Messaging.
-- ``FCM_POST_URL``: The full url that FCM notifications will be POSTed to. Defaults to https://fcm.googleapis.com/fcm/send.
+- ``FIREBASE_APP``: Firebase app instance that is used to send the push notification. If not provided, the app will be using the default app instance that you've instantiated with ``firebase_admin.initialize_app()``.
 - ``FCM_MAX_RECIPIENTS``: The maximum amount of recipients that can be contained per bulk message. If the ``registration_ids`` list is larger than that number, multiple bulk messages will be sent. Defaults to 1000 (the maximum amount supported by FCM).
-- ``FCM_ERROR_TIMEOUT``: The timeout on FCM POSTs.
-- ``GCM_API_KEY``, ``GCM_POST_URL``, ``GCM_MAX_RECIPIENTS``, ``GCM_ERROR_TIMEOUT``: Same parameters for GCM
 
 **WNS settings**
 
 - ``WNS_PACKAGE_SECURITY_KEY``: TODO
 - ``WNS_SECRET_KEY``: TODO
 
 **WP settings**
@@ -143,14 +185,24 @@
 	device.send_message("You've got mail")
 	# If you want to customize, send an extra dict and a None message.
 	# the extras dict will be mapped into the intent extras Bundle.
 	# For dicts where all values are keys this will be sent as url parameters,
 	# but for more complex nested collections the extras dict will be sent via
 	# the bulk message api.
 	device.send_message(None, extra={"foo": "bar"})
+	device.send_message(None, extra={"foo": "bar"}, use_fcm_notifications=False) # Silent message with custom data.
+
+  # You may also pass a Firebase message object.
+	device.send_message(messaging.Message(
+		notification=messaging.Notification(
+			title='Hello World',
+			body='What a beautiful day.'
+		),
+	))
+	# If you want to use gcm.send_message directly, you will have to use messaging.Message.
 
 	device = APNSDevice.objects.get(registration_id=apns_token)
 	device.send_message("You've got mail") # Alert message may only be sent as text.
 	device.send_message(None, badge=5) # No alerts but with badge.
 	device.send_message(None, content_available=1, extra={"foo": "bar"}) # Silent message with custom data.
 	# alert with title and body.
 	device.send_message(message={"title" : "Game Request", "body" : "Bob wants to play poker"}, extra={"foo": "bar"})
@@ -211,27 +263,25 @@
 .. code-block:: python
 
 	devices.send_message(
 		"Happy name day!",
 		badge=lambda token: APNSDevice.objects.get(registration_id=token).user.get_badge()
 	)
 
-Firebase vs Google Cloud Messaging
+Firebase
 ----------------------------------
 
-``django-push-notifications`` supports both Google Cloud Messaging and Firebase Cloud Messaging (which is now the officially supported messaging platform from Google). When registering a device, you must pass the ``cloud_message_type`` parameter to set the cloud type that matches the device needs.
-This is currently defaulting to ``'GCM'``, but may change to ``'FCM'`` at some point. You are encouraged to use the `officially supported library <https://developers.google.com/cloud-messaging/faq>`_.
+``django-push-notifications`` supports Firebase Cloud Messaging v1.
 
 When using FCM, ``django-push-notifications`` will automatically use the `notification and data messages format <https://firebase.google.com/docs/cloud-messaging/concept-options#notifications_and_data_messages>`_ to be conveniently handled by Firebase devices. You may want to check the payload to see if it matches your needs, and review your notification statuses in `FCM Diagnostic console <https://support.google.com/googleplay/android-developer/answer/2663268?hl=en>`_.
 
-
 .. code-block:: python
 
 	# Create a FCM device
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
+	fcm_device = GCMDevice.objects.create(registration_id="token", user=the_user)
 
 	# Send a notification message
 	fcm_device.send_message("This is a message")
 
 	# Send a notification message with additionnal payload
 	fcm_device.send_message("This is a enriched message", extra={"title": "Notification title", "icon": "icon_ressource"})
 
@@ -243,43 +293,40 @@
 
 	# Send a notification message with options
 	fcm_device.send_message("This is a message", time_to_live=3600)
 
 	# Send a data message only
 	fcm_device.send_message(None, extra={"other": "content", "misc": "data"})
 
-You can disable this default behaviour by setting ``use_fcm_notifications`` to ``False``.
-
-.. code-block:: python
 
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
 
-	# Send a data message with classic format
-	fcm_device.send_message("This is a message", use_fcm_notifications=False)
+Behind the scenes, a `Firebase Message <https://firebase.google.com/docs/reference/admin/dotnet/class/firebase-admin/messaging/message>`_ will be created.
+You can also create this yourself and pass it to the ``send_message`` method instead.
 
 
 Sending FCM/GCM messages to topic members
 -----------------------------------------
 FCM/GCM topic messaging allows your app server to send a message to multiple devices that have opted in to a particular topic. Based on the publish/subscribe model, topic messaging supports unlimited subscriptions per app. Developers can choose any topic name that matches the regular expression, "/topics/[a-zA-Z0-9-_.~%]+".
 Note: gcm_send_bulk_message must be used when sending messages to topic subscribers, and setting the first param to any value other than None will result in a 400 Http error.
 
 .. code-block:: python
 
-	from push_notifications.gcm import send_message
+	from push_notifications.gcm import send_message, dict_to_fcm_message
 
-        # First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
-        send_message(None, {"body": "Hello members of my_topic!"}, cloud_type="FCM", to="/topics/my_topic")
+	# Create message object from dictonary. You can also directly create a messaging.Message object.
+	message = dict_to_fcm_message({"body": "Hello members of my_topic!"})
+	# First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
+	send_message(None, message, to="/topics/my_topic")
 
 Reference: `FCM Documentation <https://firebase.google.com/docs/cloud-messaging/android/topic-messaging>`_
 
 Exceptions
 ----------
 
 - ``NotificationError(Exception)``: Base exception for all notification-related errors.
-- ``gcm.GCMError(NotificationError)``: An error was returned by GCM. This is never raised when using bulk notifications.
 - ``apns.APNSError(NotificationError)``: Something went wrong upon sending APNS notifications.
 - ``apns.APNSDataOverflow(APNSError)``: The APNS payload exceeds its maximum size and cannot be sent.
 
 Django REST Framework (DRF) support
 -----------------------------------
 
 ViewSets are available for both APNS and GCM devices in two permission flavors:
```

### Comparing `django-push-notifications-3.0.2/django_push_notifications.egg-info/PKG-INFO` & `django-push-notifications-3.0.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: django-push-notifications
-Version: 3.0.2
-Summary: Send push notifications to mobile devices through GCM, APNS or WNS and to WebPush (Chrome, Firefox and Opera) in Django
-Home-page: https://github.com/jazzband/django-push-notifications
-Download-URL: https://github.com/jazzband/django-push-notifications/tarball/master
-Author: Jerome Leclanche
-Author-email: jerome@leclan.ch
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: System :: Networking
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: Django>=2.2
-Provides-Extra: apns
-Requires-Dist: apns2>=0.3.0; extra == "apns"
-Requires-Dist: importlib-metadata; python_version < "3.8" and extra == "apns"
-Requires-Dist: Django>=2.2; extra == "apns"
-Provides-Extra: wp
-Requires-Dist: pywebpush>=1.3.0; extra == "wp"
-
 django-push-notifications
 =========================
 
 .. image:: https://jazzband.co/static/img/badge.svg
    :target: https://jazzband.co/
    :alt: Jazzband
 
@@ -64,52 +27,60 @@
 FCM/GCM, APNS, WNS or WebPush devices and in the action dropdown, select "Send test message" or "Send test message in bulk", accordingly.
 Note that sending a non-bulk test message to more than one device will just iterate over the devices and send multiple
 single messages.
 UPDATE_ON_DUPLICATE_REG_ID: Transform create of an existing Device (based on registration id) into a update. See below Update of device with duplicate registration ID for more details.
 
 Dependencies
 ------------
-- Python 3.6+
+- Python 3.7+
 - Django 2.2+
 - For the API module, Django REST Framework 3.7+ is required.
 - For WebPush (WP), pywebpush 1.3.0+ is required (optional). py-vapid 1.3.0+ is required for generating the WebPush private key; however this
   step does not need to occur on the application server.
 - For Apple Push (APNS), apns2 0.3+ is required (optional).
+- For FCM, firebase-admin 5+ is required (optional).
 
 Setup
 -----
 You can install the library directly from pypi using pip:
 
 .. code-block:: shell
 
-	$ pip install django-push-notifications[WP,APNS]
+	$ pip install django-push-notifications[WP,APNS,FCM]
 
 
 Edit your settings.py file:
 
 .. code-block:: python
 
 	INSTALLED_APPS = (
 		...
 		"push_notifications"
 	)
 
+	# Import the firebase service
+	from firebase_admin import auth
+
+	# Initialize the default app (either use `GOOGLE_APPLICATION_CREDENTIALS` environment variable, or pass a firebase_admin.credentials.Certificate instance)
+	default_app = firebase_admin.initialize_app()
+
 	PUSH_NOTIFICATIONS_SETTINGS = {
-		"FCM_API_KEY": "[your api key]",
-		"GCM_API_KEY": "[your api key]",
 		"APNS_CERTIFICATE": "/path/to/your/certificate.pem",
 		"APNS_TOPIC": "com.example.push_test",
 		"WNS_PACKAGE_SECURITY_ID": "[your package security id, e.g: 'ms-app://e-3-4-6234...']",
 		"WNS_SECRET_KEY": "[your app secret key, e.g.: 'KDiejnLKDUWodsjmewuSZkk']",
 		"WP_PRIVATE_KEY": "/path/to/your/private.pem",
 		"WP_CLAIMS": {'sub': "mailto:development@example.com"}
 	}
 
 .. note::
-    If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
+	To migrate from legacy FCM APIs to HTTP v1, see `docs/FCM <https://github.com/jazzband/django-push-notifications/blob/master/docs/FCM.rst>`_.
+
+.. note::
+	If you need to support multiple mobile applications from a single Django application, see `Multiple Application Support <https://github.com/jazzband/django-push-notifications/wiki/Multiple-Application-Support>`_ for details.
 
 .. note::
 	If you are planning on running your project with ``APNS_USE_SANDBOX=True``, then make sure you have set the
 	*development* certificate as your ``APNS_CERTIFICATE``. Otherwise the app will not be able to connect to the correct host. See settings_ for details.
 
 
 For more information about how to generate certificates, see `docs/APNS <https://github.com/jazzband/django-push-notifications/blob/master/docs/APNS.rst>`_.
@@ -120,15 +91,14 @@
 
 .. _settings:
 
 Settings list
 -------------
 All settings are contained in a ``PUSH_NOTIFICATIONS_SETTINGS`` dict.
 
-In order to use FCM/GCM, you are required to include ``FCM_API_KEY`` or ``GCM_API_KEY``.
 For APNS, you are required to include ``APNS_CERTIFICATE``.
 For WNS, you need both the ``WNS_PACKAGE_SECURITY_KEY`` and the ``WNS_SECRET_KEY``.
 
 **General settings**
 
 - ``USER_MODEL``: Your user model of choice. Eg. ``myapp.User``. Defaults to ``settings.AUTH_USER_MODEL``.
 - ``UPDATE_ON_DUPLICATE_REG_ID``: Transform create of an existing Device (based on registration id) into a update. See below `Update of device with duplicate registration ID`_ for more details.
@@ -142,19 +112,16 @@
 - ``APNS_TEAM_ID``: 10-character Team ID you use for developing your company’s apps for iOS.
 - ``APNS_TOPIC``: The topic of the remote notification, which is typically the bundle ID for your app. If you omit this header and your APNs certificate does not specify multiple topics, the APNs server uses the certificate’s Subject as the default topic.
 - ``APNS_USE_ALTERNATIVE_PORT``: Use port 2197 for APNS, instead of default port 443.
 - ``APNS_USE_SANDBOX``: Use 'api.development.push.apple.com', instead of default host 'api.push.apple.com'. Default value depends on ``DEBUG`` setting of your environment: if ``DEBUG`` is True and you use production certificate, you should explicitly set ``APNS_USE_SANDBOX`` to False.
 
 **FCM/GCM settings**
 
-- ``FCM_API_KEY``: Your API key for Firebase Cloud Messaging.
-- ``FCM_POST_URL``: The full url that FCM notifications will be POSTed to. Defaults to https://fcm.googleapis.com/fcm/send.
+- ``FIREBASE_APP``: Firebase app instance that is used to send the push notification. If not provided, the app will be using the default app instance that you've instantiated with ``firebase_admin.initialize_app()``.
 - ``FCM_MAX_RECIPIENTS``: The maximum amount of recipients that can be contained per bulk message. If the ``registration_ids`` list is larger than that number, multiple bulk messages will be sent. Defaults to 1000 (the maximum amount supported by FCM).
-- ``FCM_ERROR_TIMEOUT``: The timeout on FCM POSTs.
-- ``GCM_API_KEY``, ``GCM_POST_URL``, ``GCM_MAX_RECIPIENTS``, ``GCM_ERROR_TIMEOUT``: Same parameters for GCM
 
 **WNS settings**
 
 - ``WNS_PACKAGE_SECURITY_KEY``: TODO
 - ``WNS_SECRET_KEY``: TODO
 
 **WP settings**
@@ -180,14 +147,24 @@
 	device.send_message("You've got mail")
 	# If you want to customize, send an extra dict and a None message.
 	# the extras dict will be mapped into the intent extras Bundle.
 	# For dicts where all values are keys this will be sent as url parameters,
 	# but for more complex nested collections the extras dict will be sent via
 	# the bulk message api.
 	device.send_message(None, extra={"foo": "bar"})
+	device.send_message(None, extra={"foo": "bar"}, use_fcm_notifications=False) # Silent message with custom data.
+
+  # You may also pass a Firebase message object.
+	device.send_message(messaging.Message(
+		notification=messaging.Notification(
+			title='Hello World',
+			body='What a beautiful day.'
+		),
+	))
+	# If you want to use gcm.send_message directly, you will have to use messaging.Message.
 
 	device = APNSDevice.objects.get(registration_id=apns_token)
 	device.send_message("You've got mail") # Alert message may only be sent as text.
 	device.send_message(None, badge=5) # No alerts but with badge.
 	device.send_message(None, content_available=1, extra={"foo": "bar"}) # Silent message with custom data.
 	# alert with title and body.
 	device.send_message(message={"title" : "Game Request", "body" : "Bob wants to play poker"}, extra={"foo": "bar"})
@@ -248,27 +225,25 @@
 .. code-block:: python
 
 	devices.send_message(
 		"Happy name day!",
 		badge=lambda token: APNSDevice.objects.get(registration_id=token).user.get_badge()
 	)
 
-Firebase vs Google Cloud Messaging
+Firebase
 ----------------------------------
 
-``django-push-notifications`` supports both Google Cloud Messaging and Firebase Cloud Messaging (which is now the officially supported messaging platform from Google). When registering a device, you must pass the ``cloud_message_type`` parameter to set the cloud type that matches the device needs.
-This is currently defaulting to ``'GCM'``, but may change to ``'FCM'`` at some point. You are encouraged to use the `officially supported library <https://developers.google.com/cloud-messaging/faq>`_.
+``django-push-notifications`` supports Firebase Cloud Messaging v1.
 
 When using FCM, ``django-push-notifications`` will automatically use the `notification and data messages format <https://firebase.google.com/docs/cloud-messaging/concept-options#notifications_and_data_messages>`_ to be conveniently handled by Firebase devices. You may want to check the payload to see if it matches your needs, and review your notification statuses in `FCM Diagnostic console <https://support.google.com/googleplay/android-developer/answer/2663268?hl=en>`_.
 
-
 .. code-block:: python
 
 	# Create a FCM device
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
+	fcm_device = GCMDevice.objects.create(registration_id="token", user=the_user)
 
 	# Send a notification message
 	fcm_device.send_message("This is a message")
 
 	# Send a notification message with additionnal payload
 	fcm_device.send_message("This is a enriched message", extra={"title": "Notification title", "icon": "icon_ressource"})
 
@@ -280,43 +255,40 @@
 
 	# Send a notification message with options
 	fcm_device.send_message("This is a message", time_to_live=3600)
 
 	# Send a data message only
 	fcm_device.send_message(None, extra={"other": "content", "misc": "data"})
 
-You can disable this default behaviour by setting ``use_fcm_notifications`` to ``False``.
-
-.. code-block:: python
 
-	fcm_device = GCMDevice.objects.create(registration_id="token", cloud_message_type="FCM", user=the_user)
 
-	# Send a data message with classic format
-	fcm_device.send_message("This is a message", use_fcm_notifications=False)
+Behind the scenes, a `Firebase Message <https://firebase.google.com/docs/reference/admin/dotnet/class/firebase-admin/messaging/message>`_ will be created.
+You can also create this yourself and pass it to the ``send_message`` method instead.
 
 
 Sending FCM/GCM messages to topic members
 -----------------------------------------
 FCM/GCM topic messaging allows your app server to send a message to multiple devices that have opted in to a particular topic. Based on the publish/subscribe model, topic messaging supports unlimited subscriptions per app. Developers can choose any topic name that matches the regular expression, "/topics/[a-zA-Z0-9-_.~%]+".
 Note: gcm_send_bulk_message must be used when sending messages to topic subscribers, and setting the first param to any value other than None will result in a 400 Http error.
 
 .. code-block:: python
 
-	from push_notifications.gcm import send_message
+	from push_notifications.gcm import send_message, dict_to_fcm_message
 
-        # First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
-        send_message(None, {"body": "Hello members of my_topic!"}, cloud_type="FCM", to="/topics/my_topic")
+	# Create message object from dictonary. You can also directly create a messaging.Message object.
+	message = dict_to_fcm_message({"body": "Hello members of my_topic!"})
+	# First param is "None" because no Registration_id is needed, the message will be sent to all devices subscribed to the topic.
+	send_message(None, message, to="/topics/my_topic")
 
 Reference: `FCM Documentation <https://firebase.google.com/docs/cloud-messaging/android/topic-messaging>`_
 
 Exceptions
 ----------
 
 - ``NotificationError(Exception)``: Base exception for all notification-related errors.
-- ``gcm.GCMError(NotificationError)``: An error was returned by GCM. This is never raised when using bulk notifications.
 - ``apns.APNSError(NotificationError)``: Something went wrong upon sending APNS notifications.
 - ``apns.APNSDataOverflow(APNSError)``: The APNS payload exceeds its maximum size and cannot be sent.
 
 Django REST Framework (DRF) support
 -----------------------------------
 
 ViewSets are available for both APNS and GCM devices in two permission flavors:
```

### Comparing `django-push-notifications-3.0.2/django_push_notifications.egg-info/SOURCES.txt` & `django-push-notifications-3.0.3/django_push_notifications.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .github/workflows/test.yml
 django_push_notifications.egg-info/PKG-INFO
 django_push_notifications.egg-info/SOURCES.txt
 django_push_notifications.egg-info/dependency_links.txt
 django_push_notifications.egg-info/requires.txt
 django_push_notifications.egg-info/top_level.txt
 docs/APNS.rst
+docs/FCM.rst
 docs/WebPush.rst
 push_notifications/__init__.py
 push_notifications/admin.py
 push_notifications/apns.py
 push_notifications/compat.py
 push_notifications/exceptions.py
 push_notifications/fields.py
@@ -44,22 +45,25 @@
 push_notifications/migrations/0003_wnsdevice.py
 push_notifications/migrations/0004_fcm.py
 push_notifications/migrations/0005_applicationid.py
 push_notifications/migrations/0006_webpushdevice.py
 push_notifications/migrations/0007_uniquesetting.py
 push_notifications/migrations/0008_webpush_add_edge.py
 push_notifications/migrations/0009_alter_apnsdevice_device_id.py
+push_notifications/migrations/0010_alter_gcmdevice_options_and_more.py
 push_notifications/migrations/__init__.py
 tests/__init__.py
 tests/responses.py
 tests/settings.py
 tests/settings_unique.py
+tests/test_admin.py
 tests/test_apns_models.py
 tests/test_apns_push_payload.py
 tests/test_app_config.py
+tests/test_dict_to_message.py
 tests/test_fields.py
 tests/test_gcm_push_payload.py
 tests/test_legacy_config.py
 tests/test_models.py
 tests/test_rest_framework.py
 tests/test_webpush.py
 tests/test_wns.py
```

### Comparing `django-push-notifications-3.0.2/docs/APNS.rst` & `django-push-notifications-3.0.3/docs/APNS.rst`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/docs/WebPush.rst` & `django-push-notifications-3.0.3/docs/WebPush.rst`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/admin.py` & `django-push-notifications-3.0.3/push_notifications/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -128,14 +128,45 @@
 
 class GCMDeviceAdmin(DeviceAdmin):
 	list_display = (
 		"__str__", "device_id", "user", "active", "date_created", "cloud_message_type"
 	)
 	list_filter = ("active", "cloud_message_type")
 
+	def send_messages(self, request, queryset, bulk=False):
+		"""
+		Provides error handling for DeviceAdmin send_message and send_bulk_message methods.
+		"""
+		results = []
+		errors = []
+
+		if bulk:
+			results.append(queryset.send_message("Test bulk notification"))
+		else:
+			for device in queryset:
+				result = device.send_message("Test single notification")
+				if result:
+					results.append(result)
+
+		for batch in results:
+			for response in batch.responses:
+				if response.exception:
+					errors.append(repr(response.exception))
+
+		if errors:
+			self.message_user(
+				request, _("Some messages could not be processed: %s") % (", ".join(errors)),
+				level=messages.ERROR
+			)
+		else:
+			self.message_user(
+				request, _("All messages were sent."),
+				level=messages.SUCCESS
+			)
+
 
 class WebPushDeviceAdmin(DeviceAdmin):
 	list_display = ("__str__", "browser", "user", "active", "date_created")
 	list_filter = ("active", "browser")
 
 	if hasattr(User, "USERNAME_FIELD"):
 		search_fields = ("name", "registration_id", "user__%s" % (User.USERNAME_FIELD))
```

### Comparing `django-push-notifications-3.0.2/push_notifications/api/rest_framework.py` & `django-push-notifications-3.0.3/push_notifications/api/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/apns.py` & `django-push-notifications-3.0.3/push_notifications/apns.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/conf/__init__.py` & `django-push-notifications-3.0.3/push_notifications/conf/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.utils.module_loading import import_string
 
+from ..settings import PUSH_NOTIFICATIONS_SETTINGS as SETTINGS  # noqa: I001
 from .app import AppConfig  # noqa: F401
 from .appmodel import AppModelConfig  # noqa: F401
 from .legacy import LegacyConfig  # noqa: F401
-from ..settings import PUSH_NOTIFICATIONS_SETTINGS as SETTINGS  # noqa: I001
 
 
 manager = None
 
 
 def get_manager(reload=False):
 	global manager
```

### Comparing `django-push-notifications-3.0.2/push_notifications/conf/app.py` & `django-push-notifications-3.0.3/push_notifications/conf/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 MISSING_SETTING = (
 	'PUSH_NOTIFICATIONS_SETTINGS.APPLICATIONS["{application_id}"]["{setting}"] is missing.'
 )
 
 PLATFORMS = [
 	"APNS",
 	"FCM",
-	"GCM",
 	"WNS",
 	"WP",
 ]
 
 # Settings that all applications must have
 REQUIRED_SETTINGS = [
 	"PLATFORM",
@@ -51,17 +50,17 @@
 APNS_AUTH_CREDS_REQUIRED = ["AUTH_KEY_PATH", "AUTH_KEY_ID", "TEAM_ID"]
 APNS_AUTH_CREDS_OPTIONAL = ["CERTIFICATE", "ENCRYPTION_ALGORITHM", "TOKEN_LIFETIME"]
 
 APNS_OPTIONAL_SETTINGS = [
 	"USE_SANDBOX", "USE_ALTERNATIVE_PORT", "TOPIC"
 ]
 
-FCM_REQUIRED_SETTINGS = GCM_REQUIRED_SETTINGS = ["API_KEY"]
-FCM_OPTIONAL_SETTINGS = GCM_OPTIONAL_SETTINGS = [
-	"POST_URL", "MAX_RECIPIENTS", "ERROR_TIMEOUT"
+FCM_REQUIRED_SETTINGS = []
+FCM_OPTIONAL_SETTINGS = [
+	"MAX_RECIPIENTS", "FIREBASE_APP"
 ]
 
 WNS_REQUIRED_SETTINGS = ["PACKAGE_SECURITY_ID", "SECRET_KEY"]
 WNS_OPTIONAL_SETTINGS = ["WNS_ACCESS_URL"]
 
 WP_REQUIRED_SETTINGS = ["PRIVATE_KEY", "CLAIMS"]
 WP_OPTIONAL_SETTINGS = ["ERROR_TIMEOUT", "POST_URL"]
@@ -185,31 +184,16 @@
 		)
 
 		self._validate_allowed_settings(application_id, application_config, allowed)
 		self._validate_required_settings(
 			application_id, application_config, FCM_REQUIRED_SETTINGS
 		)
 
-		application_config.setdefault("POST_URL", "https://fcm.googleapis.com/fcm/send")
+		application_config.setdefault("FIREBASE_APP", None)
 		application_config.setdefault("MAX_RECIPIENTS", 1000)
-		application_config.setdefault("ERROR_TIMEOUT", None)
-
-	def _validate_gcm_config(self, application_id, application_config):
-		allowed = (
-			REQUIRED_SETTINGS + OPTIONAL_SETTINGS + GCM_REQUIRED_SETTINGS + GCM_OPTIONAL_SETTINGS
-		)
-
-		self._validate_allowed_settings(application_id, application_config, allowed)
-		self._validate_required_settings(
-			application_id, application_config, GCM_REQUIRED_SETTINGS
-		)
-
-		application_config.setdefault("POST_URL", "https://android.googleapis.com/gcm/send")
-		application_config.setdefault("MAX_RECIPIENTS", 1000)
-		application_config.setdefault("ERROR_TIMEOUT", None)
 
 	def _validate_wns_config(self, application_id, application_config):
 		allowed = (
 			REQUIRED_SETTINGS + OPTIONAL_SETTINGS + WNS_REQUIRED_SETTINGS + WNS_OPTIONAL_SETTINGS
 		)
 
 		self._validate_allowed_settings(application_id, application_config, allowed)
@@ -299,31 +283,22 @@
 				MISSING_SETTING.format(
 					application_id=application_id, setting=settings_key
 				)
 			)
 
 		return app_config.get(settings_key)
 
+	def get_firebase_app(self, application_id=None):
+		return self._get_application_settings(application_id, "FCM", "FIREBASE_APP")
+
 	def has_auth_token_creds(self, application_id=None):
 		return self.has_token_creds
 
-	def get_gcm_api_key(self, application_id=None):
-		return self._get_application_settings(application_id, "GCM", "API_KEY")
-
-	def get_fcm_api_key(self, application_id=None):
-		return self._get_application_settings(application_id, "FCM", "API_KEY")
-
-	def get_post_url(self, cloud_type, application_id=None):
-		return self._get_application_settings(application_id, cloud_type, "POST_URL")
-
-	def get_error_timeout(self, cloud_type, application_id=None):
-		return self._get_application_settings(application_id, cloud_type, "ERROR_TIMEOUT")
-
-	def get_max_recipients(self, cloud_type, application_id=None):
-		return self._get_application_settings(application_id, cloud_type, "MAX_RECIPIENTS")
+	def get_max_recipients(self, application_id=None):
+		return self._get_application_settings(application_id, "FCM", "MAX_RECIPIENTS")
 
 	def get_apns_certificate(self, application_id=None):
 		r = self._get_application_settings(application_id, "APNS", "CERTIFICATE")
 		if not isinstance(r, str):
 			# probably the (Django) file, and file path should be got
 			if hasattr(r, "path"):
 				return r.path
```

### Comparing `django-push-notifications-3.0.2/push_notifications/conf/base.py` & `django-push-notifications-3.0.3/push_notifications/conf/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from django.core.exceptions import ImproperlyConfigured
 
 
 class BaseConfig:
+
+	def get_firebase_app(self, application_id=None):
+		raise NotImplementedError
+
 	def has_auth_token_creds(self, application_id=None):
 		raise NotImplementedError
 
 	def get_apns_certificate(self, application_id=None):
 		raise NotImplementedError
 
 	def get_apns_auth_creds(self, application_id=None):
@@ -13,33 +17,21 @@
 
 	def get_apns_use_sandbox(self, application_id=None):
 		raise NotImplementedError
 
 	def get_apns_use_alternative_port(self, application_id=None):
 		raise NotImplementedError
 
-	def get_fcm_api_key(self, application_id=None):
-		raise NotImplementedError
-
-	def get_gcm_api_key(self, application_id=None):
-		raise NotImplementedError
-
 	def get_wns_package_security_id(self, application_id=None):
 		raise NotImplementedError
 
 	def get_wns_secret_key(self, application_id=None):
 		raise NotImplementedError
 
-	def get_post_url(self, cloud_type, application_id=None):
-		raise NotImplementedError
-
-	def get_error_timeout(self, cloud_type, application_id=None):
-		raise NotImplementedError
-
-	def get_max_recipients(self, cloud_type, application_id=None):
+	def get_max_recipients(self, application_id=None):
 		raise NotImplementedError
 
 	def get_applications(self):
 		"""Returns a collection containing the configured applications."""
 
 		raise NotImplementedError
```

### Comparing `django-push-notifications-3.0.2/push_notifications/conf/legacy.py` & `django-push-notifications-3.0.3/push_notifications/conf/legacy.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class empty:
 	pass
 
 
 class LegacyConfig(BaseConfig):
-
 	msg = "Setup PUSH_NOTIFICATIONS_SETTINGS properly to send messages"
 
 	def _get_application_settings(self, application_id, settings_key, error_message):
 		"""Legacy behaviour"""
 
 		if not application_id:
 			value = SETTINGS.get(settings_key, empty)
@@ -28,50 +27,25 @@
 		else:
 			msg = (
 				"LegacySettings does not support application_id. To enable "
 				"multiple application support, use push_notifications.conf.AppSettings."
 			)
 			raise ImproperlyConfigured(msg)
 
-	def get_gcm_api_key(self, application_id=None):
-		msg = (
-			'Set PUSH_NOTIFICATIONS_SETTINGS["GCM_API_KEY"] to send messages through GCM.'
-		)
-		return self._get_application_settings(application_id, "GCM_API_KEY", msg)
-
-	def get_fcm_api_key(self, application_id=None):
-		msg = (
-			'Set PUSH_NOTIFICATIONS_SETTINGS["FCM_API_KEY"] to send messages through FCM.'
-		)
-		return self._get_application_settings(application_id, "FCM_API_KEY", msg)
-
-	def get_post_url(self, cloud_type, application_id=None):
-		key = "{}_POST_URL".format(cloud_type)
+	def get_firebase_app(self, application_id=None):
+		key = "FIREBASE_APP"
 		msg = (
-			'Set PUSH_NOTIFICATIONS_SETTINGS["{}"] to send messages through {}.'.format(
-				key, cloud_type
-			)
+			'Set PUSH_NOTIFICATIONS_SETTINGS["{}"] to send messages through FCM.'.format(key)
 		)
 		return self._get_application_settings(application_id, key, msg)
 
-	def get_error_timeout(self, cloud_type, application_id=None):
-		key = "{}_ERROR_TIMEOUT".format(cloud_type)
+	def get_max_recipients(self, application_id=None):
+		key = "FCM_MAX_RECIPIENTS"
 		msg = (
-			'Set PUSH_NOTIFICATIONS_SETTINGS["{}"] to send messages through {}.'.format(
-				key, cloud_type
-			)
-		)
-		return self._get_application_settings(application_id, key, msg)
-
-	def get_max_recipients(self, cloud_type, application_id=None):
-		key = "{}_MAX_RECIPIENTS".format(cloud_type)
-		msg = (
-			'Set PUSH_NOTIFICATIONS_SETTINGS["{}"] to send messages through {}.'.format(
-				key, cloud_type
-			)
+			'Set PUSH_NOTIFICATIONS_SETTINGS["{}"] to send messages through FCM.'.format(key)
 		)
 		return self._get_application_settings(application_id, key, msg)
 
 	def has_auth_token_creds(self, application_id=None):
 		try:
 			self._get_apns_auth_key(application_id)
 			self._get_apns_auth_key_id(application_id)
```

### Comparing `django-push-notifications-3.0.2/push_notifications/fields.py` & `django-push-notifications-3.0.3/push_notifications/fields.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0001_initial.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0003_wnsdevice.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0003_wnsdevice.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0004_fcm.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0004_fcm.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0005_applicationid.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0005_applicationid.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0006_webpushdevice.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0006_webpushdevice.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0007_uniquesetting.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0007_uniquesetting.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/migrations/0008_webpush_add_edge.py` & `django-push-notifications-3.0.3/push_notifications/migrations/0008_webpush_add_edge.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/models.py` & `django-push-notifications-3.0.3/push_notifications/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,82 +54,94 @@
 	def get_queryset(self):
 		return GCMDeviceQuerySet(self.model)
 
 
 class GCMDeviceQuerySet(models.query.QuerySet):
 	def send_message(self, message, **kwargs):
 		if self.exists():
-			from .gcm import send_message as gcm_send_message
+			from .gcm import dict_to_fcm_message, messaging
+			from .gcm import send_message as fcm_send_message
 
-			data = kwargs.pop("extra", {})
-			if message is not None:
-				data["message"] = message
+			if not isinstance(message, messaging.Message):
+				data = kwargs.pop("extra", {})
+				if message is not None:
+					data["message"] = message
+				# transform legacy data to new message object
+				message = dict_to_fcm_message(data, **kwargs)
 
 			app_ids = self.filter(active=True).order_by(
 				"application_id"
 			).values_list("application_id", flat=True).distinct()
-			response = []
-			for cloud_type in ("FCM", "GCM"):
-				for app_id in app_ids:
-					reg_ids = list(
-						self.filter(
-							active=True, cloud_message_type=cloud_type, application_id=app_id).values_list(
-							"registration_id", flat=True
-						)
+
+			responses = []
+			for app_id in app_ids:
+				reg_ids = list(
+					self.filter(
+						active=True, cloud_message_type="FCM", application_id=app_id).values_list(
+						"registration_id", flat=True
 					)
-					if reg_ids:
-						r = gcm_send_message(reg_ids, data, cloud_type, application_id=app_id, **kwargs)
-						response.append(r)
+				)
+				if reg_ids:
+					r = fcm_send_message(reg_ids, message, application_id=app_id, **kwargs)
+					responses.extend(r.responses)
 
-			return response
+			return messaging.BatchResponse(responses)
 
 
 class GCMDevice(Device):
 	# device_id cannot be a reliable primary key as fragmentation between different devices
 	# can make it turn out to be null and such:
 	# http://android-developers.blogspot.co.uk/2011/03/identifying-app-installations.html
 	device_id = HexIntegerField(
 		verbose_name=_("Device ID"), blank=True, null=True, db_index=True,
 		help_text=_("ANDROID_ID / TelephonyManager.getDeviceId() (always as hex)")
 	)
 	registration_id = models.TextField(verbose_name=_("Registration ID"), unique=SETTINGS["UNIQUE_REG_ID"])
 	cloud_message_type = models.CharField(
 		verbose_name=_("Cloud Message Type"), max_length=3,
-		choices=CLOUD_MESSAGE_TYPES, default="GCM",
-		help_text=_("You should choose FCM or GCM")
+		choices=CLOUD_MESSAGE_TYPES, default="FCM",
+		help_text=_("You should choose FCM, GCM is deprecated")
 	)
 	objects = GCMDeviceManager()
 
 	class Meta:
-		verbose_name = _("GCM device")
+		verbose_name = _("FCM device")
 
 	def send_message(self, message, **kwargs):
-		from .gcm import send_message as gcm_send_message
+		from .gcm import dict_to_fcm_message, messaging
+		from .gcm import send_message as fcm_send_message
+
+		# GCM is not supported.
+		if self.cloud_message_type == "GCM":
+			return
 
-		data = kwargs.pop("extra", {})
-		if message is not None:
-			data["message"] = message
+		if not isinstance(message, messaging.Message):
+			data = kwargs.pop("extra", {})
+			if message is not None:
+				data["message"] = message
+			# transform legacy data to new message object
+			message = dict_to_fcm_message(data, **kwargs)
 
-		return gcm_send_message(
-			self.registration_id, data, self.cloud_message_type,
+		return fcm_send_message(
+			self.registration_id, message,
 			application_id=self.application_id, **kwargs
 		)
 
 
 class APNSDeviceManager(models.Manager):
 	def get_queryset(self):
 		return APNSDeviceQuerySet(self.model)
 
 
 class APNSDeviceQuerySet(models.query.QuerySet):
 	def send_message(self, message, creds=None, **kwargs):
 		if self.exists():
 			from .apns import apns_send_bulk_message
 
-			app_ids = self.filter(active=True).order_by("application_id")\
+			app_ids = self.filter(active=True).order_by("application_id") \
 				.values_list("application_id", flat=True).distinct()
 			res = []
 			for app_id in app_ids:
 				reg_ids = list(self.filter(active=True, application_id=app_id).values_list(
 					"registration_id", flat=True)
 				)
 				r = apns_send_bulk_message(
```

### Comparing `django-push-notifications-3.0.2/push_notifications/settings.py` & `django-push-notifications-3.0.3/push_notifications/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,17 @@
 
 PUSH_NOTIFICATIONS_SETTINGS = getattr(settings, "PUSH_NOTIFICATIONS_SETTINGS", {})
 
 PUSH_NOTIFICATIONS_SETTINGS.setdefault(
 	"CONFIG", "push_notifications.conf.LegacyConfig"
 )
 
-# GCM
-PUSH_NOTIFICATIONS_SETTINGS.setdefault(
-	"GCM_POST_URL", "https://android.googleapis.com/gcm/send"
-)
-PUSH_NOTIFICATIONS_SETTINGS.setdefault("GCM_MAX_RECIPIENTS", 1000)
-PUSH_NOTIFICATIONS_SETTINGS.setdefault("GCM_ERROR_TIMEOUT", None)
-
 # FCM
-PUSH_NOTIFICATIONS_SETTINGS.setdefault(
-	"FCM_POST_URL", "https://fcm.googleapis.com/fcm/send"
-)
+PUSH_NOTIFICATIONS_SETTINGS.setdefault("FIREBASE_APP", None)
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("FCM_MAX_RECIPIENTS", 1000)
-PUSH_NOTIFICATIONS_SETTINGS.setdefault("FCM_ERROR_TIMEOUT", None)
 
 # APNS
 if settings.DEBUG:
 	PUSH_NOTIFICATIONS_SETTINGS.setdefault("APNS_USE_SANDBOX", True)
 else:
 	PUSH_NOTIFICATIONS_SETTINGS.setdefault("APNS_USE_SANDBOX", False)
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("APNS_USE_ALTERNATIVE_PORT", False)
@@ -33,14 +23,19 @@
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("WNS_PACKAGE_SECURITY_ID", None)
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("WNS_SECRET_KEY", None)
 PUSH_NOTIFICATIONS_SETTINGS.setdefault(
 	"WNS_ACCESS_URL", "https://login.live.com/accesstoken.srf"
 )
 
 # WP (WebPush)
+
+PUSH_NOTIFICATIONS_SETTINGS.setdefault(
+	"FCM_POST_URL", "https://fcm.googleapis.com/fcm/send"
+)
+
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("WP_POST_URL", {
 	"CHROME": PUSH_NOTIFICATIONS_SETTINGS["FCM_POST_URL"],
 	"OPERA": PUSH_NOTIFICATIONS_SETTINGS["FCM_POST_URL"],
 	"FIREFOX": "https://updates.push.services.mozilla.com/wpush/v2",
 	"EDGE": "https://wns2-par02p.notify.windows.com/w",
 })
 PUSH_NOTIFICATIONS_SETTINGS.setdefault("WP_PRIVATE_KEY", None)
```

### Comparing `django-push-notifications-3.0.2/push_notifications/webpush.py` & `django-push-notifications-3.0.3/push_notifications/webpush.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/push_notifications/wns.py` & `django-push-notifications-3.0.3/push_notifications/wns.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/setup.cfg` & `django-push-notifications-3.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Topic :: Internet :: WWW/HTTP
 	Topic :: System :: Networking
 
 [options]
-python_requires = >= 3.6
+python_requires = >= 3.7
 packages = find:
 install_requires = 
 	Django>=2.2
 setup_requires = 
 	setuptools_scm
 
 [options.extras_require]
 APNS = 
 	apns2>=0.3.0
 	importlib-metadata;python_version < "3.8"
 	Django>=2.2
 WP = pywebpush>=1.3.0
+FCM = firebase-admin>=5,<6
 
 [options.packages.find]
 exclude = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-push-notifications-3.0.2/tests/settings_unique.py` & `django-push-notifications-3.0.3/tests/settings_unique.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_apns_models.py` & `django-push-notifications-3.0.3/tests/test_apns_models.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_apns_push_payload.py` & `django-push-notifications-3.0.3/tests/test_apns_push_payload.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_app_config.py` & `django-push-notifications-3.0.3/tests/test_app_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -66,41 +66,23 @@
 		"""
 
 		application_id = "my_fcm_app"
 		PUSH_SETTINGS = {
 			"APPLICATIONS": {
 				application_id: {
 					"PLATFORM": "FCM",
-					"API_KEY": "[my_api_key]"
 				}
 			}
 		}
 
 		manager = AppConfig(PUSH_SETTINGS)
 
 		with self.assertRaises(ImproperlyConfigured):
 			manager._get_application_settings(application_id, "APNS", "CERTIFICATE")
 
-	def test_missing_setting(self):
-		"""
-		Missing application settings raises ImproperlyConfigured.
-		"""
-
-		application_id = "my_fcm_app"
-		PUSH_SETTINGS = {
-			"APPLICATIONS": {
-				application_id: {
-					"PLATFORM": "FCM"
-				}
-			}
-		}
-
-		with self.assertRaises(ImproperlyConfigured):
-			AppConfig(PUSH_SETTINGS)
-
 	def test_validate_apns_config(self):
 		"""
 		Verify the settings for APNS platform.
 		"""
 
 		path = os.path.join(os.path.dirname(__file__), "test_data", "good_revoked.pem")
 
@@ -179,101 +161,48 @@
 		#
 		# all settings specified, required and optional, does not raise an error.
 		#
 		PUSH_SETTINGS = {
 			"APPLICATIONS": {
 				"my_fcm_app": {
 					"PLATFORM": "FCM",
-					"API_KEY": "...",
-					"POST_URL": "...",
 					"MAX_RECIPIENTS": "...",
-					"ERROR_TIMEOUT": "...",
+					"FIREBASE_APP": "...",
 				}
 			}
 		}
 		AppConfig(PUSH_SETTINGS)
 
-		# missing required settings
+		# old API_KEY does not work anymore
 		PUSH_SETTINGS = {
 			"APPLICATIONS": {
 				"my_fcm_app": {
 					"PLATFORM": "FCM",
+					"API_KEY": "...",
 				}
 			}
 		}
 
 		with self.assertRaises(ImproperlyConfigured):
 			AppConfig(PUSH_SETTINGS)
 
 		# all optional settings have default values
 		PUSH_SETTINGS = {
 			"APPLICATIONS": {
 				"my_fcm_app": {
 					"PLATFORM": "FCM",
-					"API_KEY": "...",
 				}
 			}
 		}
 
 		manager = AppConfig(PUSH_SETTINGS)
 		app_config = manager._settings["APPLICATIONS"]["my_fcm_app"]
 
-		assert app_config["POST_URL"] == "https://fcm.googleapis.com/fcm/send"
-		assert app_config["MAX_RECIPIENTS"] == 1000
-		assert app_config["ERROR_TIMEOUT"] is None
-
-	def test_get_allowed_settings_gcm(self):
-		"""Verify the settings allowed for GCM platform."""
-
-		#
-		# all settings specified, required and optional, does not raise an error.
-		#
-		PUSH_SETTINGS = {
-			"APPLICATIONS": {
-				"my_gcm_app": {
-					"PLATFORM": "GCM",
-					"API_KEY": "...",
-					"POST_URL": "...",
-					"MAX_RECIPIENTS": "...",
-					"ERROR_TIMEOUT": "...",
-				}
-			}
-		}
-		AppConfig(PUSH_SETTINGS)
-
-		#
-		# missing required settings
-		#
-		PUSH_SETTINGS = {
-			"APPLICATIONS": {
-				"my_gcm_app": {
-					"PLATFORM": "GCM",
-				}
-			}
-		}
-
-		with self.assertRaises(ImproperlyConfigured):
-			AppConfig(PUSH_SETTINGS)
-
-		# all optional settings have default values
-		PUSH_SETTINGS = {
-			"APPLICATIONS": {
-				"my_gcm_app": {
-					"PLATFORM": "GCM",
-					"API_KEY": "...",
-				}
-			}
-		}
-
-		manager = AppConfig(PUSH_SETTINGS)
-		app_config = manager._settings["APPLICATIONS"]["my_gcm_app"]
-
-		assert app_config["POST_URL"] == "https://android.googleapis.com/gcm/send"
 		assert app_config["MAX_RECIPIENTS"] == 1000
-		assert app_config["ERROR_TIMEOUT"] is None
+		assert app_config["FIREBASE_APP"] is None
 
 	def test_get_allowed_settings_wns(self):
 		"""
 		Verify the settings allowed for WNS platform.
 		"""
 
 		# all settings specified, required and optional, does not raise an error.
```

### Comparing `django-push-notifications-3.0.2/tests/test_data/good_revoked.pem` & `django-push-notifications-3.0.3/tests/test_data/good_revoked.pem`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_data/good_with_passwd.pem` & `django-push-notifications-3.0.3/tests/test_data/good_with_passwd.pem`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_data/without_private.pem` & `django-push-notifications-3.0.3/tests/test_data/without_private.pem`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_fields.py` & `django-push-notifications-3.0.3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_rest_framework.py` & `django-push-notifications-3.0.3/tests/test_rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_webpush.py` & `django-push-notifications-3.0.3/tests/test_webpush.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/test_wns.py` & `django-push-notifications-3.0.3/tests/test_wns.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tests/tst_unique.py` & `django-push-notifications-3.0.3/tests/tst_unique.py`

 * *Files identical despite different names*

### Comparing `django-push-notifications-3.0.2/tox.ini` & `django-push-notifications-3.0.3/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tox]
 skipsdist = False
 usedevelop = true
 envlist =
-    py{36,37,38,39}-dj{22,32}
+    py{37,38,39}-dj{22,32}
     py{38,39}-dj{40,405}
     flake8
 
 [gh-actions]
 python =
-    3.6: py36
     3.7: py37
     3.8: py38
     3.9: py39, flake8
 
 [gh-actions:env]
 DJANGO =
     2.2: dj22
@@ -32,14 +31,15 @@
 deps =
     apns2
     pytest
     pytest-cov
     pytest-django
     pywebpush
     djangorestframework
+    firebase-admin>=5,<6
     dj22: Django>=2.2,<3.0
     dj32: Django>=3.2,<3.3
     dj40: Django>=4.0,<4.0.5
 	dj405: Django>=4.0.5,<4.1
 
 [testenv:flake8]
 commands = flake8 --exit-zero
```

