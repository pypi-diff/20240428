# Comparing `tmp/pytest-xdist-3.5.0.tar.gz` & `tmp/pytest_xdist-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-xdist-3.5.0.tar", last modified: Tue Nov 21 14:38:45 2023, max compression
+gzip compressed data, was "pytest_xdist-3.6.0.tar", last modified: Fri Apr 19 19:45:29 2024, max compression
```

## Comparing `pytest-xdist-3.5.0.tar` & `pytest_xdist-3.6.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.306871 pytest-xdist-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34413 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2023-11-21 14:38:45.306871 pytest-xdist-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.294871 pytest-xdist-3.5.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/changelog/_template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.298871 pytest-xdist-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/crash.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/distribution.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/how-it-works.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/how-to.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/known-limitations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/remote.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/docs/subprocess.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.298871 pytest-xdist-3.5.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/boxed.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.298871 pytest-xdist-3.5.0/example/loadscope/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.298871 pytest-xdist-3.5.0/example/loadscope/epsilon/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/epsilon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.298871 pytest-xdist-3.5.0/example/loadscope/test/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/test/test_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/test/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/test/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/test/test_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/example/loadscope/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-11-21 14:38:45.306871 pytest-xdist-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.290871 pytest-xdist-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.302871 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/pytest_xdist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.302871 pytest-xdist-3.5.0/src/xdist/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-21 14:38:45.000000 pytest-xdist-3.5.0/src/xdist/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/dsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/looponfail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/newhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11561 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.302871 pytest-xdist-3.5.0/src/xdist/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/each.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/loadfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/loadgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14493 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/loadscope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/scheduler/worksteal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16552 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/src/xdist/workermanage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:38:45.302871 pytest-xdist-3.5.0/testing/
--rw-r--r--   0 runner    (1001) docker     (127)    53118 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/acceptance_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21498 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_dsession.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_looponfail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_newhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/test_workermanage.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-11-21 14:38:24.000000 pytest-xdist-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    36774 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.638512 pytest_xdist-3.6.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.638512 pytest_xdist-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/crash.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/how-it-works.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/how-to.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/known-limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/remote.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/docs/subprocess.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.638512 pytest_xdist-3.6.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/boxed.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.638512 pytest_xdist-3.6.0/example/loadscope/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.638512 pytest_xdist-3.6.0/example/loadscope/epsilon/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/epsilon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.642512 pytest_xdist-3.6.0/example/loadscope/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/test/test_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/test/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/test/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/test/test_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/example/loadscope/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.634513 pytest_xdist-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/pytest_xdist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.642512 pytest_xdist-3.6.0/src/xdist/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 19:45:29.000000 pytest_xdist-3.6.0/src/xdist/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22718 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/dsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12518 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/src/xdist/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/each.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/loadfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/loadgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/loadscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/scheduler/worksteal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17911 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/src/xdist/workermanage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:45:29.646512 pytest_xdist-3.6.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)    54027 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/acceptance_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22850 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_dsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14814 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/test_workermanage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 19:45:23.000000 pytest_xdist-3.6.0/tox.ini
```

### Comparing `pytest-xdist-3.5.0/CHANGELOG.rst` & `pytest_xdist-3.6.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,51 @@
+pytest-xdist 3.6.0 (2024-04-19)
+===============================
+
+Features
+--------
+
+- `#1027 <https://github.com/pytest-dev/pytest-xdist/pull/1027>`_:``pytest-xdist`` workers now always execute the tests in the main thread.
+  Previously some tests might end up executing in a separate thread other than ``main`` in the workers, due to some internal `execnet`` details. This can cause problems specially with async frameworks where the event loop is running in the ``main`` thread (for example `#620 <https://github.com/pytest-dev/pytest-xdist/issues/620>`__).
+
+Bug Fixes
+---------
+
+- `#1024 <https://github.com/pytest-dev/pytest-xdist/issues/1024>`_: Added proper handling of ``shouldstop`` (such as set by ``--max-fail``) and ``shouldfail`` conditions in workers.
+  Previously, a worker might have continued executing further tests before the controller could terminate the session.
+
+- `#1028 <https://github.com/pytest-dev/pytest-xdist/issues/1028>`_: Fixed compatibility issue between `looponfail` and editable installs.
+
+- `#620 <https://github.com/pytest-dev/pytest-xdist/issues/620>`_: Use the new ``main_thread_only`` ``execnet`` "execmodel" so that code which expects to only run in the main thread will now work as expected.
+
+- `#937 <https://github.com/pytest-dev/pytest-xdist/issues/937>`_: Fixed a bug where plugin would raise an incompatibility error with ``--pdb`` despite using ``-n0``.
+
+
+Removals
+--------
+
+- `#1053 <https://github.com/pytest-dev/pytest-xdist/issues/1053>`_: Dropped support for Python 3.7.
+
+- `#1057 <https://github.com/pytest-dev/pytest-xdist/issues/1057>`_: pytest>=7.0.0 is now required.
+
+  execnet>=2.1.0 is now required.
+
+
+Trivial Changes
+---------------
+
+- `#1020 <https://github.com/pytest-dev/pytest-xdist/issues/1020>`_: pytest-xdist's ``setup.py`` file is removed.
+
+  If you relied on this file, e.g. to install pytest using ``setup.py install``,
+  please see `Why you shouldn't invoke setup.py directly <https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html#summary>`_ for alternatives.
+
+- `#1057 <https://github.com/pytest-dev/pytest-xdist/issues/1057>`_: The internals of pytest-xdist are now fully typed. The typing is not exposed yet.
+
+- `#996 <https://github.com/pytest-dev/pytest-xdist/issues/996>`_: Adjusted license file format and content to ensure security scanners will identity the license.
+
 pytest-xdist 3.5.0 (2023-11-21)
 ===============================
 
 Features
 --------
 
 - `#632 <https://github.com/pytest-dev/pytest-xdist/issues/632>`_: ``--dist=loadscope`` now sorts scopes by number of tests to assign largest scopes early -- in many cases this should improve overall test session running time, as there is less chance of a large scope being left to be processed near the end of the session, leaving other workers idle.
```

### Comparing `pytest-xdist-3.5.0/LICENSE` & `pytest_xdist-3.6.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+MIT License
 
-  Permission is hereby granted, free of charge, to any person obtaining a copy
-  of this software and associated documentation files (the "Software"), to deal
-  in the Software without restriction, including without limitation the rights
-  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-  copies of the Software, and to permit persons to whom the Software is
-  furnished to do so, subject to the following conditions:
+Copyright (c) 2010 Holger Krekel and contributors.
 
-  The above copyright notice and this permission notice shall be included in all
-  copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-  SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pytest-xdist-3.5.0/README.rst` & `pytest_xdist-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/RELEASING.rst` & `pytest_xdist-3.6.0/RELEASING.rst`

 * *Files 18% similar despite different names*

```diff
@@ -30,10 +30,12 @@
 
 #. Update the necessary files with::
 
     $ tox -e release -- X.Y.Z
 
 #. Commit and push the branch to ``upstream`` and open a PR.
 
-#. Once the PR is **green** and **approved**, start the ``deploy`` workflow manually from the branch ``release-VERSION``, passing ``VERSION`` as parameter.
+#. Once the PR is **green** and **approved**, start the ``deploy`` workflow manually from the branch ``release-VERSION``, passing ``VERSION`` as parameter, or execute::
+
+   gh workflow run deploy.yml -R pytest-dev/pytest-xdist --ref release-X.Y.Z --field version=X.Y.Z
 
 #. Merge the release PR to ``master``.
```

### Comparing `pytest-xdist-3.5.0/changelog/_template.rst` & `pytest_xdist-3.6.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/docs/conf.py` & `pytest_xdist-3.6.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "pytest-xdist"
-copyright = "2022, holger krekel and contributors"
+copyright = "2010, holger krekel and contributors"
 author = "holger krekel and contributors"
 
 master_doc = "index"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `pytest-xdist-3.5.0/docs/distribution.rst` & `pytest_xdist-3.6.0/docs/distribution.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
     pytest -n auto
 
 This can lead to considerable speed ups, especially if your test suite takes a
 noticeable amount of time.
 
 With ``-n auto``, pytest-xdist will use as many processes as your computer
-has CPU cores.
+has physical CPU cores.
 
 Use ``-n logical`` to use the number of *logical* CPU cores rather than
-physical ones. This currently requires the ``psutil`` package to be installed;
-if it is not, pytest-xdist will fall back to ``-n auto`` behavior.
+physical ones. This currently requires the `psutil <https://pypi.org/project/psutil/>`__ package to be installed;
+if it is not or if it fails to determine the number of logical CPUs, fall back to ``-n auto`` behavior.
 
 Pass a number, e.g. ``-n 8``, to specify the number of processes explicitly.
 
 To specify a different meaning for ``-n auto`` and ``-n logical`` for your
 tests, you can:
 
 * Set the environment variable ``PYTEST_XDIST_AUTO_NUM_WORKERS`` to the
```

### Comparing `pytest-xdist-3.5.0/docs/how-it-works.rst` & `pytest_xdist-3.6.0/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/docs/how-to.rst` & `pytest_xdist-3.6.0/docs/how-to.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/docs/index.rst` & `pytest_xdist-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/docs/known-limitations.rst` & `pytest_xdist-3.6.0/docs/known-limitations.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/docs/remote.rst` & `pytest_xdist-3.6.0/docs/remote.rst`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
 platforms - and report back failures from all platforms
 at once. The specifications strings use the `xspec syntax`_.
 
 .. _`xspec syntax`: https://codespeak.net/execnet/basics.html#xspec
 
 .. _`execnet`: https://codespeak.net/execnet
 
-.. _`socketserver.py`: https://raw.githubusercontent.com/pytest-dev/execnet/master/execnet/script/socketserver.py
+.. _`socketserver.py`: https://raw.githubusercontent.com/pytest-dev/execnet/master/src/execnet/script/socketserver.py
```

### Comparing `pytest-xdist-3.5.0/docs/subprocess.rst` & `pytest_xdist-3.6.0/docs/subprocess.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/example/boxed.txt` & `pytest_xdist-3.6.0/example/boxed.txt`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/example/loadscope/test/test_alpha.py` & `pytest_xdist-3.6.0/example/loadscope/test/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/example/loadscope/test/test_beta.py` & `pytest_xdist-3.6.0/example/loadscope/test/test_beta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/example/loadscope/test/test_delta.py` & `pytest_xdist-3.6.0/example/loadscope/test/test_delta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/example/loadscope/test/test_gamma.py` & `pytest_xdist-3.6.0/example/loadscope/test/test_gamma.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.5.0/src/pytest_xdist.egg-info/SOURCES.txt` & `pytest_xdist-3.6.0/src/pytest_xdist.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .readthedocs.yaml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 RELEASING.rst
 pyproject.toml
-setup.cfg
 tox.ini
 changelog/_template.rst
 docs/.gitignore
 docs/changelog.rst
 docs/conf.py
 docs/crash.rst
 docs/distribution.rst
@@ -47,14 +46,15 @@
 src/xdist/workermanage.py
 src/xdist/scheduler/__init__.py
 src/xdist/scheduler/each.py
 src/xdist/scheduler/load.py
 src/xdist/scheduler/loadfile.py
 src/xdist/scheduler/loadgroup.py
 src/xdist/scheduler/loadscope.py
+src/xdist/scheduler/protocol.py
 src/xdist/scheduler/worksteal.py
 testing/acceptance_test.py
 testing/conftest.py
 testing/test_dsession.py
 testing/test_looponfail.py
 testing/test_newhooks.py
 testing/test_plugin.py
```

### Comparing `pytest-xdist-3.5.0/src/xdist/_path.py` & `pytest_xdist-3.6.0/src/xdist/_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import os
 from itertools import chain
+import os
 from pathlib import Path
-from typing import Callable, Iterator
+from typing import Callable
+from typing import Iterator
 
 
 def visit_path(
     path: Path, *, filter: Callable[[Path], bool], recurse: Callable[[Path], bool]
 ) -> Iterator[Path]:
     """
     Implements the interface of ``py.path.local.visit()`` for Path objects,
```

### Comparing `pytest-xdist-3.5.0/src/xdist/dsession.py` & `pytest_xdist-3.6.0/src/xdist/dsession.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,121 +1,136 @@
 from __future__ import annotations
+
+from enum import auto
+from enum import Enum
+from queue import Empty
+from queue import Queue
 import sys
-from enum import Enum, auto
+from typing import Any
 from typing import Sequence
+import warnings
 
+import execnet
 import pytest
 
 from xdist.remote import Producer
+from xdist.remote import WorkerInfo
+from xdist.scheduler import EachScheduling
+from xdist.scheduler import LoadFileScheduling
+from xdist.scheduler import LoadGroupScheduling
+from xdist.scheduler import LoadScheduling
+from xdist.scheduler import LoadScopeScheduling
+from xdist.scheduler import Scheduling
+from xdist.scheduler import WorkStealingScheduling
 from xdist.workermanage import NodeManager
-from xdist.scheduler import (
-    EachScheduling,
-    LoadScheduling,
-    LoadScopeScheduling,
-    LoadFileScheduling,
-    LoadGroupScheduling,
-    WorkStealingScheduling,
-)
-
-
-from queue import Empty, Queue
+from xdist.workermanage import WorkerController
 
 
 class Interrupted(KeyboardInterrupt):
     """signals an immediate interruption."""
 
 
 class DSession:
-    """A pytest plugin which runs a distributed test session
+    """A pytest plugin which runs a distributed test session.
 
     At the beginning of the test session this creates a NodeManager
     instance which creates and starts all nodes.  Nodes then emit
     events processed in the pytest_runtestloop hook using the worker_*
     methods.
 
     Once a node is started it will automatically start running the
     pytest mainloop with some custom hooks.  This means a node
     automatically starts collecting tests.  Once tests are collected
     it will wait for instructions.
     """
 
-    def __init__(self, config):
+    shouldstop: bool | str
+
+    def __init__(self, config: pytest.Config) -> None:
         self.config = config
         self.log = Producer("dsession", enabled=config.option.debug)
-        self.nodemanager = None
-        self.sched = None
+        self.nodemanager: NodeManager | None = None
+        self.sched: Scheduling | None = None
         self.shuttingdown = False
         self.countfailures = 0
-        self.maxfail = config.getvalue("maxfail")
-        self.queue = Queue()
-        self._session = None
-        self._failed_collection_errors = {}
-        self._active_nodes = set()
+        self.maxfail: int = config.getvalue("maxfail")
+        self.queue: Queue[tuple[str, dict[str, Any]]] = Queue()
+        self._session: pytest.Session | None = None
+        self._failed_collection_errors: dict[object, bool] = {}
+        self._active_nodes: set[WorkerController] = set()
         self._failed_nodes_count = 0
         self._max_worker_restart = get_default_max_worker_restart(self.config)
         # summary message to print at the end of the session
-        self._summary_report = None
+        self._summary_report: str | None = None
         self.terminal = config.pluginmanager.getplugin("terminalreporter")
         if self.terminal:
             self.trdist = TerminalDistReporter(config)
             config.pluginmanager.register(self.trdist, "terminaldistreporter")
 
     @property
-    def session_finished(self):
-        """Return True if the distributed session has finished
+    def session_finished(self) -> bool:
+        """Return True if the distributed session has finished.
 
         This means all nodes have executed all test items.  This is
         used by pytest_runtestloop to break out of its loop.
         """
         return bool(self.shuttingdown and not self._active_nodes)
 
-    def report_line(self, line):
+    def report_line(self, line: str) -> None:
         if self.terminal and self.config.option.verbose >= 0:
             self.terminal.write_line(line)
 
     @pytest.hookimpl(trylast=True)
-    def pytest_sessionstart(self, session):
+    def pytest_sessionstart(self, session: pytest.Session) -> None:
         """Creates and starts the nodes.
 
         The nodes are setup to put their events onto self.queue.  As
         soon as nodes start they will emit the worker_workerready event.
         """
         self.nodemanager = NodeManager(self.config)
         nodes = self.nodemanager.setup_nodes(putevent=self.queue.put)
         self._active_nodes.update(nodes)
         self._session = session
 
     @pytest.hookimpl
-    def pytest_sessionfinish(self, session):
+    def pytest_sessionfinish(self) -> None:
         """Shutdown all nodes."""
         nm = getattr(self, "nodemanager", None)  # if not fully initialized
         if nm is not None:
             nm.teardown_nodes()
         self._session = None
 
     @pytest.hookimpl
-    def pytest_collection(self):
+    def pytest_collection(self) -> bool:
         # prohibit collection of test items in controller process
         return True
 
     @pytest.hookimpl(trylast=True)
-    def pytest_xdist_make_scheduler(self, config, log):
+    def pytest_xdist_make_scheduler(
+        self,
+        config: pytest.Config,
+        log: Producer,
+    ) -> Scheduling | None:
         dist = config.getvalue("dist")
-        schedulers = {
-            "each": EachScheduling,
-            "load": LoadScheduling,
-            "loadscope": LoadScopeScheduling,
-            "loadfile": LoadFileScheduling,
-            "loadgroup": LoadGroupScheduling,
-            "worksteal": WorkStealingScheduling,
-        }
-        return schedulers[dist](config, log)
+        if dist == "each":
+            return EachScheduling(config, log)
+        if dist == "load":
+            return LoadScheduling(config, log)
+        if dist == "loadscope":
+            return LoadScopeScheduling(config, log)
+        if dist == "loadfile":
+            return LoadFileScheduling(config, log)
+        if dist == "loadgroup":
+            return LoadGroupScheduling(config, log)
+        if dist == "worksteal":
+            return WorkStealingScheduling(config, log)
+        return None
 
     @pytest.hookimpl
-    def pytest_runtestloop(self):
+    def pytest_runtestloop(self) -> bool:
         self.sched = self.config.hook.pytest_xdist_make_scheduler(
             config=self.config, log=self.log
         )
         assert self.sched is not None
 
         self.shouldstop = False
         pending_exception = None
@@ -124,15 +139,15 @@
             if self.shouldstop:
                 self.triggershutdown()
                 pending_exception = Interrupted(str(self.shouldstop))
         if pending_exception:
             raise pending_exception
         return True
 
-    def loop_once(self):
+    def loop_once(self) -> None:
         """Process one callback from one of the workers."""
         while 1:
             if not self._active_nodes:
                 # If everything has died stop looping
                 self.triggershutdown()
                 raise RuntimeError("Unexpectedly no active workers available")
             try:
@@ -142,76 +157,92 @@
                 continue
         callname, kwargs = eventcall
         assert callname, kwargs
         method = "worker_" + callname
         call = getattr(self, method)
         self.log("calling method", method, kwargs)
         call(**kwargs)
+        assert self.sched is not None
         if self.sched.tests_finished:
             self.triggershutdown()
 
     #
     # callbacks for processing events from workers
     #
 
-    def worker_workerready(self, node, workerinfo):
+    def worker_workerready(
+        self,
+        node: WorkerController,
+        workerinfo: WorkerInfo,
+    ) -> None:
         """Emitted when a node first starts up.
 
         This adds the node to the scheduler, nodes continue with
         collection without any further input.
         """
         node.workerinfo = workerinfo
         node.workerinfo["id"] = node.gateway.id
         node.workerinfo["spec"] = node.gateway.spec
 
         self.config.hook.pytest_testnodeready(node=node)
         if self.shuttingdown:
             node.shutdown()
         else:
+            assert self.sched is not None
             self.sched.add_node(node)
 
-    def worker_workerfinished(self, node):
+    def worker_workerfinished(self, node: WorkerController) -> None:
         """Emitted when node executes its pytest_sessionfinish hook.
 
         Removes the node from the scheduler.
 
         The node might not be in the scheduler if it had not emitted
         workerready before shutdown was triggered.
         """
         self.config.hook.pytest_testnodedown(node=node, error=None)
         if node.workeroutput["exitstatus"] == 2:  # keyboard-interrupt
             self.shouldstop = f"{node} received keyboard-interrupt"
             self.worker_errordown(node, "keyboard-interrupt")
             return
-        if node in self.sched.nodes:
-            crashitem = self.sched.remove_node(node)
-            assert not crashitem, (crashitem, node)
+        shouldfail = node.workeroutput["shouldfail"]
+        shouldstop = node.workeroutput["shouldstop"]
+        for shouldx in [shouldfail, shouldstop]:
+            if shouldx:
+                if not self.shouldstop:
+                    self.shouldstop = shouldx
+                break
+        else:
+            assert self.sched is not None
+            if node in self.sched.nodes:
+                crashitem = self.sched.remove_node(node)
+                assert not crashitem, (crashitem, node)
         self._active_nodes.remove(node)
 
-    def worker_internal_error(self, node, formatted_error):
+    def worker_internal_error(
+        self, node: WorkerController, formatted_error: str
+    ) -> None:
         """
         pytest_internalerror() was called on the worker.
 
         pytest_internalerror() arguments are an excinfo and an excrepr, which can't
         be serialized, so we go with a poor man's solution of raising an exception
         here ourselves using the formatted message.
         """
         self._active_nodes.remove(node)
         try:
             assert False, formatted_error
         except AssertionError:
-            from _pytest._code import ExceptionInfo
-
-            excinfo = ExceptionInfo.from_current()
+            excinfo = pytest.ExceptionInfo.from_current()
             excrepr = excinfo.getrepr()
             self.config.hook.pytest_internalerror(excrepr=excrepr, excinfo=excinfo)
 
-    def worker_errordown(self, node, error):
+    def worker_errordown(self, node: WorkerController, error: object | None) -> None:
         """Emitted by the WorkerController when a node dies."""
         self.config.hook.pytest_testnodedown(node=node, error=error)
+        assert self.sched is not None
         try:
             crashitem = self.sched.remove_node(node)
         except KeyError:
             pass
         else:
             if crashitem:
                 self.handle_crashitem(crashitem, node)
@@ -219,48 +250,50 @@
         self._failed_nodes_count += 1
         maximum_reached = (
             self._max_worker_restart is not None
             and self._failed_nodes_count > self._max_worker_restart
         )
         if maximum_reached:
             if self._max_worker_restart == 0:
-                msg = "worker {} crashed and worker restarting disabled".format(
-                    node.gateway.id
-                )
+                msg = f"worker {node.gateway.id} crashed and worker restarting disabled"
             else:
-                msg = "maximum crashed workers reached: %d" % self._max_worker_restart
+                msg = f"maximum crashed workers reached: {self._max_worker_restart}"
             self._summary_report = msg
             self.report_line("\n" + msg)
             self.triggershutdown()
         else:
             self.report_line("\nreplacing crashed worker %s" % node.gateway.id)
             self.shuttingdown = False
             self._clone_node(node)
         self._active_nodes.remove(node)
 
     @pytest.hookimpl
-    def pytest_terminal_summary(self, terminalreporter):
+    def pytest_terminal_summary(self, terminalreporter: Any) -> None:
         if self.config.option.verbose >= 0 and self._summary_report:
             terminalreporter.write_sep("=", f"xdist: {self._summary_report}")
 
-    def worker_collectionfinish(self, node, ids):
-        """worker has finished test collection.
+    def worker_collectionfinish(
+        self, node: WorkerController, ids: Sequence[str]
+    ) -> None:
+        """Worker has finished test collection.
 
         This adds the collection for this node to the scheduler.  If
         the scheduler indicates collection is finished (i.e. all
         initial nodes have submitted their collections), then tells the
         scheduler to schedule the collected items.  When initiating
         scheduling the first time it logs which scheduler is in use.
         """
         if self.shuttingdown:
             return
         self.config.hook.pytest_xdist_node_collection_finished(node=node, ids=ids)
         # tell session which items were effectively collected otherwise
         # the controller node will finish the session with EXIT_NOTESTSCOLLECTED
+        assert self._session is not None
         self._session.testscollected = len(ids)
+        assert self.sched is not None
         self.sched.add_node_collection(node, ids)
         if self.terminal:
             self.trdist.setstatus(
                 node.gateway.spec, WorkerStatus.CollectionDone, tests_collected=len(ids)
             )
         if self.sched.collection_is_completed:
             if self.terminal and not self.sched.has_pending:
@@ -268,120 +301,152 @@
                 self.terminal.write_line("")
                 if self.config.option.verbose > 0:
                     self.terminal.write_line(
                         f"scheduling tests via {self.sched.__class__.__name__}"
                     )
             self.sched.schedule()
 
-    def worker_logstart(self, node, nodeid, location):
+    def worker_logstart(
+        self,
+        node: WorkerController,
+        nodeid: str,
+        location: tuple[str, int | None, str],
+    ) -> None:
         """Emitted when a node calls the pytest_runtest_logstart hook."""
         self.config.hook.pytest_runtest_logstart(nodeid=nodeid, location=location)
 
-    def worker_logfinish(self, node, nodeid, location):
+    def worker_logfinish(
+        self,
+        node: WorkerController,
+        nodeid: str,
+        location: tuple[str, int | None, str],
+    ) -> None:
         """Emitted when a node calls the pytest_runtest_logfinish hook."""
         self.config.hook.pytest_runtest_logfinish(nodeid=nodeid, location=location)
 
-    def worker_testreport(self, node, rep):
+    def worker_testreport(self, node: WorkerController, rep: pytest.TestReport) -> None:
         """Emitted when a node calls the pytest_runtest_logreport hook."""
-        rep.node = node
+        rep.node = node  # type: ignore[attr-defined]
         self.config.hook.pytest_runtest_logreport(report=rep)
         self._handlefailures(rep)
 
-    def worker_runtest_protocol_complete(self, node, item_index, duration):
+    def worker_runtest_protocol_complete(
+        self, node: WorkerController, item_index: int, duration: float
+    ) -> None:
         """
         Emitted when a node fires the 'runtest_protocol_complete' event,
         signalling that a test has completed the runtestprotocol and should be
         removed from the pending list in the scheduler.
         """
+        assert self.sched is not None
         self.sched.mark_test_complete(node, item_index, duration)
 
-    def worker_unscheduled(self, node, indices):
+    def worker_unscheduled(
+        self, node: WorkerController, indices: Sequence[int]
+    ) -> None:
         """
         Emitted when a node fires the 'unscheduled' event, signalling that
         some tests have been removed from the worker's queue and should be
         sent to some worker again.
 
         This should happen only in response to 'steal' command, so schedulers
         not using 'steal' command don't have to implement it.
         """
+        assert self.sched is not None
         self.sched.remove_pending_tests_from_node(node, indices)
 
-    def worker_collectreport(self, node, rep):
+    def worker_collectreport(
+        self,
+        node: WorkerController,
+        rep: pytest.CollectReport | pytest.TestReport,
+    ) -> None:
         """Emitted when a node calls the pytest_collectreport hook.
 
         Because we only need the report when there's a failure/skip, as optimization
         we only expect to receive failed/skipped reports from workers (#330).
         """
         assert not rep.passed
         self._failed_worker_collectreport(node, rep)
 
