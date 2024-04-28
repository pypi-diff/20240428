# Comparing `tmp/pyams_security-2.3.0.tar.gz` & `tmp/pyams_security-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security-2.3.0.tar", last modified: Tue Apr  9 18:35:25 2024, max compression
+gzip compressed data, was "dist/pyams_security-2.3.1.tar", last modified: Sun Apr 28 14:59:42 2024, max compression
```

## Comparing `pyams_security-2.3.0.tar` & `pyams_security-2.3.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 10:29:46.000000 pyams_security-2.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 10:29:46.000000 pyams_security-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6772 2024-04-09 18:35:25.000000 pyams_security-2.3.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4874 2024-04-09 18:28:27.000000 pyams_security-2.3.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-01-03 10:29:46.000000 pyams_security-2.3.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 18:35:25.000000 pyams_security-2.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3016 2024-04-09 18:28:27.000000 pyams_security-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/api/
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/credentials.rst
--rw-rw-rw-   0 root         (0) root         (0)     6424 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/manager.rst
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)     7314 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/passwords.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/plugins.rst
--rw-rw-rw-   0 root         (0) root         (0)     5925 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/policy.rst
--rw-rw-rw-   0 root         (0) root         (0)    15805 2024-02-03 01:44:13.000000 pyams_security-2.3.0/src/pyams_security/doctests/principals.rst
--rw-rw-rw-   0 root         (0) root         (0)     3690 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     5633 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/rest.rst
--rw-rw-rw-   0 root         (0) root         (0)     6801 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/doctests/roles.rst
--rw-rw-rw-   0 root         (0) root         (0)    21085 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    19460 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/doctests/users.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-01-24 17:07:04.000000 pyams_security-2.3.0/src/pyams_security/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/include.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    11198 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/interfaces/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4234 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    16708 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/interfaces/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1969 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17669 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
--rw-rw-rw-   0 root         (0) root         (0)    29946 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
--rw-rw-rw-   0 root         (0) root         (0)    16683 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/locales/pyams_security.pot
--rw-rw-rw-   0 root         (0) root         (0)     2433 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/password.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8272 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/password-reset.pt
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-info.pt
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-message.pt
--rw-rw-rw-   0 root         (0) root         (0)    18335 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/principal.py
--rw-rw-rw-   0 root         (0) root         (0)     4658 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/property.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     6297 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/role.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12790 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/security.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9326 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6772 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2583 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:15.000000 pyams_security-2.3.0/src/pyams_security.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-28 14:59:13.000000 pyams_security-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-28 14:59:13.000000 pyams_security-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6809 2024-04-28 14:59:42.000000 pyams_security-2.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4911 2024-04-28 14:59:13.000000 pyams_security-2.3.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-04-28 14:59:13.000000 pyams_security-2.3.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 14:59:42.000000 pyams_security-2.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3016 2024-04-28 14:59:13.000000 pyams_security-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/credentials.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6424 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/manager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/passwords.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/plugins.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5925 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/policy.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15805 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/principals.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5633 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/rest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/roles.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19460 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/doctests/users.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4961 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    11198 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    16708 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/interfaces/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17962 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
+-rw-rw-rw-   0 root         (0) root         (0)    30366 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
+-rw-rw-rw-   0 root         (0) root         (0)    16946 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/locales/pyams_security.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8272 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/password-reset.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-info.pt
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/templates/register-message.pt
+-rw-rw-rw-   0 root         (0) root         (0)    18335 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/principal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/role.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12790 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9326 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-04-28 14:59:13.000000 pyams_security-2.3.1/src/pyams_security/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6809 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 14:59:35.000000 pyams_security-2.3.1/src/pyams_security.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-28 14:59:42.000000 pyams_security-2.3.1/src/pyams_security.egg-info/top_level.txt
```

### Comparing `pyams_security-2.3.0/LICENSE` & `pyams_security-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/PKG-INFO` & `pyams_security-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security
-Version: 2.3.0
+Version: 2.3.1
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - updated translations
+
 2.3.0
 -----
  - allow case-insensitive local user login
 
 2.2.1
 -----
  - added support for custom attributes in roles
```

### Comparing `pyams_security-2.3.0/docs/HISTORY.rst` & `pyams_security-2.3.1/docs/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.3.1
+-----
+ - updated translations
+
 2.3.0
 -----
  - allow case-insensitive local user login
 
 2.2.1
 -----
  - added support for custom attributes in roles
```

### Comparing `pyams_security-2.3.0/docs/README.rst` & `pyams_security-2.3.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/setup.py` & `pyams_security-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.3.0'
+version = '2.3.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_zmi'
 ]
```

### Comparing `pyams_security-2.3.0/src/pyams_security/__init__.py` & `pyams_security-2.3.1/src/pyams_security/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/api/__init__.py` & `pyams_security-2.3.1/src/pyams_security/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/credential.py` & `pyams_security-2.3.1/src/pyams_security/credential.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/README.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/credentials.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/credentials.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/manager.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/manager.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/notifications.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/notifications.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/passwords.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/passwords.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/plugins.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/plugins.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/policy.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/policy.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/principals.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/principals.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/profiles.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/profiles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/rest.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/rest.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/roles.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/roles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/security.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/doctests/users.rst` & `pyams_security-2.3.1/src/pyams_security/doctests/users.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/generations/__init__.py` & `pyams_security-2.3.1/src/pyams_security/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/generations/evolve1.py` & `pyams_security-2.3.1/src/pyams_security/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/include.py` & `pyams_security-2.3.1/src/pyams_security/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/index.py` & `pyams_security-2.3.1/src/pyams_security/index.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/__init__.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/base.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/names.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/names.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/notification.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/plugin.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/profile.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/rest.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/interfaces/site.py` & `pyams_security-2.3.1/src/pyams_security/interfaces/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo` & `pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -173,14 +173,19 @@
 "If enabled, REST API will check requests against currently allowed origins, "
 "and raise an HTTP forbidden exception if not allowed"
 msgstr ""
 "Lorsque cette option est activée, les API REST peuvent vérifier l'origine "
 "des requêtes vis-à-vis des origines autorisées, et lever une exception "
 "lorsqu'une requête est émise depuis une origine non autorisée"
 
+msgid "If enabled, users login will not be case sensitive"
+msgstr ""
+"Activez cette option pour rendre l'identifiant de connexion des utilisateurs "
+"insensible à la casse minuscules/majuscules"
+
 msgid ""
 "If you don't provide a custom login, your login will be your email address..."
 msgstr ""
 "Si vous n'indiquez pas de code utilisateur, vous pourrez utiliser votre "
 "adresse de messagerie pour vous connecter..."
 
 msgid ""
@@ -473,14 +478,17 @@
 msgid ""
 "To confirm your registration, please click on the following link, re-enter "
 "your login and set a new password:"
 msgstr ""
 "Pour confirmer cette inscription, veuillez cliquer sur le lien ci-dessous, "
 "indiquer votre identifiant de connexion et fournir un nouveau mot de passe."
 
+msgid "Use case insensitive login"
+msgstr "Identifiants insensibles à la casse"
+
 msgid "Use internal API"
 msgstr "Utiliser les API internes"
 
 msgid "User email address"
 msgstr "Adresse de messagerie"
 
 msgid "User login"
```

### Comparing `pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po` & `pyams_security-2.3.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #
 # French translations for PyAMS_security package
 # This file is distributed under the same license as the PyAMS_security package.
 # Thierry Florac <tflorac@ulthar.net>, 2015-2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS_security 1.0\n"
-"POT-Creation-Date: 2023-07-05 16:55+0200\n"
+"POT-Creation-Date: 2024-04-10 10:57+0200\n"
 "PO-Revision-Date: 2019-12-21 22:19+0100\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: French\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.8\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
