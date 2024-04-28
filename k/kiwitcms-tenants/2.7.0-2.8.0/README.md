# Comparing `tmp/kiwitcms-tenants-2.7.0.tar.gz` & `tmp/kiwitcms-tenants-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-tenants-2.7.0.tar", last modified: Tue Apr 23 21:48:49 2024, max compression
+gzip compressed data, was "kiwitcms-tenants-2.8.0.tar", last modified: Sun Apr 28 16:39:48 2024, max compression
```

## Comparing `kiwitcms-tenants-2.7.0.tar` & `kiwitcms-tenants-2.8.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    17995 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    17177 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.412761 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    17995 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     2087 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       51 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       38 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       45 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)      103 2024-04-17 18:56:27.000000 kiwitcms-tenants-2.7.0/requirements.txt
--rw-r--r--   0 senko     (1001) senko     (1001)      102 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1738 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.412761 kiwitcms-tenants-2.7.0/tcms_settings_dir/
--rw-r--r--   0 senko     (1001) senko     (1001)       65 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_settings_dir/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     2508 2024-04-22 20:07:06.000000 kiwitcms-tenants-2.7.0/tcms_settings_dir/multi_tenant.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.7.0/tcms_tenants/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     7647 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.7.0/tcms_tenants/apps.py
--rw-r--r--   0 senko     (1001) senko     (1001)      713 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/backends.py
--rw-r--r--   0 senko     (1001) senko     (1001)      664 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/checks.py
--rw-r--r--   0 senko     (1001) senko     (1001)      821 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/context_processors.py
--rw-r--r--   0 senko     (1001) senko     (1001)     3171 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/forms.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/
--rw-r--r--   0 senko     (1001) senko     (1001)     4016 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/management/
--rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/
--rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     2175 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/initialize_tenants.py
--rw-r--r--   0 senko     (1001) senko     (1001)      766 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/menu.py
--rw-r--r--   0 senko     (1001) senko     (1001)     2265 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/middleware.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     2782 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      608 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0002_tenant_owner.py
--rw-r--r--   0 senko     (1001) senko     (1001)      596 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0003_use_datetime_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0004_tenant_organization.py
--rw-r--r--   0 senko     (1001) senko     (1001)      553 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
--rw-r--r--   0 senko     (1001) senko     (1001)      476 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0006_tenant_extra_emails.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1409 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/models.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1168 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/oss_utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1411 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/storage.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/new.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      904 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/invite_users.html
--rw-r--r--   0 senko     (1001) senko     (1001)     3614 2024-04-23 19:00:56.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/new.html
--rw-r--r--   0 senko     (1001) senko     (1001)      297 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/tenant_name.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/tcms_tenants.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/tests/
--rw-r--r--   0 senko     (1001) senko     (1001)     3999 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/
--rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 senko     (1001) senko     (1001)      618 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     8255 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5331 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.7.0/tenant_groups/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/apps.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1405 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/backends.py
--rw-r--r--   0 senko     (1001) senko     (1001)      754 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/checks.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/management/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/refresh_tenant_permissions.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     4427 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1380 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.8.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.8.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    18479 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    17661 2024-04-28 16:39:28.000000 kiwitcms-tenants-2.8.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    18479 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     2087 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       51 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       38 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       45 2024-04-28 16:39:48.000000 kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      103 2024-04-17 18:56:27.000000 kiwitcms-tenants-2.8.0/requirements.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      102 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1738 2024-04-28 16:39:28.000000 kiwitcms-tenants-2.8.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/tcms_settings_dir/
+-rw-r--r--   0 senko     (1001) senko     (1001)       65 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_settings_dir/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2508 2024-04-22 20:07:06.000000 kiwitcms-tenants-2.8.0/tcms_settings_dir/multi_tenant.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/tcms_tenants/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.8.0/tcms_tenants/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     7647 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.8.0/tcms_tenants/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.8.0/tcms_tenants/apps.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      713 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.8.0/tcms_tenants/backends.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      664 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/checks.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      821 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.8.0/tcms_tenants/context_processors.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     3320 2024-04-27 21:47:40.000000 kiwitcms-tenants-2.8.0/tcms_tenants/forms.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.157596 kiwitcms-tenants-2.8.0/tcms_tenants/locale/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.157596 kiwitcms-tenants-2.8.0/tcms_tenants/locale/en/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/tcms_tenants/locale/en/LC_MESSAGES/
+-rw-r--r--   0 senko     (1001) senko     (1001)     4016 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.8.0/tcms_tenants/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/tcms_tenants/management/
+-rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.8.0/tcms_tenants/management/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.158596 kiwitcms-tenants-2.8.0/tcms_tenants/management/commands/
+-rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.8.0/tcms_tenants/management/commands/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2175 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.8.0/tcms_tenants/management/commands/initialize_tenants.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      766 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/menu.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2265 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/middleware.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     2782 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      608 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0002_tenant_owner.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      596 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0003_use_datetime_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0004_tenant_organization.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      553 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      476 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0006_tenant_extra_emails.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.8.0/tcms_tenants/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1409 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.8.0/tcms_tenants/models.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1168 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/oss_utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1411 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/storage.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.157596 kiwitcms-tenants-2.8.0/tcms_tenants/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/email/new.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)     1020 2024-04-27 21:47:40.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/invite_users.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     3614 2024-04-23 19:00:56.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/new.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      297 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/tenant_name.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.8.0/tcms_tenants/templatetags/tcms_tenants.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/tests/
+-rw-r--r--   0 senko     (1001) senko     (1001)     3999 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/tests/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tcms_tenants/tests/__pycache__/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.8.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 senko     (1001) senko     (1001)      618 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     8255 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tcms_tenants/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5331 2024-04-27 20:19:30.000000 kiwitcms-tenants-2.8.0/tcms_tenants/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tenant_groups/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.8.0/tenant_groups/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.8.0/tenant_groups/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.8.0/tenant_groups/apps.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1405 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tenant_groups/backends.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      754 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tenant_groups/checks.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tenant_groups/management/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.8.0/tenant_groups/management/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tenant_groups/management/commands/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.8.0/tenant_groups/management/commands/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tenant_groups/management/commands/refresh_tenant_permissions.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-28 16:39:48.159596 kiwitcms-tenants-2.8.0/tenant_groups/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     4427 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tenant_groups/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.8.0/tenant_groups/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1380 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.8.0/tenant_groups/models.py
```

### Comparing `kiwitcms-tenants-2.7.0/LICENSE` & `kiwitcms-tenants-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/PKG-INFO` & `kiwitcms-tenants-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-tenants
-Version: 2.7.0
+Version: 2.8.0
 Summary: Multi-tenant support for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/tenants/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,16 +79,18 @@
 
 When starting your multi-tenant Kiwi TCMS instance for the first time you also
 need to create information about the so called public tenant. That is the
 default tenant on which your application runs::
 
     ./manage.py initial_setup
 