-    def worker_warning_captured(self, warning_message, when, item):
-        """Emitted when a node calls the pytest_warning_captured hook (deprecated in 6.0)."""
-        # This hook as been removed in pytest 7.1, and we can remove support once we only
-        # support pytest >=7.1.
-        kwargs = dict(warning_message=warning_message, when=when, item=item)
-        self.config.hook.pytest_warning_captured.call_historic(kwargs=kwargs)
-
-    def worker_warning_recorded(self, warning_message, when, nodeid, location):
+    def worker_warning_recorded(
+        self,
+        warning_message: warnings.WarningMessage,
+        when: str,
+        nodeid: str,
+        location: tuple[str, int, str] | None,
+    ) -> None:
         """Emitted when a node calls the pytest_warning_recorded hook."""
         kwargs = dict(
             warning_message=warning_message, when=when, nodeid=nodeid, location=location
         )
         self.config.hook.pytest_warning_recorded.call_historic(kwargs=kwargs)
 
-    def _clone_node(self, node):
+    def _clone_node(self, node: WorkerController) -> WorkerController:
         """Return new node based on an existing one.
 
         This is normally for when a node dies, this will copy the spec
         of the existing node and create a new one with a new id.  The
         new node will have been setup so it will start calling the
         "worker_*" hooks and do work soon.
         """
         spec = node.gateway.spec
         spec.id = None
+        assert self.nodemanager is not None
         self.nodemanager.group.allocate_id(spec)
-        node = self.nodemanager.setup_node(spec, self.queue.put)
-        self._active_nodes.add(node)
-        return node
-
-    def _failed_worker_collectreport(self, node, rep):
+        clone = self.nodemanager.setup_node(spec, self.queue.put)
+        self._active_nodes.add(clone)
+        return clone
+
+    def _failed_worker_collectreport(
+        self,
+        node: WorkerController,
+        rep: pytest.CollectReport | pytest.TestReport,
+    ) -> None:
         # Check we haven't already seen this report (from
         # another worker).
         if rep.longrepr not in self._failed_collection_errors:
             self._failed_collection_errors[rep.longrepr] = True
             self.config.hook.pytest_collectreport(report=rep)
             self._handlefailures(rep)
 
-    def _handlefailures(self, rep):
+    def _handlefailures(
+        self,
+        rep: pytest.CollectReport | pytest.TestReport,
+    ) -> None:
         if rep.failed:
             self.countfailures += 1
             if (
                 self.maxfail
                 and self.countfailures >= self.maxfail
                 and not self.shouldstop
             ):
                 self.shouldstop = f"stopping after {self.countfailures} failures"
 
-    def triggershutdown(self):
+    def triggershutdown(self) -> None:
         if not self.shuttingdown:
             self.log("triggering shutdown")
             self.shuttingdown = True
+            assert self.sched is not None
             for node in self.sched.nodes:
                 node.shutdown()
 
-    def handle_crashitem(self, nodeid, worker):
+    def handle_crashitem(self, nodeid: str, worker: WorkerController) -> None:
         # XXX get more reporting info by recording pytest_runtest_logstart?
         # XXX count no of failures and retry N times
-        runner = self.config.pluginmanager.getplugin("runner")
         fspath = nodeid.split("::")[0]
         msg = f"worker {worker.gateway.id!r} crashed while running {nodeid!r}"
-        rep = runner.TestReport(
-            nodeid, (fspath, None, fspath), (), "failed", msg, "???"
+        rep = pytest.TestReport(
+            nodeid=nodeid,
+            location=(fspath, None, fspath),
+            keywords={},
+            outcome="failed",
+            longrepr=msg,
+            when="???",  # type: ignore[arg-type]
         )
-        rep.node = worker
+        rep.node = worker  # type: ignore[attr-defined]
 
         self.config.hook.pytest_handlecrashitem(
             crashitem=nodeid,
             report=rep,
             sched=self.sched,
         )
         self.config.hook.pytest_runtest_logreport(report=rep)
@@ -400,108 +465,115 @@
     ReadyForCollection = auto()
 
     # Worker has finished collection.
     CollectionDone = auto()
 
 
 class TerminalDistReporter:
-    def __init__(self, config) -> None:
+    def __init__(self, config: pytest.Config) -> None:
         self.config = config
         self.tr = config.pluginmanager.getplugin("terminalreporter")
-        self._status: dict[str, tuple[WorkerStatus, int]] = {}
+        self._status: dict[object, tuple[WorkerStatus, int]] = {}
         self._lastlen = 0
         self._isatty = getattr(self.tr, "isatty", self.tr.hasmarkup)
 
     def write_line(self, msg: str) -> None:
         self.tr.write_line(msg)
 
     def ensure_show_status(self) -> None:
         if not self._isatty:
             self.write_line(self.getstatus())
 
     def setstatus(
-        self, spec, status: WorkerStatus, *, tests_collected: int, show: bool = True
+        self,
+        spec: execnet.XSpec,
+        status: WorkerStatus,
+        *,
+        tests_collected: int,
+        show: bool = True,
     ) -> None:
         self._status[spec.id] = (status, tests_collected)
         if show and self._isatty:
             self.rewrite(self.getstatus())
 
     def getstatus(self) -> str:
         if self.config.option.verbose >= 0:
             line = get_workers_status_line(list(self._status.values()))
             if line:
                 return line
 
         return "bringing up nodes..."
 
-    def rewrite(self, line, newline=False):
+    def rewrite(self, line: str, newline: bool = False) -> None:
         pline = line + " " * max(self._lastlen - len(line), 0)
         if newline:
             self._lastlen = 0
             pline += "\n"
         else:
             self._lastlen = len(line)
         self.tr.rewrite(pline, bold=True)
 
     @pytest.hookimpl
-    def pytest_xdist_setupnodes(self, specs) -> None:
+    def pytest_xdist_setupnodes(self, specs: Sequence[execnet.XSpec]) -> None:
         self._specs = specs
         for spec in specs:
             self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=False)
         self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=True)
         self.ensure_show_status()
 
     @pytest.hookimpl
-    def pytest_xdist_newgateway(self, gateway) -> None:
+    def pytest_xdist_newgateway(self, gateway: execnet.Gateway) -> None:
         if self.config.option.verbose > 0:
             rinfo = gateway._rinfo()
             different_interpreter = rinfo.executable != sys.executable
             if different_interpreter:
-                version = "%s.%s.%s" % rinfo.version_info[:3]
+                version = "{}.{}.{}".format(*rinfo.version_info[:3])
                 self.rewrite(
                     f"[{gateway.id}] {rinfo.platform} Python {version} cwd: {rinfo.cwd}",
                     newline=True,
                 )
         self.setstatus(gateway.spec, WorkerStatus.Initialized, tests_collected=0)
 
     @pytest.hookimpl
-    def pytest_testnodeready(self, node) -> None:
+    def pytest_testnodeready(self, node: WorkerController) -> None:
         if self.config.option.verbose > 0:
             d = node.workerinfo
             different_interpreter = d.get("executable") != sys.executable
             if different_interpreter:
                 version = d["version"].replace("\n", " -- ")
                 self.rewrite(f"[{d['id']}] Python {version}", newline=True)
         self.setstatus(
             node.gateway.spec, WorkerStatus.ReadyForCollection, tests_collected=0
         )
 
     @pytest.hookimpl
-    def pytest_testnodedown(self, node, error) -> None:
+    def pytest_testnodedown(self, node: WorkerController, error: object) -> None:
         if not error:
             return
         self.write_line(f"[{node.gateway.id}] node down: {error}")
 
 
