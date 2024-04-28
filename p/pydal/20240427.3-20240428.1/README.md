# Comparing `tmp/pydal-20240427.3.tar.gz` & `tmp/pydal-20240428.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydal-20240427.3.tar", last modified: Sat Apr 27 08:23:38 2024, max compression
+gzip compressed data, was "pydal-20240428.1.tar", last modified: Sun Apr 28 00:51:37 2024, max compression
```

## Comparing `pydal-20240427.3.tar` & `pydal-20240428.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.624925 pydal-20240427.3/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240427.3/AUTHORS
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240427.3/CHANGES
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240427.3/LICENSE.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240427.3/MANIFEST.in
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 08:23:38.624925 pydal-20240427.3/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240427.3/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.588257 pydal-20240427.3/docs/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/Makefile
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240427.3/docs/conf.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/index.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/pydal.adapters.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/pydal.helpers.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240427.3/docs/requirements.txt
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.591591 pydal-20240427.3/pydal/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-27 08:23:23.000000 pydal-20240427.3/pydal/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240427.3/pydal/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_globals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/_load.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.598258 pydal-20240427.3/pydal/adapters/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/adapters/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240427.3/pydal/adapters/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/postgres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/adapters/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240427.3/pydal/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240427.3/pydal/connection.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.601591 pydal-20240427.3/pydal/contrib/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/contrib/imap_adapter.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/contrib/ipaddress.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/mockimaplib.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/ordereddict.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240427.3/pydal/contrib/portalocker.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/contrib/reserved_sql_keywords.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240427.3/pydal/default_validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.604925 pydal-20240427.3/pydal/dialects/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240427.3/pydal/dialects/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240427.3/pydal/dialects/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/dialects/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240427.3/pydal/dialects/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240427.3/pydal/dialects/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240427.3/pydal/dialects/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240427.3/pydal/dialects/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240427.3/pydal/dialects/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/dialects/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/drivers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/exceptions.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.608258 pydal-20240427.3/pydal/helpers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/_internals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/helpers/classes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/helpers/methods.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/regex.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/rest.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/helpers/serializers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240427.3/pydal/migrator.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   128922 2024-04-27 08:21:46.000000 pydal-20240427.3/pydal/objects.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.611591 pydal-20240427.3/pydal/parsers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/parsers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240427.3/pydal/parsers/sqlite.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.614925 pydal-20240427.3/pydal/representers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/representers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/representers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/representers/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240427.3/pydal/restapi.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.614925 pydal-20240427.3/pydal/tools/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/tools/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240427.3/pydal/tools/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240427.3/pydal/utils.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240427.3/pydal/validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.594924 pydal-20240427.3/pydal.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-27 08:23:38.000000 pydal-20240427.3/pydal.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-27 08:23:32.000000 pydal-20240427.3/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-27 08:23:38.624925 pydal-20240427.3/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.618258 pydal-20240427.3/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 08:23:38.624925 pydal-20240427.3/tests/__pycache__/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240427.3/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240427.3/tests/__pycache__/_adapt.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/_compat.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/base.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/caching.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/contribs.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/indexes.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/is_url_validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/restapi.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/smart_query.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240427.3/tests/__pycache__/sql.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/tags.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7017 2024-04-27 08:22:34.000000 pydal-20240427.3/tests/__pycache__/validation.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240427.3/tests/__pycache__/validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240427.3/tests/_adapt.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240427.3/tests/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/_helpers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240427.3/tests/caching.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/contribs.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240427.3/tests/indexes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/is_url_validators.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240427.3/tests/nosql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240427.3/tests/restapi.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/smart_query.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240427.3/tests/sql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240427.3/tests/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3786 2024-04-27 08:22:32.000000 pydal-20240427.3/tests/validation.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240427.3/tests/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.710327 pydal-20240428.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240428.1/AUTHORS
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240428.1/CHANGES
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240428.1/LICENSE.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240428.1/MANIFEST.in
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-28 00:51:37.710327 pydal-20240428.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240428.1/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.676993 pydal-20240428.1/docs/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240428.1/docs/Makefile
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240428.1/docs/conf.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240428.1/docs/index.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240428.1/docs/pydal.adapters.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240428.1/docs/pydal.helpers.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240428.1/docs/requirements.txt
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.680326 pydal-20240428.1/pydal/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-28 00:49:00.000000 pydal-20240428.1/pydal/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240428.1/pydal/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/_gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/_globals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/_load.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.686993 pydal-20240428.1/pydal/adapters/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/adapters/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240428.1/pydal/adapters/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/postgres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/adapters/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240428.1/pydal/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240428.1/pydal/connection.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.686993 pydal-20240428.1/pydal/contrib/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/contrib/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/contrib/imap_adapter.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/contrib/ipaddress.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/contrib/mockimaplib.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/contrib/ordereddict.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240428.1/pydal/contrib/portalocker.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/contrib/reserved_sql_keywords.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240428.1/pydal/default_validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.693660 pydal-20240428.1/pydal/dialects/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240428.1/pydal/dialects/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240428.1/pydal/dialects/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/dialects/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240428.1/pydal/dialects/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240428.1/pydal/dialects/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240428.1/pydal/dialects/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240428.1/pydal/dialects/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240428.1/pydal/dialects/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/dialects/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/drivers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/exceptions.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.693660 pydal-20240428.1/pydal/helpers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/_internals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/helpers/classes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/helpers/methods.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/regex.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/rest.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/helpers/serializers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240428.1/pydal/migrator.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   129740 2024-04-28 00:47:26.000000 pydal-20240428.1/pydal/objects.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.696993 pydal-20240428.1/pydal/parsers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/parsers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240428.1/pydal/parsers/sqlite.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.700327 pydal-20240428.1/pydal/representers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240428.1/pydal/representers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240428.1/pydal/representers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/representers/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240428.1/pydal/restapi.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.700327 pydal-20240428.1/pydal/tools/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/tools/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240428.1/pydal/tools/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240428.1/pydal/utils.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240428.1/pydal/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.683659 pydal-20240428.1/pydal.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-28 00:51:37.000000 pydal-20240428.1/pydal.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-28 00:51:37.000000 pydal-20240428.1/pydal.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-28 00:51:37.000000 pydal-20240428.1/pydal.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-28 00:51:37.000000 pydal-20240428.1/pydal.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-28 00:48:45.000000 pydal-20240428.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-28 00:51:37.710327 pydal-20240428.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.706993 pydal-20240428.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240428.1/tests/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-28 00:51:37.710327 pydal-20240428.1/tests/__pycache__/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240428.1/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240428.1/tests/__pycache__/_adapt.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/_compat.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/caching.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/contribs.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/indexes.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/is_url_validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/restapi.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/smart_query.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240428.1/tests/__pycache__/sql.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/tags.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7017 2024-04-27 08:22:34.000000 pydal-20240428.1/tests/__pycache__/validation.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240428.1/tests/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240428.1/tests/_adapt.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240428.1/tests/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240428.1/tests/_helpers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240428.1/tests/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240428.1/tests/caching.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240428.1/tests/contribs.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240428.1/tests/indexes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240428.1/tests/is_url_validators.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240428.1/tests/nosql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240428.1/tests/restapi.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240428.1/tests/smart_query.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240428.1/tests/sql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240428.1/tests/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3786 2024-04-27 08:22:32.000000 pydal-20240428.1/tests/validation.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240428.1/tests/validators.py
```

### Comparing `pydal-20240427.3/CHANGES` & `pydal-20240428.1/CHANGES`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/LICENSE.txt` & `pydal-20240428.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/PKG-INFO` & `pydal-20240428.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.3
+Version: 20240428.1
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.3/README.md` & `pydal-20240428.1/README.md`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/docs/Makefile` & `pydal-20240428.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/docs/conf.py` & `pydal-20240428.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/docs/index.rst` & `pydal-20240428.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/docs/pydal.adapters.rst` & `pydal-20240428.1/docs/pydal.adapters.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/docs/pydal.helpers.rst` & `pydal-20240428.1/docs/pydal.helpers.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/_compat.py` & `pydal-20240428.1/pydal/_compat.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/__init__.py` & `pydal-20240428.1/pydal/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/base.py` & `pydal-20240428.1/pydal/adapters/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/couchdb.py` & `pydal-20240428.1/pydal/adapters/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/db2.py` & `pydal-20240428.1/pydal/adapters/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/firebird.py` & `pydal-20240428.1/pydal/adapters/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/google.py` & `pydal-20240428.1/pydal/adapters/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/informix.py` & `pydal-20240428.1/pydal/adapters/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/ingres.py` & `pydal-20240428.1/pydal/adapters/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/mongo.py` & `pydal-20240428.1/pydal/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/mssql.py` & `pydal-20240428.1/pydal/adapters/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/mysql.py` & `pydal-20240428.1/pydal/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/oracle.py` & `pydal-20240428.1/pydal/adapters/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/postgres.py` & `pydal-20240428.1/pydal/adapters/postgres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/sap.py` & `pydal-20240428.1/pydal/adapters/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/snowflake.py` & `pydal-20240428.1/pydal/adapters/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/sqlite.py` & `pydal-20240428.1/pydal/adapters/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/adapters/teradata.py` & `pydal-20240428.1/pydal/adapters/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/base.py` & `pydal-20240428.1/pydal/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/connection.py` & `pydal-20240428.1/pydal/connection.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/imap_adapter.py` & `pydal-20240428.1/pydal/contrib/imap_adapter.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/ipaddress.py` & `pydal-20240428.1/pydal/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/mockimaplib.py` & `pydal-20240428.1/pydal/contrib/mockimaplib.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/ordereddict.py` & `pydal-20240428.1/pydal/contrib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/portalocker.py` & `pydal-20240428.1/pydal/contrib/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/contrib/reserved_sql_keywords.py` & `pydal-20240428.1/pydal/contrib/reserved_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/default_validators.py` & `pydal-20240428.1/pydal/default_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/__init__.py` & `pydal-20240428.1/pydal/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/base.py` & `pydal-20240428.1/pydal/dialects/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/couchdb.py` & `pydal-20240428.1/pydal/dialects/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/db2.py` & `pydal-20240428.1/pydal/dialects/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/firebird.py` & `pydal-20240428.1/pydal/dialects/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/google.py` & `pydal-20240428.1/pydal/dialects/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/informix.py` & `pydal-20240428.1/pydal/dialects/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/ingres.py` & `pydal-20240428.1/pydal/dialects/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/mongo.py` & `pydal-20240428.1/pydal/dialects/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/mssql.py` & `pydal-20240428.1/pydal/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/mysql.py` & `pydal-20240428.1/pydal/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/oracle.py` & `pydal-20240428.1/pydal/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/postgre.py` & `pydal-20240428.1/pydal/dialects/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/sap.py` & `pydal-20240428.1/pydal/dialects/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/snowflake.py` & `pydal-20240428.1/pydal/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/sqlite.py` & `pydal-20240428.1/pydal/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/dialects/teradata.py` & `pydal-20240428.1/pydal/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/drivers.py` & `pydal-20240428.1/pydal/drivers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/_internals.py` & `pydal-20240428.1/pydal/helpers/_internals.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/classes.py` & `pydal-20240428.1/pydal/helpers/classes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/gae.py` & `pydal-20240428.1/pydal/helpers/gae.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/methods.py` & `pydal-20240428.1/pydal/helpers/methods.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/regex.py` & `pydal-20240428.1/pydal/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/rest.py` & `pydal-20240428.1/pydal/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/helpers/serializers.py` & `pydal-20240428.1/pydal/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/migrator.py` & `pydal-20240428.1/pydal/migrator.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/objects.py` & `pydal-20240428.1/pydal/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,67 +896,87 @@
             return 0
         ret = self._db._adapter.insert(self, row.op_values())
         if ret and self._after_insert:
             for f in self._after_insert:
                 f(row, ret)
         return ret
 