+#. pylint: disable=invalid-name
+#: src/pyams_security/principal.py:60
+msgid "< unknown principal >"
+msgstr "< utilisateur inconnu >"
+
 #: src/pyams_security/include.py:72
 msgid "View public contents"
 msgstr "Voir les contenus publics"
 
 #: src/pyams_security/include.py:76
 msgid "View protected contents"
 msgstr "Voir les contenus protégés"
@@ -52,136 +57,14 @@
 msgid "System manager (role)"
 msgstr "Administrateur (rôle)"
 
 #: src/pyams_security/include.py:119
 msgid "System viewer (role)"
 msgstr "Invité (rôle)"
 
-#. pylint: disable=invalid-name
-#: src/pyams_security/principal.py:59
-msgid "< unknown principal >"
-msgstr "< utilisateur inconnu >"
-
-#: src/pyams_security/interfaces/notification.py:34
-msgid "Enable notifications?"
-msgstr "Activer les notifications ?"
-
-#: src/pyams_security/interfaces/notification.py:35
-msgid "If 'no', mail notifications will be disabled"
-msgstr "Si 'non', les messages de notification ne seront pas activés"
-
-#: src/pyams_security/interfaces/notification.py:39
-msgid "Mailer utility"
-msgstr "Serveur de messagerie"
-
-#: src/pyams_security/interfaces/notification.py:40
-msgid "Mail delivery utility used to send notifications"
-msgstr "Serveur de messagerie utilisé pour l'envoi des notifications"
-
-#: src/pyams_security/interfaces/notification.py:48
-msgid "Notifications can't be enabled without mailer utility"
-msgstr ""
-"Les notifications ne peuvent pas être activés sans sélection d'un serveur de "
-"messagerie"
-
-#: src/pyams_security/interfaces/notification.py:53
-msgid "Service name"
-msgstr "Nom du service"
-
-#: src/pyams_security/interfaces/notification.py:54
-msgid "Name of service as defined in registration mail subject"
-msgstr "Ce nom sera inscrit dans le sujet des messages de notification"
-
-#: src/pyams_security/interfaces/notification.py:58
-msgid "Service owner"
-msgstr "Propriétaire du service"
-
-#: src/pyams_security/interfaces/notification.py:59
-msgid ""
-"Name of the entity providing this service, which will be visible in "
-"notifications messages"
-msgstr ""
-"Nom du service ou de l'entité fournissant ce service, qui sera indiqué dans "
-"les messages de notification"
-
-#: src/pyams_security/interfaces/notification.py:63
-msgid "Sender name"
-msgstr "Nom d'expéditeur"
-
-#: src/pyams_security/interfaces/notification.py:64
-msgid "Visible name of registration mail sender"
-msgstr "Nom de l'expéditeur indiqué dans les messages de notification"
-
-#: src/pyams_security/interfaces/notification.py:67
-msgid "Sender email"
-msgstr "Adresse de l'expéditeur"
-
-#: src/pyams_security/interfaces/notification.py:68
-msgid "Email address of registration mail sender"
-msgstr "Nom de l'adresse d'expédition des messages de notification"
-
-#: src/pyams_security/interfaces/notification.py:71
-msgid "Subject prefix"
-msgstr "Préfixe des sujets"
-
-#: src/pyams_security/interfaces/notification.py:72
-msgid ""
-"This prefix will be inserted into subject prefix of each notification message"
-msgstr "Ce préfixe sera inséré en tête du sujet des messages de notification"
-
-#: src/pyams_security/interfaces/notification.py:77
-msgid "Confirmation template"
-msgstr "Message de confirmation"
-
-#: src/pyams_security/interfaces/notification.py:78
-#, python-format
-msgid ""
-"This template will be used instead of default template to send notification "
-"when a user is registered by a system administrator; you can use some user "
-"properties into the message body, like: {login}, {email}, {firstname}, "
-"{lastname}, {title} or {company_name}; message activation link and footer "
-"are added automatically"
-msgstr ""
-"S'il est renseigné, ce modèle sera utilisé en lieu et place du modèle par "
-"défaut pour l'envoi des notifications lorsqu'un utilisateur est inscrit par "
-"un administrateur ; vous pouvez utiliser certaines propriétés de "
-"l'utilisateur dans le corps du message, en les entourant avec des "
-"accolades : code utilisateur ({login}), adresse de messagerie ({email}), "
-"prénom ({firstname}), nom ({name}), titre ({title}) et société "
-"({company_name}) ; le contenu du lien de confirmation ainsi que le pied du "
-"message seront ajoutés automatiquement"
-
-#: src/pyams_security/interfaces/notification.py:86
-msgid "Registration template"
-msgstr "Message d'enregistrement"
-
-#: src/pyams_security/interfaces/notification.py:87
-#, python-format
-msgid ""
-"This template will be used instead of default template to send notificaiton "
-"when a user is auto-registered; you can use some user properties into the "
-"message body, like: {login}, {email}, {firstname}, {lastname}, {title} or "
-"{company_name}; message activation link and footer are added automatically"
-msgstr ""
-"S'il est renseigné, ce modèle sera utilisé en lieu et place du modèle par "
-"défaut pour l'envoi des notifications lorsqu'un utilisateur s'est auto-"
-"inscrit ; vous pouvez utiliser certaines propriétés de l'utilisateur dans le "
-"corps du message, en les entourant avec des accolades : code utilisateur "
-"({login}), adresse de messagerie ({email}), prénom ({firstname}), nom "
-"({name}), titre ({title}) et société ({company_name}) ; le contenu du lien "
-"de confirmation ainsi que le pied du message seront ajoutés automatiquement"
-
-#: src/pyams_security/interfaces/notification.py:94
-msgid "Email signature"
-msgstr "Signature"
-
-#: src/pyams_security/interfaces/notification.py:95
-msgid "Text displayed in email footer"
-msgstr "Ce texte sera affiché dans le pied des messages de notification"
-
 #: src/pyams_security/interfaces/names.py:35
 msgid "User login"
 msgstr "Code utilisateur"
 
 #: src/pyams_security/interfaces/plugin.py:43
 msgid "Plug-in prefix"
 msgstr "Préfixe du module"
@@ -219,203 +102,213 @@
 msgid "Admin. password"
 msgstr "Mot de passe"
 
 #: src/pyams_security/interfaces/plugin.py:195
 msgid "Users folder plug-in"
 msgstr "Dossier d'utilisateurs"
 
-#: src/pyams_security/interfaces/plugin.py:228
+#: src/pyams_security/interfaces/plugin.py:203
+msgid "Use case insensitive login"
+msgstr "Identifiants insensibles à la casse"
+
+#: src/pyams_security/interfaces/plugin.py:204
+msgid "If enabled, users login will not be case sensitive"
+msgstr ""
+"Activez cette option pour rendre l'identifiant de connexion des utilisateurs "
+"insensible à la casse minuscules/majuscules"
+
+#: src/pyams_security/interfaces/plugin.py:233
 msgid ""
 "Your password must contain at least three of these kinds of characters: "
 "lowercase letters, uppercase letters, numbers and special characters"
 msgstr ""
 "Votre mot de passe doit contenir au moins trois de ces types de caractères : "
 "minuscules, majuscules, chiffres et autres caractères"
 
-#: src/pyams_security/interfaces/plugin.py:241
+#: src/pyams_security/interfaces/plugin.py:246
 msgid ""
 "If you don't provide a custom login, your login will be your email address..."
 msgstr ""
 "Si vous n'indiquez pas de code utilisateur, vous pourrez utiliser votre "
 "adresse de messagerie pour vous connecter..."
 
-#: src/pyams_security/interfaces/plugin.py:251
+#: src/pyams_security/interfaces/plugin.py:256
 msgid "E-mail address"
 msgstr "Adresse de messagerie"
 
-#: src/pyams_security/interfaces/plugin.py:252
+#: src/pyams_security/interfaces/plugin.py:257
 msgid ""
 "An email will be sent to this address to validate account activation; it "
 "will be used as your future user login"
 msgstr ""
 "Un message sera envoyé à cette adresse, contenant un lien pour vous "
 "permettre de la confirmer et d'activer votre compte ; elle pourra être "
 "utilisée comme identifiant de connexion si vous n'avez pas indiqué de code "
 "utilisateur"
 