-def get_default_max_worker_restart(config):
-    """gets the default value of --max-worker-restart option if it is not provided.
+def get_default_max_worker_restart(config: pytest.Config) -> int | None:
+    """Gets the default value of --max-worker-restart option if it is not provided.
 
     Use a reasonable default to avoid workers from restarting endlessly due to crashing collections (#226).
     """
-    result = config.option.maxworkerrestart
-    if result is not None:
-        result = int(result)
+    result_str: str | None = config.option.maxworkerrestart
+    if result_str is not None:
+        result = int(result_str)
     elif config.option.numprocesses:
         # if --max-worker-restart was not provided, use a reasonable default (#226)
         result = config.option.numprocesses * 4
+    else:
+        result = None
     return result
 
 
 def get_workers_status_line(
-    status_and_items: Sequence[tuple[WorkerStatus, int]]
+    status_and_items: Sequence[tuple[WorkerStatus, int]],
 ) -> str:
     """
     Return the line to display during worker setup/collection based on the
     status of the workers and number of tests collected for each.
     """
     statuses = [s for s, c in status_and_items]
     total_workers = len(statuses)
```

### Comparing `pytest-xdist-3.5.0/src/xdist/looponfail.py` & `pytest_xdist-3.6.0/src/xdist/looponfail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 """
-    Implement -f aka looponfailing for pytest.
+Implement -f aka looponfailing for pytest.
 
-    NOTE that we try to avoid loading and depending on application modules
-    within the controlling process (the one that starts repeatedly test
-    processes) otherwise changes to source code can crash
-    the controlling process which should best never happen.
+NOTE that we try to avoid loading and depending on application modules
+within the controlling process (the one that starts repeatedly test
+processes) otherwise changes to source code can crash
+the controlling process which should best never happen.
 """
+
+from __future__ import annotations
+
 import os
 from pathlib import Path
-from typing import Dict, Sequence
-
-import pytest
 import sys
 import time
-import execnet
+from typing import Any
+from typing import Sequence
+
 from _pytest._io import TerminalWriter
+import execnet
+import pytest
 
 from xdist._path import visit_path
 
 
 @pytest.hookimpl
-def pytest_addoption(parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup("xdist", "distributed and subprocess testing")
     group._addoption(
         "-f",
         "--looponfail",
         action="store_true",
         dest="looponfail",
         default=False,
-        help="run tests in subprocess, wait for modified files "
-        "and re-run failing test set until all pass.",
+        help="Run tests in subprocess: wait for files to be modified, then "
+        "re-run failing test set until all pass.",
     )
 
 
 @pytest.hookimpl
-def pytest_cmdline_main(config):
+def pytest_cmdline_main(config: pytest.Config) -> int | None:
     if config.getoption("looponfail"):
         usepdb = config.getoption("usepdb", False)  # a core option
         if usepdb:
             raise pytest.UsageError("--pdb is incompatible with --looponfail.")
         looponfail_main(config)
         return 2  # looponfail only can get stop with ctrl-C anyway
+    return None
 
 
-def looponfail_main(config: "pytest.Config") -> None:
+def looponfail_main(config: pytest.Config) -> None:
     remotecontrol = RemoteControl(config)
     config_roots = config.getini("looponfailroots")
     if not config_roots:
         config_roots = [Path.cwd()]
     rootdirs = [Path(root) for root in config_roots]
     statrecorder = StatRecorder(rootdirs)
     try:
@@ -61,203 +66,213 @@
             )
             statrecorder.waitonchange(checkinterval=2.0)
     except KeyboardInterrupt:
         print()
 
 
 class RemoteControl:
-    def __init__(self, config):
+    gateway: execnet.Gateway
+
+    def __init__(self, config: pytest.Config) -> None:
         self.config = config
-        self.failures = []
+        self.failures: list[str] = []
 
-    def trace(self, *args):
+    def trace(self, *args: object) -> None:
         if self.config.option.debug:
             msg = " ".join(str(x) for x in args)
             print("RemoteControl:", msg)
 
-    def initgateway(self):
-        return execnet.makegateway("popen")
+    def initgateway(self) -> execnet.Gateway:
+        return execnet.makegateway("execmodel=main_thread_only//popen")
 
-    def setup(self, out=None):
-        if out is None:
-            out = TerminalWriter()
+    def setup(self) -> None:
         if hasattr(self, "gateway"):
             raise ValueError("already have gateway %r" % self.gateway)
         self.trace("setting up worker session")
         self.gateway = self.initgateway()
         self.channel = channel = self.gateway.remote_exec(
             init_worker_session,
             args=self.config.args,
             option_dict=vars(self.config.option),
         )
-        remote_outchannel = channel.receive()
+        remote_outchannel: execnet.Channel = channel.receive()
+
+        out = TerminalWriter()
 
-        def write(s):
+        def write(s: str) -> None:
             out._file.write(s)
             out._file.flush()
 
         remote_outchannel.setcallback(write)
 
-    def ensure_teardown(self):
+    def ensure_teardown(self) -> None:
         if hasattr(self, "channel"):
             if not self.channel.isclosed():
                 self.trace("closing", self.channel)
                 self.channel.close()
             del self.channel
         if hasattr(self, "gateway"):
             self.trace("exiting", self.gateway)
             self.gateway.exit()
             del self.gateway
 
-    def runsession(self):
+    def runsession(self) -> tuple[list[str], list[str], bool]:
         try:
             self.trace("sending", self.failures)
             self.channel.send(self.failures)
             try:
-                return self.channel.receive()
+                return self.channel.receive()  # type: ignore[no-any-return]
             except self.channel.RemoteError:
                 e = sys.exc_info()[1]
                 self.trace("ERROR", e)
                 raise
         finally:
             self.ensure_teardown()
 
-    def loop_once(self):
+    def loop_once(self) -> None:
         self.setup()
         self.wasfailing = self.failures and len(self.failures)
         result = self.runsession()
         failures, reports, collection_failed = result
         if collection_failed:
             pass  # "Collection failed, keeping previous failure set"
         else:
             uniq_failures = []
             for failure in failures:
                 if failure not in uniq_failures:
                     uniq_failures.append(failure)
             self.failures = uniq_failures
 
 
-def repr_pytest_looponfailinfo(failreports, rootdirs):
+def repr_pytest_looponfailinfo(
+    failreports: Sequence[str], rootdirs: Sequence[Path]
+) -> None:
     tr = TerminalWriter()
     if failreports:
         tr.sep("#", "LOOPONFAILING", bold=True)
         for report in failreports:
             if report:
                 tr.line(report, red=True)
     tr.sep("#", "waiting for changes", bold=True)
     for rootdir in rootdirs:
         tr.line(f"### Watching:   {rootdir}", bold=True)
 
 
-def init_worker_session(channel, args, option_dict):
+def init_worker_session(
+    channel: "execnet.Channel",  # noqa: UP037
+    args: list[str],
+    option_dict: dict[str, "Any"],  # noqa: UP037
+) -> None:
     import os
     import sys
 
     outchannel = channel.gateway.newchannel()
-    sys.stdout = sys.stderr = outchannel.makefile("w")
+    sys.stdout = sys.stderr = outchannel.makefile("w")  # type: ignore[assignment]
     channel.send(outchannel)
     # prune sys.path to not contain relative paths
     newpaths = []
     for p in sys.path:
         if p:
-            if not os.path.isabs(p):
+            # Ignore path placeholders created for editable installs
+            if not os.path.isabs(p) and not p.endswith(".__path_hook__"):
                 p = os.path.abspath(p)
             newpaths.append(p)
     sys.path[:] = newpaths
 
     # fullwidth, hasmarkup = channel.receive()
-    from _pytest.config import Config
+    from pytest import Config
 
     config = Config.fromdictargs(option_dict, list(args))
     config.args = args
     from xdist.looponfail import WorkerFailSession
 
     WorkerFailSession(config, channel).main()
 
 
 class WorkerFailSession:
-    def __init__(self, config, channel):
+    def __init__(self, config: pytest.Config, channel: execnet.Channel) -> None:
         self.config = config
         self.channel = channel
-        self.recorded_failures = []
+        self.recorded_failures: list[pytest.CollectReport | pytest.TestReport] = []
         self.collection_failed = False
         config.pluginmanager.register(self)
         config.option.looponfail = False
         config.option.usepdb = False
 
-    def DEBUG(self, *args):
+    def DEBUG(self, *args: object) -> None:
         if self.config.option.debug:
             print(" ".join(map(str, args)))
 
     @pytest.hookimpl
-    def pytest_collection(self, session):
+    def pytest_collection(self, session: pytest.Session) -> bool:
         self.session = session
         self.trails = self.current_command
         hook = self.session.ihook
         try:
             items = session.perform_collect(self.trails or None)
         except pytest.UsageError:
             items = session.perform_collect(None)
         hook.pytest_collection_modifyitems(
             session=session, config=session.config, items=items
         )
         hook.pytest_collection_finish(session=session)
         return True
 
     @pytest.hookimpl
-    def pytest_runtest_logreport(self, report):
+    def pytest_runtest_logreport(self, report: pytest.TestReport) -> None:
         if report.failed:
             self.recorded_failures.append(report)
 
     @pytest.hookimpl
-    def pytest_collectreport(self, report):
+    def pytest_collectreport(self, report: pytest.CollectReport) -> None:
         if report.failed:
             self.recorded_failures.append(report)
             self.collection_failed = True
 
-    def main(self):
+    def main(self) -> None:
         self.DEBUG("WORKER: received configuration, waiting for command trails")
         try:
             command = self.channel.receive()
         except KeyboardInterrupt:
             return  # in the worker we can't do much about this
         self.DEBUG("received", command)
         self.current_command = command
         self.config.hook.pytest_cmdline_main(config=self.config)
         trails, failreports = [], []
         for rep in self.recorded_failures:
             trails.append(rep.nodeid)
             loc = rep.longrepr
             loc = str(getattr(loc, "reprcrash", loc))
             failreports.append(loc)
-        self.channel.send((trails, failreports, self.collection_failed))
+        result = (trails, failreports, self.collection_failed)
+        self.channel.send(result)
 
 
 class StatRecorder:
     def __init__(self, rootdirlist: Sequence[Path]) -> None:
         self.rootdirlist = rootdirlist
-        self.statcache: Dict[Path, os.stat_result] = {}
+        self.statcache: dict[Path, os.stat_result] = {}
         self.check()  # snapshot state
 
     def fil(self, p: Path) -> bool:
         return p.is_file() and not p.name.startswith(".") and p.suffix != ".pyc"
 
     def rec(self, p: Path) -> bool:
         return not p.name.startswith(".") and p.exists()
 
-    def waitonchange(self, checkinterval=1.0):
+    def waitonchange(self, checkinterval: float = 1.0) -> None:
         while 1:
             changed = self.check()
             if changed:
                 return
             time.sleep(checkinterval)
 
-    def check(self, removepycfiles: bool = True) -> bool:  # noqa, too complex
+    def check(self, removepycfiles: bool = True) -> bool:
         changed = False
-        newstat: Dict[Path, os.stat_result] = {}
+        newstat: dict[Path, os.stat_result] = {}
         for rootdir in self.rootdirlist:
             for path in visit_path(rootdir, filter=self.fil, recurse=self.rec):
                 oldstat = self.statcache.pop(path, None)
                 try:
                     curstat = path.stat()
                 except OSError:
                     if oldstat:
```

### Comparing `pytest-xdist-3.5.0/src/xdist/newhooks.py` & `pytest_xdist-3.6.0/src/xdist/newhooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,87 +7,117 @@
 ``pytest_runtest_logreport``: ``rep`` parameter has a ``node`` attribute.
 
 You can use this hooks just as you would use normal pytest hooks, but some care
 must be taken in plugins in case ``xdist`` is not installed. Please see:
 
     http://pytest.org/en/latest/writing_plugins.html#optionally-using-hooks-from-3rd-party-plugins
 """
+
+from __future__ import annotations
+
+import os
+from typing import Any
+from typing import Sequence
+from typing import TYPE_CHECKING
+
+import execnet
 import pytest
 
 
+if TYPE_CHECKING:
+    from xdist.remote import Producer
+    from xdist.scheduler.protocol import Scheduling
+    from xdist.workermanage import WorkerController
+
+
 @pytest.hookspec()
-def pytest_xdist_setupnodes(config, specs):
-    """called before any remote node is set up."""
+def pytest_xdist_setupnodes(
+    config: pytest.Config, specs: Sequence[execnet.XSpec]
+) -> None:
+    """Called before any remote node is set up."""
 
 
 @pytest.hookspec()
-def pytest_xdist_newgateway(gateway):
-    """called on new raw gateway creation."""
+def pytest_xdist_newgateway(gateway: execnet.Gateway) -> None:
+    """Called on new raw gateway creation."""
 
 
 @pytest.hookspec(
     warn_on_impl=DeprecationWarning(
         "rsync feature is deprecated and will be removed in pytest-xdist 4.0"
     )
 )
-def pytest_xdist_rsyncstart(source, gateways):
-    """called before rsyncing a directory to remote gateways takes place."""
+def pytest_xdist_rsyncstart(
+    source: str | os.PathLike[str],
+    gateways: Sequence[execnet.Gateway],
+) -> None:
+    """Called before rsyncing a directory to remote gateways takes place."""
 
 
 @pytest.hookspec(
     warn_on_impl=DeprecationWarning(
         "rsync feature is deprecated and will be removed in pytest-xdist 4.0"
     )
 )
-def pytest_xdist_rsyncfinish(source, gateways):
-    """called after rsyncing a directory to remote gateways takes place."""
+def pytest_xdist_rsyncfinish(
+    source: str | os.PathLike[str],
+    gateways: Sequence[execnet.Gateway],
+) -> None:
+    """Called after rsyncing a directory to remote gateways takes place."""
 
 
 @pytest.hookspec(firstresult=True)
-def pytest_xdist_getremotemodule():
-    """called when creating remote node"""
+def pytest_xdist_getremotemodule() -> Any:
+    """Called when creating remote node."""
 
 
 @pytest.hookspec()
-def pytest_configure_node(node):
-    """configure node information before it gets instantiated."""
+def pytest_configure_node(node: WorkerController) -> None:
+    """Configure node information before it gets instantiated."""
 
 
 @pytest.hookspec()
-def pytest_testnodeready(node):
+def pytest_testnodeready(node: WorkerController) -> None:
     """Test Node is ready to operate."""
 
 
 @pytest.hookspec()
-def pytest_testnodedown(node, error):
+def pytest_testnodedown(node: WorkerController, error: object | None) -> None:
     """Test Node is down."""
 
 
 @pytest.hookspec()
-def pytest_xdist_node_collection_finished(node, ids):
-    """called by the controller node when a worker node finishes collecting."""
+def pytest_xdist_node_collection_finished(
+    node: WorkerController, ids: Sequence[str]
+) -> None:
+    """Called by the controller node when a worker node finishes collecting."""
 
 
 @pytest.hookspec(firstresult=True)
-def pytest_xdist_make_scheduler(config, log):
-    """return a node scheduler implementation"""
+def pytest_xdist_make_scheduler(
+    config: pytest.Config, log: Producer
+) -> Scheduling | None:
+    """Return a node scheduler implementation."""
 
 
 @pytest.hookspec(firstresult=True)
-def pytest_xdist_auto_num_workers(config):
+def pytest_xdist_auto_num_workers(config: pytest.Config) -> int:
     """
     Return the number of workers to spawn when ``--numprocesses=auto`` is given in the
     command-line.
 
     .. versionadded:: 2.1
     """
+    raise NotImplementedError()
 
 
 @pytest.hookspec(firstresult=True)
-def pytest_handlecrashitem(crashitem, report, sched):
+def pytest_handlecrashitem(
+    crashitem: str, report: pytest.TestReport, sched: Scheduling
+) -> None:
     """
     Handle a crashitem, modifying the report if necessary.
 
     The scheduler is provided as a parameter to reschedule the test if desired with
     `sched.mark_test_pending`.
 
     def pytest_handlecrashitem(crashitem, report, sched):
```

### Comparing `pytest-xdist-3.5.0/src/xdist/plugin.py` & `pytest_xdist-3.6.0/src/xdist/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,104 @@
+from __future__ import annotations
+
 import os
-import uuid
 import sys
+from typing import Literal
+import uuid
 import warnings
 
 import pytest
 
 
-PYTEST_GTE_7 = hasattr(pytest, "version_tuple") and pytest.version_tuple >= (7, 0)  # type: ignore[attr-defined]
-
 _sys_path = list(sys.path)  # freeze a copy of sys.path at interpreter startup
 
 
 @pytest.hookimpl
-def pytest_xdist_auto_num_workers(config):
+def pytest_xdist_auto_num_workers(config: pytest.Config) -> int:
     env_var = os.environ.get("PYTEST_XDIST_AUTO_NUM_WORKERS")
     if env_var:
         try:
             return int(env_var)
         except ValueError:
             warnings.warn(
                 "PYTEST_XDIST_AUTO_NUM_WORKERS is not a number: {env_var!r}. Ignoring it."
             )
 
     try:
         import psutil
     except ImportError:
         pass
     else:
-        use_logical = config.option.numprocesses == "logical"
+        use_logical: bool = config.option.numprocesses == "logical"
         count = psutil.cpu_count(logical=use_logical) or psutil.cpu_count()
         if count:
             return count
     try:
         from os import sched_getaffinity
 
-        def cpu_count():
+        def cpu_count() -> int:
             return len(sched_getaffinity(0))
 
     except ImportError:
         if os.environ.get("TRAVIS") == "true":
             # workaround https://bitbucket.org/pypy/pypy/issues/2375
             return 2
         try:
-            from os import cpu_count
+            from os import cpu_count  # type: ignore[assignment]
         except ImportError:
             from multiprocessing import cpu_count
     try:
         n = cpu_count()
     except NotImplementedError:
         return 1
     return n if n else 1
 
 
-def parse_numprocesses(s):
+def parse_numprocesses(s: str) -> int | Literal["auto", "logical"]:
     if s in ("auto", "logical"):
-        return s
+        return s  # type: ignore[return-value]
     elif s is not None:
         return int(s)
 
 
 @pytest.hookimpl
-def pytest_addoption(parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
+    # 'Help' formatting (same rules as pytest's):
+    # Start with capitalized letters.
+    # If a single phrase, do not end with period. If more than one phrase, all phrases end with periods.
+    # Use \n to separate logical lines.
     group = parser.getgroup("xdist", "distributed and subprocess testing")
     group._addoption(
         "-n",
         "--numprocesses",
         dest="numprocesses",
         metavar="numprocesses",
         action="store",
         type=parse_numprocesses,
-        help="Shortcut for '--dist=load --tx=NUM*popen'. With 'auto', attempt "
-        "to detect physical CPU count. With 'logical', detect logical CPU "
-        "count. If physical CPU count cannot be found, falls back to logical "
-        "count. This will be 0 when used with --pdb.",
+        help="Shortcut for '--dist=load --tx=NUM*popen'.\n"
+        "With 'logical', attempt to detect logical CPU count (requires psutil, falls back to 'auto').\n"
+        "With 'auto', attempt to detect physical CPU count. If physical CPU count cannot be determined, "
+        "falls back to 1.\n"
+        "Forced to 0 (disabled) when used with --pdb.",
     )
     group.addoption(
         "--maxprocesses",
         dest="maxprocesses",
         metavar="maxprocesses",
         action="store",
         type=int,
-        help="limit the maximum number of workers to process the tests when using --numprocesses=auto",
+        help="Limit the maximum number of workers to process the tests when using --numprocesses "
+        "with 'auto' or 'logical'",
     )
     group.addoption(
         "--max-worker-restart",
         action="store",
         default=None,
         dest="maxworkerrestart",
-        help="maximum number of workers that can be restarted "
+        help="Maximum number of workers that can be restarted "
         "when crashed (set to zero to disable this feature)",
     )
     group.addoption(
         "--dist",
         metavar="distmode",
         action="store",
         choices=[
@@ -102,136 +109,136 @@
             "loadgroup",
             "worksteal",
             "no",
         ],
         dest="dist",
         default="no",
         help=(
-            "set mode for distributing tests to exec environments.\n\n"
-            "each: send each test to all available environments.\n\n"
-            "load: load balance by sending any pending test to any"
+            "Set mode for distributing tests to exec environments.\n\n"
+            "each: Send each test to all available environments.\n\n"
+            "load: Load balance by sending any pending test to any"
             " available environment.\n\n"
-            "loadscope: load balance by sending pending groups of tests in"
+            "loadscope: Load balance by sending pending groups of tests in"
             " the same scope to any available environment.\n\n"
-            "loadfile: load balance by sending test grouped by file"
+            "loadfile: Load balance by sending test grouped by file"
             " to any available environment.\n\n"
-            "loadgroup: like load, but sends tests marked with 'xdist_group' to the same worker.\n\n"
-            "worksteal: split the test suite between available environments,"
-            " then rebalance when any worker runs out of tests.\n\n"
-            "(default) no: run tests inprocess, don't distribute."
+            "loadgroup: Like 'load', but sends tests marked with 'xdist_group' to the same worker.\n\n"
+            "worksteal: Split the test suite between available environments,"
+            " then re-balance when any worker runs out of tests.\n\n"
+            "(default) no: Run tests inprocess, don't distribute."
         ),
     )
     group.addoption(
         "--tx",
         dest="tx",
         action="append",
         default=[],
         metavar="xspec",
         help=(
-            "add a test execution environment. some examples: "
-            "--tx popen//python=python2.5 --tx socket=192.168.1.102:8888 "
+            "Add a test execution environment. Some examples:\n"
+            "--tx popen//python=python2.5 --tx socket=192.168.1.102:8888\n"
             "--tx ssh=user@codespeak.net//chdir=testcache"
         ),
     )
     group._addoption(
         "-d",
         action="store_true",
         dest="distload",
         default=False,
-        help="load-balance tests.  shortcut for '--dist=load'",
+        help="Load-balance tests. Shortcut for '--dist=load'.",
     )
     group.addoption(
         "--rsyncdir",
         action="append",
         default=[],
         metavar="DIR",
-        help="add directory for rsyncing to remote tx nodes.",
+        help="Add directory for rsyncing to remote tx nodes",
     )
     group.addoption(
         "--rsyncignore",
         action="append",
         default=[],
         metavar="GLOB",
-        help="add expression for ignores when rsyncing to remote tx nodes.",
+        help="Add expression for ignores when rsyncing to remote tx nodes",
     )
     group.addoption(
         "--testrunuid",
         action="store",
         help=(
-            "provide an identifier shared amongst all workers as the value of "
-            "the 'testrun_uid' fixture,\n\n,"
-            "if not provided, 'testrun_uid' is filled with a new unique string "
+            "Provide an identifier shared amongst all workers as the value of "
+            "the 'testrun_uid' fixture.\n"
+            "If not provided, 'testrun_uid' is filled with a new unique string "
             "on every test run."
         ),
     )
     group.addoption(
         "--maxschedchunk",
         action="store",
         type=int,
         help=(
-            "Maximum number of tests scheduled in one step for --dist=load. "
+            "Maximum number of tests scheduled in one step for --dist=load.\n"
             "Setting it to 1 will force pytest to send tests to workers one by "
-            "one - might be useful for a small number of slow tests. "
+            "one - might be useful for a small number of slow tests.\n"
             "Larger numbers will allow the scheduler to submit consecutive "
-            "chunks of tests to workers - allows reusing fixtures. "
+            "chunks of tests to workers - allows reusing fixtures.\n"
             "Due to implementation reasons, at least 2 tests are scheduled per "
-            "worker at the start. Only later tests can be scheduled one by one. "
+            "worker at the start. Only later tests can be scheduled one by one.\n"
             "Unlimited if not set."
         ),
     )
 
     parser.addini(
         "rsyncdirs",
         "list of (relative) paths to be rsynced for remote distributed testing.",
-        type="paths" if PYTEST_GTE_7 else "pathlist",
+        type="paths",
     )
     parser.addini(
         "rsyncignore",
         "list of (relative) glob-style paths to be ignored for rsyncing.",
-        type="paths" if PYTEST_GTE_7 else "pathlist",
+        type="paths",
     )
     parser.addini(
         "looponfailroots",
-        type="paths" if PYTEST_GTE_7 else "pathlist",
+        type="paths",
         help="directories to check for changes. Default: current directory.",
     )
 
 
 # -------------------------------------------------------------------------
 # distributed testing hooks
 # -------------------------------------------------------------------------
 
 
 @pytest.hookimpl
-def pytest_addhooks(pluginmanager):
+def pytest_addhooks(pluginmanager: pytest.PytestPluginManager) -> None:
     from xdist import newhooks
 
     pluginmanager.add_hookspecs(newhooks)
 
 
 # -------------------------------------------------------------------------
 # distributed testing initialization
 # -------------------------------------------------------------------------
 
 
 @pytest.hookimpl(trylast=True)
-def pytest_configure(config):
+def pytest_configure(config: pytest.Config) -> None:
     config_line = (
         "xdist_group: specify group for tests should run in same session."
         "in relation to one another. Provided by pytest-xdist."
     )
     config.addinivalue_line("markers", config_line)
 
     # Skip this plugin entirely when only doing collection.
     if config.getvalue("collectonly"):
         return
 
     # Create the distributed session in case we have a valid distribution
     # mode and test environments.
-    if config.getoption("dist") != "no" and config.getoption("tx"):
+    if _is_distribution_mode(config):
         from xdist.dsession import DSession
 
         session = DSession(config)
         config.pluginmanager.register(session, "dsession")
         tr = config.pluginmanager.getplugin("terminalreporter")
         if tr:
             tr.showfspath = False
@@ -248,16 +255,24 @@
         warning = DeprecationWarning(
             "The --rsyncdir command line argument and rsyncdirs config variable are deprecated.\n"
             "The rsync feature will be removed in pytest-xdist 4.0."
         )
         config.issue_config_time_warning(warning, 2)
 
 
+def _is_distribution_mode(config: pytest.Config) -> bool:
+    """Whether distribution mode is on."""
+    return config.getoption("dist") != "no" and bool(config.getoption("tx"))
+
+
 @pytest.hookimpl(tryfirst=True)
-def pytest_cmdline_main(config):
+def pytest_cmdline_main(config: pytest.Config) -> None:
+    if config.option.distload:
+        config.option.dist = "load"
+
     usepdb = config.getoption("usepdb", False)  # a core option
     if config.option.numprocesses in ("auto", "logical"):
         if usepdb:
             config.option.numprocesses = 0
             config.option.dist = "no"
         else:
             auto_num_cpus = config.hook.pytest_xdist_auto_num_workers(config=config)
@@ -266,38 +281,45 @@
     if config.option.numprocesses:
         if config.option.dist == "no":
             config.option.dist = "load"
         numprocesses = config.option.numprocesses
         if config.option.maxprocesses:
             numprocesses = min(numprocesses, config.option.maxprocesses)
         config.option.tx = ["popen"] * numprocesses
-    if config.option.distload:
-        config.option.dist = "load"
+
+    if config.option.numprocesses == 0:
+        config.option.dist = "no"
+        config.option.tx = []
+
     val = config.getvalue
-    if not val("collectonly") and val("dist") != "no" and usepdb:
+    if not val("collectonly") and _is_distribution_mode(config) and usepdb:
         raise pytest.UsageError(
             "--pdb is incompatible with distributing tests; try using -n0 or -nauto."
-        )  # noqa: E501
+        )
 
 
 # -------------------------------------------------------------------------
 # fixtures and API to easily know the role of current node
 # -------------------------------------------------------------------------
 
 
-def is_xdist_worker(request_or_session) -> bool:
-    """Return `True` if this is an xdist worker, `False` otherwise
+def is_xdist_worker(
+    request_or_session: pytest.FixtureRequest | pytest.Session,
+) -> bool:
+    """Return `True` if this is an xdist worker, `False` otherwise.
 
     :param request_or_session: the `pytest` `request` or `session` object
     """
     return hasattr(request_or_session.config, "workerinput")
 
 
-def is_xdist_controller(request_or_session) -> bool:
-    """Return `True` if this is the xdist controller, `False` otherwise
+def is_xdist_controller(
+    request_or_session: pytest.FixtureRequest | pytest.Session,
+) -> bool:
+    """Return `True` if this is the xdist controller, `False` otherwise.
 
     Note: this method also returns `False` when distribution has not been
     activated at all.
 
     :param request_or_session: the `pytest` `request` or `session` object
     """
     return (
@@ -306,39 +328,43 @@
     )
 
 
 # ALIAS: TODO, deprecate (#592)
 is_xdist_master = is_xdist_controller
 
 
-def get_xdist_worker_id(request_or_session):
+def get_xdist_worker_id(
+    request_or_session: pytest.FixtureRequest | pytest.Session,
+) -> str:
     """Return the id of the current worker ('gw0', 'gw1', etc) or 'master'
     if running on the controller node.
 
     If not distributing tests (for example passing `-n0` or not passing `-n` at all)
     also return 'master'.
 
     :param request_or_session: the `pytest` `request` or `session` object
     """
     if hasattr(request_or_session.config, "workerinput"):
-        return request_or_session.config.workerinput["workerid"]
+        workerid: str = request_or_session.config.workerinput["workerid"]
+        return workerid
     else:
         # TODO: remove "master", ideally for a None
         return "master"
 
 
 @pytest.fixture(scope="session")
-def worker_id(request):
+def worker_id(request: pytest.FixtureRequest) -> str:
     """Return the id of the current worker ('gw0', 'gw1', etc) or 'master'
     if running on the master node.
     """
     # TODO: remove "master", ideally for a None
     return get_xdist_worker_id(request)
 
 
 @pytest.fixture(scope="session")
-def testrun_uid(request):
+def testrun_uid(request: pytest.FixtureRequest) -> str:
     """Return the unique id of the current test."""
     if hasattr(request.config, "workerinput"):
-        return request.config.workerinput["testrunuid"]
+        testrunid: str = request.config.workerinput["testrunuid"]
+        return testrunid
     else:
         return uuid.uuid4().hex
```

### Comparing `pytest-xdist-3.5.0/src/xdist/remote.py` & `pytest_xdist-3.6.0/src/xdist/remote.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,265 +1,301 @@
 """
-    This module is executed in remote subprocesses and helps to
-    control a remote testing session and relay back information.
-    It assumes that 'py' is importable and does not have dependencies
-    on the rest of the xdist code.  This means that the xdist-plugin
-    needs not to be installed in remote environments.
+This module is executed in remote subprocesses and helps to
+control a remote testing session and relay back information.
+It assumes that 'py' is importable and does not have dependencies
+on the rest of the xdist code.  This means that the xdist-plugin
+needs not to be installed in remote environments.
 """
 
+from __future__ import annotations
+
 import contextlib
-import sys
+import enum
 import os
+import sys
 import time
 from typing import Any
+from typing import Generator
+from typing import Literal
+from typing import Sequence
+from typing import TypedDict
+import warnings
 
+from _pytest.config import _prepareconfig
+import execnet
 import pytest
-from execnet.gateway_base import dumps, DumpError
 
-from _pytest.config import _prepareconfig, Config
 
 try:
     from setproctitle import setproctitle
 except ImportError:
 
-    def setproctitle(title):
+    def setproctitle(title: str) -> None:
         pass
 
 
 class Producer:
     """
     Simplified implementation of the same interface as py.log, for backward compatibility
     since we dropped the dependency on pylib.
     Note: this is defined here because this module can't depend on xdist, so we need
     to have the other way around.
     """
 
-    def __init__(self, name: str, *, enabled: bool = True):
+    def __init__(self, name: str, *, enabled: bool = True) -> None:
         self.name = name
         self.enabled = enabled
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.name!r}, enabled={self.enabled})"
 
     def __call__(self, *a: Any, **k: Any) -> None:
         if self.enabled:
             print(f"[{self.name}]", *a, **k, file=sys.stderr)
 
-    def __getattr__(self, name: str) -> "Producer":
+    def __getattr__(self, name: str) -> Producer:
         return type(self)(name, enabled=self.enabled)
 
 
-def worker_title(title):
+def worker_title(title: str) -> None:
     try:
         setproctitle(title)
     except Exception:
         # changing the process name is very optional, no errors please
         pass
 
 
-class WorkerInteractor:
-    SHUTDOWN_MARK = object()
-    QUEUE_REPLACED_MARK = object()
+class Marker(enum.Enum):
+    SHUTDOWN = 0
+    QUEUE_REPLACED = 1
 
-    def __init__(self, config, channel):
+
+class WorkerInteractor:
+    def __init__(self, config: pytest.Config, channel: execnet.Channel) -> None:
         self.config = config
-        self.workerid = config.workerinput.get("workerid", "?")
-        self.testrunuid = config.workerinput["testrunuid"]
+        workerinput: dict[str, Any] = config.workerinput  # type: ignore[attr-defined]
+        self.workerid = workerinput.get("workerid", "?")
+        self.testrunuid = workerinput["testrunuid"]
         self.log = Producer(f"worker-{self.workerid}", enabled=config.option.debug)
         self.channel = channel
         self.torun = self._make_queue()
-        self.nextitem_index = None
+        self.nextitem_index: int | None | Literal[Marker.SHUTDOWN] = None
         config.pluginmanager.register(self)
 
-    def _make_queue(self):
+    def _make_queue(self) -> Any:
         return self.channel.gateway.execmodel.queue.Queue()
 
-    def _get_next_item_index(self):
+    def _get_next_item_index(self) -> int | Literal[Marker.SHUTDOWN]:
         """Gets the next item from test queue. Handles the case when the queue
         is replaced concurrently in another thread.
         """
         result = self.torun.get()
-        while result is self.QUEUE_REPLACED_MARK:
+        while result is Marker.QUEUE_REPLACED:
             result = self.torun.get()
-        return result
+        return result  # type: ignore[no-any-return]
 
-    def sendevent(self, name, **kwargs):
+    def sendevent(self, name: str, **kwargs: object) -> None:
         self.log("sending", name, kwargs)
         self.channel.send((name, kwargs))
 
     @pytest.hookimpl
-    def pytest_internalerror(self, excrepr):
+    def pytest_internalerror(self, excrepr: object) -> None:
         formatted_error = str(excrepr)
         for line in formatted_error.split("\n"):
             self.log("IERROR>", line)
         interactor.sendevent("internal_error", formatted_error=formatted_error)
 
     @pytest.hookimpl
-    def pytest_sessionstart(self, session):
+    def pytest_sessionstart(self, session: pytest.Session) -> None:
         self.session = session
         workerinfo = getinfodict()
         self.sendevent("workerready", workerinfo=workerinfo)
 
     @pytest.hookimpl(hookwrapper=True)
-    def pytest_sessionfinish(self, exitstatus):
+    def pytest_sessionfinish(self, exitstatus: int) -> Generator[None, object, None]:
+        workeroutput: dict[str, Any] = self.config.workeroutput  # type: ignore[attr-defined]
         # in pytest 5.0+, exitstatus is an IntEnum object
-        self.config.workeroutput["exitstatus"] = int(exitstatus)
+        workeroutput["exitstatus"] = int(exitstatus)
+        workeroutput["shouldfail"] = self.session.shouldfail
+        workeroutput["shouldstop"] = self.session.shouldstop
         yield
-        self.sendevent("workerfinished", workeroutput=self.config.workeroutput)
+        self.sendevent("workerfinished", workeroutput=workeroutput)
 
     @pytest.hookimpl
-    def pytest_collection(self, session):
+    def pytest_collection(self) -> None:
         self.sendevent("collectionstart")
 
-    def handle_command(self, command):
-        if command is self.SHUTDOWN_MARK:
-            self.torun.put(self.SHUTDOWN_MARK)
+    def handle_command(
+        self, command: tuple[str, dict[str, Any]] | Literal[Marker.SHUTDOWN]
+    ) -> None:
+        if command is Marker.SHUTDOWN:
+            self.torun.put(Marker.SHUTDOWN)
             return
 
         name, kwargs = command
 
         self.log("received command", name, kwargs)
         if name == "runtests":
             for i in kwargs["indices"]:
                 self.torun.put(i)
         elif name == "runtests_all":
             for i in range(len(self.session.items)):
                 self.torun.put(i)
         elif name == "shutdown":
-            self.torun.put(self.SHUTDOWN_MARK)
+            self.torun.put(Marker.SHUTDOWN)
         elif name == "steal":
             self.steal(kwargs["indices"])
 
-    def steal(self, indices):
-        indices = set(indices)
+    def steal(self, indices: Sequence[int]) -> None:
+        indices_set = set(indices)
         stolen = []
 
         old_queue, self.torun = self.torun, self._make_queue()
 
-        def old_queue_get_nowait_noraise():
+        def old_queue_get_nowait_noraise() -> int | None:
             with contextlib.suppress(self.channel.gateway.execmodel.queue.Empty):
-                return old_queue.get_nowait()
+                return old_queue.get_nowait()  # type: ignore[no-any-return]
+            return None
 
         for i in iter(old_queue_get_nowait_noraise, None):
-            if i in indices:
+            if i in indices_set:
                 stolen.append(i)
             else:
                 self.torun.put(i)
 
         self.sendevent("unscheduled", indices=stolen)
-        old_queue.put(self.QUEUE_REPLACED_MARK)
+        old_queue.put(Marker.QUEUE_REPLACED)
 
     @pytest.hookimpl
-    def pytest_runtestloop(self, session):
+    def pytest_runtestloop(self, session: pytest.Session) -> bool:
         self.log("entering main loop")
-        self.channel.setcallback(self.handle_command, endmarker=self.SHUTDOWN_MARK)
+        self.channel.setcallback(self.handle_command, endmarker=Marker.SHUTDOWN)
         self.nextitem_index = self._get_next_item_index()
-        while self.nextitem_index is not self.SHUTDOWN_MARK:
+        while self.nextitem_index is not Marker.SHUTDOWN:
             self.run_one_test()
+            if session.shouldfail or session.shouldstop:
+                break
         return True
 
-    def run_one_test(self):
+    def run_one_test(self) -> None:
+        assert isinstance(self.nextitem_index, int)
         self.item_index = self.nextitem_index
         self.nextitem_index = self._get_next_item_index()
 
         items = self.session.items
         item = items[self.item_index]
-        if self.nextitem_index is self.SHUTDOWN_MARK:
+        if self.nextitem_index is Marker.SHUTDOWN:
             nextitem = None
         else:
+            assert self.nextitem_index is not None
             nextitem = items[self.nextitem_index]
 
         worker_title("[pytest-xdist running] %s" % item.nodeid)
 
-        start = time.time()
+        start = time.perf_counter()
         self.config.hook.pytest_runtest_protocol(item=item, nextitem=nextitem)
-        duration = time.time() - start
+        duration = time.perf_counter() - start
 
         worker_title("[pytest-xdist idle]")
 
         self.sendevent(
             "runtest_protocol_complete", item_index=self.item_index, duration=duration
         )
 
-    def pytest_collection_modifyitems(self, session, config, items):
+    def pytest_collection_modifyitems(
+        self,
+        config: pytest.Config,
+        items: list[pytest.Item],
+    ) -> None:
         # add the group name to nodeid as suffix if --dist=loadgroup
         if config.getvalue("loadgroup"):
             for item in items:
                 mark = item.get_closest_marker("xdist_group")
                 if not mark:
                     continue
                 gname = (
                     mark.args[0]
                     if len(mark.args) > 0
                     else mark.kwargs.get("name", "default")
                 )
                 item._nodeid = f"{item.nodeid}@{gname}"
 
     @pytest.hookimpl
-    def pytest_collection_finish(self, session):
-        try:
-            topdir = str(self.config.rootpath)
-        except AttributeError:  # pytest <= 6.1.0
-            topdir = str(self.config.rootdir)
-
+    def pytest_collection_finish(self, session: pytest.Session) -> None:
         self.sendevent(
             "collectionfinish",
-            topdir=topdir,
+            topdir=str(self.config.rootpath),
             ids=[item.nodeid for item in session.items],
         )
 
     @pytest.hookimpl
-    def pytest_runtest_logstart(self, nodeid, location):
+    def pytest_runtest_logstart(
+        self,
+        nodeid: str,
+        location: tuple[str, int | None, str],
+    ) -> None:
         self.sendevent("logstart", nodeid=nodeid, location=location)
 
     @pytest.hookimpl
-    def pytest_runtest_logfinish(self, nodeid, location):
+    def pytest_runtest_logfinish(
+        self,
+        nodeid: str,
+        location: tuple[str, int | None, str],
+    ) -> None:
         self.sendevent("logfinish", nodeid=nodeid, location=location)
 
     @pytest.hookimpl
-    def pytest_runtest_logreport(self, report):
+    def pytest_runtest_logreport(self, report: pytest.TestReport) -> None:
         data = self.config.hook.pytest_report_to_serializable(
             config=self.config, report=report
         )
         data["item_index"] = self.item_index
         data["worker_id"] = self.workerid
         data["testrun_uid"] = self.testrunuid
         assert self.session.items[self.item_index].nodeid == report.nodeid
         self.sendevent("testreport", data=data)
 
     @pytest.hookimpl
-    def pytest_collectreport(self, report):
+    def pytest_collectreport(self, report: pytest.CollectReport) -> None:
         # send only reports that have not passed to controller as optimization (#330)
         if not report.passed:
             data = self.config.hook.pytest_report_to_serializable(
                 config=self.config, report=report
             )
             self.sendevent("collectreport", data=data)
 
     @pytest.hookimpl
-    def pytest_warning_recorded(self, warning_message, when, nodeid, location):
+    def pytest_warning_recorded(
+        self,
+        warning_message: warnings.WarningMessage,
+        when: str,
+        nodeid: str,
+        location: tuple[str, int, str] | None,
+    ) -> None:
         self.sendevent(
             "warning_recorded",
             warning_message_data=serialize_warning_message(warning_message),
             when=when,
             nodeid=nodeid,
             location=location,
         )
 
 
-def serialize_warning_message(warning_message):
+def serialize_warning_message(
+    warning_message: warnings.WarningMessage,
+) -> dict[str, Any]:
     if isinstance(warning_message.message, Warning):
         message_module = type(warning_message.message).__module__
         message_class_name = type(warning_message.message).__name__
         message_str = str(warning_message.message)
         # check now if we can serialize the warning arguments (#349)
         # if not, we will just use the exception message on the controller node
         try:
-            dumps(warning_message.message.args)
-        except DumpError:
+            execnet.dumps(warning_message.message.args)
+        except execnet.DumpError:
             message_args = None
         else:
             message_args = warning_message.message.args
     else:
         message_str = warning_message.message
         message_module = None
         message_class_name = None
@@ -276,60 +312,66 @@
         "message_module": message_module,
         "message_class_name": message_class_name,
         "message_args": message_args,
         "category_module": category_module,
         "category_class_name": category_class_name,
     }
     # access private _WARNING_DETAILS because the attributes vary between Python versions
-    for attr_name in warning_message._WARNING_DETAILS:
+    for attr_name in warning_message._WARNING_DETAILS:  # type: ignore[attr-defined]
         if attr_name in ("message", "category"):
             continue
         attr = getattr(warning_message, attr_name)
         # Check if we can serialize the warning detail, marking `None` otherwise
         # Note that we need to define the attr (even as `None`) to allow deserializing
         try:
-            dumps(attr)
-        except DumpError:
+            execnet.dumps(attr)
+        except execnet.DumpError:
             result[attr_name] = repr(attr)
         else:
             result[attr_name] = attr
     return result
 
 
-def getinfodict():
+class WorkerInfo(TypedDict):
+    version: str
+    version_info: tuple[int, int, int, str, int]
+    sysplatform: str
+    platform: str
+    executable: str
+    cwd: str
+    id: str
+    spec: execnet.XSpec
+
+
+def getinfodict() -> WorkerInfo:
     import platform
 
     return dict(
         version=sys.version,
-        version_info=tuple(sys.version_info),
+        version_info=tuple(sys.version_info),  # type: ignore[typeddict-item]
         sysplatform=sys.platform,
         platform=platform.platform(),
         executable=sys.executable,
         cwd=os.getcwd(),
     )
 
 
-def remote_initconfig(option_dict, args):
-    option_dict["plugins"].append("no:terminal")
-    return Config.fromdictargs(option_dict, args)
-
-
-def setup_config(config, basetemp):
+def setup_config(config: pytest.Config, basetemp: str | None) -> None:
     config.option.loadgroup = config.getvalue("dist") == "loadgroup"
     config.option.looponfail = False
     config.option.usepdb = False
     config.option.dist = "no"
     config.option.distload = False
     config.option.numprocesses = None
     config.option.maxprocesses = None
     config.option.basetemp = basetemp
 
 
 if __name__ == "__channelexec__":
-    channel = channel  # type: ignore[name-defined] # noqa: F821
+    channel: execnet.Channel = channel  # type: ignore[name-defined] # noqa: F821, PLW0127
     workerinput, args, option_dict, change_sys_path = channel.receive()  # type: ignore[name-defined]
 
     if change_sys_path is None:
         importpath = os.getcwd()
         sys.path.insert(0, importpath)
         os.environ["PYTHONPATH"] = (
             importpath + os.pathsep + os.environ.get("PYTHONPATH", "")
@@ -337,19 +379,15 @@
     else:
         sys.path = change_sys_path
 
     os.environ["PYTEST_XDIST_TESTRUNUID"] = workerinput["testrunuid"]
     os.environ["PYTEST_XDIST_WORKER"] = workerinput["workerid"]
     os.environ["PYTEST_XDIST_WORKER_COUNT"] = str(workerinput["workercount"])
 
-    if hasattr(Config, "InvocationParams"):
-        config = _prepareconfig(args, None)
-    else:
-        config = remote_initconfig(option_dict, args)
-        config.args = args
+    config = _prepareconfig(args, None)
 
     setup_config(config, option_dict.get("basetemp"))
     config._parser.prog = os.path.basename(workerinput["mainargv"][0])
     config.workerinput = workerinput  # type: ignore[attr-defined]
     config.workeroutput = {}  # type: ignore[attr-defined]
     interactor = WorkerInteractor(config, channel)  # type: ignore[name-defined]
     config.hook.pytest_cmdline_main(config=config)
```

### Comparing `pytest-xdist-3.5.0/src/xdist/report.py` & `pytest_xdist-3.6.0/src/xdist/report.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+from __future__ import annotations
+
 from difflib import unified_diff
+from typing import Sequence
 
 
-def report_collection_diff(from_collection, to_collection, from_id, to_id):
+def report_collection_diff(
+    from_collection: Sequence[str],
+    to_collection: Sequence[str],
+    from_id: str,
+    to_id: str,
+) -> str | None:
     """Report the collected test difference between two nodes.
 
     :returns: detailed message describing the difference between the given
     collections, or None if they are equal.
     """
     if from_collection == to_collection:
         return None
```

### Comparing `pytest-xdist-3.5.0/src/xdist/scheduler/load.py` & `pytest_xdist-3.6.0/src/xdist/scheduler/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
+
 from itertools import cycle
+from typing import Sequence
 
-from _pytest.runner import CollectReport
+import pytest
 
 from xdist.remote import Producer
-from xdist.workermanage import parse_spec_config
 from xdist.report import report_collection_diff
+from xdist.workermanage import parse_spec_config
+from xdist.workermanage import WorkerController
 
 
 class LoadScheduling:
     """Implement load scheduling across nodes.
 
     This distributes the tests collected across all nodes so each test
     is run just once.  All nodes collect and submit the test suite and
@@ -19,15 +23,15 @@
     scheduler to assign more tests if the number of pending tests for
     the node falls below a low-watermark.
 
     When created, ``numnodes`` defines how many nodes are expected to
     submit a collection. This is used to know when all nodes have
     finished collection or how large the chunks need to be created.
 
-    Attributes:
+    Attributes::
 
     :numnodes: The expected number of nodes taking part.  The actual
        number of nodes will vary during the scheduler's lifetime as
        nodes are added by the DSession as they are brought up and
        removed either because of a dead node or normal shutdown.  This
        number is primarily used to know when the initial collection is
        completed.
@@ -49,83 +53,85 @@
        to process.
 
     :log: A py.log.Producer instance.
 
     :config: Config object, used for handling hooks.
     """
 
-    def __init__(self, config, log=None):
+    def __init__(self, config: pytest.Config, log: Producer | None = None) -> None:
         self.numnodes = len(parse_spec_config(config))
-        self.node2collection = {}
-        self.node2pending = {}
-        self.pending = []
-        self.collection = None
+        self.node2collection: dict[WorkerController, list[str]] = {}
+        self.node2pending: dict[WorkerController, list[int]] = {}
+        self.pending: list[int] = []
+        self.collection: list[str] | None = None
         if log is None:
             self.log = Producer("loadsched")
         else:
             self.log = log.loadsched
         self.config = config
         self.maxschedchunk = self.config.getoption("maxschedchunk")
 
     @property
-    def nodes(self):
+    def nodes(self) -> list[WorkerController]:
         """A list of all nodes in the scheduler."""
         return list(self.node2pending.keys())
 
     @property
-    def collection_is_completed(self):
+    def collection_is_completed(self) -> bool:
         """Boolean indication initial test collection is complete.
 
         This is a boolean indicating all initial participating nodes
         have finished collection.  The required number of initial
         nodes is defined by ``.numnodes``.
         """
         return len(self.node2collection) >= self.numnodes
 
     @property
-    def tests_finished(self):
+    def tests_finished(self) -> bool:
         """Return True if all tests have been executed by the nodes."""
         if not self.collection_is_completed:
             return False
         if self.pending:
             return False
         for pending in self.node2pending.values():
             if len(pending) >= 2:
                 return False
         return True
 
     @property
-    def has_pending(self):
-        """Return True if there are pending test items
+    def has_pending(self) -> bool:
+        """Return True if there are pending test items.
 
         This indicates that collection has finished and nodes are
         still processing test items, so this can be thought of as
         "the scheduler is active".
         """
         if self.pending:
             return True
         for pending in self.node2pending.values():
             if pending:
                 return True
         return False
 
-    def add_node(self, node):
+    def add_node(self, node: WorkerController) -> None:
         """Add a new node to the scheduler.
 
         From now on the node will be allocated chunks of tests to
         execute.
 
         Called by the ``DSession.worker_workerready`` hook when it
         successfully bootstraps a new node.
         """
         assert node not in self.node2pending
         self.node2pending[node] = []
 
-    def add_node_collection(self, node, collection):
-        """Add the collected test items from a node
+    def add_node_collection(
+        self, node: WorkerController, collection: Sequence[str]
+    ) -> None:
+        """Add the collected test items from a node.
 
         The collection is stored in the ``.node2collection`` map.
         Called by the ``DSession.worker_collectionfinish`` hook.
         """
         assert node in self.node2pending
         if self.collection_is_completed:
             # A new node has been added later, perhaps an original one died.
@@ -137,35 +143,45 @@
                 msg = report_collection_diff(
                     self.collection, collection, other_node.gateway.id, node.gateway.id
                 )
                 self.log(msg)
                 return
         self.node2collection[node] = list(collection)
 
-    def mark_test_complete(self, node, item_index, duration=0):
-        """Mark test item as completed by node
+    def mark_test_complete(
+        self, node: WorkerController, item_index: int, duration: float = 0
+    ) -> None:
+        """Mark test item as completed by node.
 
         The duration it took to execute the item is used as a hint to
         the scheduler.
 
         This is called by the ``DSession.worker_testreport`` hook.
         """
         self.node2pending[node].remove(item_index)
         self.check_schedule(node, duration=duration)
 
-    def mark_test_pending(self, item):
+    def mark_test_pending(self, item: str) -> None:
+        assert self.collection is not None
         self.pending.insert(
             0,
             self.collection.index(item),
         )
         for node in self.node2pending:
             self.check_schedule(node)
 
-    def check_schedule(self, node, duration=0):
-        """Maybe schedule new items on the node
+    def remove_pending_tests_from_node(
+        self,
+        node: WorkerController,
+        indices: Sequence[int],
+    ) -> None:
+        raise NotImplementedError()
+
+    def check_schedule(self, node: WorkerController, duration: float = 0) -> None:
+        """Maybe schedule new items on the node.
 
         If there are any globally pending nodes left then this will
         check if the given node should be given any more tests.  The
         ``duration`` of the last test is optionally used as a
         heuristic to influence how many tests the node is assigned.
         """
         if node.shutting_down:
@@ -190,40 +206,41 @@
                 maxschedchunk = max(2 - len(node_pending), self.maxschedchunk)
                 self._send_tests(node, min(num_send, maxschedchunk))
         else:
             node.shutdown()
 
         self.log("num items waiting for node:", len(self.pending))
 
-    def remove_node(self, node):
-        """Remove a node from the scheduler
+    def remove_node(self, node: WorkerController) -> str | None:
+        """Remove a node from the scheduler.
 
         This should be called either when the node crashed or at
         shutdown time.  In the former case any pending items assigned
         to the node will be re-scheduled.  Called by the
         ``DSession.worker_workerfinished`` and
         ``DSession.worker_errordown`` hooks.
 
         Return the item which was being executing while the node
         crashed or None if the node has no more pending items.
 
         """
         pending = self.node2pending.pop(node)
         if not pending:
-            return
+            return None
 
         # The node crashed, reassing pending items
+        assert self.collection is not None
         crashitem = self.collection[pending.pop(0)]
         self.pending.extend(pending)
         for node in self.node2pending:
             self.check_schedule(node)
         return crashitem
 
-    def schedule(self):
-        """Initiate distribution of the test collection
+    def schedule(self) -> None:
+        """Initiate distribution of the test collection.
 
         Initiate scheduling of the items across the nodes.  If this
         gets called again later it behaves the same as calling
         ``.check_schedule()`` on all nodes so that newly added nodes
         will start to be used.
 
         This is called by the ``DSession.worker_collectionfinish`` hook
@@ -239,15 +256,15 @@
 
         # XXX allow nodes to have different collections
         if not self._check_nodes_have_same_collection():
             self.log("**Different tests collected, aborting run**")
             return
 
         # Collections are identical, create the index of pending items.
-        self.collection = list(self.node2collection.values())[0]
+        self.collection = next(iter(self.node2collection.values()))
         self.pending[:] = range(len(self.collection))
         if not self.collection:
             return
 
         if self.maxschedchunk is None:
             self.maxschedchunk = len(self.collection)
 
@@ -256,15 +273,15 @@
         # shutdown signals and get all nodes working.
         if len(self.pending) < 2 * len(self.nodes):
             # Distribute tests round-robin. Try to load all nodes if there are
             # enough tests. The other branch tries sends at least 2 tests
             # to each node - which is suboptimal when you have less than
             # 2 * len(nodes) tests.
             nodes = cycle(self.nodes)
-            for i in range(len(self.pending)):
+            for _ in range(len(self.pending)):
                 self._send_tests(next(nodes), 1)
         else:
             # Send batches of consecutive tests. By default, pytest sorts tests
             # in order for optimal single-threaded execution, minimizing the
             # number of necessary fixture setup/teardown. Try to keep that
             # optimal order for every worker.
 
@@ -278,22 +295,22 @@
                 self._send_tests(node, node_chunksize)
 
         if not self.pending:
             # initial distribution sent all tests, start node shutdown
             for node in self.nodes:
                 node.shutdown()
 
-    def _send_tests(self, node, num):
+    def _send_tests(self, node: WorkerController, num: int) -> None:
         tests_per_node = self.pending[:num]
         if tests_per_node:
             del self.pending[:num]
             self.node2pending[node].extend(tests_per_node)
             node.send_runtest_some(tests_per_node)
 
-    def _check_nodes_have_same_collection(self):
+    def _check_nodes_have_same_collection(self) -> bool:
         """Return True if all nodes have collected the same items.
 
         If collections differ, this method returns False while logging
         the collection differences and posting collection errors to
         pytest_collectreport hook.
         """
         node_collection_items = list(self.node2collection.items())
@@ -303,13 +320,16 @@
             msg = report_collection_diff(
                 col, collection, first_node.gateway.id, node.gateway.id
             )
             if msg:
                 same_collection = False
                 self.log(msg)
                 if self.config is not None:
-                    rep = CollectReport(
-                        node.gateway.id, "failed", longrepr=msg, result=[]
+                    rep = pytest.CollectReport(
+                        nodeid=node.gateway.id,
+                        outcome="failed",
+                        longrepr=msg,
+                        result=[],
                     )
                     self.config.hook.pytest_collectreport(report=rep)
 
         return same_collection
```

### Comparing `pytest-xdist-3.5.0/src/xdist/scheduler/loadfile.py` & `pytest_xdist-3.6.0/src/xdist/scheduler/loadfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from .loadscope import LoadScopeScheduling
+from __future__ import annotations
+
+import pytest
+
 from xdist.remote import Producer
 
+from .loadscope import LoadScopeScheduling
+
 
 class LoadFileScheduling(LoadScopeScheduling):
     """Implement load scheduling across nodes, but grouping test test file.
 
     This distributes the tests collected across all nodes so each test is run
     just once.  All nodes collect and submit the list of tests and when all
     collections are received it is verified they are identical collections.
@@ -16,22 +21,22 @@
 
     When created, ``numnodes`` defines how many nodes are expected to submit a
     collection. This is used to know when all nodes have finished collection.
 
     This class behaves very much like LoadScopeScheduling, but with a file-level scope.
     """
 
-    def __init__(self, config, log=None):
+    def __init__(self, config: pytest.Config, log: Producer | None = None) -> None:
         super().__init__(config, log)
         if log is None:
             self.log = Producer("loadfilesched")
         else:
             self.log = log.loadfilesched
 
-    def _split_scope(self, nodeid):
+    def _split_scope(self, nodeid: str) -> str:
         """Determine the scope (grouping) of a nodeid.
 
         There are usually 3 cases for a nodeid::
 
             example/loadsuite/test/test_beta.py::test_beta0
             example/loadsuite/test/test_delta.py::Delta1::test_delta0
             example/loadsuite/epsilon/__init__.py::epsilon.epsilon
@@ -39,14 +44,17 @@
         #. Function in a test module.
         #. Method of a class in a test module.
         #. Doctest in a function in a package.
 
         This function will group tests with the scope determined by splitting
         the first ``::`` from the left. That is, test will be grouped in a
         single work unit when they reside in the same file.
-         In the above example, scopes will be::
+
+        In the above example, scopes will be::
+
+        .. code-block:: text
 
             example/loadsuite/test/test_beta.py
             example/loadsuite/test/test_delta.py
             example/loadsuite/epsilon/__init__.py
         """
         return nodeid.split("::", 1)[0]
```

### Comparing `pytest-xdist-3.5.0/src/xdist/scheduler/loadgroup.py` & `pytest_xdist-3.6.0/src/xdist/scheduler/loadgroup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from .loadscope import LoadScopeScheduling
+from __future__ import annotations
+
+import pytest
+
 from xdist.remote import Producer
 
+from .loadscope import LoadScopeScheduling
+
 
 class LoadGroupScheduling(LoadScopeScheduling):
     """Implement load scheduling across nodes, but grouping test by xdist_group mark.
 
     This class behaves very much like LoadScopeScheduling, but it groups tests by xdist_group mark
     instead of the module or class to which they belong to.
     """
 
-    def __init__(self, config, log=None):
+    def __init__(self, config: pytest.Config, log: Producer | None = None) -> None:
         super().__init__(config, log)
         if log is None:
             self.log = Producer("loadgroupsched")
         else:
             self.log = log.loadgroupsched
 
-    def _split_scope(self, nodeid):
+    def _split_scope(self, nodeid: str) -> str:
         """Determine the scope (grouping) of a nodeid.
 
         There are usually 3 cases for a nodeid::
 
             example/loadsuite/test/test_beta.py::test_beta0
             example/loadsuite/test/test_delta.py::Delta1::test_delta0
             example/loadsuite/epsilon/__init__.py::epsilon.epsilon
```

### Comparing `pytest-xdist-3.5.0/src/xdist/scheduler/loadscope.py` & `pytest_xdist-3.6.0/src/xdist/scheduler/loadscope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
 from collections import OrderedDict
+from typing import NoReturn
+from typing import Sequence
+
+import pytest
 
-from _pytest.runner import CollectReport
 from xdist.remote import Producer
 from xdist.report import report_collection_diff
 from xdist.workermanage import parse_spec_config
+from xdist.workermanage import WorkerController
 
 
 class LoadScopeScheduling:
     """Implement load scheduling across nodes, but grouping test by scope.
 
     This distributes the tests collected across all nodes so each test is run
     just once.  All nodes collect and submit the list of tests and when all
@@ -17,15 +23,15 @@
     item, it calls ``.mark_test_complete()`` which will trigger the scheduler
     to assign more work units if the number of pending tests for the node falls
     below a low-watermark.
 
     When created, ``numnodes`` defines how many nodes are expected to submit a
     collection. This is used to know when all nodes have finished collection.
 
-    Attributes:
+    Attributes::
 
     :numnodes: The expected number of nodes taking part.  The actual number of
        nodes will vary during the scheduler's lifetime as nodes are added by
        the DSession as they are brought up and removed either because of a dead
        node or normal shutdown.  This number is primarily used to know when the
        initial collection is completed.
 
@@ -80,61 +86,61 @@
             }
 
     :log: A py.log.Producer instance.
 
     :config: Config object, used for handling hooks.
     """
 
-    def __init__(self, config, log=None):
+    def __init__(self, config: pytest.Config, log: Producer | None = None) -> None:
         self.numnodes = len(parse_spec_config(config))
-        self.collection = None
+        self.collection: list[str] | None = None
 
-        self.workqueue = OrderedDict()
-        self.assigned_work = OrderedDict()
-        self.registered_collections = OrderedDict()
+        self.workqueue: OrderedDict[str, dict[str, bool]] = OrderedDict()
+        self.assigned_work: dict[WorkerController, dict[str, dict[str, bool]]] = {}
+        self.registered_collections: dict[WorkerController, list[str]] = {}
 
         if log is None:
             self.log = Producer("loadscopesched")
         else:
             self.log = log.loadscopesched
 
         self.config = config
 
     @property
-    def nodes(self):
+    def nodes(self) -> list[WorkerController]:
         """A list of all active nodes in the scheduler."""
         return list(self.assigned_work.keys())
 
     @property
-    def collection_is_completed(self):
+    def collection_is_completed(self) -> bool:
         """Boolean indication initial test collection is complete.
 
         This is a boolean indicating all initial participating nodes have
         finished collection.  The required number of initial nodes is defined
         by ``.numnodes``.
         """
         return len(self.registered_collections) >= self.numnodes
 
     @property
-    def tests_finished(self):
+    def tests_finished(self) -> bool:
         """Return True if all tests have been executed by the nodes."""
         if not self.collection_is_completed:
             return False
 
         if self.workqueue:
             return False
 
         for assigned_unit in self.assigned_work.values():
             if self._pending_of(assigned_unit) >= 2:
                 return False
 
         return True
 
     @property
-    def has_pending(self):
+    def has_pending(self) -> bool:
         """Return True if there are pending test items.
 
         This indicates that collection has finished and nodes are still
         processing test items, so this can be thought of as
         "the scheduler is active".
         """
         if self.workqueue:
@@ -142,26 +148,26 @@
 
         for assigned_unit in self.assigned_work.values():
             if self._pending_of(assigned_unit) > 0:
                 return True
 
         return False
 
-    def add_node(self, node):
+    def add_node(self, node: WorkerController) -> None:
         """Add a new node to the scheduler.
 
         From now on the node will be assigned work units to be executed.
 
         Called by the ``DSession.worker_workerready`` hook when it successfully
         bootstraps a new node.
         """
         assert node not in self.assigned_work
-        self.assigned_work[node] = OrderedDict()
+        self.assigned_work[node] = {}
 
-    def remove_node(self, node):
+    def remove_node(self, node: WorkerController) -> str | None:
         """Remove a node from the scheduler.
 
         This should be called either when the node crashed or at shutdown time.
         In the former case any pending items assigned to the node will be
         re-scheduled.
 
         Called by the hooks:
@@ -194,24 +200,25 @@
         self.workqueue.update(workload)
 
         for node in self.assigned_work:
             self._reschedule(node)
 
         return crashitem
 
-    def add_node_collection(self, node, collection):
+    def add_node_collection(
+        self, node: WorkerController, collection: Sequence[str]
+    ) -> None:
         """Add the collected test items from a node.
 
         The collection is stored in the ``.registered_collections`` dictionary.
 
         Called by the hook:
 
         - ``DSession.worker_collectionfinish``.
         """
-
         # Check that add_node() was called on the node before
         assert node in self.assigned_work
 
         # A new node has been added later, perhaps an original one died.
         if self.collection_is_completed:
             # Assert that .schedule() should have been called by now
             assert self.collection
@@ -224,52 +231,61 @@
                     self.collection, collection, other_node.gateway.id, node.gateway.id
                 )
                 self.log(msg)
                 return
 
         self.registered_collections[node] = list(collection)
 
