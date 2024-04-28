# Comparing `tmp/adafruit_circuitpython_connectionmanager-1.1.0.tar.gz` & `tmp/adafruit_circuitpython_connectionmanager-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_connectionmanager-1.1.0.tar", last modified: Thu Apr 25 21:22:39 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_connectionmanager-1.2.0.tar", last modified: Sun Apr 28 04:21:43 2024, max compression
```

## Comparing `adafruit_circuitpython_connectionmanager-1.1.0.tar` & `adafruit_circuitpython_connectionmanager-1.2.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.778110 adafruit_circuitpython_connectionmanager-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.782110 adafruit_circuitpython_connectionmanager-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.782110 adafruit_circuitpython_connectionmanager-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.782110 adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-25 21:22:39.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 21:22:39.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:22:39.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 21:22:39.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 21:22:39.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/adafruit_connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.782110 adafruit_circuitpython_connectionmanager-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.782110 adafruit_circuitpython_connectionmanager-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/examples/connectionmanager_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/examples/connectionmanager_ssltest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:22:39.786110 adafruit_circuitpython_connectionmanager-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/close_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/free_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/get_connection_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/get_radio_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/get_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-25 21:22:37.000000 adafruit_circuitpython_connectionmanager-1.1.0/tests/ssl_context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-25 21:22:31.000000 adafruit_circuitpython_connectionmanager-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.784328 adafruit_circuitpython_connectionmanager-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.784328 adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_ssltest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/close_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/connection_manager_close_all_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/free_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_connection_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_radio_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/ssl_context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/tox.ini
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/.gitignore` & `adafruit_circuitpython_connectionmanager-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_connectionmanager-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/.pylintrc` & `adafruit_circuitpython_connectionmanager-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_connectionmanager-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/LICENSE` & `adafruit_circuitpython_connectionmanager-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/PKG-INFO` & `adafruit_circuitpython_connectionmanager-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 1.1.0
+Version: 1.2.0
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/README.rst` & `adafruit_circuitpython_connectionmanager-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO` & `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 1.1.0
+Version: 1.2.0
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt` & `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/connectionmanager_helpers.py
 examples/connectionmanager_ssltest.py
 tests/close_socket_test.py
 tests/conftest.py
+tests/connection_manager_close_all_test.py
 tests/free_socket_test.py
 tests/get_connection_manager_test.py
 tests/get_radio_test.py
 tests/get_socket_test.py
 tests/mocket.py
 tests/protocol_test.py
 tests/ssl_context_test.py
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/adafruit_connection_manager.py` & `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_connection_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
 # imports
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager.git"
 
 import errno
 import sys
 
 WIZNET5K_SSL_SUPPORT_VERSION = (9, 1)
 
 # typing
 
 
 if not sys.implementation.name == "circuitpython":
