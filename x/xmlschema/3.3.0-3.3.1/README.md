# Comparing `tmp/xmlschema-3.3.0.tar.gz` & `tmp/xmlschema-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-3.3.0.tar", last modified: Wed Apr 17 17:34:43 2024, max compression
+gzip compressed data, was "xmlschema-3.3.1.tar", last modified: Sun Apr 28 08:22:28 2024, max compression
```

## Comparing `xmlschema-3.3.0.tar` & `xmlschema-3.3.1.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.723928 xmlschema-3.3.0/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.3.0/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28284 2024-04-17 17:34:18.000000 xmlschema-3.3.0/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-01-07 11:20:34.000000 xmlschema-3.3.0/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.3.0/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-17 17:34:43.723928 xmlschema-3.3.0/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-02-18 21:08:04.000000 xmlschema-3.3.0/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.570928 xmlschema-3.3.0/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.3.0/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11907 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.3.0/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-04-17 17:34:18.000000 xmlschema-3.3.0/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.3.0/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.3.0/doc/extras.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9946 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.3.0/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2024-04-08 08:13:09.000000 xmlschema-3.3.0/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-02-03 22:44:00.000000 xmlschema-3.3.0/doc/requirements.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.3.0/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31284 2024-03-25 21:28:10.000000 xmlschema-3.3.0/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.3.0/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.3.0/pyproject.toml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-03-13 05:27:13.000000 xmlschema-3.3.0/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-04-17 17:34:43.724928 xmlschema-3.3.0/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-04-17 17:34:18.000000 xmlschema-3.3.0/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.579928 xmlschema-3.3.0/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.3.0/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.541928 xmlschema-3.3.0/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.580928 xmlschema-3.3.0/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.582928 xmlschema-3.3.0/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.3.0/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.0/tests/templates/filters/wrong-template.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3576 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.582928 xmlschema-3.3.0/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.541928 xmlschema-3.3.0/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.586928 xmlschema-3.3.0/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-default.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-04-17 17:12:21.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.590928 xmlschema-3.3.0/tests/test_cases/examples/menù/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.591928 xmlschema-3.3.0/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.596928 xmlschema-3.3.0/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-redef.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.542928 xmlschema-3.3.0/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.597928 xmlschema-3.3.0/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.597928 xmlschema-3.3.0/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.599928 xmlschema-3.3.0/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.3.0/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.601928 xmlschema-3.3.0/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.602928 xmlschema-3.3.0/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.609928 xmlschema-3.3.0/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.3.0/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.3.0/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.618928 xmlschema-3.3.0/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/dynamic-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case7.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case8.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included6-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included7-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/features/namespaces/included8-redefine.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.619928 xmlschema-3.3.0/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.621928 xmlschema-3.3.0/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.552928 xmlschema-3.3.0/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.622928 xmlschema-3.3.0/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.622928 xmlschema-3.3.0/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.623928 xmlschema-3.3.0/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.624928 xmlschema-3.3.0/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.624928 xmlschema-3.3.0/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.625928 xmlschema-3.3.0/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.627928 xmlschema-3.3.0/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.628928 xmlschema-3.3.0/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.629928 xmlschema-3.3.0/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.630928 xmlschema-3.3.0/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.631928 xmlschema-3.3.0/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.632928 xmlschema-3.3.0/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.633928 xmlschema-3.3.0/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.634928 xmlschema-3.3.0/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.635928 xmlschema-3.3.0/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.636928 xmlschema-3.3.0/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.637928 xmlschema-3.3.0/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.637928 xmlschema-3.3.0/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.638928 xmlschema-3.3.0/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.641928 xmlschema-3.3.0/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.643928 xmlschema-3.3.0/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.643928 xmlschema-3.3.0/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.644928 xmlschema-3.3.0/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.645928 xmlschema-3.3.0/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.547928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.645928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.646928 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.647928 xmlschema-3.3.0/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.648928 xmlschema-3.3.0/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.648928 xmlschema-3.3.0/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.649928 xmlschema-3.3.0/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.650928 xmlschema-3.3.0/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.651928 xmlschema-3.3.0/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.651928 xmlschema-3.3.0/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.652928 xmlschema-3.3.0/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.653928 xmlschema-3.3.0/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.654928 xmlschema-3.3.0/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.655928 xmlschema-3.3.0/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.656928 xmlschema-3.3.0/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.657928 xmlschema-3.3.0/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.658928 xmlschema-3.3.0/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.659928 xmlschema-3.3.0/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.660928 xmlschema-3.3.0/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_349/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.661928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.662928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.662928 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_362/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.664928 xmlschema-3.3.0/tests/test_cases/issues/issue_363/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.665928 xmlschema-3.3.0/tests/test_cases/issues/issue_372/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.666928 xmlschema-3.3.0/tests/test_cases/issues/issue_386/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.667928 xmlschema-3.3.0/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.3.0/tests/test_cases/mypy/extra_validator.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_cases/mypy/protocols.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.3.0/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.3.0/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.669928 xmlschema-3.3.0/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/resources/dummy file.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.3.0/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.3.0/tests/test_cases/resources/with_entity.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.671928 xmlschema-3.3.0/tests/test_cases/serialization/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/abdera.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/badgerfish.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/document.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/jsonml.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_cases/serialization/parker.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6725 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/test_cases/testfiles
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.553928 xmlschema-3.3.0/tests/test_cases/translations/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.671928 xmlschema-3.3.0/tests/test_cases/translations/pl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.3.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-3.3.0/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16654 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_exports.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-3.3.0/tests/test_files.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30654 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19738 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/test_locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5738 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23506 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.3.0/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    58232 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/test_translations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-03-13 05:27:13.000000 xmlschema-3.3.0/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.3.0/tests/test_validation.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27292 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/test_w3c_suite.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2024-04-16 19:49:32.000000 xmlschema-3.3.0/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.677928 xmlschema-3.3.0/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.0/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79224 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/validation/test_decoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33245 2024-01-07 11:20:34.000000 xmlschema-3.3.0/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    29598 2024-04-14 19:45:21.000000 xmlschema-3.3.0/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.682928 xmlschema-3.3.0/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.0/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.3.0/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-02-18 21:08:04.000000 xmlschema-3.3.0/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.3.0/tests/validators/test_elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16509 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    63262 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.3.0/tests/validators/test_global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15868 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.3.0/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    55290 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.3.0/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    39368 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2024-03-23 21:43:51.000000 xmlschema-3.3.0/tests/validators/test_simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34306 2024-04-17 17:34:18.000000 xmlschema-3.3.0/tests/validators/test_wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38338 2024-03-25 21:28:10.000000 xmlschema-3.3.0/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1441 2024-03-13 05:41:48.000000 xmlschema-3.3.0/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.687928 xmlschema-3.3.0/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3089 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6145 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/aliases.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11866 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.692928 xmlschema-3.3.0/xmlschema/converters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6255 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6372 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7504 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24133 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7629 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/gdata.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5271 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5824 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5409 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24831 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38425 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.3.0/xmlschema/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15000 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/exports.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.695928 xmlschema-3.3.0/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.3.0/xmlschema/extras/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-3.3.0/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.556928 xmlschema-3.3.0/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.697928 xmlschema-3.3.0/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.3.0/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.3.0/xmlschema/extras/templates/python/sample.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24452 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16326 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.3.0/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.557928 xmlschema-3.3.0/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.698928 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64464 2024-03-19 14:02:56.000000 xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.557928 xmlschema-3.3.0/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.699928 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/pl/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.700928 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.558928 xmlschema-3.3.0/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.700928 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10643 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9653 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.3.0/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49667 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.561928 xmlschema-3.3.0/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.701928 xmlschema-3.3.0/xmlschema/schemas/DSIG/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.702928 xmlschema-3.3.0/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.703928 xmlschema-3.3.0/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.704928 xmlschema-3.3.0/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.706928 xmlschema-3.3.0/xmlschema/schemas/XENC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema-11.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.707928 xmlschema-3.3.0/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.708928 xmlschema-3.3.0/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.708928 xmlschema-3.3.0/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.709928 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.710928 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.710928 xmlschema-3.3.0/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.3.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.712928 xmlschema-3.3.0/xmlschema/testing/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.3.0/xmlschema/testing/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31080 2024-04-16 10:58:59.000000 xmlschema-3.3.0/xmlschema/testing/_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-10-18 10:59:40.000000 xmlschema-3.3.0/xmlschema/testing/_case_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.3.0/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7658 2024-01-07 11:20:34.000000 xmlschema-3.3.0/xmlschema/testing/_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-3.3.0/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.3.0/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.718928 xmlschema-3.3.0/xmlschema/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3677 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7277 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-04-16 13:14:15.000000 xmlschema-3.3.0/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.3.0/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46820 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67446 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17473 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31285 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33583 2024-04-07 16:34:58.000000 xmlschema-3.3.0/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    64335 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7108 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19395 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27717 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.3.0/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7924 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   107664 2024-04-16 13:49:31.000000 xmlschema-3.3.0/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    62097 2024-03-25 21:28:10.000000 xmlschema-3.3.0/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    37949 2024-04-17 17:34:18.000000 xmlschema-3.3.0/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    42960 2024-03-30 06:19:36.000000 xmlschema-3.3.0/xmlschema/validators/xsdbase.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.719928 xmlschema-3.3.0/xmlschema/xpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-02-18 21:08:04.000000 xmlschema-3.3.0/xmlschema/xpath/assertion_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-02-18 21:08:04.000000 xmlschema-3.3.0/xmlschema/xpath/identity_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/mixin.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4101 2024-03-13 05:27:13.000000 xmlschema-3.3.0/xmlschema/xpath/proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-02-13 06:35:18.000000 xmlschema-3.3.0/xmlschema/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-17 17:34:43.719928 xmlschema-3.3.0/xmlschema.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    19948 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-04-17 17:34:43.000000 xmlschema-3.3.0/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.897755 xmlschema-3.3.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.3.1/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28514 2024-04-28 08:15:54.000000 xmlschema-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-04-24 11:40:07.000000 xmlschema-3.3.1/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.3.1/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-28 08:22:28.897755 xmlschema-3.3.1/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-04-24 11:40:07.000000 xmlschema-3.3.1/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.851756 xmlschema-3.3.1/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.3.1/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11907 2024-04-24 11:40:07.000000 xmlschema-3.3.1/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.3.1/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-04-28 08:15:54.000000 xmlschema-3.3.1/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.3.1/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.3.1/doc/extras.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9946 2024-04-24 11:40:07.000000 xmlschema-3.3.1/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.3.1/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2024-04-24 11:40:07.000000 xmlschema-3.3.1/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-04-24 11:40:07.000000 xmlschema-3.3.1/doc/requirements.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.3.1/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31284 2024-04-24 11:40:07.000000 xmlschema-3.3.1/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.3.1/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.3.1/pyproject.toml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-04-24 11:40:07.000000 xmlschema-3.3.1/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-04-28 08:22:28.897755 xmlschema-3.3.1/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-04-28 08:15:54.000000 xmlschema-3.3.1/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.853756 xmlschema-3.3.1/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.3.1/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.843756 xmlschema-3.3.1/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.853756 xmlschema-3.3.1/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.854756 xmlschema-3.3.1/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.3.1/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.3.1/tests/templates/filters/wrong-template.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3576 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.854756 xmlschema-3.3.1/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.843756 xmlschema-3.3.1/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.855756 xmlschema-3.3.1/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection-default.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection-redef-xmlns.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-04-28 07:58:31.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.3.1/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.856756 xmlschema-3.3.1/tests/test_cases/examples/menù/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù-ascii.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù-ascii.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù-cp1252.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù-cp1252.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/examples/menù/menù.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.856756 xmlschema-3.3.1/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.858756 xmlschema-3.3.1/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-redef.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.844756 xmlschema-3.3.1/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.858756 xmlschema-3.3.1/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.858756 xmlschema-3.3.1/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.859756 xmlschema-3.3.1/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.3.1/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.860756 xmlschema-3.3.1/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.860756 xmlschema-3.3.1/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.861756 xmlschema-3.3.1/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.3.1/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.3.1/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.865756 xmlschema-3.3.1/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/dynamic-case1-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/dynamic-case1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/dynamic-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case7.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case8.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included6-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included7-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/features/namespaces/included8-redefine.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.865756 xmlschema-3.3.1/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.3.1/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.866756 xmlschema-3.3.1/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.847756 xmlschema-3.3.1/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.866756 xmlschema-3.3.1/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.866756 xmlschema-3.3.1/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.866756 xmlschema-3.3.1/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.866756 xmlschema-3.3.1/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.867756 xmlschema-3.3.1/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.867756 xmlschema-3.3.1/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.867756 xmlschema-3.3.1/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.868756 xmlschema-3.3.1/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.868756 xmlschema-3.3.1/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.868756 xmlschema-3.3.1/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.868756 xmlschema-3.3.1/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.869756 xmlschema-3.3.1/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.869756 xmlschema-3.3.1/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.869756 xmlschema-3.3.1/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.869756 xmlschema-3.3.1/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.870756 xmlschema-3.3.1/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.871756 xmlschema-3.3.1/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.871756 xmlschema-3.3.1/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.871756 xmlschema-3.3.1/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.871756 xmlschema-3.3.1/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.872756 xmlschema-3.3.1/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.872756 xmlschema-3.3.1/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.872756 xmlschema-3.3.1/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.846756 xmlschema-3.3.1/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.872756 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.873756 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.873756 xmlschema-3.3.1/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.873756 xmlschema-3.3.1/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.873756 xmlschema-3.3.1/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.873756 xmlschema-3.3.1/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.874756 xmlschema-3.3.1/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.875756 xmlschema-3.3.1/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.875756 xmlschema-3.3.1/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.875756 xmlschema-3.3.1/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.876756 xmlschema-3.3.1/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.876756 xmlschema-3.3.1/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.876756 xmlschema-3.3.1/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.877756 xmlschema-3.3.1/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.877756 xmlschema-3.3.1/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.877756 xmlschema-3.3.1/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.878756 xmlschema-3.3.1/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.878756 xmlschema-3.3.1/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.878756 xmlschema-3.3.1/tests/test_cases/issues/issue_349/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_349/issue_349.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_349/issue_349.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.878756 xmlschema-3.3.1/tests/test_cases/issues/issue_362/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.878756 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir1/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.879756 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir1/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.879756 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_362/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.879756 xmlschema-3.3.1/tests/test_cases/issues/issue_363/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.879756 xmlschema-3.3.1/tests/test_cases/issues/issue_372/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_372/issue_372-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_372/issue_372-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_372/issue_372.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.880756 xmlschema-3.3.1/tests/test_cases/issues/issue_386/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386-2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.880756 xmlschema-3.3.1/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.3.1/tests/test_cases/mypy/extra_validator.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/mypy/protocols.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.3.1/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.3.1/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.881756 xmlschema-3.3.1/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/resources/dummy file.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.3.1/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.3.1/tests/test_cases/resources/with_entity.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.882756 xmlschema-3.3.1/tests/test_cases/serialization/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/serialization/abdera.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/serialization/badgerfish.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/serialization/document.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/serialization/jsonml.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cases/serialization/parker.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6760 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_cases/testfiles
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.847756 xmlschema-3.3.1/tests/test_cases/translations/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.882756 xmlschema-3.3.1/tests/test_cases/translations/pl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/translations/pl/tw-1(5)8e.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.3.1/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26547 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16648 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_exports.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3232 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_files.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30654 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24748 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5626 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23503 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.3.1/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    58208 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.3.1/tests/test_schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.3.1/tests/test_validation.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27268 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2024-04-16 19:49:32.000000 xmlschema-3.3.1/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.882756 xmlschema-3.3.1/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.1/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79183 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validation/test_decoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38298 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    29640 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.885756 xmlschema-3.3.1/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.3.1/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.3.1/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.3.1/tests/validators/test_elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17319 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validators/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63246 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.3.1/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15860 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.3.1/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    55282 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.3.1/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    39368 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2024-03-23 21:43:51.000000 xmlschema-3.3.1/tests/validators/test_simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34234 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tests/validators/test_wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38338 2024-04-24 11:40:07.000000 xmlschema-3.3.1/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1443 2024-04-28 08:15:54.000000 xmlschema-3.3.1/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.886756 xmlschema-3.3.1/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3089 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6145 2024-04-24 11:40:07.000000 xmlschema-3.3.1/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11786 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.888756 xmlschema-3.3.1/xmlschema/converters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-04-24 11:40:07.000000 xmlschema-3.3.1/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6212 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6325 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7435 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24085 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7587 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/gdata.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5228 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5791 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5409 2024-04-24 11:40:07.000000 xmlschema-3.3.1/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24719 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38344 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.3.1/xmlschema/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14983 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/exports.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.888756 xmlschema-3.3.1/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.3.1/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21868 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.847756 xmlschema-3.3.1/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.888756 xmlschema-3.3.1/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.3.1/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.3.1/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24173 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16616 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.3.1/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.889756 xmlschema-3.3.1/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64464 2024-03-19 14:02:56.000000 xmlschema-3.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.889756 xmlschema-3.3.1/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/locale/pl/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.889756 xmlschema-3.3.1/xmlschema/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.889756 xmlschema-3.3.1/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13137 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9653 2024-04-24 11:40:07.000000 xmlschema-3.3.1/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-04-24 11:40:07.000000 xmlschema-3.3.1/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.3.1/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49645 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.848756 xmlschema-3.3.1/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.890756 xmlschema-3.3.1/xmlschema/schemas/DSIG/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.890756 xmlschema-3.3.1/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.890756 xmlschema-3.3.1/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.890756 xmlschema-3.3.1/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.890756 xmlschema-3.3.1/xmlschema/schemas/XENC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/schemas/XENC/xenc-schema-11.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/schemas/XENC/xenc-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.891756 xmlschema-3.3.1/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.891756 xmlschema-3.3.1/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.891756 xmlschema-3.3.1/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.891756 xmlschema-3.3.1/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.891756 xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.892756 xmlschema-3.3.1/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.3.1/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.892756 xmlschema-3.3.1/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.3.1/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31057 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7924 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.3.1/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7641 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4873 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.3.1/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.895756 xmlschema-3.3.1/xmlschema/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3676 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7257 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.3.1/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    46718 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67353 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17336 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31243 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33545 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64379 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7142 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19283 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27694 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.3.1/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7924 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   107844 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    62602 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    37800 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43687 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/validators/xsdbase.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.895756 xmlschema-3.3.1/xmlschema/xpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/xpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/xpath/assertion_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/xpath/identity_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/xpath/mixin.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4059 2024-04-28 08:15:54.000000 xmlschema-3.3.1/xmlschema/xpath/proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-04-24 11:40:08.000000 xmlschema-3.3.1/xmlschema/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-04-28 08:22:28.895756 xmlschema-3.3.1/xmlschema.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    19948 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-04-28 08:22:28.000000 xmlschema-3.3.1/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-3.3.0/CHANGELOG.rst` & `xmlschema-3.3.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v3.3.1`_ (2024-04-27)
+======================
+* Update validation errors with logging stacktrace in debug mode
+* Improve locations parsing and URL encoding
+
 `v3.3.0`_ (2024-04-17)
 ======================
 * Rewrite the validation of openContent using InterleavedModelVisitor and SuffixedModelVisitor
 * Fix validation of XSD 1.1 'all' nested models
 
 `v3.2.1`_ (2024-04-07)
 ======================
@@ -694,7 +699,8 @@
 .. _v3.0.0: https://github.com/brunato/xmlschema/compare/v2.5.1...v3.0.0
 .. _v3.0.1: https://github.com/brunato/xmlschema/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/brunato/xmlschema/compare/v3.0.1...v3.0.2
 .. _v3.1.0: https://github.com/brunato/xmlschema/compare/v3.0.2...v3.1.0
 .. _v3.2.0: https://github.com/brunato/xmlschema/compare/v3.1.0...v3.2.0
 .. _v3.2.1: https://github.com/brunato/xmlschema/compare/v3.2.0...v3.2.1
 .. _v3.3.0: https://github.com/brunato/xmlschema/compare/v3.2.1...v3.3.0
+.. _v3.3.1: https://github.com/brunato/xmlschema/compare/v3.3.0...v3.3.1
```

### Comparing `xmlschema-3.3.0/LICENSE` & `xmlschema-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/PKG-INFO` & `xmlschema-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.3.0
+Version: 3.3.1
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.3.0/README.rst` & `xmlschema-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/Makefile` & `xmlschema-3.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/api.rst` & `xmlschema-3.3.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/components.rst` & `xmlschema-3.3.1/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/conf.py` & `xmlschema-3.3.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '3.3'
 # The full version, including alpha/beta/rc tags.
-release = '3.3.0'
+release = '3.3.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-3.3.0/doc/converters.rst` & `xmlschema-3.3.1/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/extras.rst` & `xmlschema-3.3.1/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/features.rst` & `xmlschema-3.3.1/doc/features.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/intro.rst` & `xmlschema-3.3.1/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/testing.rst` & `xmlschema-3.3.1/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/doc/usage.rst` & `xmlschema-3.3.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/setup.py` & `xmlschema-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='3.3.0',
+    version='3.3.1',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
```

### Comparing `xmlschema-3.3.0/tests/check_memory.py` & `xmlschema-3.3.1/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_all.py` & `xmlschema-3.3.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection-redef-xmlns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.py` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xml` & `xmlschema-3.3.1/tests/test_cases/examples/menù/menù-ascii.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-ascii.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/menù/menù-ascii.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/menù/menù-cp1252.xml` & `xmlschema-3.3.1/tests/test_cases/examples/menù/menù-cp1252.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/menù/menù.xml` & `xmlschema-3.3.1/tests/test_cases/examples/menù/menù.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-3.3.1/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-3.3.1/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-3.3.1/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-3.3.1/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-3.3.1/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-3.3.1/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/data.xml` & `xmlschema-3.3.1/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/data2.xml` & `xmlschema-3.3.1/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/data3.xml` & `xmlschema-3.3.1/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-3.3.1/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-3.3.1/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-3.3.1/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/complex11-restrictions.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/complex11-restrictions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/invalid-restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-3.3.1/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-3.3.1/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-3.3.1/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/models.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-3.3.1/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-3.3.1/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-3.3.1/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-3.3.1/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-3.3.1/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_022/README.md` & `xmlschema-3.3.1/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-3.3.1/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-3.3.1/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_349/issue_349.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_349/issue_349.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_362/issue_362_1.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_362/issue_362_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_363/issue_363.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_363/issue_363.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_372/issue_372.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_372/issue_372.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386-2.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/issues/issue_386/issue_386.xsd` & `xmlschema-3.3.1/tests/test_cases/issues/issue_386/issue_386.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/mypy/extra_validator.py` & `xmlschema-3.3.1/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/mypy/protocols.py` & `xmlschema-3.3.1/tests/test_cases/mypy/protocols.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/mypy/schema_source.py` & `xmlschema-3.3.1/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/mypy/simple_types.py` & `xmlschema-3.3.1/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/serialization/abdera.json` & `xmlschema-3.3.1/tests/test_cases/serialization/abdera.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/serialization/badgerfish.json` & `xmlschema-3.3.1/tests/test_cases/serialization/badgerfish.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/serialization/document.xml` & `xmlschema-3.3.1/tests/test_cases/serialization/document.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/serialization/jsonml.json` & `xmlschema-3.3.1/tests/test_cases/serialization/jsonml.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/serialization/parker.json` & `xmlschema-3.3.1/tests/test_cases/serialization/parker.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/testfiles` & `xmlschema-3.3.1/tests/test_cases/testfiles`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 features/derivations/complex-extensions.xsd --errors=1
 features/derivations/complex11-restrictions.xsd --version=1.1
 features/derivations/complex-with-simple-content-restriction.xsd
 features/derivations/list_types.xsd --errors=1
 features/derivations/list_types.xml --errors=2
 features/derivations/invalid-enumeration-restriction.xsd --errors=1
-features/derivations/invalid-restrictions1.xsd --errors=2
+features/derivations/invalid-restrictions1.xsd --errors=2  # FIXME? (should be three errors)
 features/derivations/invalid-restrictions1.xsd --version=1.1 --errors=1
 features/derivations/invalid-restrictions2.xsd --errors=1
 features/derivations/invalid-restrictions2.xsd --version=1.1 --errors=1
 
 features/elements/type_alternatives.xsd --errors=3
 features/elements/type_alternatives.xsd --version=1.1
 features/elements/type_alternatives-no-ns.xsd --version=1.1
```

### Comparing `xmlschema-3.3.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd` & `xmlschema-3.3.1/tests/test_cases/translations/pl/tw-1(5)8e.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml` & `xmlschema-3.3.1/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_cli.py` & `xmlschema-3.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_codegen.py` & `xmlschema-3.3.1/tests/test_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,19 +185,19 @@
     def test_schema_argument(self):
         generator = self.generator_class(self.schema)
         class_name = generator.__class__.__name__
         namespace = 'http://xmlschema.test/ns'
 
         self.assertIs(generator.schema, self.schema)
         self.assertIsInstance(generator._env, jinja2.Environment)
-        self.assertEqual(repr(generator), "{}(namespace={!r})".format(class_name, namespace))
+        self.assertEqual(repr(generator), f"{class_name}(namespace={namespace!r})")
 
         generator = self.generator_class(self.col_xsd_file)
         self.assertIsInstance(generator.schema, XMLSchema11)
-        self.assertEqual(repr(generator), "{}(schema='collection.xsd')".format(class_name))
+        self.assertEqual(repr(generator), f"{class_name}(schema='collection.xsd')")
 
     def test_searchpath_argument(self):
         class DemoGenerator2(AbstractGenerator):
             formal_language = 'Demo2'
 
         with self.assertRaises(ValueError) as ec:
             DemoGenerator2(self.schema)
@@ -235,15 +235,15 @@
         self.assertIsNot(generator.builtin_types, generator.types_map)
         self.assertEqual(generator.builtin_types, generator.types_map)
 
     def test_list_templates(self):
         template_dir = Path(__file__).parent.joinpath('templates')
         language = self.generator_class.formal_language.lower()
 
-        templates = set(x.name for x in template_dir.glob('{}/*'.format(language)))
+        templates = {x.name for x in template_dir.glob(f'{language}/*')}
         templates.update(x.name for x in template_dir.glob('filters/*'))
         self.assertSetEqual(set(self.generator.list_templates()), templates)
 
     def test_matching_templates(self):
         self.assertSetEqual(set(self.generator.matching_templates('name*_filter*')),
                             {'name_filter_test.jinja', 'namespace_filter_test.jinja'})
```

### Comparing `xmlschema-3.3.0/tests/test_converters.py` & `xmlschema-3.3.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_dataobjects.py` & `xmlschema-3.3.1/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_documents.py` & `xmlschema-3.3.1/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_exports.py` & `xmlschema-3.3.1/tests/test_exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,18 +251,18 @@
         self.assertIn('{http://xmlschema.test/tns1}item1', schema.maps.elements)
         self.assertIn('{http://xmlschema.test/tns2}item2', schema.maps.elements)
         self.assertIn('{http://xmlschema.test/tns2}item3', schema.maps.elements)
 
         with tempfile.TemporaryDirectory() as dirname:
             schema.export(target=dirname)
 
-            exported_files = set(
+            exported_files = {
                 str(x.relative_to(dirname)).replace('\\', '/')
                 for x in pathlib.Path(dirname).glob('**/*.xsd')
-            )
+            }
             self.assertSetEqual(
                 exported_files,
                 {'issue_362_1.xsd', 'dir2/issue_362_2.xsd', 'dir1/issue_362_1.xsd',
                  'dir1/dir2/issue_362_2.xsd', 'issue_362_1.xsd', 'dir2/issue_362_2.xsd',
                  'dir1/issue_362_1.xsd', 'dir1/dir2/issue_362_2.xsd'}
             )
 
@@ -340,15 +340,15 @@
         url = ("https://raw.githubusercontent.com/brewpoo/"
                "BeerXML-Standard/master/schema/BeerXML.xsd")
 
         with tempfile.TemporaryDirectory() as dirname:
             location_map = download_schemas(url, target=dirname, modify=True)
             self.assertEqual(location_map, {})
 
