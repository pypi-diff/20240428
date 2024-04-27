# Comparing `tmp/oresat-olaf-3.4.0.tar.gz` & `tmp/oresat_olaf-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-3.4.0.tar", last modified: Thu Mar  7 05:17:54 2024, max compression
+gzip compressed data, was "oresat_olaf-3.5.0.tar", last modified: Sat Apr 27 22:21:52 2024, max compression
```

## Comparing `oresat-olaf-3.4.0.tar` & `oresat_olaf-3.5.0.tar`

### file list

```diff
@@ -1,135 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.143331 oresat-olaf-3.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.147331 oresat-olaf-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.151331 oresat-olaf-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.151331 oresat-olaf-3.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/adc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/app.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/cpufreq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/daemon.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/ecss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/gpio.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/node.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/oresat_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/oresat_file_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/pru.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/resource.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/rest_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/service.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/timer_loop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/api/updater.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/rest_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.151331 oresat-olaf-3.4.0/docs/updater/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/updater/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/docs/updater/update_archive.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.151331 oresat-olaf-3.4.0/olaf/
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/master_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    19247 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/daemons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/resources/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)    13228 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/daemons.html
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/reset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/updater.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.155331 oresat-olaf-3.4.0/olaf/_internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/services/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/services/os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/services/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/_internals/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/olaf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.159331 oresat-olaf-3.4.0/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/pru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 05:17:54.000000 oresat-olaf-3.4.0/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/run.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.159331 oresat-olaf-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.159331 oresat-olaf-3.4.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/test_oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/test_pru.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/common/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/resources/test_fwrite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/tests/internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/services/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/test_rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:17:54.163331 oresat-olaf-3.4.0/tests/internals/updater/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test-script.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611941111.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611947777.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611948888.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-03-07 05:17:48.000000 oresat-olaf-3.4.0/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.036912 oresat_olaf-3.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.040912 oresat_olaf-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.040912 oresat_olaf-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/adc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/cpufreq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/daemon.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/ecss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/gpio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/node.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/oresat_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/oresat_file_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/pru.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/rest_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/service.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/timer_loop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/updater.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/rest_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/docs/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/updater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/updater/update_archive.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    13228 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/daemons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/reset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/updater.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/_internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 22:21:51.000000 oresat_olaf-3.5.0/olaf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/pru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/canopen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_pru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_fwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/services/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/tests/internals/updater/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-script.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611941111.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611947777.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611948888.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-3.4.0/.github/workflows/pypi.yaml` & `oresat_olaf-3.5.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/.github/workflows/tests.yaml` & `oresat_olaf-3.5.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/.gitignore` & `oresat_olaf-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/LICENSE` & `oresat_olaf-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/PKG-INFO` & `oresat_olaf-3.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.4.0
+Version: 3.5.0
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: flask
 Requires-Dist: loguru
 Requires-Dist: natsort
 Requires-Dist: psutil
+Requires-Dist: python-can>=4.3.0
 Requires-Dist: oresat-configs
 
 OLAF (OreSat Linux App Framework)
 =================================
 
 .. image:: https://img.shields.io/github/license/oresat/oresat-olaf
    :target: https://github.com/oresat/oresat-olaf/blob/master/LICENSE
```

### Comparing `oresat-olaf-3.4.0/README.rst` & `oresat_olaf-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/Makefile` & `oresat_olaf-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/api/ecss.rst` & `oresat_olaf-3.5.0/docs/api/ecss.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/api/oresat_file.rst` & `oresat_olaf-3.5.0/docs/api/oresat_file.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/api/rest_api.rst` & `oresat_olaf-3.5.0/docs/api/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/conf.py` & `oresat_olaf-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/glossary.rst` & `oresat_olaf-3.5.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/index.rst` & `oresat_olaf-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/make.bat` & `oresat_olaf-3.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/rest_api.rst` & `oresat_olaf-3.5.0/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/updater/index.rst` & `oresat_olaf-3.5.0/docs/updater/index.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/docs/updater/update_archive.rst` & `oresat_olaf-3.5.0/docs/updater/update_archive.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/__init__.py` & `oresat_olaf-3.5.0/olaf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """OLAF (OreSat Linux App Framework)"""
 
 import sys
 from argparse import ArgumentParser, Namespace
 from logging.handlers import SysLogHandler
 from typing import Optional
 
-import can
 from loguru import logger
 from oresat_configs import OreSatConfig, OreSatId
 
 from ._internals.app import App, app
-from ._internals.master_node import MasterNode
-from ._internals.node import NetworkError, Node, NodeStop
 from ._internals.rest_api import RestAPI, render_olaf_template, rest_api
 from ._internals.services.logs import logger_tmp_file_setup
 from ._internals.updater import Updater, UpdaterState
-from .common.adc import Adc
-from .common.cpufreq import A8_CPUFREQS, get_cpufreq, get_cpufreq_gov, set_cpufreq, set_cpufreq_gov
+from .board.adc import Adc
+from .board.cpufreq import A8_CPUFREQS, get_cpufreq, get_cpufreq_gov, set_cpufreq, set_cpufreq_gov
+from .board.gpio import GPIO_HIGH, GPIO_IN, GPIO_LOW, GPIO_OUT, Gpio, GpioError
+from .board.pru import Pru, PruError, PruState
+from .canopen.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
+from .canopen.master_node import MasterNode
+from .canopen.network import CanNetwork, CanNetworkError, CanNetworkState, NetworkError
+from .canopen.node import Node, NodeStop
 from .common.daemon import Daemon, DaemonState
-from .common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
-from .common.gpio import GPIO_HIGH, GPIO_IN, GPIO_LOW, GPIO_OUT, Gpio, GpioError
 from .common.oresat_file import OreSatFile, new_oresat_file
 from .common.oresat_file_cache import OreSatFileCache