-    def mark_test_complete(self, node, item_index, duration=0):
+    def mark_test_complete(
+        self, node: WorkerController, item_index: int, duration: float = 0
+    ) -> None:
         """Mark test item as completed by node.
 
         Called by the hook:
 
         - ``DSession.worker_testreport``.
         """
         nodeid = self.registered_collections[node][item_index]
         scope = self._split_scope(nodeid)
 
         self.assigned_work[node][scope][nodeid] = True
         self._reschedule(node)
 
-    def mark_test_pending(self, item):
+    def mark_test_pending(self, item: str) -> NoReturn:
+        raise NotImplementedError()
+
+    def remove_pending_tests_from_node(
+        self,
+        node: WorkerController,
+        indices: Sequence[int],
+    ) -> None:
         raise NotImplementedError()
 
-    def _assign_work_unit(self, node):
+    def _assign_work_unit(self, node: WorkerController) -> None:
         """Assign a work unit to a node."""
         assert self.workqueue
 
         # Grab a unit of work
         scope, work_unit = self.workqueue.popitem(last=False)
 
         # Keep track of the assigned work
-        assigned_to_node = self.assigned_work.setdefault(node, default=OrderedDict())
+        assigned_to_node = self.assigned_work.setdefault(node, {})
         assigned_to_node[scope] = work_unit
 
         # Ask the node to execute the workload
         worker_collection = self.registered_collections[node]
         nodeids_indexes = [
             worker_collection.index(nodeid)
             for nodeid, completed in work_unit.items()
             if not completed
         ]
 
         node.send_runtest_some(nodeids_indexes)
 
-    def _split_scope(self, nodeid):
+    def _split_scope(self, nodeid: str) -> str:
         """Determine the scope (grouping) of a nodeid.
 
         There are usually 3 cases for a nodeid::
 
             example/loadsuite/test/test_beta.py::test_beta0
             example/loadsuite/test/test_delta.py::Delta1::test_delta0
             example/loadsuite/epsilon/__init__.py::epsilon.epsilon
@@ -285,26 +301,25 @@
 
             example/loadsuite/test/test_beta.py
             example/loadsuite/test/test_delta.py::Delta1
             example/loadsuite/epsilon/__init__.py
         """
         return nodeid.rsplit("::", 1)[0]
 
-    def _pending_of(self, workload):
+    def _pending_of(self, workload: dict[str, dict[str, bool]]) -> int:
         """Return the number of pending tests in a workload."""
         pending = sum(list(scope.values()).count(False) for scope in workload.values())
         return pending
 
-    def _reschedule(self, node):
+    def _reschedule(self, node: WorkerController) -> None:
         """Maybe schedule new items on the node.
 
         If there are any globally pending work units left then this will check
         if the given node should be given any more tests.
         """
-
         # Do not add more work to a node shutting down
         if node.shutting_down:
             return
 
         # Check that more work is available
         if not self.workqueue:
             node.shutdown()
@@ -316,15 +331,15 @@
         # 2: Heuristic of minimum tests to enqueue more work
         if self._pending_of(self.assigned_work[node]) > 2:
             return
 
         # Pop one unit of work and assign it
         self._assign_work_unit(node)
 
-    def schedule(self):
+    def schedule(self) -> None:
         """Initiate distribution of the test collection.
 
         Initiate scheduling of the items across the nodes.  If this gets called
         again later it behaves the same as calling ``._reschedule()`` on all
         nodes so that newly added nodes will start to be used.
 
         If ``.collection_is_completed`` is True, this is called by the hook:
@@ -346,18 +361,18 @@
 
         # Collections are identical, create the final list of items
         self.collection = list(next(iter(self.registered_collections.values())))
         if not self.collection:
             return
 
         # Determine chunks of work (scopes)
-        unsorted_workqueue = OrderedDict()
+        unsorted_workqueue: dict[str, dict[str, bool]] = {}
         for nodeid in self.collection:
             scope = self._split_scope(nodeid)
-            work_unit = unsorted_workqueue.setdefault(scope, default=OrderedDict())
+            work_unit = unsorted_workqueue.setdefault(scope, {})
             work_unit[nodeid] = False
 
         # Insert tests scopes into work queue ordered by number of tests.
         for scope, nodeids in sorted(
             unsorted_workqueue.items(), key=lambda item: -len(item[1])
         ):
             self.workqueue[scope] = nodeids
@@ -365,15 +380,15 @@
         # Avoid having more workers than work
         extra_nodes = len(self.nodes) - len(self.workqueue)
 
         if extra_nodes > 0:
             self.log(f"Shutting down {extra_nodes} nodes")
 
             for _ in range(extra_nodes):
-                unused_node, assigned = self.assigned_work.popitem(last=True)
+                unused_node, assigned = self.assigned_work.popitem()
 
                 self.log(f"Shutting down unused node {unused_node}")
                 unused_node.shutdown()
 
         # Assign initial workload
         for node in self.nodes:
             self._assign_work_unit(node)
@@ -383,15 +398,15 @@
             self._reschedule(node)
 
         # Initial distribution sent all tests, start node shutdown
         if not self.workqueue:
             for node in self.nodes:
                 node.shutdown()
 
-    def _check_nodes_have_same_collection(self):
+    def _check_nodes_have_same_collection(self) -> bool:
         """Return True if all nodes have collected the same items.
 
         If collections differ, this method returns False while logging
         the collection differences and posting collection errors to
         pytest_collectreport hook.
         """
         node_collection_items = list(self.registered_collections.items())
@@ -404,14 +419,16 @@
             )
             if not msg:
                 continue
 
             same_collection = False
             self.log(msg)
 
-            if self.config is None:
-                continue
-
-            rep = CollectReport(node.gateway.id, "failed", longrepr=msg, result=[])
+            rep = pytest.CollectReport(
+                nodeid=node.gateway.id,
+                outcome="failed",
+                longrepr=msg,
+                result=[],
+            )
             self.config.hook.pytest_collectreport(report=rep)
 
         return same_collection
```

### Comparing `pytest-xdist-3.5.0/src/xdist/scheduler/worksteal.py` & `pytest_xdist-3.6.0/src/xdist/scheduler/worksteal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-from collections import namedtuple
+from __future__ import annotations
 
-from _pytest.runner import CollectReport
+from typing import NamedTuple
+from typing import Sequence
+
+import pytest
 
 from xdist.remote import Producer
-from xdist.workermanage import parse_spec_config
 from xdist.report import report_collection_diff
+from xdist.workermanage import parse_spec_config
+from xdist.workermanage import WorkerController
 
 
-NodePending = namedtuple("NodePending", ["node", "pending"])
+class NodePending(NamedTuple):
+    node: WorkerController
+    pending: list[int]
+
 
 # Every worker needs at least 2 tests in queue - the current and the next one.
 MIN_PENDING = 2
 
 
 class WorkStealingScheduling:
     """Implement work-stealing scheduling.
 
     Initially, tests are distributed evenly among all nodes.
 
     When some node completes most of its assigned tests (when only one pending
     test remains), an attempt is made to reassign ("steal") some tests from
     other nodes to this node.
 
-    Attributes:
+    Attributes::
 
     :numnodes: The expected number of nodes taking part.  The actual
        number of nodes will vary during the scheduler's lifetime as
        nodes are added by the DSession as they are brought up and
        removed either because of a dead node or normal shutdown.  This
        number is primarily used to know when the initial collection is
        completed.
@@ -53,85 +60,87 @@
 
     :steal_requested_from_node: The node to which the current "steal" request
        was sent. ``None`` if there is no request in progress. Only one request
        can be in progress at any time, the scheduler doesn't send multiple
        simultaneous requests.
     """
 
-    def __init__(self, config, log=None):
+    def __init__(self, config: pytest.Config, log: Producer | None = None) -> None:
         self.numnodes = len(parse_spec_config(config))
-        self.node2collection = {}
-        self.node2pending = {}
-        self.pending = []
-        self.collection = None
+        self.node2collection: dict[WorkerController, list[str]] = {}
+        self.node2pending: dict[WorkerController, list[int]] = {}
+        self.pending: list[int] = []
+        self.collection: list[str] | None = None
         if log is None:
             self.log = Producer("workstealsched")
         else:
             self.log = log.workstealsched
         self.config = config
-        self.steal_requested_from_node = None
+        self.steal_requested_from_node: WorkerController | None = None
 
     @property
-    def nodes(self):
+    def nodes(self) -> list[WorkerController]:
         """A list of all nodes in the scheduler."""
         return list(self.node2pending.keys())
 
     @property
-    def collection_is_completed(self):
+    def collection_is_completed(self) -> bool:
         """Boolean indication initial test collection is complete.
 
         This is a boolean indicating all initial participating nodes
         have finished collection.  The required number of initial
         nodes is defined by ``.numnodes``.
         """
         return len(self.node2collection) >= self.numnodes
 
     @property
-    def tests_finished(self):
+    def tests_finished(self) -> bool:
         """Return True if all tests have been executed by the nodes."""
         if not self.collection_is_completed:
             return False
         if self.pending:
             return False
         if self.steal_requested_from_node is not None:
             return False
         for pending in self.node2pending.values():
             if len(pending) >= MIN_PENDING:
                 return False
         return True
 
     @property
-    def has_pending(self):
-        """Return True if there are pending test items
+    def has_pending(self) -> bool:
+        """Return True if there are pending test items.
 
         This indicates that collection has finished and nodes are
         still processing test items, so this can be thought of as
         "the scheduler is active".
         """
         if self.pending:
             return True
         for pending in self.node2pending.values():
             if pending:
                 return True
         return False
 
-    def add_node(self, node):
+    def add_node(self, node: WorkerController) -> None:
         """Add a new node to the scheduler.
 
         From now on the node will be allocated chunks of tests to
         execute.
 
         Called by the ``DSession.worker_workerready`` hook when it
         successfully bootstraps a new node.
         """
         assert node not in self.node2pending
         self.node2pending[node] = []
 
