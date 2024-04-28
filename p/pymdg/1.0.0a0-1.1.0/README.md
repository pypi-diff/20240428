# Comparing `tmp/pymdg-1.0.0a0.tar.gz` & `tmp/pymdg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymdg-1.0.0a0.tar", last modified: Mon Feb 19 09:15:41 2024, max compression
+gzip compressed data, was "pymdg-1.1.0.tar", last modified: Sun Apr 28 21:01:24 2024, max compression
```

## Comparing `pymdg-1.0.0a0.tar` & `pymdg-1.1.0.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/generate/
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/generate/confluence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/confluence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/confluence/content_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/confluence/image_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/confluence/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/generate/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/parse/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/bouml_xmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/drawio_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/erwin_xmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/sparx_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/sparx_db_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    21487 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/parse/sparx_xmi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/templates/Arango/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Arango/models.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.881535 pymdg-1.0.0a0/mdg/templates/Django/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/Django/.azure/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/.azure/config.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/.azure/setup.ps1.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/Django/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/admin.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/apps.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/serializers.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/urls.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/app/views.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/manage.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/Django/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/asgi.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/settings.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/urls.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/validators.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/project/wsgi.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Django/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/Java/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Java/entities.jdl.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Java/enums.java.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Java/pojos.java.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/SQLAlchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/SQLAlchemy/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/SQLAlchemy/schemas.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.885535 pymdg-1.0.0a0/mdg/templates/Schema/
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Schema/avro.avsc.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/Schema/openapi.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/base.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/hasura.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/templates/postgresql.sql.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/mdg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_uml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tests/test_xmi_model_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/mdg/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/DrawIO MDG UML Library.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/mdg_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    46970 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/tools/sparx_db_models_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/mdg/uml/
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/uml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/mdg/uml/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:15:41.889535 pymdg-1.0.0a0/pymdg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-19 09:15:41.000000 pymdg-1.0.0a0/pymdg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 09:15:41.893535 pymdg-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-19 09:15:30.000000 pymdg-1.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.637621 pymdg-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-28 21:01:21.000000 pymdg-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 21:01:21.000000 pymdg-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-28 21:01:24.637621 pymdg-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-28 21:01:21.000000 pymdg-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/generate/confluence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/content_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/image_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/bouml_xmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/drawio_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/erwin_xmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21487 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_xmi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Arango/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Arango/models.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/.azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/.azure/config.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/.azure/setup.ps1.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/admin.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/apps.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/serializers.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/urls.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/views.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/manage.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/asgi.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/settings.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/urls.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/validators.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/wsgi.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/Java/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/entities.jdl.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/enums.java.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/pojos.java.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/SQLAlchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/SQLAlchemy/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/SQLAlchemy/schemas.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/Schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Schema/avro.avsc.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Schema/openapi.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/base.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/hasura-abac.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/hasura.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/postgresql.sql.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_uml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_xmi_model_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/DrawIO MDG UML Library.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/mdg_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46970 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/sparx_db_models_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/uml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/uml/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.637621 pymdg-1.1.0/pymdg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 21:01:21.000000 pymdg-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:01:24.637621 pymdg-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-28 21:01:21.000000 pymdg-1.1.0/setup.py
```

### Comparing `pymdg-1.0.0a0/LICENSE` & `pymdg-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/PKG-INFO` & `pymdg-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymdg
-Version: 1.0.0a0
+Version: 1.1.0
 Summary: Model driven genration - from UML to Code & Docs
 Home-page: https://github.com/semprini/pyMDG
 Author: Semprini
 Author-email: dont@contact.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -44,14 +44,17 @@
  > python mdg-tool.py generate ./sample_recipe/drawio/config-drawio-django.yaml
 
 Or once installed into site-packages execute:
  > mdg-tool generate <my/config.yaml>
 
 See the sample_recipe configs for examples
 
+## Limitations
+Most templates have a limit of single inheritance and no chained inheritance (a is a specialisation of b which is a specialisation of c). The results of this are unknown.
+
 ## Sparx EA XMI (versions earlier than V16) Export Process
 The UML parser expects a specific package hierarchy, please see the sample EA file.
 - In Sparx select the domain root node  (e.g. Model/Sample )
 - Select the publish tab at the top
 - Select Publish As... from top menu
 - Set export type as XMI 2.1
 - Optionally select 'Export Diagrams', 'Generate Diagram Images' and PNG format
```

### Comparing `pymdg-1.0.0a0/README.md` & `pymdg-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
  > python mdg-tool.py generate ./sample_recipe/drawio/config-drawio-django.yaml
 
 Or once installed into site-packages execute:
  > mdg-tool generate <my/config.yaml>
 
 See the sample_recipe configs for examples
 
+## Limitations
+Most templates have a limit of single inheritance and no chained inheritance (a is a specialisation of b which is a specialisation of c). The results of this are unknown.
+
 ## Sparx EA XMI (versions earlier than V16) Export Process
 The UML parser expects a specific package hierarchy, please see the sample EA file.
 - In Sparx select the domain root node  (e.g. Model/Sample )
 - Select the publish tab at the top
 - Select Publish As... from top menu
 - Set export type as XMI 2.1
 - Optionally select 'Export Diagrams', 'Generate Diagram Images' and PNG format