-            xsd_files = set(x.name for x in pathlib.Path(dirname).glob('*.xsd'))
+            xsd_files = {x.name for x in pathlib.Path(dirname).glob('*.xsd')}
             self.assertSetEqual(xsd_files, {
                 'BeerXML.xsd', 'measureable_units.xsd', 'hops.xsd',
                 'yeast.xsd', 'mash.xsd', 'style.xsd', 'water.xsd',
                 'grain.xsd', 'misc.xsd', 'recipes.xsd', 'mash_step.xsd'
             })
 
             xsd_path = pathlib.Path(dirname).joinpath('BeerXML.xsd')
```

### Comparing `xmlschema-3.3.0/tests/test_files.py` & `xmlschema-3.3.1/tests/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             test_class = make_validation_test_class(
                 test_file, test_args, test_num, schema_class, check_with_lxml
             )
             test_num += 1
         else:
             continue
 
-        print("Add test %r for file %r ..." % (test_class.__name__, test_file))
+        print(f"Add test {test_class.__name__!r} for file {test_file!r} ...")
         test_suite.addTest(test_loader.loadTestsFromTestCase(test_class))
 
     if test_num == 1:
         print("No XSD or XML file to test, exiting ...")
     else:
         runner = unittest.TextTestRunner()
         runner.run(test_suite)
```

### Comparing `xmlschema-3.3.0/tests/test_helpers.py` & `xmlschema-3.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_locations.py` & `xmlschema-3.3.1/tests/test_locations.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from urllib.parse import urlsplit, uses_relative
 from pathlib import Path, PurePath, PureWindowsPath, PurePosixPath
 from unittest.mock import patch, MagicMock
 
 import xmlschema.locations
 from xmlschema.locations import LocationPath, LocationPosixPath, LocationWindowsPath, \
     is_url, is_local_url, is_remote_url, url_path_is_file, normalize_url, \
-    normalize_locations, match_location
+    normalize_locations, match_location, is_encoded_url, is_safe_url, encode_url, decode_url
 
 TEST_CASES_DIR = str(pathlib.Path(__file__).absolute().parent.joinpath('test_cases'))
 
-DRIVE_REGEX = '(/[a-zA-Z]:|/)' if platform.system() == 'Windows' else ''
+DRIVE_REGEX = '(/[a-zA-Z]:|)' if platform.system() == 'Windows' else ''
 
 XML_WITH_NAMESPACES = '<pfa:root xmlns:pfa="http://xmlschema.test/nsa">\n' \
                       '  <pfb:elem xmlns:pfb="http://xmlschema.test/nsb"/>\n' \
                       '</pfa:root>'
 
 
 def casepath(relative_path):
@@ -81,14 +81,41 @@
             path = PureWindowsPath(filter_windows_path(url_parts.path))
             expected_path = PureWindowsPath(filter_windows_path(expected_parts.path))
         else:
             path = PurePath(url_parts.path)
             expected_path = PurePath(expected_parts.path)
         self.assertEqual(path, expected_path, "%r: Paths differ." % url)
 
+    def test_urlsplit(self):
+        url = "https://xmlschema.test/schema/test.xsd"
+        self.assertEqual(
+            urlsplit(url), ("https", "xmlschema.test", "/schema/test.xsd", '', '')
+        )
+
+        url = "https://xmlschema.test/xs:schema/test.xsd"
+        self.assertEqual(
+            urlsplit(url), ("https", "xmlschema.test", "/xs:schema/test.xsd", '', '')
+        )
+
+        url = "https://xmlschema.test/schema/test.xsd#xs:element"
+        self.assertEqual(
+            urlsplit(url), ("https", "xmlschema.test", "/schema/test.xsd", '', 'xs:element')
+        )
+
+        url = "https://xmlschema.test@username:password/schema/test.xsd"
+        self.assertEqual(
+            urlsplit(url),
+            ("https", "xmlschema.test@username:password", "/schema/test.xsd", '', '')
+        )
+
+        url = "https://xmlschema.test/schema/test.xsd?id=10"
+        self.assertEqual(
+            urlsplit(url), ("https", "xmlschema.test", "/schema/test.xsd", 'id=10', '')
+        )
+
     def test_path_from_uri(self):
         with self.assertRaises(ValueError) as ec:
             LocationPath.from_uri('')
         self.assertEqual(str(ec.exception), 'Empty URI provided!')
 
         path = LocationPath.from_uri('https://example.com/names/?name=foo')
         self.assertIsInstance(path, LocationPosixPath)
@@ -98,25 +125,31 @@
         self.assertIsInstance(path, LocationPosixPath)
         self.assertEqual(str(path), '/home/foo/names')
 
         path = LocationPosixPath.from_uri('file:///home/foo/names#foo')
         self.assertIsInstance(path, LocationPosixPath)
         self.assertEqual(str(path), '/home/foo/names')
 
-        path = LocationPosixPath.from_uri('file:///home\\foo\\names#foo')
-        self.assertIsInstance(path, LocationWindowsPath)
+        path = LocationPath.from_uri('file:///home\\foo\\names#foo')
         self.assertTrue(path.as_posix().endswith('/home/foo/names'))
+        self.assertIsInstance(path, LocationWindowsPath)
 
         path = LocationPosixPath.from_uri('file:///c:/home/foo/names/')
         self.assertIsInstance(path, LocationWindowsPath)
+
+        path = LocationPath.from_uri('file:///c:/home/foo/names/')
+        self.assertIsInstance(path, LocationWindowsPath)
         self.assertEqual(str(path), r'c:\home\foo\names')
         self.assertEqual(path.as_uri(), 'file:///c:/home/foo/names')
 
         path = LocationPosixPath.from_uri('file:c:/home/foo/names/')
         self.assertIsInstance(path, LocationWindowsPath)
+
+        path = LocationPath.from_uri('file:c:/home/foo/names/')
+        self.assertIsInstance(path, LocationWindowsPath)
         self.assertEqual(str(path), r'c:\home\foo\names')
         self.assertEqual(path.as_uri(), 'file:///c:/home/foo/names')
 
         with self.assertRaises(ValueError) as ec:
             LocationPath.from_uri('file://c:/home/foo/names/')
         self.assertEqual(str(ec.exception), "Invalid URI 'file://c:/home/foo/names/'")
 
@@ -132,27 +165,28 @@
         self.check_url(normalize_url('../dir1/./dir2', 'file:///home'), 'file:///dir1/dir2')
 
         self.check_url(normalize_url('other.xsd', 'file:///home'), 'file:///home/other.xsd')
         self.check_url(normalize_url('other.xsd', 'file:///home/'), 'file:///home/other.xsd')
         self.check_url(normalize_url('file:other.xsd', 'file:///home'), 'file:///home/other.xsd')
 
         cwd = os.getcwd()
-        cwd_url = 'file://{}/'.format(cwd) if cwd.startswith('/') else 'file:///{}/'.format(cwd)
+        cwd_url = f'file://{cwd}/' if cwd.startswith('/') else f'file:///{cwd}/'
 
         self.check_url(normalize_url('other.xsd', keep_relative=True), 'file:other.xsd')
         self.check_url(normalize_url('file:other.xsd', keep_relative=True), 'file:other.xsd')
         self.check_url(normalize_url('file:other.xsd'), cwd_url + 'other.xsd')
         self.check_url(normalize_url('file:other.xsd', 'https://site/base', True), 'file:other.xsd')
         self.check_url(normalize_url('file:other.xsd', 'http://site/base'), cwd_url + 'other.xsd')
 
         self.check_url(normalize_url('dummy path.xsd'), cwd_url + 'dummy%20path.xsd')
         self.check_url(normalize_url('dummy path.xsd', 'http://site/base'),
                        'http://site/base/dummy%20path.xsd')
-        self.check_url(normalize_url('dummy path.xsd', 'file://host/home/'),
-                       PurePath('//host/home/dummy path.xsd').as_uri())
+
+        self.assertEqual(normalize_url('dummy path.xsd', 'file://host/home/'),
+                         'file:////host/home/dummy%20path.xsd')
 
         url = "file:///c:/Downloads/file.xsd"
         self.check_url(normalize_url(url, base_url="file:///d:/Temp/"), url)
 
     def test_normalize_url_windows(self):
         win_abs_path1 = 'z:\\Dir_1_0\\Dir2-0\\schemas/XSD_1.0/XMLSchema.xsd'
         win_abs_path2 = 'z:\\Dir-1.0\\Dir-2_0\\'
@@ -168,28 +202,33 @@
         self.check_url(normalize_url('xsd1.0/schema.xsd', win_abs_path2),
                        'file:///z:/Dir-1.0/Dir-2_0/xsd1.0/schema.xsd')
 
         with self.assertRaises(ValueError) as ec:
             normalize_url('file:///\\k:\\Dir A\\schema.xsd')
         self.assertIn("Invalid URI", str(ec.exception))
 
+        # u
+        base_url = 'D:/a/xmlschema/xmlschema/tests/test_cases/examples/'
+        self.assertEqual(normalize_url('vehicles.xsd', base_url),
+                         f'file:///{base_url}vehicles.xsd')
+
     def test_normalize_url_unc_paths__issue_246(self):
         url = PureWindowsPath(r'\\host\share\file.xsd').as_uri()
         self.assertNotEqual(normalize_url(r'\\host\share\file.xsd'),
                             url)  # file://host/share/file.xsd
         self.assertEqual(normalize_url(r'\\host\share\file.xsd'),
                          url.replace('file://', 'file:////'))
 
     def test_normalize_url_unc_paths__issue_268(self,):
         unc_path = r'\\filer01\MY_HOME\dev\XMLSCHEMA\test.xsd'
         url = PureWindowsPath(unc_path).as_uri()
         self.assertEqual(str(PureWindowsPath(unc_path)), unc_path)
         self.assertEqual(url, 'file://filer01/MY_HOME/dev/XMLSCHEMA/test.xsd')
 
-        # Same UNC path as URI with the host inserted in path path.
+        # Same UNC path as URI with the host inserted in path.
         url_host_in_path = url.replace('file://', 'file:////')
         self.assertEqual(url_host_in_path, 'file:////filer01/MY_HOME/dev/XMLSCHEMA/test.xsd')
 
         self.assertEqual(normalize_url(unc_path), url_host_in_path)
 
         with patch.object(os, 'name', 'nt'):
             self.assertEqual(os.name, 'nt')
@@ -219,15 +258,15 @@
 
     def test_normalize_url_with_base_unc_path(self,):
         base_unc_path = '\\\\filer01\\MY_HOME\\'
         base_url = PureWindowsPath(base_unc_path).as_uri()
         self.assertEqual(str(PureWindowsPath(base_unc_path)), base_unc_path)
         self.assertEqual(base_url, 'file://filer01/MY_HOME/')
 
-        # Same UNC path as URI with the host inserted in path path.
+        # Same UNC path as URI with the host inserted in path
         base_url_host_in_path = base_url.replace('file://', 'file:////')
         self.assertEqual(base_url_host_in_path, 'file:////filer01/MY_HOME/')
 
         self.assertEqual(normalize_url(base_unc_path), base_url_host_in_path)
 
         with patch.object(os, 'name', 'nt'):
             self.assertEqual(os.name, 'nt')
@@ -257,46 +296,83 @@
             url = normalize_url(r'dev/XMLSCHEMA/test.xsd', base_url=base_url_host_in_path)
             self.assertEqual(url, 'file:////filer01/MY_HOME/dev/XMLSCHEMA/test.xsd')
 
     def test_normalize_url_slashes(self):
         # Issue #116
         url = '//anaconda/envs/testenv/lib/python3.6/site-packages/xmlschema/validators/schemas/'
         if os.name == 'posix':
+            normalize_url(url)
             self.assertEqual(normalize_url(url), pathlib.PurePath(url).as_uri())
         else:
             # On Windows // is interpreted as a network share UNC path
             self.assertEqual(os.name, 'nt')
             self.assertEqual(normalize_url(url),
                              pathlib.PurePath(url).as_uri().replace('file://', 'file:////'))
 
         self.assertRegex(normalize_url('/root/dir1/schema.xsd'),
                          f'file://{DRIVE_REGEX}/root/dir1/schema.xsd')
 
         self.assertRegex(normalize_url('////root/dir1/schema.xsd'),
-                         f'file://{DRIVE_REGEX}/root/dir1/schema.xsd')
+                         f'file://{DRIVE_REGEX}//root/dir1/schema.xsd')
         self.assertRegex(normalize_url('dir2/schema.xsd', '////root/dir1'),
-                         f'file://{DRIVE_REGEX}/root/dir1/dir2/schema.xsd')
+                         f'file://{DRIVE_REGEX}//root/dir1/dir2/schema.xsd')
 
         self.assertEqual(normalize_url('//root/dir1/schema.xsd'),
                          'file:////root/dir1/schema.xsd')
         self.assertEqual(normalize_url('dir2/schema.xsd', '//root/dir1/'),
                          'file:////root/dir1/dir2/schema.xsd')
         self.assertEqual(normalize_url('dir2/schema.xsd', '//root/dir1'),
                          'file:////root/dir1/dir2/schema.xsd')
 
     def test_normalize_url_hash_character(self):
         url = normalize_url('issue #000.xml', 'file:///dir1/dir2/')
+        self.assertRegex(url, f'file://{DRIVE_REGEX}/dir1/dir2/issue%20')
+
+        url = normalize_url('issue%20%23000.xml', 'file:///dir1/dir2/')
         self.assertRegex(url, f'file://{DRIVE_REGEX}/dir1/dir2/issue%20%23000.xml')
 
         url = normalize_url('data.xml', 'file:///dir1/dir2/issue%20001')
         self.assertRegex(url, f'file://{DRIVE_REGEX}/dir1/dir2/issue%20001/data.xml')
 
-        url = normalize_url('data.xml', '/dir1/dir2/issue #002')
+        url = normalize_url('data.xml', '/dir1/dir2/issue%20%23002')
         self.assertRegex(url, f'{DRIVE_REGEX}/dir1/dir2/issue%20%23002/data.xml')
 
+    def test_normalize_url_with_query_part(self):
+        url = "https://xmlschema.test/schema 2/test.xsd?name=2 id=3"
+        self.assertEqual(
+            normalize_url(url),
+            "https://xmlschema.test/schema%202/test.xsd?name=2%20id=3"
+        )
+
+        url = "https://xmlschema.test/schema 2/test.xsd?name=2 id=3"
+        self.assertEqual(
+            normalize_url(url, method='html'),
+            "https://xmlschema.test/schema%202/test.xsd?name=2+id=3"
+        )
+
+        url = "/path/schema 2/test.xsd?name=2 id=3"
+        self.assertRegex(
+            normalize_url(url),
+            f'file://{DRIVE_REGEX}/path/schema%202/test.xsd'
+        )
+
+        self.assertRegex(
+            normalize_url('other.xsd?id=2', 'file:///home?name=2&id='),
+            f'file://{DRIVE_REGEX}/home/other.xsd'
+        )
+        self.assertRegex(
+            normalize_url('other.xsd#element', 'file:///home#attribute'),
+            f'file://{DRIVE_REGEX}/home/other.xsd'
+        )
+
+        self.check_url(normalize_url('other.xsd?id=2', 'https://host/path?name=2&id='),
+                       'https://host/path/other.xsd?id=2')
+        self.check_url(normalize_url('other.xsd#element', 'https://host/path?name=2&id='),
+                       'https://host/path/other.xsd#element')
+
     def test_is_url_function(self):
         self.assertTrue(is_url(self.col_xsd_file))
         self.assertFalse(is_url('http://example.com['))
         self.assertTrue(is_url(b'http://example.com'))
         self.assertFalse(is_url(' \t<root/>'))
         self.assertFalse(is_url(b'  <root/>'))
         self.assertFalse(is_url('line1\nline2'))
@@ -342,14 +418,52 @@
         self.assertTrue(url_path_is_file(normalize_url(self.col_xml_file)))
         self.assertFalse(url_path_is_file(self.col_dir))
         self.assertFalse(url_path_is_file('http://example.com/'))
 
         with patch('platform.system', MagicMock(return_value="Windows")):
             self.assertFalse(url_path_is_file('file:///c:/Windows/unknown'))
 
+    def test_is_encoded_url(self):
+        self.assertFalse(is_encoded_url("https://xmlschema.test/schema/test.xsd"))
+        self.assertTrue(is_encoded_url("https://xmlschema.test/schema/issue%20%231999.xsd"))
+        self.assertFalse(is_encoded_url("a b c"))
+        self.assertFalse(is_encoded_url("a+b+c"))
+        self.assertFalse(is_encoded_url("a b+c"))
+
+    def test_is_safe_url(self):
+        self.assertTrue(is_safe_url("https://xmlschema.test/schema/test.xsd"))
+        self.assertFalse(is_safe_url("https://xmlschema.test/schema 2/test.xsd"))
+        self.assertTrue(is_safe_url("https://xmlschema.test/schema/test.xsd#elements"))
+        self.assertTrue(is_safe_url("https://xmlschema.test/schema/test.xsd?id=2"))
+        self.assertFalse(is_safe_url("https://xmlschema.test/schema/test.xsd?id=2 name=foo"))
+
+    def test_encode_and_decode_url(self):
+        url = "https://xmlschema.test/schema/test.xsd"
+        self.assertEqual(encode_url(url), url)
+        self.assertEqual(decode_url(encode_url(url)), url)
+
+        url = "https://xmlschema.test/schema 2/test.xsd"
+        self.assertEqual(encode_url(url), "https://xmlschema.test/schema%202/test.xsd")
+        self.assertEqual(decode_url(encode_url(url)), url)
+
+        url = "https://xmlschema.test@u:p/xs:schema@2/test.xsd"
+        self.assertEqual(encode_url(url), "https://xmlschema.test@u:p/xs%3Aschema%402/test.xsd")
+        self.assertEqual(decode_url(encode_url(url)), url)
+
+        url = "https://xmlschema.test/schema 2/test.xsd?name=2 id=3"
+        self.assertEqual(
+            encode_url(url), "https://xmlschema.test/schema%202/test.xsd?name=2%20id=3")
+        self.assertEqual(decode_url(encode_url(url)), url)
+
+        self.assertEqual(encode_url(url, method='html'),
+                         "https://xmlschema.test/schema%202/test.xsd?name=2+id=3")
+        self.assertEqual(decode_url(encode_url(url, method='html'), method='html'), url)
+        self.assertEqual(decode_url(encode_url(url), method='html'), url)
+        self.assertNotEqual(decode_url(encode_url(url, method='html')), url)
+
     def test_normalize_locations_function(self):
         locations = normalize_locations(
             [('tns0', 'alpha'), ('tns1', 'http://example.com/beta')], base_url='/home/user'
         )
         self.assertEqual(locations[0][0], 'tns0')
         self.assertRegex(locations[0][1], f'file://{DRIVE_REGEX}/home/user/alpha')
         self.assertEqual(locations[1][0], 'tns1')
```

### Comparing `xmlschema-3.3.0/tests/test_memory.py` & `xmlschema-3.3.1/tests/test_memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,35 +43,35 @@
             raise ValueError("Cannot the a memory profile output of more than one function!")
         return max(v - mem_usage[0] for v in mem_usage[1:])
 
     @unittest.skip
     def test_package_memory_usage(self):
         test_dir = os.path.dirname(__file__) or '.'
         cmd = [sys.executable, os.path.join(test_dir, 'check_memory.py'), '1']
-        output = subprocess.check_output(cmd, universal_newlines=True)
+        output = subprocess.check_output(cmd, text=True)
         package_mem = self.check_memory_profile(output)
         self.assertLess(package_mem, 20)
 
     def test_element_tree_memory_usage(self):
         test_dir = os.path.dirname(__file__) or '.'
         xsd10_schema_file = os.path.join(
             os.path.dirname(os.path.abspath(test_dir)),
             'xmlschema/schemas/XSD_1.0/XMLSchema.xsd'
         )
 
         cmd = [sys.executable, os.path.join(test_dir, 'check_memory.py'), '2', xsd10_schema_file]
-        output = subprocess.check_output(cmd, universal_newlines=True)
+        output = subprocess.check_output(cmd, text=True)
         parse_mem = self.check_memory_profile(output)
 
         cmd = [sys.executable, os.path.join(test_dir, 'check_memory.py'), '3', xsd10_schema_file]
-        output = subprocess.check_output(cmd, universal_newlines=True)
+        output = subprocess.check_output(cmd, text=True)
         iterparse_mem = self.check_memory_profile(output)
 
         cmd = [sys.executable, os.path.join(test_dir, 'check_memory.py'), '4', xsd10_schema_file]
-        output = subprocess.check_output(cmd, universal_newlines=True)
+        output = subprocess.check_output(cmd, text=True)
         lazy_iterparse_mem = self.check_memory_profile(output)
 
         self.assertLess(parse_mem, 2)
         self.assertLess(lazy_iterparse_mem, parse_mem)
         self.assertLess(lazy_iterparse_mem, iterparse_mem)
 
     def test_decode_memory_usage(self):
@@ -87,19 +87,19 @@
                 fp.write('xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" ')
                 fp.write(f'xsi:noNamespaceSchemaLocation="{xsd_file.as_uri()}">\n')
                 for k in range(1000):
                     fp.write('<chunk><a><b1/><b2/><b3/></a></chunk>\n')
                 fp.write('</data>\n')
 
             cmd = [sys.executable, python_script, '5', str(xml_file)]
-            output = subprocess.check_output(cmd, universal_newlines=True)
+            output = subprocess.check_output(cmd, text=True)
             decode_mem = self.check_memory_profile(output)
 
             cmd = [sys.executable, python_script, '6', str(xml_file)]
-            output = subprocess.check_output(cmd, universal_newlines=True)
+            output = subprocess.check_output(cmd, text=True)
             lazy_decode_mem = self.check_memory_profile(output)
 
         self.assertLessEqual(decode_mem, 2.6)
         self.assertLessEqual(lazy_decode_mem, 2.1)
 
     def test_validate_memory_usage(self):
         with tempfile.TemporaryDirectory() as dirname:
@@ -114,19 +114,19 @@
                 fp.write('xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" ')
                 fp.write(f'xsi:noNamespaceSchemaLocation="{xsd_file.as_uri()}">\n')
                 for k in range(1000):
                     fp.write('<chunk><a><b1/><b2/><b3/></a></chunk>\n')
                 fp.write('</data>\n')
 
             cmd = [sys.executable, python_script, '7', str(xml_file)]
-            output = subprocess.check_output(cmd, universal_newlines=True)
+            output = subprocess.check_output(cmd, text=True)
             validate_mem = self.check_memory_profile(output)
 
             cmd = [sys.executable, python_script, '8', str(xml_file)]
-            output = subprocess.check_output(cmd, universal_newlines=True)
+            output = subprocess.check_output(cmd, text=True)
             lazy_validate_mem = self.check_memory_profile(output)
 
             self.assertLess(validate_mem, 2.6)
             self.assertLess(lazy_validate_mem, 2.1)
 
 
 if __name__ == '__main__':
```

### Comparing `xmlschema-3.3.0/tests/test_namespaces.py` & `xmlschema-3.3.1/tests/test_namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def test_dictionary_methods(self):
         namespaces = NamespaceResourcesMap()
         namespaces['tns0'] = 'schema1.xsd'
         namespaces['tns1'] = 'schema2.xsd'
         self.assertEqual(namespaces, {'tns0': ['schema1.xsd'], 'tns1': ['schema2.xsd']})
 
         self.assertEqual(len(namespaces), 2)
-        self.assertEqual(set(x for x in namespaces), {'tns0', 'tns1'})
+        self.assertEqual({x for x in namespaces}, {'tns0', 'tns1'})
 
         del namespaces['tns0']
         self.assertEqual(namespaces, {'tns1': ['schema2.xsd']})
         self.assertEqual(len(namespaces), 1)
 
         namespaces.clear()
         self.assertEqual(namespaces, {})
```

### Comparing `xmlschema-3.3.0/tests/test_package.py` & `xmlschema-3.3.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_resources.py` & `xmlschema-3.3.1/tests/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
 
         xml_text = resource.get_text()
         self.assertIn('<vh:vehicles ', xml_text)
         self.assertIn('<!-- Comment -->', xml_text)
         self.assertIn('</vh:vehicles>', xml_text)
 
     def test_xml_resource_from_resource(self):
-        xml_file = urlopen('file://{}'.format(add_leading_slash(self.vh_xml_file)))
+        xml_file = urlopen(f'file://{add_leading_slash(self.vh_xml_file)}')
         try:
             resource = XMLResource(xml_file, lazy=False)
             self.assertEqual(resource.source, xml_file)
             self.assertEqual(resource.root.tag, '{http://example.com/vehicles}vehicles')
             self.assertIsNone(resource.url)
             self.assertIsNone(resource.text)
             resource.load()
@@ -479,15 +479,15 @@
         )
 
         source = "/tmp/vehicles.xsd"
         with self.assertRaises(XMLResourceError) as ctx:
             XMLResource(source, base_url=base_url, allow='sandbox')
         self.assertEqual(
             str(ctx.exception),
-            "block access to out of sandbox file {}".format(normalize_url(source)),
+            f"block access to out of sandbox file {normalize_url(source)}",
         )
 
         with self.assertRaises(TypeError) as ctx:
             XMLResource("https://xmlschema.test/vehicles.xsd", allow=None)
         self.assertEqual(str(ctx.exception),
                          "invalid type <class 'NoneType'> for argument 'allow'")
 
@@ -1170,15 +1170,15 @@
         """XMLResource gets correct data when passed a file like object
         with a name attribute that isn't on disk.
 
         These file descriptors appear when working with the contents from a
         zip using the zipfile module and with Django files in some
         instances.
         """
-        class FileProxy(object):
+        class FileProxy:
             def __init__(self, fid, fake_name):
                 self._fid = fid
                 self.name = fake_name
 
             def __getattr__(self, attr):
                 try:
                     return self.__dict__[attr]
```

### Comparing `xmlschema-3.3.0/tests/test_schemas.py` & `xmlschema-3.3.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_translations.py` & `xmlschema-3.3.1/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_typing.py` & `xmlschema-3.3.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_validation.py` & `xmlschema-3.3.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_w3c_suite.py` & `xmlschema-3.3.1/tests/test_w3c_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
                         else:
                             schema_tree = lxml_etree.parse(source)
                             lxml_etree.XMLSchema(schema_tree)
                         continue
 
                     schema_class = XMLSchema11 if version == '1.1' else XMLSchema10
                     if expected == 'invalid':
-                        message = "schema %s should be invalid with XSD %s" % (rel_path, version)
+                        message = f"schema {rel_path} should be invalid with XSD {version}"
                         with self.assertRaises(XMLSchemaException, msg=message):
                             with warnings.catch_warnings():
                                 warnings.simplefilter('ignore')
                                 if len(item['sources']) <= 1:
                                     schema_class(source, use_meta=use_meta,
                                                  use_fallback=use_fallback)
                                 else:
@@ -437,15 +437,15 @@
             for item in filter(lambda x: not x['source'].endswith('.xsd'), group_tests):
                 source = item['source']
                 rel_path = os.path.relpath(source)
 
                 for version, expected in sorted(filter(lambda x: x[0] != 'source', item.items())):
                     schema_class = XMLSchema11 if version == '1.1' else XMLSchema10
                     if expected == 'invalid':
-                        message = "instance %s should be invalid with XSD %s" % (rel_path, version)
+                        message = f"instance {rel_path} should be invalid with XSD {version}"
                         with self.assertRaises((XMLSchemaException, ElementTree.ParseError),
                                                msg=message):
                             with warnings.catch_warnings():
                                 warnings.simplefilter('ignore')
                                 if not schemas:
                                     validate(source, schema=schema, cls=schema_class)
                                 else:
@@ -479,15 +479,15 @@
 
     if not any(g['source'].endswith('.xsd') for g in group_tests):
         del TestGroupCase.test_xsd_schema
     if not any(g['source'].endswith('.xml') for g in group_tests):
         del TestGroupCase.test_xml_instances
 
     TestGroupCase.__name__ = TestGroupCase.__qualname__ = str(
-        'TestGroupCase{0:05}_{1}'.format(group_num, name.replace('-', '_'))
+        'TestGroupCase{:05}_{}'.format(group_num, name.replace('-', '_'))
     )
     return TestGroupCase
 
 
 def w3c_tests_factory(argv=None):
     import sys
 
@@ -599,15 +599,15 @@
                 xsd_version=testgroup_version,
             )
             if cls is not None:
                 test_classes[cls.__name__] = cls
                 testset_groups += 1
 
         if args.verbose and testset_groups and not quiet:
-            print("Added {} test groups from {}".format(testset_groups, href_attr))
+            print(f"Added {testset_groups} test groups from {href_attr}")
 
     if test_classes and not quiet:
         print("\n+++ Number of classes under test: %d +++" % len(test_classes))
         if total_xml_files:
             print("+++ Number of XSD schemas under test: %d +++" % total_xsd_files)
             print("+++ Number of XML files under test: %d +++" % total_xml_files)
         print()
```

### Comparing `xmlschema-3.3.0/tests/test_wsdl.py` & `xmlschema-3.3.1/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/test_xpath.py` & `xmlschema-3.3.1/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validation/test_decoding.py` & `xmlschema-3.3.1/tests/validation/test_decoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         {
             '@available': True,
             '@id': 'b0836217463',
             'author': {
                 '@id': 'JM',
                 'born': '1893-04-20',
                 'dead': '1983-12-25',
-                'name': u'Joan Miró',
+                'name': 'Joan Miró',
                 'qualification': 'painter, sculptor and ceramicist'
             },
             'position': 2,
             'title': None,
             'year': '1925'
     }]
 }
@@ -163,15 +163,15 @@
                            'qualification': 'painter'},
                 'estimation': 10000.0,
                 'position': 1,
                 'title': 'The Umbrellas',
                 'year': '1886'},
                {'author': {'born': '1893-04-20',
                            'dead': '1983-12-25',
-                           'name': u'Joan Miró',
+                           'name': 'Joan Miró',
                            'qualification': 'painter, sculptor and ceramicist'},
                 'position': 2,
                 'title': None,
                 'year': '1925'}]}
 
 COLLECTION_PARKER_ROOT = {
     'col:collection': {'object': [{'author': {'born': '1841-02-25',
@@ -180,15 +180,15 @@
                                               'qualification': 'painter'},
                                    'estimation': 10000.0,
                                    'position': 1,
                                    'title': 'The Umbrellas',
                                    'year': '1886'},
                                   {'author': {'born': '1893-04-20',
                                               'dead': '1983-12-25',
-                                              'name': u'Joan Miró',
+                                              'name': 'Joan Miró',
                                               'qualification': 'painter, sculptor and ceramicist'},
                                    'position': 2,
                                    'title': None,
                                    'year': '1925'}]}}
 
 COLLECTION_BADGERFISH = {
     'col:collection': {
@@ -212,15 +212,15 @@
             {
                 '@available': True,
                 '@id': 'b0836217463',
                 'author': {
                     '@id': 'JM',
                     'born': {'$': '1893-04-20'},
                     'dead': {'$': '1983-12-25'},
-                    'name': {'$': u'Joan Miró'},
+                    'name': {'$': 'Joan Miró'},
                     'qualification': {
                         '$': 'painter, sculptor and ceramicist'}
                 },
                 'position': {'$': 2},
                 'title': {},
                 'year': {'$': '1925'}
         }]
@@ -255,15 +255,15 @@
                         'attributes': {'available': True, 'id': 'b0836217463'},
                         'children': [{
                             'author': {
                                 'attributes': {'id': 'JM'},
                                 'children': [{
                                     'born': '1893-04-20',
                                     'dead': '1983-12-25',
-                                    'name': u'Joan Miró',
+                                    'name': 'Joan Miró',
                                     'qualification': 'painter, sculptor and ceramicist'}
                                 ]},
                             'position': 2,
                             'title': [],
                             'year': '1925'
                         }]
                     }]
@@ -297,15 +297,15 @@
      {'available': True, 'id': 'b0836217463'},
      ['position', 2],
      ['title'],
      ['year', '1925'],
      [
          'author',
          {'id': 'JM'},
-         ['name', u'Joan Miró'],
+         ['name', 'Joan Miró'],
          ['born', '1893-04-20'],
          ['dead', '1983-12-25'],
          ['qualification', 'painter, sculptor and ceramicist']
      ]]
 ]
 
 COLLECTION_COLUMNAR = {
@@ -1114,33 +1114,33 @@
         obj = xs.attributes['b64'].decode(base64_value.decode(), binary_types=True)
         self.assertEqual(obj, expected_value)
         self.assertIsInstance(obj, datatypes.Base64Binary)
 
         # Element
         xs = self.get_schema('<xs:element name="b64" type="xs:base64Binary"/>')
 
-        obj = xs.decode('<b64>{}</b64>'.format(base64_value.decode()))
+        obj = xs.decode(f'<b64>{base64_value.decode()}</b64>')
         self.assertEqual(obj, str(expected_value))
         self.assertIsInstance(obj, str)
 
-        obj = xs.decode('<b64>{}</b64>'.format(base64_value.decode()), binary_types=True)
+        obj = xs.decode(f'<b64>{base64_value.decode()}</b64>', binary_types=True)
         self.assertEqual(obj, expected_value)
         self.assertIsInstance(obj, datatypes.Base64Binary)
 
         self.check_decode(base64_code_type, base64.b64encode(b'abcefgh'),
                           datatypes.Base64Binary('YWJjZWZnaA=='))
         self.check_decode(base64_code_type, b' Y  W J j ZWZ\t\tn\na A= =',
                           datatypes.Base64Binary('Y W J j ZWZ n a A= ='))
-        self.check_decode(base64_code_type, u' Y  W J j ZWZ\t\tn\na A= =',
+        self.check_decode(base64_code_type, ' Y  W J j ZWZ\t\tn\na A= =',
                           datatypes.Base64Binary('Y W J j ZWZ n a A= ='))
         self.check_decode(base64_code_type, base64.b64encode(b'abcefghi'),
                           datatypes.Base64Binary('YWJjZWZnaGk='))
 
-        self.check_decode(base64_code_type, u'YWJjZWZnaA=', XMLSchemaValidationError)
-        self.check_decode(base64_code_type, u'YWJjZWZna$==', XMLSchemaValidationError)
+        self.check_decode(base64_code_type, 'YWJjZWZnaA=', XMLSchemaValidationError)
+        self.check_decode(base64_code_type, 'YWJjZWZna$==', XMLSchemaValidationError)
 
         base64_length4_type = self.st_schema.types['base64Length4']
         self.check_decode(base64_length4_type, base64.b64encode(b'abc'),
                           XMLSchemaValidationError)
         self.check_decode(base64_length4_type, base64.b64encode(b'abce'),
                           datatypes.Base64Binary('YWJjZQ=='))
         self.check_decode(base64_length4_type, base64.b64encode(b'abcef'),
@@ -1291,15 +1291,15 @@
         self.assertTrue(xs.is_valid('<value>10</value>'))
         self.assertFalse(xs.is_valid('<value>alpha</value>'))
         self.assertEqual(xs.decode('<value>10</value>'), 10)
 
     def test_union_types__issue_103(self):
         decimal_or_nan = self.st_schema.types['myType']
         self.check_decode(decimal_or_nan, '95.0', Decimal('95.0'))
-        self.check_decode(decimal_or_nan, 'NaN', u'NaN')
+        self.check_decode(decimal_or_nan, 'NaN', 'NaN')
 
     def test_default_values__issue_108(self):
         # From issue #108
         xsd_text = """<?xml version="1.0" encoding="utf-8"?>
             <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
               <xs:element name="root" type="root" default="default_value"/>
               <xs:complexType name="root">
@@ -1365,30 +1365,30 @@
 
     def test_keep_unknown_tags__issue_204(self):
         schema = self.schema_class(self.casepath('issues/issue_204/issue_204.xsd'))
         self.assertTrue(schema.is_valid(self.casepath('issues/issue_204/issue_204_1.xml')))
         self.assertFalse(schema.is_valid(self.casepath('issues/issue_204/issue_204_2.xml')))
 
         data = schema.decode(self.casepath('issues/issue_204/issue_204_2.xml'), validation='lax')
-        self.assertEqual(set(x for x in data[0] if x[0] != '@'), {'child2', 'child5'})
+        self.assertEqual({x for x in data[0] if x[0] != '@'}, {'child2', 'child5'})
 
         data = schema.decode(self.casepath('issues/issue_204/issue_204_3.xml'), validation='lax')
-        self.assertEqual(set(x for x in data[0] if x[0] != '@'), {'child2', 'child5'})
+        self.assertEqual({x for x in data[0] if x[0] != '@'}, {'child2', 'child5'})
 
         data = schema.decode(self.casepath('issues/issue_204/issue_204_3.xml'),
                              validation='lax', keep_unknown=True)
-        self.assertEqual(set(x for x in data[0] if x[0] != '@'), {'child2', 'unknown', 'child5'})
+        self.assertEqual({x for x in data[0] if x[0] != '@'}, {'child2', 'unknown', 'child5'})
         self.assertEqual(data[0]['unknown'], {'a': ['1'], 'b': [None]})
 
         data = schema.decode(self.casepath('issues/issue_204/issue_204_2.xml'), validation='skip')
-        self.assertEqual(set(x for x in data if x[0] != '@'), {'child2', 'child5'})
+        self.assertEqual({x for x in data if x[0] != '@'}, {'child2', 'child5'})
 
         data = schema.decode(self.casepath('issues/issue_204/issue_204_3.xml'),
                              validation='skip', keep_unknown=True)
-        self.assertEqual(set(x for x in data if x[0] != '@'), {'child2', 'unknown', 'child5'})
+        self.assertEqual({x for x in data if x[0] != '@'}, {'child2', 'unknown', 'child5'})
         self.assertEqual(data['unknown'], {'a': ['1'], 'b': [None]})
 
     def test_error_message__issue_115(self):
         schema = self.schema_class(self.casepath('issues/issue_115/Rotation.xsd'))
         rotation_data = '<tns:rotation xmlns:tns="http://www.example.org/Rotation/" ' \
                         'pitch="0.0" roll="0.0" yaw="-1.0" />'
```

### Comparing `xmlschema-3.3.0/tests/validation/test_encoding.py` & `xmlschema-3.3.1/tests/validation/test_encoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,62 +65,62 @@
         )
         self.assertTrue(all(
             local_name(e1.tag) == local_name(e2.tag)
             for e1, e2 in zip(elem.iter(), xt.getroot().iter())
         ))
 
     def test_string_based_builtin_types(self):
-        self.check_encode(self.xsd_types['string'], 'sample string ', u'sample string ')
-        self.check_encode(self.xsd_types['normalizedString'], ' sample string ', u' sample string ')
+        self.check_encode(self.xsd_types['string'], 'sample string ', 'sample string ')
+        self.check_encode(self.xsd_types['normalizedString'], ' sample string ', ' sample string ')
         self.check_encode(self.xsd_types['normalizedString'],
-                          '\n\r sample\tstring\n', u'   sample string ')
-        self.check_encode(self.xsd_types['token'], '\n\r sample\t\tstring\n ', u'sample string')
+                          '\n\r sample\tstring\n', '   sample string ')
+        self.check_encode(self.xsd_types['token'], '\n\r sample\t\tstring\n ', 'sample string')
         self.check_encode(self.xsd_types['language'], 'sample string', XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['language'], ' en ', u'en')
-        self.check_encode(self.xsd_types['Name'], 'first_name', u'first_name')
-        self.check_encode(self.xsd_types['Name'], ' first_name ', u'first_name')
+        self.check_encode(self.xsd_types['language'], ' en ', 'en')
+        self.check_encode(self.xsd_types['Name'], 'first_name', 'first_name')
+        self.check_encode(self.xsd_types['Name'], ' first_name ', 'first_name')
         self.check_encode(self.xsd_types['Name'], 'first name', XMLSchemaValidationError)
         self.check_encode(self.xsd_types['Name'], '1st_name', XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['Name'], 'first_name1', u'first_name1')
-        self.check_encode(self.xsd_types['Name'], 'first:name', u'first:name')
-        self.check_encode(self.xsd_types['NCName'], 'first_name', u'first_name')
+        self.check_encode(self.xsd_types['Name'], 'first_name1', 'first_name1')
+        self.check_encode(self.xsd_types['Name'], 'first:name', 'first:name')
+        self.check_encode(self.xsd_types['NCName'], 'first_name', 'first_name')
         self.check_encode(self.xsd_types['NCName'], 'first:name', XMLSchemaValidationError)
         self.check_encode(self.xsd_types['ENTITY'], 'first:name', XMLSchemaValidationError)
         self.check_encode(self.xsd_types['ID'], 'first:name', XMLSchemaValidationError)
         self.check_encode(self.xsd_types['IDREF'], 'first:name', XMLSchemaValidationError)
 
     def test_decimal_based_builtin_types(self):
-        self.check_encode(self.xsd_types['decimal'], -99.09, u'-99.09')
-        self.check_encode(self.xsd_types['decimal'], '-99.09', u'-99.09')
-        self.check_encode(self.xsd_types['integer'], 1000, u'1000')
+        self.check_encode(self.xsd_types['decimal'], -99.09, '-99.09')
+        self.check_encode(self.xsd_types['decimal'], '-99.09', '-99.09')
+        self.check_encode(self.xsd_types['integer'], 1000, '1000')
         self.check_encode(self.xsd_types['integer'], 100.0, XMLSchemaEncodeError)
-        self.check_encode(self.xsd_types['integer'], 100.0, u'100', validation='lax')
-        self.check_encode(self.xsd_types['short'], 1999, u'1999')
+        self.check_encode(self.xsd_types['integer'], 100.0, '100', validation='lax')
+        self.check_encode(self.xsd_types['short'], 1999, '1999')
         self.check_encode(self.xsd_types['short'], 10000000, XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['float'], 100.0, u'100.0')
+        self.check_encode(self.xsd_types['float'], 100.0, '100.0')
         self.check_encode(self.xsd_types['float'], 'hello', XMLSchemaEncodeError)
-        self.check_encode(self.xsd_types['double'], -4531.7, u'-4531.7')
+        self.check_encode(self.xsd_types['double'], -4531.7, '-4531.7')
         self.check_encode(self.xsd_types['positiveInteger'], -1, XMLSchemaValidationError)
         self.check_encode(self.xsd_types['positiveInteger'], 0, XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['nonNegativeInteger'], 0, u'0')
+        self.check_encode(self.xsd_types['nonNegativeInteger'], 0, '0')
         self.check_encode(self.xsd_types['nonNegativeInteger'], -1, XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['negativeInteger'], -100, u'-100')
+        self.check_encode(self.xsd_types['negativeInteger'], -100, '-100')
         self.check_encode(self.xsd_types['nonPositiveInteger'], 7, XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['unsignedLong'], 101, u'101')
+        self.check_encode(self.xsd_types['unsignedLong'], 101, '101')
         self.check_encode(self.xsd_types['unsignedLong'], -101, XMLSchemaValidationError)
         self.check_encode(self.xsd_types['nonPositiveInteger'], 7, XMLSchemaValidationError)
 
     def test_list_builtin_types(self):
-        self.check_encode(self.xsd_types['IDREFS'], ['first_name'], u'first_name')
+        self.check_encode(self.xsd_types['IDREFS'], ['first_name'], 'first_name')
         self.check_encode(self.xsd_types['IDREFS'],
-                          'first_name', u'first_name')  # Transform data to list
-        self.check_encode(self.xsd_types['IDREFS'], ['one', 'two', 'three'], u'one two three')
+                          'first_name', 'first_name')  # Transform data to list
+        self.check_encode(self.xsd_types['IDREFS'], ['one', 'two', 'three'], 'one two three')
         self.check_encode(self.xsd_types['IDREFS'], [1, 'two', 'three'], XMLSchemaValidationError)
-        self.check_encode(self.xsd_types['NMTOKENS'], ['one', 'two', 'three'], u'one two three')
-        self.check_encode(self.xsd_types['ENTITIES'], ('mouse', 'cat', 'dog'), u'mouse cat dog')
+        self.check_encode(self.xsd_types['NMTOKENS'], ['one', 'two', 'three'], 'one two three')
+        self.check_encode(self.xsd_types['ENTITIES'], ('mouse', 'cat', 'dog'), 'mouse cat dog')
 
     def test_datetime_builtin_type(self):
         xs = self.get_schema('<xs:element name="dt" type="xs:dateTime"/>')
 
         dt = xs.decode('<dt>2019-01-01T13:40:00</dt>', datetime_types=True)
         self.assertIsInstance(dt, datatypes.DateTime10)
         self.assertEqual(etree_tostring(xs.encode(dt)), '<dt>2019-01-01T13:40:00</dt>')
@@ -202,32 +202,32 @@
         self.check_encode(list_of_booleans, [10, False, True], XMLSchemaEncodeError)
         self.check_encode(list_of_booleans, [True, False, 40.0], 'true false', validation='lax')
         self.check_encode(list_of_booleans, [True, False, 40.0],
                           'true false 40.0', validation='skip')
 
     def test_union_types(self):
         integer_or_float = self.st_schema.types['integer_or_float']
-        self.check_encode(integer_or_float, -95, u'-95')
-        self.check_encode(integer_or_float, -95.0, u'-95.0')
+        self.check_encode(integer_or_float, -95, '-95')
+        self.check_encode(integer_or_float, -95.0, '-95.0')
         self.check_encode(integer_or_float, True, XMLSchemaEncodeError)
-        self.check_encode(integer_or_float, True, u'1', validation='lax')
+        self.check_encode(integer_or_float, True, '1', validation='lax')
 
         integer_or_string = self.st_schema.types['integer_or_string']
-        self.check_encode(integer_or_string, 89, u'89')
-        self.check_encode(integer_or_string, 89.0, u'89', validation='lax')
+        self.check_encode(integer_or_string, 89, '89')
+        self.check_encode(integer_or_string, 89.0, '89', validation='lax')
         self.check_encode(integer_or_string, 89.0, XMLSchemaEncodeError)
         self.check_encode(integer_or_string, False, XMLSchemaEncodeError)
-        self.check_encode(integer_or_string, "Venice ", u'Venice ')
+        self.check_encode(integer_or_string, "Venice ", 'Venice ')
 
         boolean_or_integer_or_string = self.st_schema.types['boolean_or_integer_or_string']
-        self.check_encode(boolean_or_integer_or_string, 89, u'89')
-        self.check_encode(boolean_or_integer_or_string, 89.0, u'89', validation='lax')
+        self.check_encode(boolean_or_integer_or_string, 89, '89')
+        self.check_encode(boolean_or_integer_or_string, 89.0, '89', validation='lax')
         self.check_encode(boolean_or_integer_or_string, 89.0, XMLSchemaEncodeError)
-        self.check_encode(boolean_or_integer_or_string, False, u'false')
-        self.check_encode(boolean_or_integer_or_string, "Venice ", u'Venice ')
+        self.check_encode(boolean_or_integer_or_string, False, 'false')
+        self.check_encode(boolean_or_integer_or_string, "Venice ", 'Venice ')
 
     def test_simple_elements(self):
         elem = ElementTree.Element('A')
         elem.text = '89'
         self.check_encode(self.get_element('A', type='xs:string'), '89', elem)
         self.check_encode(self.get_element('A', type='xs:integer'), 89, elem)
         elem.text = '-10.4'
@@ -290,15 +290,15 @@
                 <xs:element name="B3" type="xs:boolean"/>
             </xs:sequence>
         </xs:complexType>
         """)
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('B3', False)]),
-            expected=u'<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>false</B3>\n</A>',
+            expected='<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>false</B3>\n</A>',
             indent=0,
         )
         self.check_encode(schema.elements['A'], {'B1': 'abc', 'B2': 10, 'B4': False},
                           XMLSchemaValidationError)
 
     def test_error_message(self):
         schema = self.schema_class(self.casepath('issues/issue_115/Rotation.xsd'))
@@ -380,28 +380,28 @@
             xsd_component=schema.elements['A'],
             data=dict([('B2', 10), ('B1', 'abc'), ('B3', True)]),
             expected=XMLSchemaChildrenValidationError
         )
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B2', 10), ('B1', 'abc'), ('B3', True)]),
-            expected=u'<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
+            expected='<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
             indent=0, cdata_prefix='#', converter=UnorderedConverter
         )
 
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('#1', 'hello'), ('B3', True)]),
             expected='<A>\nhello<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
             indent=0, cdata_prefix='#', converter=UnorderedConverter
         )
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('#1', 'hello'), ('B3', True)]),
-            expected=u'<A>\n<B1>abc</B1>\n<B2>10</B2>\nhello\n<B3>true</B3>\n</A>',
+            expected='<A>\n<B1>abc</B1>\n<B2>10</B2>\nhello\n<B3>true</B3>\n</A>',
             indent=0, cdata_prefix='#'
         )
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('#1', 'hello')]),
             expected=XMLSchemaValidationError, indent=0, cdata_prefix='#'
         )
@@ -419,21 +419,21 @@
             </xs:sequence>
         </xs:complexType>
         """, converter=UnorderedConverter)
 
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B2', 10), ('B1', 'abc'), ('B3', True)]),
-            expected=u'<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
+            expected='<A>\n<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
             indent=0, cdata_prefix='#'
         )
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('#1', 'hello'), ('B3', True)]),
-            expected=u'<A>\nhello<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
+            expected='<A>\nhello<B1>abc</B1>\n<B2>10</B2>\n<B3>true</B3>\n</A>',
             indent=0, cdata_prefix='#'
         )
         self.check_encode(
             xsd_component=schema.elements['A'],
             data=dict([('B1', 'abc'), ('B2', 10), ('#1', 'hello')]),
             expected=XMLSchemaValidationError, indent=0, cdata_prefix='#'
         )
@@ -691,14 +691,128 @@
         root, errors = schema.encode(instance, validation='lax',
                                      namespaces=namespaces,
                                      use_defaults=False,
                                      converter=JsonMLConverter)
         self.assertListEqual(errors, [])
         self.assertIsNone(etree_elements_assert_equal(root, ElementTree.parse(xml_data).getroot()))
 
+    def test_encoding_with_default_namespace__issue_400(self):
+        schema = self.schema_class(dedent("""\
+            <?xml version="1.0" encoding="utf-8"?>
+            <xs:schema targetNamespace="http://address0.com"
+                       xmlns:xs="http://www.w3.org/2001/XMLSchema"
+                       xmlns:ser="http://address0.com"
+                       xmlns:ds="http://www.address1.com">
+                <xs:import namespace="http://www.w3.org/2000/09/xmldsig#"
+                    schemaLocation="xmldsig-core-schema.xsd"/>
+                <xs:complexType name="class">
+                    <xs:sequence>
+                        <xs:element name="student1" type="ser:String32" minOccurs="0"/>
+                        <xs:element name="student2" type="ser:String32" minOccurs="0"/>
+                    </xs:sequence>
+                </xs:complexType>
+                <xs:element name="class" type="ser:class"/>
+                <xs:simpleType name="String32">
+                    <xs:restriction base="xs:normalizedString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="32"/>
+                    </xs:restriction>
+                </xs:simpleType>
+            </xs:schema>
+            """))
+
+        xml_data = dedent("""\n
+            <ser:class xmlns:ser="http://address0.com">
+                <student1>John</student1>
+                <student2>Rachel</student2>
+            </ser:class>""")
+
+        obj = schema.decode(xml_data, preserve_root=True)
+        self.assertDictEqual(obj, {'ser:class': {
+                             '@xmlns:ser': schema.target_namespace,
+                             "student1": "John",
+                             "student2": "Rachel"}})
+
+        root = schema.encode(obj, preserve_root=True)
+        self.assertIsNone(etree_elements_assert_equal(root, ElementTree.XML(xml_data)))
+
+        obj = schema.decode(xml_data, preserve_root=True, strip_namespaces=True)
+        self.assertDictEqual(obj, {'class': {
+                             "student1": "John",
+                             "student2": "Rachel"}})
+
+        with self.assertRaises(XMLSchemaValidationError):
+            schema.encode(obj, preserve_root=True)
+
+        obj = {
+            'ser:class': {
+                "student1": "John",
+                "student2": "Rachel"
+            }
+        }
+
+        with self.assertRaises(XMLSchemaValidationError):
+            schema.encode(obj, preserve_root=True)
+
+        root = schema.encode(
+            obj, preserve_root=True, namespaces={'ser': schema.target_namespace}
+        )
+        self.assertIsNone(etree_elements_assert_equal(root, ElementTree.XML(xml_data)))
+
+        schema = self.schema_class(dedent("""\
+            <?xml version="1.0" encoding="utf-8"?>
+            <xs:schema targetNamespace="http://address0.com"
+                       elementFormDefault="qualified"
+                       xmlns:xs="http://www.w3.org/2001/XMLSchema"
+                       xmlns:ser="http://address0.com"
+                       xmlns:ds="http://www.address1.com">
+                <xs:import namespace="http://www.w3.org/2000/09/xmldsig#"
+                    schemaLocation="xmldsig-core-schema.xsd"/>
+                <xs:complexType name="class">
+                    <xs:sequence>
+                        <xs:element name="student1" type="ser:String32" minOccurs="0"/>
+                        <xs:element name="student2" type="ser:String32" minOccurs="0"/>
+                    </xs:sequence>
+                </xs:complexType>
+                <xs:element name="class" type="ser:class"/>
+                <xs:simpleType name="String32">
+                    <xs:restriction base="xs:normalizedString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="32"/>
+                    </xs:restriction>
+                </xs:simpleType>
+            </xs:schema>
+            """))
+
+        self.assertFalse(schema.is_valid(xml_data))
+
+        xml_data = dedent("""\n
+            <ser:class xmlns:ser="http://address0.com">
+                <ser:student1>John</ser:student1>
+                <ser:student2>Rachel</ser:student2>
+            </ser:class>""")
+        self.assertTrue(schema.is_valid(xml_data))
+
+        obj = schema.decode(xml_data, preserve_root=True)
+        self.assertDictEqual(obj, {'ser:class': {
+                             '@xmlns:ser': schema.target_namespace,
+                             "ser:student1": "John",
+                             "ser:student2": "Rachel"}})
+
+        root = schema.encode(obj, preserve_root=True)
+        self.assertIsNone(etree_elements_assert_equal(root, ElementTree.XML(xml_data)))
+
+        obj = schema.decode(xml_data, preserve_root=True, strip_namespaces=True)
+        self.assertDictEqual(obj, {'class': {
+                             "student1": "John",
+                             "student2": "Rachel"}})
+
+        root = schema.encode(obj, preserve_root=True, namespaces={'': schema.target_namespace})
+        self.assertIsNone(etree_elements_assert_equal(root, ElementTree.XML(xml_data)))
+
 
 class TestEncoding11(TestEncoding):
     schema_class = XMLSchema11
 
 
 if __name__ == '__main__':
     import platform
```

### Comparing `xmlschema-3.3.0/tests/validation/test_validation.py` & `xmlschema-3.3.1/tests/validation/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         self.assertTrue(xsd_element.is_valid(root, max_depth=1))
         self.assertTrue(xsd_element.is_valid(root, max_depth=2))
         self.assertFalse(xsd_element.is_valid(root, max_depth=3))
 
         # Need to provide namespace explicitly because the default namespace is '' in this case.
         xsd_element = schema.find('collection/object', namespaces={'': schema.target_namespace})
 
+        self.assertIsNotNone(xsd_element)
         self.assertTrue(xsd_element.is_valid(root[0]))
         self.assertFalse(xsd_element.is_valid(root[1]))
         self.assertTrue(xsd_element.is_valid(root[1], max_depth=1))
         self.assertFalse(xsd_element.is_valid(root[1], max_depth=2))
 
     def test_extra_validator_argument(self):
         # Related to issue 227
```

### Comparing `xmlschema-3.3.0/tests/validators/test_attributes.py` & `xmlschema-3.3.1/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_builtins.py` & `xmlschema-3.3.1/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_complex_types.py` & `xmlschema-3.3.1/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_elements.py` & `xmlschema-3.3.1/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_exceptions.py` & `xmlschema-3.3.1/tests/validators/test_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,33 @@
         self.assertEqual(len(errors), 3)
         self.assertIsNone(errors[0].invalid_child)
         self.assertTrue(is_etree_element(errors[1].invalid_child))
         self.assertEqual(errors[1].invalid_child.tag, 'c1')
         self.assertTrue(is_etree_element(errors[2].invalid_child))
         self.assertEqual(errors[2].invalid_child.tag, 'b2')
 
+    def test_validation_error_logging(self):
+        schema = XMLSchema("""
+             <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+                 <xs:element name="root" type="xs:integer"/>
+             </xs:schema>""")
+
+        with self.assertLogs('xmlschema', level='DEBUG') as ctx:
+            with self.assertRaises(XMLSchemaValidationError):
+                schema.validate('<root/>')
+            self.assertEqual(len(ctx.output), 0)
+
+            errors = list(schema.iter_errors('<root/>'))
+            self.assertEqual(len(errors), 1)
+            self.assertIsInstance(errors[0], XMLSchemaDecodeError)
+
+            self.assertEqual(len(ctx.output), 1)
+            self.assertIn('Collect XMLSchemaDecodeError', ctx.output[0])
+            self.assertIn('with traceback:', ctx.output[0])
+
 
 if __name__ == '__main__':
     import platform
     header_template = "Test xmlschema's validator exceptions with Python {} on {}"
     header = header_template.format(platform.python_version(), platform.platform())
     print('{0}\n{1}\n{0}'.format("*" * len(header), header))
```

### Comparing `xmlschema-3.3.0/tests/validators/test_facets.py` & `xmlschema-3.3.1/tests/validators/test_facets.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
                     <xs:simpleType name="type2">
                         <xs:restriction base="type1">
                             <xs:minInclusive value="0"/>
                         </xs:restriction>
                     </xs:simpleType>
                 </xs:schema>"""))
 
