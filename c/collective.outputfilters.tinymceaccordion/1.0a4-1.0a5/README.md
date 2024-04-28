# Comparing `tmp/collective.outputfilters.tinymceaccordion-1.0a4.tar.gz` & `tmp/collective.outputfilters.tinymceaccordion-1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.outputfilters.tinymceaccordion-1.0a4.tar", last modified: Sun Apr 28 19:28:53 2024, max compression
+gzip compressed data, was "collective.outputfilters.tinymceaccordion-1.0a5.tar", last modified: Sun Apr 28 19:55:05 2024, max compression
```

## Comparing `collective.outputfilters.tinymceaccordion-1.0a4.tar` & `collective.outputfilters.tinymceaccordion-1.0a5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/
--rw-rw-r--   0 jan       (1000) jan       (1000)       81 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/.coveragerc
--rw-rw-r--   0 jan       (1000) jan       (1000)     2023 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/.pre-commit-config.yaml
--rw-rw-r--   0 jan       (1000) jan       (1000)      302 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/CHANGES.md
--rw-rw-r--   0 jan       (1000) jan       (1000)       42 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/CONTRIBUTORS.md
--rw-rw-r--   0 jan       (1000) jan       (1000)      177 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/DEVELOP.md
--rw-rw-r--   0 jan       (1000) jan       (1000)      256 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/MANIFEST.in
--rw-rw-r--   0 jan       (1000) jan       (1000)     6044 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     4365 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/README.md
--rw-rw-r--   0 jan       (1000) jan       (1000)      175 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/instance.yaml
--rw-rw-r--   0 jan       (1000) jan       (1000)     4491 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/pyproject.toml
--rw-rw-r--   0 jan       (1000) jan       (1000)       63 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/setup.cfg
--rw-rw-r--   0 jan       (1000) jan       (1000)     2885 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/setup.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.184569 collective.outputfilters.tinymceaccordion-1.0a4/src/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/
--rw-rw-r--   0 jan       (1000) jan       (1000)       56 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/
--rw-rw-r--   0 jan       (1000) jan       (1000)       56 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/
--rw-rw-r--   0 jan       (1000) jan       (1000)       22 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      618 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/configure.zcml
--rw-rw-r--   0 jan       (1000) jan       (1000)     4390 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/filter.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      367 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/interfaces.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/
--rw-rw-r--   0 jan       (1000) jan       (1000)      523 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/README.md
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1175 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/collective.outputfilters.tinymceaccordion.pot
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.184569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/de/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1224 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.184569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/en/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1091 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po
--rw-rw-r--   0 jan       (1000) jan       (1000)     1754 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/update.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)      560 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/update.sh
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.184569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/
--rw-rw-r--   0 jan       (1000) jan       (1000)      241 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/browserlayer.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)      122 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/catalog.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)      195 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/metadata.xml
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/registry/
--rw-rw-r--   0 jan       (1000) jan       (1000)      221 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/registry/main.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)      137 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/default/rolemap.xml
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/uninstall/
--rw-rw-r--   0 jan       (1000) jan       (1000)      144 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)     1145 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles.zcml
--rw-rw-r--   0 jan       (1000) jan       (1000)     2193 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/setuphandlers.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1805 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/testing.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.192569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4159 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/test_filter.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4389 2024-04-28 19:28:52.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/test_setup.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:28:53.188569 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)     6044 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     2440 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)      146 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/entry_points.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       36 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/namespace_packages.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/not-zip-safe
--rw-rw-r--   0 jan       (1000) jan       (1000)      265 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       11 2024-04-28 19:28:53.000000 collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.128310 collective.outputfilters.tinymceaccordion-1.0a5/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       81 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/.coveragerc
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2023 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/.pre-commit-config.yaml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      368 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/CHANGES.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)       42 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/CONTRIBUTORS.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)      177 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/DEVELOP.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)      256 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/MANIFEST.in
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6252 2024-04-28 19:55:05.128310 collective.outputfilters.tinymceaccordion-1.0a5/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4507 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/README.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)      175 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/instance.yaml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4491 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/pyproject.toml
+-rw-rw-r--   0 jan       (1000) jan       (1000)       63 2024-04-28 19:55:05.128310 collective.outputfilters.tinymceaccordion-1.0a5/setup.cfg
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2885 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.120310 collective.outputfilters.tinymceaccordion-1.0a5/src/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       56 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       56 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       22 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      618 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/configure.zcml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4390 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/filter.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      367 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/interfaces.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      523 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/README.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1175 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/collective.outputfilters.tinymceaccordion.pot
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.120310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/de/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1224 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.120310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/en/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1091 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1754 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/update.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      560 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/update.sh
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.120310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      241 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/browserlayer.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      122 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/catalog.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      195 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/metadata.xml
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/registry/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      221 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/registry/main.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      137 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/default/rolemap.xml
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.128310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/uninstall/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      144 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1145 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles.zcml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2193 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/setuphandlers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1805 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/testing.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.128310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4159 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/test_filter.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4389 2024-04-28 19:55:04.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/test_setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-28 19:55:05.124310 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6252 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2440 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)      146 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/entry_points.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       36 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/not-zip-safe
+-rw-rw-r--   0 jan       (1000) jan       (1000)      265 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       11 2024-04-28 19:55:05.000000 collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/top_level.txt
```

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/.pre-commit-config.yaml` & `collective.outputfilters.tinymceaccordion-1.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/PKG-INFO` & `collective.outputfilters.tinymceaccordion-1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.outputfilters.tinymceaccordion
-Version: 1.0a4
+Version: 1.0a5
 Summary: Addon for Plone 6 - Plone Outputfilter to transform TinyMCE Markup to Bootstrap5 Accordion
 Home-page: https://github.com/collective/collective.outputfilters.tinymceaccordion
 Author: 1letter
 Author-email: 1letter@gmx.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.outputfilters.tinymceaccordion/
 Project-URL: Source, https://github.com/collective/collective.outputfilters.tinymceaccordion
@@ -25,15 +25,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # README
 
-![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion)
+![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion) ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/plone/collective.outputfilters.tinymceaccordion)
+
 
 - [README](#readme)
   - [Who need this addon?](#who-need-this-addon)
   - [Registry Settings](#registry-settings)
   - [Install Addon via buildout](#install-addon-via-buildout)
   - [Install Addon via pip](#install-addon-via-pip)
   - [Install a Testenvironment](#install-a-testenvironment)
@@ -209,14 +210,21 @@
 - 1letter, 1letter@gmx.de
 
 
 # Changelog
 
 <!-- towncrier release notes start -->
 
+## 1.0a5 (2024-04-28)
+
+
+### Internal:
+
+- Update README @1letter 
+
 ## 1.0a4 (2024-04-28)
 
 
 ### Internal:
 
 - remove unused files @1letter
```

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/README.md` & `collective.outputfilters.tinymceaccordion-1.0a5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # README
 
