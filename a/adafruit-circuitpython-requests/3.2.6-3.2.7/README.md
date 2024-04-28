# Comparing `tmp/adafruit_circuitpython_requests-3.2.6.tar.gz` & `tmp/adafruit_circuitpython_requests-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_requests-3.2.6.tar", last modified: Sat Apr 27 14:14:12 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_requests-3.2.7.tar", last modified: Sun Apr 28 21:25:27 2024, max compression
```

## Comparing `adafruit_circuitpython_requests-3.2.6.tar` & `adafruit_circuitpython_requests-3.2.7.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.098722 adafruit_circuitpython_requests-3.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.082722 adafruit_circuitpython_requests-3.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.086722 adafruit_circuitpython_requests-3.2.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.090722 adafruit_circuitpython_requests-3.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.090722 adafruit_circuitpython_requests-3.2.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-27 14:14:12.098722 adafruit_circuitpython_requests-3.2.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.098722 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-27 14:14:12.000000 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-27 14:14:12.000000 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:14:12.000000 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 14:14:12.000000 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 14:14:12.000000 adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.090722 adafruit_circuitpython_requests-3.2.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.090722 adafruit_circuitpython_requests-3.2.6/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.086722 adafruit_circuitpython_requests-3.2.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.094722 adafruit_circuitpython_requests-3.2.6/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:14:12.098722 adafruit_circuitpython_requests-3.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:14:12.098722 adafruit_circuitpython_requests-3.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-27 14:14:09.000000 adafruit_circuitpython_requests-3.2.6/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 14:14:02.000000 adafruit_circuitpython_requests-3.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.651668 adafruit_circuitpython_requests-3.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.639669 adafruit_circuitpython_requests-3.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-28 21:25:27.651668 adafruit_circuitpython_requests-3.2.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.651668 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-28 21:25:27.000000 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-28 21:25:27.000000 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:25:27.000000 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 21:25:27.000000 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 21:25:27.000000 adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.639669 adafruit_circuitpython_requests-3.2.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.643669 adafruit_circuitpython_requests-3.2.7/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.647668 adafruit_circuitpython_requests-3.2.7/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.647668 adafruit_circuitpython_requests-3.2.7/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.647668 adafruit_circuitpython_requests-3.2.7/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.647668 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.647668 adafruit_circuitpython_requests-3.2.7/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:25:27.651668 adafruit_circuitpython_requests-3.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:25:27.651668 adafruit_circuitpython_requests-3.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-28 21:25:25.000000 adafruit_circuitpython_requests-3.2.7/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 21:25:19.000000 adafruit_circuitpython_requests-3.2.7/tox.ini
```

### Comparing `adafruit_circuitpython_requests-3.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_requests-3.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/.gitignore` & `adafruit_circuitpython_requests-3.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/.pre-commit-config.yaml` & `adafruit_circuitpython_requests-3.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/.pylintrc` & `adafruit_circuitpython_requests-3.2.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_requests-3.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/LICENSE` & `adafruit_circuitpython_requests-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_requests-3.2.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/LICENSES/MIT.txt` & `adafruit_circuitpython_requests-3.2.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/LICENSES/Unlicense.txt` & `adafruit_circuitpython_requests-3.2.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/PKG-INFO` & `adafruit_circuitpython_requests-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.6
+Version: 3.2.7
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_requests-3.2.6/README.rst` & `adafruit_circuitpython_requests-3.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.6
+Version: 3.2.7
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_requests-3.2.6/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit_circuitpython_requests-3.2.7/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
 examples/wifi/expanded/requests_wifi_api_premiereleague.py
 examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
 examples/wifi/expanded/requests_wifi_api_steam.py
 examples/wifi/expanded/requests_wifi_api_twitch.py
 examples/wifi/expanded/requests_wifi_api_youtube.py
 examples/wifi/expanded/requests_wifi_multiple_cookies.py
+examples/wifi/expanded/requests_wifi_status_codes.py
 examples/wiznet5k/requests_wiznet5k_advanced.py
 examples/wiznet5k/requests_wiznet5k_simpletest.py
 tests/chunk_test.py
 tests/chunked_redirect_test.py
 tests/concurrent_test.py
 tests/conftest.py
 tests/header_test.py
```

### Comparing `adafruit_circuitpython_requests-3.2.6/adafruit_requests.py` & `adafruit_circuitpython_requests-3.2.7/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.6"
+__version__ = "3.2.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
 import sys
 
 from adafruit_connection_manager import get_connection_manager
