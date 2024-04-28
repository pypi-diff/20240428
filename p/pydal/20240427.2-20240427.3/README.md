# Comparing `tmp/pydal-20240427.2.tar.gz` & `tmp/pydal-20240427.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydal-20240427.2.tar", last modified: Sat Apr 27 07:19:15 2024, max compression
+gzip compressed data, was "pydal-20240427.3.tar", last modified: Sat Apr 27 08:23:38 2024, max compression
```

## Comparing `pydal-20240427.2.tar` & `pydal-20240427.3.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.949208 pydal-20240427.2/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240427.2/AUTHORS
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240427.2/CHANGES
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240427.2/LICENSE.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240427.2/MANIFEST.in
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:19:15.949208 pydal-20240427.2/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240427.2/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.915874 pydal-20240427.2/docs/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/Makefile
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240427.2/docs/conf.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/index.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/pydal.adapters.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/pydal.helpers.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/requirements.txt
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.922541 pydal-20240427.2/pydal/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-27 07:19:02.000000 pydal-20240427.2/pydal/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240427.2/pydal/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_globals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_load.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.925874 pydal-20240427.2/pydal/adapters/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/adapters/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240427.2/pydal/adapters/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/postgres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240427.2/pydal/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240427.2/pydal/connection.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.929208 pydal-20240427.2/pydal/contrib/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/contrib/imap_adapter.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/contrib/ipaddress.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/mockimaplib.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/ordereddict.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240427.2/pydal/contrib/portalocker.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/reserved_sql_keywords.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240427.2/pydal/default_validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.932541 pydal-20240427.2/pydal/dialects/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240427.2/pydal/dialects/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240427.2/pydal/dialects/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/dialects/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240427.2/pydal/dialects/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240427.2/pydal/dialects/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240427.2/pydal/dialects/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240427.2/pydal/dialects/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240427.2/pydal/dialects/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/drivers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/exceptions.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.935875 pydal-20240427.2/pydal/helpers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/_internals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/helpers/classes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/helpers/methods.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/regex.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/rest.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/serializers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240427.2/pydal/migrator.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   128832 2024-04-27 07:18:46.000000 pydal-20240427.2/pydal/objects.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.935875 pydal-20240427.2/pydal/parsers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/parsers/sqlite.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.939208 pydal-20240427.2/pydal/representers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/representers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/representers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/restapi.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.939208 pydal-20240427.2/pydal/tools/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/tools/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240427.2/pydal/tools/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/utils.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240427.2/pydal/validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.922541 pydal-20240427.2/pydal.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-27 07:19:10.000000 pydal-20240427.2/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-27 07:19:15.949208 pydal-20240427.2/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.942541 pydal-20240427.2/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.949208 pydal-20240427.2/tests/__pycache__/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240427.2/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240427.2/tests/__pycache__/_adapt.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/_compat.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/base.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/caching.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/contribs.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/indexes.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/is_url_validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/restapi.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/smart_query.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240427.2/tests/__pycache__/sql.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/tags.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6751 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/validation.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240427.2/tests/_adapt.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240427.2/tests/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/_helpers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240427.2/tests/caching.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/contribs.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240427.2/tests/indexes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/is_url_validators.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240427.2/tests/nosql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/restapi.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/smart_query.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240427.2/tests/sql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3604 2023-11-15 06:55:22.000000 pydal-20240427.2/tests/validation.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240427.2/tests/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.624925 pydal-20240427.3/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240427.3/AUTHORS
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240427.3/CHANGES
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240427.3/LICENSE.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240427.3/MANIFEST.in
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 08:23:38.624925 pydal-20240427.3/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240427.3/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.588257 pydal-20240427.3/docs/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/Makefile
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240427.3/docs/conf.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/index.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/pydal.adapters.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/pydal.helpers.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/requirements.txt
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.591591 pydal-20240427.3/pydal/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-27 08:23:23.000000 pydal-20240427.3/pydal/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240427.3/pydal/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_globals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_load.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.598258 pydal-20240427.3/pydal/adapters/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/adapters/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240427.3/pydal/adapters/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/postgres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240427.3/pydal/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240427.3/pydal/connection.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.601591 pydal-20240427.3/pydal/contrib/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/contrib/imap_adapter.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/contrib/ipaddress.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/mockimaplib.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/ordereddict.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240427.3/pydal/contrib/portalocker.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/reserved_sql_keywords.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240427.3/pydal/default_validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.604925 pydal-20240427.3/pydal/dialects/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240427.3/pydal/dialects/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240427.3/pydal/dialects/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/dialects/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240427.3/pydal/dialects/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240427.3/pydal/dialects/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240427.3/pydal/dialects/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240427.3/pydal/dialects/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240427.3/pydal/dialects/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/drivers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/exceptions.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.608258 pydal-20240427.3/pydal/helpers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/_internals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/helpers/classes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/helpers/methods.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/regex.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/rest.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/serializers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240427.3/pydal/migrator.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   128922 2024-04-27 08:21:46.000000 pydal-20240427.3/pydal/objects.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.611591 pydal-20240427.3/pydal/parsers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/parsers/sqlite.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.614925 pydal-20240427.3/pydal/representers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/representers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/representers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/restapi.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.614925 pydal-20240427.3/pydal/tools/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/tools/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240427.3/pydal/tools/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/utils.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240427.3/pydal/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.594924 pydal-20240427.3/pydal.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-27 08:23:32.000000 pydal-20240427.3/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-27 08:23:38.624925 pydal-20240427.3/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.618258 pydal-20240427.3/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.624925 pydal-20240427.3/tests/__pycache__/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240427.3/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240427.3/tests/__pycache__/_adapt.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/_compat.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/caching.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/contribs.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/indexes.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/is_url_validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/restapi.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/smart_query.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240427.3/tests/__pycache__/sql.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/tags.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7017 2024-04-27 08:22:34.000000 pydal-20240427.3/tests/__pycache__/validation.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240427.3/tests/_adapt.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240427.3/tests/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/_helpers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240427.3/tests/caching.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/contribs.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240427.3/tests/indexes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/is_url_validators.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240427.3/tests/nosql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/restapi.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/smart_query.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240427.3/tests/sql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3786 2024-04-27 08:22:32.000000 pydal-20240427.3/tests/validation.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240427.3/tests/validators.py
```

### Comparing `pydal-20240427.2/CHANGES` & `pydal-20240427.3/CHANGES`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/LICENSE.txt` & `pydal-20240427.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/PKG-INFO` & `pydal-20240427.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.2
+Version: 20240427.3
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.2/README.md` & `pydal-20240427.3/README.md`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/docs/Makefile` & `pydal-20240427.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/docs/conf.py` & `pydal-20240427.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/docs/index.rst` & `pydal-20240427.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/docs/pydal.adapters.rst` & `pydal-20240427.3/docs/pydal.adapters.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/docs/pydal.helpers.rst` & `pydal-20240427.3/docs/pydal.helpers.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/_compat.py` & `pydal-20240427.3/pydal/_compat.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/__init__.py` & `pydal-20240427.3/pydal/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/base.py` & `pydal-20240427.3/pydal/adapters/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/couchdb.py` & `pydal-20240427.3/pydal/adapters/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/db2.py` & `pydal-20240427.3/pydal/adapters/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/firebird.py` & `pydal-20240427.3/pydal/adapters/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/google.py` & `pydal-20240427.3/pydal/adapters/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/informix.py` & `pydal-20240427.3/pydal/adapters/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/ingres.py` & `pydal-20240427.3/pydal/adapters/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/mongo.py` & `pydal-20240427.3/pydal/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/mssql.py` & `pydal-20240427.3/pydal/adapters/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/mysql.py` & `pydal-20240427.3/pydal/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/oracle.py` & `pydal-20240427.3/pydal/adapters/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/postgres.py` & `pydal-20240427.3/pydal/adapters/postgres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/sap.py` & `pydal-20240427.3/pydal/adapters/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/snowflake.py` & `pydal-20240427.3/pydal/adapters/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/sqlite.py` & `pydal-20240427.3/pydal/adapters/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/adapters/teradata.py` & `pydal-20240427.3/pydal/adapters/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/base.py` & `pydal-20240427.3/pydal/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/connection.py` & `pydal-20240427.3/pydal/connection.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/imap_adapter.py` & `pydal-20240427.3/pydal/contrib/imap_adapter.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/ipaddress.py` & `pydal-20240427.3/pydal/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/mockimaplib.py` & `pydal-20240427.3/pydal/contrib/mockimaplib.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/ordereddict.py` & `pydal-20240427.3/pydal/contrib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/portalocker.py` & `pydal-20240427.3/pydal/contrib/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/contrib/reserved_sql_keywords.py` & `pydal-20240427.3/pydal/contrib/reserved_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/default_validators.py` & `pydal-20240427.3/pydal/default_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/__init__.py` & `pydal-20240427.3/pydal/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/base.py` & `pydal-20240427.3/pydal/dialects/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/couchdb.py` & `pydal-20240427.3/pydal/dialects/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/db2.py` & `pydal-20240427.3/pydal/dialects/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/firebird.py` & `pydal-20240427.3/pydal/dialects/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/google.py` & `pydal-20240427.3/pydal/dialects/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/informix.py` & `pydal-20240427.3/pydal/dialects/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/ingres.py` & `pydal-20240427.3/pydal/dialects/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/mongo.py` & `pydal-20240427.3/pydal/dialects/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/mssql.py` & `pydal-20240427.3/pydal/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/mysql.py` & `pydal-20240427.3/pydal/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/oracle.py` & `pydal-20240427.3/pydal/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/postgre.py` & `pydal-20240427.3/pydal/dialects/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/sap.py` & `pydal-20240427.3/pydal/dialects/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/snowflake.py` & `pydal-20240427.3/pydal/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/sqlite.py` & `pydal-20240427.3/pydal/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/dialects/teradata.py` & `pydal-20240427.3/pydal/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/drivers.py` & `pydal-20240427.3/pydal/drivers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/_internals.py` & `pydal-20240427.3/pydal/helpers/_internals.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/classes.py` & `pydal-20240427.3/pydal/helpers/classes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/gae.py` & `pydal-20240427.3/pydal/helpers/gae.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/methods.py` & `pydal-20240427.3/pydal/helpers/methods.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/regex.py` & `pydal-20240427.3/pydal/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/rest.py` & `pydal-20240427.3/pydal/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/helpers/serializers.py` & `pydal-20240427.3/pydal/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/migrator.py` & `pydal-20240427.3/pydal/migrator.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/objects.py` & `pydal-20240427.3/pydal/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,45 +898,47 @@
         if ret and self._after_insert:
             for f in self._after_insert:
                 f(row, ret)
         return ret
 
     def _validate_fields(self, fields, defattr="default", id=None):
         from .validators import CRYPT