```

### Comparing `pymdg-1.0.0a0/mdg/__init__.py` & `pymdg-1.1.0/mdg/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/config.py` & `pymdg-1.1.0/mdg/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 generation_artifacts: List[Dict] = []
 
 defaults: Dict = {
     "default_dialect": "default",
     "root_package": "default",
     "generation_artifacts": generation_artifacts,
-    "case_package": "CamelCase",
-    "case_class": "CamelCase",
+    "case_package": "PascalCase",
+    "case_class": "PascalCase",
     "case_attribute": "snake_case",
     "parser": None,
     "use_alias": True,
+    "default_string_length": 50,
 }
 
 
 def load():
     config_filename = os.environ.get('PYMDG_SETTINGS_MODULE', "")
     try:
         with open(config_filename, 'r') as config_file:
```

### Comparing `pymdg-1.0.0a0/mdg/generate/__init__.py` & `pymdg-1.1.0/mdg/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/generate/confluence/content_update.py` & `pymdg-1.1.0/mdg/generate/confluence/content_update.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/generate/confluence/image_update.py` & `pymdg-1.1.0/mdg/generate/confluence/image_update.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/generate/confluence/util.py` & `pymdg-1.1.0/mdg/generate/confluence/util.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/generate/render.py` & `pymdg-1.1.0/mdg/generate/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python
-import json
 import os
 import logging
 from typing import Dict, Optional, List, Any
+import json
+import yaml
 
 from jinja2 import Environment, FileSystemLoader, Template, BaseLoader
 from jinja2.exceptions import TemplateNotFound
 
 from mdg.config import settings
 from mdg.tools.filters import get_filters
 
@@ -189,28 +190,32 @@
 
     logger.info("Generating test case output")
     filters = get_filters()
     env = Environment(loader=BaseLoader())
     env.filters = {**env.filters, **filters}
 
     for case in test_cases:
-        serialised = json.dumps(serialize_instance(case), indent=2)
+        serialised_json = json.dumps(serialize_instance(case), indent=2)
+        serialised_yaml = yaml.dump(serialize_instance(case), Dumper=yaml.CDumper)
 
         template_definition: Dict
         for template_definition in settings['test_templates']:
             filename_template: Template = env.from_string(template_definition['dest'])
             filename: str = os.path.abspath(filename_template.render(ins=case))
             dirname: str = os.path.dirname(filename)
 
             # make sure computed distination path exists
             if not os.path.exists(dirname):
                 os.makedirs(dirname)
 
             with open(filename, 'w') as fh:
-                fh.write(serialised)
+                if filename[-4:] in ['yaml', '.yml']:
+                    fh.write(serialised_yaml)
+                else:
+                    fh.write(serialised_json)
 
 
 def serialize_instance(instance: UMLInstance):
     """ Generates a dictionary of attributes, values, dicts and lists from UML instance
         Recurses through associations originaing from supplied instance to serialise sub-objects
     """
     ret: Dict = {}