-from .common.pru import Pru, PruError, PruState
 from .common.resource import Resource
 from .common.service import Service, ServiceState
 from .common.timer_loop import TimerLoop
 
 try:
     from ._version import version as __version__  # type: ignore
 except ImportError:
@@ -141,20 +141,18 @@
     if args.hardware_version != "0.0":
         od["versions"]["hw_version"].value = args.hardware_version
 
     is_octavo = config.cards[name].processor == "octavo"
     if is_octavo:
         od["versions"]["olaf_version"].value = __version__
 
-    bus = can.interface.Bus(
-        interface=args.bus_type, host=args.socketcand_host, port=29536, channel=args.bus
-    )
+    network = CanNetwork(args.bus_type, args.bus, args.socketcand_host)
     od_db = config.od_db if name == "c3" else None
 
-    app.setup(od, bus, od_db, is_octavo)
+    app.setup(network, od, od_db, is_octavo)
     rest_api.setup(address=args.address, port=args.port)
 
     return args, config
 
 
 def olaf_run():
     """Start the app and REST API."""
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/app.py` & `oresat_olaf-3.5.0/olaf/_internals/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """OLAF App."""
 
 import os
 import signal
 import subprocess
 from typing import Union
 
-import can
 import canopen
 from loguru import logger
 
+from ..canopen.master_node import MasterNode
+from ..canopen.network import CanNetwork
+from ..canopen.node import Node, NodeStop
 from ..common.resource import Resource
 from ..common.service import Service
-from .master_node import MasterNode
-from .node import Node, NodeStop
 from .resources.ecss import EcssResource
 from .resources.fread import FreadResource
 from .resources.fwrite import FwriteResource
 from .resources.system import SystemResource
 from .services.logs import LogsService
-
-# from .resources.daemons import DaemonsResource
 from .services.os_command import OsCommandService
 from .services.updater import UpdaterService
 from .updater import Updater
 
 
 class App:
     """
-    The application class that manages the CAN bus and resources.
+    The application class that manages the CANopen node and resources.
 
     Use the global ``olaf.app`` obect.
     """
 
     def __init__(self):
         self._od = None
         self._resources = []
@@ -47,45 +45,45 @@
         """Called when signals are caught"""
 
         logger.debug(f"signal {signal.Signals(signo).name} was caught")
         self.stop()
 
     def setup(
         self,
+        network: CanNetwork,
         od: canopen.ObjectDictionary,
-        bus: can.BusABC,
         master_od_db: Union[dict, None] = None,
         load_core: bool = True,
     ):
         """
         Setup the app. Will be called by ``olaf_setup`` automatically.
 
         Parameters
         ----------
-        node: Node
-            The node for the app.
-        bus: can.BusABC
-            The can bus object to use.
+        network: CanNetwork
+            The CAN network to use.
+        od: canopen.ObjectDictionary
+            The nodes object dictionary.
         master_od_db: dict
             Master node od database. Only for the C3.
         load_core: bool
             Load the core olaf services and resources
 
         Raises
         ------
         ValueError
             Invalid parameter(s)
         """
 
         self._od = od
 
         if master_od_db:
-            self._node = MasterNode(self._od, master_od_db, bus)
+            self._node = MasterNode(network, self._od, master_od_db)
         else:
-            self._node = Node(self._od, bus)
+            self._node = Node(network, self._od)
 
         # setup updater
         self._updater = Updater(
             f"{self._node.work_base_dir}/updater", f"{self._node.cache_base_dir}/updates"
         )
 
         if load_core:
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/master_node.py` & `oresat_olaf-3.5.0/olaf/canopen/master_node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 """OreSat CANopen Master Node class to support the C3"""
 
 from collections import namedtuple
 from time import monotonic
 from typing import Any, Dict, Union
 
-import can
 import canopen
 from loguru import logger
 
-from .node import NetworkError, Node
+from ..canopen.network import CanNetwork, CanNetworkError, CanNetworkState
+from .node import Node
 
 NodeHeartbeatInfo = namedtuple("NodeHeartbeatInfo", ["state", "timestamp", "time_since_boot"])
 
 
 class MasterNode(Node):
     """OreSat CANopen Master Node (only used by the C3)"""
 
     def __init__(
         self,
+        network: CanNetwork,
         od: canopen.ObjectDictionary,
         od_db: Dict[Any, canopen.ObjectDictionary],
-        bus: can.BusABC,
     ):
         """
         Parameters
         ----------
+        network: CanNetwork
+            The CAN network
         od: canopen.ObjectDictionary
             The CANopen ObjectDictionary
         od_db: Dict[Any, canopen.ObjectDictionary]
             Database of other nodes's ODs. The dict key will be used by class fields and methods.
-        bus: can.BusABC
-            The can bus object to use.
         """
 
-        super().__init__(od, bus)
+        super().__init__(network, od)
 
         self._od_db = od_db
-
+        self.network = network
         self._node_id_to_key = {od.node_id: key for key, od in od_db.items()}
 
         self._remote_nodes = {}
         self.node_status = {}
-        for key in od_db:
-            if od_db[key] == od:
+        for k, v in self._od_db.items():
+            if v == od:
                 continue  # skip itself