-    from typing import Optional, Tuple
+    from typing import List, Optional, Tuple
 
     from circuitpython_typing.socket import (
         CircuitPythonSocketType,
         InterfaceType,
         SocketpoolModuleType,
         SocketType,
         SSLContextType,
@@ -60,23 +60,22 @@
         self.recv_into = socket.recv_into
 
     def connect(self, address: Tuple[str, int]) -> None:
         """Connect wrapper to add non-standard mode parameter"""
         try:
             return self._socket.connect(address, self._mode)
         except RuntimeError as error:
-            raise OSError(errno.ENOMEM) from error
+            raise OSError(errno.ENOMEM, str(error)) from error
 
 
 class _FakeSSLContext:
     def __init__(self, iface: InterfaceType) -> None:
         self._iface = iface
 
-    # pylint: disable=unused-argument
-    def wrap_socket(
+    def wrap_socket(  # pylint: disable=unused-argument
         self, socket: CircuitPythonSocketType, server_hostname: Optional[str] = None
     ) -> _FakeSSLSocket:
         """Return the same socket"""
         if hasattr(self._iface, "TLS_MODE"):
             return _FakeSSLSocket(socket, self._iface.TLS_MODE)
 
         raise AttributeError("This radio does not support TLS/HTTPS")
@@ -95,29 +94,30 @@
      * `Adafruit AirLift FeatherWing – ESP32 WiFi Co-Processor
        <https://www.adafruit.com/product/4264>`_
     """
     socket_pool.set_interface(iface)
     return _FakeSSLContext(iface)
 
 
-_global_socketpool = {}
+_global_connection_managers = {}
+_global_socketpools = {}
 _global_ssl_contexts = {}
 
 
 def get_radio_socketpool(radio):
     """Helper to get a socket pool for common boards
 
     Currently supported:
 
      * Boards with onboard WiFi (ESP32S2, ESP32S3, Pico W, etc)
      * Using the ESP32 WiFi Co-Processor (like the Adafruit AirLift)
      * Using a WIZ5500 (Like the Adafruit Ethernet FeatherWing)
     """
     class_name = radio.__class__.__name__
-    if class_name not in _global_socketpool:
+    if class_name not in _global_socketpools:
         if class_name == "Radio":
             import ssl  # pylint: disable=import-outside-toplevel
 
             import socketpool  # pylint: disable=import-outside-toplevel
 
             pool = socketpool.SocketPool(radio)
             ssl_context = ssl.create_default_context()
@@ -147,18 +147,18 @@
 
             if ssl_context is None:
                 ssl_context = create_fake_ssl_context(pool, radio)
 
         else:
             raise AttributeError(f"Unsupported radio class: {class_name}")
 
-        _global_socketpool[class_name] = pool
+        _global_socketpools[class_name] = pool
         _global_ssl_contexts[class_name] = ssl_context
 
-    return _global_socketpool[class_name]
+    return _global_socketpools[class_name]
 
 
 def get_radio_ssl_context(radio):
     """Helper to get ssl_contexts for common boards
 
     Currently supported:
 
@@ -179,50 +179,83 @@
 
     def __init__(
         self,
         socket_pool: SocketpoolModuleType,
     ) -> None:
         self._socket_pool = socket_pool
         # Hang onto open sockets so that we can reuse them.
-        self._available_socket = {}
-        self._open_sockets = {}
-
-    def _free_sockets(self) -> None:
-        available_sockets = []
-        for socket, free in self._available_socket.items():
-            if free:
-                available_sockets.append(socket)
-
+        self._available_sockets = set()
+        self._key_by_managed_socket = {}
+        self._managed_socket_by_key = {}
+
+    def _free_sockets(self, force: bool = False) -> None:
+        # cloning lists since items are being removed
+        available_sockets = list(self._available_sockets)
         for socket in available_sockets:
             self.close_socket(socket)
+        if force:
+            open_sockets = list(self._managed_socket_by_key.values())
+            for socket in open_sockets:
+                self.close_socket(socket)
 
-    def _get_key_for_socket(self, socket):
+    def _get_connected_socket(  # pylint: disable=too-many-arguments
+        self,
+        addr_info: List[Tuple[int, int, int, str, Tuple[str, int]]],
+        host: str,
+        port: int,
+        timeout: float,
+        is_ssl: bool,
+        ssl_context: Optional[SSLContextType] = None,
+    ):
         try:
-            return next(
-                key for key, value in self._open_sockets.items() if value == socket
-            )
-        except StopIteration:
-            return None
+            socket = self._socket_pool.socket(addr_info[0], addr_info[1])
+        except (OSError, RuntimeError) as exc:
+            return exc
+
+        if is_ssl:
+            socket = ssl_context.wrap_socket(socket, server_hostname=host)
+            connect_host = host
+        else:
+            connect_host = addr_info[-1][0]
+        socket.settimeout(timeout)  # socket read timeout
+
+        try:
+            socket.connect((connect_host, port))
+        except (MemoryError, OSError) as exc:
+            socket.close()
+            return exc
+
+        return socket
+
+    @property
+    def available_socket_count(self) -> int:
+        """Get the count of freeable open sockets"""
+        return len(self._available_sockets)
+
+    @property
+    def managed_socket_count(self) -> int:
+        """Get the count of open sockets"""
+        return len(self._managed_socket_by_key)
 
     def close_socket(self, socket: SocketType) -> None:
         """Close a previously opened socket."""
-        if socket not in self._open_sockets.values():
+        if socket not in self._managed_socket_by_key.values():
             raise RuntimeError("Socket not managed")
-        key = self._get_key_for_socket(socket)
         socket.close()
-        del self._available_socket[socket]
-        del self._open_sockets[key]
+        key = self._key_by_managed_socket.pop(socket)
+        del self._managed_socket_by_key[key]
+        if socket in self._available_sockets:
+            self._available_sockets.remove(socket)
 
     def free_socket(self, socket: SocketType) -> None:
         """Mark a previously opened socket as available so it can be reused if needed."""
-        if socket not in self._open_sockets.values():
+        if socket not in self._managed_socket_by_key.values():
             raise RuntimeError("Socket not managed")
-        self._available_socket[socket] = True
+        self._available_sockets.add(socket)
 
-    # pylint: disable=too-many-branches,too-many-locals,too-many-statements
     def get_socket(
         self,
         host: str,
         port: int,
         proto: str,
         session_id: Optional[str] = None,
         *,
@@ -230,18 +263,18 @@
         is_ssl: bool = False,
         ssl_context: Optional[SSLContextType] = None,
     ) -> CircuitPythonSocketType:
         """Get a new socket and connect"""
         if session_id:
             session_id = str(session_id)
         key = (host, port, proto, session_id)
-        if key in self._open_sockets:
-            socket = self._open_sockets[key]
-            if self._available_socket[socket]:
-                self._available_socket[socket] = False
+        if key in self._managed_socket_by_key:
+            socket = self._managed_socket_by_key[key]
+            if socket in self._available_sockets:
+                self._available_sockets.remove(socket)
                 return socket
 
             raise RuntimeError(f"Socket already connected to {proto}//{host}:{port}")
 
         if proto == "https:":
             is_ssl = True
         if is_ssl and not ssl_context:
@@ -249,68 +282,72 @@
                 "ssl_context must be set before using adafruit_requests for https"
             )
 
         addr_info = self._socket_pool.getaddrinfo(
             host, port, 0, self._socket_pool.SOCK_STREAM
         )[0]
 
-        try_count = 0
-        socket = None
-        last_exc = None
-        while try_count < 2 and socket is None:
-            try_count += 1
-            if try_count > 1:
-                if any(
-                    socket
-                    for socket, free in self._available_socket.items()
-                    if free is True
-                ):
-                    self._free_sockets()
-                else:
-                    break
+        first_exception = None
+        result = self._get_connected_socket(
+            addr_info, host, port, timeout, is_ssl, ssl_context
+        )
+        if isinstance(result, Exception):
+            # Got an error, if there are any available sockets, free them and try again
+            if self.available_socket_count:
+                first_exception = result
+                self._free_sockets()
+                result = self._get_connected_socket(
+                    addr_info, host, port, timeout, is_ssl, ssl_context
+                )
+        if isinstance(result, Exception):
+            last_result = f", first error: {first_exception}" if first_exception else ""
+            raise RuntimeError(
+                f"Error connecting socket: {result}{last_result}"
+            ) from result
+
+        self._key_by_managed_socket[result] = key
+        self._managed_socket_by_key[key] = result
+        return result
 
-            try:
-                socket = self._socket_pool.socket(addr_info[0], addr_info[1])
-            except OSError as exc:
-                last_exc = exc
-                continue
-            except RuntimeError as exc:
-                last_exc = exc
-                continue
-
-            if is_ssl:
-                socket = ssl_context.wrap_socket(socket, server_hostname=host)
-                connect_host = host
-            else:
-                connect_host = addr_info[-1][0]
-            socket.settimeout(timeout)  # socket read timeout
-
-            try:
-                socket.connect((connect_host, port))
-            except MemoryError as exc:
-                last_exc = exc
-                socket.close()
-                socket = None
-            except OSError as exc:
-                last_exc = exc
-                socket.close()
-                socket = None
 
-        if socket is None:
-            raise RuntimeError(f"Error connecting socket: {last_exc}") from last_exc
+# global helpers
 
-        self._available_socket[socket] = False
-        self._open_sockets[key] = socket
-        return socket
 
+def connection_manager_close_all(
+    socket_pool: Optional[SocketpoolModuleType] = None, release_references: bool = False
+) -> None:
+    """Close all open sockets for pool"""
+    if socket_pool:
+        socket_pools = [socket_pool]
+    else:
+        socket_pools = _global_connection_managers.keys()
+
+    for pool in socket_pools:
+        connection_manager = _global_connection_managers.get(pool, None)
+        if connection_manager is None:
+            raise RuntimeError("SocketPool not managed")
+
+        connection_manager._free_sockets(force=True)  # pylint: disable=protected-access
+
+        if release_references:
+            radio_key = None
+            for radio_check, pool_check in _global_socketpools.items():
+                if pool == pool_check:
+                    radio_key = radio_check
+                    break
 
-# global helpers
+            if radio_key:
+                if radio_key in _global_socketpools:
+                    del _global_socketpools[radio_key]
 
+                if radio_key in _global_ssl_contexts:
+                    del _global_ssl_contexts[radio_key]
 
-_global_connection_manager = {}
+            if pool in _global_connection_managers:
+                del _global_connection_managers[pool]
 
 
 def get_connection_manager(socket_pool: SocketpoolModuleType) -> ConnectionManager:
     """Get the ConnectionManager singleton for the given pool"""
-    if socket_pool not in _global_connection_manager:
-        _global_connection_manager[socket_pool] = ConnectionManager(socket_pool)
-    return _global_connection_manager[socket_pool]
+    if socket_pool not in _global_connection_managers:
+        _global_connection_managers[socket_pool] = ConnectionManager(socket_pool)
+    return _global_connection_managers[socket_pool]
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/docs/conf.py` & `adafruit_circuitpython_connectionmanager-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/docs/examples.rst` & `adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/docs/index.rst` & `adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/examples/connectionmanager_ssltest.py` & `adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_ssltest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/pyproject.toml` & `adafruit_circuitpython_connectionmanager-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-connectionmanager"
 description = "A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections"
-version = "1.1.0"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/close_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/close_socket_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     # validate socket is tracked
     socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
     key = (mocket.MOCK_HOST_1, 80, "http:", None)
     assert socket == mock_socket_1
-    assert socket in connection_manager._available_socket
-    assert key in connection_manager._open_sockets
+    assert socket not in connection_manager._available_sockets
+    assert key in connection_manager._managed_socket_by_key
 
     # validate socket is no longer tracked
     connection_manager.close_socket(socket)
-    assert socket not in connection_manager._available_socket
-    assert key not in connection_manager._open_sockets
+    assert socket not in connection_manager._available_sockets
+    assert key not in connection_manager._managed_socket_by_key
 
 
 def test_close_socket_not_managed():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/conftest.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,18 @@
     del sys.modules["adafruit_wiznet5k"]
     del sys.modules["adafruit_wiznet5k.adafruit_wiznet5k_socket"]
 
 
 @pytest.fixture(autouse=True)
 def reset_connection_manager(monkeypatch):
     monkeypatch.setattr(
-        "adafruit_connection_manager._global_socketpool",
+        "adafruit_connection_manager._global_connection_managers",
+        {},
+    )
+    monkeypatch.setattr(
+        "adafruit_connection_manager._global_socketpools",
         {},
     )
     monkeypatch.setattr(
         "adafruit_connection_manager._global_ssl_contexts",
         {},
     )
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/free_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/free_socket_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 
 def test_free_socket():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.return_value = mock_socket_1
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
+    assert connection_manager.managed_socket_count == 0
+    assert connection_manager.available_socket_count == 0
 
     # validate socket is tracked and not available
     socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
     key = (mocket.MOCK_HOST_1, 80, "http:", None)
     assert socket == mock_socket_1
-    assert socket in connection_manager._available_socket
-    assert connection_manager._available_socket[socket] is False
-    assert key in connection_manager._open_sockets
+    assert socket not in connection_manager._available_sockets
+    assert key in connection_manager._managed_socket_by_key
+    assert connection_manager.managed_socket_count == 1
+    assert connection_manager.available_socket_count == 0
 
     # validate socket is tracked and is available
     connection_manager.free_socket(socket)
-    assert socket in connection_manager._available_socket
-    assert connection_manager._available_socket[socket] is True
-    assert key in connection_manager._open_sockets
+    assert socket in connection_manager._available_sockets
+    assert key in connection_manager._managed_socket_by_key
+    assert connection_manager.managed_socket_count == 1
+    assert connection_manager.available_socket_count == 1
 
 
 def test_free_socket_not_managed():
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
@@ -50,50 +54,35 @@
     mock_socket_2 = mocket.Mocket()
     mock_pool.socket.side_effect = [
         mock_socket_1,
         mock_socket_2,
     ]
 
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
+    assert connection_manager.managed_socket_count == 0
+    assert connection_manager.available_socket_count == 0
 
     # validate socket is tracked and not available
     socket_1 = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
     assert socket_1 == mock_socket_1
-    assert socket_1 in connection_manager._available_socket
-    assert connection_manager._available_socket[socket_1] is False
+    assert socket_1 not in connection_manager._available_sockets
+    assert connection_manager.managed_socket_count == 1
+    assert connection_manager.available_socket_count == 0
 
     socket_2 = connection_manager.get_socket(mocket.MOCK_HOST_2, 80, "http:")
     assert socket_2 == mock_socket_2
+    assert connection_manager.managed_socket_count == 2
+    assert connection_manager.available_socket_count == 0
 
     # validate socket is tracked and is available
     connection_manager.free_socket(socket_1)
-    assert socket_1 in connection_manager._available_socket
-    assert connection_manager._available_socket[socket_1] is True
+    assert socket_1 in connection_manager._available_sockets
+    assert connection_manager.managed_socket_count == 2
+    assert connection_manager.available_socket_count == 1
 
     # validate socket is no longer tracked
     connection_manager._free_sockets()
-    assert socket_1 not in connection_manager._available_socket
-    assert socket_2 in connection_manager._available_socket
+    assert socket_1 not in connection_manager._available_sockets
+    assert socket_2 not in connection_manager._available_sockets
     mock_socket_1.close.assert_called_once()
-
-
-def test_get_key_for_socket():
-    mock_pool = mocket.MocketPool()
-    mock_socket_1 = mocket.Mocket()
-    mock_pool.socket.return_value = mock_socket_1
-
-    connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
-
-    # validate tracked socket has correct key
-    socket = connection_manager.get_socket(mocket.MOCK_HOST_1, 80, "http:")
-    key = (mocket.MOCK_HOST_1, 80, "http:", None)
-    assert connection_manager._get_key_for_socket(socket) == key
-
-
-def test_get_key_for_socket_not_managed():
-    mock_pool = mocket.MocketPool()
-    mock_socket_1 = mocket.Mocket()
-
-    connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
-
-    # validate untracked socket has no key
-    assert connection_manager._get_key_for_socket(mock_socket_1) is None
+    assert connection_manager.managed_socket_count == 1
+    assert connection_manager.available_socket_count == 0
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/get_connection_manager_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_connection_manager_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/get_radio_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_radio_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,31 +15,34 @@
 
 def test_get_radio_socketpool_wifi(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
     radio = mocket.MockRadio.Radio()
     socket_pool = adafruit_connection_manager.get_radio_socketpool(radio)
     assert isinstance(socket_pool, mocket.MocketPool)
+    assert socket_pool in adafruit_connection_manager._global_socketpools.values()
 
 
 def test_get_radio_socketpool_esp32spi(  # pylint: disable=unused-argument
     adafruit_esp32spi_socket_module,
 ):
     radio = mocket.MockRadio.ESP_SPIcontrol()
     socket_pool = adafruit_connection_manager.get_radio_socketpool(radio)
     assert socket_pool.__name__ == "adafruit_esp32spi_socket"
+    assert socket_pool in adafruit_connection_manager._global_socketpools.values()
 
 
 def test_get_radio_socketpool_wiznet5k(  # pylint: disable=unused-argument
     adafruit_wiznet5k_socket_module,
 ):
     radio = mocket.MockRadio.WIZNET5K()
     with mock.patch("sys.implementation", return_value=[9, 0, 0]):
         socket_pool = adafruit_connection_manager.get_radio_socketpool(radio)
     assert socket_pool.__name__ == "adafruit_wiznet5k_socket"
+    assert socket_pool in adafruit_connection_manager._global_socketpools.values()
 
 
 def test_get_radio_socketpool_unsupported():
     radio = mocket.MockRadio.Unsupported()
     with pytest.raises(AttributeError) as context:
         adafruit_connection_manager.get_radio_socketpool(radio)
     assert "Unsupported radio class" in str(context)
@@ -48,48 +51,53 @@
 def test_get_radio_socketpool_returns_same_one(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
     radio = mocket.MockRadio.Radio()
     socket_pool_1 = adafruit_connection_manager.get_radio_socketpool(radio)
     socket_pool_2 = adafruit_connection_manager.get_radio_socketpool(radio)
     assert socket_pool_1 == socket_pool_2
+    assert socket_pool_1 in adafruit_connection_manager._global_socketpools.values()
 
 
 def test_get_radio_ssl_context_wifi(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
     radio = mocket.MockRadio.Radio()
-    ssl_contexts = adafruit_connection_manager.get_radio_ssl_context(radio)
-    assert isinstance(ssl_contexts, ssl.SSLContext)
+    ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
+    assert isinstance(ssl_context, ssl.SSLContext)
+    assert ssl_context in adafruit_connection_manager._global_ssl_contexts.values()
 
 
 def test_get_radio_ssl_context_esp32spi(  # pylint: disable=unused-argument
     adafruit_esp32spi_socket_module,
 ):
     radio = mocket.MockRadio.ESP_SPIcontrol()
-    ssl_contexts = adafruit_connection_manager.get_radio_ssl_context(radio)
-    assert isinstance(ssl_contexts, adafruit_connection_manager._FakeSSLContext)
+    ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
+    assert isinstance(ssl_context, adafruit_connection_manager._FakeSSLContext)
+    assert ssl_context in adafruit_connection_manager._global_ssl_contexts.values()
 
 
 def test_get_radio_ssl_context_wiznet5k(  # pylint: disable=unused-argument
     adafruit_wiznet5k_socket_module,
 ):
     radio = mocket.MockRadio.WIZNET5K()
     with mock.patch("sys.implementation", return_value=[9, 0, 0]):
-        ssl_contexts = adafruit_connection_manager.get_radio_ssl_context(radio)
-    assert isinstance(ssl_contexts, adafruit_connection_manager._FakeSSLContext)
+        ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
+    assert isinstance(ssl_context, adafruit_connection_manager._FakeSSLContext)
+    assert ssl_context in adafruit_connection_manager._global_ssl_contexts.values()
 
 
 def test_get_radio_ssl_context_unsupported():
     radio = mocket.MockRadio.Unsupported()
     with pytest.raises(AttributeError) as context:
         adafruit_connection_manager.get_radio_ssl_context(radio)
     assert "Unsupported radio class" in str(context)
 
 
 def test_get_radio_ssl_context_returns_same_one(  # pylint: disable=unused-argument
     circuitpython_socketpool_module,
 ):
     radio = mocket.MockRadio.Radio()
-    ssl_contexts_1 = adafruit_connection_manager.get_radio_ssl_context(radio)
-    ssl_contexts_2 = adafruit_connection_manager.get_radio_ssl_context(radio)
-    assert ssl_contexts_1 == ssl_contexts_2
+    ssl_context_1 = adafruit_connection_manager.get_radio_ssl_context(radio)
+    ssl_context_2 = adafruit_connection_manager.get_radio_ssl_context(radio)
+    assert ssl_context_1 == ssl_context_2
+    assert ssl_context_1 in adafruit_connection_manager._global_ssl_contexts.values()
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/get_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_socket_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     assert socket == mock_socket_1
     connection_manager.free_socket(socket)
     free_sockets_mock.assert_not_called()
 
     # try to get a socket that returns a RuntimeError twice
     with pytest.raises(RuntimeError) as context:
         connection_manager.get_socket(mocket.MOCK_HOST_2, 80, "http:")
-    assert "Error connecting socket: error 2" in str(context)
+    assert "Error connecting socket: error 2, first error: error 1" in str(context)
     free_sockets_mock.assert_called_once()
 
 
 def test_fake_ssl_context_connect(  # pylint: disable=unused-argument
     adafruit_esp32spi_socket_module,
 ):
     mock_pool = mocket.MocketPool()
@@ -238,18 +238,18 @@
 
 def test_fake_ssl_context_connect_error(  # pylint: disable=unused-argument
     adafruit_esp32spi_socket_module,
 ):
     mock_pool = mocket.MocketPool()
     mock_socket_1 = mocket.Mocket()
     mock_pool.socket.return_value = mock_socket_1
-    mock_socket_1.connect.side_effect = RuntimeError("RuntimeError ")
+    mock_socket_1.connect.side_effect = RuntimeError("RuntimeError")
 
     radio = mocket.MockRadio.ESP_SPIcontrol()
     ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
     connection_manager = adafruit_connection_manager.ConnectionManager(mock_pool)
 
     with pytest.raises(RuntimeError) as context:
         connection_manager.get_socket(
             mocket.MOCK_HOST_1, 443, "https:", ssl_context=ssl_context
         )
-    assert "Error connecting socket: 12" in str(context)
+    assert "Error connecting socket: [Errno 12] RuntimeError" in str(context)
```

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/mocket.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/protocol_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tests/ssl_context_test.py` & `adafruit_circuitpython_connectionmanager-1.2.0/tests/ssl_context_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.1.0/tox.ini` & `adafruit_circuitpython_connectionmanager-1.2.0/tox.ini`

 * *Files identical despite different names*