```

### Comparing `pymdg-1.0.0a0/mdg/parse/__init__.py` & `pymdg-1.1.0/mdg/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/bouml_xmi.py` & `pymdg-1.1.0/mdg/parse/bouml_xmi.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/drawio_xml.py` & `pymdg-1.1.0/mdg/parse/drawio_xml.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/erwin_xmi.py` & `pymdg-1.1.0/mdg/parse/erwin_xmi.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/sparx_db.py` & `pymdg-1.1.0/mdg/parse/sparx_db.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/sparx_db_models.py` & `pymdg-1.1.0/mdg/parse/sparx_db_models.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/parse/sparx_xmi.py` & `pymdg-1.1.0/mdg/parse/sparx_xmi.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Arango/models.py.jinja` & `pymdg-1.1.0/mdg/templates/Arango/models.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/.azure/setup.ps1.jinja` & `pymdg-1.1.0/mdg/templates/Django/.azure/setup.ps1.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/admin.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/admin.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/apps.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/apps.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/models.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/models.py.jinja`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from django.utils.translation import gettext_lazy as _
 from django.db import models
 
 {% for cls in package.classes %}{% if cls.generalization != None %}{% if cls.generalization.package != package %}
 from {{ cls.generalization.package.name | case_package }}.models import {{ cls.generalization.name | case_class }}{% endif %}{% endif %}{% endfor %}
 
-{% for enum in package.enumerations %}class ENUM_{{ enum.name | case_class }}(models.TextChoices):
-{% for attr in enum.values %}
+{% for enum in package.enumerations %}class ENUM_{{ enum.name | case_class }}(models.TextChoices):{% for attr in enum.values %}
     {{ attr.upper() }} = '{{ attr }}', _('{{ attr }}'){% endfor %}
-{% endfor %}
-{% for cls in package.classes %}{% if cls.is_abstract %}class {{ cls.name | case_class }}( models.Model ):
-{% for attr in cls.attributes %}
-{% if attr.classification %}    {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name}}.choices, blank=True, null=True )
-{% else %}    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %} )
+
+{% endfor %}{% for cls in package.classes %}{% if cls.is_abstract %}class {{ cls.name | case_class }}( models.Model ):{% for attr in cls.attributes %}{% if attr.classification %}
+    {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name}}.choices, blank=True, null=True ){% else %}
+    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %} )
 {% endif %}{% endfor %}
     class Meta:
         abstract = True
 {% endif %}{% endfor %}
 
-{% for cls in package.classes %}{% if not cls.is_abstract %}class {{ cls.name | case_class }}( {% if cls.generalization %}{{ cls.generalization.name }}{% else %}models.Model{% endif %} ):
-{% for attr in cls.attributes %}
-{% if attr.classification %}    {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name | case_class }}.choices, blank=True, null=True )
-{% else %}    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
-{% endif %}{% endfor %}
+{% for cls in package.classes %}{% if not cls.is_abstract and cls.specialized_by | length > 0 %}class {{ cls.name | case_class }}( {% if cls.generalization %}{{ cls.generalization.name | case_class }}{% else %}models.Model{% endif %} ):{% for attr in cls.attributes %}{% if attr.classification %}
+    {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name | case_class }}.choices, blank=True, null=True ){% else %}
+    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
+{% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if rel.association_type.name == "ASSOCIATION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_MANY" %}
+    {{ rel.destination_name | snakecase }} = models.ManyToManyField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', blank=True ){% endif %}{% elif rel.association_type.name == "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% else %}
+    {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% endif %}
+{% endif %}{% endfor %}{% for rel in cls.associations_to %}{% if rel.association_type.name != "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_MANY" %}
+    {{ rel.source_name | snakecase }} = models.ForeignKey( '{{ rel.source.package.name | case_package }}.{{ rel.source.name | case_class }}', on_delete=models.CASCADE, related_name='{{ rel.destination_name | snakecase }}', blank=True, null=True ){% endif %}
+{% endif %}{% endfor %}{% endif %}
 
-{% for rel in cls.associations_from %}{% if rel.association_type.name == "ASSOCIATION" %}
-    {% if rel.cardinality.name == "ONE_TO_ONE" %}{{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', on_delete=models.CASCADE, blank=True, null=True )
-    {% elif rel.cardinality.name == "MANY_TO_ONE" %}{{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE, blank=True, null=True )
-    {% elif rel.cardinality.name == "MANY_TO_MANY" %}{{ rel.destination_name | snakecase }} = models.ManyToManyField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', blank=True ){% endif %}
-{% elif rel.association_type.name == "COMPOSITION" %}
-    {% if rel.cardinality.name == "ONE_TO_ONE" %}{{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE )
-    {% else %}{{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% endif %}
-{% endif %}{% endfor %}
-{% for rel in cls.associations_to %}{% if rel.association_type.name != "COMPOSITION" %}
-    {% if rel.cardinality.name == "ONE_TO_MANY" %}{{ rel.source_name | snakecase }} = models.ForeignKey( '{{ rel.source.package.name | case_package }}.{{ rel.source.name | case_class }}', on_delete=models.CASCADE, related_name='{{ rel.destination_name | snakecase }}', blank=True, null=True ){% endif %}
-{% endif %}{% endfor %}
-
-{% if 'auditable' in cls.stereotypes %}
-    history = HistoricalRecords(){% endif%}
+{% endfor %}
+{% for cls in package.classes %}{% if not cls.is_abstract and cls.specialized_by | length == 0 %}class {{ cls.name | case_class }}( {% if cls.generalization %}{{ cls.generalization.name | case_class }}{% else %}models.Model{% endif %} ):{% for attr in cls.attributes %}{% if attr.classification %}
+    {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name | case_class }}.choices, blank=True, null=True ){% else %}
+    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
+{% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if rel.association_type.name == "ASSOCIATION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_MANY" %}
+    {{ rel.destination_name | snakecase }} = models.ManyToManyField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', blank=True ){% endif %}{% elif rel.association_type.name == "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
+    {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% else %}
+    {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% endif %}
+{% endif %}{% endfor %}{% for rel in cls.associations_to %}{% if rel.association_type.name != "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_MANY" %}
+    {{ rel.source_name | snakecase }} = models.ForeignKey( '{{ rel.source.package.name | case_package }}.{{ rel.source.name | case_class }}', on_delete=models.CASCADE, related_name='{{ rel.destination_name | snakecase }}', blank=True, null=True ){% endif %}
+{% endif %}{% endfor %}{% endif %}
 
-{% endif %}{% endfor %}
+{% endfor %}
```

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/serializers.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/serializers.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/urls.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/urls.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/app/views.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/app/views.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/manage.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/project/settings.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/project/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Django/project/urls.py.jinja` & `pymdg-1.1.0/mdg/templates/Django/project/urls.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Java/entities.jdl.jinja` & `pymdg-1.1.0/mdg/templates/Java/entities.jdl.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Java/pojos.java.jinja` & `pymdg-1.1.0/mdg/templates/Java/pojos.java.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/SQLAlchemy/models.py.jinja` & `pymdg-1.1.0/mdg/templates/SQLAlchemy/models.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/SQLAlchemy/schemas.py.jinja` & `pymdg-1.1.0/mdg/templates/SQLAlchemy/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/Schema/avro.avsc.jinja` & `pymdg-1.1.0/mdg/templates/Schema/avro.avsc.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,149 @@
 [
-{% for assoc in cls.associations_to %}{% if assoc.association_type.name in ['AGGREGATION', 'COMPOSITION', 'ASSOCIATION'] %}
+{% for assoc in cls.associations_to %}{% if assoc.association_type.name in ['AGGREGATION', 'COMPOSITION', 'ASSOCIATION'] and "aggregate root" not in assoc.source.stereotypes %}
 	{
 		"namespace": "{{ assoc.source.package.path[1:-1] | replace("/",".") | snakecase }}",
 		"type": "record",
 		"name": "{{ assoc.source.name | case_class }}",
 		"fields": [{% if assoc.source.generalization %}{% for attr in assoc.source.generalization.attributes %}
 			{ 
 				"name": "{{ attr.name | case_attribute }}", 
-				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif attr.classification %}"type":
+				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif attr.classification %}"type":
 					{
 						"type": "enum",
-						"name": "{{ attr.classification.name | case_class }}",
+						"name": "{{ attr.classification.name | case_class }}", 
 						"symbols": [{% for enum in attr.classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_")}}",{% endfor %}
 							"{{ attr.classification.values[-1] | uppercase | replace(" ","_") }}"
 						]
-					}{% else %}"type": {% if not attr.is_id %}[ {% if attr.dest_type != 'string' %}"string",{% endif %}"null", {% endif %}"{{attr.dest_type}}"{% if not attr.is_id %} ], "default": "undefined"{% endif %}{% endif %}
+					}{% else %}"type": {% if not attr.is_id %}[ "string", "null"{% if attr.dest_type != 'string' %}, "{{attr.dest_type}}"{% endif %} ], "default": "__"{% else %}"{{attr.dest_type}}"{% endif %}{% endif %}
 			},{% endfor %}{% endif %}{% for attr in assoc.source.attributes[:-1] %}
 			{ 
 				"name": "{{ attr.name | case_attribute }}", 
-				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif attr.classification %}"type":
+				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif attr.classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ attr.classification.name | case_class }}",
 						"symbols": [{% for enum in attr.classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_") }}",{% endfor %}
 							"{{ attr.classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not attr.is_id %}[ {% if attr.dest_type != 'string' %}"string", {% endif %}"null",{% endif %}"{{attr.dest_type}}"{% if not attr.is_id %} ], "default": "undefined"{% endif %}{% endif %} 
+					}{% else %}"type": {% if not attr.is_id %}[ "string", "null"{% if attr.dest_type != 'string' %}, "{{attr.dest_type}}"{% endif %} ], "default": "__"{% else %}"{{attr.dest_type}}"{% endif %}{% endif %}
 			},{% endfor %}
 			{ 
 				"name": "{{ assoc.source.attributes[-1].name | case_attribute }}", 
-				{% if assoc.source.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif assoc.source.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif assoc.source.attributes[-1].classification %}"type":
+				{% if assoc.source.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif assoc.source.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif assoc.source.attributes[-1].classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ assoc.source.attributes[-1].classification.name | case_class }}",
 						"symbols": [{% for enum in assoc.source.attributes[-1].classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_") }}",{% endfor %}
 							"{{ assoc.source.attributes[-1].classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not assoc.source.attributes[-1].is_id %}[ {% if assoc.source.attributes[-1].dest_type != 'string' %}"string", {% endif %}"null", {% endif %}"{{assoc.source.attributes[-1].dest_type}}"{% if not assoc.source.attributes[-1].is_id %} ], "default": "undefined"{% endif %}{% endif %}
+					}{% else %}"type": {% if not assoc.source.attributes[-1].is_id %}[ "string", "null"{% if assoc.source.attributes[-1].dest_type != 'string' %}, "{{assoc.source.attributes[-1].dest_type}}"{% endif %} ], "default": "__"{% else %}"{{assoc.source.attributes[-1].dest_type}}"{% endif %}{% endif %}
 			}{% for assoc in assoc.source.associations_from %}{% if assoc.association_type.name not in ['AGGREGATION', 'COMPOSITION'] %}
 			,{ 
 				"name": "{{ assoc.destination_name | case_attribute }}_id", 
 				"type": ["string", "null"{% if assoc.destination_multiplicity[1] == '*' %}, 
 					{ 
 						"type": "array", 
 						"items": "string" 
-					}{% else %}], "default": "undefined"{% endif %} 
+					}{% else %}], "default": "__"{% endif %} 
 			}{% endif %}{% endfor %}
 		]
 	},{% endif %}{% endfor %}	
 	{
 		"namespace": "{{ cls.package.path[1:-1] | replace("/",".") | snakecase }}",
 		"type": "record",
 		"name": "{{ cls.name | case_class }}",
 		"fields": [{% if cls.generalization %}{% for attr in cls.generalization.attributes %}
 			{ 
 				"name": "{{ attr.name | case_attribute }}",
-				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif attr.classification %}"type":
+				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif attr.classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ attr.classification.name | case_class }}",
 						"symbols": [{% for enum in attr.classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_") }}",{% endfor %}
 							"{{ attr.classification.values[-1] | uppercase | replace(" ","_") }}"
 						]
-					}{% else %}"type": [{% if attr.dest_type!="string" %}"string", {% endif %}"{{attr.dest_type}}"{% if not attr.is_id %}, "null" ], "default": "undefined"{% else %}]{% endif %}{% endif %} 
+					}{% else %}"type": {% if not attr.is_id %}[ "string", "null"{% if attr.dest_type != 'string' %}, "{{attr.dest_type}}"{% endif %} ], "default": "__"{% else %}"{{attr.dest_type}}"{% endif %}{% endif %}
 			},{% endfor %}{% endif %}{% for attr in cls.attributes[:-1] %}
 			{ 
 				"name": "{{ attr.name | case_attribute }}",
-				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif attr.classification %}"type":
+				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif attr.classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ attr.classification.name | case_class }}",
 						"symbols": [{% for enum in attr.classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_")}}",{% endfor %}
 							"{{ attr.classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not attr.is_id %}[ {% if attr.dest_type != 'string' %}"string", {% endif %}{% endif %}"{{attr.dest_type}}"{% if not attr.is_id %},"null" ], "default": "undefined"{% endif %}{% endif %} 
+					}{% else %}"type": {% if not attr.is_id %}[ "string", "null"{% if attr.dest_type != 'string' %}, "{{attr.dest_type}}"{% endif %} ], "default": "__"{% else %}"{{attr.dest_type}}"{% endif %}{% endif %}
 			},{% endfor %}
 			{ 
 				"name": "{{ cls.attributes[-1].name | case_attribute }}",
-				{% if cls.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif cls.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif cls.attributes[-1].classification %}"type":
+				{% if cls.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif cls.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif cls.attributes[-1].classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ cls.attributes[-1].classification.name | case_class }}",
 						"symbols": [{% for enum in cls.attributes[-1].classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_") }}",{% endfor %}
 							"{{ cls.attributes[-1].classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not cls.attributes[-1].is_id %}[ {% if cls.attributes[-1].dest_type != 'string' %}"string", {% endif %}"null", {% endif %}"{{cls.attributes[-1].dest_type}}"{% if not cls.attributes[-1].is_id %} ], "default": "undefined"{% endif %}{% endif %}
+					}{% else %}"type": {% if not cls.attributes[-1].is_id %}[ "string", "null"{% if cls.attributes[-1].dest_type != 'string' %}, "{{cls.attributes[-1].dest_type}}"{% endif %} ], "default": "__"{% else %}"{{cls.attributes[-1].dest_type}}"{% endif %}{% endif %}
 			}{% for assoc in cls.associations_from %}
 			,{ 
 				"name": "{{ assoc.destination_name | case_attribute }}_id",
-				"type": [{% if assoc.destination_multiplicity[1] == '*' %}{ "type": "array", "items": "string" }{% else %}"string"{% endif %}, "null"], "default": "undefined"
+				"type": [{% if assoc.destination_multiplicity[1] == '*' %}{ "type": "array", "items": "string" }{% else %}"string"{% endif %}, "null"], "default": "__"
 			}{% endfor %}{% for assoc in cls.associations_to %}{% if assoc.association_type.name in ['AGGREGATION', 'COMPOSITION'] %}
 			,{ 
 				"name": "{{ assoc.source.name | case_attribute }}", 
 				"type": ["string", "null", {% if assoc.source_multiplicity[1] == '*' %}
 					{ 
 						"type": "array", 
 						"items": "{{ assoc.source.name | case_class }}" 
-					}{% else %}"{{ assoc.source.name | case_class }}"{% endif %}], "default": "undefined",
+					}{% else %}"{{ assoc.source.name | case_class }}"{% endif %}], "default": "__",
 				"namespace": "{{ cls.package.path[1:-1] | replace("/",".") | snakecase }}"
 			}{% endif %}{% endfor %}
 		]