-#: src/pyams_security/interfaces/plugin.py:260
+#: src/pyams_security/interfaces/plugin.py:265
 msgid "Your email address is not valid!"
 msgstr "Votre adresse de messagerie est incorrecte !"
 
-#: src/pyams_security/interfaces/plugin.py:262
-#: src/pyams_security/interfaces/plugin.py:339
+#: src/pyams_security/interfaces/plugin.py:267
+#: src/pyams_security/interfaces/plugin.py:344
 msgid "First name"
 msgstr "Prénom"
 
-#: src/pyams_security/interfaces/plugin.py:265
-#: src/pyams_security/interfaces/plugin.py:342
+#: src/pyams_security/interfaces/plugin.py:270
+#: src/pyams_security/interfaces/plugin.py:347
 msgid "Last name"
 msgstr "Nom"
 
-#: src/pyams_security/interfaces/plugin.py:268
-#: src/pyams_security/interfaces/plugin.py:347
+#: src/pyams_security/interfaces/plugin.py:273
+#: src/pyams_security/interfaces/plugin.py:352
 msgid "Company name"
 msgstr "Société"
 
-#: src/pyams_security/interfaces/plugin.py:271
-#: src/pyams_security/interfaces/plugin.py:300
-#: src/pyams_security/interfaces/plugin.py:356
+#: src/pyams_security/interfaces/plugin.py:276
+#: src/pyams_security/interfaces/plugin.py:305
+#: src/pyams_security/interfaces/plugin.py:361
 msgid "Password"
 msgstr "Mot de passe"
 
-#: src/pyams_security/interfaces/plugin.py:272
+#: src/pyams_security/interfaces/plugin.py:277
 msgid ""
 "Password must be at least 8 characters long, and contain at least three "
 "kinds of characters between lowercase letters, uppercase letters, numbers "
 "and special characters"
 msgstr ""
 "Le mot de passe doit être composé d'au moins huit caractères, et contenir au "
 "moins trois types de caractères parmi les lettres minuscules, les lettres "
 "majuscules, les chiffres et les caractères spéciaux"
 
-#: src/pyams_security/interfaces/plugin.py:280
-#: src/pyams_security/interfaces/plugin.py:304
-#: src/pyams_security/interfaces/plugin.py:360
+#: src/pyams_security/interfaces/plugin.py:285
+#: src/pyams_security/interfaces/plugin.py:309
+#: src/pyams_security/interfaces/plugin.py:365
 msgid "Confirmed password"
 msgstr "Confirmation du mot de passe"
 
-#: src/pyams_security/interfaces/plugin.py:287
-#: src/pyams_security/interfaces/plugin.py:311
+#: src/pyams_security/interfaces/plugin.py:292
+#: src/pyams_security/interfaces/plugin.py:316
 msgid "You didn't confirmed your password correctly!"
 msgstr "Vous n'avez pas confirmé votre mot de passe correctement !"
 
-#: src/pyams_security/interfaces/plugin.py:294
-#: src/pyams_security/interfaces/plugin.py:385
+#: src/pyams_security/interfaces/plugin.py:299
+#: src/pyams_security/interfaces/plugin.py:390
 msgid "Activation hash"
 msgstr "Clé d'activation"
 
-#: src/pyams_security/interfaces/plugin.py:330
+#: src/pyams_security/interfaces/plugin.py:335
 msgid "User email address"
 msgstr "Adresse de messagerie"
 
-#: src/pyams_security/interfaces/plugin.py:337
+#: src/pyams_security/interfaces/plugin.py:342
 msgid "Given email address is not valid!"
 msgstr "L'adresse de messagerie indiquée est incorrecte !"
 
-#: src/pyams_security/interfaces/plugin.py:350
+#: src/pyams_security/interfaces/plugin.py:355
 msgid "Password manager name"
 msgstr "Gestionnaire de mots de passe"
 
-#: src/pyams_security/interfaces/plugin.py:351
+#: src/pyams_security/interfaces/plugin.py:356
 msgid "Utility used to encrypt user password"
 msgstr "Utilitaire utilisé pour le cryptage des mots de passe"
 
-#: src/pyams_security/interfaces/plugin.py:364
+#: src/pyams_security/interfaces/plugin.py:369
 msgid "Wait confirmation?"
 msgstr "Attendre la confirmation ?"
 
-#: src/pyams_security/interfaces/plugin.py:365
+#: src/pyams_security/interfaces/plugin.py:370
 msgid ""
 "If 'no', user will be activated immediately without waiting email "
 "confirmation"
 msgstr ""
 "Si 'non', ce compte utilisateur sera activé immédiatement, sans attendre sa "
 "confirmation"
 
-#: src/pyams_security/interfaces/plugin.py:374
+#: src/pyams_security/interfaces/plugin.py:379
 msgid "You can't activate an account without setting a password!"
 msgstr "Vous ne pouvez pas activer un profil sans mot de passe!"
 
-#: src/pyams_security/interfaces/plugin.py:376
+#: src/pyams_security/interfaces/plugin.py:381
 msgid "Self-registered profile?"
 msgstr "Profil auto-enregistré ?"
 
-#: src/pyams_security/interfaces/plugin.py:381
+#: src/pyams_security/interfaces/plugin.py:386
 msgid "Activation secret key"
 msgstr "Clé secrète"
 
-#: src/pyams_security/interfaces/plugin.py:382
+#: src/pyams_security/interfaces/plugin.py:387
 msgid "This private secret is used to create and check activation hash"
 msgstr ""
 "Cette clé secrète est utilisée pour créer et vérifier la clé d'activation"
 
-#: src/pyams_security/interfaces/plugin.py:386
+#: src/pyams_security/interfaces/plugin.py:391
 msgid ""
 "This hash is provided into activation message URL. Activation hash is "
 "missing for local users which were registered without waiting their "
 "confirmation."
 msgstr ""
 "Cette clé d'activation est fournie dans le message de confirmation de "
 "l'inscription ; elle n'est pas définie pour les utilisateurs pour lesquels "
 "l'attente de confirmation n'a pas été demandée"
 
-#: src/pyams_security/interfaces/plugin.py:391
+#: src/pyams_security/interfaces/plugin.py:396
 msgid "Activated"
 msgstr "Activé"
 
-#: src/pyams_security/interfaces/plugin.py:395
+#: src/pyams_security/interfaces/plugin.py:400
 msgid "Activation date"
 msgstr "Date d'activation"
 
-#: src/pyams_security/interfaces/plugin.py:398
+#: src/pyams_security/interfaces/plugin.py:403
 msgid "Password reset hash"
 msgstr "Hash de reset"
 
-#: src/pyams_security/interfaces/plugin.py:399
+#: src/pyams_security/interfaces/plugin.py:404
 msgid ""
 "This hash is provided when a user is asking for a password reset; please "
 "note that password reset request should not update password..."
 msgstr ""
 "Cette clé de hashage est définie lorsqu'un utilisateur demande une "
 "réinitialisation de son mot de passe ; cette demande de réinitialisation "
 "n'invalide pas l'ancien mot de passe..."
 
-#: src/pyams_security/interfaces/plugin.py:404
+#: src/pyams_security/interfaces/plugin.py:409
 msgid "Password reset hash date"
 msgstr "Date de reset"
 
-#: src/pyams_security/interfaces/plugin.py:433
+#: src/pyams_security/interfaces/plugin.py:438
 msgid "Groups folder plug-in"
 msgstr "Dossier de groupes"
 
-#: src/pyams_security/interfaces/plugin.py:450
+#: src/pyams_security/interfaces/plugin.py:455
 msgid "Group ID"
 msgstr "ID du groupe"
 