```

### Comparing `adafruit_circuitpython_requests-3.2.6/docs/_static/favicon.ico` & `adafruit_circuitpython_requests-3.2.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/docs/conf.py` & `adafruit_circuitpython_requests-3.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/docs/examples.rst` & `adafruit_circuitpython_requests-3.2.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/docs/index.rst` & `adafruit_circuitpython_requests-3.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/cpython/requests_cpython_advanced.py` & `adafruit_circuitpython_requests-3.2.7/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/cpython/requests_cpython_simpletest.py` & `adafruit_circuitpython_requests-3.2.7/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit_circuitpython_requests-3.2.7/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit_circuitpython_requests-3.2.7/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/fona/requests_fona_advanced.py` & `adafruit_circuitpython_requests-3.2.7/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/fona/requests_fona_simpletest.py` & `adafruit_circuitpython_requests-3.2.7/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_api_youtube.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/requests_wifi_advanced.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/requests_wifi_advanced.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
+# Updated for Circuit Python 9.0
+
+""" WiFi Advanced Example """
 
 import os
-import ssl
 
-import socketpool
+import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
 # Get WiFi details, ensure these are setup in settings.toml
 ssid = os.getenv("CIRCUITPY_WIFI_SSID")
 password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
 
-# Initialize WiFi Pool (There can be only 1 pool & top of script)
-radio = wifi.radio
-pool = socketpool.SocketPool(radio)
-
-print("Connecting to AP...")
-while not wifi.radio.ipv4_address:
-    try:
-        wifi.radio.connect(ssid, password)
-    except ConnectionError as e:
-        print("could not connect to AP, retrying: ", e)
-print("Connected to", str(radio.ap_info.ssid, "utf-8"), "\tRSSI:", radio.ap_info.rssi)
-
-# Initialize a requests session
-ssl_context = ssl.create_default_context()
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
 requests = adafruit_requests.Session(pool, ssl_context)
+rssi = wifi.radio.ap_info.rssi
 
+# URL for GET request
 JSON_GET_URL = "https://httpbin.org/get"
+# Define a custom header as a dict.
+headers = {"user-agent": "blinka/1.0.0"}
+
+print(f"\nConnecting to {ssid}...")
+print(f"Signal Strength: {rssi}")
+try:
+    # Connect to the Wi-Fi network
+    wifi.radio.connect(ssid, password)
+except OSError as e:
+    print(f"❌ OSError: {e}")
+print("✅ Wifi!")
 
 # Define a custom header as a dict.
 headers = {"user-agent": "blinka/1.0.0"}
+print(f" | Fetching URL {JSON_GET_URL}")
 
-print("Fetching JSON data from %s..." % JSON_GET_URL)
+# Use with statement for retreiving GET request data
 with requests.get(JSON_GET_URL, headers=headers) as response:
-    print("-" * 60)
-
     json_data = response.json()
     headers = json_data["headers"]
-    print("Response's Custom User-Agent Header: {0}".format(headers["User-Agent"]))
-    print("-" * 60)
-
-    # Read Response's HTTP status code
-    print("Response HTTP Status Code: ", response.status_code)
-    print("-" * 60)
+    content_type = response.headers.get("content-type", "")
+    date = response.headers.get("date", "")
+    if response.status_code == 200:
+        print(f" | 🆗 Status Code: {response.status_code}")
+    else:
+        print(f" | ❌ Status Code: {response.status_code}")
+    print(f" |  | Custom User-Agent Header: {headers['User-Agent']}")
+    print(f" |  | Content-Type: {content_type}")
+    print(f" |  | Response Timestamp: {date}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wifi/requests_wifi_simpletest.py` & `adafruit_circuitpython_requests-3.2.7/examples/wifi/requests_wifi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit_circuitpython_requests-3.2.7/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit_circuitpython_requests-3.2.7/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/pyproject.toml` & `adafruit_circuitpython_requests-3.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.6"
+version = "3.2.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/chunk_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/chunked_redirect_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/concurrent_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/conftest.py` & `adafruit_circuitpython_requests-3.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/header_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/method_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/method_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/mocket.py` & `adafruit_circuitpython_requests-3.2.7/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/parse_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/protocol_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tests/reuse_test.py` & `adafruit_circuitpython_requests-3.2.7/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.6/tox.ini` & `adafruit_circuitpython_requests-3.2.7/tox.ini`

 * *Files identical despite different names*