-	}{% for special in cls.specialized_by %}{% if "root aggregate" not in special.stereotypes %},
+	}{% for special in cls.specialized_by %}{% if "aggregate root" not in special.stereotypes %},
 	{
 		"namespace": "{{ special.package.path[1:-1] | replace("/",".") | snakecase }}",
 		"type": "record",
 		"name": "{{ special.name | case_class }}",
 		"fields": [
 			{% for attr in special.attributes[:-1] %}{ 
 				"name": "{{ attr.name | case_attribute }}",
-				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif attr.classification %}"type":
+				{% if attr.dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif attr.dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif attr.classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ attr.classification.name | case_class }}",
 						"symbols": [{% for enum in attr.classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_")}}",{% endfor %}
 							"{{ attr.classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not attr.is_id %}[ {% if attr.dest_type != 'string' %}"string", {% endif %}{% endif %}"{{attr.dest_type}}"{% if not attr.is_id %},"null" ], "default": "undefined"{% endif %}{% endif %} 
+					}{% else %}"type": {% if not attr.is_id %}[ "string", "null"{% if attr.dest_type != 'string' %}, "{{attr.dest_type}}"{% endif %} ], "default": "__"{% else %}"{{attr.dest_type}}"{% endif %}{% endif %}
 			},{% endfor %}
 			{ 
 				"name": "{{ special.attributes[-1].name | case_attribute }}",
-				{% if special.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "undefined"
-				{% elif special.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "undefined"{% elif cls.attributes[-1].classification %}"type":
+				{% if special.attributes[-1].dest_type == "date" %}"type": ["string", "null", {"type": "int", "logicalType": "date"}], "default": "__"
+				{% elif special.attributes[-1].dest_type == "datetime" %}"type": ["string", "null", {"type" : "long", "logicalType": "timestamp-millis"}], "default": "__"{% elif cls.attributes[-1].classification %}"type":
 					{
 						"type": "enum",
 						"name": "{{ special.attributes[-1].classification.name | case_class }}",
 						"symbols": [{% for enum in special.attributes[-1].classification.values[:-1] %}
 							"{{ enum | uppercase | replace(" ","_") | replace("/","_") }}",{% endfor %}
 							"{{ special.attributes[-1].classification.values[-1] | uppercase | replace(" ","_")}}"
 						]
-					}{% else %}"type": {% if not special.attributes[-1].is_id %}[ {% if special.attributes[-1].dest_type != 'string' %}"string", {% endif %}"null", {% endif %}"{{special.attributes[-1].dest_type}}"{% if not special.attributes[-1].is_id %} ], "default": "undefined"{% endif %}{% endif %}
+					}{% else %}"type": {% if not special.attributes[-1].is_id %}[ "string", "null"{% if special.attributes[-1].dest_type != 'string' %}, "{{special.attributes[-1].dest_type}}"{% endif %} ], "default": "__"{% else %}"{{special.attributes[-1].dest_type}}"{% endif %}{% endif %}
 			}			
 		]
 	}{% endif %}{% endfor %}
 ]