-#: src/pyams_security/interfaces/plugin.py:451
+#: src/pyams_security/interfaces/plugin.py:456
 msgid "This ID should be unique between all groups"
 msgstr "Cet ID doit être unique entre tous les groupes"
 
-#: src/pyams_security/interfaces/plugin.py:455
+#: src/pyams_security/interfaces/plugin.py:460
 msgid "Title"
 msgstr "Nom"
 
-#: src/pyams_security/interfaces/plugin.py:456
+#: src/pyams_security/interfaces/plugin.py:461
 msgid "Public label of this group"
 msgstr "Libellé public de ce groupe"
 
-#: src/pyams_security/interfaces/plugin.py:459
+#: src/pyams_security/interfaces/plugin.py:464
 msgid "Description"
 msgstr "Description"
 
-#: src/pyams_security/interfaces/plugin.py:462
+#: src/pyams_security/interfaces/plugin.py:467
 msgid "Group principals"
 msgstr "Mandataires du groupe"
 
-#: src/pyams_security/interfaces/plugin.py:463
+#: src/pyams_security/interfaces/plugin.py:468
 msgid "IDs of principals contained in this group"
 msgstr ""
 "Liste des mandataires présents dans ce groupe ; ces mandataires peuvent être "
 "des utilisateurs, mais également d'autres groupes"
 
 #: src/pyams_security/interfaces/rest.py:37
 msgid "Check request origin"
@@ -434,37 +327,14 @@
 msgid "Allowed origins"
 msgstr "Origines autorisées"
 
 #: src/pyams_security/interfaces/rest.py:45
 msgid "List of allowed origins URLs using CORS requests"
 msgstr "Liste des URLs d'origine autorisées pour les requêtes CORS"
 
-#: src/pyams_security/interfaces/site.py:31
-msgid "Site managers"
-msgstr "Administrateurs"
-
-#: src/pyams_security/interfaces/site.py:32
-msgid ""
-"These principals are allowed to manage the whole application environment"
-msgstr ""
-"Les détenteurs de ce rôle sont habilités à gérer tous les paramètres de "
-"l'application"
-
-#: src/pyams_security/interfaces/site.py:37
-msgid "Site viewers"
-msgstr "Invités"
-
-#: src/pyams_security/interfaces/site.py:38
-msgid ""
-"These principals are allowed to view some application settings, without "
-"update"
-msgstr ""
-"Les détenteurs de ce rôle peuvent accéder à certains écrans de l'interface d'administration, "
-"mais sans droit de mise à jour"
-
 #: src/pyams_security/interfaces/profile.py:34
 msgid "Profile's avatar"
 msgstr "Image du profil"
 
 #: src/pyams_security/interfaces/profile.py:35
 msgid "This picture will be associated to your user profile"
 msgstr "Cette image sera associée à votre profil utilisateur"
@@ -501,146 +371,273 @@
 msgid "Directory plug-ins"
 msgstr "Modules d'annuaires"
 
 #: src/pyams_security/interfaces/__init__.py:102
 msgid "The plug-in can be used to extract principals information"
 msgstr "Ces modules peuvent être utilisés pour rechercher des mandataires"
 
-#: src/pyams_security/interfaces/__init__.py:135
+#: src/pyams_security/interfaces/__init__.py:147
 msgid "Access menu from home"
 msgstr "Ajouter un accès depuis l'accueil"
 
-#: src/pyams_security/interfaces/__init__.py:136
+#: src/pyams_security/interfaces/__init__.py:148
 msgid ""
 "If 'yes', a menu will be displayed to get access to security manager from "
 "site admin home page"
 msgstr ""
 "Si 'oui', un menu d'accès au gestionnaire de sécurité sera ajouté depuis la "
 "page d'accueil de l'interface d'acministration du site"
 
-#: src/pyams_security/interfaces/__init__.py:157
+#: src/pyams_security/interfaces/__init__.py:191
 msgid "Inherit parent security?"
 msgstr "Héritage de la sécurité ?"
 
-#: src/pyams_security/interfaces/__init__.py:158
+#: src/pyams_security/interfaces/__init__.py:192
 msgid "Get access control entries (ACE) inherited from parent levels"
 msgstr ""
 "Combiner les règles de contrôle d'accès (ACE) définies localement avec "
 "celles héritées du parent"
 
-#: src/pyams_security/interfaces/__init__.py:163
+#: src/pyams_security/interfaces/__init__.py:197
 msgid "Public denied permissions"
 msgstr "Permissions publiques retirées"
 
-#: src/pyams_security/interfaces/__init__.py:164
+#: src/pyams_security/interfaces/__init__.py:198
 msgid ""
 "These permissions will be denied to all users. Denied permissions take "
 "precedence over granted ones."
 msgstr ""
 "Ces permissions seront retirées aux utilisateurs non authentifiés ; les "
 "permissions retirées sont prioritaires par rapport aux permissions accordées"
 
-#: src/pyams_security/interfaces/__init__.py:169
+#: src/pyams_security/interfaces/__init__.py:203
 msgid "Public granted permissions"
 msgstr "Permissions publiques accordées"
 
-#: src/pyams_security/interfaces/__init__.py:170
+#: src/pyams_security/interfaces/__init__.py:204
 msgid "These permissions will be granted to all users"
 msgstr "Ces permissions seront accordées à tous les utilisateurs"
 
-#: src/pyams_security/interfaces/__init__.py:174
+#: src/pyams_security/interfaces/__init__.py:208
 msgid "Authenticated denied permissions"
 msgstr "Permissions authentifiées retirées"
 
-#: src/pyams_security/interfaces/__init__.py:175
+#: src/pyams_security/interfaces/__init__.py:209
 msgid ""
 "These permissions will be denied to authenticated users. Denied permissions "
 "take precedence over granted ones."
 msgstr ""
 "Ces permissions seront retirées aux utilisateurs authentifiés ; les "
 "permissions retirées sont prioritaires par rapport aux permissions accordées"
 
-#: src/pyams_security/interfaces/__init__.py:181
+#: src/pyams_security/interfaces/__init__.py:215
 msgid "Authenticated granted permissions"
 msgstr "Permissions authentifiées accordées"
 
-#: src/pyams_security/interfaces/__init__.py:182
+#: src/pyams_security/interfaces/__init__.py:216
 msgid "These permissions will be granted to authenticated users"
 msgstr "Ces permissions seront accordées aux utilisateurs authentifiés"
 
-#: src/pyams_security/interfaces/__init__.py:186
+#: src/pyams_security/interfaces/__init__.py:220
 msgid "Inherit parent roles?"
 msgstr "Héritage des rôles ?"
 
-#: src/pyams_security/interfaces/__init__.py:187
+#: src/pyams_security/interfaces/__init__.py:221
 msgid "Get roles granted on parent levels"
 msgstr "Hériter des rôles affectés aux niveaux parents"
 