-    def add_node_collection(self, node, collection):
-        """Add the collected test items from a node
+    def add_node_collection(
+        self, node: WorkerController, collection: Sequence[str]
+    ) -> None:
+        """Add the collected test items from a node.
 
         The collection is stored in the ``.node2collection`` map.
         Called by the ``DSession.worker_collectionfinish`` hook.
         """
         assert node in self.node2pending
         if self.collection_is_completed:
             # A new node has been added later, perhaps an original one died.
@@ -143,53 +152,60 @@
                 msg = report_collection_diff(
                     self.collection, collection, other_node.gateway.id, node.gateway.id
                 )
                 self.log(msg)
                 return
         self.node2collection[node] = list(collection)
 
-    def mark_test_complete(self, node, item_index, duration=None):
-        """Mark test item as completed by node
+    def mark_test_complete(
+        self, node: WorkerController, item_index: int, duration: float | None = None
+    ) -> None:
+        """Mark test item as completed by node.
 
         This is called by the ``DSession.worker_testreport`` hook.
         """
         self.node2pending[node].remove(item_index)
         self.check_schedule()
 
-    def mark_test_pending(self, item):
+    def mark_test_pending(self, item: str) -> None:
+        assert self.collection is not None
         self.pending.insert(
             0,
             self.collection.index(item),
         )
         self.check_schedule()
 
-    def remove_pending_tests_from_node(self, node, indices):
+    def remove_pending_tests_from_node(
+        self,
+        node: WorkerController,
+        indices: Sequence[int],
+    ) -> None:
         """Node returned some test indices back in response to 'steal' command.
 
         This is called by ``DSession.worker_unscheduled``.
         """
         assert node is self.steal_requested_from_node
         self.steal_requested_from_node = None
 
         indices_set = set(indices)
         self.node2pending[node] = [
             i for i in self.node2pending[node] if i not in indices_set
         ]
         self.pending.extend(indices)
         self.check_schedule()
 
-    def check_schedule(self):
+    def check_schedule(self) -> None:
         """Reschedule tests/perform load balancing."""
         nodes_up = [
             NodePending(node, pending)
             for node, pending in self.node2pending.items()
             if not node.shutting_down
         ]
 
-        def get_idle_nodes():
+        def get_idle_nodes() -> list[WorkerController]:
             return [node for node, pending in nodes_up if len(pending) < MIN_PENDING]
 
         idle_nodes = get_idle_nodes()
         if not idle_nodes:
             return
 
         if self.pending:
@@ -225,49 +241,50 @@
         if num_steal == 0:
             # Can't get more work - shutdown idle nodes. This will force them
             # to run the last test now instead of waiting for more tests.
             for node in idle_nodes:
                 node.shutdown()
             return
 
+        assert steal_from is not None
         steal_from.node.send_steal(steal_from.pending[-num_steal:])
         self.steal_requested_from_node = steal_from.node
 
-    def remove_node(self, node):
-        """Remove a node from the scheduler
+    def remove_node(self, node: WorkerController) -> str | None:
+        """Remove a node from the scheduler.
 
         This should be called either when the node crashed or at
         shutdown time.  In the former case any pending items assigned
         to the node will be re-scheduled.  Called by the
         ``DSession.worker_workerfinished`` and
         ``DSession.worker_errordown`` hooks.
 
         Return the item which was being executing while the node
         crashed or None if the node has no more pending items.
-
         """
         pending = self.node2pending.pop(node)
 
         # If node was removed without completing its assigned tests - it crashed
         if pending:
+            assert self.collection is not None
             crashitem = self.collection[pending.pop(0)]
         else:
             crashitem = None
 
         self.pending.extend(pending)
 
         # Dead node won't respond to "steal" request
         if self.steal_requested_from_node is node:
             self.steal_requested_from_node = None
 
         self.check_schedule()
         return crashitem
 
-    def schedule(self):
-        """Initiate distribution of the test collection
+    def schedule(self) -> None:
+        """Initiate distribution of the test collection.
 
         Initiate scheduling of the items across the nodes.  If this
         gets called again later it behaves the same as calling
         ``.check_schedule()`` on all nodes so that newly added nodes
         will start to be used.
 
         This is called by the ``DSession.worker_collectionfinish`` hook
@@ -281,29 +298,29 @@
             return
 
         if not self._check_nodes_have_same_collection():
             self.log("**Different tests collected, aborting run**")
             return
 
         # Collections are identical, create the index of pending items.
-        self.collection = list(self.node2collection.values())[0]
+        self.collection = next(iter(self.node2collection.values()))
         self.pending[:] = range(len(self.collection))
         if not self.collection:
             return
 
         self.check_schedule()
 
-    def _send_tests(self, node, num):
+    def _send_tests(self, node: WorkerController, num: int) -> None:
         tests_per_node = self.pending[:num]
         if tests_per_node:
             del self.pending[:num]
             self.node2pending[node].extend(tests_per_node)
             node.send_runtest_some(tests_per_node)
 
-    def _check_nodes_have_same_collection(self):
+    def _check_nodes_have_same_collection(self) -> bool:
         """Return True if all nodes have collected the same items.
 
         If collections differ, this method returns False while logging
         the collection differences and posting collection errors to
         pytest_collectreport hook.
         """
         node_collection_items = list(self.node2collection.items())
@@ -313,13 +330,16 @@
             msg = report_collection_diff(
                 col, collection, first_node.gateway.id, node.gateway.id
             )
             if msg:
                 same_collection = False
                 self.log(msg)
                 if self.config is not None:
-                    rep = CollectReport(
-                        node.gateway.id, "failed", longrepr=msg, result=[]
+                    rep = pytest.CollectReport(
+                        nodeid=node.gateway.id,
+                        outcome="failed",
+                        longrepr=msg,
+                        result=[],
                     )
                     self.config.hook.pytest_collectreport(report=rep)
 
         return same_collection
```

### Comparing `pytest-xdist-3.5.0/src/xdist/workermanage.py` & `pytest_xdist-3.6.0/src/xdist/workermanage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,36 @@
+from __future__ import annotations
+
+import enum
 import fnmatch
 import os
+from pathlib import Path
 import re
 import sys
+from typing import Any
+from typing import Callable
+from typing import Literal
+from typing import Sequence
+from typing import Union
 import uuid
-from pathlib import Path
-from typing import List, Union, Sequence, Optional, Any, Tuple, Set
+import warnings
 
-import pytest
 import execnet
+import pytest
 
+from xdist.plugin import _sys_path
 import xdist.remote
 from xdist.remote import Producer
-from xdist.plugin import _sys_path
+from xdist.remote import WorkerInfo
 
 
-def parse_spec_config(config):
+def parse_spec_config(config: pytest.Config) -> list[str]:
     xspeclist = []
-    for xspec in config.getvalue("tx"):
+    tx: list[str] = config.getvalue("tx")
+    for xspec in tx:
         i = xspec.find("*")
         try:
             num = int(xspec[:i])
         except ValueError:
             xspeclist.append(xspec)
         else:
             xspeclist.extend([xspec[i + 1 :]] * num)
@@ -31,72 +41,89 @@
     return xspeclist
 
 
 class NodeManager:
     EXIT_TIMEOUT = 10
     DEFAULT_IGNORES = [".*", "*.pyc", "*.pyo", "*~"]
 
-    def __init__(self, config, specs=None, defaultchdir="pyexecnetcache") -> None:
+    def __init__(
+        self,
+        config: pytest.Config,
+        specs: Sequence[execnet.XSpec | str] | None = None,
+        defaultchdir: str = "pyexecnetcache",
+    ) -> None:
         self.config = config
         self.trace = self.config.trace.get("nodemanager")
         self.testrunuid = self.config.getoption("testrunuid")
         if self.testrunuid is None:
             self.testrunuid = uuid.uuid4().hex
-        self.group = execnet.Group()
+        self.group = execnet.Group(execmodel="main_thread_only")
         if specs is None:
             specs = self._getxspecs()
-        self.specs = []
+        self.specs: list[execnet.XSpec] = []
         for spec in specs:
             if not isinstance(spec, execnet.XSpec):
                 spec = execnet.XSpec(spec)
+            if getattr(spec, "execmodel", None) != "main_thread_only":
+                spec = execnet.XSpec(f"execmodel=main_thread_only//{spec}")
             if not spec.chdir and not spec.popen:
                 spec.chdir = defaultchdir
             self.group.allocate_id(spec)
             self.specs.append(spec)
         self.roots = self._getrsyncdirs()
         self.rsyncoptions = self._getrsyncoptions()
-        self._rsynced_specs: Set[Tuple[Any, Any]] = set()
+        self._rsynced_specs: set[tuple[Any, Any]] = set()
 
-    def rsync_roots(self, gateway):
+    def rsync_roots(self, gateway: execnet.Gateway) -> None:
         """Rsync the set of roots to the node's gateway cwd."""
         if self.roots:
             for root in self.roots:
                 self.rsync(gateway, root, **self.rsyncoptions)
 
-    def setup_nodes(self, putevent):
+    def setup_nodes(
+        self,
+        putevent: Callable[[tuple[str, dict[str, Any]]], None],
+    ) -> list[WorkerController]:
         self.config.hook.pytest_xdist_setupnodes(config=self.config, specs=self.specs)
         self.trace("setting up nodes")
         return [self.setup_node(spec, putevent) for spec in self.specs]
 
-    def setup_node(self, spec, putevent):
+    def setup_node(
+        self,
+        spec: execnet.XSpec,
+        putevent: Callable[[tuple[str, dict[str, Any]]], None],
+    ) -> WorkerController:
+        if getattr(spec, "execmodel", None) != "main_thread_only":
+            spec = execnet.XSpec(f"execmodel=main_thread_only//{spec}")
         gw = self.group.makegateway(spec)
         self.config.hook.pytest_xdist_newgateway(gateway=gw)
         self.rsync_roots(gw)
         node = WorkerController(self, gw, self.config, putevent)
-        gw.node = node  # keep the node alive
+        # Keep the node alive.
+        gw.node = node  # type: ignore[attr-defined]
         node.setup()
         self.trace("started node %r" % node)
         return node
 
-    def teardown_nodes(self):
+    def teardown_nodes(self) -> None:
         self.group.terminate(self.EXIT_TIMEOUT)
 
-    def _getxspecs(self):
+    def _getxspecs(self) -> list[execnet.XSpec]:
         return [execnet.XSpec(x) for x in parse_spec_config(self.config)]
 
-    def _getrsyncdirs(self) -> List[Path]:
+    def _getrsyncdirs(self) -> list[Path]:
         for spec in self.specs:
             if not spec.popen or spec.chdir:
                 break
         else:
             return []
-        import pytest
         import _pytest
+        import pytest
 
-        def get_dir(p):
+        def get_dir(p: str) -> str:
             """Return the directory path if p is a package or the path to the .py file otherwise."""
             stripped = p.rstrip("co")
             if os.path.basename(stripped) == "__init__.py":
                 return os.path.dirname(p)
             else:
                 return stripped
 
@@ -106,137 +133,165 @@
         candidates = [pytestpath, pytestdir]
         candidates += config.option.rsyncdir
         rsyncroots = config.getini("rsyncdirs")
         if rsyncroots:
             candidates.extend(rsyncroots)
         roots = []
         for root in candidates:
-            root = Path(root).resolve()
-            if not root.exists():
+            root_path = Path(root).resolve()
+            if not root_path.exists():
                 raise pytest.UsageError(f"rsyncdir doesn't exist: {root!r}")
-            if root not in roots:
-                roots.append(root)
+            if root_path not in roots:
+                roots.append(root_path)
         return roots
 
-    def _getrsyncoptions(self):
+    def _getrsyncoptions(self) -> dict[str, Any]:
         """Get options to be passed for rsync."""
         ignores = list(self.DEFAULT_IGNORES)
         ignores += [str(path) for path in self.config.option.rsyncignore]
         ignores += [str(path) for path in self.config.getini("rsyncignore")]
 
         return {
             "ignores": ignores,
             "verbose": getattr(self.config.option, "verbose", 0),
         }
 
-    def rsync(self, gateway, source, notify=None, verbose=False, ignores=None):
+    def rsync(
+        self,
+        gateway: execnet.Gateway,
+        source: str | os.PathLike[str],
+        notify: (
+            Callable[[str, execnet.XSpec, str | os.PathLike[str]], Any] | None
+        ) = None,
+        verbose: int = False,
+        ignores: Sequence[str] | None = None,
+    ) -> None:
         """Perform rsync to remote hosts for node."""
         # XXX This changes the calling behaviour of
         #     pytest_xdist_rsyncstart and pytest_xdist_rsyncfinish to
         #     be called once per rsync target.
-        rsync = HostRSync(source, verbose=verbose, ignores=ignores)
+        rsync = HostRSync(source, verbose=verbose > 0, ignores=ignores)
         spec = gateway.spec
         if spec.popen and not spec.chdir:
             # XXX This assumes that sources are python-packages
             #     and that adding the basedir does not hurt.
             gateway.remote_exec(
                 """
                 import sys ; sys.path.insert(0, %r)
             """
                 % os.path.dirname(str(source))
             ).waitclose()
             return
         if (spec, source) in self._rsynced_specs:
             return
 
-        def finished():
+        def finished() -> None:
             if notify:
                 notify("rsyncrootready", spec, source)
 
         rsync.add_target_host(gateway, finished=finished)
         self._rsynced_specs.add((spec, source))
         self.config.hook.pytest_xdist_rsyncstart(source=source, gateways=[gateway])
         rsync.send()
         self.config.hook.pytest_xdist_rsyncfinish(source=source, gateways=[gateway])
 
 
 class HostRSync(execnet.RSync):
-    """RSyncer that filters out common files"""
+    """RSyncer that filters out common files."""
 
     PathLike = Union[str, "os.PathLike[str]"]
 
     def __init__(
         self,
         sourcedir: PathLike,
         *,
-        ignores: Optional[Sequence[PathLike]] = None,
-        **kwargs: object
+        ignores: Sequence[PathLike] | None = None,
+        verbose: bool = True,
     ) -> None:
         if ignores is None:
             ignores = []
         self._ignores = [re.compile(fnmatch.translate(os.fspath(x))) for x in ignores]
-        super().__init__(sourcedir=Path(sourcedir), **kwargs)
+        super().__init__(sourcedir=Path(sourcedir), verbose=verbose)
 
     def filter(self, path: PathLike) -> bool:
         path = Path(path)
         for cre in self._ignores:
             if cre.match(path.name) or cre.match(str(path)):
                 return False
         else:
             return True
 
-    def add_target_host(self, gateway, finished=None):
+    def add_target_host(
+        self,
+        gateway: execnet.Gateway,
+        finished: Callable[[], None] | None = None,
+    ) -> None:
         remotepath = os.path.basename(self._sourcedir)
         super().add_target(gateway, remotepath, finishedcallback=finished, delete=True)
 
-    def _report_send_file(self, gateway, modified_rel_path):
+    def _report_send_file(
+        self,
+        gateway: execnet.Gateway,  # type: ignore[override]
+        modified_rel_path: str,
+    ) -> None:
         if self._verbose > 0:
             path = os.path.basename(self._sourcedir) + "/" + modified_rel_path
             remotepath = gateway.spec.chdir
             print(f"{gateway.spec}:{remotepath} <= {path}")
 
 
-def make_reltoroot(roots: Sequence[Path], args: List[str]) -> List[str]:
+def make_reltoroot(roots: Sequence[Path], args: list[str]) -> list[str]:
     # XXX introduce/use public API for splitting pytest args
     splitcode = "::"
     result = []
     for arg in args:
         parts = arg.split(splitcode)
         fspath = Path(parts[0])
         try:
             exists = fspath.exists()
         except OSError:
             exists = False
         if not exists:
             result.append(arg)
             continue
         for root in roots:
-            x: Optional[Path]
+            x: Path | None
             try:
                 x = fspath.relative_to(root)
             except ValueError:
                 x = None
             if x or fspath == root:
                 parts[0] = root.name + "/" + str(x)
                 break
         else:
             raise ValueError(f"arg {arg} not relative to an rsync root")
         result.append(splitcode.join(parts))
     return result
 
 
+class Marker(enum.Enum):
+    END = -1
+
+
 class WorkerController:
-    ENDMARK = -1
+    # Set when the worker is ready.
+    workerinfo: WorkerInfo
 
     class RemoteHook:
         @pytest.hookimpl(trylast=True)
-        def pytest_xdist_getremotemodule(self):
+        def pytest_xdist_getremotemodule(self) -> Any:
             return xdist.remote
 
-    def __init__(self, nodemanager, gateway, config, putevent):
+    def __init__(
+        self,
+        nodemanager: NodeManager,
+        gateway: execnet.Gateway,
+        config: pytest.Config,
+        putevent: Callable[[tuple[str, dict[str, Any]]], None],
+    ) -> None:
         config.pluginmanager.register(self.RemoteHook())
         self.nodemanager = nodemanager
         self.putevent = putevent
         self.gateway = gateway
         self.config = config
         self.workerinput = {
             "workerid": gateway.id,
@@ -244,30 +299,26 @@
             "testrunuid": nodemanager.testrunuid,
             "mainargv": sys.argv,
         }
         self._down = False
         self._shutdown_sent = False
         self.log = Producer(f"workerctl-{gateway.id}", enabled=config.option.debug)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.gateway.id}>"
 
     @property
-    def shutting_down(self):
+    def shutting_down(self) -> bool:
         return self._down or self._shutdown_sent
 
-    def setup(self):
+    def setup(self) -> None:
         self.log("setting up worker session")
         spec = self.gateway.spec
-        if hasattr(self.config, "invocation_params"):
-            args = [str(x) for x in self.config.invocation_params.args or ()]
-            option_dict = {}
-        else:
-            args = self.config.args
-            option_dict = vars(self.config.option)
+        args = [str(x) for x in self.config.invocation_params.args or ()]
+        option_dict = {}
         if not spec.popen or spec.chdir:
             args = make_reltoroot(self.nodemanager.roots, args)
         if spec.popen:
             name = "popen-%s" % self.gateway.id
             if hasattr(self.config, "_tmp_path_factory"):
                 basetemp = self.config._tmp_path_factory.getbasetemp()
                 option_dict["basetemp"] = str(basetemp / name)
@@ -276,65 +327,68 @@
         remote_module = self.config.hook.pytest_xdist_getremotemodule()
         self.channel = self.gateway.remote_exec(remote_module)
         # change sys.path only for remote workers
         # restore sys.path from a frozen copy for local workers
         change_sys_path = _sys_path if self.gateway.spec.popen else None
         self.channel.send((self.workerinput, args, option_dict, change_sys_path))
 
-        if self.putevent:
-            self.channel.setcallback(self.process_from_remote, endmarker=self.ENDMARK)
+        # putevent is only None in a test.
+        if self.putevent:  # type: ignore[truthy-function]
+            self.channel.setcallback(self.process_from_remote, endmarker=Marker.END)
 
-    def ensure_teardown(self):
+    def ensure_teardown(self) -> None:
         if hasattr(self, "channel"):
             if not self.channel.isclosed():
                 self.log("closing", self.channel)
                 self.channel.close()
             # del self.channel
         if hasattr(self, "gateway"):
             self.log("exiting", self.gateway)
             self.gateway.exit()
             # del self.gateway
 
-    def send_runtest_some(self, indices):
+    def send_runtest_some(self, indices: Sequence[int]) -> None:
         self.sendcommand("runtests", indices=indices)
 
-    def send_runtest_all(self):
+    def send_runtest_all(self) -> None:
         self.sendcommand("runtests_all")
 
-    def send_steal(self, indices):
+    def send_steal(self, indices: Sequence[int]) -> None:
         self.sendcommand("steal", indices=indices)
 
-    def shutdown(self):
+    def shutdown(self) -> None:
         if not self._down:
             try:
                 self.sendcommand("shutdown")
             except OSError:
                 pass
             self._shutdown_sent = True
 
-    def sendcommand(self, name, **kwargs):
-        """send a named parametrized command to the other side."""
+    def sendcommand(self, name: str, **kwargs: object) -> None:
+        """Send a named parametrized command to the other side."""
         self.log(f"sending command {name}(**{kwargs})")
         self.channel.send((name, kwargs))
 
-    def notify_inproc(self, eventname, **kwargs):
+    def notify_inproc(self, eventname: str, **kwargs: object) -> None:
         self.log(f"queuing {eventname}(**{kwargs})")
         self.putevent((eventname, kwargs))
 
-    def process_from_remote(self, eventcall):  # noqa too complex
-        """this gets called for each object we receive from
+    def process_from_remote(
+        self, eventcall: tuple[str, dict[str, Any]] | Literal[Marker.END]
+    ) -> None:
+        """This gets called for each object we receive from
         the other side and if the channel closes.
 
         Note that channel callbacks run in the receiver
         thread of execnet gateways - we need to
         avoid raising exceptions or doing heavy work.
         """
         try:
-            if eventcall == self.ENDMARK:
-                err = self.channel._getremoteerror()
+            if eventcall is Marker.END:
+                err: object | None = self.channel._getremoteerror()  # type: ignore[no-untyped-call]
                 if not self._down:
                     if not err or isinstance(err, EOFError):
                         err = "Not properly terminated"  # lost connection?
                     self.notify_inproc("errordown", node=self, error=err)
                     self._down = True
                 return
             eventname, kwargs = eventcall
@@ -368,24 +422,14 @@
                 self.notify_inproc(
                     eventname,
                     message=kwargs["message"],
                     code=kwargs["code"],
                     nodeid=kwargs["nodeid"],
                     fslocation=kwargs["nodeid"],
                 )
-            elif eventname == "warning_captured":
-                warning_message = unserialize_warning_message(
-                    kwargs["warning_message_data"]
-                )
-                self.notify_inproc(
-                    eventname,
-                    warning_message=warning_message,
-                    when=kwargs["when"],
-                    item=kwargs["item"],
-                )
             elif eventname == "warning_recorded":
                 warning_message = unserialize_warning_message(
                     kwargs["warning_message_data"]
                 )
                 self.notify_inproc(
                     eventname,
                     warning_message=warning_message,
@@ -394,26 +438,23 @@
                     location=kwargs["location"],
                 )
             else:
                 raise ValueError(f"unknown event: {eventname}")
         except KeyboardInterrupt:
             # should not land in receiver-thread
             raise
-        except:  # noqa
-            from _pytest._code import ExceptionInfo
-
-            excinfo = ExceptionInfo.from_current()
+        except BaseException:
+            excinfo = pytest.ExceptionInfo.from_current()
             print("!" * 20, excinfo)
             self.config.notify_exception(excinfo)
             self.shutdown()
             self.notify_inproc("errordown", node=self, error=excinfo)
 
 
-def unserialize_warning_message(data):
-    import warnings
+def unserialize_warning_message(data: dict[str, Any]) -> warnings.WarningMessage:
     import importlib
 
     if data["message_module"]:
         mod = importlib.import_module(data["message_module"])
         cls = getattr(mod, data["message_class_name"])
         message = None
         if data["message_args"] is not None:
@@ -443,8 +484,8 @@
     kwargs = {"message": message, "category": category}
     # access private _WARNING_DETAILS because the attributes vary between Python versions
     for attr_name in warnings.WarningMessage._WARNING_DETAILS:  # type: ignore[attr-defined]
         if attr_name in ("message", "category"):
             continue
         kwargs[attr_name] = data[attr_name]
 
-    return warnings.WarningMessage(**kwargs)  # type: ignore[arg-type]
+    return warnings.WarningMessage(**kwargs)
```

### Comparing `pytest-xdist-3.5.0/testing/acceptance_test.py` & `pytest_xdist-3.6.0/testing/acceptance_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import os
 import re
 import shutil
-from typing import Dict
-from typing import List
-from typing import Tuple
+from typing import cast
 
 import pytest
+
 import xdist
 
 
 class TestDistribution:
     def test_n1_pass(self, pytester: pytest.Pytester) -> None:
         p1 = pytester.makepyfile(
             """
@@ -105,20 +106,20 @@
             [
                 "created: 2/2 workers",
                 "*2 failed, 1 passed, 1 skipped*",
             ]
         )
         assert result.ret == 1
 
