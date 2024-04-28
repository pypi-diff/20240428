# Comparing `tmp/fpx-0.6.1.tar.gz` & `tmp/fpx-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpx-0.6.1.tar", last modified: Mon Apr  1 02:08:36 2024, max compression
+gzip compressed data, was "fpx-0.6.2.tar", last modified: Sun Apr 28 12:53:37 2024, max compression
```

## Comparing `fpx-0.6.1.tar` & `fpx-0.6.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.402815 fpx-0.6.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2024-01-31 12:30:34.000000 fpx-0.6.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9392 2024-04-01 02:08:36.399482 fpx-0.6.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7952 2024-01-31 12:30:34.000000 fpx-0.6.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       96 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/__main__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2012 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1346 2024-03-31 23:13:12.000000 fpx-0.6.1/fpx/app.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/cli/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      333 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/cli/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/cli/client.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/cli/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      161 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/cli/server.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      759 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/cli/ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1567 2024-03-31 23:37:16.000000 fpx-0.6.1/fpx/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      707 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/context.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      177 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/debug_app.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1352 2024-04-01 00:39:46.000000 fpx-0.6.1/fpx/exception.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1244 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/middleware.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/migrations/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       39 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/README
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/migrations/__pycache__/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1670 2024-01-31 12:43:07.000000 fpx-0.6.1/fpx/migrations/__pycache__/env.cpython-39.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2029 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/migrations/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      512 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/versions/6a22a6995723_create_clients_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/migrations/versions/__pycache__/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      826 2024-01-31 12:43:07.000000 fpx-0.6.1/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-39.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)      862 2024-01-31 12:43:07.000000 fpx-0.6.1/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-39.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1023 2024-01-31 12:43:07.000000 fpx-0.6.1/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-39.pyc
--rw-r--r--   0 sergey    (1000) sergey    (1000)      514 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      805 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1996 2024-03-31 23:58:30.000000 fpx-0.6.1/fpx/model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6577 2024-04-01 00:07:12.000000 fpx-0.6.1/fpx/pipes.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/route/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/route/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1705 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/route/stream.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4509 2024-03-31 22:19:35.000000 fpx-0.6.1/fpx/route/ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2561 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3142 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx/tests/route/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/route/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1406 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/route/test_stream.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7910 2024-03-31 22:26:04.000000 fpx-0.6.1/fpx/tests/route/test_ticket.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       26 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/settings.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      754 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/test_model.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2024-04-01 01:55:56.000000 fpx-0.6.1/fpx/tests/test_transport.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8100 2024-04-01 02:07:50.000000 fpx-0.6.1/fpx/transport.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      437 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      631 2024-01-31 12:30:34.000000 fpx-0.6.1/fpx/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 02:08:36.399482 fpx-0.6.1/fpx.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9392 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1437 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       36 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        4 2024-04-01 02:08:36.000000 fpx-0.6.1/fpx.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4255 2024-01-31 12:30:34.000000 fpx-0.6.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1163 2024-04-01 02:08:36.402815 fpx-0.6.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-01-31 12:30:34.000000 fpx-0.6.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.392537 fpx-0.6.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2024-01-31 12:30:34.000000 fpx-0.6.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9422 2024-04-28 12:53:37.392537 fpx-0.6.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7952 2024-01-31 12:30:34.000000 fpx-0.6.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       96 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/__main__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2012 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1346 2024-03-31 23:13:12.000000 fpx-0.6.2/fpx/app.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/cli/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      333 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/cli/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/cli/client.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/cli/db.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      161 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/cli/server.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      759 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/cli/ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1567 2024-03-31 23:37:16.000000 fpx-0.6.2/fpx/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      707 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/context.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      177 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/debug_app.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1352 2024-04-01 00:39:46.000000 fpx-0.6.2/fpx/exception.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1244 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/middleware.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/migrations/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       39 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/README
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/migrations/__pycache__/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1670 2024-01-31 12:43:07.000000 fpx-0.6.2/fpx/migrations/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2029 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/migrations/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      512 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/versions/6a22a6995723_create_clients_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.389204 fpx-0.6.2/fpx/migrations/versions/__pycache__/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      826 2024-01-31 12:43:07.000000 fpx-0.6.2/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-39.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      862 2024-01-31 12:43:07.000000 fpx-0.6.2/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-39.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1023 2024-01-31 12:43:07.000000 fpx-0.6.2/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-39.pyc
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      514 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      805 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1996 2024-03-31 23:58:30.000000 fpx-0.6.2/fpx/model.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6577 2024-04-01 00:07:12.000000 fpx-0.6.2/fpx/pipes.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.392537 fpx-0.6.2/fpx/route/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/route/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1705 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/route/stream.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4509 2024-03-31 22:19:35.000000 fpx-0.6.2/fpx/route/ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2561 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.392537 fpx-0.6.2/fpx/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3142 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.392537 fpx-0.6.2/fpx/tests/route/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/route/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1406 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/route/test_stream.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7910 2024-03-31 22:26:04.000000 fpx-0.6.2/fpx/tests/route/test_ticket.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       26 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/settings.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      754 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/test_model.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2024-04-01 01:55:56.000000 fpx-0.6.2/fpx/tests/test_transport.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8100 2024-04-01 02:07:50.000000 fpx-0.6.2/fpx/transport.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      437 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      631 2024-01-31 12:30:34.000000 fpx-0.6.2/fpx/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-28 12:53:37.392537 fpx-0.6.2/fpx.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9422 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1437 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       36 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      374 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        4 2024-04-28 12:53:37.000000 fpx-0.6.2/fpx.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4255 2024-01-31 12:30:34.000000 fpx-0.6.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1179 2024-04-28 12:53:37.395870 fpx-0.6.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-01-31 12:30:34.000000 fpx-0.6.2/setup.py
```

### Comparing `fpx-0.6.1/PKG-INFO` & `fpx-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpx
-Version: 0.6.1
+Version: 0.6.2
 Summary: Stream archiver/proxy
 Home-page: https://github.com/DataShades/fpx
 Author: Sergey Motornyuk
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: alembic~=1.12.0
 Requires-Dist: asyncblink==0.3.2