-#: src/pyams_security/plugin/userfolder.py:197
+#: src/pyams_security/interfaces/site.py:31
+msgid "Site managers"
+msgstr "Administrateurs"
+
+#: src/pyams_security/interfaces/site.py:32
+msgid ""
+"These principals are allowed to manage the whole application environment"
+msgstr ""
+"Les détenteurs de ce rôle sont habilités à gérer tous les paramètres de "
+"l'application"
+
+#: src/pyams_security/interfaces/site.py:37
+msgid "Site viewers"
+msgstr "Invités"
+
+#: src/pyams_security/interfaces/site.py:38
+msgid ""
+"These principals are allowed to view some application settings, without "
+"update"
+msgstr ""
+"Les détenteurs de ce rôle peuvent accéder à certains écrans de l'interface "
+"d'administration, mais sans droit de mise à jour"
+
+#: src/pyams_security/interfaces/notification.py:34
+msgid "Enable notifications?"
+msgstr "Activer les notifications ?"
+
+#: src/pyams_security/interfaces/notification.py:35
+msgid "If 'no', mail notifications will be disabled"
+msgstr "Si 'non', les messages de notification ne seront pas activés"
+
+#: src/pyams_security/interfaces/notification.py:39
+msgid "Mailer utility"
+msgstr "Serveur de messagerie"
+
+#: src/pyams_security/interfaces/notification.py:40
+msgid "Mail delivery utility used to send notifications"
+msgstr "Serveur de messagerie utilisé pour l'envoi des notifications"
+
+#: src/pyams_security/interfaces/notification.py:48
+msgid "Notifications can't be enabled without mailer utility"
+msgstr ""
+"Les notifications ne peuvent pas être activés sans sélection d'un serveur de "
+"messagerie"
+
+#: src/pyams_security/interfaces/notification.py:53
+msgid "Service name"
+msgstr "Nom du service"
+
+#: src/pyams_security/interfaces/notification.py:54
+msgid "Name of service as defined in registration mail subject"
+msgstr "Ce nom sera inscrit dans le sujet des messages de notification"
+
+#: src/pyams_security/interfaces/notification.py:58
+msgid "Service owner"
+msgstr "Propriétaire du service"
+
+#: src/pyams_security/interfaces/notification.py:59
+msgid ""
+"Name of the entity providing this service, which will be visible in "
+"notifications messages"
+msgstr ""
+"Nom du service ou de l'entité fournissant ce service, qui sera indiqué dans "
+"les messages de notification"
+
+#: src/pyams_security/interfaces/notification.py:63
+msgid "Sender name"
+msgstr "Nom d'expéditeur"
+
+#: src/pyams_security/interfaces/notification.py:64
+msgid "Visible name of registration mail sender"
+msgstr "Nom de l'expéditeur indiqué dans les messages de notification"
+
+#: src/pyams_security/interfaces/notification.py:67
+msgid "Sender email"
+msgstr "Adresse de l'expéditeur"
+
+#: src/pyams_security/interfaces/notification.py:68
+msgid "Email address of registration mail sender"
+msgstr "Nom de l'adresse d'expédition des messages de notification"
+
+#: src/pyams_security/interfaces/notification.py:71
+msgid "Subject prefix"
+msgstr "Préfixe des sujets"
+
+#: src/pyams_security/interfaces/notification.py:72
+msgid ""
+"This prefix will be inserted into subject prefix of each notification message"
+msgstr "Ce préfixe sera inséré en tête du sujet des messages de notification"
+
+#: src/pyams_security/interfaces/notification.py:77
+msgid "Confirmation template"
+msgstr "Message de confirmation"
+
+#: src/pyams_security/interfaces/notification.py:78
+#, python-format
+msgid ""
+"This template will be used instead of default template to send notification "
+"when a user is registered by a system administrator; you can use some user "
+"properties into the message body, like: {login}, {email}, {firstname}, "
+"{lastname}, {title} or {company_name}; message activation link and footer "
+"are added automatically"
+msgstr ""
+"S'il est renseigné, ce modèle sera utilisé en lieu et place du modèle par "
+"défaut pour l'envoi des notifications lorsqu'un utilisateur est inscrit par "
+"un administrateur ; vous pouvez utiliser certaines propriétés de "
+"l'utilisateur dans le corps du message, en les entourant avec des "
+"accolades : code utilisateur ({login}), adresse de messagerie ({email}), "
+"prénom ({firstname}), nom ({name}), titre ({title}) et société "
+"({company_name}) ; le contenu du lien de confirmation ainsi que le pied du "
+"message seront ajoutés automatiquement"
+
+#: src/pyams_security/interfaces/notification.py:86
+msgid "Registration template"
+msgstr "Message d'enregistrement"
+
+#: src/pyams_security/interfaces/notification.py:87
+#, python-format
+msgid ""
+"This template will be used instead of default template to send notificaiton "
+"when a user is auto-registered; you can use some user properties into the "
+"message body, like: {login}, {email}, {firstname}, {lastname}, {title} or "
+"{company_name}; message activation link and footer are added automatically"
+msgstr ""
+"S'il est renseigné, ce modèle sera utilisé en lieu et place du modèle par "
+"défaut pour l'envoi des notifications lorsqu'un utilisateur s'est auto-"
+"inscrit ; vous pouvez utiliser certaines propriétés de l'utilisateur dans le "
+"corps du message, en les entourant avec des accolades : code utilisateur "
+"({login}), adresse de messagerie ({email}), prénom ({firstname}), nom "
+"({name}), titre ({title}) et société ({company_name}) ; le contenu du lien "
+"de confirmation ainsi que le pied du message seront ajoutés automatiquement"
+
+#: src/pyams_security/interfaces/notification.py:94
+msgid "Email signature"
+msgstr "Signature"
+
+#: src/pyams_security/interfaces/notification.py:95
+msgid "Text displayed in email footer"
+msgstr "Ce texte sera affiché dans le pied des messages de notification"
+
+#: src/pyams_security/plugin/userfolder.py:216
 #, python-format
 msgid "{prefix}{subject}"
 msgstr "{prefix}{subject}"
 
-#: src/pyams_security/plugin/userfolder.py:245
+#: src/pyams_security/plugin/userfolder.py:265
+#: src/pyams_security/plugin/userfolder.py:269
 msgid "Please confirm registration"
 msgstr "Veuillez confirmer votre inscription"
 
-#: src/pyams_security/plugin/userfolder.py:256
+#: src/pyams_security/plugin/userfolder.py:280
 msgid "Password reset"
 msgstr "Réinitialisation du mot de passe"
 
-#: src/pyams_security/plugin/userfolder.py:348
-#: src/pyams_security/plugin/userfolder.py:353
+#: src/pyams_security/plugin/userfolder.py:371
+#: src/pyams_security/plugin/userfolder.py:376
 msgid "Can't activate profile with given params!"
 msgstr ""
 "Impossible de confirmer votre inscription avec les paramètres fournis !"
 
-#: src/pyams_security/plugin/userfolder.py:371
+#: src/pyams_security/plugin/userfolder.py:394
 msgid "Invalid reset request!"
 msgstr "Demande de réinitialisation invalide !"
 
-#: src/pyams_security/plugin/userfolder.py:373
+#: src/pyams_security/plugin/userfolder.py:396
 msgid "Can't reset password with given params!"
 msgstr ""
 "Impossible de réinitialiser votre mot de passe avec les paramètres fournis !"
 
-#: src/pyams_security/plugin/userfolder.py:376
+#: src/pyams_security/plugin/userfolder.py:399
 msgid "Your password reset hash is no longer valid!"
 msgstr "Votre lien de réinitialisation du mot de passe n'est plus valide !"
 
-#: src/pyams_security/plugin/templates/register-info.pt:2
+#: src/pyams_security/plugin/templates/password-reset.pt:7
+msgid "${header} Password reset"
+msgstr "${header} Réinitialisation de mot de passe"
+
 #: src/pyams_security/plugin/templates/password-reset.pt:11
 #: src/pyams_security/plugin/templates/register-message.pt:2
+#: src/pyams_security/plugin/templates/register-info.pt:2
 msgid "Hello,"
 msgstr "Bonjour,"
 
-#: src/pyams_security/plugin/templates/register-info.pt:3
 #: src/pyams_security/plugin/templates/password-reset.pt:12
 #: src/pyams_security/plugin/templates/register-message.pt:3
+#: src/pyams_security/plugin/templates/register-info.pt:3
 msgid "${service_name} is a service provided by ${service_owner}."
 msgstr "${service_name} est un service fourni par ${service_owner}"
 
