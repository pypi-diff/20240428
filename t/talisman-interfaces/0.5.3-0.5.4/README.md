# Comparing `tmp/talisman-interfaces-0.5.3.tar.gz` & `tmp/talisman-interfaces-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-interfaces-0.5.3.tar", last modified: Wed Mar 20 12:52:53 2024, max compression
+gzip compressed data, was "talisman-interfaces-0.5.4.tar", last modified: Sat Apr 27 14:10:55 2024, max compression
```

## Comparing `talisman-interfaces-0.5.3.tar` & `talisman-interfaces-0.5.4.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.150428 talisman-interfaces-0.5.3/
--rw-r--r--   0 root         (0) root         (0)      650 2024-03-20 12:52:53.150428 talisman-interfaces-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-19 10:06:40.000000 talisman-interfaces-0.5.3/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 12:52:53.150428 talisman-interfaces-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-03-20 12:41:40.000000 talisman-interfaces-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.138428 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/
--rw-r--r--   0 root         (0) root         (0)      650 2024-03-20 12:52:53.000000 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2975 2024-03-20 12:52:53.000000 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 12:52:53.000000 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-20 12:52:53.000000 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-20 12:52:53.000000 talisman-interfaces-0.5.3/talisman_interfaces.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.138428 talisman-interfaces-0.5.3/tp_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.138428 talisman-interfaces-0.5.3/tp_interfaces/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.138428 talisman-interfaces-0.5.3/tp_interfaces/abstract/configuration/
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/configuration/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/
--rw-rw-rw-   0 root         (0) root         (0)      319 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-03-20 12:41:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/composite.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/constructable.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/merge.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-03-20 12:41:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/model/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1288 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/model.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/update.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/domain/
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/default_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/tdm_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.142428 talisman-interfaces-0.5.3/tp_interfaces/domain/model/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/_types_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_component.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_concept.py
--rw-rw-rw-   0 root         (0) root         (0)     1304 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_nerc.py
--rw-rw-rw-   0 root         (0) root         (0)     1433 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_property.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_relation.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_relext.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_value.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/domain/stub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/evaluators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/evaluators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1254 2024-03-06 14:52:27.000000 talisman-interfaces-0.5.3/tp_interfaces/evaluators/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/batch.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/convert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/mentions.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/get_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/helpers/tar_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/loader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/loader/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/logging/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/processors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/processors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4516 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/processors/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/processors/updatable_composite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.146428 talisman-interfaces-0.5.3/tp_interfaces/readers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/readers/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.150428 talisman-interfaces-0.5.3/tp_interfaces/serializable/
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializable/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializable/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     7108 2024-03-20 12:41:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializable/directory_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializable/manipulations.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializable/pickle_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:53.150428 talisman-interfaces-0.5.3/tp_interfaces/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:35.000000 talisman-interfaces-0.5.3/tp_interfaces/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-03-04 15:46:40.000000 talisman-interfaces-0.5.3/tp_interfaces/serializers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/
+-rw-r--r--   0 root         (0) root         (0)      650 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-26 13:57:33.000000 talisman-interfaces-0.5.4/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.788081 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      650 2024-04-27 14:10:55.000000 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-27 14:10:55.000000 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 14:10:55.000000 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-04-27 14:10:55.000000 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 14:10:55.000000 talisman-interfaces-0.5.4/talisman_interfaces.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.788081 talisman-interfaces-0.5.4/tp_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.788081 talisman-interfaces-0.5.4/tp_interfaces/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.788081 talisman-interfaces-0.5.4/tp_interfaces/abstract/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/configuration/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-04-26 10:20:49.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.788081 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/
+-rw-rw-rw-   0 root         (0) root         (0)      319 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/constructable.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/merge.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/model/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-26 13:57:33.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/update.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/domain/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/default_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/tdm_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/domain/model/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/_types_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_component.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_concept.py
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_nerc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1433 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-27 13:44:57.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_relext.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/domain/stub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/evaluators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/evaluators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/evaluators/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/convert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/mentions.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/get_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/helpers/tar_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/loader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/loader/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/logging/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/processors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/processors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4516 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/processors/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/processors/updatable_composite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/readers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/readers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/serializable/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializable/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializable/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     7108 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializable/directory_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializable/manipulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializable/pickle_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:10:55.792081 talisman-interfaces-0.5.4/tp_interfaces/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:46.000000 talisman-interfaces-0.5.4/tp_interfaces/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-23 13:03:27.000000 talisman-interfaces-0.5.4/tp_interfaces/serializers/abstract.py
```

### Comparing `talisman-interfaces-0.5.3/PKG-INFO` & `talisman-interfaces-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.5.3
+Version: 0.5.4
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.5.3/setup.py` & `talisman-interfaces-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/talisman_interfaces.egg-info/PKG-INFO` & `talisman-interfaces-0.5.4/talisman_interfaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.5.3
+Version: 0.5.4
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.5.3/talisman_interfaces.egg-info/SOURCES.txt` & `talisman-interfaces-0.5.4/talisman_interfaces.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 talisman_interfaces.egg-info/PKG-INFO
 talisman_interfaces.egg-info/SOURCES.txt
 talisman_interfaces.egg-info/dependency_links.txt
 talisman_interfaces.egg-info/requires.txt
 talisman_interfaces.egg-info/top_level.txt
 tp_interfaces/__init__.py
 tp_interfaces/abstract/__init__.py