-    def _validate_fields(self, fields, defattr="default", id=None):
+    def _validate_fields(self, fields, record=None):
         from .validators import CRYPT
-        valid_names = {f.name for f in self if f.writable and f.type != "id"}
-        response = {"id": None, "errors": {}}
-        new_fields = Row()
-        for name in set(fields) - valid_names:
-            response["errors"][name] = "invalid"
+        # if a field it not writable or is an id or does not exist or
+        # it is a computed field, than it is invalid
+        valid_names = {
+            f.name for f in self if
+            f.writable and
+            f.type != "id" and
+            not f.compute
+        }
+        errors = {}
+        new_fields = {}
+        for name in fields:
+            if name not in valid_names:
+                errors[name] = "invalid"
+        # loop over all expected fields
         for field in self:
-            # we validate even if not passed in case it is required
-            error = default = None
-            if field.name not in valid_names:
+            # the field already resulted in an error, skip it
+            if field.name in errors:
                 continue
-            if not field.required and not field.compute:
-                default = getattr(field, defattr)
-                if callable(default):
-                    default = default()
-            if not field.compute:
-                ovalue = fields.get(field.name, default)
-                value, error = field.validate(ovalue, id)
+            # if field is required but missing error
+            if record is None and field.required and not field.name in fields:
+                errors[field.name] = "required"
+                continue
+            # if we tried to submit **** as a password, ignore it (perhaps should be error)
+            if field.type == "password" and fields[field.name] == CRYPT.STARS:
+                continue
+            # if the field has a value use it
+            if field.name in fields:
+                id = record and record.id
+                value, error = field.validate(fields[field.name], record_id=id)
+            # this is an insert and no  value use the default value
+            elif not record and field.default:
+                value, error = field.default, None
+            # this is an update and no value use it
+            elif record and field.update:
+                value, error = field.update, None
+            else:
+                continue
+            # if error, record it
             if error:
-                response["errors"][field.name] = "%s" % error
-            elif field.type == "password" and ovalue == CRYPT.STARS:
-                pass
-            elif field.name in fields:
+                errors[field.name] = "%s" % error
+            # if no error and password
+            else:
+                # value can be a function if coming from default of update
+                if callable(value):
+                    value = value()
                 # only write if the field was passed and no error
                 new_fields[field.name] = value        
-        return response, new_fields
+        return errors, new_fields
 
     def validate_and_insert(self, **fields):
-        response, new_fields = self._validate_fields(fields, "default")
-        if not response.get("errors"):
-            response["id"] = self.insert(**new_fields)
-        return response
+        errors, new_fields = self._validate_fields(fields)
+        record_id = self.insert(**new_fields) if not errors else None
+        return {"id": record_id, "errors": errors}
 
     def validate_and_update(self, _key, **fields):
         record = self(**_key) if isinstance(_key, dict) else self(_key)
-        response, new_fields = self._validate_fields(fields, "update", record.id)
-        #: do the update
-        if not response.get("errors") and record:
+        errors, new_fields = self._validate_fields(fields, record)
+        updated = None
+        if not errors and record:
             if "_id" in self:
                 myset = self._db(self._id == record[self._id.name])
             else:
                 query = None
                 for key, value in iteritems(_key):
                     if query is None:
                         query = getattr(self, key) == value
                     else:
                         query = query & (getattr(self, key) == value)
                 myset = self._db(query)