-#: src/pyams_security/plugin/templates/register-info.pt:5
-msgid ""
-"A new account has been created for your email address, that you may confirm "
-"before being able to use the service."
-msgstr ""
-"Un nouveau compte utilisateur vient d'être créé pour votre adresse de "
-"messagerie, que vous devez confirmer avant de pouvoir utiliser ce service."
-
-#: src/pyams_security/plugin/templates/register-info.pt:7
-#: src/pyams_security/plugin/templates/register-body.pt:12
-msgid "The login that was given to your account is: ${login}."
-msgstr ""
-"L'identifiant de connexion qui a été fourni pour votre compte est : ${login}."
-
-#: src/pyams_security/plugin/templates/password-reset.pt:7
-msgid "${header} Password reset"
-msgstr "${header} Réinitialisation de mot de passe"
-
 #: src/pyams_security/plugin/templates/password-reset.pt:14
 msgid "A password reset has been requested for your account: ${login}."
 msgstr ""
 "Une demande de réinitialisation du mot de passe a été effectuée pour votre "
 "compte : ${login}."
 
 #: src/pyams_security/plugin/templates/password-reset.pt:15
@@ -662,26 +659,24 @@
 "réinitialisation de votre mot de passe."
 
 #: src/pyams_security/plugin/templates/password-reset.pt:22
 #: src/pyams_security/plugin/templates/register-body.pt:20
 msgid "Thank you for using our services."
 msgstr "Merci d'utiliser nos services."
 
-#: src/pyams_security/plugin/templates/register-message.pt:5
-msgid ""
-"You have registered a new account that you may confirm before being able to "
-"use the service."
-msgstr ""
-"Vous avez enregistré un nouveau compte que vous devez confirmer avant de "
-"pouvoir utiliser ce service."
-
 #: src/pyams_security/plugin/templates/register-body.pt:7
 msgid "${header} Registration notice"
 msgstr "${header} Inscription effectuée"
 
+#: src/pyams_security/plugin/templates/register-body.pt:12
+#: src/pyams_security/plugin/templates/register-info.pt:7
+msgid "The login that was given to your account is: ${login}."
+msgstr ""
+"L'identifiant de connexion qui a été fourni pour votre compte est : ${login}."
+
 #: src/pyams_security/plugin/templates/register-body.pt:13
 msgid ""
 "To confirm your registration, please click on the following link, re-enter "
 "your login and set a new password:"
 msgstr ""
 "Pour confirmer cette inscription, veuillez cliquer sur le lien ci-dessous, "
 "indiquer votre identifiant de connexion et fournir un nouveau mot de passe."
@@ -691,14 +686,30 @@
 "If you don't want to confirm this registration, please just ignore this "
 "message and your registration information will be deleted within 30 days."
 msgstr ""
 "Si vous ne souhaitez pas confirmer cette inscription, ou si celle-ci a été "
 "faite sans votre consentement, il vous suffit d'ignorer ce message et votre "
 "inscription sera supprimée automatiquement dans un délai de 30 jours"
 
+#: src/pyams_security/plugin/templates/register-message.pt:5
+msgid ""
+"You have registered a new account that you may confirm before being able to "
+"use the service."
+msgstr ""
+"Vous avez enregistré un nouveau compte que vous devez confirmer avant de "
+"pouvoir utiliser ce service."
+
+#: src/pyams_security/plugin/templates/register-info.pt:5
+msgid ""
+"A new account has been created for your email address, that you may confirm "
+"before being able to use the service."
+msgstr ""
+"Un nouveau compte utilisateur vient d'être créé pour votre adresse de "
+"messagerie, que vous devez confirmer avant de pouvoir utiliser ce service."
+
 #~ msgid "Enable free registration?"
 #~ msgstr "Autoriser l'inscription publique ?"
 
 #~ msgid "If 'Yes', any use will be able to create a new user account"
 #~ msgstr ""
 #~ "Si 'oui', toute personne visitant le site sera à même de s'enregistrer et "
 #~ "de faire une demande de création de compte utilisateur"
```

### Comparing `pyams_security-2.3.0/src/pyams_security/locales/pyams_security.pot` & `pyams_security-2.3.1/src/pyams_security/locales/pyams_security.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-07-05 16:55+0200\n"
+"POT-Creation-Date: 2024-04-10 10:57+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
+#. pylint: disable=invalid-name
+#: ./src/pyams_security/principal.py:60
+msgid "< unknown principal >"
+msgstr ""
+
 #: ./src/pyams_security/include.py:72
 msgid "View public contents"
 msgstr ""
 
 #: ./src/pyams_security/include.py:76
 msgid "View protected contents"
 msgstr ""
@@ -52,117 +57,14 @@
 msgid "System manager (role)"
 msgstr ""
 
 #: ./src/pyams_security/include.py:119
 msgid "System viewer (role)"
 msgstr ""
 
-#. pylint: disable=invalid-name
-#: ./src/pyams_security/principal.py:59
-msgid "< unknown principal >"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:34
-msgid "Enable notifications?"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:35
-msgid "If 'no', mail notifications will be disabled"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:39
-msgid "Mailer utility"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:40
-msgid "Mail delivery utility used to send notifications"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:48
-msgid "Notifications can't be enabled without mailer utility"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:53
-msgid "Service name"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:54
-msgid "Name of service as defined in registration mail subject"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:58
-msgid "Service owner"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:59
-msgid ""
-"Name of the entity providing this service, which will be visible in "
-"notifications messages"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:63
-msgid "Sender name"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:64
-msgid "Visible name of registration mail sender"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:67
-msgid "Sender email"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:68
-msgid "Email address of registration mail sender"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:71
-msgid "Subject prefix"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:72
-msgid ""
-"This prefix will be inserted into subject prefix of each notification message"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:77
-msgid "Confirmation template"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:78
-#, python-format
-msgid ""
-"This template will be used instead of default template to send notification "
-"when a user is registered by a system administrator; you can use some user "
-"properties into the message body, like: {login}, {email}, {firstname}, "
-"{lastname}, {title} or {company_name}; message activation link and footer are"
-" added automatically"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:86
-msgid "Registration template"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:87
-#, python-format
-msgid ""
-"This template will be used instead of default template to send notificaiton "
-"when a user is auto-registered; you can use some user properties into the "
-"message body, like: {login}, {email}, {firstname}, {lastname}, {title} or "
-"{company_name}; message activation link and footer are added automatically"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:94
-msgid "Email signature"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/notification.py:95
-msgid "Text displayed in email footer"
-msgstr ""
-
 #: ./src/pyams_security/interfaces/names.py:35
 msgid "User login"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/plugin.py:43
 msgid "Plug-in prefix"
 msgstr ""
@@ -196,182 +98,190 @@
 msgid "Admin. password"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/plugin.py:195
 msgid "Users folder plug-in"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:228
+#: ./src/pyams_security/interfaces/plugin.py:203
+msgid "Use case insensitive login"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/plugin.py:204
+msgid "If enabled, users login will not be case sensitive"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/plugin.py:233
 msgid ""
 "Your password must contain at least three of these kinds of characters: "
 "lowercase letters, uppercase letters, numbers and special characters"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:241
+#: ./src/pyams_security/interfaces/plugin.py:246
 msgid ""
 "If you don't provide a custom login, your login will be your email address..."
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:251
+#: ./src/pyams_security/interfaces/plugin.py:256
 msgid "E-mail address"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:252
+#: ./src/pyams_security/interfaces/plugin.py:257
 msgid ""
 "An email will be sent to this address to validate account activation; it will"
 " be used as your future user login"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:260
+#: ./src/pyams_security/interfaces/plugin.py:265
 msgid "Your email address is not valid!"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:262
-#: ./src/pyams_security/interfaces/plugin.py:339
+#: ./src/pyams_security/interfaces/plugin.py:267
+#: ./src/pyams_security/interfaces/plugin.py:344
 msgid "First name"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:265
-#: ./src/pyams_security/interfaces/plugin.py:342
+#: ./src/pyams_security/interfaces/plugin.py:270
+#: ./src/pyams_security/interfaces/plugin.py:347
 msgid "Last name"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:268
-#: ./src/pyams_security/interfaces/plugin.py:347
+#: ./src/pyams_security/interfaces/plugin.py:273
+#: ./src/pyams_security/interfaces/plugin.py:352
 msgid "Company name"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:271