+tp_interfaces/abstract/exception.py
 tp_interfaces/abstract/schema.py
 tp_interfaces/abstract/configuration/__init__.py
 tp_interfaces/abstract/configuration/factory.py
 tp_interfaces/abstract/model/__init__.py
 tp_interfaces/abstract/model/composite.py
 tp_interfaces/abstract/model/constructable.py
 tp_interfaces/abstract/model/merge.py
```

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/__init__.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/model/composite.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/model/composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/model/merge.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/model/merge.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/model/wrapper.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/category.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/category.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/node.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/node.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/processor.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from tp_interfaces.serializable import Serializable
 
 _Config = TypeVar('_Config', bound=ImmutableBaseModel)
 
 
 @runtime_checkable
 class AbstractDocumentProcessor(AsyncModel, Protocol[_Config]):
+
     async def process_doc(self, document: TalismanDocument, config: _Config) -> TalismanDocument:
         pass
 
     async def process_docs(self, documents: Sequence[TalismanDocument], config: _Config) -> Tuple[TalismanDocument, ...]:
         log_extras = with_log_extras(doc_id=lambda kwargs: kwargs['document'].id)
         return tuple(await asyncio.gather(*map(partial(log_extras(self.process_doc), config=config), documents)))
```

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/processor/trainer.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/processor/trainer.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/model.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/abstract/updatable/wrapper.py` & `talisman-interfaces-0.5.4/tp_interfaces/abstract/updatable/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/filters.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/filters.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/hooks/configuration.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/hooks/configuration.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/interfaces.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/interfaces.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/manager.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/manager.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/_types_registry.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/_types_registry.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/__init__.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_nerc.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_nerc.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_property.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_property.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_relation.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_relation.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_relext.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_relext.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/model/types/_value.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/model/types/_value.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/domain/stub.py` & `talisman-interfaces-0.5.4/tp_interfaces/domain/stub.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/evaluators/abstract.py` & `talisman-interfaces-0.5.4/tp_interfaces/evaluators/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/batch.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/batch.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/fact.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/fact.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/datamodel/mentions.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/datamodel/mentions.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/get_indexes.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/get_indexes.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/io.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/io.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/helpers/tar_model.py` & `talisman-interfaces-0.5.4/tp_interfaces/helpers/tar_model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/loader/interfaces.py` & `talisman-interfaces-0.5.4/tp_interfaces/loader/interfaces.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/logging/context.py` & `talisman-interfaces-0.5.4/tp_interfaces/logging/context.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/processors/composite.py` & `talisman-interfaces-0.5.4/tp_interfaces/processors/composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/processors/updatable_composite.py` & `talisman-interfaces-0.5.4/tp_interfaces/processors/updatable_composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/readers/abstract.py` & `talisman-interfaces-0.5.4/tp_interfaces/readers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/serializable/abstract.py` & `talisman-interfaces-0.5.4/tp_interfaces/serializable/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/serializable/directory_mixin.py` & `talisman-interfaces-0.5.4/tp_interfaces/serializable/directory_mixin.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/serializable/manipulations.py` & `talisman-interfaces-0.5.4/tp_interfaces/serializable/manipulations.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/serializable/pickle_mixin.py` & `talisman-interfaces-0.5.4/tp_interfaces/serializable/pickle_mixin.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.5.3/tp_interfaces/serializers/abstract.py` & `talisman-interfaces-0.5.4/tp_interfaces/serializers/abstract.py`

 * *Files identical despite different names*