-
+        valid_names = {f.name for f in self if f.writable and f.type != "id"}
         response = {"id": None, "errors": {}}
         new_fields = Row()
+        for name in set(fields) - valid_names:
+            response["errors"][name] = "invalid"
         for field in self:
             # we validate even if not passed in case it is required
             error = default = None
+            if field.name not in valid_names:
+                continue
             if not field.required and not field.compute:
                 default = getattr(field, defattr)
                 if callable(default):
                     default = default()
             if not field.compute:
                 ovalue = fields.get(field.name, default)
                 value, error = field.validate(ovalue, id)
             if error:
                 response["errors"][field.name] = "%s" % error
             elif field.type == "password" and ovalue == CRYPT.STARS:
                 pass
             elif field.name in fields:
                 # only write if the field was passed and no error
-                new_fields[field.name] = value
+                new_fields[field.name] = value        
         return response, new_fields
 
     def validate_and_insert(self, **fields):
-        fields = self._filter_fields(fields, allow_id=False, writable_only=True)
         response, new_fields = self._validate_fields(fields, "default")
         if not response.get("errors"):
             response["id"] = self.insert(**new_fields)
         return response
 
     def validate_and_update(self, _key, **fields):
-        fields = self._filter_fields(fields, allow_id=False, writable_only=True)
         record = self(**_key) if isinstance(_key, dict) else self(_key)
         response, new_fields = self._validate_fields(fields, "update", record.id)
         #: do the update
         if not response.get("errors") and record:
             if "_id" in self:
                 myset = self._db(self._id == record[self._id.name])
             else:
```

### Comparing `pydal-20240427.2/pydal/parsers/__init__.py` & `pydal-20240427.3/pydal/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/parsers/base.py` & `pydal-20240427.3/pydal/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/parsers/mongo.py` & `pydal-20240427.3/pydal/parsers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/parsers/oracle.py` & `pydal-20240427.3/pydal/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/parsers/postgre.py` & `pydal-20240427.3/pydal/parsers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/parsers/sqlite.py` & `pydal-20240427.3/pydal/parsers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/__init__.py` & `pydal-20240427.3/pydal/representers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/base.py` & `pydal-20240427.3/pydal/representers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/couchdb.py` & `pydal-20240427.3/pydal/representers/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/db2.py` & `pydal-20240427.3/pydal/representers/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/google.py` & `pydal-20240427.3/pydal/representers/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/informix.py` & `pydal-20240427.3/pydal/representers/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/mongo.py` & `pydal-20240427.3/pydal/representers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/mssql.py` & `pydal-20240427.3/pydal/representers/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/oracle.py` & `pydal-20240427.3/pydal/representers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/postgre.py` & `pydal-20240427.3/pydal/representers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/representers/sqlite.py` & `pydal-20240427.3/pydal/representers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/restapi.py` & `pydal-20240427.3/pydal/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/tools/tags.py` & `pydal-20240427.3/pydal/tools/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/utils.py` & `pydal-20240427.3/pydal/utils.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal/validators.py` & `pydal-20240427.3/pydal/validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pydal.egg-info/PKG-INFO` & `pydal-20240427.3/pydal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.2
+Version: 20240427.3
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.2/pydal.egg-info/SOURCES.txt` & `pydal-20240427.3/pydal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/pyproject.toml` & `pydal-20240427.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydal"
-version = "20240427.2"
+version = "20240427.3"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = 'pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pydal-20240427.2/tests/__pycache__/__init__.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/_adapt.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/_adapt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/_helpers.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/base.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/caching.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/caching.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/contribs.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/contribs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/indexes.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/is_url_validators.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/is_url_validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/restapi.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/restapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/smart_query.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/smart_query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/sql.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/sql.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/tags.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/__pycache__/validation.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/validation.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5a6b5465 (Wed Nov 15 06:55:22 2023 UTC)
-files sz: 3604
+moddate:  0xc8b52c66 (Sat Apr 27 08:22:32 2024 UTC)
+files sz: 3786
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a030100640064
@@ -107,36 +107,36 @@
                214 CALL                     3
    
     47         224 PRECALL                  0
                228 CALL                     0
    
     48         238 STORE_NAME              21 (TestValidateAndInsert)
    
-    73         240 PUSH_NULL
+    76         240 PUSH_NULL
                242 LOAD_NAME               12 (unittest)
                244 LOAD_ATTR               19 (skipIf)
                254 LOAD_NAME                8 (IS_IMAP)
                256 LOAD_CONST              12 ('TODO: IMAP test')
                258 PRECALL                  2
                262 CALL                     2
    
-    74         272 PUSH_NULL
+    77         272 PUSH_NULL
                274 LOAD_BUILD_CLASS
-               276 LOAD_CONST              15 (<code object TestValidateUpdateInsert, file "/home/mdipierro/Dropbox/packages/pydal/tests/validation.py", line 73>)
+               276 LOAD_CONST              15 (<code object TestValidateUpdateInsert, file "/home/mdipierro/Dropbox/packages/pydal/tests/validation.py", line 76>)
                278 MAKE_FUNCTION            0
                280 LOAD_CONST              16 ('TestValidateUpdateInsert')
                282 LOAD_NAME               12 (unittest)
                284 LOAD_ATTR               20 (TestCase)
                294 PRECALL                  3
                298 CALL                     3
    
-    73         308 PRECALL                  0
+    76         308 PRECALL                  0
                312 CALL                     0
    
-    74         322 STORE_NAME              22 (TestValidateUpdateInsert)
+    77         322 STORE_NAME              22 (TestValidateUpdateInsert)
                324 LOAD_CONST               1 (None)
                326 RETURN_VALUE
    consts
       0
       None
       ('DAL', 'Field')
       ('integer_types',)
@@ -431,36 +431,41 @@
                flags     : 3
                code
                   0x9700740100000000000000000000740200000000000000000000640167
                   01ac02a6020000ab0200000000000000007d017c01a00200000000000000
                   0000000000000000000000000064037407000000000000000000006404a6
                   010000ab0100000000000000007407000000000000000000006405640674
                   090000000000000000000064076408a6020000ab020000000000000000ac
