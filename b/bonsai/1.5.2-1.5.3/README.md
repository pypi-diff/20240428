# Comparing `tmp/bonsai-1.5.2.tar.gz` & `tmp/bonsai-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai-1.5.2.tar", last modified: Mon Nov 20 19:25:22 2023, max compression
+gzip compressed data, was "bonsai-1.5.3.tar", last modified: Sun Apr 28 08:47:51 2024, max compression
```

## Comparing `bonsai-1.5.2.tar` & `bonsai-1.5.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.535933 bonsai-1.5.2/
--rw-r--r--   0 noirello  (1000) noirello  (1000)    16562 2023-11-20 19:24:18.000000 bonsai-1.5.2/CHANGELOG.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1077 2023-11-20 19:24:18.000000 bonsai-1.5.2/LICENSE
--rw-r--r--   0 noirello  (1000) noirello  (1000)      234 2022-02-26 11:03:09.000000 bonsai-1.5.2/MANIFEST.in
--rw-r--r--   0 noirello  (1000) noirello  (1000)     5177 2023-11-20 19:25:22.535933 bonsai-1.5.2/PKG-INFO
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3607 2023-11-20 19:24:18.000000 bonsai-1.5.2/README.rst
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.535933 bonsai-1.5.2/bonsai.egg-info/
--rw-r--r--   0 noirello  (1000) noirello  (1000)     5177 2023-11-20 19:25:22.000000 bonsai-1.5.2/bonsai.egg-info/PKG-INFO
--rwxrwxrwx   0 noirello  (1000) noirello  (1000)     2015 2023-11-20 19:25:22.000000 bonsai-1.5.2/bonsai.egg-info/SOURCES.txt
--rwxrwxrwx   0 noirello  (1000) noirello  (1000)        1 2023-11-20 19:25:22.000000 bonsai-1.5.2/bonsai.egg-info/dependency_links.txt
--rwxrwxrwx   0 noirello  (1000) noirello  (1000)      123 2023-11-20 19:25:22.000000 bonsai-1.5.2/bonsai.egg-info/requires.txt
--rwxrwxrwx   0 noirello  (1000) noirello  (1000)        7 2023-11-20 19:25:22.000000 bonsai-1.5.2/bonsai.egg-info/top_level.txt
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.125933 bonsai-1.5.2/docs/
--rw-r--r--   0 noirello  (1000) noirello  (1000)     6762 2022-02-26 11:03:09.000000 bonsai-1.5.2/docs/Makefile
--rw-r--r--   0 noirello  (1000) noirello  (1000)    31572 2022-12-03 10:48:47.000000 bonsai-1.5.2/docs/advanced.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)    31599 2022-08-24 13:11:05.000000 bonsai-1.5.2/docs/api.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)       43 2022-02-26 11:03:09.000000 bonsai-1.5.2/docs/changelog.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)     9161 2023-11-20 19:24:18.000000 bonsai-1.5.2/docs/conf.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1393 2022-08-24 13:11:05.000000 bonsai-1.5.2/docs/index.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2660 2023-11-20 19:24:18.000000 bonsai-1.5.2/docs/install.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)     6701 2022-02-26 11:03:09.000000 bonsai-1.5.2/docs/make.bat
--rw-r--r--   0 noirello  (1000) noirello  (1000)     8138 2023-11-20 19:24:18.000000 bonsai-1.5.2/docs/tutorial.rst
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1222 2023-11-20 19:24:18.000000 bonsai-1.5.2/pyproject.toml
--rw-r--r--   0 noirello  (1000) noirello  (1000)      121 2023-11-20 19:25:22.545933 bonsai-1.5.2/setup.cfg
--rw-r--r--   0 noirello  (1000) noirello  (1000)     6107 2023-11-20 19:24:18.000000 bonsai-1.5.2/setup.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.065933 bonsai-1.5.2/src/
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.265933 bonsai-1.5.2/src/_bonsai/
--rw-r--r--   0 noirello  (1000) noirello  (1000)     5545 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/bonsaimodule.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)    27112 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/_bonsai/ldap-xplat.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2514 2022-08-24 13:11:05.000000 bonsai-1.5.2/src/_bonsai/ldap-xplat.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)    48723 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/_bonsai/ldapconnection.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)      629 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapconnection.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)    22044 2023-11-20 19:24:18.000000 bonsai-1.5.2/src/_bonsai/ldapconnectiter.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)      961 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapconnectiter.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)    31919 2022-12-25 01:19:41.000000 bonsai-1.5.2/src/_bonsai/ldapentry.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)      842 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapentry.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)     6729 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapmodlist.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)      592 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapmodlist.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7729 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/_bonsai/ldapsearchiter.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)      488 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/ldapsearchiter.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)    20234 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/utils.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2257 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/utils.h
--rw-r--r--   0 noirello  (1000) noirello  (1000)    40813 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/_bonsai/wldap-utf8.c
--rw-r--r--   0 noirello  (1000) noirello  (1000)     8078 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/_bonsai/wldap-utf8.h
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.335933 bonsai-1.5.2/src/bonsai/
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1596 2023-11-20 19:24:18.000000 bonsai-1.5.2/src/bonsai/__init__.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.355933 bonsai-1.5.2/src/bonsai/active_directory/
--rw-r--r--   0 noirello  (1000) noirello  (1000)    12680 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/active_directory/__init__.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    19767 2022-08-24 13:11:05.000000 bonsai-1.5.2/src/bonsai/active_directory/acl.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7088 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/active_directory/sid.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.365933 bonsai-1.5.2/src/bonsai/asyncio/
--rw-r--r--   0 noirello  (1000) noirello  (1000)      139 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/asyncio/__init__.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3351 2022-08-24 13:11:05.000000 bonsai-1.5.2/src/bonsai/asyncio/aioconnection.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3318 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/asyncio/aiopool.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7611 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/bonsai/errors.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.375933 bonsai-1.5.2/src/bonsai/gevent/
--rw-r--r--   0 noirello  (1000) noirello  (1000)       87 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/gevent/__init__.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1626 2022-02-26 11:03:09.000000 bonsai-1.5.2/src/bonsai/gevent/geventconnection.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    26531 2023-11-20 19:24:18.000000 bonsai-1.5.2/src/bonsai/ldapclient.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    13689 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldapconnection.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     4829 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldapdn.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    10341 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldapentry.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1383 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/bonsai/ldapreference.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     9186 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldapurl.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7555 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldapvaluelist.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    13328 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/ldif.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7988 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/pool.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)        0 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/py.typed
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.385933 bonsai-1.5.2/src/bonsai/tornado/
--rw-r--r--   0 noirello  (1000) noirello  (1000)       90 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/tornado/__init__.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3517 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/bonsai/tornado/tornadoconnection.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.405933 bonsai-1.5.2/src/bonsai/trio/
--rw-r--r--   0 noirello  (1000) noirello  (1000)       81 2022-12-03 10:48:47.000000 bonsai-1.5.2/src/bonsai/trio/__init__.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2694 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/bonsai/trio/trioconnection.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1323 2022-03-12 11:50:15.000000 bonsai-1.5.2/src/bonsai/utils.py
-drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2023-11-20 19:25:22.535933 bonsai-1.5.2/tests/
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1723 2022-08-24 13:11:05.000000 bonsai-1.5.2/tests/conftest.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)      668 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test.ini
--rw-r--r--   0 noirello  (1000) noirello  (1000)     9039 2022-08-24 13:11:05.000000 bonsai-1.5.2/tests/test_ad_acl.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    11321 2022-08-24 13:11:05.000000 bonsai-1.5.2/tests/test_ad_securitydescriptor.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3801 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ad_sid.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1025 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_ad_useraccountcontrol.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     8760 2022-12-03 10:48:47.000000 bonsai-1.5.2/tests/test_asyncio.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     5129 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_gevent.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    10745 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ldapclient.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    28996 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ldapconnection.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2584 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_ldapdn.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)    18458 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ldapentry.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     2913 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ldapreference.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3937 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_ldapurl.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     3312 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_ldapvaluelist.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     9256 2022-12-03 10:48:47.000000 bonsai-1.5.2/tests/test_ldifreader.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     4085 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_ldifwriter.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     5001 2022-08-24 13:11:05.000000 bonsai-1.5.2/tests/test_pool.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     8677 2022-08-24 13:11:05.000000 bonsai-1.5.2/tests/test_tornado.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     7218 2022-03-12 11:50:15.000000 bonsai-1.5.2/tests/test_trio.py
--rw-r--r--   0 noirello  (1000) noirello  (1000)     1077 2022-02-26 11:03:09.000000 bonsai-1.5.2/tests/test_utils.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.529855 bonsai-1.5.3/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    17120 2024-04-28 08:10:11.000000 bonsai-1.5.3/CHANGELOG.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1077 2024-04-28 08:04:21.000000 bonsai-1.5.3/LICENSE
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      234 2022-02-26 11:03:09.000000 bonsai-1.5.3/MANIFEST.in
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     5851 2024-04-28 08:47:51.529855 bonsai-1.5.3/PKG-INFO
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3607 2023-11-20 19:24:18.000000 bonsai-1.5.3/README.rst
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.359856 bonsai-1.5.3/bonsai.egg-info/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     5851 2024-04-28 08:47:44.000000 bonsai-1.5.3/bonsai.egg-info/PKG-INFO
+-rwxrwxrwx   0 noirello  (1000) noirello  (1000)     2015 2024-04-28 08:47:44.000000 bonsai-1.5.3/bonsai.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noirello  (1000) noirello  (1000)        1 2024-04-28 08:47:44.000000 bonsai-1.5.3/bonsai.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noirello  (1000) noirello  (1000)      123 2024-04-28 08:47:44.000000 bonsai-1.5.3/bonsai.egg-info/requires.txt
+-rwxrwxrwx   0 noirello  (1000) noirello  (1000)        7 2024-04-28 08:47:44.000000 bonsai-1.5.3/bonsai.egg-info/top_level.txt
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.419855 bonsai-1.5.3/docs/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     6762 2022-02-26 11:03:09.000000 bonsai-1.5.3/docs/Makefile
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    31572 2022-12-03 10:48:47.000000 bonsai-1.5.3/docs/advanced.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    31745 2024-01-20 13:29:37.000000 bonsai-1.5.3/docs/api.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)       43 2022-02-26 11:03:09.000000 bonsai-1.5.3/docs/changelog.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     9161 2024-04-28 08:04:54.000000 bonsai-1.5.3/docs/conf.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1393 2022-08-24 13:11:05.000000 bonsai-1.5.3/docs/index.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2660 2023-11-20 19:24:18.000000 bonsai-1.5.3/docs/install.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     6701 2022-02-26 11:03:09.000000 bonsai-1.5.3/docs/make.bat
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     8138 2023-11-20 19:24:18.000000 bonsai-1.5.3/docs/tutorial.rst
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1222 2024-04-28 08:06:26.000000 bonsai-1.5.3/pyproject.toml
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      121 2024-04-28 08:47:51.529855 bonsai-1.5.3/setup.cfg
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     6107 2023-11-20 19:24:18.000000 bonsai-1.5.3/setup.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.349856 bonsai-1.5.3/src/
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.439855 bonsai-1.5.3/src/_bonsai/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     5545 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/bonsaimodule.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    27266 2024-01-20 13:29:27.000000 bonsai-1.5.3/src/_bonsai/ldap-xplat.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2514 2022-08-24 13:11:05.000000 bonsai-1.5.3/src/_bonsai/ldap-xplat.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    49224 2024-01-20 13:29:37.000000 bonsai-1.5.3/src/_bonsai/ldapconnection.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      629 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapconnection.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    22044 2023-11-20 19:24:18.000000 bonsai-1.5.3/src/_bonsai/ldapconnectiter.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      961 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapconnectiter.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    31919 2022-12-25 01:19:41.000000 bonsai-1.5.3/src/_bonsai/ldapentry.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      842 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapentry.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     6729 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapmodlist.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      592 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapmodlist.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     7729 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/_bonsai/ldapsearchiter.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      488 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/ldapsearchiter.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    20234 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/utils.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2257 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/utils.h
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    40813 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/_bonsai/wldap-utf8.c
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     8078 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/_bonsai/wldap-utf8.h
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.459855 bonsai-1.5.3/src/bonsai/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1596 2024-04-28 08:05:09.000000 bonsai-1.5.3/src/bonsai/__init__.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.469855 bonsai-1.5.3/src/bonsai/active_directory/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    12680 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/active_directory/__init__.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    19767 2022-08-24 13:11:05.000000 bonsai-1.5.3/src/bonsai/active_directory/acl.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     7088 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/active_directory/sid.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.469855 bonsai-1.5.3/src/bonsai/asyncio/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      139 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/asyncio/__init__.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3351 2022-08-24 13:11:05.000000 bonsai-1.5.3/src/bonsai/asyncio/aioconnection.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3318 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/asyncio/aiopool.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     7611 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/bonsai/errors.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.469855 bonsai-1.5.3/src/bonsai/gevent/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)       87 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/gevent/__init__.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1626 2022-02-26 11:03:09.000000 bonsai-1.5.3/src/bonsai/gevent/geventconnection.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    26531 2023-11-20 19:24:18.000000 bonsai-1.5.3/src/bonsai/ldapclient.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    13689 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldapconnection.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     4829 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldapdn.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    10341 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldapentry.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1383 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/bonsai/ldapreference.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     9186 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldapurl.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     7555 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldapvaluelist.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    13328 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/ldif.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     8426 2024-01-20 13:29:37.000000 bonsai-1.5.3/src/bonsai/pool.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)        0 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/py.typed
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.469855 bonsai-1.5.3/src/bonsai/tornado/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)       90 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/tornado/__init__.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3517 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/bonsai/tornado/tornadoconnection.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.469855 bonsai-1.5.3/src/bonsai/trio/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)       81 2022-12-03 10:48:47.000000 bonsai-1.5.3/src/bonsai/trio/__init__.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2694 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/bonsai/trio/trioconnection.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1323 2022-03-12 11:50:15.000000 bonsai-1.5.3/src/bonsai/utils.py
+drwxr-xr-x   0 noirello  (1000) noirello  (1000)        0 2024-04-28 08:47:51.529855 bonsai-1.5.3/tests/
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1723 2022-08-24 13:11:05.000000 bonsai-1.5.3/tests/conftest.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)      668 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test.ini
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     9039 2022-08-24 13:11:05.000000 bonsai-1.5.3/tests/test_ad_acl.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    11321 2022-08-24 13:11:05.000000 bonsai-1.5.3/tests/test_ad_securitydescriptor.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3801 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_ad_sid.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1025 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_ad_useraccountcontrol.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     8760 2022-12-03 10:48:47.000000 bonsai-1.5.3/tests/test_asyncio.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     5129 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_gevent.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    10745 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_ldapclient.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    29387 2024-01-20 13:29:37.000000 bonsai-1.5.3/tests/test_ldapconnection.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2584 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_ldapdn.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)    18458 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_ldapentry.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     2913 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_ldapreference.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3937 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_ldapurl.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     3312 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_ldapvaluelist.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     9256 2022-12-03 10:48:47.000000 bonsai-1.5.3/tests/test_ldifreader.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     4085 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_ldifwriter.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     5001 2022-08-24 13:11:05.000000 bonsai-1.5.3/tests/test_pool.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     8677 2022-08-24 13:11:05.000000 bonsai-1.5.3/tests/test_tornado.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     7218 2022-03-12 11:50:15.000000 bonsai-1.5.3/tests/test_trio.py
+-rw-r--r--   0 noirello  (1000) noirello  (1000)     1077 2022-02-26 11:03:09.000000 bonsai-1.5.3/tests/test_utils.py
```

### Comparing `bonsai-1.5.2/CHANGELOG.rst` & `bonsai-1.5.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 Changelog
 ==========
 