-            facet = schema.types['type1'].get_facet('{%s}%s' % (XSD_NAMESPACE, base_facet))
+            facet = schema.types['type1'].get_facet(f'{{{XSD_NAMESPACE}}}{base_facet}')
             self.assertIsNone(facet(0))
             facet2 = schema.types['type2'].get_facet(XSD_MIN_INCLUSIVE)
             self.assertIsNone(facet2(0))
             self.assertIsNot(facet, facet2)
 
         for base_facet in ['minInclusive', 'minExclusive']:
             with self.assertRaises(XMLSchemaParseError):
@@ -465,15 +465,15 @@
                     <xs:simpleType name="type2">
                         <xs:restriction base="type1">
                             <xs:minExclusive value="0"/>
                         </xs:restriction>
                     </xs:simpleType>
                 </xs:schema>"""))
 
-            facet = schema.types['type1'].get_facet('{%s}%s' % (XSD_NAMESPACE, base_facet))
+            facet = schema.types['type1'].get_facet(f'{{{XSD_NAMESPACE}}}{base_facet}')
             self.assertIsNone(facet(1))
             facet2 = schema.types['type2'].get_facet(XSD_MIN_EXCLUSIVE)
             self.assertIsNone(facet2(1))
             self.assertIsNot(facet, facet2)
 
         for base_facet in ['maxInclusive', 'maxExclusive']:
             with self.assertRaises(XMLSchemaParseError):
@@ -566,15 +566,15 @@
                     <xs:simpleType name="type2">
                         <xs:restriction base="type1">
                             <xs:maxInclusive value="0"/>
                         </xs:restriction>
                     </xs:simpleType>
                 </xs:schema>"""))
 
-            facet = schema.types['type1'].get_facet('{%s}%s' % (XSD_NAMESPACE, base_facet))
+            facet = schema.types['type1'].get_facet(f'{{{XSD_NAMESPACE}}}{base_facet}')
             self.assertIsNone(facet(0))
             facet2 = schema.types['type2'].get_facet(XSD_MAX_INCLUSIVE)
             self.assertIsNone(facet2(0))
             self.assertIsNot(facet, facet2)
 
         for base_facet in ['maxInclusive', 'maxExclusive']:
             with self.assertRaises(XMLSchemaParseError):
@@ -666,15 +666,15 @@
                     <xs:simpleType name="type2">
                         <xs:restriction base="type1">
                             <xs:maxExclusive value="0"/>
                         </xs:restriction>
                     </xs:simpleType>
                 </xs:schema>"""))
 
-            facet = schema.types['type1'].get_facet('{%s}%s' % (XSD_NAMESPACE, base_facet))
+            facet = schema.types['type1'].get_facet(f'{{{XSD_NAMESPACE}}}{base_facet}')
             self.assertIsNone(facet(-1))
             facet2 = schema.types['type2'].get_facet(XSD_MAX_EXCLUSIVE)
             self.assertIsNone(facet2(-1))
             self.assertIsNot(facet, facet2)
 
         for base_facet in ['minInclusive', 'minExclusive']:
             with self.assertRaises(XMLSchemaParseError):
```

### Comparing `xmlschema-3.3.0/tests/validators/test_global_maps.py` & `xmlschema-3.3.1/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_groups.py` & `xmlschema-3.3.1/tests/validators/test_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class ModelGroup(XsdGroup):
     """A subclass for testing XSD models, that disables element parsing and schema bindings."""
 
     def __init__(self, model: str, min_occurs: int = 1, max_occurs: Optional[int] = 1) -> None:
         ParticleMixin.__init__(self, min_occurs, max_occurs)
         if model not in {'sequence', 'choice', 'all'}:
-            raise XMLSchemaValueError("invalid model {!r} for a group".format(model))
+            raise XMLSchemaValueError(f"invalid model {model!r} for a group")
         self._group: List[Union[ParticleMixin, 'ModelGroup']] = []
         self.content = self._group
         self.model: str = model
 
     def __repr__(self) -> str:
         return '%s(model=%r, occurs=%r)' % (self.__class__.__name__, self.model, self.occurs)
```

### Comparing `xmlschema-3.3.0/tests/validators/test_identities.py` & `xmlschema-3.3.1/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_models.py` & `xmlschema-3.3.1/tests/validators/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class ModelGroup(XsdGroup):
     """A subclass for testing XSD models, that disables element parsing and schema bindings."""
 
     def __init__(self, model: str, min_occurs: int = 1, max_occurs: Optional[int] = 1) -> None:
         ParticleMixin.__init__(self, min_occurs, max_occurs)
         if model not in {'sequence', 'choice', 'all'}:
-            raise XMLSchemaValueError("invalid model {!r} for a group".format(model))
+            raise XMLSchemaValueError(f"invalid model {model!r} for a group")
         self._group: List[Union[ParticleMixin, 'ModelGroup']] = []
         self.content = self._group
         self.model: str = model
 
     def __repr__(self) -> str:
         return '%s(model=%r, occurs=%r)' % (self.__class__.__name__, self.model, self.occurs)
```

### Comparing `xmlschema-3.3.0/tests/validators/test_notations.py` & `xmlschema-3.3.1/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_particles.py` & `xmlschema-3.3.1/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_schemas.py` & `xmlschema-3.3.1/tests/validators/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_simple_types.py` & `xmlschema-3.3.1/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tests/validators/test_wildcards.py` & `xmlschema-3.3.1/tests/validators/test_wildcards.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 
 class TestXsd11Wildcards(TestXsdWildcards):
 
     schema_class = XMLSchema11
 
     def test_parsing(self):
-        super(TestXsd11Wildcards, self).test_parsing()
+        super().test_parsing()
         schema = self.schema_class("""
         <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="tns1">
             <xs:group name="group1">
               <xs:choice>
                 <xs:any notNamespace="##all"/>
               </xs:choice>
             </xs:group>
@@ -726,15 +726,15 @@
               <xs:sequence>
                 <xs:any notNamespace="##local" notQName="c d e"/>
               </xs:sequence>
             </xs:group>
         </xs:schema>""", XMLSchemaParseError)
 
     def test_any_wildcard(self):
-        super(TestXsd11Wildcards, self).test_any_wildcard()
+        super().test_any_wildcard()
         self.check_schema("""
         <xs:complexType name="taggedType">
           <xs:sequence>
             <xs:element name="tag" type="xs:string"/>
             <xs:any namespace="##other" notNamespace="##targetNamespace" />
           </xs:sequence>
         </xs:complexType>""", XMLSchemaParseError)
@@ -772,15 +772,15 @@
               </xs:sequence>
             </xs:complexType>
         </xs:schema>""")
         self.assertEqual(schema.types['taggedType'].content[-1].not_qname,
                          ['##defined', '{tns1}foo', '##definedSibling'])
 
     def test_any_attribute_wildcard(self):