```

### Comparing `pymdg-1.0.0a0/mdg/templates/Schema/openapi.yaml.jinja` & `pymdg-1.1.0/mdg/templates/Schema/openapi.yaml.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/hasura.json.jinja` & `pymdg-1.1.0/mdg/templates/hasura-abac.json.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/templates/postgresql.sql.jinja` & `pymdg-1.1.0/mdg/templates/postgresql.sql.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tests/test_dumps.py` & `pymdg-1.1.0/mdg/tests/test_dumps.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tests/test_instance.py` & `pymdg-1.1.0/mdg/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tests/test_sample.py` & `pymdg-1.1.0/mdg/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tests/test_uml_model.py` & `pymdg-1.1.0/mdg/tests/test_uml_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import unittest
 
 from mdg.uml import UMLClass, UMLPackage, UMLAssociation, Cardinality, UMLAssociationType, UMLAttribute, UMLEnumeration, SearchTypes
+from mdg.config import defaults
 
 
 class TestUMLModel(unittest.TestCase):
     def setUp(self):
         self.root_package = UMLPackage("1", "root")
         child = UMLPackage("2", "child1", self.root_package)
         self.root_package.children.append(child)
-        cls = UMLClass(child, "class1", "3")
-        child.classes.append(cls)
+        self.cls = UMLClass(child, "class1", "3")
+        child.classes.append(self.cls)
         cls = UMLClass(child, "class2", "4")
         child.classes.append(cls)
         enum = UMLEnumeration(child, "enum1", "4")
         child.enumerations.append(enum)
 
     def test_find_package(self):
         res = self.root_package.find_by_id("2")