-            self._remote_nodes[key] = canopen.RemoteNode(od_db[key].node_id, od_db[key])
-            self.node_status[key] = NodeHeartbeatInfo(
+            self._remote_nodes[k] = canopen.RemoteNode(v.node_id, v)
+            self.node_status[k] = NodeHeartbeatInfo(
                 0xFF,
                 0.0,
                 0.0,
             )  # 0xFF is a flag, not a CANopen standard
+            self._network.subscribe(0x80 + v.node_id, self._on_emergency)
+            self._network.subscribe(0x700 + v.node_id, self._on_heartbeat)
+
+        self._network.add_reset_callback(self._restart_network)
 
     def _restart_network(self):
         """Restart the CANopen network"""
-        super()._restart_network()
 
         for key, od in self._od_db.items():
             if od == self._od:
                 continue  # skip itself
             self.node_status[key] = NodeHeartbeatInfo(0xFF, 0.0, 0.0)
-            self._network.subscribe(0x80 + od.node_id, self._on_emergency)
-            self._network.subscribe(0x700 + od.node_id, self._on_heartbeat)
 
         for remote_node in self._remote_nodes.values():
             self._network.add_node(remote_node)
 
     def _on_heartbeat(self, cob_id: int, data: bytes, timestamp: float):
         """Callback on node hearbeat messages."""
 
@@ -79,25 +80,17 @@
         node_id = cob_id - 0x80
         value_str = data.hex(sep=" ")
         logger.error(f"node {node_id:02X} raised emergency: {value_str}")
 
     def send_sync(self):
         """
         Send a CANopen SYNC message.
-
-        Raises
-        ------
-        NetworkError
-            Cannot send a SYNC message when the network is down.
         """
 
-        if self._network is None:
-            raise NetworkError("network is down cannot send an SYNC message")
-
-        self._network.sync.transmit()
+        self._network.send_message(0x80, b"", False)
 
     def sdo_read(self, key: Any, index: Union[int, str], subindex: Union[int, str]) -> Any:
         """
         Read a value from a remote node's object dictionary using an SDO.
 
         Parameters
         ----------
@@ -106,27 +99,27 @@
         index: int or str
             The index to read from.
         subindex: int or str
             The subindex to read from.
 
         Raises
         ------
-        NetworkError
+        CanNetworkError
             Cannot send a SDO read message when the network is down.
         canopen.SdoError
             Error with the SDO.
 
         Returns
         -------
         Any
             The value read.
         """
 
-        if self._network is None:
-            raise NetworkError("network is down cannot send an SDO read message")
+        if self._network.status == CanNetworkState.NETWORK_UP:
+            raise CanNetworkError("network is down cannot send an SDO read message")
 
         if subindex == 0 and isinstance(self._od_db[key][index], canopen.objectdictionary.Variable):
             value = self._remote_nodes[key].sdo[index].raw
         else:
             value = self._remote_nodes[key].sdo[index][subindex].raw
 
         return value
@@ -144,22 +137,22 @@
         subindex: int
             The subindex to write to.
         value: Any
             The value to write.
 
         Raises
         ------
-        NetworkError
+        CanNetworkError
             Cannot send a SDO write message when the network is down.
         canopen.SdoError
             Error with the SDO.
         """
 
-        if self._network is None:
-            raise NetworkError("network is down cannot send an SDO write message")
+        if self._network.status == CanNetworkState.NETWORK_UP:
+            raise CanNetworkError("network is down cannot send an SDO write message")
 
         if subindex == 0 and isinstance(self._od_db[key][index], canopen.objectdictionary.Variable):
             self._remote_nodes[key].sdo[index].raw = value
         else:
             self._remote_nodes[key].sdo[index][subindex].raw = value
 
     @property
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/node.py` & `oresat_olaf-3.5.0/olaf/canopen/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 """OreSat CANopen Node"""
 
 import os
 import struct
-import subprocess
-from enum import IntEnum, auto
+from enum import IntEnum
 from pathlib import Path
 from threading import Event
+from time import monotonic
 from typing import Any, Callable, Dict, Union
 
-import can
 import canopen
-import psutil
 from loguru import logger
 
+from ..canopen.network import CanNetwork, CanNetworkState
 from ..common.daemon import Daemon
 from ..common.oresat_file_cache import OreSatFileCache
-from ..common.timer_loop import TimerLoop
-
-
-class CanState(IntEnum):
-    """CAN bus states."""
-
-    BUS_UP_NETWORK_UP = auto()
-    BUS_UP_NETWORK_DOWN = auto()
-    BUS_DOWN = auto()
-    BUS_NOT_FOUND = auto()
 
 
 class NodeStop(IntEnum):
     """Node stop commands."""
 
     SOFT_RESET = 1
     """Just stop the app and exit. Systemd will restart the app."""
@@ -36,65 +25,51 @@
     """Reboot system after app has stopped"""
     FACTORY_RESET = 3
     """Clear all file cachces and reboot system after app has stopped"""
     POWER_OFF = 4
     """Just power off the system."""
 
 
-class NetworkError(Exception):
-    """Error with the CANopen network / bus"""
-
-
 class Node:
     """
     OreSat CANopen Node class
 
     Jobs:
     - It abstracts away the canopen.LocalNode and canopen.Network from Resources and Services.
     - Provides access to the OD for Resources and Services.
     - Lets Resources and Services send TPDOs.
     - Lets Resources and Services send EMCY messages.
     - Set up the file transfer caches.
     - Starts/stops all Resources and Services.
-    - Sets up all timer-base TPDO threads.
+    - Sets up all timer-base TPDOs.
     - Sets up all RPDO callbacks.
-    - Monitor and resets the CAN bus if it goes into a bad state.
 
     Basically it tries to abstract all the CANopen things as much a possible, while providing a
     basic API for CANopen things.
     """
 
-    def __init__(
-        self,
-        od: canopen.ObjectDictionary,
-        bus: can.BusABC,
-    ):
+    def __init__(self, network: CanNetwork, od: canopen.ObjectDictionary):
         """
         Parameters
         ----------
+        network: CanNetwork
+            The CAN network
         od: canopen.ObjectDictionary
             The CANopen ObjectDictionary
-        bus: can.BusABC
-            The can bus object to use.
         """
 
+        self._event = Event()
         self._od = od
-        self._bus = bus
-        self._channel = self._bus.channel_info.split(" ")[-1].replace("'", "")
-        self._bus_state = CanState.BUS_DOWN
         self._node: canopen.LocalNode = None
-        self._network: canopen.Network = None
-        self._event = Event()
+        self._network: CanNetwork = network
         self._read_cbs = {}  # type: ignore
         self._write_cbs = {}  # type: ignore
         self._syncs = 0
         self._reset = NodeStop.SOFT_RESET
-        self._tpdo_timers = []  # type: ignore
         self._daemons = {}  # type: ignore
-        self.first_bus_reset = False
 
         if os.geteuid() == 0:  # running as root
             self.work_base_dir = "/var/lib/oresat"
             self.cache_base_dir = "/var/cache/oresat"
         else:
             self.work_base_dir = str(Path.home()) + "/.oresat"
             self.cache_base_dir = str(Path.home()) + "/.cache/oresat"
@@ -104,71 +79,87 @@
 
         self._fread_cache = OreSatFileCache(fread_path)
         self._fwrite_cache = OreSatFileCache(fwrite_path)
 
         logger.debug(f"fread cache path {self._fread_cache.dir}")
         logger.debug(f"fwrite cache path {self._fwrite_cache.dir}")
 
+        self._start_time = monotonic()
+        self._network.monitor()
+        self._first_network_reset = True
+        self._network.add_reset_callback(self._setup_node)
+        self._network.subscribe(0x80, self._on_sync)
+
+        self._rpdo_cobid_to_num: dict[int, int] = {}
+        for i in range(self._od.device_information.nr_of_RXPDO):
+            cob_id = self._od[0x1400 + i][1].value
+            self._rpdo_cobid_to_num[cob_id] = i
+            self._network.subscribe(cob_id, self._on_pdo)
+
     def __del__(self):
         # stop the monitor thread if it is running
         if not self._event.is_set():
             self.stop()
 
-        # stop the CANopen network
-        if self._network:
-            try:
-                self._network.disconnect()
-            except Exception:  # pylint: disable=W0718
-                pass
-
-        self._bus.shutdown()
-
     def _on_sync(self, cob_id: int, data: bytes, timestamp: float):  # pylint: disable=W0613
         """On SYNC message send TPDOs configured to be SYNC-based"""
 
         self._syncs += 1
         if self._syncs == 241:
             self._syncs = 1
 
-        for i in range(16):
+        for i in range(self.od.device_information.nr_of_TXPDO):
             transmission_type = self.od[0x1800 + i][2].value
             if self._syncs % transmission_type == 0:
                 self.send_tpdo(i)
 
+    def _on_pdo(self, cob_id: int, data: bytes, timestamp: float):  # pylint: disable=W0613
+        rpdo = self._rpdo_cobid_to_num[cob_id]
+        maps = self.od[0x1600 + rpdo][0].value
+
+        offset = 0
+        for i in range(maps):
+            pdo_map = self.od[0x1600 + rpdo][i + 1].value
+
+            if pdo_map == 0:
+                break  # nothing todo
+
+            pdo_map_bytes = pdo_map.to_bytes(4, "big")
+            index, subindex, size = struct.unpack(">HBB", pdo_map_bytes)
+            size //= 8
+
+            # call sdo callback(s) and convert data to bytes
+            if isinstance(self.od[index], canopen.objectdictionary.Variable):
+                self._node.sdo[index].raw = data[offset : offset + size]
+            else:  # record or array
+                self._node.sdo[index][subindex].raw = data[offset : offset + size]
+
+            offset += size
+
     def send_tpdo(self, tpdo: int):
         """
         Send a TPDO. Will not be sent if not node is not in operational state.
 
         Parameters
         ----------
         tpdo: int
             TPDO number to send, should be between 1 and 16.
-
-        Raises
-        ------
-        NetworkError
-            Cannot send a TPDO message when the network is down.
         """
 
-        if self._network is None:
-            raise NetworkError("network is down cannot send an TPDO message")
-
         if tpdo < 1:
             raise ValueError("TPDO number must be greather than 1")
 
+        if self._network.status != CanNetworkState.NETWORK_UP:
+            logger.debug("network is down cannot send an TPDO message")
+            return
+
         tpdo -= 1  # number to offset
 
-        # PDOs can't be sent if CAN bus is down and PDOs should not be sent if CAN bus not in
-        # 'OPERATIONAL' state
-        can_bus = psutil.net_if_stats().get(self._channel)
-        if (
-            can_bus is None
-            or self._node is None
-            or (can_bus.isup and self._node.nmt.state != "OPERATIONAL")
-        ):
+        # PDOs should not be sent if CAN bus not in 'OPERATIONAL' state as defined by spec
+        if self._node is None or self._node.nmt.state != "OPERATIONAL":
             return
 
         cob_id = self.od[0x1800 + tpdo][1].value & 0x3F_FF_FF_FF
         maps = self.od[0x1A00 + tpdo][0].value
 
         data = b""
         for i in range(maps):
@@ -187,28 +178,15 @@
             else:  # record or array
                 value = self._node.sdo[index][subindex].phys
                 value_bytes = self.od[index][subindex].encode_raw(value)
 
             # pack pdo with bytes
             data += value_bytes
 
-        try:
-            self._network.send_message(cob_id, data)
-        except Exception as e:  # pylint: disable=W0718
-            logger.exception(f"TPDO{tpdo} failed with: {e}")
-
-    def _tpdo_timer_loop(self, tpdo: int) -> bool:
-        """Send TPDO for TPDO loop. Can handle network errors."""
-
-        try:
-            self.send_tpdo(tpdo)
-        except NetworkError:
-            pass
-
-        return True
+        self._network.send_message(cob_id, data, False)
 
     def _on_rpdo_update_od(self, mapping: canopen.pdo.base.Map):
         """Handle parsering an RPDO"""
 
         for i in mapping.map_array:
             if i == 0:
                 continue
@@ -220,166 +198,79 @@
             index, subindex, _ = struct.unpack(">HBB", value.to_bytes(4, "big"))
             if isinstance(self.od[index], canopen.objectdictionary.Variable):
                 self._node.sdo[index].raw = mapping.map[i - 1].get_data()
             else:
                 self._node.sdo[index][subindex].raw = mapping.map[i - 1].get_data()
 
     def _setup_node(self):
-        """Create the CANopen and TPDO timer loops"""
+        """Create the CANopen node."""
 
         if self._od.node_id is None:
             self._od.node_id = 0x7C
 
         self._node = canopen.LocalNode(self._od.node_id, self._od)
+        self._network.add_node(self._node)
+        self._node.nmt.state = "OPERATIONAL"
 
         self._node.add_read_callback(self._on_sdo_read)
         self._node.add_write_callback(self._on_sdo_write)
 
-        for i in range(16):
-            if i + 0x1800 not in self.od:
-                continue
-            transmission_type = self.od[0x1800 + i][2].default
-            event_time = self.od[0x1800 + i][5].default
-            if transmission_type in [0xFE, 0xFF] and event_time > 0:
-                timer = TimerLoop(
-                    name=f"TPDO{i + 1}",
-                    loop_func=self._tpdo_timer_loop,
-                    delay=self.od[0x1800 + i][5],
-                    start_delay=self.od[0x1800 + i][3],
-                    args=(i + 1,),
-                )
-                self._tpdo_timers.append(timer)
-                timer.start()
+        if not self._first_network_reset or monotonic() - self._start_time > 5:
+            self.send_emcy(0x8140)
+        else:
+            self._first_network_reset = False
 
     def _destroy_node(self):
-        """Destroy the CANopen and TPDO timer loops"""
-
-        for timer in self._tpdo_timers:
-            timer.stop()
-
-        self._tpdo_timers = []  # remove all
+        """Destroy the CANopen node."""
 
         self._node = None
 
-    def _restart_bus(self):
-        """Try to restart the CAN bus"""
-
-        if os.path.exists(self._channel):
-            return  # skip. On MacOS, the CAN bus is always up, if it exists
-
-        if self.first_bus_reset:
-            logger.error(f"{self._channel} is down")
-
-        if os.geteuid() == 0:  # running as root
-            if self.first_bus_reset:
-                logger.info(f"trying to restart CAN bus {self._channel}")
-            cmd = (
-                f"ip link set {self._channel} down;"
-                f"ip link set {self._channel} type can bitrate 1000000;"
-                f"ip link set {self._channel} up"
-            )
-            out = subprocess.run(cmd, shell=True, check=False)
-            if out.returncode != 0:
-                logger.error(out)
-
-        self.first_bus_reset = False
-
-    def _restart_network(self):
-        """Restart the CANopen network"""
-
-        logger.info("(re)starting CANopen network")
-
-        self._network = canopen.Network(self._bus)
-        self._network.notifier = can.Notifier(self._network.bus, self._network.listeners, 1)
-        self._setup_node()
-        self._network.add_node(self._node)
-
-        try:
-            self._node.nmt.start_heartbeat(self.od[0x1017].default)
-            self._node.nmt.state = "OPERATIONAL"
-        except Exception as e:  # pylint: disable=W0718
-            logger.exception(f"failed to (re)start CANopen network with {e}")
-
-        self._network.subscribe(0x80, self._on_sync)
-
-        # setup RPDOs callbacks
-        self._node.rpdo.read()
-        for i in self._node.rpdo:
-            if self._node.rpdo[i].enabled:
-                self._node.rpdo[i].add_callback(self._on_rpdo_update_od)
-
-    def _disable_network(self):
-        """Disable the CANopen network"""
-
-        try:
-            if self._network:
-                self._network.disconnect()
-            self._destroy_node()
-        except Exception:  # pylint: disable=W0718
-            self._network = None  # make sure the canopen network is down
-            self._node = None
-
-    def _monitor_can(self):
-        """Monitor the CAN bus and CAN network"""
-
-        first_bus_down = True  # flag to only log error message on first error
-        self.first_bus_reset = True  # flag to only log error message on first error
-        bus_type = self._bus.channel_info.split(" ")[0]
-        if bus_type == "socketcand":
-            self._restart_network()
-            self._bus_state = CanState.BUS_UP_NETWORK_UP
-        while not self._event.is_set():
-            if bus_type == "socketcand":
-                self._event.wait(1)
-                continue
-
-            bus = psutil.net_if_stats().get(self._channel)
-            if bus is None and not os.path.exists(self._channel):  # bus does not exist
-                self._bus_state = CanState.BUS_NOT_FOUND
-                self._disable_network()
-                if first_bus_down:
-                    logger.critical(f"{self._channel} does not exists, nothing OLAF can do")
-                    first_bus_down = False
-            elif (bus and not bus.isup) or os.path.exists(self._channel):  # bus is down
-                self._bus_state = CanState.BUS_DOWN
-                first_bus_down = True  # reset flag
-                self._disable_network()
-                self._restart_bus()
-            elif not self._network:  # bus is up, network is down
-                self._bus_state = CanState.BUS_UP_NETWORK_DOWN
-                first_bus_down = True  # reset flag
-                self._restart_network()
-            else:  # bus is up, network is up
-                self._bus_state = CanState.BUS_UP_NETWORK_UP
-                self.first_bus_reset = True  # reset flag
-                first_bus_down = True  # reset flag
-
-            self._event.wait(1)
-
-    def run(self) -> int:
+    def run(self) -> NodeStop:
         """
         Go into operational mode, start all the resources, start all the threads, and monitor
         everything in a loop.
 
         Returns
         -------
         NodeStop
             Reset / power off condition.
         """
 
         logger.info(f"{self.name} node is starting")
-        if os.geteuid() != 0:  # running as root
-            logger.warning("not running as root, cannot restart CAN bus if it goes down")
 
-        try:
-            self._monitor_can()
-        except Exception as e:  # pylint: disable=W0718
-            logger.exception(e)
+        loops = -1
+        delay_ms = 100
+        delay = delay_ms / 1000
+        start_time = monotonic()
+        while not self._event.is_set():
+            loops += 1
+            self._event.wait(delay - ((monotonic() - start_time) % delay))
+            self._network.monitor()
+
+            if self._network.status != CanNetworkState.NETWORK_UP:
+                continue
+
+            # send heartbeat
+            event_time = self.od[0x1017].value
+            if loops % (event_time // delay_ms) == 0:
+                self._network.send_message(0x700 + self.od.node_id, b"\x05", False)
+
+            # send all timer-based TPDOs
+            for i in range(self._od.device_information.nr_of_TXPDO):
+                if i + 0x1800 not in self.od:
+                    continue
+                transmission_type = self.od[0x1800 + i][2].value
+                event_time = self.od[0x1800 + i][5].value
+                if (
+                    transmission_type in [0xFE, 0xFF]
+                    and event_time != 0
+                    and loops % (event_time // delay_ms) == 0
+                ):
+                    self.send_tpdo(i + 1)
 
-        # stop the node and TPDO timers
         self._destroy_node()
 
         logger.info(f"{self.name} node has ended")
         return self._reset
 
     def stop(self, reset: Union[NodeStop, None] = None):
         """End the run loop"""
@@ -436,38 +327,33 @@
                 return
 
         if read_cb is not None:
             self._read_cbs[index, subindex] = read_cb
         if write_cb is not None:
             self._write_cbs[index, subindex] = write_cb
 
-    def send_emcy(self, code: int, register: int = 0, data: bytes = b""):
+    def send_emcy(self, code: int, data: bytes = b""):
         """
-        Send a EMCY message. Wrapper on canopen's `EmcyProducer.send`.
+        Send a EMCY message.
 
         Parameters
         ----------
         code: int
             The EMCY code.
-        register: int
-            Optional error register value in EMCY message (uint8). See Object 1001 def for bit
-            field.
-        manufacturer_code: bytes
-            Optional manufacturer error code (up to 5 bytes).
-
-        Raises
-        ------
-        NetworkError
-            Cannot send a EMCY message when the network is down.
+        data: bytes
+            Optional manufacturer error code/data (up to 5 bytes).
         """
 
-        if self._network is None:
-            raise NetworkError("network is down cannot send an EMCY message")
+        if len(data) > 5:
+            raise ValueError("data must be 5 or less bytes")
 
-        self._node.emcy.send(code, register, data)
+        frame = code.to_bytes(2, "little") + self.od[0x1001].value.to_bytes(1, "little") + data
+        frame += b"\x00" * (5 - len(data))
+        self._network.send_message(self.od.node_id + 0x80, frame)
+        logger.error(f"sent emcy 0x{code:04X} {data.hex()}")
 
     def _on_sdo_read(self, index: int, subindex: int, od: canopen.objectdictionary.Variable):
         """
         SDO read callback function. Allows overriding the data being sent on a SDO read. Return
         valid datatype for object, if overriding read data, or :py:data:`None` to use the the value
         on object dictionary.
 
@@ -544,21 +430,21 @@
         if (index, subindex) in self._write_cbs:
             self._write_cbs[index, subindex](od.value)
 
     @property
     def bus(self) -> str:
         """str: The CAN bus."""
 
-        return self._channel
+        return self._network.channel
 
     @property
     def bus_state(self) -> str:
         """str: The CAN bus status."""
 
-        return self._bus_state.name
+        return self._network.status.name
 
     @property
     def name(self) -> str:
         """str: The nodes name."""
 
         return self._od.device_information.product_name
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/resources/daemons.py` & `oresat_olaf-3.5.0/olaf/_internals/resources/daemons.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/resources/ecss.py` & `oresat_olaf-3.5.0/olaf/_internals/resources/ecss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Resource for ECSS CANBus Extended Protocal standards"""
 
 from os import geteuid
 from time import CLOCK_REALTIME, clock_settime, time
 
 from loguru import logger
 
-from ...common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
+from ...canopen.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from ...common.resource import Resource
 
 
 class EcssResource(Resource):
     """Resource for ECSS CANBus Extended Protocal standards"""
 
     def on_start(self):
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/resources/fread.py` & `oresat_olaf-3.5.0/olaf/_internals/resources/fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/resources/fwrite.py` & `oresat_olaf-3.5.0/olaf/_internals/resources/fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/resources/system.py` & `oresat_olaf-3.5.0/olaf/_internals/resources/system.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from time import monotonic, time
 
 import psutil
 
 from olaf import logger
 
-from ...common.eeprom import Eeprom
+from ...board.eeprom import Eeprom
+from ...canopen.node import NodeStop
 from ...common.resource import Resource
-from ..node import NodeStop
 
 
 class SystemResource(Resource):
     """Resource for the system."""
 
     def on_start(self):
         self.node.od["system"]["reset"].value = 0
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/__init__.py` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/static/favicon.ico` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/_base.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/_base.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/base.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "_base.html" %}
 
 {% block baseContent %}
   <style>
     #headerGrid {
       display: grid;
-      grid-template-columns: 25% 50% 25%;
+      grid-template-columns: 35% 30% 35%;
     }
     #headerCenter {
       text-align: center;
     }
     #headerRight {
       text-align: right;
     }
@@ -17,15 +17,15 @@
     <div id="headerLeft">
        <a href="/">home</a>
     </div>
     <div id="headerCenter">
       <h2>{{name}}</h2>
     </div>
     <div id="headerRight">
-      <text><b><span id="busChannel">vcan0</span></b>: <span id="busStatus">BUS_DOWN</span> | </text>
+      <text><b><span id="busChannel">vcan0</span></b>: <span id="busStatus">NETWORK_DOWN</span> | </text>
       <label for="flightMode"><b>Flight Mode</b>: </label>
       <input type="checkbox" id="flightMode" onclick="toggleFlightMode()"></input>
     </div>
   </div>
   <div id="content">
     {% block content %}{% endblock %}
   </div>
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/daemons.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/daemons.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/fread.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/fwrite.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/logs.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/od.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/od.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/os_command.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/reset.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/reset.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/root.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/root.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "_base.html" %}
 
 {% block baseContent %}
   <style>
     #headerGrid {
       display: grid;
-      grid-template-columns: 25% 50% 25%;
+      grid-template-columns: 35% 30% 35%;
     }
     #headerCenter {
       text-align: center;
     }
     #headerRight {
       text-align: right;
     }
```

### Comparing `oresat-olaf-3.4.0/olaf/_internals/rest_api/templates/updater.html` & `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/services/logs.py` & `oresat_olaf-3.5.0/olaf/_internals/services/logs.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/services/os_command.py` & `oresat_olaf-3.5.0/olaf/_internals/services/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/services/updater.py` & `oresat_olaf-3.5.0/olaf/_internals/services/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/_internals/updater.py` & `oresat_olaf-3.5.0/olaf/_internals/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/adc.py` & `oresat_olaf-3.5.0/olaf/board/adc.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/cpufreq.py` & `oresat_olaf-3.5.0/olaf/board/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/daemon.py` & `oresat_olaf-3.5.0/olaf/common/daemon.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/ecss.py` & `oresat_olaf-3.5.0/olaf/canopen/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/eeprom.py` & `oresat_olaf-3.5.0/olaf/board/eeprom.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/gpio.py` & `oresat_olaf-3.5.0/olaf/board/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/oresat_file.py` & `oresat_olaf-3.5.0/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/oresat_file_cache.py` & `oresat_olaf-3.5.0/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/pru.py` & `oresat_olaf-3.5.0/olaf/board/pru.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/olaf/common/resource.py` & `oresat_olaf-3.5.0/olaf/common/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The OreSat Linux base app resource. It is a nice way to organize OD callbacks."""
 
 from loguru import logger
 
-from .._internals.node import Node
+from ..canopen.node import Node
 
 
 class Resource:
     """
     OreSat Linux app resource. Used to setup OD callbacks in a common, isolated environment.
 
     All the ``on_*`` members can be overridden as needed.
```

### Comparing `oresat-olaf-3.4.0/olaf/common/service.py` & `oresat_olaf-3.5.0/olaf/common/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The OLAF base Service class. A Resource with a dedicated thread."""
 
 from enum import IntEnum
 from threading import Event, Thread
 
 from loguru import logger
 
-from .._internals.node import Node
+from ..canopen.node import Node
 
 
 class ServiceState(IntEnum):
     """State a service can be in."""
 
     STOPPED = 0
     """Service is not running."""
```

### Comparing `oresat-olaf-3.4.0/olaf/common/timer_loop.py` & `oresat_olaf-3.5.0/olaf/common/timer_loop.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/oresat_olaf.egg-info/PKG-INFO` & `oresat_olaf-3.5.0/oresat_olaf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.4.0
+Version: 3.5.0
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: flask
 Requires-Dist: loguru
 Requires-Dist: natsort
 Requires-Dist: psutil
+Requires-Dist: python-can>=4.3.0
 Requires-Dist: oresat-configs
 
 OLAF (OreSat Linux App Framework)
 =================================
 
 .. image:: https://img.shields.io/github/license/oresat/oresat-olaf
    :target: https://github.com/oresat/oresat-olaf/blob/master/LICENSE
```

### Comparing `oresat-olaf-3.4.0/oresat_olaf.egg-info/SOURCES.txt` & `oresat_olaf-3.5.0/oresat_olaf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 docs/api/updater.rst
 docs/updater/index.rst
 docs/updater/update_archive.rst
 olaf/__init__.py
 olaf/_version.py
 olaf/_internals/__init__.py
 olaf/_internals/app.py
-olaf/_internals/master_node.py
-olaf/_internals/node.py
 olaf/_internals/updater.py
 olaf/_internals/resources/__init__.py
 olaf/_internals/resources/daemons.py
 olaf/_internals/resources/ecss.py
 olaf/_internals/resources/fread.py
 olaf/_internals/resources/fwrite.py
 olaf/_internals/resources/system.py
@@ -57,24 +55,28 @@
 olaf/_internals/rest_api/templates/reset.html
 olaf/_internals/rest_api/templates/root.html
 olaf/_internals/rest_api/templates/updater.html
 olaf/_internals/services/__init__.py
 olaf/_internals/services/logs.py
 olaf/_internals/services/os_command.py
 olaf/_internals/services/updater.py
+olaf/board/adc.py
+olaf/board/cpufreq.py
+olaf/board/eeprom.py
+olaf/board/gpio.py
+olaf/board/pru.py
+olaf/canopen/__init__.py
+olaf/canopen/ecss.py
+olaf/canopen/master_node.py
+olaf/canopen/network.py
+olaf/canopen/node.py
 olaf/common/__init__.py
-olaf/common/adc.py
-olaf/common/cpufreq.py
 olaf/common/daemon.py
-olaf/common/ecss.py
-olaf/common/eeprom.py
-olaf/common/gpio.py
 olaf/common/oresat_file.py
 olaf/common/oresat_file_cache.py
-olaf/common/pru.py
 olaf/common/resource.py
 olaf/common/service.py
 olaf/common/timer_loop.py
 oresat_olaf.egg-info/PKG-INFO
 oresat_olaf.egg-info/SOURCES.txt
 oresat_olaf.egg-info/dependency_links.txt
 oresat_olaf.egg-info/requires.txt
```

### Comparing `oresat-olaf-3.4.0/pyproject.toml` & `oresat_olaf-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ]
 dependencies = [
     "canopen",
     "flask",
     "loguru",
     "natsort",
     "psutil",
+    "python-can>=4.3.0",
     "oresat-configs",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
```

### Comparing `oresat-olaf-3.4.0/tests/common/test_ecss.py` & `oresat_olaf-3.5.0/tests/common/test_ecss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test the ECSS functions."""
 
 import unittest
 from time import time
 
-from olaf.common.ecss import (
+from olaf.canopen.ecss import (
     scet_int_from_time,
     scet_int_to_time,
     utc_int_from_time,
     utc_int_to_time,
 )
```

### Comparing `oresat-olaf-3.4.0/tests/common/test_oresat_file.py` & `oresat_olaf-3.5.0/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/common/test_oresat_file_cache.py` & `oresat_olaf-3.5.0/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/common/test_pru.py` & `oresat_olaf-3.5.0/tests/common/test_pru.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test the PRU class."""
 
 import unittest
 from os.path import isdir
 
-from olaf.common.pru import Pru, PruError, PruState
+from olaf.board.pru import Pru, PruError, PruState
 
 PRU_EXIST = isdir("/dev/remoteproc/pruss-core0") and isdir("/dev/remoteproc/pruss-core1")
 
 
 class TestPru(unittest.TestCase):
     """Test the PRU class."""
```

### Comparing `oresat-olaf-3.4.0/tests/common/test_resources.py` & `oresat_olaf-3.5.0/tests/common/test_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test the Resource class."""
 
 import unittest
 
-import can
 from oresat_configs import OreSatConfig, OreSatId
 
-from olaf import Node, Resource
+from olaf import CanNetwork, Node, Resource
 
 
 class BadResource(Resource):
     """Bad Resource for testing."""
 
     def on_start(self):
         raise Exception("a random exception")  # pylint: disable=W0719
@@ -21,16 +20,16 @@
 class TestResource(unittest.TestCase):
     """Test the Resource class."""
 
     def test_start_stop(self):
         """All exception should be caught"""
 
         od = OreSatConfig(OreSatId.ORESAT0).od_db["gps"]
-        bus = can.interface.Bus(interface="virtual", channel="vcan0")
-        node = Node(od, bus)
+        network = CanNetwork("virtual", "vcan0")
+        node = Node(network, od)
 
         good_res = Resource()
         bad_res = BadResource()
 
         good_res.start(node)
         bad_res.start(node)
```

### Comparing `oresat-olaf-3.4.0/tests/internals/resources/__init__.py` & `oresat_olaf-3.5.0/tests/internals/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Tests for Resources."""
 
-import can
 import canopen
 from oresat_configs import OreSatConfig, OreSatId
 
 from olaf import OreSatFileCache, Resource, logger
-from olaf._internals.node import Node
+from olaf.canopen.network import CanNetwork
+from olaf.canopen.node import Node
 
 logger.disable("olaf")
 
 
 class MockNode(Node):
     """Mock node for testing Resources."""
 
     def __init__(self):
         od = OreSatConfig(OreSatId.ORESAT0).od_db["gps"]
-        bus = can.interface.Bus(interface="virtual", channel="vcan0")
-        super().__init__(od, bus)
+        network = CanNetwork("virtual", "vcan0")
+        super().__init__(network, od)
 
         self._fread_cache = OreSatFileCache("/tmp/fread")
         self._fread_cache.clear()
         self._fwrite_cache = OreSatFileCache("/tmp/fwrite")
         self._fwrite_cache.clear()
 
         self._setup_node()
```

### Comparing `oresat-olaf-3.4.0/tests/internals/resources/test_ecss.py` & `oresat_olaf-3.5.0/tests/internals/resources/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/resources/test_fread.py` & `oresat_olaf-3.5.0/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/resources/test_fwrite.py` & `oresat_olaf-3.5.0/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/services/__init__.py` & `oresat_olaf-3.5.0/tests/internals/services/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Mock node for testing services."""
 
-import can
 import canopen
 from oresat_configs import OreSatConfig, OreSatId
 
 from olaf import OreSatFileCache, Service, logger
-from olaf._internals.node import Node
+from olaf.canopen.network import CanNetwork
+from olaf.canopen.node import Node
 
 logger.disable("olaf")
 
 
 class MockNode(Node):
     """Mock node for testing services."""
 
     def __init__(self):
         od = OreSatConfig(OreSatId.ORESAT0).od_db["gps"]
-        bus = can.interface.Bus(interface="virtual", channel="vcan0")
-        super().__init__(od, bus)
+        network = CanNetwork("virtual", "vcan0")
+        super().__init__(network, od)
 
         self._fread_cache = OreSatFileCache("/tmp/fread")
         self._fread_cache.clear()
         self._fwrite_cache = OreSatFileCache("/tmp/fwrite")
         self._fwrite_cache.clear()
 
         self._setup_node()
```

### Comparing `oresat-olaf-3.4.0/tests/internals/services/test_os_command.py` & `oresat_olaf-3.5.0/tests/internals/services/test_os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/test_rest_api.py` & `oresat_olaf-3.5.0/tests/internals/test_rest_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Test the REST API."""
 
 import unittest
 
-import can
 from oresat_configs import OreSatConfig, OreSatId
 
-from olaf import app, rest_api
+from olaf import CanNetwork, app, rest_api
 
 
 class TestRestApi(unittest.TestCase):
     """Test the REST API."""
 
     @classmethod
     def setUpClass(cls):
         # Setup OLAF for unit testing.
         config = OreSatConfig(OreSatId.ORESAT0_5)
         od = config.od_db["gps"]
-        bus = can.interface.Bus(interface="virtual", channel="vcan0")
-        app.setup(od, bus, None, False)
+        network = CanNetwork("virtual", "vcan0")
+        app.setup(network, od, None, False)
         rest_api.setup(address="localhost", port=8000)
 
         cls.client = rest_api.app.test_client()
 
         app.node._setup_node()
 
         for i in app._resources:
```

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/README.md` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/README.md`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz` & `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat-olaf-3.4.0/tests/internals/updater/test_updater.py` & `oresat_olaf-3.5.0/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