-        super(TestXsd11Wildcards, self).test_any_attribute_wildcard()
+        super().test_any_attribute_wildcard()
         schema = self.schema_class("""
         <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema"
                 xmlns:tns1="tns1" targetNamespace="tns1">
             <xs:complexType name="taggedType">
               <xs:sequence>
                 <xs:element name="tag" type="xs:string"/>
                 <xs:any namespace="##other" processContents="skip"/>
```

### Comparing `xmlschema-3.3.0/tests/validators/test_xsdbase.py` & `xmlschema-3.3.1/tests/validators/test_xsdbase.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/tox.ini` & `xmlschema-3.3.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     flake8
 commands =
     flake8 xmlschema
     flake8 tests
 
 [testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.9.0
+    mypy==1.10.0
     elementpath==4.4.0
     lxml-stubs
     jinja2
 commands =
     mypy --config-file {toxinidir}/mypy.ini xmlschema
     python tests/test_typing.py
 
@@ -65,15 +65,15 @@
 [testenv:pytest]
 deps =
     pytest
     pytest-randomly
     elementpath>=4.4.0, <5.0.0
     lxml
     jinja2
-    mypy==1.9.0
+    mypy==1.10.0
     lxml-stubs
 commands =
     pytest tests -ra
 
 [testenv:build]
 deps =
     build
```

### Comparing `xmlschema-3.3.0/xmlschema/__init__.py` & `xmlschema-3.3.1/xmlschema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaStopValidation, XMLSchemaIncludeWarning, XMLSchemaImportWarning,
     XMLSchemaTypeTableWarning, XMLSchemaAssertPathWarning, XsdGlobals, XMLSchemaBase,
     XMLSchema, XMLSchema10, XMLSchema11, XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '3.3.0'
+__version__ = '3.3.1'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2024, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
```

### Comparing `xmlschema-3.3.0/xmlschema/aliases.py` & `xmlschema-3.3.1/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/cli.py` & `xmlschema-3.3.1/xmlschema/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 def get_converter(name):
     if not isinstance(name, str):
         return None
 
     try:
         return CONVERTERS_MAP[name.lower()]
     except KeyError:
-        raise ValueError("--converter must be in {!r}".format(tuple(CONVERTERS_MAP)))
+        raise ValueError(f"--converter must be in {tuple(CONVERTERS_MAP)!r}")
 
 
 def xml2json():
     parser = argparse.ArgumentParser(prog=PROGRAM_NAME, add_help=True,
                                      description="decode a set of XML files to JSON.")
     parser.usage = "%(prog)s [OPTION]... [FILE]...\n" \
                    "Try '%(prog)s --help' for more information."
@@ -113,21 +113,21 @@
     if args.indent is not None and args.indent >= 0:
         json_options['indent'] = args.indent
 
     base_path = pathlib.Path(args.output)
     if not base_path.exists():
         base_path.mkdir()
     elif not base_path.is_dir():
-        raise XMLSchemaValueError("{!r} is not a directory".format(str(base_path)))
+        raise XMLSchemaValueError(f"{str(base_path)!r} is not a directory")
 
     tot_errors = 0
     for xml_path in map(pathlib.Path, args.files):
         json_path = base_path.joinpath(xml_path.name).with_suffix('.json')
         if json_path.exists() and not args.force:
-            print("skip {}: the destination file exists!".format(str(json_path)))
+            print(f"skip {str(json_path)}: the destination file exists!")
             continue
 
         with open(str(json_path), 'w') as fp:
             try:
                 errors = to_json(
                     xml_document=str(xml_path),
                     fp=fp,
@@ -137,19 +137,19 @@
                     lazy=args.lazy,
                     defuse=args.defuse,
                     validation='lax',
                     json_options=json_options,
                 )
             except (xmlschema.XMLSchemaException, URLError) as err:
                 tot_errors += 1
-                print("error with {}: {}".format(str(xml_path), str(err)))
+                print(f"error with {str(xml_path)}: {str(err)}")
                 continue
             else:
                 if not errors:
-                    print("{} converted to {}".format(str(xml_path), str(json_path)))
+                    print(f"{str(xml_path)} converted to {str(json_path)}")
                 else:
                     tot_errors += len(errors)
                     print("{} converted to {} with {} errors".format(
                         str(xml_path), str(json_path), len(errors)
                     ))
 
     sys.exit(tot_errors)
@@ -189,39 +189,39 @@
     converter = get_converter(args.converter)
     schema = schema_class(args.schema, locations=args.locations, loglevel=loglevel)
 
     base_path = pathlib.Path(args.output)
     if not base_path.exists():
         base_path.mkdir()
     elif not base_path.is_dir():
-        raise XMLSchemaValueError("{!r} is not a directory".format(str(base_path)))
+        raise XMLSchemaValueError(f"{str(base_path)!r} is not a directory")
 
     tot_errors = 0
     for json_path in map(pathlib.Path, args.files):
         xml_path = base_path.joinpath(json_path.name).with_suffix('.xml')
         if xml_path.exists() and not args.force:
-            print("skip {}: the destination file exists!".format(str(xml_path)))
+            print(f"skip {str(xml_path)}: the destination file exists!")
             continue
 
         with open(str(json_path)) as fp:
             try:
                 root, errors = from_json(
                     source=fp,
                     schema=schema,
                     converter=converter,
                     validation='lax',
                     indent=args.indent,
                 )
             except (xmlschema.XMLSchemaException, URLError) as err:
                 tot_errors += 1
-                print("error with {}: {}".format(str(xml_path), str(err)))
+                print(f"error with {str(xml_path)}: {str(err)}")
                 continue
             else:
                 if not errors:
-                    print("{} converted to {}".format(str(json_path), str(xml_path)))
+                    print(f"{str(json_path)} converted to {str(xml_path)}")
                 else:
                     tot_errors += len(errors)
                     print("{} converted to {} with {} errors".format(
                         str(json_path), str(xml_path), len(errors)
                     ))
 
         with open(str(xml_path), 'w') as fp:
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/__init__.py` & `xmlschema-3.3.1/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/converters/abdera.py` & `xmlschema-3.3.1/xmlschema/converters/abdera.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     __slots__ = ()
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  **kwargs: Any) -> None:
         kwargs.update(attr_prefix='', text_key='', cdata_prefix=None)
-        super(AbderaConverter, self).__init__(
-            namespaces, dict_class, list_class, **kwargs
-        )
+        super().__init__(namespaces, dict_class, list_class, **kwargs)
 
     @property
     def xmlns_processing_default(self) -> str:
         return 'stacked' if isinstance(self.source, XMLResource) else 'none'
 
     @property
     def lossy(self) -> bool:
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/badgerfish.py` & `xmlschema-3.3.1/xmlschema/converters/badgerfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     __slots__ = ()
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  **kwargs: Any) -> None:
         kwargs.update(attr_prefix='@', text_key='$', cdata_prefix='$')
-        super(BadgerFishConverter, self).__init__(
-            namespaces, dict_class, list_class, **kwargs
-        )
+        super().__init__(namespaces, dict_class, list_class, **kwargs)
 
     @property
     def lossy(self) -> bool:
         return False
 
     def get_xmlns_from_data(self, obj: Any) -> Optional[List[Tuple[str, str]]]:
         if not self._use_namespaces or not isinstance(obj, MutableMapping) or '@xmlns' not in obj:
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/columnar.py` & `xmlschema-3.3.1/xmlschema/converters/columnar.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  attr_prefix: Optional[str] = '',
                  **kwargs: Any) -> None:
         kwargs.update(text_key=None, cdata_prefix=None)
-        super(ColumnarConverter, self).__init__(namespaces, dict_class, list_class,
-                                                attr_prefix=attr_prefix, **kwargs)
+        super().__init__(namespaces, dict_class, list_class,
+                         attr_prefix=attr_prefix, **kwargs)
 
     @property
     def xmlns_processing_default(self) -> str:
         return 'stacked' if isinstance(self.source, XMLResource) else 'none'
 
     @property
     def lossy(self) -> bool:
@@ -50,15 +50,15 @@
 
     @property
     def loss_xmlns(self) -> bool:
         return True
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name != 'attr_prefix':
-            super(ColumnarConverter, self).__setattr__(name, value)
+            super().__setattr__(name, value)
         elif not isinstance(value, str):
             msg = "%(name)r must be a <class 'str'> instance, not %(type)r"
             raise XMLSchemaTypeError(msg % {'name': name, 'type': type(value)})
         elif value not in ('', '_', '__'):
             msg = '%r can be the empty string or a single/double underscore'
             raise XMLSchemaValueError(msg % name)
         else:
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/default.py` & `xmlschema-3.3.1/xmlschema/converters/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         self.ns_prefix = 'xmlns' if attr_prefix is None else f'{attr_prefix}xmlns'
 
         self.indent = indent
         self.preserve_root = preserve_root
         self.force_dict = force_dict
         self.force_list = force_list
 
-        super(XMLSchemaConverter, self).__init__(
+        super().__init__(
             namespaces, process_namespaces, strip_namespaces, xmlns_processing, source
         )
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in {'attr_prefix', 'text_key', 'cdata_prefix'}:
             if value is not None and not isinstance(value, str):
                 msg = "%(name)r must be a <class 'str'> instance or None, not %(type)r"
@@ -178,15 +178,15 @@
                 raise XMLSchemaTypeError(msg % {'name': 'dict_class', 'type': type(value)})
 
         elif name == 'list':
             if not issubclass(value, MutableSequence):
                 msg = "%(name)r must be a MutableSequence object, not %(type)r"
                 raise XMLSchemaTypeError(msg % {'name': 'list_class', 'type': type(value)})
 
-        super(XMLSchemaConverter, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     @property
     def xmlns_processing_default(self) -> str:
         """
         Returns the default of the xmlns processing mode, used if `None` is provided.
         """
         if isinstance(self.source, XMLResource):
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/gdata.py` & `xmlschema-3.3.1/xmlschema/converters/gdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     __slots__ = ()
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  **kwargs: Any) -> None:
         kwargs.update(attr_prefix='', text_key='$t', cdata_prefix='$')
-        super(GDataConverter, self).__init__(
-            namespaces, dict_class, list_class, **kwargs
-        )
+        super().__init__(namespaces, dict_class, list_class, **kwargs)
 
     @property
     def lossy(self) -> bool:
         return True  # a child element can override an attribute in the same namespace
 
     def map_qname(self, qname: str) -> str:
         name = super().map_qname(qname)
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/jsonml.py` & `xmlschema-3.3.1/xmlschema/converters/jsonml.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,15 @@
     __slots__ = ()
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  **kwargs: Any) -> None:
         kwargs.update(attr_prefix='', text_key='', cdata_prefix='')
-        super(JsonMLConverter, self).__init__(
-            namespaces, dict_class, list_class, **kwargs
-        )
+        super().__init__(namespaces, dict_class, list_class, **kwargs)
 
     @property
     def lossy(self) -> bool:
         return False
 
     @property
     def losslessly(self) -> bool:
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/parker.py` & `xmlschema-3.3.1/xmlschema/converters/parker.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,16 @@
     __slots__ = ()
 
     def __init__(self, namespaces: Optional[NamespacesType] = None,
                  dict_class: Optional[Type[Dict[str, Any]]] = None,
                  list_class: Optional[Type[List[Any]]] = None,
                  preserve_root: bool = False, **kwargs: Any) -> None:
         kwargs.update(attr_prefix=None, text_key='', cdata_prefix=None)
-        super(ParkerConverter, self).__init__(
-            namespaces, dict_class, list_class,
-            preserve_root=preserve_root, **kwargs
+        super().__init__(
+            namespaces, dict_class, list_class, preserve_root=preserve_root, **kwargs
         )
 
     @property
     def xmlns_processing_default(self) -> str:
         return 'stacked' if isinstance(self.source, XMLResource) else 'none'
 
     @property
```

### Comparing `xmlschema-3.3.0/xmlschema/converters/unordered.py` & `xmlschema-3.3.1/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/dataobjects.py` & `xmlschema-3.3.1/xmlschema/dataobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                  value: Optional[Any] = None,
                  attrib: Optional[Dict[str, Any]] = None,
                  nsmap: Optional[MutableMapping[str, str]] = None,
                  xmlns: Optional[List[Tuple[str, str]]] = None,
                  xsd_element: Optional['XsdElement'] = None,
                  xsd_type: Optional[BaseXsdType] = None) -> None:
 
-        super(DataElement, self).__init__()
+        super().__init__()
         self._children = []
         self.tag = tag
         self.attrib = {}
         self.nsmap = {}
 
         if value is not None:
             self.value = value
@@ -132,15 +132,15 @@
                 self._encoder = value.schema.create_element(
                     self.tag, parent=value, form='unqualified'
                 )
                 self._encoder.type = value
             else:
                 self._encoder = self.xsd_element
 
-        super(DataElement, self).__setattr__(key, value)
+        super().__setattr__(key, value)
 
     @property
     def text(self) -> Optional[str]:
         """The string value of the data element."""
         return raw_xml_encode(self.value)
 
     def get(self, key: str, default: Any = None) -> Any:
@@ -154,15 +154,15 @@
             # Try a match with mapped/unmapped name
             if key.startswith('{'):
                 key = get_prefixed_qname(key, self.nsmap)
                 return self.attrib.get(key, default)
             elif ':' in key:
                 try:
                     _prefix, _local_name = key.split(':')
-                    key = '{%s}%s' % (self.nsmap[_prefix], _local_name)
+                    key = f'{{{self.nsmap[_prefix]}}}{_local_name}'
                 except (ValueError, KeyError):
                     pass
                 else:
                     return self.attrib.get(key, default)
             return default
 
     def set(self, key: str, value: Any) -> None:
@@ -428,21 +428,21 @@
         try:
             xsd_element = attrs['xsd_element']
         except KeyError:
             msg = "attribute 'xsd_element' is required for an XSD data binding class"
             raise XMLSchemaAttributeError(msg) from None
 
         if not isinstance(xsd_element, validators.XsdElement):
-            raise XMLSchemaTypeError("{!r} is not an XSD element".format(xsd_element))
+            raise XMLSchemaTypeError(f"{xsd_element!r} is not an XSD element")
 
         attrs['__module__'] = None
-        return super(DataBindingMeta, mcs).__new__(mcs, name, bases, attrs)
+        return super().__new__(mcs, name, bases, attrs)
 
     def __init__(cls, name: str, bases: Tuple[Type[Any], ...], attrs: Dict[str, Any]) -> None:
-        super(DataBindingMeta, cls).__init__(name, bases, attrs)
+        super().__init__(name, bases, attrs)
         cls.xsd_version = cls.xsd_element.xsd_version
         cls.namespace = cls.xsd_element.target_namespace
 
     def fromsource(cls, source: Union[XMLSourceType, XMLResource],
                    allow: str = 'all', defuse: str = 'remote',
                    timeout: int = 300, **kwargs: Any) -> DecodeType[Any]:
         if not isinstance(source, XMLResource):
@@ -471,15 +471,15 @@
         if data_element_class is None:
             self.data_element_class = DataElement
         else:
             self.data_element_class = data_element_class
 
         self.map_attribute_names = map_attribute_names
         kwargs.update(attr_prefix='', text_key='', cdata_prefix='')
-        super(DataElementConverter, self).__init__(namespaces, **kwargs)
+        super().__init__(namespaces, **kwargs)
 
     @property
     def xmlns_processing_default(self) -> str:
         return 'stacked'
 
     def get_xmlns_from_data(self, obj: Any) -> Optional[List[Tuple[str, str]]]:
         return obj.xmlns if isinstance(obj, DataElement) else None
```

### Comparing `xmlschema-3.3.0/xmlschema/documents.py` & `xmlschema-3.3.1/xmlschema/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,22 +101,22 @@
     if tag.startswith('{'):
         namespace, name = tag[1:].split('}')
     else:
         namespace, name = '', tag
 
     if namespace:
         return cls(
-            '<xs:schema xmlns:xs="{0}" targetNamespace="{1}">\n'
-            '    <xs:element name="{2}"/>\n'
+            '<xs:schema xmlns:xs="{}" targetNamespace="{}">\n'
+            '    <xs:element name="{}"/>\n'
             '</xs:schema>'.format(XSD_NAMESPACE, namespace, name)
         )
     else:
         return cls(
-            '<xs:schema xmlns:xs="{0}">\n'
-            '    <xs:element name="{1}"/>\n'
+            '<xs:schema xmlns:xs="{}">\n'
+            '    <xs:element name="{}"/>\n'
             '</xs:schema>'.format(XSD_NAMESPACE, name)
         )
 
 
 def get_lazy_json_encoder(errors: List[XMLSchemaValidationError]) -> Type[json.JSONEncoder]:
 
     class JSONLazyEncoder(json.JSONEncoder):
@@ -610,16 +610,15 @@
                  uri_mapper: Optional[UriMapperType] = None,
                  use_location_hints: bool = True) -> None:
 
         if cls is None:
             cls = XMLSchema10
         self.validation = validation
         self._namespaces = get_namespace_map(namespaces)
-        super(XmlDocument, self).__init__(source, base_url, allow, defuse,
-                                          timeout, lazy, thin_lazy)
+        super().__init__(source, base_url, allow, defuse, timeout, lazy, thin_lazy)
 
         if isinstance(schema, XMLSchemaBase) and self.namespace in schema.maps.namespaces:
             self.schema = schema
         elif schema is not None and not isinstance(schema, XMLSchemaBase):
             self.schema = cls(
                 source=schema,
                 locations=locations,
@@ -666,15 +665,15 @@
             self.schema.validate(self, namespaces=self.namespaces)
         elif validation == 'lax':
             self.errors = [e for e in self.schema.iter_errors(self, namespaces=self.namespaces)]
         elif validation != 'skip':
             raise XMLSchemaValueError("%r is not a validation mode" % validation)
 
     def parse(self, source: XMLSourceType, lazy: LazyType = False) -> None:
-        super(XmlDocument, self).parse(source, lazy)
+        super().parse(source, lazy)
         self.namespaces = self.get_namespaces(root_only=True)
 
         if self.schema is None:
             pass
         elif self.validation == 'strict':
             self.schema.validate(self, namespaces=self.namespaces)
         elif self.validation == 'lax':
```

### Comparing `xmlschema-3.3.0/xmlschema/exceptions.py` & `xmlschema-3.3.1/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/exports.py` & `xmlschema-3.3.1/xmlschema/exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return locations
 
     def replace_location(self, location: str, repl_location: str) -> None:
         if location == repl_location:
             return
 
         logger.debug("Replace location %r with %r", location, repl_location)
-        repl = 'schemaLocation="{}"'.format(repl_location)
+        repl = f'schemaLocation="{repl_location}"'
         pattern = REPLACE_PATTERN.format(re.escape(location))
         self.text = re.sub(pattern, repl, self.text)
         self.modified = True
 
     def get_location_path(self, location: str,
                           ref: Union['XMLSchemaBase', XMLResource],
                           modify: bool = True) -> LocationPath:
@@ -349,15 +349,15 @@
 
                 url = normalize_url(location, resource.base_url)
                 if any(x.url == url for x in downloads):
                     continue
 
                 try:
                     ref_resource = XMLResource(url, defuse=defuse, timeout=timeout)
-                except (OSError, IOError, XMLResourceError) as err:
+                except (OSError, XMLResourceError) as err:
                     logger.error('Error accessing resource at URL %s: %s', url, err)
                     continue
                 except ElementTree.ParseError as err:
                     logger.error('Error parsing XML resource at URL %s: %s', url, err)
                     continue
                 else:
                     logger.info("Downloaded XML resource from %s", url)
```

### Comparing `xmlschema-3.3.0/xmlschema/extras/codegen.py` & `xmlschema-3.3.1/xmlschema/extras/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 def is_shell_wildcard(pathname):
     return '*' in pathname or '?' in pathname or '[' in pathname
 
 
 def xsd_qname(name):
-    return '{%s}%s' % (XSD_NAMESPACE, name)
+    return f'{{{XSD_NAMESPACE}}}{name}'
 
 
 def filter_method(func):
     """Marks a method for registration as template filter."""
     func.is_filter = True
     return func
 
@@ -93,15 +93,15 @@
             for path in attrs['searchpaths']:
                 if Path(path).is_absolute():
                     dirpath = Path(path)
                 else:
                     dirpath = Path(module_path).parent.joinpath(path)
 
                 if not dirpath.is_dir():
-                    raise ValueError("path {!r} is not a directory!".format(str(path)))
+                    raise ValueError(f"path {str(path)!r} is not a directory!")
                 searchpaths.append(dirpath)
 
         except (KeyError, TypeError):
             pass
         else:
             attrs['searchpaths'] = searchpaths
 
@@ -183,26 +183,26 @@
             elif inspect.isroutine(method) and hasattr(method, '__func__'):
                 # class and instance methods
                 if getattr(method.__func__, 'is_filter', False):
                     self.filters[name] = method
                 elif getattr(method.__func__, 'is_test', False):
                     self.tests[name] = method
 
-        type_mapping_filter = '{}_type'.format(self.formal_language).lower().replace(' ', '_')
+        type_mapping_filter = f'{self.formal_language}_type'.lower().replace(' ', '_')
         if type_mapping_filter not in self.filters:
             self.filters[type_mapping_filter] = self.map_type
 
         self._env = Environment(loader=loader)
         self._env.filters.update(self.filters)
         self._env.tests.update(self.tests)
 
     def __repr__(self):
         if self.schema.url:
-            return '%s(schema=%r)' % (self.__class__.__name__, self.schema.name)
-        return '%s(namespace=%r)' % (self.__class__.__name__, self.schema.target_namespace)
+            return f'{self.__class__.__name__}(schema={self.schema.name!r})'
+        return f'{self.__class__.__name__}(namespace={self.schema.target_namespace!r})'
 
     def list_templates(self, extensions=None, filter_func=None):
         return self._env.list_templates(extensions, filter_func)
 
     def matching_templates(self, name):
         return self._env.list_templates(filter_func=lambda x: fnmatch(x, name))
 
@@ -358,15 +358,15 @@
                 return unnamed
 
             try:
                 if obj[0] == '{':
                     namespace, local_name = obj[1:].split('}')
                     for prefix, uri in self.schema.namespaces.items():
                         if uri == namespace:
-                            qname = '%s:%s' % (prefix, local_name)
+                            qname = f'{prefix}:{local_name}'
                             break
                     else:
                         qname = local_name
                 else:
                     qname = obj
             except IndexError:
                 return ''
@@ -423,15 +423,15 @@
 
         if name.endswith('Type'):
             name = name[:-4]
         elif name.endswith('_type'):
             name = name[:-5]
 
         if suffix:
-            name = '{}{}'.format(name, suffix)
+            name = f'{name}{suffix}'
 
         return name.replace('.', '_').replace('-', '_')
 
     @staticmethod
     @filter_method
     def type_qname(obj, suffix=None, unnamed='none', sep='__'):
         """
@@ -453,15 +453,15 @@
 
         if qname.endswith('Type'):
             qname = qname[:-4]
         elif qname.endswith('_type'):
             qname = qname[:-5]
 
         if suffix:
-            qname = '{}{}'.format(qname, suffix)
+            qname = f'{qname}{suffix}'
 
         return qname.replace('.', '_').replace('-', '_').replace(':', sep)
 
     @staticmethod
     @filter_method
     def sort_types(xsd_types, accept_circularity=False):
         """
@@ -498,15 +498,15 @@
                         deleted += 1
 
             for xsd_type in unordered:
                 unordered[xsd_type] = [x for x in unordered[xsd_type] if x in unordered]
 
             if not deleted:
                 if not accept_circularity:
-                    raise ValueError("circularity found between {!r}".format(list(unordered)))
+                    raise ValueError(f"circularity found between {list(unordered)!r}")
                 ordered_types.extend(list(unordered))
                 break
 
         assert len(xsd_types) == len(ordered_types)
         return ordered_types
 
     def is_derived(self, xsd_type, *names, derivation=None):
```

### Comparing `xmlschema-3.3.0/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-3.3.1/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-3.3.1/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/extras/wsdl.py` & `xmlschema-3.3.1/xmlschema/extras/wsdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         except KeyError:
             return  # a missing attribute is already caught by XSD validator
 
 
 class WsdlMessage(WsdlComponent):
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlMessage, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.parts = {}
         xsd_elements = wsdl_document.schema.maps.elements
         xsd_types = wsdl_document.schema.maps.types
 
         for child in elem.iterfind(WSDL_PART):
             part_name = child.get('name')
             if part_name is None:
@@ -134,15 +134,15 @@
                     wsdl_document.parse_error(msg)
 
                 element_name = get_extended_qname(element_attr, wsdl_document.namespaces)
                 try:
                     self.parts[part_name] = xsd_elements[element_name]
                 except KeyError:
                     self.parts[part_name] = xsd_types[XSD_ANY_TYPE]
-                    msg = "missing schema element {!r}".format(element_name)
+                    msg = f"missing schema element {element_name!r}"
                     wsdl_document.parse_error(msg)
 
                 continue  # pragma: no cover
 
             try:
                 type_attr = child.attrib['type']
             except KeyError:
@@ -150,22 +150,22 @@
                 wsdl_document.parse_error(msg)
             else:
                 type_name = get_extended_qname(type_attr, wsdl_document.namespaces)
                 try:
                     self.parts[part_name] = xsd_types[type_name]
                 except KeyError:
                     self.parts[part_name] = xsd_types[XSD_ANY_TYPE]
-                    msg = "missing schema type {!r}".format(type_name)
+                    msg = f"missing schema type {type_name!r}"
                     wsdl_document.parse_error(msg)
 
 
 class WsdlPortType(WsdlComponent):
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlPortType, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.operations = {}
 
         for child in elem.iterfind(WSDL_OPERATION):
             operation_name = child.get('name')
             if operation_name is None:
                 continue  # Ignore, missing name is already caught by XSD validator
 
@@ -180,15 +180,15 @@
 
 class WsdlOperation(WsdlComponent):
 
     input = output = None
     soap_operation = None
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlOperation, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.faults = {}
 
         input_child = elem.find(WSDL_INPUT)
         if input_child is not None:
             self.input = WsdlInput(input_child, wsdl_document)
 
         output_child = elem.find(WSDL_OUTPUT)
@@ -240,15 +240,15 @@
             return style if style in ('rpc', 'document') else 'document'
 
 
 class WsdlMessageReference(WsdlComponent):
     message = None
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlMessageReference, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         message_name = self._parse_reference(elem, 'message')
         try:
             self.message = wsdl_document.maps.messages[message_name]
         except KeyError:
             if message_name:
                 msg = "unknown message {!r} for {!r}"
                 wsdl_document.parse_error(msg.format(message_name, self))
@@ -284,28 +284,28 @@
         return self.elem.get('namespace', '')
 
 
 class SoapBody(SoapParameter):
     """Class for soap:body bindings."""
 
     def __init__(self, elem, wsdl_document):
-        super(SoapBody, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.parts = elem.get('parts', '').split()
 
 
 class SoapFault(SoapParameter):
     """Class for soap:fault bindings."""
 
 
 class SoapHeader(WsdlMessageReference, SoapParameter):
     """Class for soap:header bindings."""
     part = None
 
     def __init__(self, elem, wsdl_document):
-        super(SoapHeader, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         if self.message is not None and 'part' in elem.attrib:
             try:
                 self.part = self.message.parts[elem.attrib['part']]
             except KeyError:
                 msg = "missing message part {!r}"
                 wsdl_document.parse_error(msg.format(elem.attrib['part']))
 
@@ -323,15 +323,15 @@
     port_type = None
     """The wsdl:portType definition related to the binding instance."""
 
     soap_binding = None
     """The SOAP binding element if any, `None` otherwise."""
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlBinding, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.operations = {}
 
         if wsdl_document.soap_binding:
             self.soap_binding = elem.find(SOAP_BINDING)
             if self.soap_binding is None:
                 msg = "missing soap:binding element for {!r}"
                 wsdl_document.parse_error(msg.format(self))
@@ -418,15 +418,15 @@
 
 class WsdlPort(WsdlComponent):
 
     binding = None
     soap_location = None
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlPort, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
 
         binding_name = self._parse_reference(elem, 'binding')
         try:
             self.binding = wsdl_document.maps.bindings[binding_name]
         except KeyError:
             if binding_name:
                 msg = "unknown binding {!r} for {!r} output"
@@ -437,15 +437,15 @@
                 self.soap_location = child.get('location')
                 break
 
 
 class WsdlService(WsdlComponent):
 
     def __init__(self, elem, wsdl_document):
-        super(WsdlService, self).__init__(elem, wsdl_document)
+        super().__init__(elem, wsdl_document)
         self.ports = {}
 
         for port_child in elem.iterfind(WSDL_PORT):
             port = WsdlPort(port_child, wsdl_document)
             port_name = port.local_name
 
             if port_name is None:
@@ -508,15 +508,15 @@
             self.maps = Wsdl11Maps(self)
 
         if locations:
             self.locations = NamespaceResourcesMap(locations)
         else:
             self.locations = NamespaceResourcesMap()
 
-        super(Wsdl11Document, self).__init__(
+        super().__init__(
             source=source,
             schema=self.schema,
             validation=validation,
             namespaces=namespaces,
             locations=locations,
             base_url=base_url,
             allow=allow,
@@ -547,17 +547,17 @@
     @property
     def services(self):
         """WSDL 1.1 services."""
         return self.maps.services
 
     def parse(self, source, lazy=False):
         if lazy:
-            raise WsdlParseError("{!r} instance cannot be lazy".format(self.__class__))
+            raise WsdlParseError(f"{self.__class__!r} instance cannot be lazy")
 
-        super(Wsdl11Document, self).parse(source, lazy)
+        super().parse(source, lazy)
         self.target_namespace = self._root.get('targetNamespace', '')
         self.soap_binding = SOAP_NAMESPACE in self.namespaces.values()
 
         if self.namespace == XSD_NAMESPACE:
             self.schema.__class__(self, global_maps=self.schema.maps, locations=self.locations)
             return
 
@@ -574,49 +574,49 @@
     def parse_error(self, message):
         if self.validation == 'strict':
             raise WsdlParseError(message)
         elif self.validation == 'lax':
             self.errors.append(WsdlParseError(message))
 
     def _parse_types(self):
-        path = '{}/{}'.format(WSDL_TYPES, XSD_SCHEMA)
+        path = f'{WSDL_TYPES}/{XSD_SCHEMA}'
 
         for child in self._root.iterfind(path):
             source = self.subresource(child)
             self.schema.__class__(source, global_maps=self.schema.maps)
 
     def _parse_messages(self):
         for child in self.iterfind(WSDL_MESSAGE):
             message = WsdlMessage(child, self)
             if message.name in self.maps.messages:
-                self.parse_error("duplicated message {!r}".format(message.prefixed_name))
+                self.parse_error(f"duplicated message {message.prefixed_name!r}")
             else:
                 self.maps.messages[message.name] = message
 
     def _parse_port_types(self):
         for child in self.iterfind(WSDL_PORT_TYPE):
             port_type = WsdlPortType(child, self)
             if port_type.name in self.maps.port_types:
-                self.parse_error("duplicated port type {!r}".format(port_type.prefixed_name))
+                self.parse_error(f"duplicated port type {port_type.prefixed_name!r}")
             else:
                 self.maps.port_types[port_type.name] = port_type
 
     def _parse_bindings(self):
         for child in self.iterfind(WSDL_BINDING):
             binding = WsdlBinding(child, self)
             if binding.name in self.maps.bindings:
-                self.parse_error("duplicated binding {!r}".format(binding.prefixed_name))
+                self.parse_error(f"duplicated binding {binding.prefixed_name!r}")
             else:
                 self.maps.bindings[binding.name] = binding
 
     def _parse_services(self):
         for child in self.iterfind(WSDL_SERVICE):
             service = WsdlService(child, self)
             if service.name in self.maps.services:
-                self.parse_error("duplicated service {!r}".format(service.prefixed_name))
+                self.parse_error(f"duplicated service {service.prefixed_name!r}")
             else:
                 self.maps.services[service.name] = service
 
     def _parse_imports(self):
         namespace_imports = NamespaceResourcesMap(map(
             lambda x: (x.get('namespace', ''), x.get('location', '')),
             filter(lambda x: x.tag == WSDL_IMPORT, self.root)
@@ -629,19 +629,19 @@
             except KeyError:
                 pass
 
             import_error = None
             for url in locations:
                 try:
                     self.import_namespace(namespace, url, self.base_url)
-                except (OSError, IOError) as err:
+                except OSError as err:
                     if import_error is None:
                         import_error = err
                 except SyntaxError as err:
-                    msg = "cannot import namespace %r: %s." % (namespace, err)
+                    msg = f"cannot import namespace {namespace!r}: {err}."
                     self.parse_error(msg)
                 except XMLSchemaValueError as err:
                     self.parse_error(err)
                 else:
                     break
             else:
                 if import_error is not None:
```

### Comparing `xmlschema-3.3.0/xmlschema/helpers.py` & `xmlschema-3.3.1/xmlschema/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import re
+import os
 import logging
+import traceback
 from collections import Counter
 from decimal import Decimal
 from functools import wraps
 from typing import Any, Callable, Iterable, Iterator, List, MutableMapping, \
     MutableSequence, Optional, Tuple, TypeVar, Union
 from xml.etree.ElementTree import ParseError
 
@@ -64,14 +66,20 @@
                 return func(*args, **kwargs)
             finally:
                 logger.setLevel(current_level)
 
     return wrapper
 
 
+def format_xmlschema_stack() -> str:
+    """Extract a formatted traceback for xmlschema package from current stack frame."""
+    package_path = os.path.dirname(__file__)
+    return ''.join(line for line in traceback.format_stack()[:-1] if package_path in line)
+
+
 ###
 # Helper functions for QNames and namespaces
 
 NAMESPACE_PATTERN = re.compile(r'{([^}]*)}')
 
 
 def get_namespace(qname: str, namespaces: Optional[NamespacesType] = None) -> str:
```

### Comparing `xmlschema-3.3.0/xmlschema/limits.py` & `xmlschema-3.3.1/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.1/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.1/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.1/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-3.3.1/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/locations.py` & `xmlschema-3.3.1/xmlschema/locations.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import ntpath
 import posixpath
 import platform
 import string
 from collections.abc import MutableMapping
 from pathlib import Path, PurePath, PurePosixPath, PureWindowsPath
 from typing import Optional, Iterable
-from urllib.parse import urlsplit, urlunsplit, unquote, quote_from_bytes
+from urllib.parse import urlsplit, urlunsplit, quote, quote_plus, unquote, \
+    unquote_plus, quote_from_bytes
 
 from .exceptions import XMLSchemaValueError
 from .aliases import NormalizedLocationsType, LocationsType
 
 
 DRIVE_LETTERS = frozenset(string.ascii_letters)
 
@@ -42,78 +43,72 @@
     def __new__(cls, *args: str) -> 'LocationPath':
         if cls is LocationPath:
             cls = LocationWindowsPath if os.name == 'nt' else LocationPosixPath
         return super().__new__(cls, *args)
 
     @classmethod
     def from_uri(cls, uri: str) -> 'LocationPath':
+        """
+        Parse a URI and return a LocationPath. For non-local schemes like 'http',
+        'https', etc. a LocationPosixPath is returned. For Windows related file
+        paths, like a path with a drive, a UNC path or a path containing a backslash,
+        a LocationWindowsPath is returned.
+        """
         uri = uri.strip()
         if not uri:
             raise XMLSchemaValueError("Empty URI provided!")
 
-        if uri.startswith(r'\\'):
-            return LocationWindowsPath(uri)  # UNC path
-        elif uri.startswith('/'):
-            return cls(uri)
-
         parts = urlsplit(uri)
-        if not parts.scheme:
-            return cls(uri)
+        if not parts.scheme or parts.scheme == 'file':
+            path = urlunsplit(('', parts.netloc, parts.path, '', ''))
         elif parts.scheme in DRIVE_LETTERS and len(parts.scheme) == 1:
-            return LocationWindowsPath(uri)  # Eg. k:/Python/lib/....
-        elif parts.scheme != 'file':
-            return LocationPosixPath(unquote(parts.path))
+            # uri is a Windows path with a drive, e.g. k:/Python/lib/file
 
-        # Get file URI path because urlsplit does not parse it well
-        start = 7 if uri.startswith('file:///') else 5
-        if parts.query:
-            path = uri[start:uri.index('?')]
-        elif parts.fragment:
-            path = uri[start:uri.index('#')]
+            # urlsplit() converts the scheme to lowercase so use uri[0]
+            path = urlunsplit((uri[0], parts.netloc, parts.path, '', ''))
+
+            return LocationWindowsPath(unquote(path))
         else:
-            path = uri[start:]
+            return LocationPosixPath(unquote(parts.path))
 
-        if ':' in path:
-            # Windows path with a drive
-            pos = path.index(':')
-            if pos == 2 and path[0] == '/' and path[1] in DRIVE_LETTERS:
+        if parts.scheme == 'file':
+            if path.startswith('/') and ntpath.splitdrive(path[1:])[0]:
                 return LocationWindowsPath(unquote(path[1:]))
+            elif path.startswith(('//', '/\\')) and ntpath.splitdrive(path[2:])[0]:
+                raise XMLSchemaValueError(f"Invalid URI {uri!r}")
 
-            obj = LocationWindowsPath(unquote(path))
-            if len(obj.drive) != 2 or obj.drive[1] != ':':
-                raise XMLSchemaValueError("Invalid URI %r" % uri)
-            return obj
-
-        if '\\' in path:
+        if ntpath.splitdrive(path)[0] or '\\' in path:
             return LocationWindowsPath(unquote(path))
         return cls(unquote(path))
 
     def as_uri(self) -> str:
-        if not self.is_absolute():
-            # Converts relative paths to not RFC 8089 compliant relative
-            # file URIs because urlopen() doesn't accept simple paths
-            drive = self.drive
-            if len(drive) == 2 and drive[1] == ':':
-                prefix = 'file:' + drive
-                path = self.as_posix()[2:]
-            elif drive:
-                prefix = 'file:'
-                path = self.as_posix()
+        # Implementation that maps relative paths to not RFC 8089 compliant relative
+        # file URIs because urlopen() doesn't accept simple paths. For UNC paths uses
+        # the format with four slashes to let urlopen() works.
+
+        drive = self.drive
+        if len(drive) == 2 and drive[1] == ':':
+            # A Windows path with a drive: 'c:\dir\file' => 'file:///c:/dir/file'
+            prefix = 'file:///' + drive
+            path = self.as_posix()[2:]
+        elif drive:
+            # UNC format case: '\\host\dir\file' => 'file:////host/dir/file'
+            prefix = 'file://'
+            path = self.as_posix()
+        else:
+            path = self.as_posix()
+            if path.startswith('/'):
+                # A Windows relative path or an absolute posix path:
+                #  ('\dir\file' | '/dir/file') => 'file://dir/file'
+                prefix = 'file://'
             else:
+                # A relative posix path: 'dir/file' => 'file:dir/file'
                 prefix = 'file:'
-                path = str(self)
-            return prefix + quote_from_bytes(os.fsencode(path))
 
-        uri = super().as_uri()
-        if isinstance(self, LocationWindowsPath) and str(self).startswith(r'\\'):
-            # UNC format case: use the format where the host part is included
-            # in the path part, to let urlopen() works.
-            if not uri.startswith('file:////'):
-                return uri.replace('file://', 'file:////')
-        return uri
+        return prefix + quote_from_bytes(os.fsencode(path))
 
     def normalize(self) -> 'LocationPath':
         normalized_path = self._path_module.normpath(str(self))
         return self.__class__(normalized_path)
 
 
 class LocationPosixPath(LocationPath, PurePosixPath):
@@ -123,48 +118,52 @@
 
 class LocationWindowsPath(LocationPath, PureWindowsPath):
     _path_module = ntpath
     __slots__ = ()
 
 
 def normalize_url(url: str, base_url: Optional[str] = None,
-                  keep_relative: bool = False) -> str:
+                  keep_relative: bool = False, method: str = 'xml') -> str:
     """
     Returns a normalized URL eventually joining it to a base URL if it's a relative path.
-    Path names are converted to 'file' scheme URLs.
+    Path names are converted to 'file' scheme URLs and unsafe characters are encoded.
+    Query and fragments parts are kept only for non-local URLs
 
     :param url: a relative or absolute URL.
     :param base_url: a reference base URL.
     :param keep_relative: if set to `True` keeps relative file paths, which would \
     not strictly conformant to specification (RFC 8089), because *urlopen()* doesn't \
     accept a simple pathname.
+    :param method: method used to encode query and fragment parts. If set to `html` \
+    the whitespaces are replaced with `+` characters.
     :return: a normalized URL string.
     """
     url_parts = urlsplit(url)
     if not is_local_scheme(url_parts.scheme):
-        return url_parts.geturl()
+        return encode_url(url_parts.geturl(), method)
 
     path = LocationPath.from_uri(url)
     if path.is_absolute():
         return path.normalize().as_uri()
 
     if base_url is not None:
         base_url_parts = urlsplit(base_url)
         base_path = LocationPath.from_uri(base_url)
+
         if is_local_scheme(base_url_parts.scheme):
             path = base_path.joinpath(path)
         elif not url_parts.scheme:
-            path = base_path.joinpath(path).normalize()
-            return urlunsplit((
+            url = urlunsplit((
                 base_url_parts.scheme,
                 base_url_parts.netloc,
-                quote_from_bytes(bytes(path)),
+                base_path.joinpath(path).normalize().as_posix(),
                 url_parts.query,
                 url_parts.fragment
             ))
+            return encode_url(url, method)
 
     if path.is_absolute() or keep_relative:
         return path.normalize().as_uri()
 
     base_path = LocationPath(os.getcwd())
     return base_path.joinpath(path).normalize().as_uri()
 
@@ -235,14 +234,75 @@
         return True
     path = unquote(urlsplit(normalize_url(url)).path)
     if path.startswith('/') and platform.system() == 'Windows':
         path = path[1:]
     return os.path.isfile(path)
 
 
+def is_encoded_url(url: str) -> bool:
+    """
+    Determines whether the given URL is encoded. The case with '+' and without
+    spaces is not univocal and the plus signs are ignored for the result.
+    """
+    return unquote(url) != url or \
+        '+' in url and ' ' not in url and \
+        unquote(url.replace('+', '$')) != url.replace('+', '$')
+
+
+def is_safe_url(url: str, method: str = 'xml') -> bool:
+    """Determines whether the given URL is safe."""
+    query_quote = quote_plus if method == 'html' else quote
+    query_unquote = unquote_plus if method == 'html' else unquote
+
+    parts = urlsplit(url)
+    path_safe = ':/\\' if is_local_scheme(parts.scheme) else '/'
+
+    return parts.netloc == quote(unquote(parts.netloc), safe='@:') and \
+        parts.path == quote(unquote(parts.path), safe=path_safe) and \
+        parts.query == query_quote(query_unquote(parts.query), safe=';/?:@=&') and \
+        parts.fragment == query_quote(query_unquote(parts.fragment), safe=';/?:@=&')
+
+
+def encode_url(url: str, method: str = 'xml') -> str:
+    """Encode the given url, if necessary."""
+    if is_safe_url(url, method):
+        return url
+    elif is_encoded_url(url):
+        url = decode_url(url, method)
+
+    query_quote = quote_plus if method == 'html' else quote
+    parts = urlsplit(url)
+    path_safe = ':/\\' if is_local_scheme(parts.scheme) else '/'
+
+    return urlunsplit((
+        parts.scheme,
+        quote(parts.netloc, safe='@:'),
+        quote(parts.path, safe=path_safe),
+        query_quote(parts.query, safe=';/?:@=&'),
+        query_quote(parts.fragment, safe=';/?:@=&'),
+    ))
+
+
+def decode_url(url: str, method: str = 'xml') -> str:
+    """Decode the given url, if necessary."""
+    if not is_encoded_url(url):
+        return url
+
+    query_unquote = unquote_plus if method == 'html' else unquote
+
+    parts = urlsplit(url)
+    return urlunsplit((
+        parts.scheme,
+        unquote(parts.netloc),
+        unquote(parts.path),
+        query_unquote(parts.query),
+        query_unquote(parts.fragment),
+    ))
+
+
 def normalize_locations(locations: LocationsType,
                         base_url: Optional[str] = None,
                         keep_relative: bool = False) -> NormalizedLocationsType:
     """
     Returns a list of normalized locations. The locations are normalized using
     the base URL of the instance.
```

### Comparing `xmlschema-3.3.0/xmlschema/names.py` & `xmlschema-3.3.1/xmlschema/names.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/namespaces.py` & `xmlschema-3.3.1/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/resources.py` & `xmlschema-3.3.1/xmlschema/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,20 +747,20 @@
         Lazy resources have only the namespace declarations for the root element.
         """
         return self._xmlns.get(elem)
 
     def get_absolute_path(self, path: Optional[str] = None) -> str:
         if path is None:
             if self._lazy:
-                return '/%s/%s' % (self._root.tag, '/'.join('*' * int(self._lazy)))
-            return '/%s' % self._root.tag
+                return f"/{self._root.tag}/{'/'.join('*' * int(self._lazy))}"
+            return f'/{self._root.tag}'
         elif path.startswith('/'):
             return path
         else:
-            return '/%s/%s' % (self._root.tag, path)
+            return f'/{self._root.tag}/{path}'
 
     def get_text(self) -> str:
         """
         Gets the source text of the XML document. If the source text is not
         available creates an encoded string representation of the XML tree.
         Il the resource is lazy raises a resource error.
         """
@@ -988,15 +988,15 @@
           4. The elements at *depth_level* and then a pruned root\n
           5. An incomplete root at start, the elements at *depth_level* and a pruned root\n
 
         :param mode: an integer in range [1..5] that defines the iteration mode.
         :param ancestors: provide a list for tracking the ancestors of yielded elements.
         """
         if mode not in (1, 2, 3, 4, 5):
-            raise XMLSchemaValueError("invalid argument mode={!r}".format(mode))
+            raise XMLSchemaValueError(f"invalid argument mode={mode!r}")
 
         if ancestors is not None:
             ancestors.clear()
         elif mode <= 2:
             ancestors = []
 
         if not self._lazy:
@@ -1087,15 +1087,15 @@
             return
 
         resource = self.open()
         lazy_depth = int(self._lazy)
         level = 0
 
         path = path.replace(' ', '').replace('./', '')
-        select_all = '*' in path and set(path).issubset({'*', '/'})
+        select_all = '*' in path and set(path).issubset(('*', '/'))
         if path == '.':
             path_depth = 0
         elif path.startswith('/'):
             path_depth = path.count('/') - 1
         else:
             path_depth = path.count('/') + 1
```

### Comparing `xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd` & `xmlschema-3.3.1/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd` & `xmlschema-3.3.1/xmlschema/schemas/DSIG/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-3.3.1/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-3.3.1/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-3.3.1/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-3.3.1/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-3.3.1/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-3.3.1/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema-11.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XENC/xenc-schema-11.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XENC/xenc-schema.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XENC/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-3.3.1/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/testing/__init__.py` & `xmlschema-3.3.1/xmlschema/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/testing/_builders.py` & `xmlschema-3.3.1/xmlschema/testing/_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                                       defuse=defuse, loglevel=loglevel)
             else:
                 schema = schema_class(xsd_file, locations=locations,
                                       defuse=defuse, loglevel=loglevel)
             self.errors.extend(schema.maps.all_errors)
 
             if inspect:
-                components_ids = set([id(c) for c in schema.maps.iter_components()])
+                components_ids = {id(c) for c in schema.maps.iter_components()}
                 components_ids.update(id(c) for c in schema.meta_schema.iter_components())
                 missing = [
                     c for c in SchemaObserver.components if id(c) not in components_ids
                 ]
                 if missing:
                     raise ValueError("schema missing %d components: %r" % (len(missing), missing))
 
@@ -217,15 +217,15 @@
                 self.check_xsd_file()
 
             # Check with lxml.etree.XMLSchema class
             if check_with_lxml and lxml_etree is not None:
                 self.check_xsd_file_with_lxml(xmlschema_time=time.time() - start_time)
             self.check_errors(xsd_file, expected_errors)
 
