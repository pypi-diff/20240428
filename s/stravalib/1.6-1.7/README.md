# Comparing `tmp/stravalib-1.6.tar.gz` & `tmp/stravalib-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stravalib-1.6.tar", last modified: Sat Jan 27 20:51:54 2024, max compression
+gzip compressed data, was "stravalib-1.7.tar", last modified: Sat Apr 27 23:10:08 2024, max compression
```

## Comparing `stravalib-1.6.tar` & `stravalib-1.7.tar`

### file list

```diff
@@ -1,128 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.996626 stravalib-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-27 20:51:41.000000 stravalib-1.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-27 20:51:41.000000 stravalib-1.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.980626 stravalib-1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.980626 stravalib-1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-01-27 20:51:41.000000 stravalib-1.6/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-27 20:51:41.000000 stravalib-1.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-01-27 20:51:41.000000 stravalib-1.6/.github/ISSUE_TEMPLATE/documentation-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-01-27 20:51:41.000000 stravalib-1.6/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.980626 stravalib-1.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-01-27 20:51:41.000000 stravalib-1.6/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-01-27 20:51:41.000000 stravalib-1.6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-01-27 20:51:41.000000 stravalib-1.6/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-27 20:51:41.000000 stravalib-1.6/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-27 20:51:41.000000 stravalib-1.6/.github/workflows/check-strava-api.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-27 20:51:41.000000 stravalib-1.6/.github/workflows/push-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-27 20:51:41.000000 stravalib-1.6/.github/workflows/type-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-27 20:51:41.000000 stravalib-1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-01-27 20:51:41.000000 stravalib-1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-27 20:51:41.000000 stravalib-1.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-01-27 20:51:41.000000 stravalib-1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-01-27 20:51:41.000000 stravalib-1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-27 20:51:41.000000 stravalib-1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-27 20:51:41.000000 stravalib-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-01-27 20:51:53.996626 stravalib-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-01-27 20:51:41.000000 stravalib-1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-01-27 20:51:41.000000 stravalib-1.6/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:41.000000 stravalib-1.6/docs/_static/keepme
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-27 20:51:41.000000 stravalib-1.6/docs/_static/stravalib.css
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-01-27 20:51:41.000000 stravalib-1.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-01-27 20:51:41.000000 stravalib-1.6/docs/contributing/build-release-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-01-27 20:51:41.000000 stravalib-1.6/docs/contributing/development-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-27 20:51:41.000000 stravalib-1.6/docs/contributing/documentation-changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-27 20:51:41.000000 stravalib-1.6/docs/contributing/how-to-contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-01-27 20:51:41.000000 stravalib-1.6/docs/contributing/resources-for-new-contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-27 20:51:41.000000 stravalib-1.6/docs/get-started/activities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-27 20:51:41.000000 stravalib-1.6/docs/get-started/athletes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-01-27 20:51:41.000000 stravalib-1.6/docs/get-started/authenticate-with-strava.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-01-27 20:51:41.000000 stravalib-1.6/docs/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-01-27 20:51:41.000000 stravalib-1.6/docs/get-started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.984626 stravalib-1.6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    78545 2024-01-27 20:51:41.000000 stravalib-1.6/docs/images/stravalib_architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-01-27 20:51:41.000000 stravalib-1.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.988626 stravalib-1.6/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/field-conversions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/strava_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/unithelper.rst
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-27 20:51:41.000000 stravalib-1.6/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-27 20:51:41.000000 stravalib-1.6/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.976626 stravalib-1.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.988626 stravalib-1.6/examples/strava-oauth/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.988626 stravalib-1.6/examples/strava-oauth/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/static/ConnectWithStrava.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.988626 stravalib-1.6/examples/strava-oauth/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/templates/login_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-27 20:51:41.000000 stravalib-1.6/examples/strava-oauth/templates/login_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-01-27 20:51:41.000000 stravalib-1.6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-27 20:51:41.000000 stravalib-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-27 20:51:41.000000 stravalib-1.6/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-27 20:51:41.000000 stravalib-1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 20:51:53.996626 stravalib-1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.976626 stravalib-1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.988626 stravalib-1.6/src/stravalib/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    76301 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38296 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36038 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/strava_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.992626 stravalib-1.6/src/stravalib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/auth_responder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.992626 stravalib-1.6/src/stravalib/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/functional/test_client_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/functional/test_client_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/functional/test_result_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.992626 stravalib-1.6/src/stravalib/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/integration/strava_api_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)    30517 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/integration/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.996626 stravalib-1.6/src/stravalib/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/activity-manual.3.json
--rw-r--r--   0 runner    (1001) docker     (127)    23891 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/activity.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/athlete.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/athlete.3.json
--rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/example_route_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/example_zone_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   451575 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/sample.tcx
--rw-r--r--   0 runner    (1001) docker     (127)   102647 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/resources/strava_swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/test.ini-example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.996626 stravalib-1.6/src/stravalib/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/test_client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/test_field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/tests/unit/test_unithelper.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/unit_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/unithelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.996626 stravalib-1.6/src/stravalib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-01-27 20:51:41.000000 stravalib-1.6/src/stravalib/util/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 20:51:53.996626 stravalib-1.6/src/stravalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 20:51:53.000000 stravalib-1.6/src/stravalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.179026 stravalib-1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 23:09:44.000000 stravalib-1.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-27 23:09:44.000000 stravalib-1.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-27 23:09:44.000000 stravalib-1.7/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-27 23:09:44.000000 stravalib-1.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-27 23:09:44.000000 stravalib-1.7/.github/ISSUE_TEMPLATE/documentation-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-27 23:09:44.000000 stravalib-1.7/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-27 23:09:44.000000 stravalib-1.7/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-27 23:09:44.000000 stravalib-1.7/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-27 23:09:44.000000 stravalib-1.7/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-27 23:09:44.000000 stravalib-1.7/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-27 23:09:44.000000 stravalib-1.7/.github/workflows/check-strava-api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-27 23:09:44.000000 stravalib-1.7/.github/workflows/push-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-27 23:09:44.000000 stravalib-1.7/.github/workflows/type-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-27 23:09:44.000000 stravalib-1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-27 23:09:44.000000 stravalib-1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 23:09:44.000000 stravalib-1.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-27 23:09:44.000000 stravalib-1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 23:09:44.000000 stravalib-1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-27 23:09:44.000000 stravalib-1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-27 23:09:44.000000 stravalib-1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-27 23:10:08.179026 stravalib-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-27 23:09:44.000000 stravalib-1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-04-27 23:09:44.000000 stravalib-1.7/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.163026 stravalib-1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:09:44.000000 stravalib-1.7/docs/_static/keepme
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 23:09:44.000000 stravalib-1.7/docs/_static/stravalib.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-27 23:09:44.000000 stravalib-1.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.167026 stravalib-1.7/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/build-release-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/development-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/documentation-changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/how-to-contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-27 23:09:44.000000 stravalib-1.7/docs/contributing/resources-for-new-contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.167026 stravalib-1.7/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-27 23:09:44.000000 stravalib-1.7/docs/get-started/activities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-27 23:09:44.000000 stravalib-1.7/docs/get-started/athletes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-27 23:09:44.000000 stravalib-1.7/docs/get-started/authenticate-with-strava.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-27 23:09:44.000000 stravalib-1.7/docs/get-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-27 23:09:44.000000 stravalib-1.7/docs/get-started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.167026 stravalib-1.7/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    78545 2024-04-27 23:09:44.000000 stravalib-1.7/docs/images/stravalib_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-27 23:09:44.000000 stravalib-1.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.167026 stravalib-1.7/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/field-conversions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/strava_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/unithelper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-27 23:09:44.000000 stravalib-1.7/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 23:09:44.000000 stravalib-1.7/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-27 23:09:44.000000 stravalib-1.7/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-27 23:09:44.000000 stravalib-1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:10:08.179026 stravalib-1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.159026 stravalib-1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.171026 stravalib-1.7/src/stravalib/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77053 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38296 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36862 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/strava_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.171026 stravalib-1.7/src/stravalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/auth_responder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.171026 stravalib-1.7/src/stravalib/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/integration/strava_api_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31318 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/integration/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.175026 stravalib-1.7/src/stravalib/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/activity-manual.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23891 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/activity.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/athlete.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/athlete.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/example_route_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/example_zone_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   451575 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/sample.tcx
+-rw-r--r--   0 runner    (1001) docker     (127)   102646 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/resources/strava_swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/test.ini-example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.175026 stravalib-1.7/src/stravalib/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_unithelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/tests/unit/test_validate_activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/unit_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/unithelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.175026 stravalib-1.7/src/stravalib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-04-27 23:09:44.000000 stravalib-1.7/src/stravalib/util/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:10:08.175026 stravalib-1.7/src/stravalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 23:10:08.000000 stravalib-1.7/src/stravalib.egg-info/top_level.txt
```

### Comparing `stravalib-1.6/.github/ISSUE_TEMPLATE/bug-report.yml` & `stravalib-1.7/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/.github/ISSUE_TEMPLATE/documentation-issue.yml` & `stravalib-1.7/.github/ISSUE_TEMPLATE/documentation-issue.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/.github/ISSUE_TEMPLATE/feature-request.yml` & `stravalib-1.7/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md` & `stravalib-1.7/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/.github/PULL_REQUEST_TEMPLATE.md` & `stravalib-1.7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/.github/workflows/build-docs.yml` & `stravalib-1.7/.github/workflows/build-docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,41 +6,39 @@
     branches:
       - main
 
 jobs:
   build-doc:
     runs-on: ubuntu-latest
     env:
-      PYTHON-VERSION: "3.10"
+      PYTHON-VERSION: "3.11"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON-VERSION }}
       - name: Upgrade pip & install nox
         run: |
           # install pip=>20.1 to use "pip cache dir"
           python3 -m pip install --upgrade pip
           pip install nox
       - name: Set Variables
         id: set_variables
         shell: bash
         run: |
           echo "PY=$(python -c 'import hashlib, sys;print(hashlib.sha256(sys.version.encode()+sys.executable.encode()).hexdigest())')" >> $GITHUB_OUTPUT
           echo "PIP_CACHE=$(pip cache dir)" >> $GITHUB_OUTPUT
       - name: Cache dependencies
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ steps.set_variables.outputs.PIP_CACHE }}
           key: ${{ runner.os }}-pip-${{ steps.set_variables.outputs.PY }}
       - name: Install dependencies
         run: |
-          python3 -m pip install -r ./requirements.txt
-          python3 -m pip install .
           pip install nox
       - name: Build docs & linkcheck
         run: |
           # Build html and link check
           nox -s docs
       - name: Print doc link failures in the output.txt file
         if: success() || failure()
```

### Comparing `stravalib-1.6/.github/workflows/build-test.yml` & `stravalib-1.7/.github/workflows/build-test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -15,34 +15,34 @@
   build-test:
     name: Test Run (${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           # fetch more than the last single commit to help scm generate proper version
           fetch-depth: 20
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Set Variables
         id: set_variables
         shell: bash
         run: |
           echo "PY=$(python -c 'import hashlib, sys;print(hashlib.sha256(sys.version.encode()+sys.executable.encode()).hexdigest())')" >> $GITHUB_OUTPUT
           echo "PIP_CACHE=$(pip cache dir)" >> $GITHUB_OUTPUT
       - name: Cache dependencies
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ steps.set_variables.outputs.PIP_CACHE }}
           key: ${{ runner.os }}-pip-${{ steps.set_variables.outputs.PY }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install nox
@@ -53,9 +53,13 @@
         run: git fetch origin 'refs/tags/*:refs/tags/*'
         # For now i made a separate tests run so we can see each version
         # build via github actions. There may be a better way to do this.
       - name: Run tests with pytest & nox
         run: |
           nox -s tests-${{ matrix.python-version }}
       - name: Upload coverage to Codecov
-        if: ${{ matrix.os == 'ubuntu-latest' &&  matrix.python-version == '3.10'}}
+        if: ${{ matrix.os == 'ubuntu-latest' &&  matrix.python-version == '3.11'}}
         uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          verbose: true
+          files: ./coverage.xml
```

### Comparing `stravalib-1.6/.github/workflows/check-strava-api.yml` & `stravalib-1.7/.github/workflows/check-strava-api.yml`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,26 @@
   workflow_dispatch:
 
 jobs:
   update-model:
     name: Update Model
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Fetch API
         run: curl https://developers.strava.com/swagger/swagger.json > src/stravalib/tests/resources/strava_swagger.json
       - name: Fetch API Schema
         uses: stravalib/strava_swagger2pydantic@v1
         with:
           model_file: "src/stravalib/strava_model.py"
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@v4
+        uses: peter-evans/create-pull-request@v6
         with:
           add-paths: |
-            stravalib
+            src/stravalib
           commit-message: Strava API Change
           branch: api-change
           delete-branch: true
           title: "[CHANGE] Strava API Change"
           body: |
             There were changes in the Strava API:
             [Please edit this comment to indicate what has changed]
```

### Comparing `stravalib-1.6/.github/workflows/push-pypi.yml` & `stravalib-1.7/.github/workflows/push-pypi.yml`

 * *Files 19% similar despite different names*

```diff
@@ -8,53 +8,43 @@
 jobs:
   build-publish:
     runs-on: ubuntu-latest
     # Only run build action on base repo - not forks
     if: github.repository_owner == 'stravalib'
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           # So scm can view previous commits
           fetch-depth: 100
 
       # Need the tags so that setuptools-scm can form a valid version number
       - name: Fetch git tags
         run: git fetch origin 'refs/tags/*:refs/tags/*'
 
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.9"
+          python-version: "3.10"
 
-      - name: Install requirements
+      - name: Install dependencies
         run: |
-          python -m pip install -r requirements-build.txt
+          python -m pip install --upgrade pip
+          python -m pip install build twine
           pip list
 
       - name: Build package
         run: |
-          python3 -m build
+          python -m build
           echo ""
           echo "Generated files:"
           ls -lh dist/
 
       - name: Check the archives
         run: twine check dist/*
 
-      - name: Publish package on test PyPI on merge
-        # Test push to test pypi on merge to main
-        if: github.event_name == 'push'
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.TEST_PYPI_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
-          # Allow existing releases on test PyPI without errors.
-          # NOT TO BE USED in PyPI!
-          skip_existing: true
-
       - name: Publish package to PyPI
         # Only publish to real PyPI on release
         if: github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `stravalib-1.6/.github/workflows/type-check.yml` & `stravalib-1.7/.github/workflows/type-check.yml`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,32 @@
   mypy:
     name: Run mypy
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python 3.10
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
       - name: Set Variables
         id: set_variables
         shell: bash
         run: |
           echo "PY=$(python -c 'import hashlib, sys;print(hashlib.sha256(sys.version.encode()+sys.executable.encode()).hexdigest())')" >> $GITHUB_OUTPUT
           echo "PIP_CACHE=$(pip cache dir)" >> $GITHUB_OUTPUT
       - name: Cache dependencies
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ steps.set_variables.outputs.PIP_CACHE }}
           key: ubuntu-latest-pip-${{ steps.set_variables.outputs.PY }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r requirements.txt
-          python -m pip install -r requirements-build.txt
+          python -m pip install nox
       - name: List installed packages
         run: python -m pip freeze
       - name: Run tests with mypy
         run: |
           nox -s mypy
```

### Comparing `stravalib-1.6/.gitignore` & `stravalib-1.7/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 stravalib/docs/api
 .vscode/
 stravalib-2023/
 .nox/*
 
 # Ignore Sphinx auto-generated API stubs #
 docs/reference/api
+coverage.xml
```

### Comparing `stravalib-1.6/.pre-commit-config.yaml` & `stravalib-1.7/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,22 @@
       # Lint: Check for files with names that would conflict on a
       # case-insensitive filesystem like MacOS HFS+ or Windows FAT.
       - id: check-case-conflict
       - id: trailing-whitespace
 
   # Linting code using ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.9
+    rev: v0.3.5
     hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
   # Black for auto code formatting
   - repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.3.0
     hooks:
       - id: black
         entry: bash -c 'black "$@"; git add -u' --
         language_version: python3.10
         args: ["--line-length=79"]
 
   - repo: https://github.com/adamchainz/blacken-docs
@@ -57,9 +57,14 @@
       - id: blacken-docs
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         files: ^.*\.(py|md|rst)$
+        exclude: >
+            (?x)^(
+                src/stravalib/strava_model.py|
+                src/stravalib/tests/resources/strava_swagger.json
+            )$
         additional_dependencies:
           - tomli
```

### Comparing `stravalib-1.6/CODE_OF_CONDUCT.md` & `stravalib-1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/CONTRIBUTING.md` & `stravalib-1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/LICENSE.txt` & `stravalib-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/PKG-INFO` & `stravalib-1.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: stravalib
-Version: 1.6
-Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
-Author-email: Hans Lellelid <hans@xmpl.org>
-Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong, Émile Nadeau
-License: Apache 2.0 License
-Project-URL: documentation, https://stravalib.readthedocs.io
-Project-URL: repository, https://github.com/stravalib/stravalib
-Project-URL: changelog, https://github.com/stravalib/stravalib/blob/main/changelog.md
-Keywords: strava,running,cycling,athletes
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pint
-Requires-Dist: pytz
-Requires-Dist: arrow
-Requires-Dist: requests
-Requires-Dist: pydantic==1.10.9
-
 # Welcome to stravalib
 
 [![DOI](https://zenodo.org/badge/8828908.svg)](https://zenodo.org/badge/latestdoi/8828908)
 ![PyPI](https://img.shields.io/pypi/v/stravalib?style=plastic) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stravalib?style=plastic) [![Documentation Status](https://readthedocs.org/projects/stravalib/badge/?version=latest)](https://stravalib.readthedocs.io/en/latest/?badge=latest) ![Package Tests Status](https://github.com/stravalib/stravalib/actions/workflows/build-test.yml/badge.svg) ![PyPI - Downloads](https://img.shields.io/pypi/dm/stravalib?style=plastic) [![codecov](https://codecov.io/gh/stravalib/stravalib/branch/main/graph/badge.svg?token=sHbFJn7epy)](https://codecov.io/gh/stravalib/stravalib)
 
 The **stravalib** Python package provides easy-to-use tools for accessing and
 downloading Strava data from the Strava V3 web service. Stravalib provides a Client class that supports:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stravalib-1.6/changelog.md` & `stravalib-1.7/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 # Change Log
 
 ## Unreleased
 
+## v1.7
+
+### Added
+- Add: Strava API change - Route objects have a new waypoints attribute (@bot, #480)
+
+### Fixed
+- Fix: Docs - add contributing section to top bar for easier discovery and a few small syntax fixes in the docs (@lwasser)
+- Fix: Manifest.in file - remove example dir (@lwasser, #307)
+- Fix: Codecov report wasn't generating correctly (@lwasser, #469)
+- Fix: Add sport type to create_activity and create type validator method. NOTE: this fix contains a breaking change in `Client.create_activity()` activity_type is now an optional keyword argument rather than a required positional argument (@lwasser, #279)
+- Fix: Fixes the Strava API update bot (@jsamoocha, #477)
+- Fix: Cleanup dependencies to only use pyproject toml (@lwasser, #466)
+- Fix: use parse_obj rather than deserialize internally where possible (@lwasser, #358)
+
+## Removed
+- Remove: functional test suite from stravalib (@lwasser, #457)
+- Remove: `client.delete_activity` method is no longer supported by Strava (@lwasser, #238)
+- Remove/Add: Drop Python 3.9, add Python 3.12 (@lwasser, #487)
+
+### Breaking Changes
+If you have been using the `client.delete_activity` method then your code will
+no longer work as this method was removed due to being deprecated by Strava. We also are dropping support for Python 3.9 (end of life / no more security fixes in October 2024 and now only getting security fixes) in this release and adding support for 3.12.
+
+### Contributors to this release
+
+@jsamoocha, @lwasser, stravalib bot :)
+
 ## v1.6
 
 ### Added
 - Add: Support for Strava's new read rate limits (@jsamoocha, #446)
 - Add: Improved handling of unexpected activity types (@jsamoocha, #454)
 
 ### Fixed
```

### Comparing `stravalib-1.6/docs/conf.py` & `stravalib-1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/contributing/build-release-guide.md` & `stravalib-1.7/docs/contributing/build-release-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/contributing/development-guide.md` & `stravalib-1.7/docs/contributing/development-guide.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,24 @@
 ```
 
 Finally install the package dependencies and the `stravalib` package in
 development / editable mode (`-e`). Editable mode allows you to make updates
 to the package and test them in realtime.
 
 ```bash
-# install the package requirements
-$ pip install -r requirements.txt
-# Install stravalib in editable mode
-$ pip install -e .
+# Install the package in editable model and all requirements
+$ pip install -e ".[build, tests, docs]"
+```
+
+```{note}
+If you only want to install dependencies for building and testing the package (and exclude the docs requirements), you can run:
+
+`pip install -e ".[build, tests]"`
+
+Also note that some shells may not need the `".[build, tests]"` but it is needed for zsh shells and will likely work on most if not all shells with the quotes.
 ```
 
 ## Architecture Overview
 
 ![Stravalib Architecture](../images/stravalib_architecture.png)
 
 Stravalib contains the following main components:
@@ -89,14 +95,21 @@
 undocumented Strava features.
 
 The module `protocol.py` manages the sending of HTTP requests
 to Strava and handling the received responses (including rate limiting).
 It is used by methods in `client.py` to de-serialize raw response data into
 the domain entities in `model.py`.
 
+## Python support
+We loosely follow the [Numpy guidelines defined in NEP 29](https://numpy.org/neps/nep-0029-deprecation_policy.html)
+for Python version support. However, in some cases we may decide to
+support older versions of Python given visible community demand for
+such support.
+
+
 ## Code style, linting & typing
 
 We use the following tools to ensure consistent code format that follows
 the Python Enhancement Protocol (PEP) 008 standards. These standards dictate
 best practices for Python code readability and consistency:
 
 - [black](https://black.readthedocs.io/en/stable/) for consistent code format
```

### Comparing `stravalib-1.6/docs/contributing/resources-for-new-contributors.md` & `stravalib-1.7/docs/contributing/resources-for-new-contributors.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/get-started/activities.rst` & `stravalib-1.7/docs/get-started/activities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/get-started/athletes.rst` & `stravalib-1.7/docs/get-started/athletes.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/get-started/authenticate-with-strava.rst` & `stravalib-1.7/docs/get-started/authenticate-with-strava.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/get-started/index.md` & `stravalib-1.7/docs/get-started/index.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,25 +8,14 @@
 Overview <overview>
 Authentication <authenticate-with-strava>
 Activities <activities>
 Athletes <athletes>
 
 ```
 
-```{toctree}
-:hidden:
-:caption: Contributing
-:maxdepth: 2
-
-Contributing Guide <../contributing/how-to-contribute>
-Development Guide <../contributing/development-guide>
-Build & Release Guide <../contributing/build-release-guide>
-New Contributor Resources <../contributing/resources-for-new-contributors>
-Change Log <../contributing/documentation-changelog>
-```
 
 ## Install stravalib
 
 The package is available on PyPI to be installed using `pip`.
 
 ```bash
 $ pip install stravalib
```

### Comparing `stravalib-1.6/docs/get-started/overview.rst` & `stravalib-1.7/docs/get-started/overview.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/images/stravalib_architecture.png` & `stravalib-1.7/docs/images/stravalib_architecture.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/index.md` & `stravalib-1.7/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,7 +102,16 @@
 ```{toctree}
 :hidden:
 :caption: API Documentation
 :maxdepth: 2
 
 Code/API Reference <reference>
 ```
+
+
+:::{toctree}
+:hidden:
+:caption: Contribute
+:maxdepth: 2
+
+Contribute <contributing/intro.md>
+:::
```

### Comparing `stravalib-1.6/docs/reference/client.rst` & `stravalib-1.7/docs/reference/client.rst`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
    Client.delete_activity
    Client.get_activity_zones
    Client.get_activity_comments
    Client.get_activity_kudos
    Client.get_activity_photos
    Client.get_activity_laps
    Client.get_related_activities
+   Client._validate_activity_type
 
 Segment related methods
 -------------------------
 .. autosummary::
    :toctree: api/
 
    Client.get_segment_effort
```

### Comparing `stravalib-1.6/docs/reference/model.rst` & `stravalib-1.7/docs/reference/model.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/reference/utilities.rst` & `stravalib-1.7/docs/reference/utilities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/docs/reference.rst` & `stravalib-1.7/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/noxfile.py` & `stravalib-1.7/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,77 +5,60 @@
 
 import nox
 
 nox.options.reuse_existing_virtualenvs = True
 
 
 # Use this for venv envs nox -s test
-@nox.session(python=["3.9", "3.10", "3.11"])
+@nox.session(python=["3.10", "3.11", "3.12"])
 def tests(session):
     """Install requirements in a venv and run tests."""
-    session.install(".[all]")
-    session.install("-r", "requirements.txt")
+    session.install(".[tests]")
     session.run(
         "pytest",
-        "--cov",
-        "src/stravalib",
-        "src/stravalib/tests/unit/",
-        "src/stravalib/tests/integration/",
-    )
-
-
-# Use this for conda/mamba = nox -s test_mamba
-@nox.session(venv_backend="mamba", python=["3.9", "3.10", "3.11"])
-def test_mamba(session):
-    session.install(".[all]")
-    session.install("-r", "requirements.txt")
-    session.run(
-        "pytest",
-        "--cov",
-        "src/stravalib",
+        "--cov=src/stravalib",
+        "--cov-report=xml:coverage.xml",
+        "--cov-report=term",
         "src/stravalib/tests/unit/",
         "src/stravalib/tests/integration/",
     )
 
 
 # Build docs
 build_command = ["-b", "html", "docs/", "docs/_build/html"]
 
 
 @nox.session
 def docs(session):
-    session.install(".[all]")
-    session.install("-r", "requirements.txt")
+    session.install(".[docs]")
     cmd = ["sphinx-build"]
     cmd.extend(build_command + session.posargs)
     session.run(*cmd)
 
 
 @nox.session(name="docs-live")
 def docs_live(session):
-    session.install("-r", "requirements.txt")
-    session.install(".[all]")
+    session.install(".[docs]")
 
     AUTOBUILD_IGNORE = [
         "_build",
         "build_assets",
         "tmp",
     ]
     cmd = ["sphinx-autobuild"]
     for folder in AUTOBUILD_IGNORE:
         cmd.extend(["--ignore", f"*/{folder}/*"])
     cmd.extend(build_command + session.posargs)
     session.run(*cmd)
 
 
-# Use this for venv envs nox -s test
+# Use this for venv envs nox -s mypy
 @nox.session(python="3.10")
 def mypy(session):
-    session.install(".[all]")
-    session.install("-r", "requirements.txt")
+    session.install(".[lint]")
     session.run(
         "mypy",
     )
 
 
 @nox.session(name="docs-clean")
 def clean_docs(session):
@@ -96,36 +79,31 @@
 
 
 @nox.session()
 def build(session):
     """Build the package's SDist and wheel using PyPA build and
     setuptools / setuptools_scm"""
 
-    session.install("-r", "requirements-build.txt")
+    session.install(".[build]")
     session.run("python", "-m", "build")
 
 
 @nox.session()
 def install_wheel(session):
     """If you have several wheels in your dist/ directory this will
     try to install each one. so be sure to clean things out before
     running."""
 
     wheel_files = glob(os.path.join("dist", "*.whl"))
     print(wheel_files)
-    session.run(
-        "pip",
-        "install",
-        "--no-deps",
-        "dist/stravalib-1.4.post24-py3-none-any.whl",
-    )
+
     if wheel_files:
-        for wheel_path in wheel_files:
-            print("Installing:", wheel_path)
-            session.install(wheel_path)
+        most_recent_wheel = max(wheel_files, key=os.path.getmtime)
+        print("Installing:", most_recent_wheel)
+        session.install(most_recent_wheel)
     else:
         print("No wheel files found matching the pattern: *.whl")
 
 
 @nox.session()
 def clean_build(session):
     """Clean out the dist/ directory and also clean out other remnant
```

### Comparing `stravalib-1.6/pyproject.toml` & `stravalib-1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,39 +28,68 @@
 maintainers = [
   { name = "Leah Wasser" },
   { name = "Hans Lellelid" },
   { name = "Jonatan Samoocha" },
   { name = "Yihong" },
   { name = "Émile Nadeau" },
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
-  # Because license is listed below does it need to be here too?
   "License :: OSI Approved :: Apache Software License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Libraries",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 
-dependencies = ["pint", "pytz", "arrow", "requests", "pydantic==1.10.9"]
+dependencies = ["pint", "pytz", "arrow", "requests", "pydantic<2.0"]
 
 [project.urls]
 documentation = "https://stravalib.readthedocs.io"
 repository = "https://github.com/stravalib/stravalib"
 changelog = "https://github.com/stravalib/stravalib/blob/main/changelog.md"
 
+
+[project.optional-dependencies]
+build = ["build"]
+tests = [
+  "pytest",
+  "pytest-cov",
+  "responses"
+]
+docs = [
+  "sphinx",
+  "pydata-sphinx-theme",
+  "autodoc_pydantic",
+  "sphinx_remove_toctrees",
+  "myst-nb",
+  "sphinx-autobuild",
+  "sphinx-inline-tabs",
+  "sphinx_copybutton",
+  "sphinx_design",
+  "sphinxext-opengraph",
+  # Needed for sphinx open graph
+  "matplotlib"
+]
+lint = [
+  "pre-commit",
+  "mypy",
+  "types-requests",
+  "types-pytz",
+  "types-Flask"
+]
+
 [tool.black]
 line-length = 79
 # When editing the config for black in this file, be sure to make
 # the same edits in the repo stravalib/strava_swagger2pydantic
 
 [tool.isort]
 profile = "black"
@@ -91,13 +120,13 @@
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.codespell]
 skip = './docs/_build, ./build, ./src/stravalib/tests/resources'
 
 [tool.ruff]
-select = [
+lint.select = [
   "F", # pyflakes
   "I", # isort
 ]
-ignore = ["F841"]
+lint.ignore = ["F841"]
 line-length = 79
```

### Comparing `stravalib-1.6/src/stravalib/client.py` & `stravalib-1.7/src/stravalib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         Parameters
         ----------
         athlete_id : int, default=None
             Strava ID value for the athlete.
 
         Returns
         -------
-        py:class:`stravalib.model.AthleteStats`
+        :class:`stravalib.model.AthleteStats`
             A model containing the Stats
 
         """
         if athlete_id is None:
             athlete_id = self.get_athlete().id
 
         raw = self.protocol.get("/athletes/{id}/stats", id=athlete_id)
@@ -454,15 +454,15 @@
         """List the clubs for the currently authenticated athlete.
 
         https://developers.strava.com/docs/reference/#api-Clubs-getLoggedInAthleteClubs
 
 
         Returns
         -------
-        py:class:`list`
+        :class:`list`
             A list of :class:`stravalib.model.Club`
 
         """
 
         # TODO: This should return a BatchedResultsIterator or otherwise at
         # most 30 clubs are returned!
         club_structs = self.protocol.get("/athlete/clubs")
@@ -634,93 +634,167 @@
 
         """
         raise NotImplementedError(
             "The /activities/following endpoint was removed by Strava.  "
             "See https://developers.strava.com/docs/january-2018-update/"
         )
 
+    def _validate_activity_type(
+        self,
+        params: dict[str, Any],
+        activity_type: str | None,
+        sport_type: str | None,
+    ) -> dict[str, Any]:
+        """Validate activity type and sport type values.
+
+        Parameters
+        ----------
+        params : dict
+            A dictionary of activity values used to update or create an
+            activity.
+        activity_type : str, default=None
+            The activity type (case-insensitive).
+            Deprecated. Prefer to use sport_type. In a request where both type
+            and sport_type are present, this field will be ignored.
+            See https://developers.strava.com/docs/reference/#api-models-UpdatableActivity.
+            For possible values see: :class:`stravalib.model.Activity.TYPES`
+        sport_type : str, default=None
+            For possible values (case-sensitive) see:
+            :class:`stravalib.model.Activity.SPORT_TYPES`
+
+        Returns
+        -------
+        dict
+            Dictionary containing overlapping parameter values between the two
+            methods
+        Raises
+        ------
+        ValueError
+            If the activity_type or sport_type is invalid.
+        """
+
+        # Check for sport_type first. If provided, it is favored over
+        # activity_type / type
+        if sport_type is not None:
+            if not sport_type in model.Activity.SPORT_TYPES:
+                raise ValueError(
+                    f"Invalid activity type: {sport_type}. Possible values: {model.Activity.SPORT_TYPES!r}"
+                )
+            params["sport_type"] = sport_type
+            return params
+
+        # Handle activity type throwing warning given sport type is preferred
+        # This also ONLY adds activity type if the user provides it over
+        # sport_type.
+        elif activity_type is not None:
+            if not activity_type.lower() in [
+                t.lower() for t in model.Activity.TYPES
+            ]:
+                raise ValueError(
+                    f"Invalid activity type: {activity_type}. Possible values: {model.Activity.TYPES!r}"
+                )
+            params["type"] = activity_type.lower()
+            warn_param_deprecation(
+                "activity_type",
+                "sport_type",
+                "https://developers.strava.com/docs/reference/#api-models-UpdatableActivity",
+            )
+
+        return params
+
+    # TODO: according to the strava api docs we can add an optional trainer
+    # and commute param here with boolean 0/1 values
     def create_activity(
         self,
         name: str,
-        activity_type: ActivityType,
         start_date_local: datetime | str,
         elapsed_time: int | timedelta,
+        sport_type: SportType | None = None,
+        activity_type: ActivityType | None = None,
         description: str | None = None,
         distance: pint.Quantity | float | None = None,
     ) -> model.Activity:
         """Create a new manual activity.
 
         If you would like to create an activity from an uploaded GPS file, see the
         :meth:`stravalib.client.Client.upload_activity` method instead.
 
         Parameters
         ----------
         name : str
             The name of the activity.
-        activity_type : str
+        activity_type : str, default=None
             The activity type (case-insensitive).
-            Possible values: ride, run, swim, workout, hike, walk, nordicski,
-            alpineski, backcountryski, iceskate, inlineskate, kitesurf,
-            rollerski, windsurf, workout, snowboard, snowshoe
+            Deprecated. Prefer to use sport_type. In a request where both type
+            and sport_type are present, this field will be ignored.
+            See https://developers.strava.com/docs/reference/#api-models-UpdatableActivity.
+            For possible values see: :class:`stravalib.model.Activity.TYPES`
+        sport_type : str, default=None
+            For possible values (case-sensitive) see: For possible values
+            see: :class:`stravalib.model.Activity.SPORT_TYPES`
         start_date_local : class:`datetime.datetime` or string in ISO8601 format
             Local date/time of activity start. (TZ info will be ignored)
         elapsed_time : class:`datetime.timedelta` or int (seconds)
             The time in seconds or a :class:`datetime.timedelta` object.
         description : str, default=None
             The description for the activity.
         distance : class:`pint.Quantity` or float (meters), default=None
             The distance in meters (float) or a :class:`pint.Quantity` instance.
 
         """
+
+        # Strava API requires either sport_type or activity_type to be defined
+        # to create an activity. Check for that here.
+        if sport_type is None and activity_type is None:
+            raise ValueError(
+                "Either 'sport_type' or 'activity_type' must be provided to create an activity."
+            )
+
         if isinstance(elapsed_time, timedelta):
             elapsed_time = elapsed_time.seconds
 
         if is_quantity_type(distance):
             distance = float(unithelper.meters(cast(pint.Quantity, distance)))
 
         if isinstance(start_date_local, datetime):
             start_date_local = start_date_local.strftime("%Y-%m-%dT%H:%M:%SZ")
 
-        if not activity_type.lower() in [
-            t.lower() for t in model.Activity.TYPES
-        ]:
-            raise ValueError(
-                f"Invalid activity type: {activity_type}. Possible values: {model.Activity.TYPES!r}"
-            )
-
         params: dict[str, Any] = dict(
             name=name,
-            type=activity_type.lower(),
             start_date_local=start_date_local,
             elapsed_time=elapsed_time,
         )
 
         if description is not None:
             params["description"] = description
 
         if distance is not None:
             params["distance"] = distance
 
+        params = self._validate_activity_type(
+            params, activity_type, sport_type
+        )
+
         raw_activity = self.protocol.post("/activities", **params)
 
         return model.Activity.parse_obj(
             {**raw_activity, **{"bound_client": self}}
         )
 
     def update_activity(
         self,
         activity_id: int,
         name: str | None = None,
         activity_type: ActivityType | None = None,
         sport_type: SportType | None = None,
+        description: str | None = None,
         private: bool | None = None,
         commute: bool | None = None,
         trainer: bool | None = None,
         gear_id: int | None = None,
-        description: str | None = None,
         device_name: str | None = None,
         hide_from_home: bool | None = None,
     ) -> model.Activity:
         """Updates the properties of a specific activity.
 
         https://developers.strava.com/docs/reference/#api-Activities-updateActivityById
 
@@ -731,28 +805,17 @@
         name : str, default=None
             The name of the activity.
         activity_type : str, default=None
             The activity type (case-insensitive).
             Deprecated. Prefer to use sport_type. In a request where both type
             and sport_type are present, this field will be ignored.
             See https://developers.strava.com/docs/reference/#api-models-UpdatableActivity.
-            Possible values: ride, run, swim, workout, hike, walk, nordicski,
-            alpineski, backcountryski, iceskate, inlineskate, kitesurf,
-            rollerski, windsurf, workout, snowboard, snowshoe
+            For possible values see: :class:`stravalib.model.Activity.TYPES`
         sport_type : str, default=None
-            Possible values (case-sensitive): AlpineSki, BackcountrySki,
-            Badminton, Canoeing, Crossfit, EBikeRide, Elliptical,
-            EMountainBikeRide, Golf, GravelRide, Handcycle,
-            HighIntensityIntervalTraining, Hike, IceSkate, InlineSkate,
-            Kayaking, Kitesurf, MountainBikeRide, NordicSki, Pickleball,
-            Pilates, Racquetball, Ride, RockClimbing, RollerSki, Rowing, Run,
-            Sail, Skateboard, Snowboard, Snowshoe, Soccer, Squash,
-            StairStepper, StandUpPaddling, Surfing, Swim, TableTennis, Tennis,
-            TrailRun, Velomobile, VirtualRide, VirtualRow, VirtualRun, Walk,
-            WeightTraining, Wheelchair, Windsurf, Workout, Yoga
+            For possible values see: :class:`stravalib.model.Activity.SPORT_TYPES`
         private : bool, default=None
             Whether the activity is private.
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
         commute : bool, default=None
             Whether the activity is a commute.
@@ -769,48 +832,22 @@
             removed in the future.
         hide_from_home : bool, default=None
             Whether the activity is muted (hidden from Home and Club feeds).
 
         Returns
         -------
             Updates the activity in the selected Strava account
-
-
         """
 
         # Convert the kwargs into a params dict
         params: dict[str, Any] = {}
 
         if name is not None:
             params["name"] = name
 
-        if activity_type is not None:
-            if not activity_type.lower() in [
-                t.lower() for t in model.Activity.TYPES
-            ]:
-                raise ValueError(
-                    f"Invalid activity type: {activity_type}. Possible values: {model.Activity.TYPES!r}"
-                )
-            params["type"] = activity_type.lower()
-            warn_param_deprecation(
-                "activity_type",
-                "sport_type",
-                "https://developers.strava.com/docs/reference/#api-models-UpdatableActivity",
-            )
-
-        if sport_type is not None:
-            if not sport_type in model.Activity.SPORT_TYPES:
-                raise ValueError(
-                    f"Invalid activity type: {sport_type}. Possible values: {model.Activity.SPORT_TYPES!r}"
-                )
-            params["sport_type"] = sport_type
-            params.pop(
-                "type", None
-            )  # Just to be sure we don't confuse the Strava API
-
         if private is not None:
             warn_param_unsupported("private")
             params["private"] = int(private)
 
         if commute is not None:
             params["commute"] = int(commute)
 
@@ -826,14 +863,19 @@
         if device_name is not None:
             warn_param_unsupported("device_name")
             params["device_name"] = device_name
 
         if hide_from_home is not None:
             params["hide_from_home"] = int(hide_from_home)
 
+        # Validate sport and activity types
+        params = self._validate_activity_type(
+            params, activity_type, sport_type
+        )
+
         raw_activity = self.protocol.put(
             "/activities/{activity_id}", activity_id=activity_id, **params
         )
 
         return model.Activity.parse_obj(
             {**raw_activity, **{"bound_client": self}}
         )
@@ -864,15 +906,15 @@
             gpx, gpx.gz
         name : str, optional, default=None
             If not provided, will be populated using start date and location,
             if available
         description : str, optional, default=None
             The description for the activity
         activity_type : str, optional
-            case-insensitive type of activity.
+            Case-insensitive type of activity.
             possible values: ride, run, swim, workout, hike, walk,
             nordicski, alpineski, backcountryski, iceskate, inlineskate,
             kitesurf, rollerski, windsurf, workout, snowboard, snowshoe
             Type detected from file overrides, uses athlete's default type if
             not specified
             WARNING - This param is supported (as of 2022-11-15), but not
             documented and may be removed in the future.
@@ -887,15 +929,14 @@
             An arbitrary unique identifier may be specified which
             will be included in status responses.
         trainer : bool, optional, default=None
             Whether the resulting activity should be marked as having
             been performed on a trainer.
         commute : bool, optional, default=None
             Whether the resulting activity should be tagged as a commute.
-
         """
         if not hasattr(activity_file, "read"):
             if isinstance(activity_file, str):
                 activity_file = BytesIO(activity_file.encode("utf-8"))
             elif isinstance(activity_file, bytes):
                 activity_file = BytesIO(activity_file)
             else:
@@ -940,27 +981,14 @@
             files={"file": activity_file},
             check_for_errors=False,
             **params,
         )
 
         return ActivityUploader(self, response=initial_response)
 
-    def delete_activity(self, activity_id: int) -> None:
-        """Deletes the specified activity.
-
-        https://developers.strava.com/docs/reference/#api-Activities
-
-        Parameters
-        ----------
-        activity_id : int
-            The activity to delete.
-
-        """
-        self.protocol.delete("/activities/{id}", id=activity_id)
-
     def get_activity_zones(
         self, activity_id: int
     ) -> list[model.BaseActivityZone]:
         """Gets zones for activity.
 
         Requires premium account.
 
@@ -969,15 +997,15 @@
         Parameters
         ----------
         activity_id : int
             The activity for which to get zones.
 
         Returns
         -------
-        py:class:`list`
+        :class:`list`
             A list of :class:`stravalib.model.BaseActivityZone` objects.
 
         """
         zones = self.protocol.get("/activities/{id}/zones", id=activity_id)
         return [
             model.BaseActivityZone.parse_obj({**z, **{"bound_client": self}})
             for z in zones
@@ -1367,16 +1395,18 @@
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def explore_segments(
         self,
-        bounds: tuple[float, float, float, float]
-        | tuple[tuple[float, float], tuple[float, float]],
+        bounds: (
+            tuple[float, float, float, float]
+            | tuple[tuple[float, float], tuple[float, float]]
+        ),
         activity_type: ActivityType | None = None,
         min_cat: int | None = None,
         max_cat: int | None = None,
     ) -> list[model.SegmentExplorerResult]:
         """Returns an array of up to 10 segments.
 
         https://developers.strava.com/docs/reference/#api-Segments-exploreSegments
@@ -1391,15 +1421,15 @@
         min_cat : int, optional, default=None
             Minimum climb category filter
         max_cat : int, optional, default=None
             Maximum climb category filter
 
         Returns
         -------
-        py:class:`list`
+        :class:`list`
             An list of :class:`stravalib.model.Segment`.
 
         """
         if len(bounds) == 2:
             bounds = (
                 bounds[0][0],
                 bounds[0][1],
@@ -1540,26 +1570,28 @@
             The ID of activity.
         types : list[str], optional, default=None
             A list of the types of streams to fetch.
         resolution : str, optional
             Indicates desired number of data points. 'low' (100), 'medium'
             (1000) or 'high' (10000).
             .. deprecated::
+
                 This param is not officially supported by the Strava API and
                 may be removed in the future.
         series_type : str, optional
             Relevant only if using resolution either 'time' or 'distance'.
             Used to index the streams if the stream is being reduced.
             .. deprecated::
+
                 This param is not officially supported by the Strava API and may be
                 removed in the future.
 
         Returns
         -------
-        py:class:`dict`
+        :class:`dict`
             A dictionary of :class:`stravalib.model.Stream` from the activity
         """
         return self._get_streams(
             f"/activities/{activity_id}/streams",
             types=types,
             resolution=resolution,
             series_type=series_type,
@@ -1607,15 +1639,15 @@
             .. deprecated::
 
                 This param is not officially supported by the Strava API and
                 may be removed in the future.
 
         Returns
         -------
-        py:class:`dict`
+        :class:`dict`
             An dictionary of :class:`stravalib.model.Stream` from the effort.
 
         """
         return self._get_streams(
             f"/segment_efforts/{effort_id}/streams",
             types=types,
             resolution=resolution,
@@ -1625,15 +1657,15 @@
     def get_segment_streams(
         self,
         segment_id: int,
         types: list[StreamType] | None = None,
         resolution: Literal["low", "medium", "high"] | None = None,
         series_type: Literal["time", "distance"] | None = None,
     ) -> dict[StreamType, model.Stream]:
-        """Returns an streams for a segment.
+        """Returns streams for a segment.
 
         https://developers.strava.com/docs/reference/#api-Streams-getSegmentStreams
 
         Streams represent the raw data of the uploaded file. External
         applications may only access this information for activities owned
         by the authenticated athlete.
 
@@ -1650,26 +1682,28 @@
             The ID of segment.
         types : list, optional, default=None
             A list of the the types of streams to fetch.
         resolution : str, optional
             Indicates desired number of data points. 'low' (100), 'medium'
             (1000) or 'high' (10000).
             .. deprecated::
+
                 This param is not officially supported by the Strava API and may be
                 removed in the future.
         series_type : str, optional
             Relevant only if using resolution either 'time' or 'distance'.
             Used to index the streams if the stream is being reduced.
             .. deprecated::
+
                 This param is not officially supported by the Strava API and may be
                 removed in the future.
 
         Returns
         -------
-        py:class:`dict`
+        :class:`dict`
             An dictionary of :class:`stravalib.model.Stream` from the effort.
 
         """
         return self._get_streams(
             f"/segments/{segment_id}/streams",
             types=types,
             resolution=resolution,
@@ -1747,15 +1781,15 @@
         Parameters
         ----------
         route_id : int
             The ID of activity.
 
         Returns
         -------
-        py:class:`dict`
+        :class:`dict`
             A dictionary of :class:`stravalib.model.Stream` from the route.
 
         """
 
         result_fetcher = functools.partial(
             self.protocol.get, f"/routes/{route_id}/streams/"
         )
@@ -1833,15 +1867,15 @@
 
         Returns
         -------
         dict[str, str]
             The JSON response expected by Strava to the challenge request.
 
         """
-        callback = model.SubscriptionCallback.deserialize(raw)
+        callback = model.SubscriptionCallback.parse_obj(raw)
         callback.validate_token(verify_token)
 
         assert callback.hub_challenge is not None
         response_raw = {"hub.challenge": callback.hub_challenge}
         return response_raw
 
     def handle_subscription_update(
@@ -1924,16 +1958,15 @@
         # Expects a 204 response if all goes well.
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class ResultFetcher(Protocol):
-    def __call__(self, *, page: int, per_page: int) -> Iterable[Any]:
-        ...
+    def __call__(self, *, page: int, per_page: int) -> Iterable[Any]: ...
 
 
 class BatchedResultsIterator(Generic[T]):
     """An iterator that enables iterating over requests that return
     paged results."""
 
     # Number of results returned in a batch. We maximize this to minimize
@@ -1998,24 +2031,17 @@
             self._eof()
         raw_results = self.result_fetcher(
             page=self._page, per_page=self.per_page
         )
 
         entities = []
         for raw in raw_results:
-            try:
-                new_entity = self.entity.parse_obj(
-                    {**raw, **{"bound_client": self.bind_client}}
-                )
-            except AttributeError:
-                # Entity doesn't have a parse_obj() method, so must be of a
-                # legacy type
-                new_entity = self.entity.deserialize(  # type: ignore[attr-defined]
-                    raw, bind_client=self.bind_client
-                )
+            new_entity = self.entity.parse_obj(
+                {**raw, **{"bound_client": self.bind_client}}
+            )
             entities.append(new_entity)
 
         self._buffer = collections.deque(entities)
 
         self.log.debug(
             "Requested page {} (got: {} items)".format(
                 self._page, len(self._buffer)
@@ -2114,15 +2140,15 @@
     def update_from_response(
         self, response: dict[str, Any], raise_exc: bool = True
     ) -> None:
         """Updates internal state of object.
 
         Parameters
         ----------
-        response : py:class:`dict`
+        response : :class:`dict`
             The response object (dict).
         raise_exc : bool
 
         Raises
         ------
         stravalib.exc.ActivityUploadFailed
             If the response indicates an
```

### Comparing `stravalib-1.6/src/stravalib/exc.py` & `stravalib-1.7/src/stravalib/exc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Exceptions & Error Handling
 ============================
 Exceptions and error handling for stravalib.
 These are classes designed to capture and handle various errors encountered when interacting with the Strava API.
 """
+
 from __future__ import annotations
 
 import logging
 import warnings
 
 import requests.exceptions
```

### Comparing `stravalib-1.6/src/stravalib/field_conversions.py` & `stravalib-1.7/src/stravalib/field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/model.py` & `stravalib-1.7/src/stravalib/model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/protocol.py` & `stravalib-1.7/src/stravalib/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Protocol
 ==============
 Low-level classes for interacting directly with the Strava API webservers.
 """
+
 from __future__ import annotations
 
 import abc
 import functools
 import logging
 from typing import TYPE_CHECKING, Any, Callable, Literal, TypedDict
 from urllib.parse import urlencode, urljoin, urlunsplit
@@ -55,16 +56,17 @@
     server = "www.strava.com"
     api_base = "/api/v3"
 
     def __init__(
         self,
         access_token: str | None = None,
         requests_session: requests.Session | None = None,
-        rate_limiter: Callable[[dict[str, str], RequestMethod], None]
-        | None = None,
+        rate_limiter: (
+            Callable[[dict[str, str], RequestMethod], None] | None
+        ) = None,
     ):
         """Initialize this protocol client, optionally providing a (shared)
         :class:`requests.Session` object.
 
         Parameters
         ----------
         access_token : str
```

### Comparing `stravalib-1.6/src/stravalib/strava_model.py` & `stravalib-1.7/src/stravalib/strava_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,15 +704,15 @@
     """
     pr_date: Optional[datetime] = None
     """
     The time at which the PR effort was started.
     """
     pr_elapsed_time: Optional[int] = None
     """
-    The elapsed time of the PR effort.
+    The elapsed time ot the PR effort.
     """
 
 
 class SummarySegmentEffort(BaseModel):
     activity_id: Optional[int] = None
     """
     The unique identifier of the activity related to this effort
@@ -812,14 +812,41 @@
     """
     status: Optional[str] = None
     """
     The status of this upload
     """
 
 
+class Waypoint(BaseModel):
+    categories: Optional[list[str]] = Field(None, min_items=0)
+    """
+    Categories that the waypoint belongs to
+    """
+    description: Optional[str] = None
+    """
+    A description of the waypoint (optional)
+    """
+    distance_into_route: Optional[int] = None
+    """
+    The number meters along the route that the waypoint is located
+    """
+    latlng: Optional[LatLng] = None
+    """
+    The location along the route that the waypoint is closest to
+    """
+    target_latlng: Optional[LatLng] = None
+    """
+    A location off of the route that the waypoint is (optional)
+    """
+    title: Optional[str] = None
+    """
+    A title for the waypoint
+    """
+
+
 class ZoneRange(BaseModel):
     max: Optional[int] = None
     """
     The maximum value in the range.
     """
     min: Optional[int] = None
     """
@@ -1040,17 +1067,17 @@
     """
     The segment's average grade, in percents
     """
     climb_category: Optional[int] = Field(None, ge=0, le=5)
     """
     The category of the climb [0, 5]. Higher is harder ie. 5 is Hors catégorie, 0 is uncategorized in climb_category. If climb_category = 5, climb_category_desc = HC. If climb_category = 2, climb_category_desc = 3.
     """
-    climb_category_desc: Optional[
-        Literal["NC", "4", "3", "2", "1", "HC"]
-    ] = None
+    climb_category_desc: Optional[Literal["NC", "4", "3", "2", "1", "HC"]] = (
+        None
+    )
     """
     The description for the category of the climb
     """
     distance: Optional[float] = None
     """
     The segment's distance, in meters
     """
@@ -1390,14 +1417,18 @@
     """
     This route's type (1 for ride, 2 for runs)
     """
     updated_at: Optional[datetime] = None
     """
     The time at which the route was last updated
     """
+    waypoints: Optional[list[Waypoint]] = Field(None, min_items=0)
+    """
+    The custom waypoints along this route
+    """
 
 
 class TimedZoneDistribution(BaseModel):
     """
     Stores the exclusive ranges representing zones and the time spent in each.
     """
```

### Comparing `stravalib-1.6/src/stravalib/tests/auth_responder.py` & `stravalib-1.7/src/stravalib/tests/auth_responder.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/integration/strava_api_stub.py` & `stravalib-1.7/src/stravalib/tests/integration/strava_api_stub.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/integration/test_client.py` & `stravalib-1.7/src/stravalib/tests/integration/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,40 @@
 from stravalib.client import ActivityUploader
 from stravalib.exc import AccessUnauthorized, ActivityPhotoUploadFailed
 from stravalib.model import Athlete
 from stravalib.tests import RESOURCES_DIR
 from stravalib.unithelper import UnitConverter, meters, miles
 
 
+@pytest.fixture
+def default_call_kwargs():
+    """A fixture containing default input / call parameters for a create
+    activity call to the strava API"""
+
+    default_call_kwargs = {
+        "name": "test",
+        "start_date_local": "2022-01-01T09:00:00",
+        "elapsed_time": 3600,
+    }
+    return default_call_kwargs
+
+
+@pytest.fixture
+def default_request_params():
+    """A fixture containing default request parameters for a create activity
+    request to the strava API"""
+
+    default_request_params = {
+        "name": "test",
+        "start_date_local": "2022-01-01T09:00:00",
+        "elapsed_time": "3600",
+    }
+    return default_request_params
+
+
 def test_get_athlete(mock_strava_api, client):
     mock_strava_api.get("/athlete", response_update={"id": 42})
     athlete = client.get_athlete()
     assert athlete.id == 42
     assert athlete.measurement_preference == "feet"
 
 
@@ -266,39 +292,40 @@
         )
 
 
 @pytest.mark.parametrize(
     "update_kwargs,expected_params,expected_warning,expected_exception",
     (
         ({}, {}, None, None),
-        ({"name": "foo"}, {"name": "foo"}, None, None),
-        ({"activity_type": "foo"}, {}, None, ValueError),
         ({"activity_type": "Run"}, {"type": "run"}, DeprecationWarning, None),
-        ({"activity_type": "run"}, {"type": "run"}, DeprecationWarning, None),
-        ({"activity_type": "RUN"}, {"type": "run"}, DeprecationWarning, None),
-        ({"sport_type": "foo"}, {}, None, ValueError),
         ({"sport_type": "TrailRun"}, {"sport_type": "TrailRun"}, None, None),
         (
             {"activity_type": "Run", "sport_type": "TrailRun"},
             {"sport_type": "TrailRun"},
-            DeprecationWarning,
+            None,
             None,
         ),
         ({"private": True}, {"private": "1"}, DeprecationWarning, None),
         ({"commute": True}, {"commute": "1"}, None, None),
         ({"trainer": True}, {"trainer": "1"}, None, None),
         ({"gear_id": "fb42"}, {"gear_id": "fb42"}, None, None),
         ({"description": "foo"}, {"description": "foo"}, None, None),
         (
             {"device_name": "foo"},
             {"device_name": "foo"},
             DeprecationWarning,
             None,
         ),
         ({"hide_from_home": False}, {"hide_from_home": "0"}, None, None),
+        (
+            {"name": "My awesome activity"},
+            {"name": "My awesome activity"},
+            None,
+            None,
+        ),
     ),
 )
 def test_update_activity(
     mock_strava_api,
     client,
     update_kwargs,
     expected_params,
@@ -482,54 +509,70 @@
         else:
             _call_and_assert()
 
 
 @pytest.mark.parametrize(
     "extra_create_kwargs,extra_expected_params,expected_exception",
     (
-        ({}, {}, None),
-        ({"activity_type": "run"}, {"type": "run"}, None),
-        ({"activity_type": "Run"}, {"type": "run"}, None),
-        ({"activity_type": "sleep"}, {}, ValueError),
         (
-            {"start_date_local": datetime.datetime(2022, 1, 1, 10, 0, 0)},
-            {"start_date_local": "2022-01-01T10:00:00Z"},
+            {
+                "sport_type": "TrailRun",
+                "start_date_local": datetime.datetime(2022, 1, 1, 10, 0, 0),
+            },
+            {
+                "sport_type": "TrailRun",
+                "start_date_local": "2022-01-01T10:00:00Z",
+            },
             None,
         ),
         (
-            {"elapsed_time": datetime.timedelta(minutes=1)},
-            {"elapsed_time": "60"},
+            {
+                "sport_type": "TrailRun",
+                "elapsed_time": datetime.timedelta(minutes=1),
+            },
+            {"sport_type": "TrailRun", "elapsed_time": "60"},
             None,
         ),
-        ({"distance": 1000}, {"distance": "1000"}, None),
-        ({"distance": miles(1)}, {"distance": "1609.344"}, None),
-        ({"description": "foo"}, {"description": "foo"}, None),
+        (
+            {"sport_type": "TrailRun", "distance": 1000},
+            {"sport_type": "TrailRun", "distance": "1000"},
+            None,
+        ),
+        (
+            {"sport_type": "TrailRun", "distance": miles(1)},
+            {"sport_type": "TrailRun", "distance": "1609.344"},
+            None,
+        ),
+        (
+            {"sport_type": "TrailRun", "description": "foo"},
+            {"sport_type": "TrailRun", "description": "foo"},
+            None,
+        ),
+        (
+            {"description": "foo"},
+            {"description": "foo"},
+            ValueError,
+        ),
     ),
 )
 def test_create_activity(
+    default_call_kwargs,
+    default_request_params,
     mock_strava_api,
     client,
     extra_create_kwargs,
     extra_expected_params,
     expected_exception,
 ):
-    default_call_kwargs = {
-        "name": "test",
-        "activity_type": "Run",
-        "start_date_local": "2022-01-01T09:00:00",
-        "elapsed_time": 3600,
-    }
-    default_request_params = {
-        "name": "test",
-        "type": "run",
-        "start_date_local": "2022-01-01T09:00:00",
-        "elapsed_time": "3600",
-    }
-    call_kwargs = {**default_call_kwargs, **extra_create_kwargs}
-    expected_params = {**default_request_params, **extra_expected_params}
+    """Test what happens when create activity receives valid and invalid
+    sport type values and also what happens when a required API item
+    is missing."""
+
+    call_kwargs = default_call_kwargs | extra_create_kwargs
+    expected_params = default_request_params | extra_expected_params
 
     def _call_and_assert():
         _ = client.create_activity(**call_kwargs)
         assert mock_strava_api.calls[-1].request.params == expected_params
 
     if expected_exception:
         with pytest.raises(expected_exception):
```

### Comparing `stravalib-1.6/src/stravalib/tests/resources/activity-manual.3.json` & `stravalib-1.7/src/stravalib/tests/resources/activity-manual.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/activity.3.json` & `stravalib-1.7/src/stravalib/tests/resources/activity.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/athlete.2.json` & `stravalib-1.7/src/stravalib/tests/resources/athlete.2.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/athlete.3.json` & `stravalib-1.7/src/stravalib/tests/resources/athlete.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/example_route_response.json` & `stravalib-1.7/src/stravalib/tests/resources/example_route_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/example_zone_response.json` & `stravalib-1.7/src/stravalib/tests/resources/example_zone_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/sample.tcx` & `stravalib-1.7/src/stravalib/tests/resources/sample.tcx`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/resources/strava_swagger.json` & `stravalib-1.7/src/stravalib/tests/resources/strava_swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999674479166666%*

 * *Differences: {"'paths'": "{'/athletes/{id}/stats': {'get': {'description': 'Returns the activity stats of an "*

 * *            "athlete. Only includes data from activities set to Everyone visibilty.'}}}"}*

```diff
@@ -1475,15 +1475,15 @@
                 "tags": [
                     "Routes"
                 ]
             }
         },
         "/athletes/{id}/stats": {
             "get": {
-                "description": "Returns the activity stats of an athlete. Only includes data from activities set to Everyone visibility.",
+                "description": "Returns the activity stats of an athlete. Only includes data from activities set to Everyone visibilty.",
                 "operationId": "getStats",
                 "parameters": [
                     {
                         "description": "The identifier of the athlete. Must match the authenticated athlete.",
                         "format": "int64",
                         "in": "path",
                         "name": "id",
```

### Comparing `stravalib-1.6/src/stravalib/tests/unit/test_client_utils.py` & `stravalib-1.7/src/stravalib/tests/unit/test_client_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,17 +97,18 @@
 
     def test_upload_activity_file_with_different_types(self):
         """
         Test uploading an activity with different activity_file object types.
 
         """
 
-        with mock.patch(
-            "stravalib.protocol.ApiV3.post", return_value={}
-        ), open(os.path.join(RESOURCES_DIR, "sample.tcx")) as fp:
+        with (
+            mock.patch("stravalib.protocol.ApiV3.post", return_value={}),
+            open(os.path.join(RESOURCES_DIR, "sample.tcx")) as fp,
+        ):
             # test activity_file with type TextIOWrapper
             uploader = self.client.upload_activity(fp, data_type="tcx")
             self.assertTrue(uploader.is_processing)
 
             # test activity_file with type str
             uploader = self.client.upload_activity(
                 fp.read(), data_type="tcx", activity_type="ride"
```

### Comparing `stravalib-1.6/src/stravalib/tests/unit/test_field_conversions.py` & `stravalib-1.7/src/stravalib/tests/unit/test_field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/unit/test_limiter.py` & `stravalib-1.7/src/stravalib/tests/unit/test_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/tests/unit/test_model.py` & `stravalib-1.7/src/stravalib/tests/unit/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from stravalib.strava_model import LatLng
 from stravalib.tests import TestBase
 from stravalib.unithelper import Quantity, UnitConverter
 
 
 @pytest.mark.parametrize("model_class,attr,value", ((Club, "name", "foo"),))
 class TestLegacyModelSerialization:
+
     def test_legacy_deserialize(self, model_class, attr, value):
         with pytest.warns(DeprecationWarning):
             model_obj = model_class.deserialize({attr: value})
             assert getattr(model_obj, attr) == value
 
     def test_legacy_from_dict(self, model_class, attr, value):
         with pytest.warns(DeprecationWarning):
```

### Comparing `stravalib-1.6/src/stravalib/tests/unit/test_unithelper.py` & `stravalib-1.7/src/stravalib/tests/unit/test_unithelper.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.6/src/stravalib/unithelper.py` & `stravalib-1.7/src/stravalib/unithelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Unit Helper
 ==============
 Helpers for converting Strava's units to something more practical.
 """
+
 from numbers import Number
 from typing import Any, Protocol, Union, cast, runtime_checkable
 
 import pint
 
 from stravalib.exc import warn_units_deprecated
 from stravalib.unit_registry import Q_
```

### Comparing `stravalib-1.6/src/stravalib/util/limiter.py` & `stravalib-1.7/src/stravalib/util/limiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   Strava API usage is limited on a per-application basis using a short term,
   15 minute, limit and a long term, daily, limit. The default rate limit allows
   600 requests every 15 minutes, with up to 30,000 requests per day.
 
   This limit allows applications to make 40 requests per minute for about
   half the day.
 """
+
 from __future__ import annotations
 
 import logging
 import time
 from logging import Logger
 from typing import Callable, Literal, NamedTuple
```

### Comparing `stravalib-1.6/src/stravalib.egg-info/SOURCES.txt` & `stravalib-1.7/src/stravalib.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 changelog.md
 environment.yml
 noxfile.py
 pyproject.toml
-requirements-build.txt
-requirements.txt
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug-report.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/documentation-issue.yml
 .github/ISSUE_TEMPLATE/feature-request.yml
 .github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
 .github/workflows/build-docs.yml
@@ -30,14 +28,15 @@
 docs/reference.rst
 docs/_static/keepme
 docs/_static/stravalib.css
 docs/contributing/build-release-guide.md
 docs/contributing/development-guide.md
 docs/contributing/documentation-changelog.md
 docs/contributing/how-to-contribute.md
+docs/contributing/intro.md
 docs/contributing/resources-for-new-contributors.md
 docs/get-started/activities.rst
 docs/get-started/athletes.rst
 docs/get-started/authenticate-with-strava.rst
 docs/get-started/index.md
 docs/get-started/overview.rst
 docs/images/stravalib_architecture.png
@@ -45,21 +44,14 @@
 docs/reference/exceptions.rst
 docs/reference/field-conversions.rst
 docs/reference/model.rst
 docs/reference/protocol.rst
 docs/reference/strava_model.rst
 docs/reference/unithelper.rst
 docs/reference/utilities.rst
-examples/strava-oauth/README.md
-examples/strava-oauth/requirements.txt
-examples/strava-oauth/server.py
-examples/strava-oauth/static/ConnectWithStrava.png
-examples/strava-oauth/templates/login.html
-examples/strava-oauth/templates/login_error.html
-examples/strava-oauth/templates/login_results.html
 src/stravalib/__init__.py
 src/stravalib/_version_generated.py
 src/stravalib/client.py
 src/stravalib/exc.py
 src/stravalib/field_conversions.py
 src/stravalib/model.py
 src/stravalib/protocol.py
@@ -70,22 +62,17 @@
 src/stravalib.egg-info/PKG-INFO
 src/stravalib.egg-info/SOURCES.txt
 src/stravalib.egg-info/dependency_links.txt
 src/stravalib.egg-info/requires.txt
 src/stravalib.egg-info/top_level.txt
 src/stravalib/tests/__init__.py
 src/stravalib/tests/auth_responder.py
+src/stravalib/tests/conftest.py
 src/stravalib/tests/test.ini-example
-src/stravalib/tests/functional/__init__.py
-src/stravalib/tests/functional/test_client.py
-src/stravalib/tests/functional/test_client_rate_limiter.py
-src/stravalib/tests/functional/test_client_write.py
-src/stravalib/tests/functional/test_result_iterator.py
 src/stravalib/tests/integration/__init__.py
-src/stravalib/tests/integration/conftest.py
 src/stravalib/tests/integration/strava_api_stub.py
 src/stravalib/tests/integration/test_client.py
 src/stravalib/tests/resources/activity-manual.3.json
 src/stravalib/tests/resources/activity.3.json
 src/stravalib/tests/resources/athlete.2.json
 src/stravalib/tests/resources/athlete.3.json
 src/stravalib/tests/resources/example_route_response.json
@@ -94,9 +81,10 @@
 src/stravalib/tests/resources/strava_swagger.json
 src/stravalib/tests/unit/__init__.py
 src/stravalib/tests/unit/test_client_utils.py
 src/stravalib/tests/unit/test_field_conversions.py
 src/stravalib/tests/unit/test_limiter.py
 src/stravalib/tests/unit/test_model.py
 src/stravalib/tests/unit/test_unithelper.py
+src/stravalib/tests/unit/test_validate_activity_type.py
 src/stravalib/util/__init__.py
 src/stravalib/util/limiter.py
```