-                  09a6030000ab030000000000000000a6030000ab03000000000000000001
-                  007c016a050000000000000000a006000000000000000000000000000000
-                  0000000000640a640bac0ca6020000ab0200000000000000007d02740e00
-                  000000000000000000723d7c00a008000000000000000000000000000000
-                  00000000007413000000000000000000007c02a00a000000000000000000
-                  0000000000000000000000640da6010000ab010000000000000000741600
-                  000000000000000000a6020000ab020000000000000000640ea6020000ab
-                  02000000000000000001006e297c00a00800000000000000000000000000
-                  000000000000007c02a00a00000000000000000000000000000000000000
-                  00640da6010000ab0100000000000000006407a6020000ab020000000000
-                  00000001007c00a00c00000000000000000000000000000000000000007c
-                  02a00a0000000000000000000000000000000000000000640fa6010000ab
-                  0100000000000000000c00a6010000ab01000000000000000001007c016a
-                  050000000000000000a00600000000000000000000000000000000000000
-                  006410ac11a6010000ab0100000000000000007d027c00a0080000000000
-                  0000000000000000000000000000007c02a00a0000000000000000000000
-                  000000000000000000640da6010000ab0100000000000000006400a60200
-                  00ab02000000000000000001007c00a00d00000000000000000000000000
-                  000000000000007c02640f19000000000000000000640519000000000000
-                  0000006400a6020000ab0200000000000000000100741d00000000000000
-                  0000007c016a050000000000000000a6010000ab01000000000000000001
-                  0064005300
+                  09a6030000ab030000000000000000740700000000000000000000640a64
+                  0bac0ca6020000ab020000000000000000a6040000ab0400000000000000
+                  0001007c016a050000000000000000a00600000000000000000000000000
+                  00000000000000640d640e640fac10a6030000ab0300000000000000007d
+                  027c00a0070000000000000000000000000000000000000000640a7c0264
+                  11190000000000000000007600a6010000ab01000000000000000001007c
+                  016a050000000000000000a0060000000000000000000000000000000000
+                  000000640d640eac12a6020000ab0200000000000000007d027410000000
+                  00000000000000723d7c00a0090000000000000000000000000000000000
+                  0000007415000000000000000000007c02a00b0000000000000000000000
+                  0000000000000000006413a6010000ab0100000000000000007418000000
+                  00000000000000a6020000ab0200000000000000006414a6020000ab0200
+                  0000000000000001006e297c00a009000000000000000000000000000000
+                  00000000007c02a00b000000000000000000000000000000000000000064
+                  13a6010000ab0100000000000000006407a6020000ab0200000000000000
+                  0001007c00a00700000000000000000000000000000000000000007c02a0
+                  0b00000000000000000000000000000000000000006411a6010000ab0100
+                  000000000000000c00a6010000ab01000000000000000001007c016a0500
+                  00000000000000a006000000000000000000000000000000000000000064
+                  15ac16a6010000ab0100000000000000007d027c00a00900000000000000
+                  000000000000000000000000007c02a00b00000000000000000000000000
+                  000000000000006413a6010000ab0100000000000000006400a6020000ab
+                  02000000000000000001007c00a00d000000000000000000000000000000
+                  00000000007c026411190000000000000000006405190000000000000000
+                  006400a6020000ab0200000000000000000100741d000000000000000000
+                  007c016a050000000000000000a6010000ab010000000000000000010064
+                  005300
                 49           0 RESUME                   0
                
                 50           2 LOAD_GLOBAL              1 (NULL + DAL)
                             14 LOAD_GLOBAL              2 (DEFAULT_URI)
                             26 LOAD_CONST               1 ('all')
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
@@ -486,142 +491,176 @@
                            132 LOAD_CONST               8 (5)
                            134 PRECALL                  2
                            138 CALL                     2
                            148 KW_NAMES                 9
                            150 PRECALL                  3
                            154 CALL                     3
                
-                51         164 PRECALL                  3
-                           168 CALL                     3
-                           178 POP_TOP
-               
-                56         180 LOAD_FAST                1 (db)
-                           182 LOAD_ATTR                5 (val_and_insert)
-                           192 LOAD_METHOD              6 (validate_and_insert)
-                           214 LOAD_CONST              10 ('test1')
-                           216 LOAD_CONST              11 (2)
-                           218 KW_NAMES                12
-                           220 PRECALL                  2
-                           224 CALL                     2
-                           234 STORE_FAST               2 (rtn)
-               
-                57         236 LOAD_GLOBAL             14 (IS_NOSQL)
-                           248 POP_JUMP_FORWARD_IF_FALSE    61 (to 372)
-               
-                58         250 LOAD_FAST                0 (self)
-                           252 LOAD_METHOD              8 (assertEqual)
-                           274 LOAD_GLOBAL             19 (NULL + isinstance)
-                           286 LOAD_FAST                2 (rtn)
-                           288 LOAD_METHOD             10 (get)
-                           310 LOAD_CONST              13 ('id')
+                55         164 LOAD_GLOBAL              7 (NULL + Field)
+                           176 LOAD_CONST              10 ('cc')
+                           178 LOAD_CONST              11 (False)
+                           180 KW_NAMES                12
+                           182 PRECALL                  2
+                           186 CALL                     2
+               
+                51         196 PRECALL                  4
+                           200 CALL                     4
+                           210 POP_TOP
+               
+                57         212 LOAD_FAST                1 (db)
+                           214 LOAD_ATTR                5 (val_and_insert)
+                           224 LOAD_METHOD              6 (validate_and_insert)
+                           246 LOAD_CONST              13 ('test1')
+                           248 LOAD_CONST              14 (2)
+                           250 LOAD_CONST              15 ('not-alloed')
+                           252 KW_NAMES                16
+                           254 PRECALL                  3
+                           258 CALL                     3
+                           268 STORE_FAST               2 (rtn)
+               
+                58         270 LOAD_FAST                0 (self)
+                           272 LOAD_METHOD              7 (assertTrue)
+                           294 LOAD_CONST              10 ('cc')
+                           296 LOAD_FAST                2 (rtn)
+                           298 LOAD_CONST              17 ('errors')
+                           300 BINARY_SUBSCR
+                           310 CONTAINS_OP              0
                            312 PRECALL                  1
                            316 CALL                     1