+[1.5.3 - 2024-04-28]
+--------------------
+
+Changed
+~~~~~~~
+
+-  Any exception that rasied during closing a connection pool is 
+   catched and a warning message will be logged.
+-  LDAPconnection.close method is no longer try to abandon on-going
+   requests by default.
+
+Added
+~~~~~
+
+-  New `abandon_requests` parameter for LDAPconnection.close method
+   to call abandon operations on on-going requests during connection
+   close.
+-  Arm64 wheels for macOS.
+
+Fixed
+~~~~~
+
+-  Memory leak during Kerberos credential creation. (PR #84, thanks
+   to @dafanasiev)
+
+
 [1.5.2] - 2023-11-20
 --------------------
 
 Changed
 ~~~~~~~
 
 -  The module is no longer tested with 3.7.
```

### Comparing `bonsai-1.5.2/LICENSE` & `bonsai-1.5.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 [fullname]
+Copyright (c) 2024 [fullname]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bonsai-1.5.2/README.rst` & `bonsai-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/bonsai.egg-info/SOURCES.txt` & `bonsai-1.5.3/bonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/Makefile` & `bonsai-1.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/advanced.rst` & `bonsai-1.5.3/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/api.rst` & `bonsai-1.5.3/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -135,18 +135,21 @@
     means the operation could be performed anyway. Nevertheless, it is a good programming paradigm
     to abandon unwanted operations (e.g after a timeout is exceeded).
 
     :param int msg_id: the ID of an ongoing LDAP operation.
 
 .. automethod:: LDAPConnection.add(entry, timeout=None)
 