-Your tenant will be available at https://public.$KIWI_TENANTS_DOMAIN!
-Other tenants can also be created via the web interface as well.
+Your tenant will be available at https://$KIWI_TENANTS_DOMAIN!
+Other tenants can be created via the web interface and will be available
+under team-01.$KIWI_TENANTS_DOMAIN, product-02.$KIWI_TENANTS_DOMAIN, etc
+depnding on the actual ``schema name`` you give them.
 
 
 DNS configuration
 -----------------
 
 You need wildcard DNS resolution to be configured for ``*.tenants.example.org``!
 
@@ -154,22 +156,33 @@
 Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
 
     PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
 
 Then point your browser to https://tenant.example.bg:8000/.
 The SSL warning from the browser is expected!
 
-You can use ``/etc/hosts`` to configure DNS resolution during development::
+You can use your `OS hosts file <https://en.wikipedia.org/wiki/Hosts_(file)>`_
+to configure DNS resolution during development::
 
     127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
 
 
 Changelog
 ---------
 
+v2.8.0 (28 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Refactor HTML template for Invite Users page to display form field errors
+- When inviting users validate addresses taking into account the value of
+  ``settings.EMAIL_VALIDATORS``
+- Updated documentation
+- Adjust tests for newer version of django-grappelli
+
+
 v2.7.0 (24 Apr 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Add the ``Tenant.extra_emails`` field for storing information like
   technical email, billing email, etc. To be used by add-on tools
 - Add the ``initialize_tenants`` management command
 - Update local development instructions
```

### Comparing `kiwitcms-tenants-2.7.0/README.rst` & `kiwitcms-tenants-2.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,18 @@
 
 When starting your multi-tenant Kiwi TCMS instance for the first time you also
 need to create information about the so called public tenant. That is the
 default tenant on which your application runs::
 
     ./manage.py initial_setup
 
-Your tenant will be available at https://public.$KIWI_TENANTS_DOMAIN!
-Other tenants can also be created via the web interface as well.
+Your tenant will be available at https://$KIWI_TENANTS_DOMAIN!
+Other tenants can be created via the web interface and will be available
+under team-01.$KIWI_TENANTS_DOMAIN, product-02.$KIWI_TENANTS_DOMAIN, etc
+depnding on the actual ``schema name`` you give them.
 
 
 DNS configuration
 -----------------
 
 You need wildcard DNS resolution to be configured for ``*.tenants.example.org``!
 
@@ -133,22 +135,33 @@
 Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
 
     PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
 
 Then point your browser to https://tenant.example.bg:8000/.
 The SSL warning from the browser is expected!
 
-You can use ``/etc/hosts`` to configure DNS resolution during development::
+You can use your `OS hosts file <https://en.wikipedia.org/wiki/Hosts_(file)>`_
+to configure DNS resolution during development::
 
     127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
 
 
 Changelog
 ---------
 
+v2.8.0 (28 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Refactor HTML template for Invite Users page to display form field errors
+- When inviting users validate addresses taking into account the value of
+  ``settings.EMAIL_VALIDATORS``
+- Updated documentation
+- Adjust tests for newer version of django-grappelli
+
+
 v2.7.0 (24 Apr 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Add the ``Tenant.extra_emails`` field for storing information like
   technical email, billing email, etc. To be used by add-on tools
 - Add the ``initialize_tenants`` management command
 - Update local development instructions
```

### Comparing `kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/PKG-INFO` & `kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-tenants
-Version: 2.7.0
+Version: 2.8.0
 Summary: Multi-tenant support for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/tenants/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,16 +79,18 @@
 
 When starting your multi-tenant Kiwi TCMS instance for the first time you also
 need to create information about the so called public tenant. That is the
 default tenant on which your application runs::
 
     ./manage.py initial_setup
 
-Your tenant will be available at https://public.$KIWI_TENANTS_DOMAIN!
-Other tenants can also be created via the web interface as well.
+Your tenant will be available at https://$KIWI_TENANTS_DOMAIN!
+Other tenants can be created via the web interface and will be available
+under team-01.$KIWI_TENANTS_DOMAIN, product-02.$KIWI_TENANTS_DOMAIN, etc
+depnding on the actual ``schema name`` you give them.
 
 
 DNS configuration
 -----------------
 
 You need wildcard DNS resolution to be configured for ``*.tenants.example.org``!
 
@@ -154,22 +156,33 @@
 Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
 
     PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
 
 Then point your browser to https://tenant.example.bg:8000/.
 The SSL warning from the browser is expected!
 
-You can use ``/etc/hosts`` to configure DNS resolution during development::
+You can use your `OS hosts file <https://en.wikipedia.org/wiki/Hosts_(file)>`_
+to configure DNS resolution during development::
 
     127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
 
 
 Changelog
 ---------
 
+v2.8.0 (28 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Refactor HTML template for Invite Users page to display form field errors
+- When inviting users validate addresses taking into account the value of
+  ``settings.EMAIL_VALIDATORS``
+- Updated documentation
+- Adjust tests for newer version of django-grappelli
+
+
 v2.7.0 (24 Apr 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Add the ``Tenant.extra_emails`` field for storing information like
   technical email, billing email, etc. To be used by add-on tools
 - Add the ``initialize_tenants`` management command
 - Update local development instructions
```

### Comparing `kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/SOURCES.txt` & `kiwitcms-tenants-2.8.0/kiwitcms_tenants.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/setup.py` & `kiwitcms-tenants-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-tenants",
-    version="2.7.0",
+    version="2.8.0",
     description="Multi-tenant support for Kiwi TCMS",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/tenants/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-tenants-2.7.0/tcms_settings_dir/multi_tenant.py` & `kiwitcms-tenants-2.8.0/tcms_settings_dir/multi_tenant.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/admin.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/backends.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/backends.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/checks.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/context_processors.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/context_processors.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/forms.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright (c) 2019-2021 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 import re
 
 from django import forms
 from django.forms.utils import ErrorList
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 
 from django_tenants.postgresql_backend import base as validators
 
+from tcms.core.utils.mailto import custom_email_validators
 from tcms_tenants import models
 from tcms_tenants import utils
 
 
 VALIDATION_RE = re.compile(r"^[a-z0-9]{1,63}$")
 
 
@@ -53,21 +54,24 @@
 class InviteUsersForm(forms.Form):  # pylint: disable=must-inherit-from-model-form
     number_of_fields = 10
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         for i in self.range:
-            self.fields[f"email_{i}"] = forms.CharField(required=False)
+            self.fields[f"email_{i}"] = forms.EmailField(
+                required=False,
+                validators=[custom_email_validators],
+            )
 
     def clean(self):
         emails = set()
 
         for i in self.range:
-            email = self.cleaned_data[f"email_{i}"]
+            email = self.cleaned_data.get(f"email_{i}")
             if email:
                 emails.add(email)
 
         self.cleaned_data["emails"] = emails
 
     @property
     def range(self):
```

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/django.po` & `kiwitcms-tenants-2.8.0/tcms_tenants/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/initialize_tenants.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/management/commands/initialize_tenants.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/menu.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/menu.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/middleware.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/middleware.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0001_initial.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0002_tenant_owner.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0002_tenant_owner.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0003_use_datetime_fields.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0003_use_datetime_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/models.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/oss_utils.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/oss_utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/storage.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/storage.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/invite_users.html` & `kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/invite_users.html`

 * *Files 25% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 
 
 {% block contents %}
     <div class="container-fluid container-cards-pf">
         <form class="form-horizontal" action="{% url 'tcms_tenants:invite-users' %}" method="post">
         {% csrf_token %}
 
-        {% for i in form.range %}
+        {% for field in form %}
             <div class="form-group">
-                <label class="col-md-1 col-lg-1" for="email_{{ i }}">{% trans "Email" %}</label>
-                <div class="col-sm-4 col-md-4 col-lg-4">
-                    <input type="text" id="email_{{ i }}" name="email_{{ i }}" class="form-control">
+                <label class="col-md-1 col-lg-1" for="{{ field.name }}">{% trans "Email" %}</label>
+                <div class="col-sm-4 col-md-4 col-lg-4" {% if field.errors %}has-error{% endif %}">
+                    <input type="text" id="{{ field.name }}" name="{{ field.name }}" value="{{ field.value }}" class="form-control">
+
+                    {{ field.errors }}
                 </div>
             </div>
         {% endfor %}
             <button type="submit" class="btn btn-default btn-lg">{% trans "Save" %}</button>
         </form>
     </div>
 {% endblock %}
```

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/new.html` & `kiwitcms-tenants-2.8.0/tcms_tenants/templates/tcms_tenants/new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/tests/__init__.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc` & `kiwitcms-tenants-2.8.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/urls.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/utils.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tcms_tenants/views.py` & `kiwitcms-tenants-2.8.0/tcms_tenants/views.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/admin.py` & `kiwitcms-tenants-2.8.0/tenant_groups/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/backends.py` & `kiwitcms-tenants-2.8.0/tenant_groups/backends.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/checks.py` & `kiwitcms-tenants-2.8.0/tenant_groups/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/management/commands/refresh_tenant_permissions.py` & `kiwitcms-tenants-2.8.0/tenant_groups/management/commands/refresh_tenant_permissions.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/migrations/0001_initial.py` & `kiwitcms-tenants-2.8.0/tenant_groups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.7.0/tenant_groups/models.py` & `kiwitcms-tenants-2.8.0/tenant_groups/models.py`

 * *Files identical despite different names*