-                           326 LOAD_GLOBAL             22 (long)
-                           338 PRECALL                  2
-                           342 CALL                     2
-                           352 LOAD_CONST              14 (True)
-                           354 PRECALL                  2
-                           358 CALL                     2
-                           368 POP_TOP
-                           370 JUMP_FORWARD            41 (to 454)
-               
-                60     >>  372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD              8 (assertEqual)
-                           396 LOAD_FAST                2 (rtn)
-                           398 LOAD_METHOD             10 (get)
-                           420 LOAD_CONST              13 ('id')
-                           422 PRECALL                  1
-                           426 CALL                     1
-                           436 LOAD_CONST               7 (1)
-                           438 PRECALL                  2
-                           442 CALL                     2
-                           452 POP_TOP
-               
-                62     >>  454 LOAD_FAST                0 (self)
-                           456 LOAD_METHOD             12 (assertTrue)
-                           478 LOAD_FAST                2 (rtn)
-                           480 LOAD_METHOD             10 (get)
-                           502 LOAD_CONST              15 ('errors')
-                           504 PRECALL                  1
-                           508 CALL                     1
-                           518 UNARY_NOT
-                           520 PRECALL                  1
-                           524 CALL                     1
-                           534 POP_TOP
-               
-                64         536 LOAD_FAST                1 (db)
-                           538 LOAD_ATTR                5 (val_and_insert)
-                           548 LOAD_METHOD              6 (validate_and_insert)
-                           570 LOAD_CONST              16 ('a')
-                           572 KW_NAMES                17
-                           574 PRECALL                  1
-                           578 CALL                     1
-                           588 STORE_FAST               2 (rtn)
-               
-                66         590 LOAD_FAST                0 (self)
-                           592 LOAD_METHOD              8 (assertEqual)
-                           614 LOAD_FAST                2 (rtn)
-                           616 LOAD_METHOD             10 (get)
-                           638 LOAD_CONST              13 ('id')
-                           640 PRECALL                  1
-                           644 CALL                     1
-                           654 LOAD_CONST               0 (None)
-                           656 PRECALL                  2
-                           660 CALL                     2
-                           670 POP_TOP
-               
-                68         672 LOAD_FAST                0 (self)
-                           674 LOAD_METHOD             13 (assertNotEqual)
-                           696 LOAD_FAST                2 (rtn)
-                           698 LOAD_CONST              15 ('errors')
-                           700 BINARY_SUBSCR
-                           710 LOAD_CONST               5 ('bb')
-                           712 BINARY_SUBSCR
-                           722 LOAD_CONST               0 (None)
-                           724 PRECALL                  2
-                           728 CALL                     2
-                           738 POP_TOP
-               
-                70         740 LOAD_GLOBAL             29 (NULL + drop)
-                           752 LOAD_FAST                1 (db)
-                           754 LOAD_ATTR                5 (val_and_insert)
-                           764 PRECALL                  1
-                           768 CALL                     1
-                           778 POP_TOP
-                           780 LOAD_CONST               0 (None)
-                           782 RETURN_VALUE
+                           326 POP_TOP
+               
+                59         328 LOAD_FAST                1 (db)
+                           330 LOAD_ATTR                5 (val_and_insert)
+                           340 LOAD_METHOD              6 (validate_and_insert)
+                           362 LOAD_CONST              13 ('test1')
+                           364 LOAD_CONST              14 (2)
+                           366 KW_NAMES                18
+                           368 PRECALL                  2
+                           372 CALL                     2
+                           382 STORE_FAST               2 (rtn)
+               
+                60         384 LOAD_GLOBAL             16 (IS_NOSQL)
+                           396 POP_JUMP_FORWARD_IF_FALSE    61 (to 520)
+               
+                61         398 LOAD_FAST                0 (self)
+                           400 LOAD_METHOD              9 (assertEqual)
+                           422 LOAD_GLOBAL             21 (NULL + isinstance)
+                           434 LOAD_FAST                2 (rtn)
+                           436 LOAD_METHOD             11 (get)
+                           458 LOAD_CONST              19 ('id')
+                           460 PRECALL                  1
+                           464 CALL                     1
+                           474 LOAD_GLOBAL             24 (long)
+                           486 PRECALL                  2
+                           490 CALL                     2
+                           500 LOAD_CONST              20 (True)
+                           502 PRECALL                  2
+                           506 CALL                     2
+                           516 POP_TOP
+                           518 JUMP_FORWARD            41 (to 602)
+               
+                63     >>  520 LOAD_FAST                0 (self)
+                           522 LOAD_METHOD              9 (assertEqual)
+                           544 LOAD_FAST                2 (rtn)
+                           546 LOAD_METHOD             11 (get)
+                           568 LOAD_CONST              19 ('id')
+                           570 PRECALL                  1
+                           574 CALL                     1
+                           584 LOAD_CONST               7 (1)
+                           586 PRECALL                  2
+                           590 CALL                     2
+                           600 POP_TOP
+               
+                65     >>  602 LOAD_FAST                0 (self)
+                           604 LOAD_METHOD              7 (assertTrue)
+                           626 LOAD_FAST                2 (rtn)
+                           628 LOAD_METHOD             11 (get)
+                           650 LOAD_CONST              17 ('errors')
+                           652 PRECALL                  1
+                           656 CALL                     1
+                           666 UNARY_NOT
+                           668 PRECALL                  1
+                           672 CALL                     1
+                           682 POP_TOP
+               
+                67         684 LOAD_FAST                1 (db)
+                           686 LOAD_ATTR                5 (val_and_insert)
+                           696 LOAD_METHOD              6 (validate_and_insert)
+                           718 LOAD_CONST              21 ('a')
+                           720 KW_NAMES                22
+                           722 PRECALL                  1
+                           726 CALL                     1
+                           736 STORE_FAST               2 (rtn)
+               
+                69         738 LOAD_FAST                0 (self)
+                           740 LOAD_METHOD              9 (assertEqual)
+                           762 LOAD_FAST                2 (rtn)
+                           764 LOAD_METHOD             11 (get)
+                           786 LOAD_CONST              19 ('id')
+                           788 PRECALL                  1
+                           792 CALL                     1
+                           802 LOAD_CONST               0 (None)
+                           804 PRECALL                  2
+                           808 CALL                     2
+                           818 POP_TOP
+               
+                71         820 LOAD_FAST                0 (self)
+                           822 LOAD_METHOD             13 (assertNotEqual)
+                           844 LOAD_FAST                2 (rtn)
+                           846 LOAD_CONST              17 ('errors')
+                           848 BINARY_SUBSCR
+                           858 LOAD_CONST               5 ('bb')
+                           860 BINARY_SUBSCR
+                           870 LOAD_CONST               0 (None)
+                           872 PRECALL                  2
+                           876 CALL                     2
+                           886 POP_TOP
+               
+                73         888 LOAD_GLOBAL             29 (NULL + drop)
+                           900 LOAD_FAST                1 (db)
+                           902 LOAD_ATTR                5 (val_and_insert)
+                           912 PRECALL                  1
+                           916 CALL                     1
+                           926 POP_TOP
+                           928 LOAD_CONST               0 (None)
+                           930 RETURN_VALUE
                consts
                   None
                   'all'
                   ('check_reserved',)
                   'val_and_insert'
                   'aa'
                   'bb'
                   'integer'
                   1
                   5
                   ('requires',)