-    TestSchema.__name__ = TestSchema.__qualname__ = str('TestSchema{0:03}'.format(test_num))
+    TestSchema.__name__ = TestSchema.__qualname__ = str(f'TestSchema{test_num:03}')
     return TestSchema
 
 
 def make_validation_test_class(test_file, test_args, test_num, schema_class, check_with_lxml):
     """
     Creates a test class for checking xml instance validation.
 
@@ -663,9 +663,9 @@
                     not self.errors and not self.schema.all_errors and \
                     all('schemaLocation' in e.attrib
                         for e in self.schema.root
                         if e.tag == XSD_IMPORT):
 
                 self.check_validation_with_generated_code()
 
-    TestValidator.__name__ = TestValidator.__qualname__ = 'TestValidator{0:03}'.format(test_num)
+    TestValidator.__name__ = TestValidator.__qualname__ = f'TestValidator{test_num:03}'
     return TestValidator
```

### Comparing `xmlschema-3.3.0/xmlschema/testing/_case_class.py` & `xmlschema-3.3.1/xmlschema/testing/_case_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 return SCHEMA_TEMPLATE.format(self.schema_class.XSD_VERSION, source)
 
     def get_schema(self, source, **kwargs):
         return self.schema_class(self.get_schema_source(source), **kwargs)
 
     def get_element(self, name, **attrib):
         source = '<xs:element name="{}" {}/>'.format(
-            name, ' '.join('%s="%s"' % (k, v) for k, v in attrib.items())
+            name, ' '.join(f'{k}="{v}"' for k, v in attrib.items())
         )
         schema = self.schema_class(self.get_schema_source(source))
         return schema.elements[name]
 
     def check_etree_elements(self, elem, other):
         """Checks if two ElementTree elements are equal."""
         try:
@@ -138,15 +138,15 @@
         except AssertionError as err:
             self.assertIsNone(err, None)
 
     def check_namespace_prefixes(self, s):
         """Checks that a string doesn't contain protected prefixes (ns0, ns1 ...)."""
         match = PROTECTED_PREFIX_PATTERN.search(s)
         if match:
-            msg = "Protected prefix {!r} found:\n {}".format(match.group(0), s)
+            msg = f"Protected prefix {match.group(0)!r} found:\n {s}"
             self.assertIsNone(match, msg)
 
     def check_schema(self, source, expected=None, **kwargs):
         """
         Create a schema for a test case.
 
         :param source: A relative path or a root Element or a portion of schema for a template.
@@ -174,15 +174,15 @@
         for e in self.errors:
             error_string = str(e)
             self.assertTrue(e.path, "Missing path for: %s" % error_string)
             if e.namespaces:
                 self.check_namespace_prefixes(error_string)
 
         if not self.errors and expected:
-            raise ValueError("{!r}: found no errors when {} expected.".format(path, expected))
+            raise ValueError(f"{path!r}: found no errors when {expected} expected.")
         elif len(self.errors) != expected:
             num_errors = len(self.errors)
             if num_errors == 1:
                 msg = "{!r}: n.{} errors expected, found {}:\n\n{}"
             elif num_errors <= 5:
                 msg = "{!r}: n.{} errors expected, found {}. Errors follow:\n\n{}"
             else:
```

### Comparing `xmlschema-3.3.0/xmlschema/testing/_factory.py` & `xmlschema-3.3.1/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/testing/_helpers.py` & `xmlschema-3.3.1/xmlschema/testing/_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     if isinstance(items, dict_class):
         for k, v in items.items():
             yield from iter_nested_items(v, dict_class, list_class)
     elif isinstance(items, list_class):
         for item in items:
             yield from iter_nested_items(item, dict_class, list_class)
     elif isinstance(items, dict):
-        raise TypeError("%r: is a dict() instead of %r." % (items, dict_class))
+        raise TypeError(f"{items!r}: is a dict() instead of {dict_class!r}.")
     elif isinstance(items, list):
-        raise TypeError("%r: is a list() instead of %r." % (items, list_class))
+        raise TypeError(f"{items!r}: is a list() instead of {list_class!r}.")
     else:
         yield items
 
 
 def etree_elements_assert_equal(elem: Element, other: Element,
                                 strict: bool = True, skip_comments: bool = True,
                                 unordered: bool = False,
@@ -65,23 +65,23 @@
         if skip_comments and callable(e1.tag):
             continue
 
         for e2 in other_children:
             if not skip_comments or not callable(e2.tag):
                 break
         else:
-            raise AssertionError("Node %r has more children than %r" % (elem, other))
+            raise AssertionError(f"Node {elem!r} has more children than {other!r}")
 
         if strict or e1 is elem:
             if e1.tag != e2.tag:
-                raise AssertionError("%r != %r: tags differ" % (e1, e2))
+                raise AssertionError(f"{e1!r} != {e2!r}: tags differ")
         else:
             namespace = get_namespace(e1.tag) or namespace
             if get_qname(namespace, e1.tag) != get_qname(namespace, e2.tag):
-                raise AssertionError("%r != %r: tags differ." % (e1, e2))
+                raise AssertionError(f"{e1!r} != {e2!r}: tags differ")
 
         # Attributes
         if e1.attrib != e2.attrib:
             if strict:
                 msg = "{!r} != {!r}: attributes differ: {!r} != {!r}"
                 raise AssertionError(msg.format(e1, e2, e1.attrib, e2.attrib))
             else:
@@ -120,15 +120,15 @@
             nc2 = len(e2)
         if nc1 != nc2:
             msg = "%r != %r: children number differ: %r != %r"
             raise AssertionError(msg % (e1, e2, nc1, nc2))
 
         # Text
         if e1.text != e2.text:
-            message = "%r != %r: texts differ: %r != %r" % (e1, e2, e1.text, e2.text)
+            message = f"{e1!r} != {e2!r}: texts differ: {e1.text!r} != {e2.text!r}"
             if strict:
                 raise AssertionError(message)
             elif e1.text is None:
                 if e2.text is not None and e2.text.strip():
                     raise AssertionError(message)
             elif e2.text is None:
                 if e1.text.strip():
@@ -157,15 +157,15 @@
                         if not all(float(x1) == float(x2) for x1, x2 in zip(items1, items2)):
                             raise ValueError()
                     except (AssertionError, ValueError, TypeError):
                         raise AssertionError(message) from None
 
         # Tail
         if e1.tail != e2.tail:
-            message = "%r != %r: tails differ: %r != %r" % (e1, e2, e1.tail, e2.tail)
+            message = f"{e1!r} != {e2!r}: tails differ: {e1.tail!r} != {e2.tail!r}"
             if strict:
                 raise AssertionError(message)
             elif e1.tail is None:
                 if e2.tail is not None and e2.tail.strip():
                     raise AssertionError(message)
             elif e2.tail is None:
                 if e1.tail.strip():
@@ -176,8 +176,8 @@
         etree_elements_assert_equal(e1, e2, strict, skip_comments, unordered)
 
     try:
         next(other_children)
     except StopIteration:
         pass
     else:
-        raise AssertionError("Node %r has lesser children than %r." % (elem, other))
+        raise AssertionError(f"Node {elem!r} has lesser children than {other!r}.")
```

### Comparing `xmlschema-3.3.0/xmlschema/testing/_observers.py` & `xmlschema-3.3.1/xmlschema/testing/_observers.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     dummy_components = []
 
     @classmethod
     def observed_builder(cls, builder):
         if isinstance(builder, type):
             class BuilderProxy(builder):
                 def __init__(self, *args, **kwargs):
-                    super(BuilderProxy, self).__init__(*args, **kwargs)
+                    super().__init__(*args, **kwargs)
                     assert isinstance(self, XsdComponent)
 
                     if not cls.is_dummy_component(self):
                         cls.components.append(self)
                     else:
                         cls.dummy_components.append(self)
```

### Comparing `xmlschema-3.3.0/xmlschema/translation.py` & `xmlschema-3.3.1/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/validators/__init__.py` & `xmlschema-3.3.1/xmlschema/validators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Copyright (c), 2016-2020, SISSA (International School for Advanced Studies).
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/assertions.py` & `xmlschema-3.3.1/xmlschema/validators/assertions.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: 'XsdComplexType',
                  base_type: 'XsdComplexType') -> None:
 
         self._xpath_lock = threading.Lock()
         self.base_type = base_type
-        super(XsdAssert, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         if len(self.path) < 40:
             return '%s(test=%r)' % (self.__class__.__name__, self.path)
         else:
             return '%s(test=%r)' % (self.__class__.__name__, self.path[:37] + '...')
 
@@ -127,15 +127,15 @@
                     f"ent so these operators will return empty sequences."
                 )
                 warnings.warn(msg, category=XMLSchemaAssertPathWarning, stacklevel=4)
         finally:
             if self.parser.variable_types:
                 self.parser.variable_types.clear()
 
-    def __call__(self, elem: ElementType,
+    def __call__(self, obj: ElementType,
                  value: Any = None,
                  namespaces: Optional[NamespacesType] = None,
                  source: Optional['XMLResource'] = None,
                  **kwargs: Any) -> Iterator[XMLSchemaValidationError]:
 
         if self.parser is None or self.token is None:
             raise XMLSchemaNotBuiltError(self, 'schema bound parser not set')
@@ -154,24 +154,24 @@
             'uri': source.url if source is not None else None,
             'fragment': True,
             'variables': variables,
         }
 
         if source is not None:
             context = XPathContext(
-                source.get_xpath_node(elem), _namespaces, **context_kwargs
+                source.get_xpath_node(obj), _namespaces, **context_kwargs
             )
         else:
-            context = XPathContext(LazyElementNode(elem), **context_kwargs)
+            context = XPathContext(LazyElementNode(obj), **context_kwargs)
 
         try:
             if not self.token.evaluate(context):
-                yield XMLSchemaValidationError(self, obj=elem, reason="assertion test if false")
+                yield XMLSchemaValidationError(self, obj=obj, reason="assertion test if false")
         except ElementPathError as err:
-            yield XMLSchemaValidationError(self, obj=elem, reason=str(err))
+            yield XMLSchemaValidationError(self, obj=obj, reason=str(err))
 
     # For implementing ElementPathMixin
     def __iter__(self) -> Iterator[Union['XsdElement', 'XsdAnyElement']]:
         if isinstance(self.parent.content, XsdGroup):
             yield from self.parent.content.iter_elements()
 
     @property
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/attributes.py` & `xmlschema-3.3.1/xmlschema/validators/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
             else:
                 if name == 'xmlns':
                     msg = _("an attribute name must be different from 'xmlns'")
                     self.parse_error(msg)
 
                 if self.parent is None or self.qualified:
                     if self.target_namespace == XSI_NAMESPACE and \
-                            name not in {'nil', 'type', 'schemaLocation',
-                                         'noNamespaceSchemaLocation'}:
+                            name not in ('nil', 'type', 'schemaLocation',
+                                         'noNamespaceSchemaLocation'):
                         msg = _("cannot add attributes in %r namespace")
                         self.parse_error(msg % XSI_NAMESPACE)
                     self.name = get_qname(self.target_namespace, name)
                 else:
                     self.name = name
 
             child = self._parse_child_component(self.elem)
@@ -313,15 +313,15 @@
 
     def _parse(self) -> None:
         super()._parse()
         if self.use == 'prohibited' and 'fixed' in self.elem.attrib:
             msg = _("attribute 'fixed' with use=prohibited is not allowed in XSD 1.1")
             self.parse_error(msg)
         if 'inheritable' in self.elem.attrib:
-            if self.elem.attrib['inheritable'].strip() in {'true', '1'}:
+            if self.elem.attrib['inheritable'].strip() in ('true', '1'):
                 self.inheritable = True
         self._parse_target_namespace()
 
 
 class XsdAttributeGroup(
         MutableMapping[Optional[str], Union[XsdAttribute, XsdAnyAttribute]], XsdComponent,
         ValidationMixin[MutableMapping[str, str], List[Tuple[str, Any]]]
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/builtins.py` & `xmlschema-3.3.1/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/validators/complex_types.py` & `xmlschema-3.3.1/xmlschema/validators/complex_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 self.attributes = kwargs['attributes']
             if 'mixed' in kwargs:
                 self.mixed = kwargs['mixed']
             if 'block' in kwargs:
                 self._block = kwargs['block']
             if 'final' in kwargs:
                 self._final = kwargs['final']
-        super(XsdComplexType, self).__init__(elem, schema, parent, name)
+        super().__init__(elem, schema, parent, name)
         assert self.content is not None
 
     def __repr__(self) -> str:
         if self.name is not None:
             return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
         elif not hasattr(self, 'content') or not hasattr(self, 'attributes'):
             return '%s(id=%r)' % (self.__class__.__name__, id(self))
@@ -103,15 +103,15 @@
             )
 
     def _parse(self) -> None:
         if self.elem.tag == XSD_RESTRICTION:
             return  # a local restriction is already parsed by the caller
 
         if 'abstract' in self.elem.attrib:
-            if self.elem.attrib['abstract'].strip() in {'true', '1'}:
+            if self.elem.attrib['abstract'].strip() in ('true', '1'):
                 self.abstract = True
 
         if 'block' in self.elem.attrib:
             try:
                 self._block = get_xsd_derivation_attribute(self.elem, 'block', XSD_TYPE_DERIVATIONS)
             except ValueError as err:
                 self.parse_error(err)
@@ -617,15 +617,15 @@
         kwargs: Any = {
             'use_defaults': use_defaults,
             'namespaces': namespaces,
             'max_depth': max_depth,
             'extra_validator': extra_validator
         }
         if not isinstance(obj, (str, bytes)):
-            super(XsdComplexType, self).validate(obj, **kwargs)
+            super().validate(obj, **kwargs)
         elif isinstance(self.content, XsdSimpleType):
             self.content.validate(obj, **kwargs)
         elif not self.mixed and self.base_type is not None:
             self.base_type.validate(obj, **kwargs)
 
     def is_valid(self, obj: Union[ElementType, str, bytes],
                  use_defaults: bool = True,
@@ -635,15 +635,15 @@
         kwargs: Any = {
             'use_defaults': use_defaults,
             'namespaces': namespaces,
             'max_depth': max_depth,
             'extra_validator': extra_validator
         }
         if not isinstance(obj, (str, bytes)):
-            return super(XsdComplexType, self).is_valid(obj, **kwargs)
+            return super().is_valid(obj, **kwargs)
         elif isinstance(self.content, XsdSimpleType):
             return self.content.is_valid(obj, **kwargs)
         else:
             return self.mixed or self.base_type is not None and \
                 self.base_type.is_valid(obj, **kwargs)
 
     def is_derived(self, other: Union[BaseXsdType, Tuple[ElementType, SchemaType]],
@@ -712,15 +712,15 @@
             return cast(Optional[AtomicValueType], self.content.decode(text, 'skip'))
         else:
             return text
 
     def decode(self, obj: Union[ElementType, str, bytes], *args: Any, **kwargs: Any) \
             -> DecodeType[Any]:
         if not isinstance(obj, (str, bytes)):
-            return super(XsdComplexType, self).decode(obj, *args, **kwargs)
+            return super().decode(obj, *args, **kwargs)
         elif isinstance(self.content, XsdSimpleType):
             return self.content.decode(obj, *args, **kwargs)
         else:
             msg = _("cannot decode %(obj)r data with %(decoder)r")
             raise XMLSchemaDecodeError(
                 self, obj, str, msg % {'obj': obj, 'decoder': self}
             )
@@ -830,15 +830,15 @@
                 schema = self.schema.includes[child.attrib['schemaLocation']]
                 if schema.override is self.schema:
                     return schema.default_open_content
         else:
             return self.schema.default_open_content
 
     def _parse(self) -> None:
-        super(Xsd11ComplexType, self)._parse()
+        super()._parse()
 
         if self.base_type and self.base_type.base_type is self.any_simple_type and \
                 self.base_type.derivation == 'extension' and not self.attributes:
             # Derivation from xs:anySimpleType with missing variety.
             # See: http://www.w3.org/TR/xmlschema11-1/#Simple_Type_Definition_details
             msg = _("the simple content of {!r} is not a valid simple type in XSD 1.1")
             self.parse_error(msg.format(self.base_type))
@@ -860,15 +860,15 @@
                         self.attributes[name] = attr
                     elif not self.attributes[name].inheritable:
                         msg = _("attribute %r must be inheritable")
                         self.parse_error(msg % name)
 
         if 'defaultAttributesApply' not in self.elem.attrib:
             self.default_attributes_apply = True
-        elif self.elem.attrib['defaultAttributesApply'].strip() in {'false', '0'}:
+        elif self.elem.attrib['defaultAttributesApply'].strip() in ('false', '0'):
             self.default_attributes_apply = False
         else:
             self.default_attributes_apply = True
 
         # Add default attributes
         if self.default_attributes_apply and \
                 isinstance(self.default_attributes, XsdAttributeGroup):
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/elements.py` & `xmlschema-3.3.1/xmlschema/validators/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                  schema: SchemaType,
                  parent: Optional[XsdComponent] = None,
                  build: bool = True) -> None:
 
         if not build:
             self._build = False
         self.selected_by = set()
-        super(XsdElement, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         return '%s(%s=%r, occurs=%r)' % (
             self.__class__.__name__,
             'name' if self.ref is None else 'ref',
             self.prefixed_name,
             list(self.occurs)
@@ -137,15 +137,15 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == "type":
             if isinstance(value, XsdSimpleType):
                 self.attributes = self.schema.create_empty_attribute_group(self)
             else:
                 self.attributes = value.attributes
-        super(XsdElement, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     def __iter__(self) -> Iterator[SchemaElementType]:
         if self.type.has_complex_content():
             yield from self.type.content.iter_elements()  # type: ignore[union-attr]
 
     def _parse(self) -> None:
         if not self._build:
@@ -179,16 +179,16 @@
                 self.default = xsd_element.default
                 self.fixed = xsd_element.fixed
                 self.substitution_group = xsd_element.substitution_group
                 self.identities = xsd_element.identities
                 self.alternatives = xsd_element.alternatives
                 self.selected_by = xsd_element.selected_by
 
-            for attr_name in {'type', 'nillable', 'default', 'fixed', 'form',
-                              'block', 'abstract', 'final', 'substitutionGroup'}:
+            for attr_name in ('type', 'nillable', 'default', 'fixed', 'form',
+                              'block', 'abstract', 'final', 'substitutionGroup'):
                 if attr_name in attrib:
                     msg = _("attribute {!r} is not allowed when element reference is used")
                     self.parse_error(msg.format(attr_name))
             return
 
         if 'form' in attrib:
             self.form = attrib['form']
@@ -205,43 +205,43 @@
         except KeyError:
             pass
 
         if 'abstract' in attrib:
             if self.parent is not None:
                 msg = _("local scope elements cannot have abstract attribute")
                 self.parse_error(msg)
-            if attrib['abstract'].strip() in {'true', '1'}:
+            if attrib['abstract'].strip() in ('true', '1'):
                 self.abstract = True
 
         if 'block' in attrib:
             try:
                 self._block = get_xsd_derivation_attribute(
                     self.elem, 'block', XSD_ELEMENT_DERIVATIONS
                 )
             except ValueError as err:
                 self.parse_error(err)
 
-        if 'nillable' in attrib and attrib['nillable'].strip() in {'true', '1'}:
+        if 'nillable' in attrib and attrib['nillable'].strip() in ('true', '1'):
             self.nillable = True
 
         if self.parent is None:
             if 'final' in attrib:
                 try:
                     self._final = get_xsd_derivation_attribute(
                         self.elem, 'final', XSD_TYPE_DERIVATIONS
                     )
                 except ValueError as err:
                     self.parse_error(err)
 
-            for attr_name in {'ref', 'form', 'minOccurs', 'maxOccurs'}:
+            for attr_name in ('ref', 'form', 'minOccurs', 'maxOccurs'):
                 if attr_name in attrib:
                     msg = _("attribute {!r} is not allowed in a global element declaration")
                     self.parse_error(msg.format(attr_name))
         else:
-            for attr_name in {'final', 'substitutionGroup'}:
+            for attr_name in ('final', 'substitutionGroup'):
                 if attr_name in attrib:
                     msg = _("attribute {!r} not allowed in a local element declaration")
                     self.parse_error(msg.format(attr_name))
 
     def _parse_type(self) -> None:
         type_name = self.elem.get('type')
         if type_name is not None:
@@ -573,15 +573,15 @@
                 else:
                     self.schema.import_schema(ns, url, base_url, build=True)
 
             except (XMLSchemaValidationError, ParseError) as err:
                 yield self.validation_error(validation, err, elem, **options)
             except XMLSchemaParseError as err:
                 yield self.validation_error(validation, err.message, elem, **options)
-            except (OSError, IOError):
+            except OSError:
                 continue
 
     def iter_decode(self, obj: ElementType, validation: str = 'lax', **kwargs: Any) \
             -> IterDecodeType[Any]:
         """
         Creates an iterator for decoding an Element instance.
 
@@ -603,14 +603,15 @@
             value = kwargs['validation_hook'](obj, self)
             if value:
                 if isinstance(value, str) and value in XSD_VALIDATION_MODES:
                     validation = value
                 else:
                     return
 
+        kwargs['elem'] = obj
         try:
             level = kwargs['level']
         except KeyError:
             level = kwargs['level'] = 0
 
         try:
             identities = kwargs['identities']
@@ -854,15 +855,15 @@
                     assert isinstance(counter, KeyrefCounter)
                     for error in counter.iter_errors(identities):
                         yield self.validation_error(validation, error, obj, **kwargs)
         elif level:
             for identity in self.identities:
                 identities[identity].enabled = False
 