-    def test_exitfail_waits_for_workers_to_finish(
+    def test_exitfirst_waits_for_workers_to_finish(
         self, pytester: pytest.Pytester
     ) -> None:
         """The DSession waits for workers before exiting early on failure.
 
-        When -x/--exitfail is set, the DSession wait for the workers to finish
+        When -x/--exitfirst is set, the DSession wait for all workers to finish
         before raising an Interrupt exception. This prevents reports from the
         faiing test and other tests from being discarded.
         """
         p1 = pytester.makepyfile(
             """
             import time
 
@@ -134,23 +135,22 @@
                 time.sleep(0.3)
             def test_fail5():
                 time.sleep(0.3)
             def test_fail6():
                 time.sleep(0.3)
         """
         )
+        # Two workers are used
         result = pytester.runpytest(p1, "-x", "-rA", "-v", "-n2")
         assert result.ret == 2
-        result.stdout.re_match_lines([".*Interrupted: stopping.*[12].*"])
-        m = re.search(r"== (\d+) failed, (\d+) passed in ", str(result.stdout))
-        assert m
-        n_failed, n_passed = (int(s) for s in m.groups())
-        assert 1 <= n_failed <= 2
-        assert 1 <= n_passed <= 3
-        assert (n_passed + n_failed) < 6
+        # DSession should stop when the first failure is reached. Two failures
+        # may actually occur, due to timing.
+        outcomes = result.parseoutcomes()
+        assert "failed" in outcomes, "Expected at least one failure"
+        assert 1 <= outcomes["failed"] <= 2, "Expected no more than 2 failures"
 
     def test_basetemp_in_subprocesses(self, pytester: pytest.Pytester) -> None:
         p1 = pytester.makepyfile(
             """
             def test_send(tmp_path):
                 from pathlib import Path
                 assert tmp_path.relative_to(Path(%r)), tmp_path
@@ -220,15 +220,15 @@
                 "*node*down*",
                 "*3 failed, 1 passed, 1 skipped*",
             ]
         )
         assert result.ret == 1
 
     def test_distribution_rsyncdirs_example(
-        self, pytester: pytest.Pytester, monkeypatch
+        self, pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch
     ) -> None:
         # use a custom plugin that has a custom command-line option to ensure
         # this is propagated to workers (see #491)
         pytester.makepyfile(
             **{
                 "myplugin/src/foobarplugin.py": """
             from __future__ import print_function
@@ -262,16 +262,16 @@
         result = pytester.runpytest_subprocess(
             "-v",
             "-d",
             "-s",
             "-pfoobarplugin",
             "--foobar=123",
             "--dist=load",
-            "--rsyncdir=%(subdir)s" % locals(),
-            "--tx=popen//chdir=%(dest)s" % locals(),
+            f"--rsyncdir={subdir}",
+            f"--tx=popen//chdir={dest}",
             p,
         )
         assert result.ret == 0
         result.stdout.fnmatch_lines(
             [
                 "*1 passed*",
             ]
@@ -412,15 +412,15 @@
         s = result.stdout.str()
         assert "2...5" in s
         assert "2...6" in s
 
 
 class TestTerminalReporting:
     @pytest.mark.parametrize("verbosity", ["", "-q", "-v"])
-    def test_output_verbosity(self, pytester, verbosity: str) -> None:
+    def test_output_verbosity(self, pytester: pytest.Pytester, verbosity: str) -> None:
         pytester.makepyfile(
             """
             def test_ok():
                 pass
         """
         )
         args = ["-n1"]
@@ -478,15 +478,15 @@
                 "*def test_func():",
                 ">       assert 0",
                 "E       assert 0",
             ]
         )
 
     def test_logfinish_hook(self, pytester: pytest.Pytester) -> None:
-        """Ensure the pytest_runtest_logfinish hook is being properly handled"""
+        """Ensure the pytest_runtest_logfinish hook is being properly handled."""
         pytester.makeconftest(
             """
             def pytest_runtest_logfinish():
                 print('pytest_runtest_logfinish hook called')
         """
         )
         pytester.makepyfile(
@@ -607,17 +607,17 @@
     )
     result = pytester.runpytest_subprocess(p, "-n1")
     result.stdout.fnmatch_lines(["*ValueError*42*", "*1 passed*1 error*"])
     assert result.ret
 
 
 def test_config_initialization(
-    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, pytestconfig
+    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch
 ) -> None:
-    """Ensure workers and controller are initialized consistently. Integration test for #445"""
+    """Ensure workers and controller are initialized consistently. Integration test for #445."""
     pytester.makepyfile(
         **{
             "dir_a/test_foo.py": """
                 def test_1(request):
                     assert request.config.option.verbose == 2
         """
         }
@@ -632,16 +632,16 @@
     monkeypatch.setenv("PYTEST_ADDOPTS", "-v")
     result = pytester.runpytest("-n2", "-c", "myconfig.ini", "-v")
     result.stdout.fnmatch_lines(["dir_a/test_foo.py::test_1*", "*= 1 passed in *"])
     assert result.ret == 0
 
 
 @pytest.mark.parametrize("when", ["setup", "call", "teardown"])
-def test_crashing_item(pytester, when) -> None:
-    """Ensure crashing item is correctly reported during all testing stages"""
+def test_crashing_item(pytester: pytest.Pytester, when: str) -> None:
+    """Ensure crashing item is correctly reported during all testing stages."""
     code = dict(setup="", call="", teardown="")
     code[when] = "os._exit(1)"
     p = pytester.makepyfile(
         """
         import os
         import pytest
 
@@ -653,17 +653,15 @@
 
         def test_crash(fix):
             {call}
             pass
 
         def test_ok():
             pass
-    """.format(
-            **code
-        )
+    """.format(**code)
     )
     passes = 2 if when == "teardown" else 1
     result = pytester.runpytest("-n2", p)
     result.stdout.fnmatch_lines(
         ["*crashed*test_crash*", "*1 failed*%d passed*" % passes]
     )
 
@@ -765,30 +763,30 @@
     )
     result = pytester.runpytest(p1, "-n1", "-p", "no:tmpdir")
     assert result.ret == 0
     result.stdout.fnmatch_lines("*1 passed*")
 
 
 @pytest.mark.parametrize("plugin", ["xdist.looponfail"])
-def test_sub_plugins_disabled(pytester, plugin) -> None:
-    """Test that xdist doesn't break if we disable any of its sub-plugins. (#32)"""
+def test_sub_plugins_disabled(pytester: pytest.Pytester, plugin: str) -> None:
+    """Test that xdist doesn't break if we disable any of its sub-plugins (#32)."""
     p1 = pytester.makepyfile(
         """
         def test_ok():
             pass
     """
     )
     result = pytester.runpytest(p1, "-n1", "-p", f"no:{plugin}")
     assert result.ret == 0
     result.stdout.fnmatch_lines("*1 passed*")
 
 
 class TestWarnings:
     @pytest.mark.parametrize("n", ["-n0", "-n1"])
-    def test_warnings(self, pytester, n) -> None:
+    def test_warnings(self, pytester: pytest.Pytester, n: str) -> None:
         pytester.makepyfile(
             """
             import warnings, py, pytest
 
             @pytest.mark.filterwarnings('ignore:config.warn has been deprecated')
             def test_func(request):
                 warnings.warn(UserWarning('this is a warning'))
@@ -796,17 +794,15 @@
         )
         result = pytester.runpytest(n)
         result.stdout.fnmatch_lines(["*this is a warning*", "*1 passed, 1 warning*"])
 
     def test_warning_captured_deprecated_in_pytest_6(
         self, pytester: pytest.Pytester
     ) -> None:
-        """
-        Do not trigger the deprecated pytest_warning_captured hook in pytest 6+ (#562)
-        """
+        """Do not trigger the deprecated pytest_warning_captured hook in pytest 6+ (#562)."""
         from _pytest import hookspec
 
         if not hasattr(hookspec, "pytest_warning_captured"):
             pytest.skip(
                 f"pytest {pytest.__version__} does not have the pytest_warning_captured hook."
             )
 
@@ -828,17 +824,17 @@
         """
         )
         result = pytester.runpytest("-n1", "-Wignore")
         result.stdout.fnmatch_lines(["*1 passed*"])
         result.stdout.no_fnmatch_line("*this hook should not be called in this version")
 
     @pytest.mark.parametrize("n", ["-n0", "-n1"])
-    def test_custom_subclass(self, pytester, n) -> None:
+    def test_custom_subclass(self, pytester: pytest.Pytester, n: str) -> None:
         """Check that warning subclasses that don't honor the args attribute don't break
-        pytest-xdist (#344)
+        pytest-xdist (#344).
         """
         pytester.makepyfile(
             """
             import warnings, py, pytest
 
             class MyWarning(UserWarning):
 
@@ -852,15 +848,15 @@
         """
         )
         pytester.syspathinsert()
         result = pytester.runpytest(n)
         result.stdout.fnmatch_lines(["*MyWarning*", "*1 passed, 1 warning*"])
 
     @pytest.mark.parametrize("n", ["-n0", "-n1"])
-    def test_unserializable_arguments(self, pytester, n) -> None:
+    def test_unserializable_arguments(self, pytester: pytest.Pytester, n: str) -> None:
         """Check that warnings with unserializable arguments are handled correctly (#349)."""
         pytester.makepyfile(
             """
             import warnings, pytest
 
             def test_func(tmp_path):
                 fn = tmp_path / 'foo.txt'
@@ -870,15 +866,17 @@
         """
         )
         pytester.syspathinsert()
         result = pytester.runpytest(n)
         result.stdout.fnmatch_lines(["*UserWarning*foo.txt*", "*1 passed, 1 warning*"])
 
     @pytest.mark.parametrize("n", ["-n0", "-n1"])
-    def test_unserializable_warning_details(self, pytester, n) -> None:
+    def test_unserializable_warning_details(
+        self, pytester: pytest.Pytester, n: str
+    ) -> None:
         """Check that warnings with unserializable _WARNING_DETAILS are
         handled correctly (#379).
         """
         pytester.makepyfile(
             """
             import warnings, pytest
             import socket
@@ -1050,15 +1048,15 @@
                 "* xdist: worker gw* crashed and worker restarting disabled *",
                 "* 1 failed, 2 passed in *",
             ]
         )
 
 
 @pytest.mark.parametrize("n", [0, 2])
-def test_worker_id_fixture(pytester, n) -> None:
+def test_worker_id_fixture(pytester: pytest.Pytester, n: int) -> None:
     import glob
 
     f = pytester.makepyfile(
         """
         import pytest
         @pytest.mark.parametrize("run_num", range(2))
         def test_worker_id1(worker_id, run_num):
@@ -1066,24 +1064,24 @@
                 f.write(worker_id)
     """
     )
     result = pytester.runpytest(f, "-n%d" % n)
     result.stdout.fnmatch_lines("* 2 passed in *")
     worker_ids = set()
     for fname in glob.glob(str(pytester.path / "*.txt")):
-        with open(fname) as f:
-            worker_ids.add(f.read().strip())
+        with open(fname) as fp:
+            worker_ids.add(fp.read().strip())
     if n == 0:
         assert worker_ids == {"master"}
     else:
         assert worker_ids == {"gw0", "gw1"}
 
 
 @pytest.mark.parametrize("n", [0, 2])
-def test_testrun_uid_fixture(pytester, n) -> None:
+def test_testrun_uid_fixture(pytester: pytest.Pytester, n: int) -> None:
     import glob
 
     f = pytester.makepyfile(
         """
         import pytest
         @pytest.mark.parametrize("run_num", range(2))
         def test_testrun_uid1(testrun_uid, run_num):
@@ -1091,43 +1089,40 @@
                 f.write(testrun_uid)
     """
     )
     result = pytester.runpytest(f, "-n%d" % n)
     result.stdout.fnmatch_lines("* 2 passed in *")
     testrun_uids = set()
     for fname in glob.glob(str(pytester.path / "*.txt")):
-        with open(fname) as f:
-            testrun_uids.add(f.read().strip())
+        with open(fname) as fp:
+            testrun_uids.add(fp.read().strip())
     assert len(testrun_uids) == 1
     assert len(testrun_uids.pop()) == 32
 
 
 @pytest.mark.parametrize("tb", ["auto", "long", "short", "no", "line", "native"])
-def test_error_report_styles(pytester, tb) -> None:
+def test_error_report_styles(pytester: pytest.Pytester, tb: str) -> None:
     pytester.makepyfile(
         """
         import pytest
         def test_error_report_styles():
             raise RuntimeError('some failure happened')
     """
     )
     result = pytester.runpytest("-n1", "--tb=%s" % tb)
     if tb != "no":
         result.stdout.fnmatch_lines("*some failure happened*")
     result.assert_outcomes(failed=1)
 
 
-def test_color_yes_collection_on_non_atty(pytester, request) -> None:
-    """skip collect progress report when working on non-terminals.
+def test_color_yes_collection_on_non_atty(pytester: pytest.Pytester) -> None:
+    """Skip collect progress report when working on non-terminals.
 
     Similar to pytest-dev/pytest#1397
     """
-    tr = request.config.pluginmanager.getplugin("terminalreporter")
-    if not hasattr(tr, "isatty"):
-        pytest.skip("only valid for newer pytest versions")
     pytester.makepyfile(
         """
         import pytest
         @pytest.mark.parametrize('i', range(10))
         def test_this(i):
             assert 1
     """
@@ -1137,34 +1132,30 @@
     assert "test session starts" in result.stdout.str()
     assert "\x1b[1m" in result.stdout.str()
     assert "created: 2/2 workers" in result.stdout.str()
     assert "2 workers [10 items]" in result.stdout.str()
     assert "collecting:" not in result.stdout.str()
 
 
-def test_without_terminal_plugin(pytester, request) -> None:
-    """
-    No output when terminal plugin is disabled
-    """
+def test_without_terminal_plugin(pytester: pytest.Pytester) -> None:
+    """No output when terminal plugin is disabled."""
     pytester.makepyfile(
         """
         def test_1():
             pass
     """
     )
     result = pytester.runpytest("-p", "no:terminal", "-n2")
     assert result.stdout.str() == ""
     assert result.stderr.str() == ""
     assert result.ret == 0
 
 
 def test_internal_error_with_maxfail(pytester: pytest.Pytester) -> None:
-    """
-    Internal error when using --maxfail option (#62, #65).
-    """
+    """Internal error when using --maxfail option (#62, #65)."""
     pytester.makepyfile(
         """
         import pytest
 
         @pytest.fixture(params=['1', '2'])
         def crasher():
             raise RuntimeError
@@ -1176,14 +1167,29 @@
     """
     )
     result = pytester.runpytest_subprocess("--maxfail=1", "-n1")
     result.stdout.re_match_lines([".* [12] errors? in .*"])
     assert "INTERNALERROR" not in result.stderr.str()
 
 
+def test_maxfail_causes_early_termination(pytester: pytest.Pytester) -> None:
+    """Ensure subsequent tests on a worker aren't run when using --maxfail (#1024)."""
+    pytester.makepyfile(
+        """
+        def test1():
+            assert False
+
+        def test2():
+            pass
+    """
+    )
+    result = pytester.runpytest_subprocess("--maxfail=1", "-n 1")
+    result.assert_outcomes(failed=1)
+
+
 def test_internal_errors_propagate_to_controller(pytester: pytest.Pytester) -> None:
     pytester.makeconftest(
         """
         def pytest_collection_modifyitems():
             raise RuntimeError("Some runtime error")
         """
     )
@@ -1361,25 +1367,25 @@
         assert a in ({"gw0": 1}, {"gw1": 1})
         assert b in ({"gw0": 1}, {"gw1": 1})
         assert a.items() != b.items()
         assert c1 == c2
 
 
 class TestGroupScope:
-    def test_by_module(self, testdir):
+    def test_by_module(self, pytester: pytest.Pytester) -> None:
         test_file = """
             import pytest
             class TestA:
                 @pytest.mark.xdist_group(name="xdist_group")
                 @pytest.mark.parametrize('i', range(5))
                 def test(self, i):
                     pass
         """
-        testdir.makepyfile(test_a=test_file, test_b=test_file)
-        result = testdir.runpytest("-n2", "--dist=loadgroup", "-v")
+        pytester.makepyfile(test_a=test_file, test_b=test_file)
+        result = pytester.runpytest("-n2", "--dist=loadgroup", "-v")
         test_a_workers_and_test_count = get_workers_and_test_count_by_prefix(
             "test_a.py::TestA", result.outlines
         )
         test_b_workers_and_test_count = get_workers_and_test_count_by_prefix(
             "test_b.py::TestA", result.outlines
         )
 
@@ -1392,31 +1398,31 @@
             {"gw1": 0},
         ) or test_b_workers_and_test_count in ({"gw0": 0}, {"gw1": 5})
         assert (
             test_a_workers_and_test_count.items()
             == test_b_workers_and_test_count.items()
         )
 
-    def test_by_class(self, testdir):
-        testdir.makepyfile(
+    def test_by_class(self, pytester: pytest.Pytester) -> None:
+        pytester.makepyfile(
             test_a="""
             import pytest
             class TestA:
                 @pytest.mark.xdist_group(name="xdist_group")
                 @pytest.mark.parametrize('i', range(10))
                 def test(self, i):
                     pass
             class TestB:
                 @pytest.mark.xdist_group(name="xdist_group")
                 @pytest.mark.parametrize('i', range(10))
                 def test(self, i):
                     pass
         """
         )
-        result = testdir.runpytest("-n2", "--dist=loadgroup", "-v")
+        result = pytester.runpytest("-n2", "--dist=loadgroup", "-v")
         test_a_workers_and_test_count = get_workers_and_test_count_by_prefix(
             "test_a.py::TestA", result.outlines
         )
         test_b_workers_and_test_count = get_workers_and_test_count_by_prefix(
             "test_a.py::TestB", result.outlines
         )
 
@@ -1429,49 +1435,49 @@
             {"gw1": 0},
         ) or test_b_workers_and_test_count in ({"gw0": 0}, {"gw1": 10})
         assert (
             test_a_workers_and_test_count.items()
             == test_b_workers_and_test_count.items()
         )
 
-    def test_module_single_start(self, testdir):
+    def test_module_single_start(self, pytester: pytest.Pytester) -> None:
         test_file1 = """
             import pytest
             @pytest.mark.xdist_group(name="xdist_group")
             def test():
                 pass
         """
         test_file2 = """
             import pytest
             def test_1():
                 pass
             @pytest.mark.xdist_group(name="xdist_group")
             def test_2():
                 pass
         """
-        testdir.makepyfile(test_a=test_file1, test_b=test_file1, test_c=test_file2)
-        result = testdir.runpytest("-n2", "--dist=loadgroup", "-v")
+        pytester.makepyfile(test_a=test_file1, test_b=test_file1, test_c=test_file2)
+        result = pytester.runpytest("-n2", "--dist=loadgroup", "-v")
         a = get_workers_and_test_count_by_prefix("test_a.py::test", result.outlines)
         b = get_workers_and_test_count_by_prefix("test_b.py::test", result.outlines)
         c = get_workers_and_test_count_by_prefix("test_c.py::test_2", result.outlines)
 
         assert a.keys() == b.keys() and b.keys() == c.keys()
 
-    def test_with_two_group_names(self, testdir):
+    def test_with_two_group_names(self, pytester: pytest.Pytester) -> None:
         test_file = """
             import pytest
             @pytest.mark.xdist_group(name="group1")
             def test_1():
                 pass
             @pytest.mark.xdist_group("group2")
             def test_2():
                 pass
         """
-        testdir.makepyfile(test_a=test_file, test_b=test_file)
-        result = testdir.runpytest("-n2", "--dist=loadgroup", "-v")
+        pytester.makepyfile(test_a=test_file, test_b=test_file)
+        result = pytester.runpytest("-n2", "--dist=loadgroup", "-v")
         a_1 = get_workers_and_test_count_by_prefix("test_a.py::test_1", result.outlines)
         a_2 = get_workers_and_test_count_by_prefix("test_a.py::test_2", result.outlines)
         b_1 = get_workers_and_test_count_by_prefix("test_b.py::test_1", result.outlines)
         b_2 = get_workers_and_test_count_by_prefix("test_b.py::test_2", result.outlines)
 
         assert a_1.keys() == b_1.keys() and a_2.keys() == b_2.keys()
 
@@ -1500,37 +1506,39 @@
     """
 
     test_file1 = """
     import filelock
 
     FILE_LOCK = filelock.FileLock("test.lock")
 
-    """ + (
-        (_test_content * 4) % ("A", "B", "C", "D")
-    )
+    """ + ((_test_content * 4) % ("A", "B", "C", "D"))
 
-    @pytest.mark.parametrize("scope", ["each", "load", "loadscope", "loadfile", "no"])
-    def test_single_file(self, pytester, scope) -> None:
+    @pytest.mark.parametrize(
+        "scope", ["each", "load", "loadscope", "loadfile", "worksteal", "no"]
+    )
+    def test_single_file(self, pytester: pytest.Pytester, scope: str) -> None:
         pytester.makepyfile(test_a=self.test_file1)
         result = pytester.runpytest("-n2", "--dist=%s" % scope, "-v")
         result.assert_outcomes(passed=(12 if scope != "each" else 12 * 2))
 
-    @pytest.mark.parametrize("scope", ["each", "load", "loadscope", "loadfile", "no"])
-    def test_multi_file(self, pytester, scope) -> None:
+    @pytest.mark.parametrize(
+        "scope", ["each", "load", "loadscope", "loadfile", "worksteal", "no"]
+    )
+    def test_multi_file(self, pytester: pytest.Pytester, scope: str) -> None:
         pytester.makepyfile(
             test_a=self.test_file1,
             test_b=self.test_file1,
             test_c=self.test_file1,
             test_d=self.test_file1,
         )
         result = pytester.runpytest("-n2", "--dist=%s" % scope, "-v")
         result.assert_outcomes(passed=(48 if scope != "each" else 48 * 2))
 
 
-def parse_tests_and_workers_from_output(lines: List[str]) -> List[Tuple[str, str, str]]:
+def parse_tests_and_workers_from_output(lines: list[str]) -> list[tuple[str, str, str]]:
     result = []
     for line in lines:
         # example match: "[gw0] PASSED test_a.py::test[7]"
         m = re.match(
             r"""
             \[(gw\d)\]  # worker
             \s*
@@ -1544,92 +1552,92 @@
         if m:
             worker, status, nodeid = m.groups()
             result.append((worker, status, nodeid))
     return result
 
 
 def get_workers_and_test_count_by_prefix(
-    prefix: str, lines: List[str], expected_status: str = "PASSED"
-) -> Dict[str, int]:
-    result: Dict[str, int] = {}
+    prefix: str, lines: list[str], expected_status: str = "PASSED"
+) -> dict[str, int]:
+    result: dict[str, int] = {}
     for worker, status, nodeid in parse_tests_and_workers_from_output(lines):
         if expected_status == status and nodeid.startswith(prefix):
             result[worker] = result.get(worker, 0) + 1
     return result
 
 
 class TestAPI:
     @pytest.fixture
-    def fake_request(self):
+    def fake_request(self) -> pytest.FixtureRequest:
         class FakeOption:
-            def __init__(self):
+            def __init__(self) -> None:
                 self.dist = "load"
 
         class FakeConfig:
-            def __init__(self):
+            def __init__(self) -> None:
                 self.workerinput = {"workerid": "gw5"}
                 self.option = FakeOption()
 
         class FakeRequest:
-            def __init__(self):
+            def __init__(self) -> None:
                 self.config = FakeConfig()
 
-        return FakeRequest()
+        return cast(pytest.FixtureRequest, FakeRequest())
 
-    def test_is_xdist_worker(self, fake_request) -> None:
+    def test_is_xdist_worker(self, fake_request: pytest.FixtureRequest) -> None:
         assert xdist.is_xdist_worker(fake_request)
-        del fake_request.config.workerinput
+        del fake_request.config.workerinput  # type: ignore[attr-defined]
         assert not xdist.is_xdist_worker(fake_request)
 
-    def test_is_xdist_controller(self, fake_request) -> None:
+    def test_is_xdist_controller(self, fake_request: pytest.FixtureRequest) -> None:
         assert not xdist.is_xdist_master(fake_request)
         assert not xdist.is_xdist_controller(fake_request)
 
-        del fake_request.config.workerinput
+        del fake_request.config.workerinput  # type: ignore[attr-defined]
         assert xdist.is_xdist_master(fake_request)
         assert xdist.is_xdist_controller(fake_request)
 
         fake_request.config.option.dist = "no"
         assert not xdist.is_xdist_master(fake_request)
         assert not xdist.is_xdist_controller(fake_request)
 
-    def test_get_xdist_worker_id(self, fake_request) -> None:
+    def test_get_xdist_worker_id(self, fake_request: pytest.FixtureRequest) -> None:
         assert xdist.get_xdist_worker_id(fake_request) == "gw5"
-        del fake_request.config.workerinput
+        del fake_request.config.workerinput  # type: ignore[attr-defined]
         assert xdist.get_xdist_worker_id(fake_request) == "master"
 
 
-def test_collection_crash(testdir):
-    p1 = testdir.makepyfile(
+def test_collection_crash(pytester: pytest.Pytester) -> None:
+    p1 = pytester.makepyfile(
         """
         assert 0
     """
     )
-    result = testdir.runpytest(p1, "-n1")
+    result = pytester.runpytest(p1, "-n1")
     assert result.ret == 1
     result.stdout.fnmatch_lines(
         [
             "created: 1/1 worker",
             "1 worker [[]0 items[]]",
             "*_ ERROR collecting test_collection_crash.py _*",
             "E   assert 0",
             "*= 1 error in *",
         ]
     )
 
 
-def test_dist_in_addopts(testdir):
+def test_dist_in_addopts(pytester: pytest.Pytester) -> None:
     """Users can set a default distribution in the configuration file (#789)."""
-    testdir.makepyfile(
+    pytester.makepyfile(
         """
         def test():
             pass
         """
     )
-    testdir.makeini(
+    pytester.makeini(
         """
         [pytest]
         addopts = --dist loadscope
         """
     )
-    result = testdir.runpytest()
+    result = pytester.runpytest()
     assert result.ret == 0
```

### Comparing `pytest-xdist-3.5.0/testing/conftest.py` & `pytest_xdist-3.6.0/testing/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,68 @@
+from __future__ import annotations
+
+import shutil
+from typing import Callable
+from typing import Generator
+
 import execnet
 import pytest
-import shutil
-from typing import List
+
 
 pytest_plugins = "pytester"
 
 
 @pytest.fixture(autouse=True)
-def _divert_atexit(request, monkeypatch: pytest.MonkeyPatch):
+def _divert_atexit(monkeypatch: pytest.MonkeyPatch) -> Generator[None, None, None]:
     import atexit
 
     finalizers = []
 
-    def fake_register(func, *args, **kwargs):
+    def fake_register(
+        func: Callable[..., object], *args: object, **kwargs: object
+    ) -> None:
         finalizers.append((func, args, kwargs))
 
     monkeypatch.setattr(atexit, "register", fake_register)
 
     yield
 
     while finalizers:
         func, args, kwargs = finalizers.pop()
         func(*args, **kwargs)
 
 
-def pytest_addoption(parser) -> None:
+def pytest_addoption(parser: pytest.Parser) -> None:
     parser.addoption(
         "--gx",
         action="append",
         dest="gspecs",
         help="add a global test environment, XSpec-syntax. ",
     )
 
 
 @pytest.fixture
-def specssh(request) -> str:
+def specssh(request: pytest.FixtureRequest) -> str:
     return getspecssh(request.config)
 
 
 # configuration information for tests
-def getgspecs(config) -> List[execnet.XSpec]:
+def getgspecs(config: pytest.Config) -> list[execnet.XSpec]:
     return [execnet.XSpec(spec) for spec in config.getvalueorskip("gspecs")]
 
 
-def getspecssh(config) -> str:  # type: ignore[return]
+def getspecssh(config: pytest.Config) -> str:
     xspecs = getgspecs(config)
     for spec in xspecs:
         if spec.ssh:
             if not shutil.which("ssh"):
                 pytest.skip("command not found: ssh")
             return str(spec)
     pytest.skip("need '--gx ssh=...'")
 
 
-def getsocketspec(config) -> execnet.XSpec:
+def getsocketspec(config: pytest.Config) -> execnet.XSpec:
     xspecs = getgspecs(config)
     for spec in xspecs:
         if spec.socket:
             return spec
     pytest.skip("need '--gx socket=...'")
```

### Comparing `pytest-xdist-3.5.0/testing/test_dsession.py` & `pytest_xdist-3.6.0/testing/test_dsession.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,127 +1,142 @@
 from __future__ import annotations
-from xdist.dsession import (
-    DSession,
-    get_default_max_worker_restart,
-    get_workers_status_line,
-    WorkerStatus,
-)
-from xdist.report import report_collection_diff
-from xdist.scheduler import EachScheduling, LoadScheduling, WorkStealingScheduling
+
+from typing import Any
+from typing import cast
 from typing import Sequence
+from typing import TYPE_CHECKING
 
-import pytest
 import execnet
+import pytest
+
+from xdist.dsession import DSession
+from xdist.dsession import get_default_max_worker_restart
+from xdist.dsession import get_workers_status_line
+from xdist.dsession import WorkerStatus
+from xdist.report import report_collection_diff
+from xdist.scheduler import EachScheduling
+from xdist.scheduler import LoadScheduling
+from xdist.scheduler import WorkStealingScheduling
+from xdist.workermanage import WorkerController
 
 
-class MockGateway:
+if TYPE_CHECKING:
+    BaseOfMockGateway = execnet.Gateway
+    BaseOfMockNode = WorkerController
+else:
+    BaseOfMockGateway = object
+    BaseOfMockNode = object
+
+
+class MockGateway(BaseOfMockGateway):
     def __init__(self) -> None:
         self._count = 0
         self.id = str(self._count)
         self._count += 1
 
 
-class MockNode:
+class MockNode(BaseOfMockNode):
     def __init__(self) -> None:
-        self.sent = []  # type: ignore[var-annotated]
-        self.stolen = []  # type: ignore[var-annotated]
+        self.sent: list[int | str] = []
+        self.stolen: list[int] = []
         self.gateway = MockGateway()
         self._shutdown = False
 
-    def send_runtest_some(self, indices) -> None:
+    def send_runtest_some(self, indices: Sequence[int]) -> None:
         self.sent.extend(indices)
 
     def send_runtest_all(self) -> None:
         self.sent.append("ALL")
 
-    def send_steal(self, indices) -> None:
+    def send_steal(self, indices: Sequence[int]) -> None:
         self.stolen.extend(indices)
 
     def shutdown(self) -> None:
         self._shutdown = True
 
     @property
     def shutting_down(self) -> bool:
         return self._shutdown
 
 
 class TestEachScheduling:
     def test_schedule_load_simple(self, pytester: pytest.Pytester) -> None:
-        node1 = MockNode()
-        node2 = MockNode()
         config = pytester.parseconfig("--tx=2*popen")
         sched = EachScheduling(config)
+        node1, node2 = MockNode(), MockNode()
         sched.add_node(node1)
         sched.add_node(node2)
         collection = ["a.py::test_1"]
         assert not sched.collection_is_completed
         sched.add_node_collection(node1, collection)
         assert not sched.collection_is_completed
         sched.add_node_collection(node2, collection)
-        assert sched.collection_is_completed
+        assert bool(sched.collection_is_completed)
         assert sched.node2collection[node1] == collection
         assert sched.node2collection[node2] == collection
         sched.schedule()
         assert sched.tests_finished
         assert node1.sent == ["ALL"]
         assert node2.sent == ["ALL"]
         sched.mark_test_complete(node1, 0)
         assert sched.tests_finished
         sched.mark_test_complete(node2, 0)
         assert sched.tests_finished
 
     def test_schedule_remove_node(self, pytester: pytest.Pytester) -> None:
-        node1 = MockNode()
         config = pytester.parseconfig("--tx=popen")
         sched = EachScheduling(config)
+        node1 = MockNode()
         sched.add_node(node1)
         collection = ["a.py::test_1"]
         assert not sched.collection_is_completed
         sched.add_node_collection(node1, collection)
-        assert sched.collection_is_completed
+        assert bool(sched.collection_is_completed)
         assert sched.node2collection[node1] == collection
         sched.schedule()
         assert sched.tests_finished
         crashitem = sched.remove_node(node1)
         assert crashitem
         assert sched.tests_finished
         assert not sched.nodes
 
 
 class TestLoadScheduling:
     def test_schedule_load_simple(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         collection = ["a.py::test_1", "a.py::test_2"]
         assert not sched.collection_is_completed
         sched.add_node_collection(node1, collection)
         assert not sched.collection_is_completed
         sched.add_node_collection(node2, collection)
-        assert sched.collection_is_completed
+        assert bool(sched.collection_is_completed)
         assert sched.node2collection[node1] == collection
         assert sched.node2collection[node2] == collection
         sched.schedule()
         assert not sched.pending
         assert sched.tests_finished
         assert len(node1.sent) == 1
         assert len(node2.sent) == 1
         assert node1.sent == [0]
         assert node2.sent == [1]
-        sched.mark_test_complete(node1, node1.sent[0])
+        sent10 = node1.sent[0]
+        assert isinstance(sent10, int)
+        sched.mark_test_complete(node1, sent10)
         assert sched.tests_finished
 
     def test_schedule_batch_size(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         col = ["xyz"] * 6
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.schedule()
         # assert not sched.tests_finished
         sent1 = node1.sent
         sent2 = node2.sent
@@ -138,17 +153,17 @@
         sched.mark_test_complete(node1, 1)
         assert node1.sent == [0, 1, 4, 5]
         assert not sched.pending
 
     def test_schedule_maxchunk_none(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         col = [f"test{i}" for i in range(16)]
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.schedule()
         assert node1.sent == [0, 1]
         assert node2.sent == [2, 3]
         assert sched.pending == list(range(4, 16))
@@ -159,47 +174,49 @@
         assert sched.pending == list(range(6, 16))
         sched.mark_test_complete(node1, 1)
         assert node1.sent == [0, 1, 4, 5]
         assert sched.pending == list(range(6, 16))
 
         for i in range(7, 16):
             sched.mark_test_complete(node1, i - 3)
-            assert node1.sent == [0, 1] + list(range(4, i))
+            assert node1.sent == [0, 1, *range(4, i)]
             assert node2.sent == [2, 3]
             assert sched.pending == list(range(i, 16))
 
     def test_schedule_maxchunk_1(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen", "--maxschedchunk=1")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         col = [f"test{i}" for i in range(16)]
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.schedule()
         assert node1.sent == [0, 1]
         assert node2.sent == [2, 3]
         assert sched.pending == list(range(4, 16))
         assert sched.node2pending[node1] == node1.sent
         assert sched.node2pending[node2] == node2.sent
 
         for complete_index, first_pending in enumerate(range(5, 16)):
-            sched.mark_test_complete(node1, node1.sent[complete_index])
-            assert node1.sent == [0, 1] + list(range(4, first_pending))
+            sent_index = node1.sent[complete_index]
+            assert isinstance(sent_index, int)
+            sched.mark_test_complete(node1, sent_index)
+            assert node1.sent == [0, 1, *range(4, first_pending)]
             assert node2.sent == [2, 3]
             assert sched.pending == list(range(first_pending, 16))
 
     def test_schedule_fewer_tests_than_nodes(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=3*popen")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2, node3 = sched.nodes
+        node1, node2, node3 = MockNode(), MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
+        sched.add_node(node3)
         col = ["xyz"] * 2
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.add_node_collection(node3, col)
         assert sched.collection_is_completed
         sched.schedule()
         # assert not sched.tests_finished
@@ -209,34 +226,34 @@
         assert not sched.pending
 
     def test_schedule_fewer_than_two_tests_per_node(
         self, pytester: pytest.Pytester
     ) -> None:
         config = pytester.parseconfig("--tx=3*popen")
         sched = LoadScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2, node3 = sched.nodes
+        node1, node2, node3 = MockNode(), MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
+        sched.add_node(node3)
         col = ["xyz"] * 5
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.add_node_collection(node3, col)
         assert sched.collection_is_completed
         sched.schedule()
         # assert not sched.tests_finished
         assert node1.sent == [0, 3]
         assert node2.sent == [1, 4]
         assert node3.sent == [2]
         assert not sched.pending
 
     def test_add_remove_node(self, pytester: pytest.Pytester) -> None:
-        node = MockNode()
         config = pytester.parseconfig("--tx=popen")
         sched = LoadScheduling(config)
+        node = MockNode()
         sched.add_node(node)
         collection = ["test_file.py::test_func"]
         sched.add_node_collection(node, collection)
         assert sched.collection_is_completed
         sched.schedule()
         assert not sched.pending
         crashitem = sched.remove_node(node)
@@ -245,86 +262,90 @@
     def test_different_tests_collected(self, pytester: pytest.Pytester) -> None:
         """
         Test that LoadScheduling is reporting collection errors when
         different test ids are collected by workers.
         """
 
         class CollectHook:
-            """
-            Dummy hook that stores collection reports.
-            """
+            """Dummy hook that stores collection reports."""
 
-            def __init__(self):
-                self.reports = []
+            def __init__(self) -> None:
+                self.reports: list[pytest.CollectReport] = []
 
-            def pytest_collectreport(self, report):
+            def pytest_collectreport(self, report: pytest.CollectReport) -> None:
                 self.reports.append(report)
 
         collect_hook = CollectHook()
         config = pytester.parseconfig("--tx=2*popen")
         config.pluginmanager.register(collect_hook, "collect_hook")
-        node1 = MockNode()
-        node2 = MockNode()
         sched = LoadScheduling(config)
+        node1, node2 = MockNode(), MockNode()
         sched.add_node(node1)
         sched.add_node(node2)
         sched.add_node_collection(node1, ["a.py::test_1"])
         sched.add_node_collection(node2, ["a.py::test_2"])
         sched.schedule()
         assert len(collect_hook.reports) == 1
         rep = collect_hook.reports[0]
+        assert isinstance(rep.longrepr, str)
         assert "Different tests were collected between" in rep.longrepr
 
 
 class TestWorkStealingScheduling:
     def test_ideal_case(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen")
         sched = WorkStealingScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         collection = [f"test_workstealing.py::test_{i}" for i in range(16)]
         assert not sched.collection_is_completed
         sched.add_node_collection(node1, collection)
         assert not sched.collection_is_completed
         sched.add_node_collection(node2, collection)
-        assert sched.collection_is_completed
+        assert bool(sched.collection_is_completed)
         assert sched.node2collection[node1] == collection
         assert sched.node2collection[node2] == collection
         sched.schedule()
         assert not sched.pending
         assert not sched.tests_finished
-        assert node1.sent == list(range(0, 8))
+        assert node1.sent == list(range(8))
         assert node2.sent == list(range(8, 16))
         for i in range(8):
-            sched.mark_test_complete(node1, node1.sent[i])
-            sched.mark_test_complete(node2, node2.sent[i])
-        assert sched.tests_finished
+            sent1, sent2 = node1.sent[i], node2.sent[i]
+            assert isinstance(sent1, int) and isinstance(sent2, int)
+            sched.mark_test_complete(node1, sent1)
+            sched.mark_test_complete(node2, sent2)
+        assert bool(sched.tests_finished)
         assert node1.stolen == []
         assert node2.stolen == []
 
     def test_stealing(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=2*popen")
         sched = WorkStealingScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2 = sched.nodes
+        node1, node2 = MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
         collection = [f"test_workstealing.py::test_{i}" for i in range(16)]
         sched.add_node_collection(node1, collection)
         sched.add_node_collection(node2, collection)
         assert sched.collection_is_completed
         sched.schedule()
-        assert node1.sent == list(range(0, 8))
+        assert node1.sent == list(range(8))
         assert node2.sent == list(range(8, 16))
         for i in range(8):
-            sched.mark_test_complete(node1, node1.sent[i])
+            sent = node1.sent[i]
+            assert isinstance(sent, int)
+            sched.mark_test_complete(node1, sent)
         assert node2.stolen == list(range(12, 16))
         sched.remove_pending_tests_from_node(node2, node2.stolen)
         for i in range(4):
-            sched.mark_test_complete(node2, node2.sent[i])
+            sent = node2.sent[i]
+            assert isinstance(sent, int)
+            sched.mark_test_complete(node2, sent)
         assert node1.stolen == [14, 15]
         sched.remove_pending_tests_from_node(node1, node1.stolen)
         sched.mark_test_complete(node1, 12)
         sched.mark_test_complete(node2, 14)
         assert node2.stolen == list(range(12, 16))
         assert node1.stolen == [14, 15]
         assert sched.tests_finished
@@ -351,18 +372,18 @@
         sched.mark_test_complete(node2, 3)
         assert sched.tests_finished
         assert node2.stolen == []
 
     def test_schedule_fewer_tests_than_nodes(self, pytester: pytest.Pytester) -> None:
         config = pytester.parseconfig("--tx=3*popen")
         sched = WorkStealingScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2, node3 = sched.nodes
+        node1, node2, node3 = MockNode(), MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
+        sched.add_node(node3)
         col = ["xyz"] * 2
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.add_node_collection(node3, col)
         sched.schedule()
         assert node1.sent == []
         assert node1.stolen == []
@@ -374,33 +395,41 @@
         assert sched.tests_finished
 
     def test_schedule_fewer_than_two_tests_per_node(
         self, pytester: pytest.Pytester
     ) -> None:
         config = pytester.parseconfig("--tx=3*popen")
         sched = WorkStealingScheduling(config)
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        sched.add_node(MockNode())
-        node1, node2, node3 = sched.nodes
+        node1, node2, node3 = MockNode(), MockNode(), MockNode()
+        sched.add_node(node1)
+        sched.add_node(node2)
+        sched.add_node(node3)
         col = ["xyz"] * 5
         sched.add_node_collection(node1, col)
         sched.add_node_collection(node2, col)
         sched.add_node_collection(node3, col)
         sched.schedule()
         assert node1.sent == [0]
         assert node2.sent == [1, 2]
         assert node3.sent == [3, 4]
         assert not sched.pending
         assert not sched.tests_finished
-        sched.mark_test_complete(node1, node1.sent[0])
-        sched.mark_test_complete(node2, node2.sent[0])
-        sched.mark_test_complete(node3, node3.sent[0])
-        sched.mark_test_complete(node3, node3.sent[1])
-        assert sched.tests_finished
+        sent10 = node1.sent[0]
+        assert isinstance(sent10, int)
+        sent20 = node2.sent[0]
+        assert isinstance(sent20, int)
+        sent30 = node3.sent[0]
+        assert isinstance(sent30, int)
+        sent31 = node3.sent[1]
+        assert isinstance(sent31, int)
+        sched.mark_test_complete(node1, sent10)
+        sched.mark_test_complete(node2, sent20)
+        sched.mark_test_complete(node3, sent30)
+        sched.mark_test_complete(node3, sent31)
+        assert bool(sched.tests_finished)
         assert node1.stolen == []
         assert node2.stolen == []
         assert node3.stolen == []
 
     def test_add_remove_node(self, pytester: pytest.Pytester) -> None:
         node = MockNode()
         config = pytester.parseconfig("--tx=popen")
@@ -412,41 +441,41 @@
         sched.schedule()
         assert not sched.pending
         crashitem = sched.remove_node(node)
         assert crashitem == collection[0]
 
     def test_different_tests_collected(self, pytester: pytest.Pytester) -> None:
         class CollectHook:
-            def __init__(self):
-                self.reports = []
+            def __init__(self) -> None:
+                self.reports: list[pytest.CollectReport] = []
 
-            def pytest_collectreport(self, report):
+            def pytest_collectreport(self, report: pytest.CollectReport) -> None:
                 self.reports.append(report)
 
         collect_hook = CollectHook()
         config = pytester.parseconfig("--tx=2*popen")
         config.pluginmanager.register(collect_hook, "collect_hook")
-        node1 = MockNode()
-        node2 = MockNode()
         sched = WorkStealingScheduling(config)
+        node1, node2 = MockNode(), MockNode()
         sched.add_node(node1)
         sched.add_node(node2)
         sched.add_node_collection(node1, ["a.py::test_1"])
         sched.add_node_collection(node2, ["a.py::test_2"])
         sched.schedule()
         assert len(collect_hook.reports) == 1
         rep = collect_hook.reports[0]
+        assert isinstance(rep.longrepr, str)
         assert "Different tests were collected between" in rep.longrepr
 
 
 class TestDistReporter:
     @pytest.mark.xfail
-    def test_rsync_printing(self, pytester: pytest.Pytester, linecomp) -> None:
+    def test_rsync_printing(self, pytester: pytest.Pytester, linecomp: Any) -> None:
         config = pytester.parseconfig()
-        from _pytest.pytest_terminal import TerminalReporter
+        from _pytest.terminal import TerminalReporter
 
         rep = TerminalReporter(config, file=linecomp.stringio)
         config.pluginmanager.register(rep, "terminalreporter")
         dsession = DSession(config)
 
         class gw1:
             id = "X1"
@@ -469,23 +498,25 @@
         dsession.pytest_xdist_rsyncstart(source="hello", gateways=[gw1, gw2])  # type: ignore[attr-defined]
         linecomp.assert_contains_lines(["[X1,X2] rsyncing: hello"])
 
 
 def test_report_collection_diff_equal() -> None:
     """Test reporting of equal collections."""
     from_collection = to_collection = ["aaa", "bbb", "ccc"]
-    assert report_collection_diff(from_collection, to_collection, 1, 2) is None
+    assert report_collection_diff(from_collection, to_collection, "1", "2") is None
 
 
 def test_default_max_worker_restart() -> None:
-    class config:
+    class MockConfig:
         class option:
             maxworkerrestart: str | None = None
             numprocesses: int = 0
 
+    config = cast(pytest.Config, MockConfig)
+
     assert get_default_max_worker_restart(config) is None
 
     config.option.numprocesses = 2
     assert get_default_max_worker_restart(config) == 8
 
     config.option.maxworkerrestart = "1"
     assert get_default_max_worker_restart(config) == 1
```

### Comparing `pytest-xdist-3.5.0/testing/test_looponfail.py` & `pytest_xdist-3.6.0/testing/test_looponfail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import unittest.mock
-from typing import List
+from __future__ import annotations
 
-import pytest
+import pathlib
+from pathlib import Path
 import shutil
+import tempfile
 import textwrap
-from pathlib import Path
+import unittest.mock
+
+import pytest
 
 from xdist.looponfail import RemoteControl
 from xdist.looponfail import StatRecorder
 
 
-PYTEST_GTE_7 = hasattr(pytest, "version_tuple") and pytest.version_tuple >= (7, 0)  # type: ignore[attr-defined]
-
-
 class TestStatRecorder:
     def test_filechange(self, tmp_path: Path) -> None:
         tmp = tmp_path
         hello = tmp / "hello.py"
         hello.touch()
         sd = StatRecorder([tmp])
         changed = sd.check()
@@ -72,15 +72,15 @@
         changed = sd.check()
         assert changed
 
         p.unlink()
         # make check()'s visit() call return our just removed
         # path as if we were in a race condition
         dirname = str(tmp)
-        dirnames: List[str] = []
+        dirnames: list[str] = []
         filenames = [str(p)]
         with unittest.mock.patch(
             "os.walk", return_value=[(dirname, dirnames, filenames)], autospec=True
         ):
             changed = sd.check()
         assert changed
 
@@ -119,20 +119,19 @@
         topdir, failures = control.runsession()[:2]
         assert not failures
 
     def test_failures_somewhere(self, pytester: pytest.Pytester) -> None:
         item = pytester.getitem("def test_func():\n assert 0\n")
         control = RemoteControl(item.config)
         control.setup()
-        failures = control.runsession()
+        failures = control.runsession()[0]
         assert failures
         control.setup()
-        item_path = item.path if PYTEST_GTE_7 else Path(str(item.fspath))  # type: ignore[attr-defined]
-        item_path.write_text("def test_func():\n assert 1\n")
-        removepyc(item_path)
+        item.path.write_text("def test_func():\n assert 1\n")
+        removepyc(item.path)
         topdir, failures = control.runsession()[:2]
         assert not failures
 
     def test_failure_change(self, pytester: pytest.Pytester) -> None:
         modcol = pytester.getitem(
             textwrap.dedent(
                 """
@@ -140,18 +139,15 @@
                     assert 0
                 """
             )
         )
         control = RemoteControl(modcol.config)
         control.loop_once()
         assert control.failures
-        if PYTEST_GTE_7:
-            modcol_path = modcol.path  # type:ignore[attr-defined]
-        else:
-            modcol_path = Path(str(modcol.fspath))
+        modcol_path = modcol.path
 
         modcol_path.write_text(
             textwrap.dedent(
                 """
                 def test_func():
                     assert 1
                 def test_new():
@@ -173,28 +169,62 @@
             textwrap.dedent(
                 """
                 def test_func():
                     assert 0
                 """
             )
         )
-        if PYTEST_GTE_7:
-            parent = modcol.path.parent.parent  # type: ignore[attr-defined]
-        else:
-            parent = Path(modcol.fspath.dirpath().dirpath())
+        parent = modcol.path.parent.parent
         monkeypatch.chdir(parent)
         modcol.config.args = [
             str(Path(x).relative_to(parent)) for x in modcol.config.args
         ]
         control = RemoteControl(modcol.config)
         control.loop_once()
         assert control.failures
         control.loop_once()
         assert control.failures
 
+    def test_ignore_sys_path_hook_entry(
+        self, pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch
+    ) -> None:
+        # Modifying sys.path as seen by the worker process is a bit tricky,
+        # because any changes made in the current process do not carry over.
+        # However, we can leverage the `sitecustomize` behavior to run arbitrary
+        # code when the subprocess interpreter is starting up. We just need to
+        # install our module in the search path, which we can accomplish by
+        # adding a temporary directory to PYTHONPATH.
+        tmpdir = tempfile.TemporaryDirectory()
+        with open(pathlib.Path(tmpdir.name) / "sitecustomize.py", "w") as custom:
+            print(
+                textwrap.dedent(
+                    """
+                    import sys
+                    sys.path.append('dummy.__path_hook__')
+                    """
+                ),
+                file=custom,
+            )
+
+        monkeypatch.setenv("PYTHONPATH", tmpdir.name, prepend=":")
+
+        item = pytester.getitem(
+            textwrap.dedent(
+                """
+                def test_func():
+                    import sys
+                    assert "dummy.__path_hook__" in sys.path
+                """
+            )
+        )
+        control = RemoteControl(item.config)
+        control.setup()
+        topdir, failures = control.runsession()[:2]
+        assert not failures
+
 
 class TestLooponFailing:
     def test_looponfail_from_fail_to_ok(self, pytester: pytest.Pytester) -> None:
         modcol = pytester.getmodulecol(
             textwrap.dedent(
                 """
                 def test_one():
@@ -205,26 +235,25 @@
                 """
             )
         )
         remotecontrol = RemoteControl(modcol.config)
         remotecontrol.loop_once()
         assert len(remotecontrol.failures) == 1
 
-        modcol_path = modcol.path if PYTEST_GTE_7 else Path(modcol.fspath)
-        modcol_path.write_text(
+        modcol.path.write_text(
             textwrap.dedent(
                 """
                 def test_one():
                     assert 1
                 def test_two():
                     assert 1
                 """
             )
         )
-        removepyc(modcol_path)
+        removepyc(modcol.path)
         remotecontrol.loop_once()
         assert not remotecontrol.failures
 
     def test_looponfail_from_one_to_two_tests(self, pytester: pytest.Pytester) -> None:
         modcol = pytester.getmodulecol(
             textwrap.dedent(
                 """
@@ -234,26 +263,25 @@
             )
         )
         remotecontrol = RemoteControl(modcol.config)
         remotecontrol.loop_once()
         assert len(remotecontrol.failures) == 1
         assert "test_one" in remotecontrol.failures[0]
 
-        modcol_path = modcol.path if PYTEST_GTE_7 else Path(modcol.fspath)
-        modcol_path.write_text(
+        modcol.path.write_text(
             textwrap.dedent(
                 """
                 def test_one():
                     assert 1 # passes now
                 def test_two():
                     assert 0 # new and fails
                 """
             )
         )
-        removepyc(modcol_path)
+        removepyc(modcol.path)
         remotecontrol.loop_once()
         assert len(remotecontrol.failures) == 0
         remotecontrol.loop_once()
         assert len(remotecontrol.failures) == 1
         assert "test_one" not in remotecontrol.failures[0]
         assert "test_two" in remotecontrol.failures[0]
 
@@ -300,15 +328,15 @@
                     assert 0
                 """
             )
         )
         remotecontrol = RemoteControl(modcol.config)
         orig_runsession = remotecontrol.runsession
 
-        def runsession_dups():
+        def runsession_dups() -> tuple[list[str], list[str], bool]:
             # twisted.trial test cases may report multiple errors.
             failures, reports, collection_failed = orig_runsession()
             print(failures)
             return failures * 2, reports, collection_failed
 
         monkeypatch.setattr(remotecontrol, "runsession", runsession_dups)
         remotecontrol.loop_once()
```

### Comparing `pytest-xdist-3.5.0/testing/test_newhooks.py` & `pytest_xdist-3.6.0/testing/test_newhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
             def test_a(): pass
             def test_b(): pass
             def test_c(): pass
         """
         )
 
     def test_runtest_logreport(self, pytester: pytest.Pytester) -> None:
-        """Test that log reports from pytest_runtest_logreport when running
-        with xdist contain "node", "nodeid", "worker_id", and "testrun_uid" attributes. (#8)
-        """
+        """Test that log reports from pytest_runtest_logreport when running with
+        xdist contain "node", "nodeid", "worker_id", and "testrun_uid"
+        attributes (#8)."""
         pytester.makeconftest(
             """
             def pytest_runtest_logreport(report):
                 if hasattr(report, 'node'):
                     if report.when == "call":
                         workerid = report.node.workerinput['workerid']
                         testrunuid = report.node.workerinput['testrunuid']
```

### Comparing `pytest-xdist-3.5.0/testing/test_plugin.py` & `pytest_xdist-3.6.0/testing/test_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from contextlib import suppress
+import os
 from pathlib import Path
 import sys
-import os
 
 import execnet
-from xdist.workermanage import NodeManager
-
 import pytest
 
+from xdist.workermanage import NodeManager
+
 
 @pytest.fixture
-def monkeypatch_3_cpus(monkeypatch: pytest.MonkeyPatch):
-    """Make pytest-xdist believe the system has 3 CPUs"""
+def monkeypatch_3_cpus(monkeypatch: pytest.MonkeyPatch) -> None:
+    """Make pytest-xdist believe the system has 3 CPUs."""
     # block import
-    monkeypatch.setitem(sys.modules, "psutil", None)  # type: ignore
+    monkeypatch.setitem(sys.modules, "psutil", None)
     monkeypatch.delattr(os, "sched_getaffinity", raising=False)
     monkeypatch.setattr(os, "cpu_count", lambda: 3)
 
 
 def test_dist_incompatibility_messages(pytester: pytest.Pytester) -> None:
     result = pytester.runpytest("--pdb", "--looponfail")
     assert result.ret != 0
@@ -44,14 +44,31 @@
     check_options(config)
     assert config.option.dist == "load"
     assert config.option.tx == ["popen"] * 2
     config = pytester.parseconfigure("-d")
     check_options(config)
     assert config.option.dist == "load"
 
+    config = pytester.parseconfigure("--numprocesses", "0")
+    check_options(config)
+    assert config.option.dist == "no"
+    assert config.option.tx == []
+
+    config = pytester.parseconfigure("--numprocesses", "0", "-d")
+    check_options(config)
+    assert config.option.dist == "no"
+    assert config.option.tx == []
+
+    config = pytester.parseconfigure(
+        "--numprocesses", "0", "--dist", "each", "--tx", "2*popen"
+    )
+    check_options(config)
+    assert config.option.dist == "no"
+    assert config.option.tx == []
+
 
 def test_auto_detect_cpus(
     pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch
 ) -> None:
     from xdist.plugin import pytest_cmdline_main as check_options
 
     monkeypatch.delenv("PYTEST_XDIST_AUTO_NUM_WORKERS", raising=False)
@@ -73,25 +90,20 @@
     config = pytester.parseconfigure("-n2")
     assert config.getoption("numprocesses") == 2
 
     config = pytester.parseconfigure("-nauto")
     check_options(config)
     assert config.getoption("numprocesses") == 99
 
-    config = pytester.parseconfigure("-nauto", "--pdb")
-    check_options(config)
-    assert config.getoption("usepdb")
-    assert config.getoption("numprocesses") == 0
-    assert config.getoption("dist") == "no"
-
-    config = pytester.parseconfigure("-nlogical", "--pdb")
-    check_options(config)
-    assert config.getoption("usepdb")
-    assert config.getoption("numprocesses") == 0
-    assert config.getoption("dist") == "no"
+    for numprocesses in (0, "auto", "logical"):
+        config = pytester.parseconfigure(f"-n{numprocesses}", "--pdb")
+        check_options(config)
+        assert config.getoption("usepdb")
+        assert config.getoption("numprocesses") == 0
+        assert config.getoption("dist") == "no"
 
     monkeypatch.delattr(os, "sched_getaffinity", raising=False)
     monkeypatch.setenv("TRAVIS", "true")
     config = pytester.parseconfigure("-nauto")
     check_options(config)
     assert config.getoption("numprocesses") == 2
 
@@ -112,15 +124,15 @@
 
     config = pytester.parseconfigure("-nlogical")
     check_options(config)
     assert config.getoption("numprocesses") == 84
 
 
 def test_auto_detect_cpus_os(
-    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus
+    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus: None
 ) -> None:
     from xdist.plugin import pytest_cmdline_main as check_options
 
     monkeypatch.delenv("PYTEST_XDIST_AUTO_NUM_WORKERS", raising=False)
 
     config = pytester.parseconfigure("-nauto")
     check_options(config)
@@ -173,15 +185,15 @@
 
     config = pytester.parseconfigure("-nlogical")
     check_options(config)
     assert config.getoption("numprocesses") == 8
 
 
 def test_hook_auto_num_workers_none(
-    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus
+    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus: None
 ) -> None:
     # Returning None from a hook to skip it is pytest behavior,
     # but we document it so let's test it.
     from xdist.plugin import pytest_cmdline_main as check_options
 
     monkeypatch.delenv("PYTEST_XDIST_AUTO_NUM_WORKERS", raising=False)
 
@@ -215,28 +227,28 @@
 
     config = pytester.parseconfigure("-nlogical")
     check_options(config)
     assert config.getoption("numprocesses") == 7
 
 
 def test_envvar_auto_num_workers_warn(
-    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus
+    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus: None
 ) -> None:
     from xdist.plugin import pytest_cmdline_main as check_options
 
     monkeypatch.setenv("PYTEST_XDIST_AUTO_NUM_WORKERS", "fourscore")
 
     config = pytester.parseconfigure("-nauto")
     with pytest.warns(UserWarning):
         check_options(config)
     assert config.getoption("numprocesses") == 3
 
 
 def test_auto_num_workers_hook_overrides_envvar(
-    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus
+    pytester: pytest.Pytester, monkeypatch: pytest.MonkeyPatch, monkeypatch_3_cpus: None
 ) -> None:
     from xdist.plugin import pytest_cmdline_main as check_options
 
     monkeypatch.setenv("PYTEST_XDIST_AUTO_NUM_WORKERS", "987")
     pytester.makeconftest(
         """
         def pytest_xdist_auto_num_workers():
```

### Comparing `pytest-xdist-3.5.0/testing/test_remote.py` & `pytest_xdist-3.6.0/testing/test_remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,115 @@
+from __future__ import annotations
+
+import marshal
 import pprint
-import pytest
+from queue import Queue
 import sys
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import Dict
+from typing import Union
 import uuid
 
-from xdist.workermanage import WorkerController
 import execnet
-import marshal
+import pytest
+
+from xdist.workermanage import NodeManager
+from xdist.workermanage import WorkerController
 
-from queue import Queue
 
 WAIT_TIMEOUT = 10.0
 
 
-def check_marshallable(d):
+def check_marshallable(d: object) -> None:
     try:
-        marshal.dumps(d)
-    except ValueError:
+        marshal.dumps(d)  # type: ignore[arg-type]
+    except ValueError as e:
         pprint.pprint(d)
-        raise ValueError("not marshallable")
+        raise ValueError("not marshallable") from e
 
 
 class EventCall:
-    def __init__(self, eventcall):
+    def __init__(self, eventcall: tuple[str, dict[str, Any]]) -> None:
         self.name, self.kwargs = eventcall
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"<EventCall {self.name}(**{self.kwargs})>"
 
 
 class WorkerSetup:
-    def __init__(self, request, pytester: pytest.Pytester) -> None:
+    def __init__(
+        self, request: pytest.FixtureRequest, pytester: pytest.Pytester
+    ) -> None:
         self.request = request
         self.pytester = pytester
         self.use_callback = False
         self.events = Queue()  # type: ignore[var-annotated]
 
     def setup(self) -> None:
         self.pytester.chdir()
         # import os ; os.environ['EXECNET_DEBUG'] = "2"
-        self.gateway = execnet.makegateway()
+        self.gateway = execnet.makegateway("execmodel=main_thread_only//popen")
         self.config = config = self.pytester.parseconfigure()
         putevent = self.events.put if self.use_callback else None
 
         class DummyMananger:
             testrunuid = uuid.uuid4().hex
             specs = [0, 1]
 
-        self.slp = WorkerController(DummyMananger, self.gateway, config, putevent)
+        nodemanager = cast(NodeManager, DummyMananger)
+
+        self.slp = WorkerController(
+            nodemanager=nodemanager,
+            gateway=self.gateway,
+            config=config,
+            putevent=putevent,  # type: ignore[arg-type]
+        )
         self.request.addfinalizer(self.slp.ensure_teardown)
         self.slp.setup()
 
-    def popevent(self, name=None):
+    def popevent(self, name: str | None = None) -> EventCall:
         while 1:
             if self.use_callback:
                 data = self.events.get(timeout=WAIT_TIMEOUT)
             else:
                 data = self.slp.channel.receive(timeout=WAIT_TIMEOUT)
             ev = EventCall(data)
             if name is None or ev.name == name:
                 return ev
             print(f"skipping {ev}")
 
-    def sendcommand(self, name, **kwargs):
+    def sendcommand(self, name: str, **kwargs: Any) -> None:
         self.slp.sendcommand(name, **kwargs)
 
 
 @pytest.fixture
-def worker(request, pytester: pytest.Pytester) -> WorkerSetup:
+def worker(request: pytest.FixtureRequest, pytester: pytest.Pytester) -> WorkerSetup:
     return WorkerSetup(request, pytester)
 
 
-@pytest.mark.xfail(reason="#59")
-def test_remoteinitconfig(pytester: pytest.Pytester) -> None:
-    from xdist.remote import remote_initconfig
-
-    config1 = pytester.parseconfig()
-    config2 = remote_initconfig(config1.option.__dict__, config1.args)
-    assert config2.option.__dict__ == config1.option.__dict__
-    assert config2.pluginmanager.getplugin("terminal") in (-1, None)
-
-
 class TestWorkerInteractor:
+    UnserializerReport = Callable[
+        [Dict[str, Any]], Union[pytest.CollectReport, pytest.TestReport]
+    ]
+
     @pytest.fixture
-    def unserialize_report(self, pytestconfig):
-        def unserialize(data):
-            return pytestconfig.hook.pytest_report_from_serializable(
+    def unserialize_report(self, pytestconfig: pytest.Config) -> UnserializerReport:
+        def unserialize(
+            data: dict[str, Any],
+        ) -> pytest.CollectReport | pytest.TestReport:
+            return pytestconfig.hook.pytest_report_from_serializable(  # type: ignore[no-any-return]
                 config=pytestconfig, data=data
             )
 
         return unserialize
 
     def test_basic_collect_and_runtests(
-        self, worker: WorkerSetup, unserialize_report
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
     ) -> None:
         worker.pytester.makepyfile(
             """
             def test_func():
                 pass
         """
         )
@@ -120,45 +134,52 @@
         rep = unserialize_report(ev.kwargs["data"])
         assert rep.nodeid.endswith("::test_func")
         assert rep.passed
         assert rep.when == "call"
         ev = worker.popevent("workerfinished")
         assert "workeroutput" in ev.kwargs
 
-    def test_remote_collect_skip(self, worker: WorkerSetup, unserialize_report) -> None:
+    def test_remote_collect_skip(
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
+    ) -> None:
         worker.pytester.makepyfile(
             """
             import pytest
             pytest.skip("hello", allow_module_level=True)
         """
         )
         worker.setup()
         ev = worker.popevent("collectionstart")
         assert not ev.kwargs
         ev = worker.popevent()
         assert ev.name == "collectreport"
         rep = unserialize_report(ev.kwargs["data"])
         assert rep.skipped
+        assert isinstance(rep.longrepr, tuple)
         assert rep.longrepr[2] == "Skipped: hello"
         ev = worker.popevent("collectionfinish")
         assert not ev.kwargs["ids"]
 
-    def test_remote_collect_fail(self, worker: WorkerSetup, unserialize_report) -> None:
+    def test_remote_collect_fail(
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
+    ) -> None:
         worker.pytester.makepyfile("""aasd qwe""")
         worker.setup()
         ev = worker.popevent("collectionstart")
         assert not ev.kwargs
         ev = worker.popevent()
         assert ev.name == "collectreport"
         rep = unserialize_report(ev.kwargs["data"])
         assert rep.failed
         ev = worker.popevent("collectionfinish")
         assert not ev.kwargs["ids"]
 
-    def test_runtests_all(self, worker: WorkerSetup, unserialize_report) -> None:
+    def test_runtests_all(
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
+    ) -> None:
         worker.pytester.makepyfile(
             """
             def test_func(): pass
             def test_func2(): pass
         """
         )
         worker.setup()
@@ -169,15 +190,15 @@
         assert not ev.kwargs
         ev = worker.popevent("collectionfinish")
         ids = ev.kwargs["ids"]
         assert len(ids) == 2
         worker.sendcommand("runtests_all")
         worker.sendcommand("shutdown")
         for func in "::test_func", "::test_func2":
-            for i in range(3):  # setup/call/teardown
+            for _ in range(3):  # setup/call/teardown
                 ev = worker.popevent("testreport")
                 assert ev.name == "testreport"
                 rep = unserialize_report(ev.kwargs["data"])
                 assert rep.nodeid.endswith(func)
         ev = worker.popevent("workerfinished")
         assert "workeroutput" in ev.kwargs
 
@@ -210,21 +231,23 @@
         )
 
     def test_process_from_remote_error_handling(
         self, worker: WorkerSetup, capsys: pytest.CaptureFixture[str]
     ) -> None:
         worker.use_callback = True
         worker.setup()
-        worker.slp.process_from_remote(("<nonono>", ()))
+        worker.slp.process_from_remote(("<nonono>", {}))
         out, err = capsys.readouterr()
         assert "INTERNALERROR> ValueError: unknown event: <nonono>" in out
         ev = worker.popevent()
         assert ev.name == "errordown"
 
-    def test_steal_work(self, worker: WorkerSetup, unserialize_report) -> None:
+    def test_steal_work(
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
+    ) -> None:
         worker.pytester.makepyfile(
             """
             import time
             def test_func(): time.sleep(1)
             def test_func2(): pass
             def test_func3(): pass
             def test_func4(): pass
@@ -267,15 +290,17 @@
             rep = unserialize_report(ev.kwargs["data"])
             assert rep.nodeid.endswith("::test_func4")
             assert rep.when == when
 
         ev = worker.popevent("workerfinished")
         assert "workeroutput" in ev.kwargs
 
-    def test_steal_empty_queue(self, worker: WorkerSetup, unserialize_report) -> None:
+    def test_steal_empty_queue(
+        self, worker: WorkerSetup, unserialize_report: UnserializerReport
+    ) -> None:
         worker.pytester.makepyfile(
             """
             def test_func(): pass
             def test_func2(): pass
         """
         )
         worker.setup()
@@ -334,28 +359,24 @@
     assert result.ret == 0
 
 
 def test_remote_mainargv(pytester: pytest.Pytester) -> None:
     outer_argv = sys.argv
 
     pytester.makepyfile(
-        """
+        f"""
         def test_mainargv(request):
-            assert request.config.workerinput["mainargv"] == {!r}
-        """.format(
-            outer_argv
-        )
+            assert request.config.workerinput["mainargv"] == {outer_argv!r}
+        """
     )
     result = pytester.runpytest("-n1")
     assert result.ret == 0
 
 
-def test_remote_usage_prog(pytester: pytest.Pytester, request) -> None:
-    if not hasattr(request.config._parser, "prog"):
-        pytest.skip("prog not available in config parser")
+def test_remote_usage_prog(pytester: pytest.Pytester) -> None:
     pytester.makeconftest(
         """
         import pytest
 
         config_parser = None
 
         @pytest.fixture
```

### Comparing `pytest-xdist-3.5.0/testing/test_workermanage.py` & `pytest_xdist-3.6.0/testing/test_workermanage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-import execnet
-import pytest
+from __future__ import annotations
+
+from pathlib import Path
 import shutil
 import textwrap
 import warnings
-from pathlib import Path
+
+import execnet
+import pytest
 from util import generate_warning
+
 from xdist import workermanage
 from xdist._path import visit_path
 from xdist.remote import serialize_warning_message
-from xdist.workermanage import HostRSync, NodeManager, unserialize_warning_message
+from xdist.workermanage import HostRSync
+from xdist.workermanage import NodeManager
+from xdist.workermanage import unserialize_warning_message
+
 
 pytest_plugins = "pytester"
 
 
 @pytest.fixture
-def hookrecorder(request, config, pytester: pytest.Pytester):
+def hookrecorder(
+    config: pytest.Config, pytester: pytest.Pytester
+) -> pytest.HookRecorder:
     hookrecorder = pytester.make_hook_recorder(config.pluginmanager)
     return hookrecorder
 
 
 @pytest.fixture
-def config(pytester: pytest.Pytester):
+def config(pytester: pytest.Pytester) -> pytest.Config:
     return pytester.parseconfig()
 
 
 @pytest.fixture
 def source(tmp_path: Path) -> Path:
     source = tmp_path / "source"
     source.mkdir()
@@ -35,86 +44,92 @@
 def dest(tmp_path: Path) -> Path:
     dest = tmp_path / "dest"
     dest.mkdir()
     return dest
 
 
 @pytest.fixture
-def workercontroller(monkeypatch: pytest.MonkeyPatch):
+def workercontroller(monkeypatch: pytest.MonkeyPatch) -> None:
     class MockController:
-        def __init__(self, *args):
+        def __init__(self, *args: object) -> None:
             pass
 
-        def setup(self):
+        def setup(self) -> None:
             pass
 
     monkeypatch.setattr(workermanage, "WorkerController", MockController)
-    return MockController
 
 
 class TestNodeManagerPopen:
-    def test_popen_no_default_chdir(self, config) -> None:
+    def test_popen_no_default_chdir(self, config: pytest.Config) -> None:
         gm = NodeManager(config, ["popen"])
         assert gm.specs[0].chdir is None
 
-    def test_default_chdir(self, config) -> None:
+    def test_default_chdir(self, config: pytest.Config) -> None:
         specs = ["ssh=noco", "socket=xyz"]
         for spec in NodeManager(config, specs).specs:
             assert spec.chdir == "pyexecnetcache"
         for spec in NodeManager(config, specs, defaultchdir="abc").specs:
             assert spec.chdir == "abc"
 
     def test_popen_makegateway_events(
-        self, config, hookrecorder, workercontroller
+        self,
+        config: pytest.Config,
+        hookrecorder: pytest.HookRecorder,
+        workercontroller: None,
     ) -> None:
         hm = NodeManager(config, ["popen"] * 2)
-        hm.setup_nodes(None)
+        hm.setup_nodes(None)  # type: ignore[arg-type]
         call = hookrecorder.popcall("pytest_xdist_setupnodes")
         assert len(call.specs) == 2
 
         call = hookrecorder.popcall("pytest_xdist_newgateway")
-        assert call.gateway.spec == execnet.XSpec("popen")
+        assert call.gateway.spec == execnet.XSpec("execmodel=main_thread_only//popen")
         assert call.gateway.id == "gw0"
         call = hookrecorder.popcall("pytest_xdist_newgateway")
         assert call.gateway.id == "gw1"
         assert len(hm.group) == 2
         hm.teardown_nodes()
         assert not len(hm.group)
 
     def test_popens_rsync(
-        self, config, source: Path, dest: Path, workercontroller
+        self,
+        config: pytest.Config,
+        source: Path,
+        dest: Path,
+        workercontroller: None,
     ) -> None:
         hm = NodeManager(config, ["popen"] * 2)
-        hm.setup_nodes(None)
+        hm.setup_nodes(None)  # type: ignore[arg-type]
         assert len(hm.group) == 2
         for gw in hm.group:
 
             class pseudoexec:
                 args = []  # type: ignore[var-annotated]
 
-                def __init__(self, *args):
+                def __init__(self, *args: object) -> None:
                     self.args.extend(args)
 
-                def waitclose(self):
+                def waitclose(self) -> None:
                     pass
 
-            gw.remote_exec = pseudoexec
+            gw.remote_exec = pseudoexec  # type: ignore[assignment]
         notifications = []
         for gw in hm.group:
             hm.rsync(gw, source, notify=lambda *args: notifications.append(args))
         assert not notifications
         hm.teardown_nodes()
         assert not len(hm.group)
-        assert "sys.path.insert" in gw.remote_exec.args[0]
+        assert "sys.path.insert" in gw.remote_exec.args[0]  # type: ignore[attr-defined]
 
     def test_rsync_popen_with_path(
-        self, config, source: Path, dest: Path, workercontroller
+        self, config: pytest.Config, source: Path, dest: Path, workercontroller: None
     ) -> None:
         hm = NodeManager(config, ["popen//chdir=%s" % dest] * 1)
-        hm.setup_nodes(None)
+        hm.setup_nodes(None)  # type: ignore[arg-type]
         source.joinpath("dir1", "dir2").mkdir(parents=True)
         source.joinpath("dir1", "dir2", "hello").touch()
         notifications = []
         for gw in hm.group:
             hm.rsync(gw, source, notify=lambda *args: notifications.append(args))
         assert len(notifications) == 1
         assert notifications[0] == ("rsyncrootready", hm.group["gw0"].spec, source)
@@ -122,23 +137,23 @@
         dest = dest.joinpath(source.name)
         assert dest.joinpath("dir1").exists()
         assert dest.joinpath("dir1", "dir2").exists()
         assert dest.joinpath("dir1", "dir2", "hello").exists()
 
     def test_rsync_same_popen_twice(
         self,
-        config,
+        config: pytest.Config,
         source: Path,
         dest: Path,
-        hookrecorder,
-        workercontroller,
+        hookrecorder: pytest.HookRecorder,
+        workercontroller: None,
     ) -> None:
         hm = NodeManager(config, ["popen//chdir=%s" % dest] * 2)
         hm.roots = []
-        hm.setup_nodes(None)
+        hm.setup_nodes(None)  # type: ignore[arg-type]
         source.joinpath("dir1", "dir2").mkdir(parents=True)
         source.joinpath("dir1", "dir2", "hello").touch()
         gw = hm.group[0]
         hm.rsync(gw, source)
         call = hookrecorder.popcall("pytest_xdist_rsyncstart")
         assert call.source == source
         assert len(call.gateways) == 1
@@ -158,15 +173,15 @@
         source.joinpath("somedir", "editfile~").touch()
         syncer = HostRSync(source, ignores=NodeManager.DEFAULT_IGNORES)
         files = list(visit_path(source, recurse=syncer.filter, filter=syncer.filter))
         names = {x.name for x in files}
         assert names == {"dir", "file.txt", "somedir"}
 
     def test_hrsync_one_host(self, source: Path, dest: Path) -> None:
-        gw = execnet.makegateway("popen//chdir=%s" % dest)
+        gw = execnet.makegateway("execmodel=main_thread_only//popen//chdir=%s" % dest)
         finished = []
         rsync = HostRSync(source)
         rsync.add_target_host(gw, finished=lambda: finished.append(1))
         source.joinpath("hello.py").write_text("world")
         rsync.send()
         gw.exit()
         assert dest.joinpath(source.name, "hello.py").exists()
@@ -191,64 +206,79 @@
         p = Path(p)
         print("remote curdir", p)
         assert p == dest.joinpath(config.rootpath.name)
         assert p.joinpath("dir1").check()
         assert p.joinpath("dir1", "file1").check()
 
     def test_popen_rsync_subdir(
-        self, pytester: pytest.Pytester, source: Path, dest: Path, workercontroller
+        self,
+        pytester: pytest.Pytester,
+        source: Path,
+        dest: Path,
+        workercontroller: None,
     ) -> None:
         dir1 = source / "dir1"
         dir1.mkdir()
         dir2 = dir1 / "dir2"
         dir2.mkdir()
         dir2.joinpath("hello").touch()
         for rsyncroot in (dir1, source):
             shutil.rmtree(str(dest), ignore_errors=True)
             nodemanager = NodeManager(
                 pytester.parseconfig(
                     "--tx", "popen//chdir=%s" % dest, "--rsyncdir", rsyncroot, source
                 )
             )
-            nodemanager.setup_nodes(None)  # calls .rsync_roots()
+            # calls .rsync_roots()
+            nodemanager.setup_nodes(None)  # type: ignore[arg-type]
             if rsyncroot == source:
                 dest = dest.joinpath("source")
             assert dest.joinpath("dir1").exists()
             assert dest.joinpath("dir1", "dir2").exists()
             assert dest.joinpath("dir1", "dir2", "hello").exists()
             nodemanager.teardown_nodes()
 
     @pytest.mark.parametrize(
-        "flag, expects_report", [("-q", False), ("", False), ("-v", True)]
+        ["flag", "expects_report"],
+        [
+            ("-q", False),
+            ("", False),
+            ("-v", True),
+        ],
     )
     def test_rsync_report(
         self,
         pytester: pytest.Pytester,
         source: Path,
         dest: Path,
-        workercontroller,
+        workercontroller: None,
         capsys: pytest.CaptureFixture[str],
         flag: str,
         expects_report: bool,
     ) -> None:
         dir1 = source / "dir1"
         dir1.mkdir()
         args = ["--tx", "popen//chdir=%s" % dest, "--rsyncdir", str(dir1), str(source)]
         if flag:
             args.append(flag)
         nodemanager = NodeManager(pytester.parseconfig(*args))
-        nodemanager.setup_nodes(None)  # calls .rsync_roots()
+        # calls .rsync_roots()
+        nodemanager.setup_nodes(None)  # type: ignore[arg-type]
         out, _ = capsys.readouterr()
         if expects_report:
             assert "<= pytest/__init__.py" in out
         else:
             assert "<= pytest/__init__.py" not in out
 
     def test_init_rsync_roots(
-        self, pytester: pytest.Pytester, source: Path, dest: Path, workercontroller
+        self,
+        pytester: pytest.Pytester,
+        source: Path,
+        dest: Path,
+        workercontroller: None,
     ) -> None:
         dir2 = source.joinpath("dir1", "dir2")
         dir2.mkdir(parents=True)
         source.joinpath("dir1", "somefile").mkdir()
         dir2.joinpath("hello").touch()
         source.joinpath("bogusdir").mkdir()
         source.joinpath("bogusdir", "file").touch()
@@ -258,21 +288,26 @@
                 [pytest]
                 rsyncdirs=dir1/dir2
                 """
             )
         )
         config = pytester.parseconfig(source)
         nodemanager = NodeManager(config, ["popen//chdir=%s" % dest])
-        nodemanager.setup_nodes(None)  # calls .rsync_roots()
+        # calls .rsync_roots()
+        nodemanager.setup_nodes(None)  # type: ignore[arg-type]
         assert dest.joinpath("dir2").exists()
         assert not dest.joinpath("dir1").exists()
         assert not dest.joinpath("bogus").exists()
 
     def test_rsyncignore(
-        self, pytester: pytest.Pytester, source: Path, dest: Path, workercontroller
+        self,
+        pytester: pytest.Pytester,
+        source: Path,
+        dest: Path,
+        workercontroller: None,
     ) -> None:
         dir2 = source.joinpath("dir1", "dir2")
         dir2.mkdir(parents=True)
         source.joinpath("dir5", "dir6").mkdir(parents=True)
         source.joinpath("dir5", "dir6", "bogus").touch()
         source.joinpath("dir5", "file").touch()
         dir2.joinpath("hello").touch()
@@ -288,31 +323,37 @@
                 rsyncignore = dir1/dir2 dir5/dir6 foo*
                 """
             )
         )
         config = pytester.parseconfig(source)
         config.option.rsyncignore = ["bar"]
         nodemanager = NodeManager(config, ["popen//chdir=%s" % dest])
-        nodemanager.setup_nodes(None)  # calls .rsync_roots()
+        # calls .rsync_roots()
+        nodemanager.setup_nodes(None)  # type: ignore[arg-type]
         assert dest.joinpath("dir1").exists()
         assert not dest.joinpath("dir1", "dir2").exists()
         assert dest.joinpath("dir5", "file").exists()
         assert not dest.joinpath("dir6").exists()
         assert not dest.joinpath("foo").exists()
         assert not dest.joinpath("bar").exists()
 
     def test_optimise_popen(
-        self, pytester: pytest.Pytester, source: Path, dest: Path, workercontroller
+        self,
+        pytester: pytest.Pytester,
+        source: Path,
+        dest: Path,
+        workercontroller: None,
     ) -> None:
         specs = ["popen"] * 3
         source.joinpath("conftest.py").write_text("rsyncdirs = ['a']")
         source.joinpath("a").mkdir()
         config = pytester.parseconfig(source)
         nodemanager = NodeManager(config, specs)
-        nodemanager.setup_nodes(None)  # calls .rysnc_roots()
+        # calls .rysnc_roots()
+        nodemanager.setup_nodes(None)  # type: ignore[arg-type]
         for gwspec in nodemanager.specs:
             assert gwspec._samefilesystem()
             assert not gwspec.chdir
 
     def test_ssh_setup_nodes(self, specssh: str, pytester: pytest.Pytester) -> None:
         pytester.makepyfile(
             __init__="",
@@ -340,17 +381,16 @@
         "Imported",
         pytest.param(
             "Nested",
             marks=pytest.mark.xfail(reason="Nested warning classes are not supported."),
         ),
     ],
 )
-def test_unserialize_warning_msg(w_cls):
-    """Test that warning serialization process works well"""
-
+def test_unserialize_warning_msg(w_cls: type[Warning] | str) -> None:
+    """Test that warning serialization process works well."""
     # Create a test warning message
     with pytest.warns(UserWarning) as w:
         if not isinstance(w_cls, str):
             warnings.warn("hello", w_cls)
         elif w_cls == "Imported":
             generate_warning()
         elif w_cls == "Nested":
@@ -382,17 +422,16 @@
 
 class MyWarningUnknown(UserWarning):
     # Changing the __module__ attribute is only safe if class can be imported
     # from there
     __module__ = "unknown"
 
 
-def test_warning_serialization_tweaked_module():
-    """Test for GH#404"""
-
+def test_warning_serialization_tweaked_module() -> None:
+    """Test for GH#404."""
     # Create a test warning message
     with pytest.warns(UserWarning) as w:
         warnings.warn("hello", MyWarningUnknown)
 
     # Unpack
     assert len(w) == 1
     w_msg = w[0]
```

### Comparing `pytest-xdist-3.5.0/tox.ini` & `pytest_xdist-3.6.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tox]
 envlist=
   linting
-  py{37,38,39,310,311,312}-pytestlatest
+  py{38,39,310,311,312}-pytestlatest
   py310-pytestmain
   py310-psutil
   py310-setproctitle
 isolated_build = true
 [testenv]
 extras = testing
 deps =
+  pytestmin: pytest==7.0.0
   pytestlatest: pytest
   pytestmain: git+https://github.com/pytest-dev/pytest.git
 commands=
   pytest {posargs}
 
 [testenv:py310-psutil]
 extras =
@@ -59,11 +60,7 @@
     sphinx-build -W --keep-going -b html docs docs/_build/html {posargs:}
 
 [pytest]
 # pytest-services also defines a worker_id fixture, disable
 # it so they don't conflict with each other (#611).
 addopts = -ra -p no:pytest-services
 testpaths = testing
-
-[flake8]
-max-line-length = 120
-ignore = E203,W503
```