+                  'cc'
+                  False
+                  ('writable',)
                   'test1'
                   2
+                  'not-alloed'
+                  ('aa', 'bb', 'cc')
+                  'errors'
                   ('aa', 'bb')
                   'id'
                   True
-                  'errors'
                   'a'
                   ('bb',)
-               names      ('DAL', 'DEFAULT_URI', 'define_table', 'Field', 'IS_INT_IN_RANGE', 'val_and_insert', 'validate_and_insert', 'IS_NOSQL', 'assertEqual', 'isinstance', 'get', 'long', 'assertTrue', 'assertNotEqual', 'drop')
+               names      ('DAL', 'DEFAULT_URI', 'define_table', 'Field', 'IS_INT_IN_RANGE', 'val_and_insert', 'validate_and_insert', 'assertTrue', 'IS_NOSQL', 'assertEqual', 'isinstance', 'get', 'long', 'assertNotEqual', 'drop')
                varnames   ('self', 'db', 'rtn')
                freevars   ()
                cellvars   ()
                filename   '/home/mdipierro/Dropbox/packages/pydal/tests/validation.py'
                name       'testRun'
                firstlineno 49
                lnotab
-                  0x02012e01180102011c013efd100538010e017a02520252023602520244
-                  02
+                  0x02012e01180102011c013e0120fc10063a013a0138010e017a02520252
+                  02360252024402
             None
          names      ('__name__', '__module__', '__qualname__', 'testRun')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/mdipierro/Dropbox/packages/pydal/tests/validation.py'
          name       'TestValidateAndInsert'
@@ -630,21 +669,21 @@
       'TestValidateAndInsert'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          73           0 RESUME                   0
+          76           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TestValidateUpdateInsert')
                        8 STORE_NAME               2 (__qualname__)
          