-            response["updated"] = myset.update(**new_fields)
-        if record:
-            response["id"] = record.id
-        return response
+            updated = myset.update(**new_fields)
+        return {"id": record and record.id, "updated": updated, "errors": errors}
 
     def update_or_insert(self, _key=DEFAULT, **values):
         if _key is DEFAULT:
             record = self(**values)
         elif isinstance(_key, dict):
             record = self(**_key)
         else:
@@ -2803,33 +2823,32 @@
         row = table._fields_and_values_for_update(update_fields)
         if not row._values:
             raise ValueError("No fields to update")
         ret = self.db._adapter.update(table, self.query, row.op_values())
         return ret
 
     def validate_and_update(self, **update_fields):
+        response = {"updated": 0, "errors": {}}
         table = self.db._adapter.get_table(self.query)
-        response = {}
-        response["errors"] = {}
-        new_fields = copy.copy(update_fields)
-        for key, value in iteritems(update_fields):
-            value, error = table[key].validate(value, update_fields.get("id"))
-            if error:
-                response["errors"][key] = "%s" % error
-            else:
-                new_fields[key] = value
-        if response["errors"]:
+        # use {} instead of None to make an empty record
+        # to that we use update values instead of default values
+        errors, new_fields = table._validate_fields(update_fields, {})
+        if errors:
             response["updated"] = 0