-![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion)
+![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion) ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/plone/collective.outputfilters.tinymceaccordion)
+
 
 - [README](#readme)
   - [Who need this addon?](#who-need-this-addon)
   - [Registry Settings](#registry-settings)
   - [Install Addon via buildout](#install-addon-via-buildout)
   - [Install Addon via pip](#install-addon-via-pip)
   - [Install a Testenvironment](#install-a-testenvironment)
```

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/pyproject.toml` & `collective.outputfilters.tinymceaccordion-1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/setup.py` & `collective.outputfilters.tinymceaccordion-1.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CONTRIBUTORS.md").read(),
         open("CHANGES.md").read(),
     ]
 )
 
 setup(
     name="collective.outputfilters.tinymceaccordion",
-    version="1.0a4",
+    version="1.0a5",
     description="Addon for Plone 6 - Plone Outputfilter to transform TinyMCE Markup to Bootstrap5 Accordion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
```

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/configure.zcml` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/filter.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/filter.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/README.md` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/README.md`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/collective.outputfilters.tinymceaccordion.pot` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/collective.outputfilters.tinymceaccordion.pot`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/de/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/en/LC_MESSAGES/collective.outputfilters.tinymceaccordion.po`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/update.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/locales/update.sh` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/profiles.zcml` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/setuphandlers.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/testing.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/testing.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/test_filter.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective/outputfilters/tinymceaccordion/tests/test_setup.py` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective/outputfilters/tinymceaccordion/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/PKG-INFO` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.outputfilters.tinymceaccordion
-Version: 1.0a4
+Version: 1.0a5
 Summary: Addon for Plone 6 - Plone Outputfilter to transform TinyMCE Markup to Bootstrap5 Accordion
 Home-page: https://github.com/collective/collective.outputfilters.tinymceaccordion
 Author: 1letter
 Author-email: 1letter@gmx.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.outputfilters.tinymceaccordion/
 Project-URL: Source, https://github.com/collective/collective.outputfilters.tinymceaccordion
@@ -25,15 +25,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # README
 
-![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion)
+![Plone Meta Workflow](https://github.com/collective/collective.outputfilters.tinymceaccordion/actions/workflows/meta.yml/badge.svg "Plone Meta Workflow") [![codecov](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion/graph/badge.svg?token=Fr1Av8spXo "Code Coverage Workflow")](https://codecov.io/gh/collective/collective.outputfilters.tinymceaccordion) ![PyPI - Versions from Framework Classifiers](https://img.shields.io/pypi/frameworkversions/plone/collective.outputfilters.tinymceaccordion)
+
 
 - [README](#readme)
   - [Who need this addon?](#who-need-this-addon)
   - [Registry Settings](#registry-settings)
   - [Install Addon via buildout](#install-addon-via-buildout)
   - [Install Addon via pip](#install-addon-via-pip)
   - [Install a Testenvironment](#install-a-testenvironment)
@@ -209,14 +210,21 @@
 - 1letter, 1letter@gmx.de
 
 
 # Changelog
 
 <!-- towncrier release notes start -->
 
+## 1.0a5 (2024-04-28)
+
+
+### Internal:
+
+- Update README @1letter 
+
 ## 1.0a4 (2024-04-28)
 
 
 ### Internal:
 
 - remove unused files @1letter
```

### Comparing `collective.outputfilters.tinymceaccordion-1.0a4/src/collective.outputfilters.tinymceaccordion.egg-info/SOURCES.txt` & `collective.outputfilters.tinymceaccordion-1.0a5/src/collective.outputfilters.tinymceaccordion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