-    def collect_key_fields(self, elem: ElementType, xsd_type: BaseXsdType,
+    def collect_key_fields(self, obj: ElementType, xsd_type: BaseXsdType,
                            validation: str = 'lax', nilled: bool = False,
                            **kwargs: Any) -> Iterator[XMLSchemaValidationError]:
         element_node: Union[ElementNode, LazyElementNode]
         xsd_fields: Optional[IdentityCounterType]
 
         try:
             identities = kwargs['identities']
@@ -872,15 +873,15 @@
             return
 
         try:
             namespaces = kwargs['namespaces']
         except KeyError:
             namespaces = None
 
-        element_node = resource.get_xpath_node(elem)
+        element_node = resource.get_xpath_node(obj)
 
         xsd_element = self if self.ref is None else self.ref
         if xsd_element.type is not xsd_type:
             xsd_element = _copy(xsd_element)
             xsd_element.type = xsd_type
 
         # Collect field values for identities that refer to this element.
@@ -896,15 +897,15 @@
             if counter.elements is None:
                 # Apply selector on Element ancestor for obtain the selected elements
                 root_node = resource.get_xpath_node(counter.elem)
                 context = XPathContext(root_node)
                 assert identity.selector is not None and identity.selector.token is not None
                 counter.elements = set(identity.selector.token.select_results(context))
 
-            if elem not in counter.elements:
+            if obj not in counter.elements:
                 continue
 
             try:
                 if xsd_element.type is self.type and xsd_element in identity.elements:
                     xsd_fields = identity.elements[xsd_element]
                     if xsd_fields is None:
                         xsd_fields = identity.get_fields(xsd_element.xpath_node)
@@ -914,21 +915,21 @@
 
                 if all(x is None for x in xsd_fields):
                     continue
 
                 decoders = cast(Tuple[XsdAttribute, ...], xsd_fields)
                 fields = identity.get_fields(element_node, namespaces, decoders=decoders)
             except (XMLSchemaValueError, XMLSchemaTypeError) as err:
-                yield self.validation_error(validation, err, elem, **kwargs)
+                yield self.validation_error(validation, err, obj, **kwargs)
             else:
                 if any(x is not None for x in fields) or nilled:
                     try:
                         counter.increase(fields)
                     except ValueError as err:
-                        yield self.validation_error(validation, err, elem, **kwargs)
+                        yield self.validation_error(validation, err, obj, **kwargs)
 
     def to_objects(self, obj: ElementType, with_bindings: bool = False, **kwargs: Any) \
             -> DecodeType['dataobjects.DataElement']:
         """
         Decodes XML data to Python data objects.
 
         :param obj: the XML data source.
@@ -1016,15 +1017,15 @@
             else:
                 attributes = result
 
         if XSI_NIL in element_data.attributes:
             xsi_nil = element_data.attributes[XSI_NIL].strip()
             if not self.nillable:
                 errors.append("element is not nillable.")
-            elif xsi_nil not in {'0', '1', 'true', 'false'}:
+            elif xsi_nil not in ('0', '1', 'true', 'false'):
                 errors.append("xsi:nil attribute must has a boolean value.")
             elif xsi_nil in ('0', 'false'):
                 pass
             elif self.fixed is not None:
                 errors.append("xsi:nil='true' but the element has a fixed value.")
             elif element_data.text not in (None, '') or element_data.content:
                 errors.append("xsi:nil='true' but the element is not empty.")
@@ -1084,15 +1085,14 @@
                     group: Optional['XsdGroup'] = None, **kwargs: Any) -> bool:
         if not name:
             return False
         elif default_namespace and name[0] != '{':
             name = f'{{{default_namespace}}}{name}'
 
             # Workaround for backward compatibility of XPath selectors on schemas.
-            # It could be removed in v3.0.
             if not self.qualified and default_namespace == self.target_namespace:
                 return (name == self.qualified_name or
                         any(name == e.qualified_name for e in self.iter_substitutes()))
 
         return name == self.name or any(name == e.name for e in self.iter_substitutes())
 
     def match(self, name: Optional[str], default_namespace: Optional[str] = None,
@@ -1461,15 +1461,15 @@
                                f"assessment outcome of previous items")
                     yield self.validation_error(validation, reason, elem, **options)
 
             except (XMLSchemaValidationError, ParseError) as err:
                 yield self.validation_error(validation, err, elem, **options)
             except XMLSchemaParseError as err:
                 yield self.validation_error(validation, err.message, elem, **options)
-            except (OSError, IOError):
+            except OSError:
                 continue
 
 
 class XsdAlternative(XsdComponent):
     """
     XSD 1.1 type *alternative* definitions.
 
@@ -1485,15 +1485,15 @@
     parent: XsdElement
     type: BaseXsdType
     path: Optional[str] = None
     token: Optional[XPathToken] = None
     _ADMITTED_TAGS = {XSD_ALTERNATIVE}
 
     def __init__(self, elem: ElementType, schema: SchemaType, parent: XsdElement) -> None:
-        super(XsdAlternative, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         return '%s(type=%r, test=%r)' % (
             self.__class__.__name__, self.elem.get('type'), self.elem.get('test')
         )
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/exceptions.py` & `xmlschema-3.3.1/xmlschema/validators/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     :param message: the error message.
     :param elem: the element that contains the error.
     :param source: the XML resource or the decoded data that contains the error.
     :param namespaces: is an optional mapping from namespace prefix to URI.
     """
     _path: Optional[str]
 
+    # Optional dump of the execution stack that can be set in collected
+    # validator errors for debugging purposes.
+    stack_trace: Optional[str] = None
+
     def __init__(self, validator: ValidatorType,
                  message: str,
                  elem: Optional[ElementType] = None,
                  source: Optional[Any] = None,
                  namespaces: Optional[NamespacesType] = None) -> None:
         self._path = None
         self.validator = validator
@@ -85,15 +89,15 @@
                     root=self.source.root,
                     namespaces=self.namespaces,
                     relative=False,
                     add_position=True
                 )
                 if self.source.is_lazy():
                     value = None  # Don't save the element of a lazy resource
-        super(XMLSchemaValidatorError, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     @property
     def sourceline(self) -> Any:
         """XML element *sourceline* if available (lxml Element) and *elem* is set."""
         return getattr(self.elem, 'sourceline', None)
 
     @property
@@ -158,15 +162,15 @@
     """
     Raised when there is an improper usage attempt of a not built XSD validator.
 
     :param validator: the XSD validator.
     :param message: the error message.
     """
     def __init__(self, validator: 'XsdValidator', message: str) -> None:
-        super(XMLSchemaNotBuiltError, self).__init__(
+        super().__init__(
             validator=validator,
             message=message,
             elem=getattr(validator, 'elem', None),
             source=getattr(validator, 'source', None),
             namespaces=getattr(validator, 'namespaces', None)
         )
 
@@ -177,15 +181,15 @@
 
     :param validator: the XSD validator.
     :param message: the error message.
     :param elem: the element that contains the error.
     """
     def __init__(self, validator: 'XsdValidator', message: str,
                  elem: Optional[ElementType] = None) -> None:
-        super(XMLSchemaParseError, self).__init__(
+        super().__init__(
             validator=validator,
             message=message,
             elem=elem if elem is not None else getattr(validator, 'elem', None),
             source=getattr(validator, 'source', None),
             namespaces=getattr(validator, 'namespaces', None),
         )
 
@@ -194,28 +198,28 @@
     """
     Raised when a model error is found during the checking of a model group.
 
     :param group: the XSD model group.
     :param message: the error message.
     """
     def __init__(self, group: 'XsdGroup', message: str) -> None:
-        super(XMLSchemaModelError, self).__init__(
+        super().__init__(
             validator=group,
             message=message,
             elem=getattr(group, 'elem', None),
             source=getattr(group, 'source', None),
             namespaces=getattr(group, 'namespaces', None)
         )
 
 
 class XMLSchemaModelDepthError(XMLSchemaModelError):
     """Raised when recursion depth is exceeded while iterating a model group."""
     def __init__(self, group: 'XsdGroup') -> None:
-        msg = "maximum model recursion depth exceeded while iterating {!r}".format(group)
-        super(XMLSchemaModelDepthError, self).__init__(group, message=msg)
+        msg = f"maximum model recursion depth exceeded while iterating {group!r}"
+        super().__init__(group, message=msg)
 
 
 class XMLSchemaValidationError(XMLSchemaValidatorError, ValueError):
     """
     Raised when the XML data is not validated with the XSD component or schema.
     It's used by decoding and encoding methods. Encoding validation errors do
     not include XML data element and source, so the error is limited to a message
@@ -238,17 +242,17 @@
             obj_repr = repr(obj.encode('ascii', 'xmlcharrefreplace').decode('utf-8'))
         else:
             obj_repr = repr(obj)
 
         if len(obj_repr) > 200:
             obj_repr = f"{type(obj)} instance"
 
-        super(XMLSchemaValidationError, self).__init__(
+        super().__init__(
             validator=validator,
-            message="failed validating {} with {!r}".format(obj_repr, validator),
+            message=f"failed validating {obj_repr} with {validator!r}",
             elem=obj if is_etree_element(obj) else None,
             source=source,
             namespaces=namespaces,
         )
         self.obj = obj
         self.reason = reason
 
@@ -270,17 +274,17 @@
             instance_as_string = self.get_elem_as_string(indent='  ', max_lines=20)
         else:
             chunks.append(f"Instance type: {type(self.obj)}\n")
             instance_as_string = self.get_obj_as_string(indent='  ', max_lines=20)
 
         if hasattr(self.elem, 'sourceline'):
             line = getattr(self.elem, 'sourceline')
-            chunks.append("Instance (line %r):\n\n%s\n" % (line, instance_as_string))
+            chunks.append(f"Instance (line {line!r}):\n\n{instance_as_string}\n")
         else:
-            chunks.append("Instance:\n\n%s\n" % instance_as_string)
+            chunks.append(f"Instance:\n\n{instance_as_string}\n")
 
         if self.path is not None:
             chunks.append("Path: %s\n" % self.path)
 
         return '\n'.join(chunks) if len(chunks) > 1 else chunks[0][:-2]
 
     def get_obj_as_string(self, indent: str = '', max_lines: Optional[int] = None) -> str:
@@ -318,15 +322,15 @@
 
     def __init__(self, validator: Union['XsdValidator', Callable[[Any], None]],
                  obj: Any,
                  decoder: Any,
                  reason: Optional[str] = None,
                  source: Optional[Any] = None,
                  namespaces: Optional[NamespacesType] = None) -> None:
-        super(XMLSchemaDecodeError, self).__init__(validator, obj, reason, source, namespaces)
+        super().__init__(validator, obj, reason, source, namespaces)
         self.decoder = decoder
 
 
 class XMLSchemaEncodeError(XMLSchemaValidationError):
     """
     Raised when an object is not encodable to an XML data string.
 
@@ -341,15 +345,15 @@
 
     def __init__(self, validator: Union['XsdValidator', Callable[[Any], None]],
                  obj: Any,
                  encoder: Any,
                  reason: Optional[str] = None,
                  source: Optional[Any] = None,
                  namespaces: Optional[NamespacesType] = None) -> None:
-        super(XMLSchemaEncodeError, self).__init__(validator, obj, reason, source, namespaces)
+        super().__init__(validator, obj, reason, source, namespaces)
         self.encoder = encoder
 
 
 class XMLSchemaChildrenValidationError(XMLSchemaValidationError):
     """
     Raised when a child element is not validated.
 
@@ -415,16 +419,15 @@
             elif len(expected_tags) > 1:
                 reason += _(" Tag (%s) expected.") % ' | '.join(repr(tag) for tag in expected_tags)
             elif expected_tags[0].startswith('from '):
                 reason += _(" Tag %s expected.") % expected_tags[0]
             else:
                 reason += _(" Tag %r expected.") % expected_tags[0]
 
-        super(XMLSchemaChildrenValidationError, self).\
-            __init__(validator, elem, reason, source, namespaces)
+        super().__init__(validator, elem, reason, source, namespaces)
 
     @property
     def invalid_child(self) -> Optional[ElementType]:
         """
         The invalid child element, if any, `None` otherwise. It's `None` in case of
         incomplete content or if the parent has been cleared during lazy validation.
         """
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/facets.py` & `xmlschema-3.3.1/xmlschema/validators/facets.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Union['XsdList', 'XsdAtomicRestriction'],
                  base_type: Optional[BaseXsdType]) -> None:
         self.base_type = base_type
         self._validator = self._skip_validation
-        super(XsdFacet, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         return '%s(value=%r, fixed=%r)' % (self.__class__.__name__, self.value, self.fixed)
 
     def __call__(self, value: Any) -> None:
         try:
             self._validator(value)
@@ -450,15 +450,15 @@
     _ADMITTED_TAGS = XSD_FRACTION_DIGITS,
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: 'XsdAtomicRestriction',
                  base_type: BaseXsdType) -> None:
 
-        super(XsdFractionDigitsFacet, self).__init__(elem, schema, parent, base_type)
+        super().__init__(elem, schema, parent, base_type)
         if not base_type.is_derived(self.maps.types[XSD_DECIMAL]):
             msg = _("fractionDigits facet can be applied only to types derived from xs:decimal")
             self.parse_error(msg)
 
     def _parse_value(self, elem: ElementType) -> None:
         # Errors are detected by meta-schema validation. For schemas with
         # 'lax' validation mode use 9999 in case of an invalid value.
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/global_maps.py` & `xmlschema-3.3.1/xmlschema/validators/global_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         XSD_GROUP: 'lookup_group',
         XSD_ATTRIBUTE: 'lookup_attribute',
         XSD_ATTRIBUTE_GROUP: 'lookup_attribute_group',
         XSD_NOTATION: 'lookup_notation',
     }
 
     def __init__(self, validator: SchemaType, validation: str = 'strict') -> None:
-        super(XsdGlobals, self).__init__(validation)
+        super().__init__(validation)
 
         self.validator = validator
         self.namespaces = NamespaceResourcesMap()  # Registered schemas by namespace URI
         self.missing_locations = []     # Missing or failing resource locations
 
         self.types = {}                 # Global types (both complex and simple)
         self.attributes = {}            # Global attributes
@@ -514,15 +514,15 @@
                 if url in self.missing_locations:
                     continue
 
                 try:
                     if schema.import_schema(namespace, url, schema.base_url) is not None:
                         if build:
                             self.build()
-                except (OSError, IOError):
+                except OSError:
                     pass
                 except XMLSchemaNotBuiltError:
                     self.clear(remove_schemas=True, only_unbuilt=True)
                     self.missing_locations.append(url)
                 else:
                     return True
 
@@ -530,15 +530,15 @@
         if namespace in self.validator.fallback_locations:
             url = self.validator.fallback_locations[namespace]
             if url not in self.missing_locations:
                 try:
                     if self.validator.import_schema(namespace, url) is not None:
                         if build:
                             self.build()
-                except (OSError, IOError):
+                except OSError:
                     return False
                 except XMLSchemaNotBuiltError:
                     self.clear(remove_schemas=True, only_unbuilt=True)
                     self.missing_locations.append(url)
                 else:
                     return True
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/groups.py` & `xmlschema-3.3.1/xmlschema/validators/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                  parent: Optional[Union['XsdComplexType', 'XsdGroup']] = None) -> None:
 
         self._group: List[ModelParticleType] = []
         self.content = self._group
         self.oid = (self,)
         if parent is not None and parent.mixed:
             self.mixed = parent.mixed
-        super(XsdGroup, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         if self.name is None:
             return '%s(model=%r, occurs=%r)' % (
                 self.__class__.__name__, self.model, list(self.occurs)
             )
         elif self.ref is None:
@@ -270,15 +270,15 @@
 
     def has_occurs_restriction(
             self, other: Union[ModelParticleType, ParticleMixin, 'OccursCalculator']) -> bool:
 
         if not self:
             return True
         elif isinstance(other, XsdGroup):
-            return super(XsdGroup, self).has_occurs_restriction(other)
+            return super().has_occurs_restriction(other)
 
         # Group particle compared to element particle
         if self.max_occurs is None or any(e.max_occurs is None for e in self):
             if other.max_occurs is not None:
                 return False
             elif self.model == 'choice':
                 return self.min_occurs * min(e.min_occurs for e in self) >= other.min_occurs
@@ -992,15 +992,15 @@
         except KeyError:
             converter = self._get_converter(obj, kwargs)
 
         errors: List[Tuple[int, ModelParticleType, int, Optional[List[SchemaElementType]]]]
         xsd_element: Optional[SchemaElementType]
         expected: Optional[List[SchemaElementType]]
 
-        if self.open_content is None:
+        if self.open_content is None or self.open_content.mode == 'none':
             model = ModelVisitor(self)
         elif self.open_content.mode == 'interleave':
             model = InterleavedModelVisitor(self, self.open_content.any_element)
         else:
             model = SuffixedModelVisitor(self, self.open_content.any_element)
 
         errors = []
@@ -1118,15 +1118,15 @@
         except KeyError:
             level = kwargs['level'] = 1
 
         converter = kwargs['converter']
         padding = '\n' + ' ' * converter.indent * level
         default_namespace = converter.get('')
 
-        if self.open_content is None:
+        if self.open_content is None or self.open_content.mode == 'none':
             model = ModelVisitor(self)
         elif self.open_content.mode == 'interleave':
             model = InterleavedModelVisitor(self, self.open_content.any_element)
         else:
             model = SuffixedModelVisitor(self, self.open_content.any_element)
 
         index = cdata_index = 0
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/helpers.py` & `xmlschema-3.3.1/xmlschema/validators/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from ..aliases import ElementType
 from ..names import XSD_ANNOTATION
 from ..exceptions import XMLSchemaValueError
 from ..translation import gettext as _
 from .exceptions import XMLSchemaValidationError
 
 XSD_FINAL_ATTRIBUTE_VALUES = {'restriction', 'extension', 'list', 'union'}
+XSD_BOOLEAN_MAP = {
+    'false': False, '0': False,
+    'true': True, '1': True
+}
 
 
 def get_xsd_derivation_attribute(elem: Element, attribute: str,
                                  values: Optional[Set[str]] = None) -> str:
     """
     Get a derivation attribute (maybe 'block', 'blockDefault', 'final' or 'finalDefault')
     checking the items with the values arguments. Returns a string.
@@ -178,19 +182,17 @@
                                    _("no value is allowed for xs:error type"))
 
 
 #
 # XSD builtin decoding functions
 
 def boolean_to_python(value: str) -> bool:
-    if value in {'true', '1'}:
-        return True
-    elif value in {'false', '0'}:
-        return False
-    else:
+    try:
+        return XSD_BOOLEAN_MAP[value]
+    except KeyError:
         raise XMLSchemaValueError(_('{!r} is not a boolean value').format(value))
 
 
 def python_to_boolean(value: object) -> str:
     return str(value).lower()
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/identities.py` & `xmlschema-3.3.1/xmlschema/validators/identities.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         anchors=False
     )
     token: Optional[XPathToken] = None
     parser: Optional[IdentityXPathParser] = None
 
     def __init__(self, elem: ElementType, schema: SchemaType,
                  parent: Optional['XsdIdentity']) -> None:
-        super(XsdSelector, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def _parse(self) -> None:
         try:
             self.path = self.elem.attrib['xpath']
         except KeyError:
             self.parse_error(_("'xpath' attribute required"))
             self.path = '*'
@@ -165,15 +165,15 @@
 
     # XSD elements bound by selector (for speed-up and for lazy mode)
     elements: Union[Tuple[()], Dict['XsdElement', Optional[IdentityCounterType]]] = ()
     root_elements: Union[Tuple[()], Set['XsdElement']] = ()
 
     def __init__(self, elem: ElementType, schema: SchemaType,
                  parent: Optional['XsdElement']) -> None:
-        super(XsdIdentity, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def _parse(self) -> None:
         try:
             self.name = get_qname(self.target_namespace, self.elem.attrib['name'])
         except KeyError:
             self.parse_error(_("missing required attribute 'name'"))
             self.name = ''
@@ -352,25 +352,25 @@
     or in a descendant element.
     """
     _ADMITTED_TAGS = {XSD_KEYREF}
     refer: Optional[Union[str, XsdKey]] = None
     refer_path = '.'
 
     def _parse(self) -> None:
-        super(XsdKeyref, self)._parse()
+        super()._parse()
         try:
             self.refer = self.schema.resolve_qname(self.elem.attrib['refer'])
         except (KeyError, ValueError, RuntimeError) as err:
             if 'refer' not in self.elem.attrib:
                 self.parse_error(_("missing required attribute 'refer'"))
             else:
                 self.parse_error(err)
 
     def build(self) -> None:
-        super(XsdKeyref, self).build()
+        super().build()
 
         if isinstance(self.refer, (XsdKey, XsdUnique)):
             return  # referenced key/unique identity constraint already set
         elif isinstance(self.ref, XsdKeyref):
             self.refer = self.ref.refer
 
         if self.refer is None:
@@ -427,31 +427,31 @@
 
 
 class Xsd11Unique(XsdUnique):
     def _parse(self) -> None:
         if self._parse_reference():
             self.ref = True  # type: ignore[assignment]
         else:
-            super(Xsd11Unique, self)._parse()
+            super()._parse()
 
 
 class Xsd11Key(XsdKey):
     def _parse(self) -> None:
         if self._parse_reference():
             self.ref = True  # type: ignore[assignment]
         else:
-            super(Xsd11Key, self)._parse()
+            super()._parse()
 
 
 class Xsd11Keyref(XsdKeyref):
     def _parse(self) -> None:
         if self._parse_reference():
             self.ref = True  # type: ignore[assignment]
         else:
-            super(Xsd11Keyref, self)._parse()
+            super()._parse()
 
 
 class IdentityCounter:
 
     def __init__(self, identity: XsdIdentity, elem: ElementType) -> None:
         self.counter: Counter[IdentityCounterType] = Counter[IdentityCounterType]()
         self.identity = identity
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/models.py` & `xmlschema-3.3.1/xmlschema/validators/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,15 @@
 
     def restart(self) -> None:
         self.clear()
         self._start()
 
     def stop(self) -> Iterator[AdvanceYieldedType]:
         while self.element is not None:
-            for e in self.advance():
-                yield e
+            yield from self.advance()
 
     def iter_group(self) -> Iterator[ModelParticleType]:
         """Returns an iterator for the current model group."""
         if self.group.model == 'all':
             for e in self.group.iter_elements():
                 if not e.is_over(self.occurs):
                     yield e
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/notations.py` & `xmlschema-3.3.1/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/validators/particles.py` & `xmlschema-3.3.1/xmlschema/validators/particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/validators/schemas.py` & `xmlschema-3.3.1/xmlschema/validators/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 from ..exports import export_schema
 from .. import dataobjects
 
 from .exceptions import XMLSchemaParseError, XMLSchemaValidationError, \
     XMLSchemaEncodeError, XMLSchemaNotBuiltError, XMLSchemaStopValidation, \
     XMLSchemaIncludeWarning, XMLSchemaImportWarning
 from .helpers import get_xsd_derivation_attribute, get_xsd_annotation_child
-from .xsdbase import check_validation_mode, XsdValidator, XsdComponent, XsdAnnotation
+from .xsdbase import XSD_ELEMENT_DERIVATIONS, check_validation_mode, XsdValidator, \
+    XsdComponent, XsdAnnotation
 from .notations import XsdNotation
 from .identities import XsdIdentity, XsdKey, XsdKeyref, XsdUnique, \
     Xsd11Key, Xsd11Unique, Xsd11Keyref, IdentityCounter, KeyrefCounter, IdentityMapType
 from .facets import XSD_10_FACETS, XSD_11_FACETS
 from .simple_types import XsdSimpleType, XsdList, XsdUnion, XsdAtomicRestriction, \
     Xsd11AtomicRestriction, Xsd11Union
 from .attributes import XsdAttribute, XsdAttributeGroup, Xsd11Attribute
@@ -122,27 +123,25 @@
                 # Use base's meta_schema class as base for the new meta-schema
                 meta_bases = (meta_schema.__class__,)
                 if len(bases) > 1:
                     meta_bases += bases[1:]
 
             meta_schema_class = cast(
                 'XMLSchemaBase',
-                super(XMLSchemaMeta, mcs).__new__(
-                    mcs, meta_schema_class_name, meta_bases, dict_
-                )
+                super().__new__(mcs, meta_schema_class_name, meta_bases, dict_)
             )
             meta_schema_class.__qualname__ = meta_schema_class_name
             module = sys.modules[dict_['__module__']]
             setattr(module, meta_schema_class_name, meta_schema_class)
 
             meta_schema = meta_schema_class.create_meta_schema(meta_schema_file)
             dict_['meta_schema'] = meta_schema
 
         # Create the class and check some basic attributes
-        cls = super(XMLSchemaMeta, mcs).__new__(mcs, name, bases, dict_)
+        cls = super().__new__(mcs, name, bases, dict_)
         if cls.XSD_VERSION not in ('1.0', '1.1'):
             raise XMLSchemaValueError(_("XSD_VERSION must be '1.0' or '1.1'"))
         return cls
 
 
 class XMLSchemaBase(XsdValidator, ElementPathMixin[Union[SchemaType, XsdElement]],
                     metaclass=XMLSchemaMeta):
@@ -318,15 +317,15 @@
                  uri_mapper: Optional[UriMapperType] = None,
                  build: bool = True,
                  use_meta: bool = True,
                  use_fallback: bool = True,
                  use_xpath3: bool = False,
                  loglevel: Optional[Union[str, int]] = None) -> None:
 
-        super(XMLSchemaBase, self).__init__(validation)
+        super().__init__(validation)
         self.lock = threading.Lock()  # Lock for build operations
 
         if loglevel is not None:
             set_logging_level(loglevel)
         elif build and global_maps is None:
             logger.setLevel(logging.WARNING)
 
@@ -401,15 +400,15 @@
 
         if 'blockDefault' in root.attrib:
             if self.meta_schema is None:
                 pass  # Skip for XSD 1.0 meta-schema that has blockDefault="#all"
             else:
                 try:
                     self.block_default = get_xsd_derivation_attribute(
-                        root, 'blockDefault', {'extension', 'restriction', 'substitution'}
+                        root, 'blockDefault', XSD_ELEMENT_DERIVATIONS
                     )
                 except ValueError as err:
                     self.parse_error(err, root)
 
         if 'finalDefault' in root.attrib:
             try:
                 self.final_default = get_xsd_derivation_attribute(root, 'finalDefault')
@@ -470,15 +469,15 @@
 
         if any(ns == VC_NAMESPACE for ns in self.namespaces.values()):
             # For XSD 1.1+ apply versioning filter to schema tree. See the paragraph
             # 4.2.2 of XSD 1.1 (Part 1: Structures) definition for details.
             # Ref: https://www.w3.org/TR/xmlschema11-1/#cip
             if prune_etree(root, selector=lambda x: not self.version_check(x)):
                 for k in list(root.attrib):
-                    if k not in {'targetNamespace', VC_MIN_VERSION, VC_MAX_VERSION}:
+                    if k not in ('targetNamespace', VC_MIN_VERSION, VC_MAX_VERSION):
                         del root.attrib[k]
 
         # Validate the schema document (transforming validation errors to parse errors)
         if validation != 'skip':
             for e in self.meta_schema.iter_errors(root, namespaces=self.namespaces):
                 self.parse_error(e.reason or e, elem=e.elem)
 
@@ -544,30 +543,30 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'maps':
             if self.meta_schema is None and hasattr(self, 'maps'):
                 msg = _("cannot change the global maps instance of a meta-schema")
                 raise XMLSchemaValueError(msg)
 
-            super(XMLSchemaBase, self).__setattr__(name, value)
+            super().__setattr__(name, value)
             self.notations = NamespaceView(value.notations, self.target_namespace)
             self.types = NamespaceView(value.types, self.target_namespace)
             self.attributes = NamespaceView(value.attributes, self.target_namespace)
             self.attribute_groups = NamespaceView(value.attribute_groups,
                                                   self.target_namespace)
             self.groups = NamespaceView(value.groups, self.target_namespace)
             self.elements = NamespaceView(value.elements, self.target_namespace)
             self.substitution_groups = NamespaceView(value.substitution_groups,
                                                      self.target_namespace)
             self.identities = NamespaceView(value.identities, self.target_namespace)
             value.register(self)
         else:
             if name == 'validation':
                 check_validation_mode(value)
-            super(XMLSchemaBase, self).__setattr__(name, value)
+            super().__setattr__(name, value)
 
     def __iter__(self) -> Iterator[XsdElement]:
         yield from sorted(self.elements.values(), key=name_attribute)
 
     def __reversed__(self) -> Iterator[XsdElement]:
         yield from sorted(self.elements.values(), key=name_attribute, reverse=True)
 
@@ -748,15 +747,15 @@
         when the schema model is complex.
         """
         if not self.elements:
             return []
         elif len(self.elements) == 1:
             return list(self.elements.values())
         elif self._root_elements is None:
-            names = set(e.name for e in self.elements.values())
+            names = {e.name for e in self.elements.values()}
             for xsd_element in self.elements.values():
                 for e in xsd_element.iter():
                     if e is xsd_element or isinstance(e, XsdAnyElement):
                         continue
                     elif e.ref or e.parent is None:
                         if e.name in names:
                             names.discard(e.name)
@@ -1197,15 +1196,15 @@
                 continue
 
             location = child.attrib['schemaLocation'].strip()
             if child.tag == XSD_INCLUDE:
                 try:
                     logger.info("Include schema from %r", location)
                     self.include_schema(location, self.base_url)
-                except (OSError, IOError) as err:
+                except OSError as err:
                     # It is not an error if the location fail to resolve:
                     #   https://www.w3.org/TR/2012/REC-xmlschema11-1-20120405/#compound-schema
                     #   https://www.w3.org/TR/2012/REC-xmlschema11-1-20120405/#src-include
                     self.warnings.append("Include schema failed: %s." % str(err))
                     warnings.warn(self.warnings[-1], XMLSchemaIncludeWarning, stacklevel=3)
                 except (XMLSchemaParseError, XMLSchemaTypeError, ParseError) as err:
                     msg = _('cannot include schema {0!r}: {1}')
@@ -1214,15 +1213,15 @@
                     else:
                         raise type(err)(msg.format(location, err))
 
             elif child.tag == XSD_REDEFINE:
                 try:
                     logger.info("Redefine schema %r", location)
                     schema = self.include_schema(location, self.base_url)
-                except (OSError, IOError) as err:
+                except OSError as err:
                     # If the xs:redefine doesn't contain components (annotation excluded)
                     # the statement is equivalent to an include, so no error is generated,
                     # otherwise fails.
                     self.warnings.append(_("Redefine schema failed: %s") % str(err))
                     warnings.warn(self.warnings[-1], XMLSchemaIncludeWarning, stacklevel=3)
                     if any(e.tag != XSD_ANNOTATION and not callable(e.tag) for e in child):
                         self.parse_error(err, child)
@@ -1235,15 +1234,15 @@
                 else:
                     schema.redefine = self
 
             elif child.tag == XSD_OVERRIDE and self.XSD_VERSION != '1.0':
                 try:
                     logger.info("Override schema %r", location)
                     schema = self.include_schema(location, self.base_url)
-                except (OSError, IOError) as err:
+                except OSError as err:
                     # If the override doesn't contain components (annotation excluded)
                     # the statement is equivalent to an include, so no error is generated,
                     # otherwise fails.
                     self.warnings.append(_("Override schema failed: %s") % str(err))
                     warnings.warn(self.warnings[-1], XMLSchemaIncludeWarning, stacklevel=3)
                     if any(e.tag != XSD_ANNOTATION and not callable(e.tag) for e in child):
                         self.parse_error(str(err), child)
@@ -1351,15 +1350,15 @@
 
     def _import_namespace(self, namespace: str, locations: List[str]) -> None:
         import_error: Optional[Exception] = None
         for url in locations:
             try:
                 logger.debug("Import namespace %r from %r", namespace, url)
                 self.import_schema(namespace, url, self.base_url)
-            except (OSError, IOError) as err:
+            except OSError as err:
                 # It's not an error if the location access fails (ref. section 4.2.6.2):
                 #   https://www.w3.org/TR/2012/REC-xmlschema11-1-20120405/#composition-schemaImport
                 logger.debug('%s', err)
                 if import_error is None:
                     import_error = err
             except (XMLSchemaParseError, XMLSchemaTypeError, ParseError) as err:
                 if is_defuse_error(err):
@@ -1694,15 +1693,16 @@
         :param use_location_hints: for default schema locations hints provided within \
         XML data are ignored in order to avoid the change of schema instance. Set this \
         option to `True` to activate dynamic schema loading using schema location hints.
         :raises: :exc:`XMLSchemaValidationError` if the XML data instance is invalid.
         """
         for error in self.iter_errors(source, path, schema_path, use_defaults,
                                       namespaces, max_depth, extra_validator,
-                                      validation_hook, allow_empty, use_location_hints):
+                                      validation_hook, allow_empty, use_location_hints,
+                                      validation='strict'):
             raise error
 
     def is_valid(self, source: Union[XMLSourceType, XMLResource],
                  path: Optional[str] = None,
                  schema_path: Optional[str] = None,
                  use_defaults: bool = True,
                  namespaces: Optional[NamespacesType] = None,
@@ -1725,15 +1725,15 @@
                     schema_path: Optional[str] = None,
                     use_defaults: bool = True,
                     namespaces: Optional[NamespacesType] = None,
                     max_depth: Optional[int] = None,
                     extra_validator: Optional[ExtraValidatorType] = None,
                     validation_hook: Optional[ValidationHookType] = None,
                     allow_empty: bool = True,
-                    use_location_hints: bool = False) \
+                    use_location_hints: bool = False, validation: str = 'lax') \
             -> Iterator[XMLSchemaValidationError]:
         """
         Creates an iterator for the errors generated by the validation of an XML data against
         the XSD schema/component instance. Accepts the same arguments of :meth:`validate`.
         """
         self.check_validator(validation='lax')
         if isinstance(source, XMLResource):
@@ -1760,14 +1760,15 @@
             'level': resource.lazy_depth or bool(path),
             'source': resource,
             'namespaces': namespaces,
             'converter': converter,
             'id_map': Counter[str](),
             'identities': identities,
             'inherited': {},
+            'validation': validation,
         }
         if not use_defaults:
             kwargs['use_defaults'] = False
         if use_location_hints and not resource.is_lazy():
             kwargs['use_location_hints'] = True
             if self.XSD_VERSION == '1.1':
                 kwargs['errors'] = []
@@ -1815,38 +1816,42 @@
             if xsd_element is None:
                 if XSI_TYPE in elem.attrib:
                     xsd_element = self.create_element(name=elem.tag)
                 elif elem is not resource.root and ancestors:
                     continue
                 else:
                     reason = _("{!r} is not an element of the schema").format(elem)
-                    yield schema.validation_error('lax', reason, elem, resource, namespaces)
+                    yield schema.validation_error(
+                        'lax', reason, elem, source=resource, namespaces=namespaces
+                    )
                     return
 
             try:
                 for result in xsd_element.iter_decode(elem, **kwargs):
                     if isinstance(result, XMLSchemaValidationError):
                         yield result
                     else:
                         del result
             except XMLSchemaStopValidation:
                 pass
         else:
             if elem is None and not allow_empty:
                 assert path is not None
                 reason = _("the provided path selects nothing to validate")
-                yield schema.validation_error('lax', reason, None, resource, namespaces)
+                yield schema.validation_error(
+                    'lax', reason, source=resource, namespaces=namespaces
+                )
                 return
 
         if kwargs['identities'] is not identities:
             for identity, counter in kwargs['identities'].items():
                 identities[identity].counter.update(counter.counter)
             kwargs['identities'] = identities
 
-        yield from self._validate_references(validation='lax', **kwargs)
+        yield from self._validate_references(**kwargs)
 
     def _validate_references(self, source: XMLResource,
                              validation: str = 'lax',
                              id_map: Optional[Counter[str]] = None,
                              identities: Optional[IdentityMapType] = None,
                              **kwargs: Any) -> Iterator[XMLSchemaValidationError]:
         # Check unresolved IDREF values
@@ -1876,15 +1881,16 @@
         for elem in selector:
             xsd_element = self.get_element(elem.tag, schema_path, namespaces)
             if xsd_element is None:
                 if XSI_TYPE in elem.attrib:
                     xsd_element = self.create_element(name=elem.tag)
                 else:
                     reason = _("{!r} is not an element of the schema").format(elem)
-                    yield self.validation_error(validation, reason, elem, source, namespaces)
+                    yield self.validation_error(validation, reason, elem,
+                                                source=source, namespaces=namespaces)
                     continue
 
             yield from xsd_element.iter_decode(elem, validation, **kwargs)
 
         if 'max_depth' not in kwargs:
             yield from self._validate_references(source, validation=validation, **kwargs)
 
@@ -2071,15 +2077,17 @@
         for elem in selector:
             xsd_element = schema.get_element(elem.tag, schema_path, namespaces)
             if xsd_element is None:
                 if XSI_TYPE in elem.attrib:
                     xsd_element = self.create_element(name=elem.tag)
                 else:
                     reason = _("{!r} is not an element of the schema").format(elem)
-                    yield schema.validation_error(validation, reason, elem, resource, namespaces)
+                    yield schema.validation_error(
+                        validation, reason, elem, source=resource, namespaces=namespaces
+                    )
                     return
 
             yield from xsd_element.iter_decode(elem, validation, **kwargs)
 
         if 'max_depth' not in kwargs:
             yield from self._validate_references(validation=validation, **kwargs)
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/simple_types.py` & `xmlschema-3.3.1/xmlschema/validators/simple_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,20 +75,20 @@
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Optional[XsdComponent] = None,
                  name: Optional[str] = None,
                  facets: Optional[Dict[Optional[str], FacetsValueType]] = None) -> None:
 
-        super(XsdSimpleType, self).__init__(elem, schema, parent, name)
+        super().__init__(elem, schema, parent, name)
         if not hasattr(self, 'facets'):
             self.facets = facets if facets is not None else {}
 
     def __setattr__(self, name: str, value: Any) -> None:
-        super(XsdSimpleType, self).__setattr__(name, value)
+        super().__setattr__(name, value)
         if name == 'facets':
             if not isinstance(self, XsdAtomicBuiltin):
                 self._parse_facets(value)
 
             if self.min_length:
                 self.allow_empty = False
 
@@ -507,26 +507,26 @@
                  facets: Optional[Dict[Optional[str], FacetsValueType]] = None,
                  base_type: Optional[BaseXsdType] = None) -> None:
 
         if base_type is None:
             self.primitive_type = self
         else:
             self.base_type = base_type
-        super(XsdAtomic, self).__init__(elem, schema, parent, name, facets)
+        super().__init__(elem, schema, parent, name, facets)
 
     def __repr__(self) -> str:
         if self.name is None:
             return '%s(primitive_type=%r)' % (
                 self.__class__.__name__, self.primitive_type.local_name
             )
         else:
             return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
 
     def __setattr__(self, name: str, value: Any) -> None:
-        super(XsdAtomic, self).__setattr__(name, value)
+        super().__setattr__(name, value)
         if name == 'base_type':
             if not hasattr(self, 'white_space'):
                 try:
                     self.white_space = value.white_space
                 except AttributeError:
                     pass
             try:
@@ -601,15 +601,15 @@
             raise XMLSchemaTypeError("%r object is not callable" % python_type.__class__)
 
         if base_type is None and not admitted_facets and name != XSD_ERROR:
             raise XMLSchemaValueError("argument 'admitted_facets' must be "
                                       "a not empty set of a primitive type")
         self._admitted_facets = admitted_facets
 
-        super(XsdAtomicBuiltin, self).__init__(elem, schema, None, name, facets, base_type)
+        super().__init__(elem, schema, None, name, facets, base_type)
         self.python_type = python_type
         self.to_python = to_python if to_python is not None else python_type
         self.from_python = from_python if from_python is not None else str
 
     def __repr__(self) -> str:
         return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
 
@@ -619,15 +619,16 @@
 
     def iter_decode(self, obj: Union[str, bytes], validation: str = 'lax', **kwargs: Any) \
             -> IterDecodeType[DecodedValueType]:
         if isinstance(obj, (str, bytes)):
             obj = self.normalize(obj)
         elif obj is not None and not isinstance(obj, self.instance_types):
             reason = _("value is not an instance of {!r}").format(self.instance_types)
-            yield XMLSchemaDecodeError(self, obj, self.to_python, reason)
+            error = XMLSchemaDecodeError(self, obj, self.to_python, reason)
+            yield self.validation_error(validation, error, **kwargs)
 
         if validation == 'skip':
             try:
                 yield self.to_python(obj)
             except (ValueError, DecimalException):
                 yield str(obj)
             return
@@ -637,21 +638,22 @@
                 self.patterns(obj)
             except XMLSchemaValidationError as err:
                 yield err
 
         try:
             result = self.to_python(obj)
         except (ValueError, DecimalException) as err:
-            yield XMLSchemaDecodeError(self, obj, self.to_python, reason=str(err))
+            error = XMLSchemaDecodeError(self, obj, self.to_python, reason=str(err))
+            yield self.validation_error(validation, error, **kwargs)
             yield None
             return
         except TypeError:
             # xs:error type (e.g. an XSD 1.1 type alternative used to catch invalid values)
             reason = _("invalid value {!r}").format(obj)
-            yield self.validation_error(validation, error=reason, obj=obj)
+            yield self.validation_error(validation, reason, obj, **kwargs)
             yield None
             return
 
         for validator in self.validators:
             try:
                 validator(result)
             except XMLSchemaValidationError as err:
@@ -668,15 +670,15 @@
                 else:
                     try:
                         result = f"{{{kwargs['namespaces'][prefix]}}}{name}"
                     except (TypeError, KeyError):
                         try:
                             if kwargs['source'].namespace != XSD_NAMESPACE:
                                 reason = _("unmapped prefix %r in a QName") % prefix
-                                yield self.validation_error(validation, error=reason, obj=obj)
+                                yield self.validation_error(validation, reason, obj, **kwargs)
                         except KeyError:
                             pass
             else:
                 try:
                     default_namespace = kwargs['namespaces']['']
                 except (TypeError, KeyError):
                     pass
@@ -702,27 +704,27 @@
                 try:
                     id_list = kwargs['id_list']
                 except KeyError:
                     if not id_map[obj]:
                         id_map[obj] = 1
                     else:
                         reason = _("duplicated xs:ID value {!r}").format(obj)
-                        yield self.validation_error(validation, error=reason, obj=obj)
+                        yield self.validation_error(validation, reason, obj, **kwargs)
                 else:
                     if not id_map[obj]:
                         id_map[obj] = 1
                         id_list.append(obj)
                         if len(id_list) > 1 and self.xsd_version == '1.0':
                             reason = _("no more than one attribute of type ID should "
                                        "be present in an element")
                             yield self.validation_error(validation, reason, obj, **kwargs)
 
                     elif obj not in id_list or self.xsd_version == '1.0':
                         reason = _("duplicated xs:ID value {!r}").format(obj)
-                        yield self.validation_error(validation, error=reason, obj=obj)
+                        yield self.validation_error(validation, reason, obj, **kwargs)
 
         yield result
 
     def iter_encode(self, obj: Any, validation: str = 'lax', **kwargs: Any) \
             -> IterEncodeType[EncodedValueType]:
         if isinstance(obj, (str, bytes)):
             obj = self.normalize(obj)
@@ -734,50 +736,55 @@
                 yield str(obj)
             return
 
         elif isinstance(obj, bool):
             types_: Any = self.instance_types
             if types_ is not bool or (isinstance(types_, tuple) and bool in types_):
                 reason = _("boolean value {0!r} requires a {1!r} decoder").format(obj, bool)
-                yield XMLSchemaEncodeError(self, obj, self.from_python, reason)
+                error = XMLSchemaEncodeError(self, obj, self.from_python, reason)
+                yield self.validation_error(validation, error, **kwargs)
                 obj = self.python_type(obj)
 
         elif not isinstance(obj, self.instance_types):
             reason = _("{0!r} is not an instance of {1!r}").format(obj, self.instance_types)
-            yield XMLSchemaEncodeError(self, obj, self.from_python, reason)
+            error = XMLSchemaEncodeError(self, obj, self.from_python, reason)
+            yield self.validation_error(validation, error, **kwargs)
 
             try:
                 value = self.python_type(obj)
                 if value != obj and not isinstance(value, str) \
                         and not isinstance(obj, (str, bytes)):
                     raise ValueError()
                 obj = value
             except (ValueError, TypeError) as err:
-                yield XMLSchemaEncodeError(self, obj, self.from_python, reason=str(err))
+                error = XMLSchemaEncodeError(self, obj, self.from_python, reason=str(err))
+                yield self.validation_error(validation, error, **kwargs)
                 yield None
                 return
             else:
                 if value == obj or str(value) == str(obj):
                     obj = value
                 else:
                     reason = _("invalid value {!r}").format(obj)
-                    yield XMLSchemaEncodeError(self, obj, self.from_python, reason)
+                    error = XMLSchemaEncodeError(self, obj, self.from_python, reason)
+                    yield self.validation_error(validation, error, **kwargs)
                     yield None
                     return
 
         for validator in self.validators:
             try:
                 validator(obj)
             except XMLSchemaValidationError as err:
                 yield err
 
         try:
             text = self.from_python(obj)
         except ValueError as err:
-            yield XMLSchemaEncodeError(self, obj, self.from_python, reason=str(err))
+            error = XMLSchemaEncodeError(self, obj, self.from_python, reason=str(err))
+            yield self.validation_error(validation, error, **kwargs)
             yield None
         else:
             if self.patterns is not None:
                 try:
                     self.patterns(text)
                 except XMLSchemaValidationError as err:
                     yield err
@@ -805,40 +812,40 @@
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Optional[XsdComponent],
                  name: Optional[str] = None) -> None:
         facets: Optional[Dict[Optional[str], FacetsValueType]] = {
             XSD_WHITE_SPACE: XsdWhiteSpaceFacet(self._white_space_elem, schema, self, self)
         }
-        super(XsdList, self).__init__(elem, schema, parent, name, facets)
+        super().__init__(elem, schema, parent, name, facets)
 
     def __repr__(self) -> str:
         if self.name is None:
             return '%s(item_type=%r)' % (self.__class__.__name__, self.item_type)
         else:
             return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'elem' and value is not None and value.tag != XSD_LIST:
             if value.tag == XSD_SIMPLE_TYPE:
                 for child in value:
                     if child.tag == XSD_LIST:
-                        super(XsdList, self).__setattr__(name, child)
+                        super().__setattr__(name, child)
                         return
             raise XMLSchemaValueError(
-                "a {0!r} definition required for {1!r}".format(XSD_LIST, self)
+                f"a {XSD_LIST!r} definition required for {self!r}"
             )
         elif name == 'item_type':
             if not value.is_atomic():
                 raise XMLSchemaValueError(
                     _("%r: a list must be based on atomic data types") % value
                 )
         elif name == 'white_space' and value is None:
             value = 'collapse'
-        super(XsdList, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     def _parse(self) -> None:
         item_type: Any
 
         child = self._parse_child_component(self.elem)
         if child is not None:
             # Case of a local simpleType declaration inside the list tag
@@ -979,39 +986,39 @@
     _ADMITTED_TYPES: Any = XsdSimpleType
     _ADMITTED_TAGS = {XSD_UNION}
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Optional[XsdComponent],
                  name: Optional[str] = None) -> None:
-        super(XsdUnion, self).__init__(elem, schema, parent, name, facets=None)
+        super().__init__(elem, schema, parent, name, facets=None)
 
     def __repr__(self) -> str:
         if self.name is None:
             return '%s(member_types=%r)' % (self.__class__.__name__, self.member_types)
         else:
             return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'elem' and value is not None and value.tag != XSD_UNION:
             if value.tag == XSD_SIMPLE_TYPE:
                 for child in value:
                     if child.tag == XSD_UNION:
-                        super(XsdUnion, self).__setattr__(name, child)
+                        super().__setattr__(name, child)
                         return
             raise XMLSchemaValueError(
-                "a {0!r} definition required for {1!r}".format(XSD_UNION, self)
+                f"a {XSD_UNION!r} definition required for {self!r}"
             )
 
         elif name == 'white_space':
             if not (value is None or value == 'collapse'):
                 msg = _("wrong value %r for attribute 'white_space'")
                 raise XMLSchemaValueError(msg % value)
             value = 'collapse'
-        super(XsdUnion, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     def _parse(self) -> None:
         mt: Any
         member_types = []
 
         for child in self.elem:
             if child.tag != XSD_ANNOTATION and not callable(child.tag):
@@ -1114,15 +1121,16 @@
                 break
 
         if isinstance(obj, bytes):
             obj = obj.decode('utf-8')
 
         if not isinstance(obj, str) or ' ' not in obj.strip():
             reason = _("invalid value {!r}").format(obj)
-            yield XMLSchemaDecodeError(self, obj, self.member_types, reason)
+            error = XMLSchemaDecodeError(self, obj, self.member_types, reason)
+            yield self.validation_error(validation, error, **kwargs)
             return
 
         items = []
         not_decodable = []
         for chunk in obj.split():
             for member_type in self.member_types:
                 for result in member_type.iter_decode(chunk, validation='lax', **kwargs):
@@ -1136,15 +1144,16 @@
                 if validation != 'skip':
                     not_decodable.append(chunk)
                 else:
                     items.append(str(chunk))
 
         if not_decodable:
             reason = _("no type suitable for decoding the values %r") % not_decodable
-            yield XMLSchemaDecodeError(self, obj, self.member_types, reason)
+            error = XMLSchemaDecodeError(self, obj, self.member_types, reason)
+            yield self.validation_error(validation, error, **kwargs)
 
         yield items if len(items) > 1 else items[0] if items else None
 
     def iter_encode(self, obj: Any, validation: str = 'lax', **kwargs: Any) \
             -> IterEncodeType[EncodedValueType]:
 
         for member_type in self.member_types:
@@ -1170,15 +1179,16 @@
 
                 if len(results) == len(obj):
                     yield results
                     break
 
         if validation != 'skip':
             reason = _("no type suitable for encoding the object")
-            yield XMLSchemaEncodeError(self, obj, self.member_types, reason)
+            error = XMLSchemaEncodeError(self, obj, self.member_types, reason)
+            yield self.validation_error(validation, error, **kwargs)
             yield None
         else:
             yield str(obj)
 
 
 class Xsd11Union(XsdUnion):
     _ADMITTED_TYPES = XsdAtomic, XsdList, XsdUnion
@@ -1206,15 +1216,15 @@
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'elem' and value is not None:
             if self.name != XSD_ANY_ATOMIC_TYPE and value.tag != XSD_RESTRICTION:
                 if not (value.tag == XSD_SIMPLE_TYPE and value.get('name') is not None):
                     raise XMLSchemaValueError(
                         "an xs:restriction definition required for %r." % self
                     )
-        super(XsdAtomicRestriction, self).__setattr__(name, value)
+        super().__setattr__(name, value)
 
     def _parse(self) -> None:
         elem = self.elem
         if elem.get('name') == XSD_ANY_ATOMIC_TYPE:
             return  # skip special type xs:anyAtomicType
         elif elem.tag == XSD_SIMPLE_TYPE and elem.get('name') is not None:
             # Global simpleType with internal restriction
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/wildcards.py` & `xmlschema-3.3.1/xmlschema/validators/wildcards.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
     """
     _ADMITTED_TAGS = {XSD_ANY}
     precedences: Dict[ModelGroupType, List[ModelParticleType]]
     copy: Callable[['XsdAnyElement'], 'XsdAnyElement']
 
     def __init__(self, elem: ElementType, schema: SchemaType, parent: XsdComponent) -> None:
         self.precedences = {}
-        super(XsdAnyElement, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         if self.namespace:
             return '%s(namespace=%r, process_contents=%r, occurs=%r)' % (
                 self.__class__.__name__, self.namespace,
                 self.process_contents, list(self.occurs)
             )
@@ -437,15 +437,15 @@
         return build_schema_node_tree(
             root=self,
             elements=schema_node.elements,
             global_elements=schema_node.children,
         )
 
     def _parse(self) -> None:
-        super(XsdAnyElement, self)._parse()
+        super()._parse()
         self._parse_particle(self.elem)
 
     def match(self, name: Optional[str], default_namespace: Optional[str] = None,
               resolve: bool = False, **kwargs: Any) -> Optional[SchemaElementType]:
         """
         Returns the element wildcard if name is matching the name provided
         as argument, `None` otherwise.
@@ -742,15 +742,15 @@
           notQName = List of (QName | (##defined | ##definedSibling))
           processContents = (lax | skip | strict) : strict
           {any attributes with non-schema namespace . . .}>
           Content: (annotation?)
         </any>
     """
     def _parse(self) -> None:
-        super(Xsd11AnyElement, self)._parse()
+        super()._parse()
         self._parse_not_constraints()
 
     def is_matching(self, name: Optional[str],
                     default_namespace: Optional[str] = None,
                     group: Optional[ModelGroupType] = None,
                     occurs: Optional[OccursCounterType] = None,
                     **kwargs: Any) -> bool:
@@ -819,15 +819,15 @@
           notQName = List of (QName | ##defined)
           processContents = (lax | skip | strict) : strict
           {any attributes with non-schema namespace . . .}>
           Content: (annotation?)
         </anyAttribute>
     """
     def _parse(self) -> None:
-        super(Xsd11AnyAttribute, self)._parse()
+        super()._parse()
         self._parse_not_constraints()
 
     def is_matching(self, name: Optional[str],
                     default_namespace: Optional[str] = None,
                     **kwargs: Any) -> bool:
         if name is None:
             return False
@@ -862,27 +862,27 @@
         </openContent>
     """
     _ADMITTED_TAGS = {XSD_OPEN_CONTENT}
     mode = 'interleave'
     any_element = None  # type: Xsd11AnyElement
 
     def __init__(self, elem: ElementType, schema: SchemaType, parent: XsdComponent) -> None:
-        super(XsdOpenContent, self).__init__(elem, schema, parent)
+        super().__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         return '%s(mode=%r)' % (self.__class__.__name__, self.mode)
 
     def _parse(self) -> None:
-        super(XsdOpenContent, self)._parse()
+        super()._parse()
         try:
             self.mode = self.elem.attrib['mode']
         except KeyError:
             pass
         else:
-            if self.mode not in {'none', 'interleave', 'suffix'}:
+            if self.mode not in ('none', 'interleave', 'suffix'):
                 msg = _("wrong value %r for 'mode' attribute")
                 self.parse_error(msg % self.mode)
 
         child = self._parse_child_component(self.elem)
         if self.mode == 'none':
             if child is not None and child.tag == XSD_ANY:
                 msg = _("an openContent with mode='none' cannot "
@@ -921,21 +921,21 @@
     _ADMITTED_TAGS = {XSD_DEFAULT_OPEN_CONTENT}
     applies_to_empty = False
 
     def __init__(self, elem: ElementType, schema: SchemaType) -> None:
         super(XsdOpenContent, self).__init__(elem, schema)
 
     def _parse(self) -> None:
-        super(XsdDefaultOpenContent, self)._parse()
+        super()._parse()
         if self.parent is not None:
             msg = _("defaultOpenContent must be a child of the schema")
             self.parse_error(msg)
         if self.mode == 'none':
             msg = _("the attribute 'mode' of a defaultOpenContent cannot be 'none'")
             self.parse_error(msg)
         if self._parse_child_component(self.elem) is None:
             msg = _("a defaultOpenContent declaration cannot be empty")
             self.parse_error(msg)
 
         if 'appliesToEmpty' in self.elem.attrib:
-            if self.elem.attrib['appliesToEmpty'].strip() in {'true', '1'}:
+            if self.elem.attrib['appliesToEmpty'].strip() in ('true', '1'):
                 self.applies_to_empty = True
```

### Comparing `xmlschema-3.3.0/xmlschema/validators/xsdbase.py` & `xmlschema-3.3.1/xmlschema/validators/xsdbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 """
 This module contains base functions and classes XML Schema components.
 """
+import logging
 import re
 from typing import TYPE_CHECKING, cast, Any, Dict, Generic, List, Iterator, Optional, \
     Set, Tuple, TypeVar, Union, MutableMapping
 from xml.etree import ElementTree
 
 from elementpath import select
 from elementpath.etree import etree_tostring
@@ -23,27 +24,29 @@
     XSD_ANY_TYPE, XSD_ANY_SIMPLE_TYPE, XSD_ANY_ATOMIC_TYPE, XSD_ID, \
     XSD_QNAME, XSD_OVERRIDE, XSD_NOTATION_TYPE, XSD_DECIMAL, XMLNS_NAMESPACE
 from ..aliases import ElementType, NamespacesType, SchemaType, BaseXsdType, \
     ComponentClassType, ExtraValidatorType, DecodeType, IterDecodeType, \
     EncodeType, IterEncodeType
 from ..translation import gettext as _
 from ..helpers import get_qname, local_name, get_prefixed_qname, \
-    is_etree_element, is_etree_document
+    is_etree_element, is_etree_document, format_xmlschema_stack
 from ..resources import XMLResource
 from ..converters import XMLSchemaConverter
 from .exceptions import XMLSchemaParseError, XMLSchemaValidationError
 from .helpers import get_xsd_annotation_child
 
 if TYPE_CHECKING:
     from .simple_types import XsdSimpleType
     from .complex_types import XsdComplexType
     from .elements import XsdElement
     from .groups import XsdGroup
     from .global_maps import XsdGlobals
 
+logger = logging.getLogger('xmlschema')
+
 XSD_TYPE_DERIVATIONS = {'extension', 'restriction'}
 XSD_ELEMENT_DERIVATIONS = {'extension', 'restriction', 'substitution'}
 
 XSD_VALIDATION_MODES = {'strict', 'lax', 'skip'}
 """
 XML Schema validation modes
 Ref.: https://www.w3.org/TR/xmlschema11-1/#key-va
@@ -188,56 +191,71 @@
         elif isinstance(error, str):
             error = XMLSchemaParseError(self, error, elem)
         else:
             msg = "'error' argument must be an exception or a string, not {!r}."
             raise XMLSchemaTypeError(msg.format(error))
 
         if validation == 'lax':
+            if error.stack_trace is None and logger.level == logging.DEBUG:
+                error.stack_trace = format_xmlschema_stack()
+                logger.debug("Collect %r with traceback:\n%s", error, error.stack_trace)
+
             self.errors.append(error)
         else:
             raise error
 
     def validation_error(self, validation: str,
                          error: Union[str, Exception],
                          obj: Any = None,
+                         elem: Optional[ElementType] = None,
                          source: Optional[Any] = None,
                          namespaces: Optional[NamespacesType] = None,
                          **kwargs: Any) -> XMLSchemaValidationError:
         """
         Helper method for generating and updating validation errors. If validation
         mode is 'lax' or 'skip' returns the error, otherwise raises the error.
 
         :param validation: an error-compatible validation mode: can be 'lax' or 'strict'.
         :param error: an error instance or the detailed reason of failed validation.
         :param obj: the instance related to the error.
+        :param elem: the element related to the error, can be `obj` for elements.
         :param source: the XML resource or data related to the validation process.
         :param namespaces: is an optional mapping from namespace prefix to URI.
         :param kwargs: other keyword arguments of the validation process.
         """
         check_validation_mode(validation)
+        if elem is None and is_etree_element(obj):
+            elem = cast(ElementType, obj)
+
         if isinstance(error, XMLSchemaValidationError):
             if error.namespaces is None and namespaces is not None:
                 error.namespaces = namespaces
             if error.source is None and source is not None:
                 error.source = source
             if error.obj is None and obj is not None:
                 error.obj = obj
-            if error.elem is None and obj is not None and is_etree_element(obj):
-                error.elem = obj
-                if is_etree_element(error.obj) and obj.tag == error.obj.tag:
-                    error.obj = obj
+            elif is_etree_element(error.obj) and elem is not None:
+                if elem.tag == error.obj.tag and elem is not error.obj:
+                    error.obj = elem
 
         elif isinstance(error, Exception):
             error = XMLSchemaValidationError(self, obj, str(error), source, namespaces)
         else:
             error = XMLSchemaValidationError(self, obj, error, source, namespaces)
 
+        if error.elem is None and elem is not None:
+            error.elem = elem
+
         if validation == 'strict' and error.elem is not None:
             raise error
 
+        if error.stack_trace is None and logger.level == logging.DEBUG:
+            error.stack_trace = format_xmlschema_stack()
+            logger.debug("Collect %r with traceback:\n%s", error, error.stack_trace)
+
         if 'errors' in kwargs and error not in kwargs['errors']:
             kwargs['errors'].append(error)
 
         return error
 
     def _parse_xpath_default_namespace(self, elem: ElementType) -> str:
         """
@@ -298,15 +316,15 @@
     _target_namespace: Optional[str]
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Optional['XsdComponent'] = None,
                  name: Optional[str] = None) -> None:
 
-        super(XsdComponent, self).__init__(schema.validation)
+        super().__init__(schema.validation)
         if name:
             self.name = name
         if parent is not None:
             self.parent = parent
         self.schema = schema
         self.maps: XsdGlobals = schema.maps
         self.elem = elem
@@ -314,20 +332,20 @@
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'elem':
             if value.tag not in self._ADMITTED_TAGS:
                 msg = "wrong XSD element {!r} for {!r}, must be one of {!r}"
                 raise XMLSchemaValueError(
                     msg.format(value.tag, self.__class__, self._ADMITTED_TAGS)
                 )
-            super(XsdComponent, self).__setattr__(name, value)
+            super().__setattr__(name, value)
             if self.errors:
                 self.errors.clear()
             self._parse()
         else:
-            super(XsdComponent, self).__setattr__(name, value)
+            super().__setattr__(name, value)
 
     @property
     def xsd_version(self) -> str:
         return self.schema.XSD_VERSION
 
     def is_global(self) -> bool:
         """Returns `True` if the instance is a global component, `False` if it's local."""
@@ -619,15 +637,15 @@
 
         for k in filter(lambda x: x.endswith(suffix), mapping):
             prefix = k.split(':')[0]
             if self.namespaces.get(prefix) == target_namespace:
                 return mapping[k]
 
             # Match namespace declaration within value
-            ns_declaration = '{}:{}'.format(ns_prefix, prefix)
+            ns_declaration = f'{ns_prefix}:{prefix}'
             try:
                 if mapping[k][ns_declaration] == target_namespace:
                     return mapping[k]
             except (KeyError, TypeError):
                 pass
         else:
             if match_local_name:
```

### Comparing `xmlschema-3.3.0/xmlschema/xpath/__init__.py` & `xmlschema-3.3.1/xmlschema/xpath/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/xpath/assertion_parser.py` & `xmlschema-3.3.1/xmlschema/xpath/assertion_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/xpath/identity_parser.py` & `xmlschema-3.3.1/xmlschema/xpath/identity_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/xpath/mixin.py` & `xmlschema-3.3.1/xmlschema/xpath/mixin.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema/xpath/proxy.py` & `xmlschema-3.3.1/xmlschema/xpath/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
                  base_element: Optional[BaseElementType] = None) -> None:
 
         if schema is None:
             from xmlschema import XMLSchema10
             schema = getattr(XMLSchema10, 'meta_schema', None)
             assert schema is not None
 
-        super(XMLSchemaProxy, self).__init__(
-            schema, base_element
-        )
+        super().__init__(schema, base_element)
 
         if base_element is not None:
             try:
                 if base_element.schema is not schema:
                     msg = "{} is not an element of {}"
                     raise XMLSchemaValueError(msg.format(base_element, schema))
             except AttributeError:
```

### Comparing `xmlschema-3.3.0/xmlschema/xpath3.py` & `xmlschema-3.3.1/xmlschema/xpath3.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.3.0/xmlschema.egg-info/PKG-INFO` & `xmlschema-3.3.1/xmlschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.3.0
+Version: 3.3.1
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.3.0/xmlschema.egg-info/SOURCES.txt` & `xmlschema-3.3.1/xmlschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