+            response["errors"] = errors
         else:
+            print(new_fields)
             row = table._fields_and_values_for_update(new_fields)
+            print(row)
             if not row._values:
                 raise ValueError("No fields to update")
             if any(f(self, row) for f in table._before_update):
                 ret = 0
             else:
+                print(row.op_values())
                 ret = self.db._adapter.update(table, self.query, row.op_values())
                 ret and [f(self, row) for f in table._after_update]
             response["updated"] = ret
         return response
 
 
 class LazyReferenceGetter(object):
```

### Comparing `pydal-20240427.3/pydal/parsers/__init__.py` & `pydal-20240428.1/pydal/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/parsers/base.py` & `pydal-20240428.1/pydal/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/parsers/mongo.py` & `pydal-20240428.1/pydal/parsers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/parsers/oracle.py` & `pydal-20240428.1/pydal/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/parsers/postgre.py` & `pydal-20240428.1/pydal/parsers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/parsers/sqlite.py` & `pydal-20240428.1/pydal/parsers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/__init__.py` & `pydal-20240428.1/pydal/representers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/base.py` & `pydal-20240428.1/pydal/representers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/couchdb.py` & `pydal-20240428.1/pydal/representers/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/db2.py` & `pydal-20240428.1/pydal/representers/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/google.py` & `pydal-20240428.1/pydal/representers/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/informix.py` & `pydal-20240428.1/pydal/representers/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/mongo.py` & `pydal-20240428.1/pydal/representers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/mssql.py` & `pydal-20240428.1/pydal/representers/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/oracle.py` & `pydal-20240428.1/pydal/representers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/postgre.py` & `pydal-20240428.1/pydal/representers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/representers/sqlite.py` & `pydal-20240428.1/pydal/representers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/restapi.py` & `pydal-20240428.1/pydal/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/tools/tags.py` & `pydal-20240428.1/pydal/tools/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/utils.py` & `pydal-20240428.1/pydal/utils.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal/validators.py` & `pydal-20240428.1/pydal/validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pydal.egg-info/PKG-INFO` & `pydal-20240428.1/pydal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.3
+Version: 20240428.1
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.3/pydal.egg-info/SOURCES.txt` & `pydal-20240428.1/pydal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/pyproject.toml` & `pydal-20240428.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydal"
-version = "20240427.3"
+version = "20240428.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = 'pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pydal-20240427.3/tests/__pycache__/__init__.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/_adapt.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/_adapt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/_helpers.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/base.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/caching.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/caching.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/contribs.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/contribs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/indexes.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/is_url_validators.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/is_url_validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/restapi.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/restapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/smart_query.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/smart_query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/sql.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/sql.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/tags.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/validation.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/validation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/__pycache__/validators.cpython-311.pyc` & `pydal-20240428.1/tests/__pycache__/validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/_adapt.py` & `pydal-20240428.1/tests/_adapt.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/_helpers.py` & `pydal-20240428.1/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/base.py` & `pydal-20240428.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/caching.py` & `pydal-20240428.1/tests/caching.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/contribs.py` & `pydal-20240428.1/tests/contribs.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/indexes.py` & `pydal-20240428.1/tests/indexes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/is_url_validators.py` & `pydal-20240428.1/tests/is_url_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/nosql.py` & `pydal-20240428.1/tests/nosql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/restapi.py` & `pydal-20240428.1/tests/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/smart_query.py` & `pydal-20240428.1/tests/smart_query.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/sql.py` & `pydal-20240428.1/tests/sql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/tags.py` & `pydal-20240428.1/tests/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/validation.py` & `pydal-20240428.1/tests/validation.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.3/tests/validators.py` & `pydal-20240428.1/tests/validators.py`

 * *Files identical despite different names*