+        assert res is not None
         self.assertEqual(UMLPackage, type(res))
         self.assertEqual("child1", res.name)
 
     def test_find_enumeration(self):
         # Check that we don't find the wrong thing
         res = self.root_package.find_by_id("3", SearchTypes.ENUM)
         self.assertEqual(None, res)
         # Check that we find the enum with the id=4, not the class with id=4
         res = self.root_package.find_by_id("4", SearchTypes.ENUM)
+        assert res is not None
         self.assertEqual(UMLEnumeration, type(res))
         self.assertEqual("enum1", res.name)
 
     def test_string_to_multiplicity(self):
         assoc = UMLAssociation(self.root_package, self.root_package.children[0].classes[0], self.root_package.children[0].classes[0], 1)
         self.assertEqual(assoc.string_to_multiplicity("0..1"), ("0", "1"))
         self.assertEqual(assoc.string_to_multiplicity("0..*"), ("0", "*"))
@@ -57,27 +60,28 @@
     def test_association_type(self):
         assoc = UMLAssociation(self.root_package, self.root_package.children[0].classes[0], self.root_package.children[0].classes[0], 1)
         self.assertEqual(assoc.association_type, UMLAssociationType.ASSOCIATION)
         assoc = UMLAssociation(self.root_package, self.root_package.children[0].classes[0], self.root_package.children[0].classes[0], 1, UMLAssociationType.COMPOSITION)
         self.assertEqual(assoc.association_type, UMLAssociationType.COMPOSITION)
 
     def test_attribute_type(self):