-#: ./src/pyams_security/interfaces/plugin.py:300
-#: ./src/pyams_security/interfaces/plugin.py:356
+#: ./src/pyams_security/interfaces/plugin.py:276
+#: ./src/pyams_security/interfaces/plugin.py:305
+#: ./src/pyams_security/interfaces/plugin.py:361
 msgid "Password"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:272
+#: ./src/pyams_security/interfaces/plugin.py:277
 msgid ""
 "Password must be at least 8 characters long, and contain at least three kinds"
 " of characters between lowercase letters, uppercase letters, numbers and "
 "special characters"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:280
-#: ./src/pyams_security/interfaces/plugin.py:304
-#: ./src/pyams_security/interfaces/plugin.py:360
+#: ./src/pyams_security/interfaces/plugin.py:285
+#: ./src/pyams_security/interfaces/plugin.py:309
+#: ./src/pyams_security/interfaces/plugin.py:365
 msgid "Confirmed password"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:287
-#: ./src/pyams_security/interfaces/plugin.py:311
+#: ./src/pyams_security/interfaces/plugin.py:292
+#: ./src/pyams_security/interfaces/plugin.py:316
 msgid "You didn't confirmed your password correctly!"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:294
-#: ./src/pyams_security/interfaces/plugin.py:385
+#: ./src/pyams_security/interfaces/plugin.py:299
+#: ./src/pyams_security/interfaces/plugin.py:390
 msgid "Activation hash"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:330
+#: ./src/pyams_security/interfaces/plugin.py:335
 msgid "User email address"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:337
+#: ./src/pyams_security/interfaces/plugin.py:342
 msgid "Given email address is not valid!"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:350
+#: ./src/pyams_security/interfaces/plugin.py:355
 msgid "Password manager name"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:351
+#: ./src/pyams_security/interfaces/plugin.py:356
 msgid "Utility used to encrypt user password"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:364
+#: ./src/pyams_security/interfaces/plugin.py:369
 msgid "Wait confirmation?"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:365
+#: ./src/pyams_security/interfaces/plugin.py:370
 msgid ""
 "If 'no', user will be activated immediately without waiting email "
 "confirmation"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:374
+#: ./src/pyams_security/interfaces/plugin.py:379
 msgid "You can't activate an account without setting a password!"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:376
+#: ./src/pyams_security/interfaces/plugin.py:381
 msgid "Self-registered profile?"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:381
+#: ./src/pyams_security/interfaces/plugin.py:386
 msgid "Activation secret key"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:382
+#: ./src/pyams_security/interfaces/plugin.py:387
 msgid "This private secret is used to create and check activation hash"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:386
+#: ./src/pyams_security/interfaces/plugin.py:391
 msgid ""
 "This hash is provided into activation message URL. Activation hash is missing"
 " for local users which were registered without waiting their confirmation."
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:391
+#: ./src/pyams_security/interfaces/plugin.py:396
 msgid "Activated"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:395
+#: ./src/pyams_security/interfaces/plugin.py:400
 msgid "Activation date"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:398
+#: ./src/pyams_security/interfaces/plugin.py:403
 msgid "Password reset hash"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:399
+#: ./src/pyams_security/interfaces/plugin.py:404
 msgid ""
 "This hash is provided when a user is asking for a password reset; please note"
 " that password reset request should not update password..."
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:404
+#: ./src/pyams_security/interfaces/plugin.py:409
 msgid "Password reset hash date"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:433
+#: ./src/pyams_security/interfaces/plugin.py:438
 msgid "Groups folder plug-in"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:450
+#: ./src/pyams_security/interfaces/plugin.py:455
 msgid "Group ID"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:451
+#: ./src/pyams_security/interfaces/plugin.py:456
 msgid "This ID should be unique between all groups"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:455
+#: ./src/pyams_security/interfaces/plugin.py:460
 msgid "Title"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:456
+#: ./src/pyams_security/interfaces/plugin.py:461
 msgid "Public label of this group"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:459
+#: ./src/pyams_security/interfaces/plugin.py:464
 msgid "Description"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:462
+#: ./src/pyams_security/interfaces/plugin.py:467
 msgid "Group principals"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/plugin.py:463
+#: ./src/pyams_security/interfaces/plugin.py:468
 msgid "IDs of principals contained in this group"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/rest.py:37
 msgid "Check request origin"
 msgstr ""
 
@@ -385,33 +295,14 @@
 msgid "Allowed origins"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/rest.py:45
 msgid "List of allowed origins URLs using CORS requests"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/site.py:31
-msgid "Site managers"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/site.py:32
-msgid ""
-"These principals are allowed to manage the whole application environment"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/site.py:37
-msgid "Site viewers"
-msgstr ""
-
-#: ./src/pyams_security/interfaces/site.py:38
-msgid ""
-"These principals are allowed to view some application settings, without "
-"update"
-msgstr ""
-
 #: ./src/pyams_security/interfaces/profile.py:34
 msgid "Profile's avatar"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/profile.py:35
 msgid "This picture will be associated to your user profile"
 msgstr ""
@@ -441,133 +332,240 @@
 msgid "Directory plug-ins"
 msgstr ""
 
 #: ./src/pyams_security/interfaces/__init__.py:102
 msgid "The plug-in can be used to extract principals information"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:135
+#: ./src/pyams_security/interfaces/__init__.py:147
 msgid "Access menu from home"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:136
+#: ./src/pyams_security/interfaces/__init__.py:148
 msgid ""
 "If 'yes', a menu will be displayed to get access to security manager from "
 "site admin home page"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:157
+#: ./src/pyams_security/interfaces/__init__.py:191
 msgid "Inherit parent security?"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:158
+#: ./src/pyams_security/interfaces/__init__.py:192
 msgid "Get access control entries (ACE) inherited from parent levels"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:163
+#: ./src/pyams_security/interfaces/__init__.py:197
 msgid "Public denied permissions"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:164
+#: ./src/pyams_security/interfaces/__init__.py:198
 msgid ""
 "These permissions will be denied to all users. Denied permissions take "
 "precedence over granted ones."
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:169
+#: ./src/pyams_security/interfaces/__init__.py:203
 msgid "Public granted permissions"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:170
+#: ./src/pyams_security/interfaces/__init__.py:204
 msgid "These permissions will be granted to all users"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:174
+#: ./src/pyams_security/interfaces/__init__.py:208
 msgid "Authenticated denied permissions"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:175
+#: ./src/pyams_security/interfaces/__init__.py:209
 msgid ""
 "These permissions will be denied to authenticated users. Denied permissions "
 "take precedence over granted ones."
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:181
+#: ./src/pyams_security/interfaces/__init__.py:215
 msgid "Authenticated granted permissions"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:182
+#: ./src/pyams_security/interfaces/__init__.py:216
 msgid "These permissions will be granted to authenticated users"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:186
+#: ./src/pyams_security/interfaces/__init__.py:220
 msgid "Inherit parent roles?"
 msgstr ""
 
-#: ./src/pyams_security/interfaces/__init__.py:187
+#: ./src/pyams_security/interfaces/__init__.py:221
 msgid "Get roles granted on parent levels"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:197