-          75          10 LOAD_CONST               1 (<code object testRun, file "/home/mdipierro/Dropbox/packages/pydal/tests/validation.py", line 75>)
+          78          10 LOAD_CONST               1 (<code object testRun, file "/home/mdipierro/Dropbox/packages/pydal/tests/validation.py", line 78>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (testRun)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'TestValidateUpdateInsert'
             code
@@ -690,104 +729,104 @@
                   00a6000000ab000000000000000000640ea6020000ab0200000000000000
                   0001007c00a009000000000000000000000000000000000000000002007c
                   017c026a060000000000000000640a6b0200000000a6010000ab01000000
                   0000000000a00c0000000000000000000000000000000000000000a60000
                   00ab0000000000000000006406a6020000ab020000000000000000010074
                   1b000000000000000000007c016a0e0000000000000000a6010000ab0100
                   00000000000000010064005300
-                75           0 RESUME                   0
+                78           0 RESUME                   0
                
-                76           2 LOAD_GLOBAL              1 (NULL + DAL)
+                79           2 LOAD_GLOBAL              1 (NULL + DAL)
                             14 LOAD_GLOBAL              2 (DEFAULT_URI)
                             26 LOAD_CONST               1 ('all')
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               1 (db)
                
-                77          48 LOAD_FAST                1 (db)
+                80          48 LOAD_FAST                1 (db)
                             50 LOAD_METHOD              2 (define_table)
                
-                78          72 LOAD_CONST               3 ('t1')
+                81          72 LOAD_CONST               3 ('t1')
                             74 LOAD_GLOBAL              7 (NULL + Field)
                             86 LOAD_CONST               4 ('int_level')
                             88 LOAD_CONST               5 ('integer')
                             90 LOAD_GLOBAL              9 (NULL + IS_INT_IN_RANGE)
                            102 LOAD_CONST               6 (1)
                            104 LOAD_CONST               7 (5)
                            106 PRECALL                  2
                            110 CALL                     2
                            120 KW_NAMES                 8
                            122 PRECALL                  3
                            126 CALL                     3
                
-                77         136 PRECALL                  2
+                80         136 PRECALL                  2
                            140 CALL                     2
                            150 STORE_FAST               2 (t1)
                
-                80         152 LOAD_FAST                2 (t1)
+                83         152 LOAD_FAST                2 (t1)
                            154 LOAD_METHOD              5 (validate_and_update_or_insert)
                            176 LOAD_FAST                2 (t1)
                            178 LOAD_ATTR                6 (int_level)
                            188 LOAD_CONST               6 (1)
                            190 COMPARE_OP               2 (==)
                            196 LOAD_CONST               6 (1)
                            198 KW_NAMES                 9
                            200 PRECALL                  2
                            204 CALL                     2
                            214 STORE_FAST               3 (i_response)
                
-                81         216 LOAD_FAST                2 (t1)
+                84         216 LOAD_FAST                2 (t1)
                            218 LOAD_METHOD              5 (validate_and_update_or_insert)
                            240 LOAD_FAST                2 (t1)
                            242 LOAD_ATTR                6 (int_level)
                            252 LOAD_CONST               6 (1)
                            254 COMPARE_OP               2 (==)
                            260 LOAD_CONST              10 (2)
                            262 KW_NAMES                 9
                            264 PRECALL                  2
                            268 CALL                     2
                            278 STORE_FAST               4 (u_response)
                
-                82         280 LOAD_FAST                2 (t1)
+                85         280 LOAD_FAST                2 (t1)
                            282 LOAD_METHOD              5 (validate_and_update_or_insert)
                            304 LOAD_FAST                2 (t1)
                            306 LOAD_ATTR                6 (int_level)
                            316 LOAD_CONST               6 (1)
                            318 COMPARE_OP               2 (==)
                            324 LOAD_CONST              11 (6)
                            326 KW_NAMES                 9
                            328 PRECALL                  2
                            332 CALL                     2
                            342 STORE_FAST               5 (e_response)
                
-                83         344 LOAD_FAST                0 (self)
+                86         344 LOAD_FAST                0 (self)
                            346 LOAD_METHOD              7 (assertTrue)
                            368 LOAD_FAST                3 (i_response)
                            370 LOAD_CONST              12 ('id')
                            372 BINARY_SUBSCR
                            382 LOAD_CONST               0 (None)
                            384 COMPARE_OP               3 (!=)
                            390 PRECALL                  1
                            394 CALL                     1
                            404 POP_TOP
                
-                84         406 LOAD_FAST                0 (self)
+                87         406 LOAD_FAST                0 (self)
                            408 LOAD_METHOD              7 (assertTrue)
                            430 LOAD_FAST                4 (u_response)
                            432 LOAD_CONST              12 ('id')
                            434 BINARY_SUBSCR
                            444 LOAD_CONST               0 (None)
                            446 COMPARE_OP               3 (!=)
                            452 PRECALL                  1
                            456 CALL                     1
                            466 POP_TOP
                
-                85         468 LOAD_FAST                0 (self)
+                88         468 LOAD_FAST                0 (self)
                            470 LOAD_METHOD              7 (assertTrue)
                            492 LOAD_FAST                5 (e_response)
                            494 LOAD_METHOD              8 (get)
                            516 LOAD_CONST              12 ('id')
                            518 PRECALL                  1
                            522 CALL                     1
                            532 LOAD_CONST               0 (None)
@@ -798,15 +837,15 @@
                            566 LOAD_CONST              13 ('errors')
                            568 PRECALL                  1
                            572 CALL                     1
                        >>  582 PRECALL                  1
                            586 CALL                     1
                            596 POP_TOP
                
-                86         598 LOAD_FAST                0 (self)
+                89         598 LOAD_FAST                0 (self)
                            600 LOAD_METHOD              9 (assertEqual)
                            622 LOAD_GLOBAL             21 (NULL + len)
                            634 PUSH_NULL
                            636 LOAD_FAST                1 (db)
                            638 LOAD_FAST                2 (t1)
                            640 PRECALL                  1
                            644 CALL                     1
@@ -816,30 +855,30 @@
                            690 PRECALL                  1
                            694 CALL                     1
                            704 LOAD_CONST               6 (1)
                            706 PRECALL                  2
                            710 CALL                     2
                            720 POP_TOP
                
-                87         722 LOAD_FAST                0 (self)
+                90         722 LOAD_FAST                0 (self)
                            724 LOAD_METHOD              9 (assertEqual)
                            746 PUSH_NULL
                            748 LOAD_FAST                1 (db)
                            750 LOAD_FAST                2 (t1)
                            752 PRECALL                  1
                            756 CALL                     1
                            766 LOAD_METHOD             12 (count)
                            788 PRECALL                  0
                            792 CALL                     0
                            802 LOAD_CONST               6 (1)
                            804 PRECALL                  2
                            808 CALL                     2
                            818 POP_TOP
                
-                88         820 LOAD_FAST                0 (self)
+                91         820 LOAD_FAST                0 (self)
                            822 LOAD_METHOD              9 (assertEqual)
                            844 PUSH_NULL
                            846 LOAD_FAST                1 (db)
                            848 LOAD_FAST                2 (t1)
                            850 LOAD_ATTR                6 (int_level)
                            860 LOAD_CONST               6 (1)
                            862 COMPARE_OP               2 (==)
@@ -849,15 +888,15 @@
                            904 PRECALL                  0
                            908 CALL                     0
                            918 LOAD_CONST              14 (0)
                            920 PRECALL                  2
                            924 CALL                     2
                            934 POP_TOP
                
-                89         936 LOAD_FAST                0 (self)
+                92         936 LOAD_FAST                0 (self)
                            938 LOAD_METHOD              9 (assertEqual)
                            960 PUSH_NULL
                            962 LOAD_FAST                1 (db)
                            964 LOAD_FAST                2 (t1)
                            966 LOAD_ATTR                6 (int_level)
                            976 LOAD_CONST              11 (6)
                            978 COMPARE_OP               2 (==)
@@ -867,15 +906,15 @@
                           1020 PRECALL                  0
                           1024 CALL                     0
                           1034 LOAD_CONST              14 (0)
                           1036 PRECALL                  2
                           1040 CALL                     2
                           1050 POP_TOP
                
-                90        1052 LOAD_FAST                0 (self)
+                93        1052 LOAD_FAST                0 (self)
                           1054 LOAD_METHOD              9 (assertEqual)
                           1076 PUSH_NULL
                           1078 LOAD_FAST                1 (db)
                           1080 LOAD_FAST                2 (t1)
                           1082 LOAD_ATTR                6 (int_level)
                           1092 LOAD_CONST              10 (2)
                           1094 COMPARE_OP               2 (==)
@@ -885,22 +924,22 @@
                           1136 PRECALL                  0
                           1140 CALL                     0
                           1150 LOAD_CONST               6 (1)
                           1152 PRECALL                  2
                           1156 CALL                     2
                           1166 POP_TOP
                
-                91        1168 LOAD_GLOBAL             27 (NULL + drop)
+                94        1168 LOAD_GLOBAL             27 (NULL + drop)
                           1180 LOAD_FAST                1 (db)
                           1182 LOAD_ATTR               14 (t1)
                           1192 PRECALL                  1
                           1196 CALL                     1
                           1206 POP_TOP
                
-                92        1208 LOAD_CONST               0 (None)
+                95        1208 LOAD_CONST               0 (None)
                           1210 RETURN_VALUE
                consts
                   None
                   'all'
                   ('check_reserved',)
                   't1'
                   'int_level'
@@ -916,31 +955,31 @@
                   0
                names      ('DAL', 'DEFAULT_URI', 'define_table', 'Field', 'IS_INT_IN_RANGE', 'validate_and_update_or_insert', 'int_level', 'assertTrue', 'get', 'assertEqual', 'len', 'select', 'count', 'drop', 't1')
                varnames   ('self', 'db', 't1', 'i_response', 'u_response', 'e_response')
                freevars   ()
                cellvars   ()
                filename   '/home/mdipierro/Dropbox/packages/pydal/tests/validation.py'
                name       'testRun'
-               firstlineno 75
+               firstlineno 78
                lnotab
                   0x02012e01180140ff10034001400140013e013e0182017c016201740174
                   0174012801
             None
          names      ('__name__', '__module__', '__qualname__', 'testRun')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/mdipierro/Dropbox/packages/pydal/tests/validation.py'
          name       'TestValidateUpdateInsert'
-         firstlineno 73
+         firstlineno 76
          lnotab 0x0a02
       'TestValidateUpdateInsert'
    names      ('re', 'pydal', 'DAL', 'Field', 'pydal._compat', 'integer_types', '_adapt', 'DEFAULT_URI', 'IS_IMAP', 'IS_NOSQL', 'drop', '_compat', 'unittest', 'long', 'compile', 'regex_isint', 'range_error_message', 'object', 'IS_INT_IN_RANGE', 'skipIf', 'TestCase', 'TestValidateAndInsert', 'TestValidateUpdateInsert')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/mdipierro/Dropbox/packages/pydal/tests/validation.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080210010c0218010c0210022003060f1c12200124ff0e0102
-      19200124ff0e01
+      1c200124ff0e01
```

### Comparing `pydal-20240427.2/tests/__pycache__/validators.cpython-311.pyc` & `pydal-20240427.3/tests/__pycache__/validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/_adapt.py` & `pydal-20240427.3/tests/_adapt.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/_helpers.py` & `pydal-20240427.3/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/base.py` & `pydal-20240427.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/caching.py` & `pydal-20240427.3/tests/caching.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/contribs.py` & `pydal-20240427.3/tests/contribs.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/indexes.py` & `pydal-20240427.3/tests/indexes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/is_url_validators.py` & `pydal-20240427.3/tests/is_url_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/nosql.py` & `pydal-20240427.3/tests/nosql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/restapi.py` & `pydal-20240427.3/tests/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/smart_query.py` & `pydal-20240427.3/tests/smart_query.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/sql.py` & `pydal-20240427.3/tests/sql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/tags.py` & `pydal-20240427.3/tests/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.2/tests/validation.py` & `pydal-20240427.3/tests/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 class TestValidateAndInsert(unittest.TestCase):
     def testRun(self):
         db = DAL(DEFAULT_URI, check_reserved=["all"])
         db.define_table(
             "val_and_insert",
             Field("aa"),
             Field("bb", "integer", requires=IS_INT_IN_RANGE(1, 5)),
+            Field("cc", writable=False)
         )
+        rtn = db.val_and_insert.validate_and_insert(aa="test1", bb=2, cc="not-alloed")
+        self.assertTrue("cc" in rtn["errors"])        
         rtn = db.val_and_insert.validate_and_insert(aa="test1", bb=2)
         if IS_NOSQL:
             self.assertEqual(isinstance(rtn.get("id"), long), True)
         else:
             self.assertEqual(rtn.get("id"), 1)
         # errors should be empty
         self.assertTrue(not rtn.get("errors"))
```

### Comparing `pydal-20240427.2/tests/validators.py` & `pydal-20240427.3/tests/validators.py`

 * *Files identical despite different names*