-        attr = UMLAttribute(None, "test", 123)
+        attr = UMLAttribute(self.cls, "test", 123)
         attr.set_type('String')
         self.assertEqual(attr.dest_type, 'CharField')
+        self.assertEqual(attr.length, defaults[ "default_string_length"])
         attr.set_type('String (123)')
         self.assertEqual(attr.dest_type, 'CharField')
         self.assertEqual(attr.length, 123)
         attr.set_type('decimal (12,2)')
         self.assertEqual(attr.dest_type, 'DecimalField')
         self.assertEqual(attr.precision, 12)
         self.assertEqual(attr.scale, 2)
 
     def test_attribute_get_type(self):
-        attr = UMLAttribute(None, "test", 123)
+        attr = UMLAttribute(self.cls, "test", 123)
         attr.set_type('String')
         self.assertEqual(attr.get_type('default'), 'string')
 
     def test_get_all_(self):
         self.assertEqual(len(self.root_package.get_all_classes()), 2)
         self.assertEqual(len(self.root_package.get_all_enums()), 1)
 
@@ -100,14 +104,15 @@
 
         # Create inheitance
         child.classes[1].generalization = child.classes[0]
         child.classes[0].specialized_by.append(child.classes[1])       # TODO: Setter function which does this linking
 
     def test_find_class(self):
         res = self.root_package.find_by_id("3", SearchTypes.CLASS)
+        assert res is not None
         self.assertEqual(UMLClass, type(res))
         self.assertEqual("class1", res.name)
 
     def test_get_all_attributes(self):
         # Grab class which inheits fom a class
         cls = self.root_package.children[0].classes[1]
         self.assertEqual("class2", cls.name)
```

### Comparing `pymdg-1.0.0a0/mdg/tests/test_xmi_model_parse.py` & `pymdg-1.1.0/mdg/tests/test_xmi_model_parse.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tools/DrawIO MDG UML Library.xml` & `pymdg-1.1.0/mdg/tools/DrawIO MDG UML Library.xml`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tools/case.py` & `pymdg-1.1.0/mdg/tools/case.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 String convert functions
 """
 
 from __future__ import annotations
 import re
 
 
-def camelcase(string):
+def camelcase(string:str) -> str:
     if string is None or string == "":
         return string
-    words = re.split(' |_', string)
-    return "".join(word[0].upper() + word[1:] for word in words)
+    words: list = re.split(' |_', string.strip(' _'))
+    
+    # Can't use Title function in str library as this lowers all but the first char: does not handle existing camelCased input
+    words_camel: list = [(words[0][0].lower() + words[0][1:])] + list(word[0].upper() + word[1:] for word in words[1:])
+    return "".join(words_camel)
 
 
 def capitalcase(string: str) -> str:
     """Convert string into capital case.
     First letters will be uppercase.
 
     Args:
@@ -67,15 +70,14 @@
     Args:
         string: String to convert.
 
     Returns:
         string: Pascal case string.
 
     """
-
     return capitalcase(camelcase(string))
 
 
 def pathcase(string: str) -> str:
     """Convert string into path case.
     Join punctuation with slash.
```

### Comparing `pymdg-1.0.0a0/mdg/tools/daemon.py` & `pymdg-1.1.0/mdg/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tools/filters.py` & `pymdg-1.1.0/mdg/tools/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from ..config import settings
-from .case import camelcase, snakecase, titlecase, sentencecase, uppercase
+from .case import camelcase, snakecase, titlecase, sentencecase, uppercase, pascalcase
 
 
 def get_filters():
     # Create jinja2 filter dict to pass into templates
     filters = {
         'camelcase': camelcase,
         'snakecase': snakecase,
         'titlecase': titlecase,
         'sentencecase': sentencecase,
         'uppercase': uppercase,
+        'pascalcase': pascalcase,
     }
 
     if settings['case_package'] == "CamelCase":
         filters['case_package'] = camelcase
     elif settings['case_package'] == "snake_case":
         filters['case_package'] = snakecase
+    elif settings['case_package'] == "PascalCase":
+        filters['case_package'] = pascalcase
     else:
         filters['case_package'] = camelcase
 
     if settings['case_class'] == "CamelCase":
         filters['case_class'] = camelcase
     elif settings['case_class'] == "snake_case":
         filters['case_class'] = snakecase
+    elif settings['case_class'] == "PascalCase":
+        filters['case_class'] = pascalcase
     else:
         filters['case_class'] = camelcase
 
     if settings['case_attribute'] == "CamelCase":
         filters['case_attribute'] = camelcase
     elif settings['case_attribute'] == "snake_case":
         filters['case_attribute'] = snakecase
+    elif settings['case_attribute'] == "PascalCase":
+        filters['case_attribute'] = pascalcase
     else:
         filters['case_class'] = snakecase
 
     return filters