-.. method:: LDAPConnection.close()
+.. method:: LDAPConnection.close(abandon_requests=False)
 
     Close LDAP connection.
-    
+
+    When `abandon_requests` parameter is set to `true`, then abandon operation will be called on
+    every unfinished request.
+
 .. automethod:: LDAPConnection.delete(dname, timeout=None, recursive=False)
 
 .. method:: LDAPConnection.fileno()
 
     Return the file descriptor of the underlying socket that is used for the LDAP connection.
 
     :return: The file descriptor.
```

### Comparing `bonsai-1.5.2/docs/conf.py` & `bonsai-1.5.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'bonsai'
-copyright = '2014-2023, noirello'
+copyright = '2014-2024, noirello'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = bonsai.__version__
```

### Comparing `bonsai-1.5.2/docs/index.rst` & `bonsai-1.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/install.rst` & `bonsai-1.5.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/make.bat` & `bonsai-1.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/docs/tutorial.rst` & `bonsai-1.5.3/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/pyproject.toml` & `bonsai-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bonsai"
-version = "1.5.2"
+version = "1.5.3"
 description = "Python 3 module for accessing LDAP directory servers."
 authors = ["noirello <noirello@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 gevent = { version = "^23.9.0", optional = true }
```

### Comparing `bonsai-1.5.2/setup.py` & `bonsai-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/bonsaimodule.c` & `bonsai-1.5.3/src/_bonsai/bonsaimodule.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldap-xplat.c` & `bonsai-1.5.3/src/_bonsai/ldap-xplat.c`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
                  char **errmsg) {
     int rc = 0, len = 0;
     unsigned int minor_stat = 0, major_stat = 0;
     const char *errmsg_tmp = NULL;
     const char *cctype = NULL;
     char *cname = NULL;
     krb5_ccache defcc = NULL;
+    int credsInitialized = 0;
     krb5_creds creds;
     krb5_principal princ = NULL;
     krb5_keytab keytab = NULL;
     gss_key_value_element_desc elems[2];
     gss_key_value_set_desc store;
     gss_name_t sname = NULL;
     gss_buffer_desc pr_name;
@@ -209,14 +210,15 @@
     rc = krb5_cc_initialize(ctx, *ccache, princ);
     if (rc != 0) goto end;
 
     if (password != NULL && strlen(password) > 0) {
         rc = krb5_get_init_creds_password(ctx, &creds, princ, password,
                                           0, NULL, 0, NULL, NULL);
         if (rc != 0) goto end;
+        credsInitialized = 1;
 
         rc = krb5_cc_store_cred(ctx, *ccache, &creds);
         if (rc != 0) goto end;
 
         rc = krb5_cc_get_full_name(ctx, *ccache, &cname);
         if (rc != 0) goto end;
         
@@ -225,14 +227,15 @@
         store.count++;
     } else if (ktname != NULL && strlen(ktname) > 0) {
         rc = krb5_kt_resolve(ctx, ktname, &keytab);
         if (rc != 0) goto end;
 
         rc = krb5_get_init_creds_keytab(ctx, &creds, princ, keytab, 0, NULL, NULL);
         if (rc != 0) goto end;
+        credsInitialized = 1;
         
         rc = krb5_cc_store_cred(ctx, *ccache, &creds);
         if (rc != 0) goto end;
 
         rc = krb5_cc_get_full_name(ctx, *ccache, &cname);
         if (rc != 0) goto end;
 
@@ -258,14 +261,15 @@
     major_stat = gss_acquire_cred_from(&minor_stat, sname, 0, GSS_C_NO_OID_SET,
                                        GSS_C_INITIATE, &store, gsscred,
                                        NULL, NULL);
 
 end:
     if (keytab != NULL) krb5_kt_close(ctx, keytab);
     if (princ != NULL) krb5_free_principal(ctx, princ);
+    if (credsInitialized) krb5_free_cred_contents(ctx, &creds);
     if (defcc != NULL) krb5_cc_close(ctx, defcc);
     if (cname != NULL) free(cname);
     if (pr_name.value != NULL) krb5_free_unparsed_name(ctx, pr_name.value);
     if (sname != NULL) {
         major_stat = gss_release_name(&minor_stat, &sname);
     }
```

### Comparing `bonsai-1.5.2/src/_bonsai/ldap-xplat.h` & `bonsai-1.5.3/src/_bonsai/ldap-xplat.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapconnection.c` & `bonsai-1.5.3/src/_bonsai/ldapconnection.c`

 * *Files 0% similar despite different names*

```diff
@@ -189,55 +189,68 @@
     }
 
     return PyLong_FromLong((long int)(self->csock));
 }
 
 /*  Close the LDAP connection. */
 static PyObject *
-ldapconnection_close(LDAPConnection *self) {
+ldapconnection_close(LDAPConnection *self, PyObject *args, PyObject *kwds) {
     int rc;
     int msgid;
-    PyObject *keys = PyDict_Keys(self->pending_ops);
-    PyObject *iter, *key;
+    char abandon = 0;
+    PyObject *iter, *key, *keys = NULL;
+    PyObject *abandon_obj = NULL;
+    static char *kwlist[] = {"abandon_requests", NULL};
 
     DEBUG("ldapconnection_close (self:%p)", self);
-    if (keys == NULL) return NULL;
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "|O!", kwlist, &PyBool_Type,
+            &abandon_obj)) {
+        return NULL;
+    }
+
+    if (abandon_obj != NULL) {
+        abandon = (char)PyObject_IsTrue(abandon_obj);
+    }
 
     if (self->closed == 1) {
         /* Connection is already close, nothing to do. */
-        Py_DECREF(keys);
         Py_RETURN_NONE;
     }
 
-    iter = PyObject_GetIter(keys);
-    Py_DECREF(keys);
-    if (iter == NULL) return NULL;
-
-    for (key = PyIter_Next(iter); key != NULL; key = PyIter_Next(iter)) {
-        msgid = (int)PyLong_AsLong(key);
-        /* Remove item from the dict. */
-        if (PyDict_DelItem(self->pending_ops, key) != 0) {
-            Py_DECREF(iter);
+    if (abandon == 1) {
+        keys = PyDict_Keys(self->pending_ops);
+        if (keys == NULL) return NULL;
+
+        iter = PyObject_GetIter(keys);
+        Py_DECREF(keys);
+        if (iter == NULL) return NULL;
+
+        for (key = PyIter_Next(iter); key != NULL; key = PyIter_Next(iter)) {
+            msgid = (int)PyLong_AsLong(key);
+            /* Remove item from the dict. */
+            if (PyDict_DelItem(self->pending_ops, key) != 0) {
+                Py_DECREF(iter);
+                Py_DECREF(key);
+                PyErr_BadInternalCall();
+                return NULL;
+            }
             Py_DECREF(key);
-            PyErr_BadInternalCall();
-            return NULL;
-        }
-        Py_DECREF(key);
 
-        /* Skip negatives, cause assertion error. */
-        if (msgid <= 0) continue;
-        /* Abandon the pending operations from the server. */
-        rc = ldap_abandon_ext(self->ld, msgid, NULL, NULL);
-        if (rc != LDAP_SUCCESS) {
-            Py_DECREF(iter);
-            set_exception(self->ld, rc);
-            return NULL;
+            /* Skip negatives, cause assertion error. */
+            if (msgid <= 0) continue;
+            /* Abandon the pending operations from the server. */
+            rc = ldap_abandon_ext(self->ld, msgid, NULL, NULL);
+            if (rc != LDAP_SUCCESS) {
+                Py_DECREF(iter);
+                set_exception(self->ld, rc);
+                return NULL;
+            }
         }
+        Py_DECREF(iter);
     }
-    Py_DECREF(iter);
 
     rc = ldap_unbind_ext(self->ld, NULL, NULL);
     if (rc != LDAP_SUCCESS) {
         set_exception(self->ld, rc);
         return NULL;
     }
     self->closed = 1;
@@ -1393,15 +1406,15 @@
 };
 
 static PyMethodDef ldapconnection_methods[] = {
     {"abandon", (PyCFunction)ldapconnection_abandon, METH_VARARGS,
             "Abandon ongoing operation associated with the given message id." },
     {"add", (PyCFunction)ldapconnection_add, METH_VARARGS,
             "Add new LDAPEntry to the LDAP server."},
-    {"close", (PyCFunction)ldapconnection_close, METH_NOARGS,
+    {"close", (PyCFunction)ldapconnection_close, METH_VARARGS | METH_KEYWORDS,
             "Close connection with the LDAP Server."},
     {"delete", (PyCFunction)ldapconnection_delentry, METH_VARARGS,
             "Delete an LDAPEntry with the given distinguished name."},
     {"fileno", (PyCFunction)ldapconnection_fileno, METH_NOARGS,
             "Get the socket descriptor that belongs to the connection."},
     {"get_result", (PyCFunction)ldapconnection_result, METH_VARARGS | METH_KEYWORDS,
             "Poll the status of the operation associated with the given message id from LDAP server."},
```

### Comparing `bonsai-1.5.2/src/_bonsai/ldapconnection.h` & `bonsai-1.5.3/src/_bonsai/ldapconnection.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapconnectiter.c` & `bonsai-1.5.3/src/_bonsai/ldapconnectiter.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapconnectiter.h` & `bonsai-1.5.3/src/_bonsai/ldapconnectiter.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapentry.c` & `bonsai-1.5.3/src/_bonsai/ldapentry.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapentry.h` & `bonsai-1.5.3/src/_bonsai/ldapentry.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapmodlist.c` & `bonsai-1.5.3/src/_bonsai/ldapmodlist.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapmodlist.h` & `bonsai-1.5.3/src/_bonsai/ldapmodlist.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/ldapsearchiter.c` & `bonsai-1.5.3/src/_bonsai/ldapsearchiter.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/utils.c` & `bonsai-1.5.3/src/_bonsai/utils.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/utils.h` & `bonsai-1.5.3/src/_bonsai/utils.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/wldap-utf8.c` & `bonsai-1.5.3/src/_bonsai/wldap-utf8.c`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/_bonsai/wldap-utf8.h` & `bonsai-1.5.3/src/_bonsai/wldap-utf8.h`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/__init__.py` & `bonsai-1.5.3/src/bonsai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .ldapclient import LDAPClient
 from .ldapreference import LDAPReference
 from .ldapvaluelist import LDAPValueList
 from .ldif import LDIFError, LDIFReader, LDIFWriter
 from .errors import *
 from .utils import *
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 
 __all__ = [
     "LDAPClient",
     "LDAPConnection",
     "LDAPDN",
     "LDAPEntry",
     "LDAPModOp",
```

### Comparing `bonsai-1.5.2/src/bonsai/active_directory/__init__.py` & `bonsai-1.5.3/src/bonsai/active_directory/__init__.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/active_directory/acl.py` & `bonsai-1.5.3/src/bonsai/active_directory/acl.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/active_directory/sid.py` & `bonsai-1.5.3/src/bonsai/active_directory/sid.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/asyncio/aioconnection.py` & `bonsai-1.5.3/src/bonsai/asyncio/aioconnection.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/asyncio/aiopool.py` & `bonsai-1.5.3/src/bonsai/asyncio/aiopool.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/errors.py` & `bonsai-1.5.3/src/bonsai/errors.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/gevent/geventconnection.py` & `bonsai-1.5.3/src/bonsai/gevent/geventconnection.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapclient.py` & `bonsai-1.5.3/src/bonsai/ldapclient.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapconnection.py` & `bonsai-1.5.3/src/bonsai/ldapconnection.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapdn.py` & `bonsai-1.5.3/src/bonsai/ldapdn.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapentry.py` & `bonsai-1.5.3/src/bonsai/ldapentry.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapreference.py` & `bonsai-1.5.3/src/bonsai/ldapreference.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapurl.py` & `bonsai-1.5.3/src/bonsai/ldapurl.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldapvaluelist.py` & `bonsai-1.5.3/src/bonsai/ldapvaluelist.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/ldif.py` & `bonsai-1.5.3/src/bonsai/ldif.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/pool.py` & `bonsai-1.5.3/src/bonsai/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import logging
 import threading
 from contextlib import contextmanager
 from typing import Optional, Any, Set, Generic, TypeVar, Generator
 
 from .ldapconnection import BaseLDAPConnection, LDAPConnection
 
 MYPY = False
 
 if MYPY:
     from .ldapclient import LDAPClient
 
 
+logger = logging.getLogger("bonsai.pool")
+
+
 class PoolError(Exception):
     """Connection pool related errors."""
 
     pass
 
 
 class ClosedPool(PoolError):
@@ -111,17 +115,27 @@
                 self._idles.add(conn)
         except KeyError:
             raise PoolError("The %r is not managed by this pool." % conn) from None
 
     def close(self) -> None:
         """Close the pool and all of its managed connections."""
         for conn in self._idles:
-            conn.close()
+            try:
+                conn.close()
+            except Exception as exc:
+                logger.warning(
+                    f"Exception is raised during closing idle connection: {exc}"
+                )
         for conn in self._used:
-            conn.close()
+            try:
+                conn.close()
+            except Exception as exc:
+                logger.warning(
+                    f"Exception is raised during closing used connection: {exc}"
+                )
         self._closed = True
         self._idles = set()
         self._used = set()
 
     @contextmanager
     def spawn(self, *args: Any, **kwargs: Any) -> Generator[T, None, None]:
         """
@@ -203,15 +217,15 @@
 
     def __init__(
         self,
         client: "LDAPClient",
         minconn: int = 1,
         maxconn: int = 10,
         block: bool = True,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         """Init method."""
         super().__init__(client, minconn, maxconn, **kwargs)
         self._block = block
         self._lock = threading.Condition()
 
     def get(self, timeout: Optional[float] = None) -> LDAPConnection:
```

### Comparing `bonsai-1.5.2/src/bonsai/tornado/tornadoconnection.py` & `bonsai-1.5.3/src/bonsai/tornado/tornadoconnection.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/trio/trioconnection.py` & `bonsai-1.5.3/src/bonsai/trio/trioconnection.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/src/bonsai/utils.py` & `bonsai-1.5.3/src/bonsai/utils.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/conftest.py` & `bonsai-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test.ini` & `bonsai-1.5.3/tests/test.ini`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ad_acl.py` & `bonsai-1.5.3/tests/test_ad_acl.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ad_securitydescriptor.py` & `bonsai-1.5.3/tests/test_ad_securitydescriptor.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ad_sid.py` & `bonsai-1.5.3/tests/test_ad_sid.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ad_useraccountcontrol.py` & `bonsai-1.5.3/tests/test_ad_useraccountcontrol.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_asyncio.py` & `bonsai-1.5.3/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_gevent.py` & `bonsai-1.5.3/tests/test_gevent.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapclient.py` & `bonsai-1.5.3/tests/test_ldapclient.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapconnection.py` & `bonsai-1.5.3/tests/test_ldapconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,14 +506,27 @@
 
 def test_close(conn):
     """Test close method."""
     conn.close()
     assert conn.closed
     with pytest.raises(bonsai.ClosedConnection):
         _ = conn.whoami()
+    # Can call close multiple times.
+    conn.close()
+    assert conn.closed
+
+
+def test_close_with_abandon(async_conn, basedn):
+    """Test close method with abandon requests option."""
+    msgid = async_conn.open()
+    while async_conn.get_result(msgid) is None:
+        pass
+    msgid = async_conn.search(basedn, 2)
+    async_conn.close(abandon_requests=True)
+    assert async_conn.closed
 
 
 def test_abandon(async_conn, basedn):
     """Test abandon method."""
     msgid = async_conn.open()
     while async_conn.get_result(msgid) is None:
         pass
```

### Comparing `bonsai-1.5.2/tests/test_ldapdn.py` & `bonsai-1.5.3/tests/test_ldapdn.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapentry.py` & `bonsai-1.5.3/tests/test_ldapentry.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapreference.py` & `bonsai-1.5.3/tests/test_ldapreference.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapurl.py` & `bonsai-1.5.3/tests/test_ldapurl.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldapvaluelist.py` & `bonsai-1.5.3/tests/test_ldapvaluelist.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldifreader.py` & `bonsai-1.5.3/tests/test_ldifreader.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_ldifwriter.py` & `bonsai-1.5.3/tests/test_ldifwriter.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_pool.py` & `bonsai-1.5.3/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_tornado.py` & `bonsai-1.5.3/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_trio.py` & `bonsai-1.5.3/tests/test_trio.py`

 * *Files identical despite different names*

### Comparing `bonsai-1.5.2/tests/test_utils.py` & `bonsai-1.5.3/tests/test_utils.py`

 * *Files identical despite different names*