+Requires-Dist: blinker==1.7.0
 Requires-Dist: click
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: pyjwt
 Requires-Dist: sanic~=23.12.0
 Requires-Dist: sanic_ext~=23.12.0
 Requires-Dist: sqlalchemy~=2.0.22
 Requires-Dist: typing-extensions
```

### Comparing `fpx-0.6.1/README.md` & `fpx-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/alembic.ini` & `fpx-0.6.2/fpx/alembic.ini`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/app.py` & `fpx-0.6.2/fpx/app.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/cli/client.py` & `fpx-0.6.2/fpx/cli/client.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/cli/db.py` & `fpx-0.6.2/fpx/cli/db.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/cli/ticket.py` & `fpx-0.6.2/fpx/cli/ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/config.py` & `fpx-0.6.2/fpx/config.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/context.py` & `fpx-0.6.2/fpx/context.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/exception.py` & `fpx-0.6.2/fpx/exception.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/middleware.py` & `fpx-0.6.2/fpx/middleware.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/__pycache__/env.cpython-39.pyc` & `fpx-0.6.2/fpx/migrations/__pycache__/env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/env.py` & `fpx-0.6.2/fpx/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/6a22a6995723_create_clients_table.py` & `fpx-0.6.2/fpx/migrations/versions/6a22a6995723_create_clients_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-39.pyc` & `fpx-0.6.2/fpx/migrations/versions/__pycache__/6a22a6995723_create_clients_table.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-39.pyc` & `fpx-0.6.2/fpx/migrations/versions/__pycache__/ac8a8750d3e2_add_options_column_to_ticket_table.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-39.pyc` & `fpx-0.6.2/fpx/migrations/versions/__pycache__/ef515c12c8ff_create_tickets_table.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py` & `fpx-0.6.2/fpx/migrations/versions/ac8a8750d3e2_add_options_column_to_ticket_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py` & `fpx-0.6.2/fpx/migrations/versions/ef515c12c8ff_create_tickets_table.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/model.py` & `fpx-0.6.2/fpx/model.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/pipes.py` & `fpx-0.6.2/fpx/pipes.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/route/stream.py` & `fpx-0.6.2/fpx/route/stream.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/route/ticket.py` & `fpx-0.6.2/fpx/route/ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/schema.py` & `fpx-0.6.2/fpx/schema.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/tests/conftest.py` & `fpx-0.6.2/fpx/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/tests/route/test_stream.py` & `fpx-0.6.2/fpx/tests/route/test_stream.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/tests/route/test_ticket.py` & `fpx-0.6.2/fpx/tests/route/test_ticket.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/tests/test_model.py` & `fpx-0.6.2/fpx/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/tests/test_transport.py` & `fpx-0.6.2/fpx/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/transport.py` & `fpx-0.6.2/fpx/transport.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx/utils.py` & `fpx-0.6.2/fpx/utils.py`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/fpx.egg-info/PKG-INFO` & `fpx-0.6.2/fpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpx
-Version: 0.6.1
+Version: 0.6.2
 Summary: Stream archiver/proxy
 Home-page: https://github.com/DataShades/fpx
 Author: Sergey Motornyuk
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: alembic~=1.12.0
 Requires-Dist: asyncblink==0.3.2
+Requires-Dist: blinker==1.7.0
 Requires-Dist: click
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: pyjwt
 Requires-Dist: sanic~=23.12.0
 Requires-Dist: sanic_ext~=23.12.0
 Requires-Dist: sqlalchemy~=2.0.22
 Requires-Dist: typing-extensions
```

### Comparing `fpx-0.6.1/fpx.egg-info/SOURCES.txt` & `fpx-0.6.2/fpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/pyproject.toml` & `fpx-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fpx-0.6.1/setup.cfg` & `fpx-0.6.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fpx
-version = 0.6.1
+version = 0.6.2
 description = Stream archiver/proxy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sergey Motornyuk
 url = https://github.com/DataShades/fpx
 license = AGPL
 classifiers = 
@@ -18,14 +18,15 @@
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	aiohttp[speedups]~=3.8.6
 	alembic~=1.12.0
 	asyncblink==0.3.2
+	blinker==1.7.0
 	click
 	httpx~=0.23.0
 	pyjwt
 	sanic~=23.12.0
 	sanic_ext~=23.12.0
 	sqlalchemy~=2.0.22
 	typing-extensions
```