```

### Comparing `pymdg-1.0.0a0/mdg/tools/io.py` & `pymdg-1.1.0/mdg/tools/io.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tools/mdg_tool.py` & `pymdg-1.1.0/mdg/tools/mdg_tool.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/tools/sparx_db_models_raw.py` & `pymdg-1.1.0/mdg/tools/sparx_db_models_raw.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/mdg/uml/__init__.py` & `pymdg-1.1.0/mdg/uml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,18 +333,18 @@
                 return assoc
         return None
 
     def get_array_relationships(self) -> list:
         """ Returns all related classes where this class is part of an array:
                 - associations from: many to one
                 - associations to: one to many
+                - specialisations
         """
         result = []
-        if self.generalization is not None:
-            result.append(self.generalization)
+        result += self.specialized_by
         for assoc in self.associations_from:
             if assoc.cardinality in [Cardinality.ONE_TO_MANY, Cardinality.ONE_TO_ONE, Cardinality.MANY_TO_MANY]:
                 result.append(assoc.destination)
         for assoc in self.associations_to:
             if assoc.cardinality in [Cardinality.MANY_TO_ONE, Cardinality.ONE_TO_ONE, Cardinality.MANY_TO_MANY]:
                 result.append(assoc.source)
 
@@ -353,14 +353,16 @@
     def get_object_relationships(self) -> list:
         """ Returns all related classes where this class is singular:
                 - associations from: one to one, one to many
                 - associations to: one to one, many to one
                 - generalization
         """
         result = []
+        if self.generalization is not None:
+            result.append(self.generalization)
         for assoc in self.associations_from:
             if assoc.cardinality == Cardinality.MANY_TO_ONE:
                 result.append(assoc.destination)
         for assoc in self.associations_to:
             if assoc.cardinality == Cardinality.ONE_TO_MANY:
                 result.append(assoc.source)
 
@@ -443,15 +445,15 @@
             attrs = split[1].split(',')
             if len(attrs) == 1:
                 self.length = int(attrs[0])
             elif len(attrs) == 2:
                 self.precision = int(attrs[0])
                 self.scale = int(attrs[1])
         elif source_type.lower() in ['string', 'str']:
-            self.length = 100
+            self.length = settings['default_string_length']
 
         self.type = source_type
         if source_type in generation_fields[settings['default_dialect']].keys():
             self.dest_type = generation_fields[settings['default_dialect']][source_type]
         else:
             self.dest_type = source_type
```

### Comparing `pymdg-1.0.0a0/mdg/uml/validate.py` & `pymdg-1.1.0/mdg/uml/validate.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.0.0a0/pymdg.egg-info/PKG-INFO` & `pymdg-1.1.0/pymdg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymdg
-Version: 1.0.0a0
+Version: 1.1.0
 Summary: Model driven genration - from UML to Code & Docs
 Home-page: https://github.com/semprini/pyMDG
 Author: Semprini
 Author-email: dont@contact.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -44,14 +44,17 @@
  > python mdg-tool.py generate ./sample_recipe/drawio/config-drawio-django.yaml
 
 Or once installed into site-packages execute:
  > mdg-tool generate <my/config.yaml>
 
 See the sample_recipe configs for examples
 
+## Limitations
+Most templates have a limit of single inheritance and no chained inheritance (a is a specialisation of b which is a specialisation of c). The results of this are unknown.
+
 ## Sparx EA XMI (versions earlier than V16) Export Process
 The UML parser expects a specific package hierarchy, please see the sample EA file.
 - In Sparx select the domain root node  (e.g. Model/Sample )
 - Select the publish tab at the top
 - Select Publish As... from top menu
 - Set export type as XMI 2.1
 - Optionally select 'Export Diagrams', 'Generate Diagram Images' and PNG format
```

### Comparing `pymdg-1.0.0a0/pymdg.egg-info/SOURCES.txt` & `pymdg-1.1.0/pymdg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 mdg/parse/bouml_xmi.py
 mdg/parse/drawio_xml.py
 mdg/parse/erwin_xmi.py
 mdg/parse/sparx_db.py
 mdg/parse/sparx_db_models.py
 mdg/parse/sparx_xmi.py
 mdg/templates/base.txt.jinja
+mdg/templates/hasura-abac.json.jinja
 mdg/templates/hasura.json.jinja
 mdg/templates/postgresql.sql.jinja
 mdg/templates/Arango/models.py.jinja
 mdg/templates/Django/manage.py.jinja
 mdg/templates/Django/requirements.txt.jinja
 mdg/templates/Django/.azure/config.jinja
 mdg/templates/Django/.azure/setup.ps1.jinja
```

### Comparing `pymdg-1.0.0a0/setup.py` & `pymdg-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='pymdg',
-    version='1.0.0-alpha',
+    version='1.1.0',
     author='Semprini',
     author_email='dont@contact.me',
     description='Model driven genration - from UML to Code & Docs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/semprini/pyMDG',
     packages=["mdg", ] + pymdg_packages,
```