+#: ./src/pyams_security/interfaces/site.py:31
+msgid "Site managers"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/site.py:32
+msgid ""
+"These principals are allowed to manage the whole application environment"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/site.py:37
+msgid "Site viewers"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/site.py:38
+msgid ""
+"These principals are allowed to view some application settings, without "
+"update"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:34
+msgid "Enable notifications?"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:35
+msgid "If 'no', mail notifications will be disabled"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:39
+msgid "Mailer utility"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:40
+msgid "Mail delivery utility used to send notifications"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:48
+msgid "Notifications can't be enabled without mailer utility"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:53
+msgid "Service name"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:54
+msgid "Name of service as defined in registration mail subject"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:58
+msgid "Service owner"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:59
+msgid ""
+"Name of the entity providing this service, which will be visible in "
+"notifications messages"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:63
+msgid "Sender name"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:64
+msgid "Visible name of registration mail sender"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:67
+msgid "Sender email"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:68
+msgid "Email address of registration mail sender"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:71
+msgid "Subject prefix"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:72
+msgid ""
+"This prefix will be inserted into subject prefix of each notification message"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:77
+msgid "Confirmation template"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:78
+#, python-format
+msgid ""
+"This template will be used instead of default template to send notification "
+"when a user is registered by a system administrator; you can use some user "
+"properties into the message body, like: {login}, {email}, {firstname}, "
+"{lastname}, {title} or {company_name}; message activation link and footer are"
+" added automatically"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:86
+msgid "Registration template"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:87
+#, python-format
+msgid ""
+"This template will be used instead of default template to send notificaiton "
+"when a user is auto-registered; you can use some user properties into the "
+"message body, like: {login}, {email}, {firstname}, {lastname}, {title} or "
+"{company_name}; message activation link and footer are added automatically"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:94
+msgid "Email signature"
+msgstr ""
+
+#: ./src/pyams_security/interfaces/notification.py:95
+msgid "Text displayed in email footer"
+msgstr ""
+
+#: ./src/pyams_security/plugin/userfolder.py:216
 #, python-format
 msgid "{prefix}{subject}"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:245
+#: ./src/pyams_security/plugin/userfolder.py:265
+#: ./src/pyams_security/plugin/userfolder.py:269
 msgid "Please confirm registration"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:256
+#: ./src/pyams_security/plugin/userfolder.py:280
 msgid "Password reset"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:348
-#: ./src/pyams_security/plugin/userfolder.py:353
+#: ./src/pyams_security/plugin/userfolder.py:371
+#: ./src/pyams_security/plugin/userfolder.py:376
 msgid "Can't activate profile with given params!"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:371
+#: ./src/pyams_security/plugin/userfolder.py:394
 msgid "Invalid reset request!"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:373
+#: ./src/pyams_security/plugin/userfolder.py:396
 msgid "Can't reset password with given params!"
 msgstr ""
 
-#: ./src/pyams_security/plugin/userfolder.py:376
+#: ./src/pyams_security/plugin/userfolder.py:399
 msgid "Your password reset hash is no longer valid!"
 msgstr ""
 
-#: ./src/pyams_security/plugin/templates/register-info.pt:2
+#: ./src/pyams_security/plugin/templates/password-reset.pt:7
+msgid "${header} Password reset"
+msgstr ""
+
 #: ./src/pyams_security/plugin/templates/password-reset.pt:11
 #: ./src/pyams_security/plugin/templates/register-message.pt:2
+#: ./src/pyams_security/plugin/templates/register-info.pt:2
 msgid "Hello,"
 msgstr ""
 
-#: ./src/pyams_security/plugin/templates/register-info.pt:3
 #: ./src/pyams_security/plugin/templates/password-reset.pt:12
 #: ./src/pyams_security/plugin/templates/register-message.pt:3
+#: ./src/pyams_security/plugin/templates/register-info.pt:3
 msgid "${service_name} is a service provided by ${service_owner}."
 msgstr ""
 
-#: ./src/pyams_security/plugin/templates/register-info.pt:5
-msgid ""
-"A new account has been created for your email address, that you may confirm "
-"before being able to use the service."
-msgstr ""
-
-#: ./src/pyams_security/plugin/templates/register-info.pt:7
-#: ./src/pyams_security/plugin/templates/register-body.pt:12
-msgid "The login that was given to your account is: ${login}."
-msgstr ""
-
-#: ./src/pyams_security/plugin/templates/password-reset.pt:7
-msgid "${header} Password reset"
-msgstr ""
-
 #: ./src/pyams_security/plugin/templates/password-reset.pt:14
 msgid "A password reset has been requested for your account: ${login}."
 msgstr ""
 
 #: ./src/pyams_security/plugin/templates/password-reset.pt:15
 msgid ""
 "If you want to confirm this action, please click on the following link, re-"
@@ -581,28 +579,39 @@
 msgstr ""
 
 #: ./src/pyams_security/plugin/templates/password-reset.pt:22
 #: ./src/pyams_security/plugin/templates/register-body.pt:20
 msgid "Thank you for using our services."
 msgstr ""
 
-#: ./src/pyams_security/plugin/templates/register-message.pt:5
-msgid ""
-"You have registered a new account that you may confirm before being able to "
-"use the service."
-msgstr ""
-
 #: ./src/pyams_security/plugin/templates/register-body.pt:7
 msgid "${header} Registration notice"
 msgstr ""
 
+#: ./src/pyams_security/plugin/templates/register-body.pt:12
+#: ./src/pyams_security/plugin/templates/register-info.pt:7
+msgid "The login that was given to your account is: ${login}."
+msgstr ""
+
 #: ./src/pyams_security/plugin/templates/register-body.pt:13
 msgid ""
 "To confirm your registration, please click on the following link, re-enter "
 "your login and set a new password:"
 msgstr ""
 
 #: ./src/pyams_security/plugin/templates/register-body.pt:18
 msgid ""
 "If you don't want to confirm this registration, please just ignore this "
 "message and your registration information will be deleted within 30 days."
 msgstr ""
+
+#: ./src/pyams_security/plugin/templates/register-message.pt:5
+msgid ""
+"You have registered a new account that you may confirm before being able to "
+"use the service."
+msgstr ""
+
+#: ./src/pyams_security/plugin/templates/register-info.pt:5
+msgid ""
+"A new account has been created for your email address, that you may confirm "
+"before being able to use the service."
+msgstr ""
```

### Comparing `pyams_security-2.3.0/src/pyams_security/notification.py` & `pyams_security-2.3.1/src/pyams_security/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/password.py` & `pyams_security-2.3.1/src/pyams_security/password.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/permission.py` & `pyams_security-2.3.1/src/pyams_security/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/__init__.py` & `pyams_security-2.3.1/src/pyams_security/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/admin.py` & `pyams_security-2.3.1/src/pyams_security/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/group.py` & `pyams_security-2.3.1/src/pyams_security/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/templates/password-reset.pt` & `pyams_security-2.3.1/src/pyams_security/plugin/templates/password-reset.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/templates/register-body.pt` & `pyams_security-2.3.1/src/pyams_security/plugin/templates/register-body.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/templates/register-info.pt` & `pyams_security-2.3.1/src/pyams_security/plugin/templates/register-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/plugin/userfolder.py` & `pyams_security-2.3.1/src/pyams_security/plugin/userfolder.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/policy.py` & `pyams_security-2.3.1/src/pyams_security/policy.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/principal.py` & `pyams_security-2.3.1/src/pyams_security/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/profile.py` & `pyams_security-2.3.1/src/pyams_security/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/property.py` & `pyams_security-2.3.1/src/pyams_security/property.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/rest.py` & `pyams_security-2.3.1/src/pyams_security/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/role.py` & `pyams_security-2.3.1/src/pyams_security/role.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/schema.py` & `pyams_security-2.3.1/src/pyams_security/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/security.py` & `pyams_security-2.3.1/src/pyams_security/security.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/site.py` & `pyams_security-2.3.1/src/pyams_security/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/tests/__init__.py` & `pyams_security-2.3.1/src/pyams_security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocs.py` & `pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocstrings.py` & `pyams_security-2.3.1/src/pyams_security/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/utility.py` & `pyams_security-2.3.1/src/pyams_security/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security/vocabulary.py` & `pyams_security-2.3.1/src/pyams_security/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.3.0/src/pyams_security.egg-info/PKG-INFO` & `pyams_security-2.3.1/src/pyams_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security
-Version: 2.3.0
+Version: 2.3.1
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.1
+-----
+ - updated translations
+
 2.3.0
 -----
  - allow case-insensitive local user login
 
 2.2.1
 -----
  - added support for custom attributes in roles
```

### Comparing `pyams_security-2.3.0/src/pyams_security.egg-info/SOURCES.txt` & `pyams_security-2.3.1/src/pyams_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

