# Comparing `tmp/instawow-4.0.0.tar.gz` & `tmp/instawow-4.1.0.tar.gz`

## Comparing `instawow-4.0.0.tar` & `instawow-4.1.0.tar`

### file list

```diff
@@ -1,114 +1,123 @@
--rw-r--r--   0        0        0      159 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/__init__.py
--rw-r--r--   0        0        0      105 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/__main__.py
--rw-r--r--   0        0        0     9205 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_cli_prompts.py
--rw-r--r--   0        0        0      816 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_import_wrapper.py
--rw-r--r--   0        0        0     2719 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_logging.py
--rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_version.py
--rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_version_check.py
--rw-r--r--   0        0        0    43928 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/cli.py
--rw-r--r--   0        0        0    12071 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/config.py
--rw-r--r--   0        0        0     3527 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/definitions.py
--rw-r--r--   0        0        0     1657 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/github_auth.py
--rw-r--r--   0        0        0     3915 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/manager_ctx.py
--rw-r--r--   0        0        0     1607 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/pkg_archives.py
--rw-r--r--   0        0        0    23689 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/pkg_management.py
--rw-r--r--   0        0        0     1552 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/pkg_models.py
--rw-r--r--   0        0        0     1275 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/plugins.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/py.typed
--rw-r--r--   0        0        0     6002 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/resolvers.py
--rw-r--r--   0        0        0     5344 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/results.py
--rw-r--r--   0        0        0     8220 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/utils.py
--rw-r--r--   0        0        0     6268 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/wow_installations.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/__init__.py
--rw-r--r--   0        0        0    15108 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/cfcore.py
--rw-r--r--   0        0        0    16606 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/github.py
--rw-r--r--   0        0        0     2258 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/instawow.py
--rw-r--r--   0        0        0     3697 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/tukui.py
--rw-r--r--   0        0        0     6856 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/wago.py
--rw-r--r--   0        0        0     8901 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/_sources/wowi.py
--rw-r--r--   0        0        0     1388 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/catalogue/__init__.py
--rw-r--r--   0        0        0     3636 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/catalogue/cataloguer.py
--rw-r--r--   0        0        0     3516 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/catalogue/search.py
--rw-r--r--   0        0        0     2369 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/http/__init__.py
--rw-r--r--   0        0        0     2293 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/http/_cache.py
--rw-r--r--   0        0        0     7608 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/matchers/__init__.py
--rw-r--r--   0        0        0     2850 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/matchers/_addon_hashing.py
--rw-r--r--   0        0        0     4838 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/pkg_db/__init__.py
--rw-r--r--   0        0        0      427 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow/pkg_db/_migrations.py
--rw-r--r--   0        0        0       35 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/__init__.py
--rw-r--r--   0        0        0     1035 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_cli.py
--rw-r--r--   0        0        0    12173 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_core.py
--rw-r--r--   0        0        0     7760 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_custom_slpp.py
--rw-r--r--   0        0        0      201 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_plugin.py
--rw-r--r--   0        0        0       42 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/CHANGELOG.md
--rw-r--r--   0        0        0    18046 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/COPYING.WeakAuras-Companion
--rw-r--r--   0        0        0      223 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/README
--rw-r--r--   0        0        0      308 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/WeakAurasCompanion.toc
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/__init__.py
--rw-r--r--   0        0        0     1060 1980-01-01 00:00:00.000000 instawow-4.0.0/src/instawow_wa_updater/_templates/init.lua
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4656 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3155 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test__version.py
--rw-r--r--   0        0        0     4054 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_catalogue_search.py
--rw-r--r--   0        0        0    17923 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     8073 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_config.py
--rw-r--r--   0        0        0      429 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_github_oauth_flow.py
--rw-r--r--   0        0        0     4508 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_json_rpc_api.py
--rw-r--r--   0        0        0     4585 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_matchers.py
--rw-r--r--   0        0        0     1324 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_pkg_archives.py
--rw-r--r--   0        0        0    10297 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_pkg_management.py
--rw-r--r--   0        0        0     1253 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_resolvers.py
--rw-r--r--   0        0        0     4051 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_source__curse.py
--rw-r--r--   0        0        0     6382 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_source__github.py
--rw-r--r--   0        0        0     1305 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_source__tukui.py
--rw-r--r--   0        0        0     2217 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_source__wowi.py
--rw-r--r--   0        0        0     3288 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     3632 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_wa_updater.py
--rw-r--r--   0        0        0     5428 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_wa_updater_parser.py
--rw-r--r--   0        0        0     3819 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/test_wow_installations.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/FakeAddon/FakeAddon.lua
--rw-r--r--   0        0        0      116 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/FakeAddon/FakeAddon.toc
--rw-r--r--   0        0        0     8248 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/__init__.py
--rw-r--r--   0        0        0  6619179 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/base-catalogue-v7.compact.json
--rw-r--r--   0        0        0   216968 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/curse-addon--all.json
--rw-r--r--   0        0        0      113 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/curse-addon-changelog.json
--rw-r--r--   0        0        0    94777 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/curse-addon-files.json
--rw-r--r--   0        0        0    24261 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/curse-addon-slug-search.json
--rw-r--r--   0        0        0      115 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-oauth-login-access-token.json
--rw-r--r--   0        0        0      187 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-oauth-login-device-code.json
--rw-r--r--   0        0        0      446 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-molinari-release-json.json
--rw-r--r--   0        0        0     6273 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-molinari.json
--rw-r--r--   0        0        0     1895 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-no-assets.json
--rw-r--r--   0        0        0     7859 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-no-release-json.json
--rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-release-json-release-json.json
--rw-r--r--   0        0        0     8128 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-release-release-json.json
--rw-r--r--   0        0        0     6769 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-repo-molinari.json
--rw-r--r--   0        0        0     5612 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-repo-no-release-json.json
--rw-r--r--   0        0        0     6830 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-repo-no-releases.json
--rw-r--r--   0        0        0     5536 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/github-repo-release-json.json
--rwxr-xr-x   0        0        0     4418 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/regen.sh
--rw-r--r--   0        0        0     1398 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/tukui-ui--elvui.json
--rw-r--r--   0        0        0     1305 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/tukui-ui--tukui.json
--rw-r--r--   0        0        0      938 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/wago-match-addons.json
--rw-r--r--   0        0        0     3133 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/wowi-filedetails.json
--rw-r--r--   0        0        0      925 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/fixtures/http/wowi-filelist.json
--rw-r--r--   0        0        0     1243 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/plugin/instawow_test_plugin.py
--rw-r--r--   0        0        0      276 1980-01-01 00:00:00.000000 instawow-4.0.0/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/__init__.py
--rw-r--r--   0        0        0      834 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/_plugin.py
--rw-r--r--   0        0        0     5293 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/app.py
--rw-r--r--   0        0        0    29086 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/json_rpc_server.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/py.typed
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/__init__.py
--rw-r--r--   0        0        0      472 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/index.html
--rw-r--r--   0        0        0    18213 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/assets/index-BzfSzUDv.css
--rw-r--r--   0        0        0   603544 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/assets/index-DqShBAqA.js
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/resources/__init__.py
--rw-r--r--   0        0        0   133998 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.icns
--rw-r--r--   0        0        0     8736 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.ico
--rw-r--r--   0        0        0    60410 1980-01-01 00:00:00.000000 instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.png
--rw-r--r--   0        0        0       19 1980-01-01 00:00:00.000000 instawow-4.0.0/.gitignore
--rw-r--r--   0        0        0    35147 1980-01-01 00:00:00.000000 instawow-4.0.0/COPYING
--rw-r--r--   0        0        0     8209 1980-01-01 00:00:00.000000 instawow-4.0.0/README.rst
--rw-r--r--   0        0        0     3409 1980-01-01 00:00:00.000000 instawow-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     9572 1980-01-01 00:00:00.000000 instawow-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      159 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/__init__.py
+-rw-r--r--   0        0        0      105 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/__main__.py
+-rw-r--r--   0        0        0    13847 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_cli_prompts.py
+-rw-r--r--   0        0        0      816 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_import_wrapper.py
+-rw-r--r--   0        0        0     2719 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_logging.py
+-rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_version.py
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_version_check.py
+-rw-r--r--   0        0        0    43916 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/cli.py
+-rw-r--r--   0        0        0    12147 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/config.py
+-rw-r--r--   0        0        0     3535 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/definitions.py
+-rw-r--r--   0        0        0     1657 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/github_auth.py
+-rw-r--r--   0        0        0     4060 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/manager_ctx.py
+-rw-r--r--   0        0        0     1607 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/pkg_archives.py
+-rw-r--r--   0        0        0    27463 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/pkg_management.py
+-rw-r--r--   0        0        0     1966 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/pkg_models.py
+-rw-r--r--   0        0        0     1275 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/plugins.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/py.typed
+-rw-r--r--   0        0        0     6028 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/resolvers.py
+-rw-r--r--   0        0        0     5379 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/results.py
+-rw-r--r--   0        0        0     6649 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/wow_installations.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/__init__.py
+-rw-r--r--   0        0        0    15615 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/cfcore.py
+-rw-r--r--   0        0        0    19148 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/github.py
+-rw-r--r--   0        0        0     2263 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/instawow.py
+-rw-r--r--   0        0        0     3701 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/tukui.py
+-rw-r--r--   0        0        0     6912 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/wago.py
+-rw-r--r--   0        0        0     8936 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_sources/wowi.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/__init__.py
+-rw-r--r--   0        0        0      788 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/aio.py
+-rw-r--r--   0        0        0      845 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/compat.py
+-rw-r--r--   0        0        0      892 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/file.py
+-rw-r--r--   0        0        0     2716 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/iteration.py
+-rw-r--r--   0        0        0      307 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/perf.py
+-rw-r--r--   0        0        0     1548 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/text.py
+-rw-r--r--   0        0        0      938 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/_utils/web.py
+-rw-r--r--   0        0        0     1397 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/catalogue/__init__.py
+-rw-r--r--   0        0        0     3699 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/catalogue/cataloguer.py
+-rw-r--r--   0        0        0     3543 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/catalogue/search.py
+-rw-r--r--   0        0        0     2375 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/http/__init__.py
+-rw-r--r--   0        0        0     2500 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/http/_cache.py
+-rw-r--r--   0        0        0     7719 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/matchers/__init__.py
+-rw-r--r--   0        0        0     2854 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/matchers/_addon_hashing.py
+-rw-r--r--   0        0        0     1079 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/matchers/addon_toc.py
+-rw-r--r--   0        0        0     5482 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/pkg_db/__init__.py
+-rw-r--r--   0        0        0     1526 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow/pkg_db/_migrations.py
+-rw-r--r--   0        0        0       35 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/__init__.py
+-rw-r--r--   0        0        0     1041 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_cli.py
+-rw-r--r--   0        0        0    12404 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_core.py
+-rw-r--r--   0        0        0     7760 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_custom_slpp.py
+-rw-r--r--   0        0        0      201 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_plugin.py
+-rw-r--r--   0        0        0       42 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/CHANGELOG.md
+-rw-r--r--   0        0        0    18046 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/COPYING.WeakAuras-Companion
+-rw-r--r--   0        0        0      223 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/README
+-rw-r--r--   0        0        0      308 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/WeakAurasCompanion.toc
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/__init__.py
+-rw-r--r--   0        0        0     1060 1980-01-01 00:00:00.000000 instawow-4.1.0/src/instawow_wa_updater/_templates/init.lua
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4753 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3494 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test__version.py
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_addon_toc.py
+-rw-r--r--   0        0        0     4054 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_catalogue_search.py
+-rw-r--r--   0        0        0    17595 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     8073 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_config.py
+-rw-r--r--   0        0        0      429 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_github_oauth_flow.py
+-rw-r--r--   0        0        0     4508 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_json_rpc_api.py
+-rw-r--r--   0        0        0     4585 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_matchers.py
+-rw-r--r--   0        0        0     1324 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_pkg_archives.py
+-rw-r--r--   0        0        0    10366 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_pkg_management.py
+-rw-r--r--   0        0        0     1253 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_resolvers.py
+-rw-r--r--   0        0        0     4051 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_source__curse.py
+-rw-r--r--   0        0        0     8397 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_source__github.py
+-rw-r--r--   0        0        0     1305 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_source__tukui.py
+-rw-r--r--   0        0        0     2217 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_source__wowi.py
+-rw-r--r--   0        0        0     2317 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3632 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_wa_updater.py
+-rw-r--r--   0        0        0     5428 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_wa_updater_parser.py
+-rw-r--r--   0        0        0     4374 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/test_wow_installations.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/FakeAddon/FakeAddon.lua
+-rw-r--r--   0        0        0      116 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/FakeAddon/FakeAddon.toc
+-rw-r--r--   0        0        0     8190 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/__init__.py
+-rw-r--r--   0        0        0  6619179 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/base-catalogue-v7.compact.json
+-rw-r--r--   0        0        0   216968 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/curse-addon--all.json
+-rw-r--r--   0        0        0      113 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/curse-addon-changelog.json
+-rw-r--r--   0        0        0    94777 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/curse-addon-files.json
+-rw-r--r--   0        0        0    24261 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/curse-addon-slug-search.json
+-rw-r--r--   0        0        0      115 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-oauth-login-access-token.json
+-rw-r--r--   0        0        0      187 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-oauth-login-device-code.json
+-rw-r--r--   0        0        0      446 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-molinari-release-json.json
+-rw-r--r--   0        0        0     6273 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-molinari.json
+-rw-r--r--   0        0        0     1895 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-no-assets.json
+-rw-r--r--   0        0        0     7859 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-no-release-json.json
+-rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-release-json-release-json.json
+-rw-r--r--   0        0        0     8128 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-release-release-json.json
+-rw-r--r--   0        0        0     6769 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-repo-molinari.json
+-rw-r--r--   0        0        0     5612 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-repo-no-release-json.json
+-rw-r--r--   0        0        0     6830 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-repo-no-releases.json
+-rw-r--r--   0        0        0     5536 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/github-repo-release-json.json
+-rwxr-xr-x   0        0        0     4418 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/regen.sh
+-rw-r--r--   0        0        0     1398 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/tukui-ui--elvui.json
+-rw-r--r--   0        0        0     1305 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/tukui-ui--tukui.json
+-rw-r--r--   0        0        0      938 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/wago-match-addons.json
+-rw-r--r--   0        0        0     3133 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/wowi-filedetails.json
+-rw-r--r--   0        0        0      925 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/fixtures/http/wowi-filelist.json
+-rw-r--r--   0        0        0     1243 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/plugin/instawow_test_plugin.py
+-rw-r--r--   0        0        0      276 1980-01-01 00:00:00.000000 instawow-4.1.0/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/__init__.py
+-rw-r--r--   0        0        0      834 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/_plugin.py
+-rw-r--r--   0        0        0     5312 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/app.py
+-rw-r--r--   0        0        0    29027 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/json_rpc_server.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/py.typed
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/__init__.py
+-rw-r--r--   0        0        0      472 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/index.html
+-rw-r--r--   0        0        0    18213 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/assets/index-BzfSzUDv.css
+-rw-r--r--   0        0        0   603544 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/assets/index-DqShBAqA.js
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/resources/__init__.py
+-rw-r--r--   0        0        0   133998 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.icns
+-rw-r--r--   0        0        0     8736 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.ico
+-rw-r--r--   0        0        0    60410 1980-01-01 00:00:00.000000 instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.png
+-rw-r--r--   0        0        0       19 1980-01-01 00:00:00.000000 instawow-4.1.0/.gitignore
+-rw-r--r--   0        0        0    35147 1980-01-01 00:00:00.000000 instawow-4.1.0/COPYING
+-rw-r--r--   0        0        0     8246 1980-01-01 00:00:00.000000 instawow-4.1.0/README.rst
+-rw-r--r--   0        0        0     3361 1980-01-01 00:00:00.000000 instawow-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9545 1980-01-01 00:00:00.000000 instawow-4.1.0/PKG-INFO
```

### Comparing `instawow-4.0.0/src/instawow/_import_wrapper.py` & `instawow-4.1.0/src/instawow/_import_wrapper.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/_logging.py` & `instawow-4.1.0/src/instawow/_logging.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/_version_check.py` & `instawow-4.1.0/src/instawow/_version_check.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/cli.py` & `instawow-4.1.0/src/instawow/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
-import asyncio
 import datetime as dt
 import enum
 import textwrap
 from collections.abc import Awaitable, Callable, Collection, Iterable, Mapping, Sequence
-from functools import cached_property, partial
-from itertools import chain, repeat
+from functools import cached_property, partial, reduce
+from itertools import chain, count, repeat
 from pathlib import Path
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
 import attrs
 import click
 import click.types
-from loguru import logger
 from typing_extensions import Self
 
-from . import __version__, pkg_db, pkg_management, pkg_models
+from . import __version__, _logging, pkg_management, pkg_models
 from . import manager_ctx as _manager_ctx
 from . import results as R
-from ._logging import setup_logging
+from ._utils.compat import StrEnum
+from ._utils.iteration import all_eq, bucketise, uniq
 from .config import GlobalConfig, ProfileConfig, config_converter
-from .definitions import ChangelogFormat, Defn, SourceMetadata, Strategy
+from .definitions import ChangelogFormat, Defn, Strategy
 from .http import TraceRequestCtx, init_web_client
 from .plugins import get_plugin_commands
-from .utils import StrEnum, all_eq, gather, reveal_folder, tabulate, uniq
 from .wow_installations import Flavour
 
 _T = TypeVar('_T')
 _TStrEnum = TypeVar('_TStrEnum', bound=StrEnum)
 
 
 class Report:
@@ -99,36 +97,41 @@
     def manager(self) -> pkg_management.PkgManager:
         global_config = GlobalConfig.read().ensure_dirs()
         try:
             config = ProfileConfig.read(global_config, self._ctx.params['profile']).ensure_dirs()
         except FileNotFoundError:
             config = self._ctx.invoke(configure)
 
-        setup_logging(config.logging_dir, *self._ctx.params['verbose'])
+        _logging.setup_logging(config.logging_dir, *self._ctx.params['verbose'])
 
-        return pkg_management.PkgManager(_manager_ctx.ManagerCtx(config))
+        manager_ctx = self._ctx.with_resource(_manager_ctx.ManagerCtx(config))
+        return pkg_management.PkgManager(manager_ctx)
 
     def run_with_progress(self, awaitable: Awaitable[_T]) -> _T:
-        cache_dir = self.manager.ctx.config.global_config.http_cache_dir
-        params = self._ctx.params
+        import asyncio
 
-        if any(params['verbose']):
+        make_init_web_client = partial(
+            init_web_client,
+            self.manager.ctx.config.global_config.http_cache_dir,
+            no_cache=self._ctx.params['no_cache'],
+        )
+
+        if any(self._ctx.params['verbose']):
 
             async def run():
-                async with init_web_client(cache_dir, no_cache=params['no_cache']) as web_client:
+                async with make_init_web_client() as web_client:
                     _manager_ctx.contextualise(web_client=web_client)
                     return await awaitable
 
         else:
-            from contextlib import contextmanager
-
             import aiohttp
             from prompt_toolkit.shortcuts import ProgressBar, ProgressBarCounter
 
             from ._cli_prompts import make_progress_bar
+            from ._utils.aio import cancel_tasks
 
             def init_cli_web_client(progress_bar: ProgressBar, tickers: set[asyncio.Task[None]]):
                 TICK_INTERVAL = 0.1
 
                 async def do_on_request_end(
                     client_session: aiohttp.ClientSession,
                     trace_config_ctx: Any,
@@ -174,36 +177,27 @@
                                 counters.remove(counter)
 
                         tickers.add(asyncio.create_task(ticker()))
 
                 trace_config = aiohttp.TraceConfig()
                 trace_config.on_request_end.append(do_on_request_end)
                 trace_config.freeze()
-                return init_web_client(
-                    cache_dir, no_cache=params['no_cache'], trace_configs=[trace_config]
-                )
-
-            @contextmanager
-            def cancel_tickers(progress_bar: ProgressBar):
-                tickers: set[asyncio.Task[None]] = set()
-                try:
-                    yield tickers
-                finally:
-                    for ticker in tickers:
-                        ticker.cancel()
-                    progress_bar.invalidate()
+                return make_init_web_client(trace_configs=[trace_config])
 
             async def run():
-                with (
-                    make_progress_bar() as progress_bar,
-                    cancel_tickers(progress_bar) as tickers,
-                ):
-                    async with init_cli_web_client(progress_bar, tickers) as web_client:
-                        _manager_ctx.contextualise(web_client=web_client)
-                        return await awaitable
+                with make_progress_bar() as progress_bar:
+                    tickers = set[asyncio.Task[None]]()
+
+                    try:
+                        async with init_cli_web_client(progress_bar, tickers) as web_client:
+                            _manager_ctx.contextualise(web_client=web_client)
+                            return await awaitable
+
+                    finally:
+                        await cancel_tasks(tickers)
 
         return asyncio.run(run())
 
 
 def _with_manager(fn: Callable[..., object]):
     def wrapper(ctx: click.Context, __: click.Parameter, value: object):
         return fn(ctx.obj.manager, value)
@@ -276,39 +270,27 @@
 
 def _parse_debug_option(
     _: click.Context, __: click.Parameter, value: float
 ) -> tuple[bool, bool, bool]:
     return (value > 0, value > 1, value > 2)
 
 
-@click.group(context_settings={'help_option_names': ('-h', '--help')})
-@click.version_option(__version__, prog_name=__spec__.parent)
-@click.option(
-    '--verbose',
-    '-v',
-    count=True,
-    help='Log incrementally more things.  Additive.',
-    callback=_parse_debug_option,
-)
-@click.option(
-    '--no-cache',
-    is_flag=True,
-    default=False,
-    help='Disable the HTTP cache.',
-)
-@click.option(
-    '--profile',
-    '-p',
-    default='__default__',
-    help='Activate the specified profile.',
-)
-@click.pass_context
-def cli(ctx: click.Context, **__: object) -> None:
-    "Add-on manager for World of Warcraft."
-    ctx.obj = CtxObjWrapper(ctx)
+class _SectionedHelpGroup(click.Group):
+    def format_commands(self, ctx: click.Context, formatter: click.HelpFormatter) -> None:
+        command_sections = bucketise(
+            ((s, c) for s, c in self.commands.items() if not c.hidden),
+            key=lambda c: 'Command groups' if isinstance(c[1], click.Group) else 'Commands',
+        )
+        if command_sections:
+            for section_name, commands in command_sections.items():
+                with formatter.section(section_name):
+                    limit = formatter.width - 6 - max(len(s) for s, _ in commands)
+                    formatter.write_dl(
+                        [(s, c.get_short_help_str(limit)) for s, c in commands],
+                    )
 
 
 @overload
 def _parse_uri(
     manager: pkg_management.PkgManager,
     value: str,
     *,
@@ -350,14 +332,77 @@
             defn = attrs.evolve(defn, source=source, alias=alias)
         elif raise_invalid and ':' not in defn.alias:
             raise click.BadParameter(value)
 
     return defn
 
 
+def _make_pkg_where_clause_and_params(defns: Sequence[Defn]) -> tuple[str, dict[str, Any]]:
+    def make_inner():
+        iter_named_param = (f'where_param_{i}' for i in count())
+        for defn, source_param, alias_param in zip(defns, iter_named_param, iter_named_param):
+            if not defn.source:
+                yield (
+                    f"(pkg.slug LIKE '%' || :{alias_param} || '%')",
+                    {alias_param: defn.alias},
+                )
+            elif not defn.alias:
+                yield (
+                    f'pkg.source = :{source_param}',
+                    {source_param: defn.source},
+                )
+            else:
+                yield (
+                    f'pkg.source = :{source_param} AND (pkg.id = :{alias_param} OR lower(pkg.slug) = lower(:{alias_param}))',
+                    {source_param: defn.source, alias_param: defn.alias},
+                )
+
+    if defns:
+        where_clauses, where_params = zip(*make_inner())
+        return (
+            'WHERE\n  ' + '\n  OR '.join(where_clauses),
+            reduce(lambda a, b: a | b, where_params, {}),
+        )
+    else:
+        return ('', {})
+
+
+class _ListFormat(StrEnum):
+    Simple = enum.auto()
+    Detailed = enum.auto()
+    Json = enum.auto()
+
+
+@click.group(context_settings={'help_option_names': ('-h', '--help')}, cls=_SectionedHelpGroup)
+@click.version_option(__version__, prog_name=__spec__.parent)
+@click.option(
+    '--verbose',
+    '-v',
+    count=True,
+    help='Log incrementally more things.  Additive.',
+    callback=_parse_debug_option,
+)
+@click.option(
+    '--no-cache',
+    is_flag=True,
+    default=False,
+    help='Disable the HTTP cache.',
+)
+@click.option(
+    '--profile',
+    '-p',
+    default='__default__',
+    help='Activate the specified profile.',
+)
+@click.pass_context
+def cli(ctx: click.Context, **__: object) -> None:
+    "Add-on manager for World of Warcraft."
+    ctx.obj = CtxObjWrapper(ctx)
+
+
 @cli.command
 @click.argument('addons', nargs=-1, callback=_with_manager(_parse_uri))
 @click.option(
     '--replace',
     'replace_folders',
     is_flag=True,
     default=False,
@@ -398,32 +443,18 @@
     mw: CtxObjWrapper,
     addons: Sequence[Defn],
     dry_run: bool,
 ) -> None:
     "Update installed add-ons."
 
     def filter_results(result: R.Result):
-        # Hide packages from output if they are up to date
-        # and ``update`` was invoked without args,
-        # provided that they are not pinned
-        if addons or not isinstance(result, R.PkgUpToDate):
-            return True
-        else:
-            return result.is_pinned
-
-    def installed_pkgs_to_defns():
-        with mw.manager.ctx.database.connect() as connection:
-            return [
-                mw.manager.build_pkg_from_row_mapping(connection, p).to_defn()
-                for p in connection.execute(pkg_db.sa.select(pkg_db.pkg)).mappings().all()
-            ]
+        # Hide packages from output if they are up to date and not pinned.
+        return True if addons or not isinstance(result, R.PkgUpToDate) else result.is_pinned
 
-    results = mw.run_with_progress(
-        mw.manager.update(addons or installed_pkgs_to_defns(), dry_run=dry_run)
-    )
+    results = mw.run_with_progress(mw.manager.update(addons or 'all', dry_run=dry_run))
     Report(results.items(), filter_results).generate_and_exit()
 
 
 @cli.command
 @click.argument('addons', nargs=-1, required=True, callback=_with_manager(_parse_uri))
 @click.option(
     '--keep-folders',
@@ -445,15 +476,15 @@
     is_flag=True,
     default=False,
     help='Undo rollback by reinstalling an add-on using the default strategy.',
 )
 @click.pass_obj
 def rollback(mw: CtxObjWrapper, addon: Defn, undo: bool) -> None:
     "Roll an add-on back to an older version."
-    from ._cli_prompts import Choice, ask, select
+    from ._cli_prompts import Choice, select_one
 
     pkg = mw.manager.get_pkg(addon)
     if not pkg:
         Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
     elif Strategy.VersionEq not in mw.manager.ctx.resolvers[pkg.source].metadata.strategies:
         Report([(addon, R.PkgStrategiesUnsupported({Strategy.VersionEq}))]).generate_and_exit()
     elif undo:
@@ -464,24 +495,19 @@
     reconstructed_defn = pkg.to_defn()
 
     versions = pkg.logged_versions
     if len(versions) <= 1:
         Report([(addon, R.PkgFilesMissing('cannot find older versions'))]).generate_and_exit()
 
     choices = [
-        Choice(
-            [('', v.version)],
-            value=v.version,
-            disabled='installed version' if v.version == pkg.version else None,
-        )
-        for v in versions
+        Choice(v.version, value=v.version, disabled=v.version == pkg.version) for v in versions
     ]
-    selection = ask(
-        select(f'Select version of {reconstructed_defn.as_uri()} for rollback', choices)
-    )
+    selection = select_one(
+        f'Select version of {reconstructed_defn.as_uri()} for rollback', choices
+    ).prompt()
 
     Report(
         mw.run_with_progress(
             mw.manager.update([reconstructed_defn.with_version(selection)])
         ).items()
     ).generate_and_exit()
 
@@ -497,26 +523,27 @@
 )
 @click.option(
     '--list-unreconciled', is_flag=True, default=False, help='List unreconciled add-ons and exit.'
 )
 @click.pass_obj
 def reconcile(mw: CtxObjWrapper, auto: bool, rereconcile: bool, list_unreconciled: bool) -> None:
     "Reconcile pre-installed add-ons."
-    from ._cli_prompts import PkgChoice, ask, confirm, select, skip
+    from ._cli_prompts import SKIP, Choice, confirm, select_one
+    from ._utils.text import tabulate
     from .matchers import DEFAULT_MATCHERS, AddonFolder, get_unreconciled_folders
 
     def construct_choice(pkg: pkg_models.Pkg, highlight_version: bool, disabled: bool):
         defn = pkg.to_defn()
-        return PkgChoice(
+        return Choice(
             [
                 ('', f'{defn.as_uri()}=='),
-                ('class:highlight-sub' if highlight_version else '', pkg.version),
+                ('class:attention' if highlight_version else '', pkg.version),
             ],
-            pkg=pkg,
-            value=defn,
+            defn,
+            browser_url=pkg.url,
             disabled=disabled,
         )
 
     def gather_selections(
         groups: Collection[tuple[_T, Sequence[Defn]]],
         selector: Callable[[_T, Sequence[pkg_models.Pkg]], Defn | None],
     ):
@@ -534,38 +561,33 @@
             raise click.UsageError('Cannot use "--auto" with "--installed"')
 
         def select_alternative_pkg(installed_pkg: pkg_models.Pkg, pkgs: Sequence[pkg_models.Pkg]):
             highlight_version = not all_eq(i.version for i in (installed_pkg, *pkgs))
             choices = [
                 construct_choice(installed_pkg, highlight_version, True),
                 *(construct_choice(p, highlight_version, False) for p in pkgs),
-                skip,
             ]
-            selection = ask(select(installed_pkg.name, choices))
-            return selection or None
+            selection = select_one(installed_pkg.name, choices, can_skip=True).prompt()
+            return selection if selection is not SKIP else None
 
         with mw.manager.ctx.database.connect() as connection:
             installed_pkgs = [
                 mw.manager.build_pkg_from_row_mapping(connection, p)
-                for p in connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg).order_by(pkg_db.sa.func.lower(pkg_db.pkg.c.name))
-                )
-                .mappings()
-                .all()
+                for p in connection.execute('SELECT * FROM pkg ORDER BY lower(name)').fetchall()
             ]
 
         groups = mw.run_with_progress(mw.manager.find_equivalent_pkg_defns(installed_pkgs))
         selections = [
             (p, s)
             for (p, _), s in zip(
                 groups.items(), gather_selections(groups.items(), select_alternative_pkg)
             )
             if s
         ]
-        if selections and ask(confirm('Install selected add-ons?')):
+        if selections and confirm('Install selected add-ons?').prompt():
 
             def install_selections(*, dry_run: bool):
                 return mw.run_with_progress(
                     mw.manager.install(
                         [s for _, s in selections], replace_folders=False, dry_run=dry_run
                     )
                 )
@@ -614,28 +636,27 @@
 
         def select_pkg(addons: Sequence[AddonFolder], pkgs: Sequence[pkg_models.Pkg]):
             def combine_names():
                 return textwrap.shorten(', '.join(a.name for a in addons), 60)
 
             # Highlight version if there's multiple of them
             highlight_version = not all_eq(i.version for i in chain(addons, pkgs))
-            choices = [
-                *(construct_choice(p, highlight_version, False) for p in pkgs),
-                skip,
-            ]
-            selection = ask(select(f'{combine_names()} [{addons[0].version or "?"}]', choices))
-            return selection or None
+
+            selection = select_one(
+                f'{combine_names()} [{addons[0].version or "?"}]',
+                [construct_choice(p, highlight_version, False) for p in pkgs],
+                can_skip=True,
+            ).prompt()
+            return selection if selection is not SKIP else None
 
         def pick_first_pkg(addons: Sequence[AddonFolder], pkgs: Sequence[pkg_models.Pkg]):
             return pkgs[0].to_defn()
 
         select_pkg_ = pick_first_pkg if auto else select_pkg
-        confirm_install = (
-            (lambda: True) if auto else (lambda: ask(confirm('Install selected add-ons?')))
-        )
+        confirm_install = (lambda: True) if auto else confirm('Install selected add-ons?').prompt
 
         for fn in DEFAULT_MATCHERS.values():
             groups = mw.run_with_progress(fn(mw.manager.ctx, leftovers))
             selections = [s for s in gather_selections(groups, select_pkg_) if s is not None]
             if selections and confirm_install():
                 results = mw.run_with_progress(
                     mw.manager.install(selections, replace_folders=True)
@@ -700,15 +721,15 @@
     limit: int,
     sources: Sequence[str],
     prefer_source: str | None,
     start_date: dt.datetime | None,
     no_exclude_installed: bool,
 ) -> None:
     "Search for add-ons to install."
-    from ._cli_prompts import PkgChoice, ask, checkbox, confirm
+    from ._cli_prompts import Choice, confirm, select_multiple
     from .catalogue.search import search
 
     mw: CtxObjWrapper = ctx.obj
 
     catalogue_entries = mw.run_with_progress(
         search(
             mw.manager.ctx,
@@ -722,38 +743,32 @@
     )
     results = mw.run_with_progress(
         mw.manager.resolve([Defn(e.source, e.id) for e in catalogue_entries])
     )
     pkgs, _ = pkg_management.bucketise_results(results.items())
     if pkgs:
         choices = [
-            PkgChoice(f'{p.name}  ({e.as_uri()}=={p.version})', e, pkg=p)
+            Choice(f'{p.name}  ({e.as_uri()}=={p.version})', e, browser_url=p.url)
             for d, p in pkgs.items()
             for e in (attrs.evolve(d, alias=p.slug, id=p.id),)
         ]
-        selections: list[Defn] = ask(checkbox('Select add-ons to install', choices=choices))
+        selections = select_multiple('Select add-ons to install', choices=choices).prompt()
         if selections:
-            if ask(confirm('Install selected add-ons?')):
+            if confirm('Install selected add-ons?').prompt():
                 ctx.invoke(install, addons=selections, replace_folders=False, dry_run=False)
         else:
             click.echo(
                 'Nothing was selected; select add-ons with <space>'
                 ' and confirm by pressing <enter>.'
             )
 
     else:
         click.echo('No results found.')
 
 
-class _ListFormat(StrEnum):
-    Simple = enum.auto()
-    Detailed = enum.auto()
-    Json = enum.auto()
-
-
 @cli.command('list')
 @click.argument(
     'addons', nargs=-1, callback=_with_manager(partial(_parse_uri, raise_invalid=False))
 )
 @click.option(
     '--format',
     '-f',
@@ -764,74 +779,52 @@
     help='Change the output format.',
 )
 @click.pass_obj
 def list_installed(mw: CtxObjWrapper, addons: Sequence[Defn], output_format: _ListFormat) -> None:
     "List installed add-ons."
 
     with mw.manager.ctx.database.connect() as connection:
-
-        def make_addon_filter(defn: Defn):
-            if not defn.source:
-                return pkg_db.pkg.c.slug.contains(defn.alias)
-
-            query = pkg_db.pkg.c.source == defn.source
-            if defn.alias:
-                query &= (pkg_db.pkg.c.id == defn.alias) | (
-                    pkg_db.sa.func.lower(pkg_db.pkg.c.slug) == pkg_db.sa.func.lower(defn.alias)
-                )
-            return query
-
-        pkg_select_query = pkg_db.sa.select(pkg_db.pkg)
-        if addons:
-            pkg_select_query = pkg_select_query.filter(
-                pkg_db.sa.or_(*(make_addon_filter(d) for d in addons))
-            )
-
-        pkg_mappings = (
-            connection.execute(
-                pkg_select_query.order_by(
-                    pkg_db.pkg.c.source, pkg_db.sa.func.lower(pkg_db.pkg.c.name)
-                )
-            )
-            .mappings()
-            .all()
-        )
+        where_clause, where_params = _make_pkg_where_clause_and_params(addons)
+        pkg_mappings = connection.execute(
+            f"""
+                SELECT *
+                FROM pkg
+                {where_clause}
+                ORDER BY source, lower(name)
+            """,
+            where_params,
+        ).fetchall()
 
         def row_mappings_to_pkgs():
             return map(mw.manager.build_pkg_from_row_mapping, repeat(connection), pkg_mappings)
 
         match output_format:
             case _ListFormat.Json:
                 from cattrs.preconf.json import make_converter
 
-                json_converter = make_converter()
                 click.echo(
-                    json_converter.dumps(
-                        row_mappings_to_pkgs(),
-                        list[pkg_models.Pkg],
-                        indent=2,
-                    )
+                    make_converter().dumps(list(row_mappings_to_pkgs()), indent=2),
                 )
 
             case _ListFormat.Detailed:
-                formatter = click.HelpFormatter(max_width=99)
 
                 def format_deps(pkg: pkg_models.Pkg):
                     return (
                         Defn(pkg.source, s or e.id).as_uri()
                         for e in pkg.deps
-                        for s in (
+                        for (s,) in (
                             connection.execute(
-                                pkg_db.sa.select(pkg_db.pkg.c.slug).filter_by(
-                                    source=pkg.source, id=e.id
-                                )
-                            ).scalar_one_or_none(),
+                                'SELECT slug FROM pkg WHERE source = :source AND id = :id',
+                                {'source': pkg.source, 'id': pkg.id},
+                            ).fetchone(),
                         )
                     )
 
+                formatter = click.HelpFormatter(max_width=99)
+
                 for pkg in row_mappings_to_pkgs():
                     with formatter.section(pkg.to_defn().as_uri()):
                         formatter.write_dl(
                             [
                                 ('name', pkg.name),
                                 ('description', textwrap.shorten(pkg.description, 280)),
                                 ('url', pkg.url),
@@ -866,39 +859,55 @@
 
 
 @cli.command
 @click.argument('addon', callback=_with_manager(partial(_parse_uri, raise_invalid=False)))
 @click.pass_obj
 def reveal(mw: CtxObjWrapper, addon: Defn) -> None:
     "Bring an add-on up in your file manager."
-    pkg = mw.manager.get_pkg(addon, partial_match=True)
-    if pkg:
-        reveal_folder(mw.manager.ctx.config.addon_dir / pkg.folders[0].name)
-    else:
-        Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
+    from ._utils.file import reveal_folder
+
+    with mw.manager.ctx.database.connect() as connection:
+        where_clause, where_params = _make_pkg_where_clause_and_params([addon])
+        pkg_folder = connection.execute(
+            f"""
+                SELECT pkg_folder.name
+                FROM pkg
+                JOIN pkg_folder ON pkg.source = pkg_folder.pkg_source AND pkg.id = pkg_folder.pkg_id
+                {where_clause}
+                LIMIT 1
+                """,
+            where_params,
+        ).fetchone()
+
+        if pkg_folder:
+            reveal_folder(mw.manager.ctx.config.addon_dir / pkg_folder['name'])
+        else:
+            Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
 
 
 @cli.command
 @click.argument(
-    'addon', callback=_with_manager(partial(_parse_uri, raise_invalid=False)), required=False
+    'addons', nargs=-1, callback=_with_manager(partial(_parse_uri, raise_invalid=False))
 )
 @click.option(
     '--convert/--no-convert',
     default=True,
     show_default=True,
-    help='Convert HTML and Markdown changelogs to plain text using pandoc.',
+    help='Convert HTML and Markdown changelogs to plain text using pandoc. No-op if pandoc is not installed.',
 )
 @click.pass_obj
-def view_changelog(mw: CtxObjWrapper, addon: Defn | None, convert: bool) -> None:
+def view_changelog(mw: CtxObjWrapper, addons: Sequence[Defn], convert: bool) -> None:
     """View the changelog of an installed add-on.
 
-    If `addon` is not provided, displays the changelogs of all add-ons
-    to have been installed within one minute of the last add-on.
+    If `ADDONS` is not provided, displays the changelogs of all add-ons
+    to have been installed within one minute of the newest add-on.
     """
 
+    from ._utils.aio import gather
+
     MAX_LINES = 100
 
     def make_converter():
         import shutil
 
         pandoc = shutil.which('pandoc')
         if pandoc is None:
@@ -936,105 +945,56 @@
             (
                 *(f'  {i}' for i in lines[:MAX_LINES]),
                 *(('  [...]',) if len(lines) > MAX_LINES else ()),
             )
         )
         return f'{Defn(source, slug).as_uri()}:\n{body}'
 
-    if addon:
-        pkg = mw.manager.get_pkg(addon, partial_match=True)
-        if pkg:
-            changelog = mw.run_with_progress(
-                mw.manager.get_changelog(pkg.source, pkg.changelog_url)
-            )
-            if convert:
-                changelog = make_converter()(pkg.source, changelog)
-
-            click.echo_via_pager(format_combined_changelog_entry(pkg.source, pkg.slug, changelog))
+    with mw.manager.ctx.database.connect() as connection:
+        query = """
+            SELECT pkg.source, pkg.slug, pkg.changelog_url
+            FROM pkg
+        """
+        if addons:
+            where_clause, query_params = _make_pkg_where_clause_and_params(addons)
+            last_installed_changelog_urls = connection.execute(
+                query + where_clause, query_params
+            ).fetchall()
 
         else:
-            Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
-
-    else:
-        with mw.manager.ctx.database.connect() as connection:
-            join_clause = (pkg_db.pkg.c.source == pkg_db.pkg_version_log.c.pkg_source) & (
-                pkg_db.pkg.c.id == pkg_db.pkg_version_log.c.pkg_id
-            )
-            last_installed_changelog_urls = connection.execute(
-                pkg_db.sa.select(
-                    pkg_db.pkg.c.source, pkg_db.pkg.c.slug, pkg_db.pkg.c.changelog_url
-                )
-                .join(pkg_db.pkg_version_log, join_clause)
-                .filter(
-                    pkg_db.pkg_version_log.c.install_time
-                    >= pkg_db.sa.select(
-                        pkg_db.sa.func.datetime(
-                            pkg_db.sa.func.max(pkg_db.pkg_version_log.c.install_time), '-1 minute'
-                        )
-                    )
-                    .join(pkg_db.pkg, join_clause)
-                    .scalar_subquery()
+            query += """
+                JOIN pkg_version_log ON pkg.source = pkg_version_log.pkg_source AND pkg.id = pkg_version_log.pkg_id
+                WHERE pkg_version_log.install_time >= (
+                    SELECT datetime(max(pkg_version_log.install_time), '-1 minute')
+                    FROM pkg_version_log
+                    JOIN pkg ON pkg.source = pkg_version_log.pkg_source AND pkg.id = pkg_version_log.pkg_id
                 )
-            ).all()
+            """
+            last_installed_changelog_urls = connection.execute(query).fetchall()
 
-        changelogs = mw.run_with_progress(
-            gather(
-                mw.manager.get_changelog(m.source, m.changelog_url)
-                for m in last_installed_changelog_urls
-            )
+    changelogs = mw.run_with_progress(
+        gather(
+            mw.manager.get_changelog(m['source'], m['changelog_url'])
+            for m in last_installed_changelog_urls
         )
-        if convert:
-            do_convert = make_converter()
-            changelogs = (
-                do_convert(m.source, c) for m, c in zip(last_installed_changelog_urls, changelogs)
-            )
-
-        click.echo_via_pager(
-            '\n\n'.join(
-                format_combined_changelog_entry(m.source, m.slug, c)
-                for m, c in zip(last_installed_changelog_urls, changelogs)
-            )
+    )
+    if convert:
+        do_convert = make_converter()
+        changelogs = (
+            do_convert(m['source'], c) for m, c in zip(last_installed_changelog_urls, changelogs)
         )
 
-
-@cli.command
-@click.option(
-    '--format',
-    '-f',
-    'output_format',
-    type=click.Choice([_ListFormat.Json]),
-    default=_ListFormat.Json,
-    show_default=True,
-    help='Change the output format.',
-)
-@click.pass_obj
-def list_sources(mw: CtxObjWrapper, output_format: _ListFormat) -> None:
-    "Print source metadata."
-    from cattrs.preconf.json import make_converter
-
-    json_converter = make_converter()
-
-    click.echo(
-        json_converter.dumps(
-            [r.metadata for r in mw.manager.ctx.resolvers.values()],
-            list[SourceMetadata],
-            indent=2,
+    click.echo_via_pager(
+        '\n\n'.join(
+            format_combined_changelog_entry(m['source'], m['slug'], c)
+            for m, c in zip(last_installed_changelog_urls, changelogs)
         )
     )
 
 
-@cli.command
-@click.pass_obj
-def debug(
-    mw: CtxObjWrapper,
-) -> None:
-    "Display debugging information."
-    click.echo(mw.manager.ctx.config.encode_for_display())
-
-
 async def _github_oauth_flow():
     from .github_auth import get_codes, poll_for_access_token
 
     async with init_web_client(None) as web_client:
         codes = await get_codes(web_client)
         click.echo(f'Navigate to {codes["verification_uri"]} and paste the code below:')
         click.echo(f'  {codes["user_code"]}')
@@ -1084,23 +1044,24 @@
 
     \b
     * ``configure addon_dir`` will initiate an interactive session
       with autocompletion
     * ``configure "addon_dir=~/foo"` will set ``addon_dir``'s value
       to ``~/foo`` immediately
     """
+    import asyncio
+
     from ._cli_prompts import (
+        SKIP,
         AttrsFieldValidator,
         Choice,
-        ask,
         confirm,
         password,
         path,
-        select,
-        skip,
+        select_one,
     )
     from .wow_installations import (
         ADDON_DIR_PARTS,
         find_installations,
         infer_flavour_from_addon_dir,
     )
 
@@ -1110,15 +1071,15 @@
 
     config_values: dict[str, Any] | None = None
     try:
         config_values = attrs.asdict(ProfileConfig.read(existing_global_config, profile))
     except FileNotFoundError:
         pass
     except Exception:
-        logger.exception('unable to read existing config')
+        _logging.logger.exception('unable to read existing config')
 
     is_new_profile = config_values is None
     if is_new_profile:
         config_values = {'profile': profile, 'global_config': attrs.asdict(existing_global_config)}
     assert config_values
 
     editable_config_values = dict(editable_config_values)
@@ -1146,27 +1107,20 @@
         known_installations = list(existing_global_config.iter_installations())
         unimported_installations = [
             (k, v and v['flavour'])
             for k, v in find_installations()
             if not any(d.samefile(k) for d in known_installations)
         ]
         if unimported_installations:
-            selection: tuple[Path, Flavour | None] | tuple[()] = ask(
-                select(
-                    'Installation:',
-                    choices=[
-                        *(
-                            Choice(title=f'{k}  [{v}]', value=(k, v))
-                            for k, v in unimported_installations
-                        ),
-                        skip,
-                    ],
-                )
-            )
-            if selection:
+            selection = select_one(
+                'Installation',
+                [Choice(f'{k}  [{v}]', (k, v)) for k, v in unimported_installations],
+                can_skip=True,
+            ).prompt()
+            if selection is not SKIP:
                 (installation_path, flavour) = selection
 
                 addon_dir = installation_path.joinpath(*ADDON_DIR_PARTS)
                 addon_dir.mkdir(exist_ok=True)
 
                 editable_config_values |= {
                     _EditableConfigOptions.AddonDir: addon_dir,
@@ -1174,71 +1128,68 @@
                 }
                 installation_configured = 2 if flavour else 1
 
     if (
         installation_configured == 0
         and _EditableConfigOptions.AddonDir in interactive_editable_config_keys
     ):
-        editable_config_values[_EditableConfigOptions.AddonDir] = ask(
-            path(
-                'Add-on directory:',
-                only_directories=True,
-                validate=AttrsFieldValidator(
-                    attrs.fields(attrs.resolve_types(ProfileConfig)).addon_dir,
-                    config_converter,
-                ),
-            )
-        )
+        editable_config_values[_EditableConfigOptions.AddonDir] = path(
+            'Add-on directory',
+            only_directories=True,
+            validator=AttrsFieldValidator(
+                attrs.fields(attrs.resolve_types(ProfileConfig)).addon_dir,
+                config_converter,
+            ),
+        ).prompt()
 
     if (
         installation_configured < 2
         and _EditableConfigOptions.GameFlavour in interactive_editable_config_keys
     ):
-        editable_config_values[_EditableConfigOptions.GameFlavour] = ask(
-            select(
-                'Game flavour:',
-                choices=list(Flavour),
-                initial_choice=config_values.get('addon_dir')
-                and infer_flavour_from_addon_dir(config_values['addon_dir']),
-            )
-        )
+        editable_config_values[_EditableConfigOptions.GameFlavour] = select_one(
+            'Game flavour',
+            list(map(Choice, Flavour, Flavour)),
+            initial_choice=config_values.get('addon_dir')
+            and infer_flavour_from_addon_dir(config_values['addon_dir']),
+        ).prompt()
 
     if _EditableConfigOptions.AutoUpdateCheck in interactive_editable_config_keys:
-        editable_config_values[_EditableConfigOptions.AutoUpdateCheck] = ask(
-            confirm('Periodically check for instawow updates?')
-        )
+        editable_config_values[_EditableConfigOptions.AutoUpdateCheck] = confirm(
+            'Periodically check for instawow updates?'
+        ).prompt()
 
-    if _EditableConfigOptions.GithubAccessToken in interactive_editable_config_keys and ask(
-        confirm('Set up GitHub authentication?')
+    if (
+        _EditableConfigOptions.GithubAccessToken in interactive_editable_config_keys
+        and confirm('Set up GitHub authentication?').prompt()
     ):
         editable_config_values[_EditableConfigOptions.GithubAccessToken] = asyncio.run(
             asyncio.wait_for(_github_oauth_flow(), timeout=60 * 5)
         )
 
     if _EditableConfigOptions.CfcoreAccessToken in interactive_editable_config_keys:
         click.echo(
             textwrap.fill(
                 'An access token is required to use CurseForge. '
                 'Log in to https://console.curseforge.com/ to generate an access token.'
             )
         )
         editable_config_values[_EditableConfigOptions.CfcoreAccessToken] = (
-            ask(password('CFCore access token:')) or None
+            password('CFCore access token:').prompt() or None
         )
 
     if _EditableConfigOptions.WagoAddonsAccessToken in interactive_editable_config_keys:
         click.echo(
             textwrap.fill(
                 'An access token is required to use Wago Addons. '
                 'Wago issues tokens to Patreon subscribers above a certain tier. '
                 'See https://addons.wago.io/patreon for more information.'
             )
         )
         editable_config_values[_EditableConfigOptions.WagoAddonsAccessToken] = (
-            ask(password('Wago Addons access token:')) or None
+            password('Wago Addons access token:').prompt() or None
         )
 
     for key, value in editable_config_values.items():
         parent = config_values
         for part in key.path[:-1]:
             parent = parent[part]
         parent[key.path[-1]] = value
@@ -1250,14 +1201,41 @@
     click.echo('Configuration written to:')
     click.echo(f'  {config.global_config.config_file}')
     click.echo(f'  {config.config_file}')
 
     return config
 
 
+@cli.group('debug')
+def _debug_group():
+    "Retrieve debugging information."
+
+
+@_debug_group.command('config')
+@click.pass_obj
+def debug_config(mw: CtxObjWrapper) -> None:
+    "Print the active configuration."
+    import json
+
+    click.echo(json.dumps(mw.manager.ctx.config.unstructure_for_display(), indent=2))
+
+
+@_debug_group.command('sources')
+@click.pass_obj
+def debug_sources(mw: CtxObjWrapper) -> None:
+    "Print active source metadata."
+    from cattrs.preconf.json import make_converter
+
+    json_converter = make_converter()
+
+    click.echo(
+        json_converter.dumps([r.metadata for r in mw.manager.ctx.resolvers.values()], indent=2)
+    )
+
+
 @_register_plugin_commands
 @cli.group('plugins')
 def _plugin_group() -> None:  # pyright: ignore[reportUnusedFunction]
     "Registered plug-ins."
 
 
 @cli.command(hidden=True)
@@ -1265,14 +1243,15 @@
     '--start-date',
     callback=_parse_iso_date_into_datetime,
     help='Omit results before this date.',
     metavar='YYYY-MM-DD',
 )
 def generate_catalogue(start_date: dt.datetime | None) -> None:
     "Generate the master catalogue."
+    import asyncio
     import json
 
     from .catalogue.cataloguer import Catalogue, catalogue_converter
 
     catalogue = asyncio.run(
         Catalogue.collate((r.catalogue for r in _manager_ctx.ManagerCtx.RESOLVERS), start_date)
     )
```

### Comparing `instawow-4.0.0/src/instawow/config.py` & `instawow-4.1.0/src/instawow/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 import json
 import os
 import sys
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sized
 from functools import lru_cache, partial
 from pathlib import Path
 from tempfile import gettempdir
-from typing import Any, TypedDict, TypeVar
+from typing import Any, NewType, TypedDict, TypeVar
 
 import attrs
 import cattrs
 import cattrs.gen
 import cattrs.preconf.json
 from typing_extensions import Self
 
-from .utils import add_exc_note, fauxfrozen, trash
+from ._utils.compat import add_exc_note, fauxfrozen
+from ._utils.file import trash
 from .wow_installations import Flavour, get_installation_dir_from_addon_dir
 
 _T = TypeVar('_T')
 
-_MISSING = object()
+_missing = object()
 
 _BOTTOM_DIR_NAME = 'instawow'
 
 
-class SecretStr(str):
-    pass
+SecretStr = NewType('SecretStr', str)
 
 
 def _expand_path(value: Path):
     return Path(os.path.abspath(os.path.expanduser(value)))
 
 
 def _is_writable_dir(value: Path):
@@ -39,14 +39,16 @@
 
 def _ensure_dirs(dirs: Iterable[Path]):
     for dir_ in dirs:
         dir_.mkdir(exist_ok=True, parents=True)
 
 
 def _enrich_validator_exc(validator: Callable[[object, attrs.Attribute[_T], _T], None]):
+    "Pretend validation error originates from cattrs for uniformity."
+
     def wrapper(model: object, attr: attrs.Attribute[_T], value: _T):
         try:
             validator(model, attr, value)
         except BaseException as exc:
             note = f'Structuring class {model.__class__.__name__} @ attribute {attr.name}'
             add_exc_note(exc, cattrs.AttributeValidationNote(note, attr.name, attr.type))
             raise
@@ -65,20 +67,17 @@
     def _validate_min_length(_model: object, _attr: attrs.Attribute[Sized], value: Sized):
         if len(value) < min_length:
             raise ValueError(f'Value must have a minimum length of {min_length}')
 
     return _validate_min_length
 
 
-def _encode_config_for_display(config: object):
+def _unstructure_config_for_display(config: object):
     converter = _make_display_converter()
-    return json.dumps(
-        converter.unstructure(config),
-        indent=2,
-    )
+    return converter.unstructure(config)
 
 
 def _write_config(config: object, config_path: Path):
     converter = _make_write_converter()
     config_path.write_text(
         json.dumps(converter.unstructure(config), indent=2),
         encoding='utf-8',
@@ -107,16 +106,16 @@
         return value
 
 
 def _read_env_vars(config_cls: Any, values: Mapping[str, object]):
     return {
         f.name: v
         for f in attrs.fields(config_cls)
-        for v in (_compute_var(f, values.get(f.name, _MISSING)),)
-        if v is not _MISSING
+        for v in (_compute_var(f, values.get(f.name, _missing)),)
+        if v is not _missing
     }
 
 
 def _make_attrs_instance_hook_factory(converter: cattrs.Converter, type_: type[Any]):
     "Allow passing in a structured attrs instance to ``structure``."
     structure = converter.gen_structure_attrs_fromdict(type_)
 
@@ -344,16 +343,16 @@
     @classmethod
     def read(cls, global_config: GlobalConfig, profile: str, *, env: bool = True) -> Self:
         dummy_config = cls.make_dummy_config(global_config=global_config, profile=profile)
         return cls.from_values(
             {**_read_config(dummy_config.config_file), 'global_config': global_config}, env=env
         )
 
-    def encode_for_display(self) -> str:
-        return _encode_config_for_display(self)
+    def unstructure_for_display(self) -> str:
+        return _unstructure_config_for_display(self)
 
     def ensure_dirs(self) -> Self:
         _ensure_dirs(
             [
                 self.config_dir,
                 self.state_dir,
                 self.logging_dir,
@@ -387,15 +386,15 @@
         return self.state_dir / 'plugins'
 
     @property
     def config_file(self) -> Path:
         return self.config_dir / 'config.json'
 
     @property
-    def db_uri(self) -> str:
-        return f"sqlite:///{self.config_dir / 'db.sqlite'}"
+    def db_file(self) -> Path:
+        return self.config_dir / 'db.sqlite'
 
 
 config_converter = make_config_converter()
 config_converter.register_structure_hook_factory(
     attrs.has, partial(_make_attrs_instance_hook_factory, config_converter)
 )
```

### Comparing `instawow-4.0.0/src/instawow/definitions.py` & `instawow-4.1.0/src/instawow/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from typing import Literal
 
 import attrs
 from typing_extensions import Self
 from yarl import URL
 
-from .utils import StrEnum, fauxfrozen
+from ._utils.compat import StrEnum, fauxfrozen
 
 
 class Strategy(StrEnum):
     AnyFlavour = 'any_flavour'
     AnyReleaseType = 'any_release_type'
     VersionEq = 'version_eq'
```

### Comparing `instawow-4.0.0/src/instawow/github_auth.py` & `instawow-4.1.0/src/instawow/github_auth.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/manager_ctx.py` & `instawow-4.1.0/src/instawow/manager_ctx.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,28 @@
     Sequence,
 )
 from contextlib import AbstractAsyncContextManager
 from functools import cached_property
 from itertools import chain
 from typing import TypeAlias
 
+from typing_extensions import Self
+
 from . import http, pkg_db
 from ._sources.cfcore import CfCoreResolver
 from ._sources.github import GithubResolver
 from ._sources.instawow import InstawowResolver
 from ._sources.tukui import TukuiResolver
 from ._sources.wago import WagoResolver
 from ._sources.wowi import WowiResolver
+from ._utils.iteration import WeakValueDefaultDictionary
 from .config import ProfileConfig
 from .pkg_archives import ArchiveOpener, open_zip_archive
 from .plugins import get_plugin_resolvers
 from .resolvers import Resolver
-from .utils import WeakValueDefaultDictionary
 
 
 class _DummyLock:
     async def __aenter__(self):
         pass
 
     async def __aexit__(self, *args: object):
@@ -117,17 +119,21 @@
                 builtin_resolver_classes.remove(resolver)
 
         resolver_classes = chain(
             (r for g in get_plugin_resolvers() for r in g), builtin_resolver_classes
         )
         self.resolvers: _Resolvers = _Resolvers((r.metadata.id, r(self)) for r in resolver_classes)
 
-    @cached_property
-    def database(self) -> pkg_db.sa.Engine:
-        return pkg_db.prepare_database(self.config.db_uri)
+        self.database: pkg_db.DatabaseHandle = pkg_db.DatabaseHandle(self.config.db_file)
+
+    def __enter__(self) -> Self:
+        return self
+
+    def __exit__(self, *args: object) -> None:
+        self.database.close()
 
     @property
     def locks(self) -> _Locks:
         "Lock factory used to synchronise async operations."
         return _locks.get()
 
     @property
```

### Comparing `instawow-4.0.0/src/instawow/pkg_archives.py` & `instawow-4.1.0/src/instawow/pkg_archives.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/pkg_management.py` & `instawow-4.1.0/src/instawow/pkg_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,49 +4,43 @@
     Awaitable,
     Callable,
     Collection,
     Iterable,
     Mapping,
     Sequence,
 )
-from contextlib import asynccontextmanager
+from contextlib import asynccontextmanager, nullcontext
 from functools import wraps
-from itertools import filterfalse, product, repeat, starmap
+from itertools import compress, filterfalse, product, repeat, starmap
 from pathlib import Path
 from shutil import move
 from tempfile import NamedTemporaryFile
 from typing import Concatenate, Literal, TypeVar
 
 import attrs
-from loguru import logger
 from typing_extensions import Never, ParamSpec
 from yarl import URL
 
 from . import pkg_db, pkg_models
 from . import results as R
+from ._logging import logger
+from ._utils.aio import gather, run_in_thread
+from ._utils.file import trash
+from ._utils.iteration import bucketise, chain_dict, uniq
+from ._utils.perf import time_op
+from ._utils.text import shasum
+from ._utils.web import file_uri_to_path, is_file_uri
 from .definitions import Defn, Strategy
 from .http import CACHE_INDEFINITELY, ProgressCtx
 from .manager_ctx import ManagerCtx
 from .resolvers import HeadersIntent
-from .utils import (
-    bucketise,
-    chain_dict,
-    file_uri_to_path,
-    gather,
-    is_file_uri,
-    run_in_thread,
-    shasum,
-    time_op,
-    trash,
-    uniq,
-)
 
-_P = ParamSpec('_P')
 _T = TypeVar('_T')
 _TPkgManager = TypeVar('_TPkgManager', bound='PkgManager')
+_P = ParamSpec('_P')
 
 _AsyncNamedTemporaryFile = run_in_thread(NamedTemporaryFile)
 _move_async = run_in_thread(move)
 
 _MUTATE_PKGS_LOCK = '_MUTATE_PKGS_'
 _DOWNLOAD_PKG_LOCK = '_DOWNLOAD_PKG_'
 
@@ -112,51 +106,147 @@
 
         return await _move_async(
             temp_path,
             ctx.config.global_config.install_cache_dir / shasum(pkg.download_url),
         )
 
 
-def _insert_db_pkg(pkg: pkg_models.Pkg, transaction: pkg_db.sa.Connection):
-    values = attrs.asdict(pkg)
-    source_and_id = {'pkg_source': values['source'], 'pkg_id': values['id']}
+def _insert_db_pkg(pkg: pkg_models.Pkg, transaction: pkg_db.Connection):
+    pkg_values = pkg_models.make_db_converter().unstructure(pkg)
 
-    transaction.execute(pkg_db.sa.insert(pkg_db.pkg), [values])
     transaction.execute(
-        pkg_db.sa.insert(pkg_db.pkg_folder), [{**f, **source_and_id} for f in values['folders']]
+        """
+        INSERT INTO pkg (
+            source,
+            id,
+            slug,
+            name,
+            description,
+            url,
+            download_url,
+            date_published,
+            version,
+            changelog_url
+        )
+        VALUES (
+            :source,
+            :id,
+            :slug,
+            :name,
+            :description,
+            :url,
+            :download_url,
+            :date_published,
+            :version,
+            :changelog_url
+        )
+        """,
+        pkg_values,
     )
     transaction.execute(
-        pkg_db.sa.insert(pkg_db.pkg_options), [{**values['options'], **source_and_id}]
+        """
+        INSERT INTO pkg_options (
+            any_flavour,
+            any_release_type,
+            version_eq,
+            pkg_source,
+            pkg_id
+        )
+        VALUES (
+            :any_flavour,
+            :any_release_type,
+            :version_eq,
+            :pkg_source,
+            :pkg_id
+        )
+        """,
+        pkg_values['options'] | {'pkg_source': pkg_values['source'], 'pkg_id': pkg_values['id']},
     )
-    if values['deps']:
-        transaction.execute(
-            pkg_db.sa.insert(pkg_db.pkg_dep), [{**d, **source_and_id} for d in values['deps']]
+    transaction.executemany(
+        """
+        INSERT INTO pkg_folder (
+            name,
+            pkg_source,
+            pkg_id
+        )
+        VALUES (
+            :name,
+            :pkg_source,
+            :pkg_id
+        )
+        """,
+        [
+            f | {'pkg_source': pkg_values['source'], 'pkg_id': pkg_values['id']}
+            for f in pkg_values['folders']
+        ],
+    )
+    if pkg_values['deps']:
+        transaction.executemany(
+            """
+            INSERT INTO pkg_dep (
+                id,
+                pkg_source,
+                pkg_id
+            )
+            VALUES (
+                :id,
+                :pkg_source,
+                :pkg_id
+            )
+            """,
+            [
+                f | {'pkg_source': pkg_values['source'], 'pkg_id': pkg_values['id']}
+                for f in pkg_values['deps']
+            ],
         )
     transaction.execute(
-        pkg_db.sa.insert(pkg_db.pkg_version_log).prefix_with('OR IGNORE'),
-        [{'version': values['version'], **source_and_id}],
+        """
+        INSERT OR IGNORE INTO pkg_version_log (
+            version,
+            pkg_source,
+            pkg_id
+        )
+        VALUES (
+            :version,
+            :pkg_source,
+            :pkg_id
+        )
+        """,
+        {
+            'version': pkg_values['version'],
+            'pkg_source': pkg_values['source'],
+            'pkg_id': pkg_values['id'],
+        },
     )
 
 
-def _delete_db_pkg(pkg: pkg_models.Pkg, transaction: pkg_db.sa.Connection):
-    transaction.execute(pkg_db.sa.delete(pkg_db.pkg).filter_by(source=pkg.source, id=pkg.id))
+def _delete_db_pkg(pkg: pkg_models.Pkg, transaction: pkg_db.Connection):
+    transaction.execute(
+        'DELETE FROM pkg WHERE source = :source AND id = :id',
+        pkg_models.make_db_converter().unstructure(pkg),
+    )
 
 
 @run_in_thread
 def _install_pkg(
     ctx: ManagerCtx, pkg: pkg_models.Pkg, archive: Path, *, replace_folders: bool
 ) -> R.PkgInstalled:
-    with ctx.resolvers.archive_opener_dict[pkg.source](archive) as (top_level_folders, extract):
-        with ctx.database.connect() as connection:
-            installed_conflicts = connection.execute(
-                pkg_db.sa.select(pkg_db.pkg)
-                .distinct()
-                .join(pkg_db.pkg_folder)
-                .where(pkg_db.pkg_folder.c.name.in_(top_level_folders))
-            ).all()
+    with (
+        ctx.resolvers.archive_opener_dict[pkg.source](archive) as (top_level_folders, extract),
+        ctx.database.connect() as connection,
+    ):
+        installed_conflicts = connection.execute(
+            f"""
+            SELECT DISTINCT pkg.*
+            FROM pkg
+            JOIN pkg_folder ON pkg_folder.pkg_source = pkg.source AND pkg_folder.pkg_id = pkg.id
+            WHERE pkg_folder.name IN ({', '.join(('?',) * len(top_level_folders))})
+            """,
+            tuple(top_level_folders),
+        ).fetchall()
         if installed_conflicts:
             raise R.PkgConflictsWithInstalled(installed_conflicts)
 
         if replace_folders:
             trash(
                 (ctx.config.addon_dir / f for f in top_level_folders),
                 dest=ctx.config.global_config.temp_dir,
@@ -167,42 +257,41 @@
                 f.name for f in ctx.config.addon_dir.iterdir()
             }
             if unreconciled_conflicts:
                 raise R.PkgConflictsWithUnreconciled(unreconciled_conflicts)
 
         extract(ctx.config.addon_dir)
 
-    pkg = attrs.evolve(
-        pkg, folders=[pkg_models.PkgFolder(name=f) for f in sorted(top_level_folders)]
-    )
-    with ctx.database.begin() as transaction:
-        _insert_db_pkg(pkg, transaction)
+        pkg = attrs.evolve(
+            pkg, folders=[pkg_models.PkgFolder(name=f) for f in sorted(top_level_folders)]
+        )
+        with ctx.database.transact(connection) as transaction:
+            _insert_db_pkg(pkg, transaction)
 
     return R.PkgInstalled(pkg)
 
 
 @run_in_thread
 def _update_pkg(
     ctx: ManagerCtx, old_pkg: pkg_models.Pkg, new_pkg: pkg_models.Pkg, archive: Path
 ) -> R.PkgUpdated:
-    with ctx.resolvers.archive_opener_dict[new_pkg.source](archive) as (
-        top_level_folders,
-        extract,
+    with (
+        ctx.resolvers.archive_opener_dict[new_pkg.source](archive) as (top_level_folders, extract),
+        ctx.database.connect() as connection,
     ):
-        with ctx.database.connect() as connection:
-            installed_conflicts = connection.execute(
-                pkg_db.sa.select(pkg_db.pkg)
-                .distinct()
-                .join(pkg_db.pkg_folder)
-                .where(
-                    pkg_db.pkg_folder.c.pkg_source != new_pkg.source,
-                    pkg_db.pkg_folder.c.pkg_id != new_pkg.id,
-                    pkg_db.pkg_folder.c.name.in_(top_level_folders),
-                )
-            ).all()
+        installed_conflicts = connection.execute(
+            f"""
+            SELECT DISTINCT pkg.*
+            FROM pkg
+            JOIN pkg_folder ON pkg_folder.pkg_source = pkg.source AND pkg_folder.pkg_id = pkg.id
+            WHERE (pkg_folder.pkg_source != ? AND pkg_folder.pkg_id != ?)
+                AND (pkg_folder.name IN ({', '.join(('?',) * len(top_level_folders))}))
+            """,
+            (new_pkg.source, new_pkg.id, *top_level_folders),
+        ).fetchall()
         if installed_conflicts:
             raise R.PkgConflictsWithInstalled(installed_conflicts)
 
         unreconciled_conflicts = top_level_folders - {f.name for f in old_pkg.folders} & {
             f.name for f in ctx.config.addon_dir.iterdir()
         }
         if unreconciled_conflicts:
@@ -211,34 +300,34 @@
         trash(
             (ctx.config.addon_dir / f.name for f in old_pkg.folders),
             dest=ctx.config.global_config.temp_dir,
             missing_ok=True,
         )
         extract(ctx.config.addon_dir)
 
-    new_pkg = attrs.evolve(
-        new_pkg, folders=[pkg_models.PkgFolder(name=f) for f in sorted(top_level_folders)]
-    )
-    with ctx.database.begin() as transaction:
-        _delete_db_pkg(old_pkg, transaction)
-        _insert_db_pkg(new_pkg, transaction)
+        new_pkg = attrs.evolve(
+            new_pkg, folders=[pkg_models.PkgFolder(name=f) for f in sorted(top_level_folders)]
+        )
+        with ctx.database.transact(connection) as transaction:
+            _delete_db_pkg(old_pkg, transaction)
+            _insert_db_pkg(new_pkg, transaction)
 
     return R.PkgUpdated(old_pkg, new_pkg)
 
 
 @run_in_thread
 def _remove_pkg(ctx: ManagerCtx, pkg: pkg_models.Pkg, *, keep_folders: bool) -> R.PkgRemoved:
     if not keep_folders:
         trash(
             (ctx.config.addon_dir / f.name for f in pkg.folders),
             dest=ctx.config.global_config.temp_dir,
             missing_ok=True,
         )
 
-    with ctx.database.begin() as transaction:
+    with ctx.database.connect() as connection, ctx.database.transact(connection) as transaction:
         _delete_db_pkg(pkg, transaction)
 
     return R.PkgRemoved(pkg)
 
 
 @run_in_thread
 def _check_installed_pkg_integrity(ctx: ManagerCtx, pkg: pkg_models.Pkg):
@@ -280,95 +369,137 @@
                 (r.metadata.id, a)
                 for r in self.ctx.resolvers.values()
                 if (a := r.get_alias_from_url(url))
             ),
             None,
         )
 
-    def check_pkg_exists(self, defn: Defn) -> bool:
-        "Check that a package exists in the database."
-        with self.ctx.database.connect() as connection:
-            return (
-                connection.execute(
-                    pkg_db.sa.select(pkg_db.sa.text('1'))
-                    .select_from(pkg_db.pkg)
-                    .where(
-                        pkg_db.pkg.c.source == defn.source,
-                        (pkg_db.pkg.c.id == defn.alias)
-                        | (pkg_db.pkg.c.id == defn.id)
-                        | (
-                            pkg_db.sa.func.lower(pkg_db.pkg.c.slug)
-                            == pkg_db.sa.func.lower(defn.alias)
-                        ),
+    def check_pkgs_exist(
+        self,
+        defns: Sequence[Defn],
+        *,
+        connection: pkg_db.Connection | None = None,
+    ) -> list[bool]:
+        "Check that packages exist in the database."
+        if not defns:
+            return []
+
+        with (
+            nullcontext(connection) if connection else self.ctx.database.connect() as connection,
+            self.ctx.database.use_tuple_factory(connection) as cursor,
+        ):
+            return [
+                e
+                for (e,) in cursor.execute(
+                    f"""
+                    WITH defn (source, alias, id)
+                    AS (
+                        VALUES {", ".join(("(?, ?, ?)",) * len(defns))}
                     )
-                ).scalar()
-                == 1
-            )
+                    SELECT NOT EXISTS (
+                        SELECT 1
+                        FROM pkg
+                        WHERE pkg.source = defn.source AND (
+                            pkg.id = defn.alias OR pkg.id = defn.id OR lower(pkg.slug) = lower(defn.alias)
+                        )
+                    )
+                    FROM defn
+                    """,
+                    tuple(i for d in defns for i in (d.source, d.alias, d.id)),
+                ).fetchall()
+            ]
 
-    def get_pkg(self, defn: Defn, partial_match: bool = False) -> pkg_models.Pkg | None:
-        "Retrieve a package from the database."
-        with self.ctx.database.connect() as connection:
-            maybe_row_mapping = (
-                connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg).where(
-                        pkg_db.pkg.c.source == defn.source,
-                        (pkg_db.pkg.c.id == defn.alias)
-                        | (pkg_db.pkg.c.id == defn.id)
-                        | (
-                            pkg_db.sa.func.lower(pkg_db.pkg.c.slug)
-                            == pkg_db.sa.func.lower(defn.alias)
-                        ),
+    def get_pkgs(
+        self,
+        defns: Sequence[Defn] | Literal['all'],
+        *,
+        connection: pkg_db.Connection | None = None,
+    ) -> list[pkg_models.Pkg | None]:
+        if defns != 'all' and not defns:
+            return []
+
+        with nullcontext(connection) if connection else self.ctx.database.connect() as connection:
+            if defns == 'all':
+                pkgs = connection.execute(
+                    """
+                    SELECT * FROM pkg
+                    """,
+                ).fetchall()
+            else:
+                pkgs = connection.execute(
+                    f"""
+                    WITH defn (source, alias, id)
+                    AS (
+                        VALUES {", ".join(("(?, ?, ?)",) * len(defns))}
                     )
-                )
-                .mappings()
-                .one_or_none()
-            )
-            if maybe_row_mapping is None and partial_match:
-                maybe_row_mapping = (
-                    connection.execute(
-                        pkg_db.sa.select(pkg_db.pkg)
-                        .where(pkg_db.pkg.c.slug.contains(defn.alias))
-                        .order_by(pkg_db.pkg.c.name)
+                    SELECT pkg.*
+                    FROM defn
+                    LEFT JOIN pkg ON pkg.source = defn.source AND (
+                        pkg.id = defn.alias OR pkg.id = defn.id OR lower(pkg.slug) = lower(defn.alias)
                     )
-                    .mappings()
-                    .first()
-                )
-            if maybe_row_mapping is not None:
-                return self.build_pkg_from_row_mapping(connection, maybe_row_mapping)
+                    """,
+                    tuple(i for d in defns for i in (d.source, d.alias, d.id)),
+                ).fetchall()
+
+            return [
+                self.build_pkg_from_row_mapping(connection, m) if m['source'] else None
+                for m in pkgs
+            ]
+
+    def get_pkg(
+        self,
+        defn: Defn,
+        *,
+        connection: pkg_db.Connection | None = None,
+    ) -> pkg_models.Pkg | None:
+        "Retrieve a package from the database."
+        (pkg,) = self.get_pkgs([defn], connection=connection)
+        return pkg
 
     def build_pkg_from_row_mapping(
-        self, connection: pkg_db.sa.Connection, row_mapping: pkg_db.sa.RowMapping
+        self, connection: pkg_db.Connection, row_mapping: pkg_db.Row
     ) -> pkg_models.Pkg:
-        source_and_id = {'pkg_source': row_mapping['source'], 'pkg_id': row_mapping['id']}
-        return pkg_models.make_db_pkg_converter().structure(
+        fk = {'pkg_source': row_mapping['source'], 'pkg_id': row_mapping['id']}
+        return pkg_models.make_db_converter().structure(
             {
                 **row_mapping,
                 'options': connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg_options).filter_by(**source_and_id)
-                )
-                .mappings()
-                .one(),
+                    """
+                    SELECT any_flavour, any_release_type, version_eq
+                    FROM pkg_options
+                    WHERE pkg_source = :pkg_source AND pkg_id = :pkg_id
+                    """,
+                    fk,
+                ).fetchone(),
                 'folders': connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg_folder.c.name).filter_by(**source_and_id)
-                )
-                .mappings()
-                .all(),
+                    """
+                    SELECT name
+                    FROM pkg_folder
+                    WHERE pkg_source = :pkg_source AND pkg_id = :pkg_id
+                    """,
+                    fk,
+                ).fetchall(),
                 'deps': connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg_dep.c.id).filter_by(**source_and_id)
-                )
-                .mappings()
-                .all(),
+                    """
+                    SELECT id
+                    FROM pkg_dep
+                    WHERE pkg_source = :pkg_source AND pkg_id = :pkg_id
+                    """,
+                    fk,
+                ).fetchall(),
                 'logged_versions': connection.execute(
-                    pkg_db.sa.select(pkg_db.pkg_version_log)
-                    .filter_by(**source_and_id)
-                    .order_by(pkg_db.pkg_version_log.c.install_time.desc())
-                    .limit(10)
-                )
-                .mappings()
-                .all(),
+                    """
+                    SELECT version, install_time
+                    FROM pkg_version_log
+                    WHERE pkg_source = :pkg_source AND pkg_id = :pkg_id
+                    ORDER BY install_time DESC
+                    LIMIT 10
+                    """,
+                    fk,
+                ).fetchall(),
             },
             pkg_models.Pkg,
         )
 
     async def find_equivalent_pkg_defns(
         self, pkgs: Collection[pkg_models.Pkg]
     ) -> dict[pkg_models.Pkg, list[Defn]]:
@@ -478,19 +609,16 @@
     ) -> Mapping[Defn, R.AnyResult[pkg_models.Pkg]]:
         "Resolve definitions into packages."
         if not defns:
             return {}
 
         defns_by_source = bucketise(defns, key=lambda v: v.source)
         results = await gather(
-            (
-                self.ctx.resolvers.get(s, _DummyResolver).resolve(b)
-                for s, b in defns_by_source.items()
-            ),
-            R.resultify_async_exc,
+            R.resultify_async_exc(self.ctx.resolvers.get(s, _DummyResolver).resolve(b))
+            for s, b in defns_by_source.items()
         )
         results_by_defn = chain_dict(
             defns,
             R.ManagerError(),
             *(
                 r.items() if isinstance(r, dict) else zip(d, repeat(r))
                 for d, r in zip(defns_by_source.values(), results)
@@ -508,29 +636,31 @@
     async def install(
         self, defns: Sequence[Defn], *, replace_folders: bool, dry_run: bool = False
     ) -> Mapping[Defn, R.AnyResult[R.PkgInstalled]]:
         "Install packages from a definition list."
 
         # We'll weed out installed deps from the results after resolving -
         # doing it this way isn't particularly efficient but avoids having to
-        # deal with local state in ``resolve``
+        # deal with local state in ``resolve``.
         resolve_results = await self.resolve(
-            [d for d in defns if not self.check_pkg_exists(d)], with_deps=True
+            list(compress(defns, self.check_pkgs_exist(defns))), with_deps=True
         )
         pkgs, resolve_errors = bucketise_results(resolve_results.items())
-        new_pkgs = {d: p for d, p in pkgs.items() if not self.check_pkg_exists(p.to_defn())}
+        new_pkgs = dict(
+            compress(pkgs.items(), self.check_pkgs_exist([p.to_defn() for p in pkgs.values()]))
+        )
 
         results = dict.fromkeys(defns, R.PkgAlreadyInstalled()) | resolve_errors
 
         if dry_run:
             return results | {d: R.PkgInstalled(p, dry_run=True) for d, p in new_pkgs.items()}
 
         download_results = await gather(
-            (_download_pkg_archive(self.ctx, d, r) for d, r in new_pkgs.items()),
-            R.resultify_async_exc,
+            R.resultify_async_exc(_download_pkg_archive(self.ctx, d, r))
+            for d, r in new_pkgs.items()
         )
         archive_paths, download_errors = bucketise_results(zip(new_pkgs, download_results))
 
         return (
             results
             | download_errors
             | {
@@ -539,27 +669,36 @@
                 )
                 for d, a in archive_paths.items()
             }
         )
 
     @_with_lock(_MUTATE_PKGS_LOCK)
     async def update(
-        self, defns: Sequence[Defn], *, dry_run: bool = False
+        self, defns: Sequence[Defn] | Literal['all'], *, dry_run: bool = False
     ) -> Mapping[Defn, R.AnyResult[R.PkgInstalled | R.PkgUpdated]]:
-        """Update installed packages from a definition list."""
-        defns_to_pkgs = {d: p for d in defns for p in (self.get_pkg(d),) if p}
+        "Update installed packages from a definition list."
+
+        if defns == 'all':
+            defns_to_pkgs = {p.to_defn(): p for p in self.get_pkgs(defns) if p}
+            defns = list(defns_to_pkgs)
+
+            resolve_defns = {d: d for d in defns_to_pkgs}
+
+        else:
+            defns_to_pkgs = {d: p for d, p in zip(defns, self.get_pkgs(defns)) if p}
+
+            resolve_defns = {
+                # Attach the source ID to each ``Defn`` from the
+                # corresponding installed package.  Using the ID has the benefit
+                # of resolving installed-but-renamed packages - the slug is
+                # transient but the ID isn't
+                attrs.evolve(d, id=p.id) if d.strategies.initialised else p.to_defn(): d
+                for d, p in defns_to_pkgs.items()
+            }
 
-        resolve_defns = {
-            # Attach the source ID to each ``Defn`` from the
-            # corresponding installed package.  Using the ID has the benefit
-            # of resolving installed-but-renamed packages - the slug is
-            # transient but the ID isn't
-            attrs.evolve(d, id=p.id) if d.strategies.initialised else p.to_defn(): d
-            for d, p in defns_to_pkgs.items()
-        }
         resolve_results = await self.resolve(resolve_defns, with_deps=True)
         pkgs, resolve_errors = bucketise_results(
             # Discard the reconstructed ``Defn``s
             (resolve_defns.get(d) or d, r)
             for d, r in resolve_results.items()
         )
 
@@ -587,16 +726,16 @@
         if dry_run:
             return results | {
                 d: R.PkgUpdated(o, n, dry_run=True) if o else R.PkgInstalled(n, dry_run=True)
                 for d, (o, n) in updatables.items()
             }
 
         download_results = await gather(
-            (_download_pkg_archive(self.ctx, d, n) for d, (_, n) in updatables.items()),
-            R.resultify_async_exc,
+            R.resultify_async_exc(_download_pkg_archive(self.ctx, d, n))
+            for d, (_, n) in updatables.items()
         )
         archive_paths, download_errors = bucketise_results(zip(updatables, download_results))
 
         return (
             results
             | download_errors
             | {
@@ -617,51 +756,60 @@
         "Remove packages by their definition."
         return {
             d: (
                 await R.resultify_async_exc(_remove_pkg(self.ctx, p, keep_folders=keep_folders))
                 if p
                 else R.PkgNotInstalled()
             )
-            for d in defns
-            for p in (self.get_pkg(d),)
+            for d, p in zip(defns, self.get_pkgs(defns))
         }
 
     @_with_lock(_MUTATE_PKGS_LOCK)
     async def pin(self, defns: Sequence[Defn]) -> Mapping[Defn, R.AnyResult[R.PkgInstalled]]:
         """Pin and unpin installed packages.
 
         instawow does not have true pinning.  This flips ``Strategy.VersionEq``
         on for installed packages from sources that support it.
         The net effect is the same as if the package
         had been reinstalled with the ``VersionEq`` strategy.
         """
 
-        @run_in_thread
-        def pin(defn: Defn) -> R.PkgInstalled:
+        async def pin(defn: Defn, pkg: pkg_models.Pkg | None) -> R.PkgInstalled:
             resolver = self.ctx.resolvers.get(defn.source)
             if resolver is None:
                 raise R.PkgSourceInvalid
-
-            if Strategy.VersionEq not in resolver.metadata.strategies:
+            elif Strategy.VersionEq not in resolver.metadata.strategies:
                 raise R.PkgStrategiesUnsupported({Strategy.VersionEq})
 
-            pkg = self.get_pkg(defn)
             if not pkg:
                 raise R.PkgNotInstalled
 
             version = defn.strategies.version_eq
             if version and pkg.version != version:
                 R.PkgFilesNotMatching(defn.strategies)
 
-            with self.ctx.database.begin() as transaction:
+            version_eq = version is not None
+
+            with (
+                self.ctx.database.connect() as connection,
+                self.ctx.database.transact(connection) as transaction,
+            ):
                 transaction.execute(
-                    pkg_db.sa.update(pkg_db.pkg_options)
-                    .filter_by(pkg_source=pkg.source, pkg_id=pkg.id)
-                    .values(version_eq=version is not None)
+                    """
+                    UPDATE pkg_options
+                    SET version_eq = :version_eq
+                    WHERE pkg_source = :pkg_source AND pkg_id = :pkg_id
+                    """,
+                    {
+                        'pkg_source': pkg.source,
+                        'pkg_id': pkg.id,
+                        'version_eq': version_eq,
+                    },
                 )
 
-            new_pkg = attrs.evolve(
-                pkg, options=attrs.evolve(pkg.options, version_eq=version is not None)
+            return R.PkgInstalled(
+                attrs.evolve(pkg, options=attrs.evolve(pkg.options, version_eq=version_eq)),
             )
-            return R.PkgInstalled(new_pkg)
 
-        return {d: await R.resultify_async_exc(pin(d)) for d in defns}
+        return {
+            d: await R.resultify_async_exc(pin(d, p)) for d, p in zip(defns, self.get_pkgs(defns))
+        }
```

### Comparing `instawow-4.0.0/src/instawow/pkg_models.py` & `instawow-4.1.0/src/instawow/pkg_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,30 @@
 
 import cattrs
 from attrs import field, frozen
 
 from .definitions import Defn, StrategyValues
 
 
+def _structure_datetime(value: str, value_type: type):
+    return dt.datetime.fromisoformat(value).replace(tzinfo=dt.timezone.utc)
+
+
+def _unstructure_datetime(value: dt.datetime):
+    if not value.tzinfo:
+        raise TypeError('`tzinfo` must be set')
+
+    return value.astimezone(dt.timezone.utc).replace(tzinfo=None).isoformat(' ')
+
+
 @lru_cache(1)
-def make_db_pkg_converter():
+def make_db_converter():
     converter = cattrs.Converter()
-    converter.register_structure_hook(dt.datetime, lambda d, _: d)
+    converter.register_structure_hook(dt.datetime, _structure_datetime)
+    converter.register_unstructure_hook(dt.datetime, _unstructure_datetime)
     return converter
 
 
 @frozen(kw_only=True)
 class PkgOptions:
     any_flavour: bool
     any_release_type: bool
```

### Comparing `instawow-4.0.0/src/instawow/plugins.py` & `instawow-4.1.0/src/instawow/plugins.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow/resolvers.py` & `instawow-4.1.0/src/instawow/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 import attrs
 from typing_extensions import NotRequired
 from yarl import URL
 
 from . import http, manager_ctx, matchers, pkg_archives, pkg_models
 from . import results as R
+from ._utils.aio import gather, run_in_thread
+from ._utils.web import file_uri_to_path
 from .catalogue.cataloguer import CatalogueEntry
 from .config import GlobalConfig
 from .definitions import Defn, SourceMetadata
-from .utils import file_uri_to_path, gather, run_in_thread
 
 
 class FolderHashCandidate(Protocol):  # pragma: no cover
     @property
     def name(self) -> str: ...
 
     def hash_contents(self, __method: matchers.AddonHashMethod) -> str: ...
@@ -126,15 +127,15 @@
         self, intent: HeadersIntent | None = None
     ) -> dict[str, str] | None:
         return None
 
     async def resolve(
         self, defns: Sequence[Defn]
     ) -> dict[Defn, pkg_models.Pkg | R.ManagerError | R.InternalError]:
-        results = await gather((self.resolve_one(d, None) for d in defns), R.resultify_async_exc)
+        results = await gather(R.resultify_async_exc(self.resolve_one(d, None)) for d in defns)
         return dict(zip(defns, results))
 
     async def resolve_one(self, defn: Defn, metadata: Any) -> pkg_models.Pkg:
         extraneous_strategies = defn.strategies.filled_strategies.keys() - self.metadata.strategies
         if extraneous_strategies:
             raise R.PkgStrategiesUnsupported(extraneous_strategies)
```

### Comparing `instawow-4.0.0/src/instawow/results.py` & `instawow-4.1.0/src/instawow/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-from collections.abc import Awaitable, Collection, Set
+from collections.abc import Awaitable, Collection, Mapping, Set
 from typing import Any, Final, Protocol, TypeAlias, TypeVar
 
 import attrs
-from loguru import logger
 
 from . import pkg_models
+from ._logging import logger
 from .definitions import Strategy, StrategyValues
 
 _T = TypeVar('_T')
 
 AnyResult: TypeAlias = '_T | ManagerError | InternalError'
 
 
@@ -85,24 +85,24 @@
 class PkgAlreadyInstalled(ManagerError):
     @property
     def message(self) -> str:
         return 'package already installed'
 
 
 class PkgConflictsWithInstalled(ManagerError):
-    def __init__(self, conflicting_pkgs: Collection[Any]) -> None:
+    def __init__(self, conflicting_pkgs: Collection[Mapping[str, Any]]) -> None:
         super().__init__()
         self.conflicting_pkgs = conflicting_pkgs
 
     @property
     def message(self) -> str:
         return (
             'package folders conflict with installed package'
             + ('s ' if len(self.conflicting_pkgs) > 1 else ' ')
-            + ', '.join(f'{c.name} ({c.source}:{c.id})' for c in self.conflicting_pkgs)
+            + ', '.join(f'{c["name"]} ({c["source"]}:{c["id"]})' for c in self.conflicting_pkgs)
         )
 
 
 class PkgConflictsWithUnreconciled(ManagerError):
     def __init__(self, folders: Set[str]) -> None:
         super().__init__()
         self.folders = folders
```

### Comparing `instawow-4.0.0/src/instawow/wow_installations.py` & `instawow-4.1.0/src/instawow/wow_installations.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from enum import Enum
 from functools import cache
 from pathlib import Path
 from typing import Protocol, TypedDict
 
 from typing_extensions import Self, TypeVar
 
-from .utils import StrEnum, fill
+from ._utils.compat import StrEnum
+from ._utils.iteration import fill
 
 _TEnum = TypeVar('_TEnum', bound=Enum, infer_variance=True)
 
 
 class _FlavourKeyedEnumMeta(type(Protocol)):  # pragma: no cover
     def __getitem__(self: type[_FlavourKeyedEnum[_TEnum]], __key: str) -> _TEnum: ...
 
@@ -50,14 +51,23 @@
     @classmethod
     def from_flavour_keyed_enum(cls, flavour_keyed_enum: Enum) -> Self:
         return cls[flavour_keyed_enum.name]
 
     def to_flavour_keyed_enum(self, flavour_keyed_enum: type[_FlavourKeyedEnum[_TEnum]]) -> _TEnum:
         return flavour_keyed_enum[self.name]
 
+    def get_flavour_groups(self, affine: bool) -> list[tuple[Flavour, ...] | None]:
+        match (self, affine):
+            case (self.CataclysmClassic, True):
+                return [(self, self.Classic), None]
+            case (_, True):
+                return [(self,), None]
+            case _:
+                return [(self,)]
+
 
 class FlavourVersionRange(Enum):
     Retail = (
         range(1_00_00, 1_13_00),
         range(2_00_00, 2_05_00),
         range(3_00_00, 3_04_00),
         range(4_00_00, 4_04_00),
@@ -122,15 +132,15 @@
     # },
     '_classic_': {
         'code': 'wow_classic',
         'flavour': Flavour.Classic,
     },
     '_classic_ptr_': {
         'code': 'wow_classic_ptr',
-        'flavour': Flavour.Classic,
+        'flavour': Flavour.CataclysmClassic,
     },
     '_classic_beta_': {
         'code': 'wow_classic_beta',
         'flavour': Flavour.CataclysmClassic,
     },
 }
```

### Comparing `instawow-4.0.0/src/instawow/_sources/cfcore.py` & `instawow-4.1.0/src/instawow/_sources/cfcore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
 import asyncio
-from collections.abc import AsyncIterator, Callable, Generator, Sequence
+from collections.abc import AsyncIterator, Callable, Iterator, Sequence
 from datetime import timedelta
 from enum import IntEnum
 from functools import partial
 from typing import Generic, TypeVar
 
 import iso8601
-from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import pkg_models
 from .. import results as R
+from .._logging import logger
+from .._utils.aio import gather
+from .._utils.iteration import uniq
 from ..catalogue.cataloguer import CatalogueEntry
 from ..config import GlobalConfig
 from ..definitions import ChangelogFormat, Defn, SourceMetadata, Strategy
 from ..http import CACHE_INDEFINITELY, ClientSessionType, GenericDownloadTraceRequestCtx
 from ..resolvers import BaseResolver, HeadersIntent, PkgCandidate
-from ..utils import gather, uniq
 from ..wow_installations import Flavour
 
 _T = TypeVar('_T')
 
 
 _CF_WOW_GAME_ID = 1
 
@@ -248,16 +249,16 @@
 
 class CfCoreResolver(BaseResolver):
     metadata = SourceMetadata(
         id='curse',
         name='CFCore',
         strategies=frozenset(
             {
-                Strategy.AnyReleaseType,
                 Strategy.AnyFlavour,
+                Strategy.AnyReleaseType,
                 Strategy.VersionEq,
             }
         ),
         changelog_format=ChangelogFormat.Html,
         addon_toc_key='X-Curse-Project-ID',
     )
     requires_access_token = 'cfcore'
@@ -300,16 +301,16 @@
             raise_for_status=True,
         ) as response:
             response_json: _CfCoreUnpaginatedModsResponse = await response.json()
 
         addons_by_id = {str(r['id']): r for r in response_json['data']}
 
         results = await gather(
-            (self.resolve_one(d, addons_by_id.get(d.id or d.alias)) for d in defns),
-            R.resultify_async_exc,
+            R.resultify_async_exc(self.resolve_one(d, addons_by_id.get(d.id or d.alias)))
+            for d in defns
         )
         return dict(zip(defns, results))
 
     async def _resolve_one(self, defn: Defn, metadata: _CfCoreMod | None) -> PkgCandidate:
         if metadata is None:
             if defn.alias.isdigit():
                 async with self._manager_ctx.web_client.get(
@@ -337,20 +338,22 @@
                     mod_response_json: _CfCoreModsResponse = await mod_response.json()
                     if not mod_response_json['data']:
                         raise R.PkgNonexistent
 
                     [metadata] = mod_response_json['data']
 
         if defn.strategies.version_eq:
-            game_version_type_id = self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
-                _CfCoreSortableGameVersionTypeId
-            )
-            files_url = (self.__mod_api_url / str(metadata['id']) / 'files').with_query(
-                gameVersionTypeId=game_version_type_id, pageSize=999
-            )
+            files_url = self.__mod_api_url / str(metadata['id']) / 'files'
+            if not defn.strategies.any_flavour:
+                files_url = files_url.with_query(
+                    game_version_type_id=self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
+                        _CfCoreSortableGameVersionTypeId
+                    )
+                )
+
             async with self._manager_ctx.web_client.get(
                 files_url,
                 expire_after=timedelta(hours=1),
                 headers=await self.make_request_headers(),
                 raise_for_status=True,
                 trace_request_ctx=GenericDownloadTraceRequestCtx(
                     report_progress='generic', label=f'Fetching metadata from {self.metadata.name}'
@@ -362,47 +365,59 @@
 
         else:
             files = metadata['latestFiles']
 
         if not files:
             raise R.PkgFilesMissing
 
-        def make_filter_fns() -> Generator[Callable[[_CfCoreFile], bool], None, None]:
-            yield lambda f: not f.get('exposeAsAlternative', False)
+        desired_flavour_groups = self._manager_ctx.config.game_flavour.get_flavour_groups(
+            bool(defn.strategies.any_flavour)
+        )
+        for desired_flavours in desired_flavour_groups:
 
-            if not defn.strategies.any_flavour:
-                type_id = self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
-                    _CfCoreSortableGameVersionTypeId
+            def make_filter_fns(
+                desired_flavours: Sequence[Flavour] | None,
+            ) -> Iterator[Callable[[_CfCoreFile], bool]]:
+                yield lambda f: not f.get('exposeAsAlternative', False)
+
+                if desired_flavours:
+                    type_ids = {
+                        f.to_flavour_keyed_enum(_CfCoreSortableGameVersionTypeId)
+                        for f in desired_flavours
+                    }
+                    yield lambda f: any(
+                        s['gameVersionTypeId'] in type_ids for s in f['sortableGameVersions']
+                    )
+
+                if not defn.strategies.any_release_type:
+                    yield lambda f: f['releaseType'] == _CfCoreFileReleaseType.release
+
+                if defn.strategies.version_eq:
+                    yield lambda f: f['displayName'] == defn.strategies.version_eq
+
+            filter_fns = list(make_filter_fns(desired_flavours))
+            try:
+                file = max(
+                    (f for f in files if all(r(f) for r in filter_fns)),
+                    # The ``id`` is just a counter so we don't have to go digging around dates
+                    key=lambda f: f['id'],
                 )
-                yield lambda f: any(
-                    s['gameVersionTypeId'] == type_id for s in f['sortableGameVersions']
-                )
-
-            if not defn.strategies.any_release_type:
-                yield lambda f: f['releaseType'] == _CfCoreFileReleaseType.release
-
-            if defn.strategies.version_eq:
-                yield lambda f: f['displayName'] == defn.strategies.version_eq
-
-        filter_fns = list(make_filter_fns())
+            except ValueError:
+                continue
+            break
 
-        file = max(
-            (f for f in files if all(r(f) for r in filter_fns)),
-            # The ``id`` is just a counter so we don't have to go digging around dates
-            key=lambda f: f['id'],
-            default=None,
-        )
-        if file is None:
+        else:
             raise R.PkgFilesNotMatching(defn.strategies)
 
         if file['downloadUrl'] is None:
-            if metadata['allowModDistribution'] is False:
-                raise R.PkgFilesMissing('package distribution is forbidden')
-            else:
-                raise R.PkgFilesMissing
+            raise R.PkgFilesMissing(
+                'package distribution is forbidden'
+                if metadata['allowModDistribution'] is False
+                else None
+            )
 
         return PkgCandidate(
             id=str(metadata['id']),
             slug=metadata['slug'],
             name=metadata['name'],
             description=metadata['summary'],
             url=metadata['links']['websiteUrl'],
```

### Comparing `instawow-4.0.0/src/instawow/_sources/github.py` & `instawow-4.1.0/src/instawow/_sources/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
-from collections.abc import AsyncIterator, Iterable
+import asyncio
+from collections.abc import AsyncIterator, Sequence
 from datetime import datetime, timedelta
-from itertools import tee, zip_longest
+from itertools import product, tee, zip_longest
 from typing import Any, Literal
 
 import iso8601
-from loguru import logger
+from typing_extensions import Never, TypedDict
 from typing_extensions import NotRequired as N
-from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import results as R
+from .._logging import logger
+from .._utils.aio import cancel_tasks
+from .._utils.compat import StrEnum
+from .._utils.iteration import batched
+from .._utils.web import as_plain_text_data_url, extract_byte_range_offset
 from ..catalogue.cataloguer import AddonKey, CatalogueEntry
 from ..definitions import ChangelogFormat, Defn, SourceMetadata, Strategy
 from ..http import CACHE_INDEFINITELY, ClientSessionType
+from ..matchers.addon_toc import TocReader
 from ..pkg_archives import find_archive_addon_tocs
 from ..resolvers import BaseResolver, HeadersIntent, PkgCandidate
-from ..utils import (
-    StrEnum,
-    TocReader,
-    as_plain_text_data_url,
-    extract_byte_range_offset,
-)
 from ..wow_installations import Flavour, FlavourVersionRange
 
 
 # Not exhaustive (as you might've guessed).  Reference:
 # https://docs.github.com/en/rest/reference/repos
 class _GithubRepo(TypedDict):
     id: int  # Unique, stable repository ID
@@ -47,14 +47,15 @@
 
 
 class _GithubRelease_Asset(TypedDict):
     url: str
     name: str  # filename
     content_type: str  # mime type
     state: Literal['starter', 'uploaded']
+    browser_download_url: Never  # Fake type to prevent misuse; actually a string
 
 
 class _PackagerReleaseJson(TypedDict):
     releases: list[_PackagerReleaseJson_Release]
 
 
 class _PackagerReleaseJson_Release(TypedDict):
@@ -79,14 +80,15 @@
 
 class GithubResolver(BaseResolver):
     metadata = SourceMetadata(
         id='github',
         name='GitHub',
         strategies=frozenset(
             {
+                Strategy.AnyFlavour,
                 Strategy.AnyReleaseType,
                 Strategy.VersionEq,
             }
         ),
         changelog_format=ChangelogFormat.Markdown,
         addon_toc_key=None,
     )
@@ -111,15 +113,19 @@
 
         access_token = self._get_access_token(self._manager_ctx.config.global_config, 'github')
         if access_token:
             headers['Authorization'] = f'token {access_token}'
 
         return headers
 
-    async def __find_matching_asset_from_zip_contents(self, assets: list[_GithubRelease_Asset]):
+    async def __find_match_from_zip_contents(
+        self,
+        assets: list[_GithubRelease_Asset],
+        desired_flavours: tuple[Flavour, ...] | None,
+    ):
         candidates = [
             a
             for a in assets
             if a['state'] == 'uploaded'
             and a['content_type'] in {'application/zip', 'application/x-zip-compressed'}
             and a['name'].endswith('.zip')
             # TODO: Is there a better way to detect nolib?
@@ -133,17 +139,32 @@
 
         from aiohttp import hdrs
 
         from ..matchers import NORMALISED_FLAVOUR_TOC_SUFFIXES
 
         download_headers = await self.make_request_headers(HeadersIntent.Download)
 
+        if desired_flavours is None:
+            desired_flavours = tuple(Flavour)
+
+        desired_version_ranges = {
+            f.to_flavour_keyed_enum(FlavourVersionRange) for f in desired_flavours
+        }
+        desired_toc_suffixes = tuple(
+            s for f in desired_flavours for s in NORMALISED_FLAVOUR_TOC_SUFFIXES[f]
+        )
+        all_flavourful_toc_suffixes = tuple(
+            i for s in NORMALISED_FLAVOUR_TOC_SUFFIXES.values() for i in s
+        )
+
         matching_asset = None
 
         for candidate in candidates:
+            logger.info(f'looking for match in zip file: {candidate["browser_download_url"]}')
+
             addon_zip_stream = BytesIO()
             dynamic_addon_zip = None
             is_zip_complete = False
 
             download_url = candidate['url']
 
             # A large enough initial offset that we won't typically have to
@@ -208,31 +229,26 @@
                 for n, h in find_archive_addon_tocs(f.filename for f in dynamic_addon_zip.filelist)
                 if h in candidate['name']  # Folder name is a substring of zip name.
             }
             if not toc_filenames:
                 continue
 
             game_flavour_from_toc_filename = any(
-                n.lower().endswith(
-                    NORMALISED_FLAVOUR_TOC_SUFFIXES[self._manager_ctx.config.game_flavour]
-                )
-                for n in toc_filenames
+                n.lower().endswith(desired_toc_suffixes) for n in toc_filenames
             )
             if game_flavour_from_toc_filename:
                 matching_asset = candidate
                 break
 
             try:
                 main_toc_filename = min(
                     (
                         n
                         for n in toc_filenames
-                        if not n.lower().endswith(
-                            tuple(i for s in NORMALISED_FLAVOUR_TOC_SUFFIXES.values() for i in s)
-                        )
+                        if not n.lower().endswith(all_flavourful_toc_suffixes)
                     ),
                     key=len,
                 )
             except ValueError:
                 continue
 
             if not is_zip_complete:
@@ -259,83 +275,115 @@
                 ) as toc_file_range_response:
                     addon_zip_stream.seek(main_toc_file_offset)
                     addon_zip_stream.write(await toc_file_range_response.read())
 
             toc_file_text = dynamic_addon_zip.read(main_toc_filename).decode('utf-8-sig')
             toc_reader = TocReader(toc_file_text)
 
-            interface_version = toc_reader['Interface']
-            logger.debug(f'found interface version {interface_version!r} in {main_toc_filename}')
-            if interface_version and self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
-                FlavourVersionRange
-            ).contains(int(interface_version)):
+            logger.debug(
+                f'found interface versions {toc_reader.interfaces!r} in {main_toc_filename}'
+            )
+            if toc_reader.interfaces and any(
+                r.contains(i) for r, i in product(desired_version_ranges, toc_reader.interfaces)
+            ):
                 matching_asset = candidate
                 break
 
         return matching_asset
 
-    async def __find_matching_asset_from_release_json(
-        self, assets: list[_GithubRelease_Asset], release_json_asset: _GithubRelease_Asset
+    async def __find_match_from_release_json(
+        self,
+        assets: list[_GithubRelease_Asset],
+        release_json_asset: _GithubRelease_Asset,
+        desired_flavours: tuple[Flavour, ...] | None,
     ):
+        logger.info(
+            f'looking for match in release.json: {release_json_asset["browser_download_url"]}'
+        )
+
         download_headers = await self.make_request_headers(HeadersIntent.Download)
 
         async with self._manager_ctx.web_client.get(
             release_json_asset['url'],
             expire_after=timedelta(days=1),
             headers=download_headers,
             raise_for_status=True,
         ) as response:
             packager_metadata: _PackagerReleaseJson = await response.json(
                 content_type=None  # application/octet-stream
             )
 
-        releases = packager_metadata['releases']
-        if not releases:
+        subreleases = packager_metadata['releases']
+        if not subreleases:
             return None
 
-        wanted_release_json_flavor = self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
-            _PackagerReleaseJsonFlavor
-        )
-        wanted_version_range = self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
-            FlavourVersionRange
-        )
+        if desired_flavours:
+            desired_release_json_flavors = {
+                f.to_flavour_keyed_enum(_PackagerReleaseJsonFlavor) for f in desired_flavours
+            }
+            desired_version_ranges = {
+                f.to_flavour_keyed_enum(FlavourVersionRange) for f in desired_flavours
+            }
+
+            def is_compatible(release: _PackagerReleaseJson_Release):  # pyright: ignore[reportRedeclaration]
+                for metadata in release['metadata']:
+                    if metadata['flavor'] in desired_release_json_flavors:
+                        if any(r.contains(metadata['interface']) for r in desired_version_ranges):
+                            return True
+
+                        logger.info(
+                            f'flavor and interface mismatch: {metadata["interface"]} not found in '
+                            f'{[r.value for r in desired_version_ranges]}'
+                        )
 
-        def is_compatible_release(release: _PackagerReleaseJson_Release):
-            if release['nolib']:
                 return False
 
-            for metadata in release['metadata']:
-                if metadata['flavor'] != wanted_release_json_flavor:
-                    continue
-
-                interface_version = metadata['interface']
-                if not wanted_version_range.contains(interface_version):
-                    logger.info(
-                        f'interface number "{interface_version}" and flavor "{wanted_release_json_flavor}" mismatch'
-                    )
-                    continue
+        else:
 
+            def is_compatible(release: _PackagerReleaseJson_Release):
                 return True
 
-            return False
-
-        matching_release = next(filter(is_compatible_release, releases), None)
+        matching_release = next(
+            (r for r in subreleases if not r['nolib'] and is_compatible(r)), None
+        )
         if matching_release is None:
             return None
 
         matching_asset = next(
             (
                 a
                 for a in assets
                 if a['name'] == matching_release['filename'] and a['state'] == 'uploaded'
             ),
             None,
         )
         return matching_asset
 
+    async def __find_match(
+        self,
+        release: _GithubRelease,
+        desired_flavour_groups: Sequence[tuple[Flavour, ...] | None],
+    ):
+        assets = release['assets']
+
+        release_json = next(
+            (a for a in assets if a['name'] == 'release.json' and a['state'] == 'uploaded'),
+            None,
+        )
+        for desired_flavours in desired_flavour_groups:
+            if release_json:
+                asset = await self.__find_match_from_release_json(
+                    assets, release_json, desired_flavours
+                )
+            else:
+                asset = await self.__find_match_from_zip_contents(assets, desired_flavours)
+
+            if asset:
+                return (release, asset)
+
     async def _resolve_one(self, defn: Defn, metadata: None) -> PkgCandidate:
         github_headers = await self.make_request_headers()
 
         id_or_alias = defn.id or defn.alias
         if id_or_alias.isdigit():
             repo_url = self.__api_url / 'repositories' / id_or_alias
         else:
@@ -343,14 +391,15 @@
 
         async with self._manager_ctx.web_client.get(
             repo_url, expire_after=timedelta(hours=1), headers=github_headers
         ) as response:
             if response.status == 404:
                 raise R.PkgNonexistent
             response.raise_for_status()
+
             project: _GithubRepo = await response.json()
 
         if defn.strategies.version_eq:
             release_url = URL(project['url']) / 'releases/tags' / defn.strategies.version_eq
         else:
             # Includes pre-releases
             release_url = (URL(project['url']) / 'releases').with_query(
@@ -358,59 +407,76 @@
                 per_page='10'
             )
 
         async with self._manager_ctx.web_client.get(
             release_url, expire_after=timedelta(minutes=5), headers=github_headers
         ) as response:
             if response.status == 404:
-                raise R.PkgFilesMissing('release not found')
+                raise R.PkgFilesMissing('no releases found')
             response.raise_for_status()
 
-            response_json = await response.json()
-            if defn.strategies.version_eq:
-                response_json = [response_json]
-            releases: Iterable[_GithubRelease] = response_json
+            release_json: _GithubRelease | list[_GithubRelease] = await response.json()
+            if not isinstance(release_json, list):
+                release_json = [release_json]
 
         # Only users with push access will get draft releases
         # but let's filter them out just in case.
-        releases = (r for r in releases if r['draft'] is False)
+        releases = (r for r in release_json if r['draft'] is False)
 
         if not defn.strategies.any_release_type:
             releases = (r for r in releases if r['prerelease'] is False)
 
-        seen_release_json = False
-        for release in releases:
-            assets = release['assets']
-            matching_asset = None
-
-            release_json = next(
-                (a for a in assets if a['name'] == 'release.json' and a['state'] == 'uploaded'),
-                None,
-            )
-            if not seen_release_json and release_json is None:
-                matching_asset = await self.__find_matching_asset_from_zip_contents(assets)
-            elif release_json is not None:
-                seen_release_json = True
-                matching_asset = await self.__find_matching_asset_from_release_json(
-                    assets, release_json
-                )
+        first_release = next(releases, None)
+        if first_release is None:
+            raise R.PkgFilesNotMatching(defn.strategies)
 
-            if matching_asset is not None:
-                break
+        desired_flavour_groups = self._manager_ctx.config.game_flavour.get_flavour_groups(
+            bool(defn.strategies.any_flavour)
+        )
+
+        # We'll look for affine flavours > absolutely any flavour in every release
+        # if any_flavour is true.  This is less expensive than performing
+        # separate flavour passes across the whole release list for the common case.
+        match = await self.__find_match(first_release, desired_flavour_groups)
+        if not match:
+            logger.info('looking for match in older releases')
+
+            _remaining_tasks = []
+            try:
+                for release_task, _remaining_tasks in (
+                    (t, g[o:])
+                    # 3 groups of 3 run in parallel but processed in order
+                    for b in batched(releases, 3)
+                    for g in (
+                        [
+                            asyncio.create_task(self.__find_match(r, desired_flavour_groups))
+                            for r in b
+                        ],
+                    )
+                    for o, t in enumerate(g, start=1)
+                ):
+                    match = await release_task
+                    if match:
+                        break
+            finally:
+                if _remaining_tasks:
+                    await cancel_tasks(_remaining_tasks)
 
+        if match:
+            release, asset = match
         else:
             raise R.PkgFilesNotMatching(defn.strategies)
 
         return PkgCandidate(
             id=str(project['id']),
             slug=project['full_name'].lower(),
             name=project['name'],
             description=project['description'] or '',
             url=project['html_url'],
-            download_url=matching_asset['url'],
+            download_url=asset['url'],
             date_published=iso8601.parse_date(release['published_at']),
             version=release['tag_name'],
             changelog_url=as_plain_text_data_url(release['body']),
         )
 
     @classmethod
     async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[CatalogueEntry]:
```

### Comparing `instawow-4.0.0/src/instawow/_sources/instawow.py` & `instawow-4.1.0/src/instawow/_sources/instawow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator
 from datetime import datetime, timezone
 
 from .. import results as R
+from .._utils.aio import run_in_thread
 from ..catalogue.cataloguer import CatalogueEntry
 from ..definitions import ChangelogFormat, Defn, SourceMetadata
 from ..http import ClientSessionType
 from ..resolvers import BaseResolver, PkgCandidate
-from ..utils import run_in_thread
 from ..wow_installations import Flavour
 
 _ADDONS = {
     ('0', 'weakauras-companion'),
     ('1', 'weakauras-companion-autoupdate'),
 }
```

### Comparing `instawow-4.0.0/src/instawow/_sources/tukui.py` & `instawow-4.1.0/src/instawow/_sources/tukui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator
 from datetime import datetime, timedelta, timezone
 
-from loguru import logger
 from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import results as R
+from .._logging import logger
 from ..catalogue.cataloguer import CatalogueEntry
 from ..definitions import ChangelogFormat, Defn, SourceMetadata
 from ..http import ClientSessionType
 from ..resolvers import BaseResolver, PkgCandidate
 from ..wow_installations import Flavour, FlavourVersionRange
```

### Comparing `instawow-4.0.0/src/instawow/_sources/wago.py` & `instawow-4.1.0/src/instawow/_sources/wago.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 import iso8601
 from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import matchers
 from .. import results as R
+from .._utils.aio import run_in_thread
+from .._utils.compat import StrEnum
+from .._utils.web import as_plain_text_data_url
 from ..definitions import ChangelogFormat, Defn, SourceMetadata, Strategy
 from ..http import GenericDownloadTraceRequestCtx
 from ..resolvers import BaseResolver, HeadersIntent, PkgCandidate, TFolderHashCandidate
-from ..utils import StrEnum, as_plain_text_data_url, run_in_thread
 
 _WagoStability = Literal['stable', 'beta', 'alpha']
 
 
 class _WagoGameVersion(StrEnum):
     Retail = 'retail'
     VanillaClassic = 'classic'
```

### Comparing `instawow-4.0.0/src/instawow/_sources/wowi.py` & `instawow-4.1.0/src/instawow/_sources/wowi.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 
 import re
 from collections.abc import AsyncIterator, Sequence
 from datetime import datetime, timedelta, timezone
 from itertools import takewhile
 from typing import Literal
 
-from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import pkg_models
 from .. import results as R
+from .._logging import logger
+from .._utils.aio import gather
+from .._utils.iteration import uniq
+from .._utils.text import slugify
+from .._utils.web import as_plain_text_data_url
 from ..catalogue.cataloguer import CatalogueEntry
 from ..definitions import ChangelogFormat, Defn, SourceMetadata
 from ..http import ClientSessionType, GenericDownloadTraceRequestCtx
 from ..resolvers import BaseResolver, PkgCandidate
-from ..utils import as_plain_text_data_url, gather, slugify, uniq
 from ..wow_installations import Flavour, FlavourVersionRange
 
 _lock_prefix = object()
 
 _LOAD_WOWI_CATALOGUE_LOCK = '_LOAD_WOWI_CATALOGUE_LOCK_'
 
 
@@ -149,20 +152,17 @@
             response.raise_for_status()
 
             details_items_by_id: dict[str, _WowiDetailsApiItem] = {
                 i['UID']: i for i in await response.json()
             }
 
         results = await gather(
-            (
-                self.resolve_one(d, {**a, **b} if a and b else None)
-                for d, i in defns_to_ids.items()
-                for a, b in ((list_items_by_id.get(i), details_items_by_id.get(i)),)
-            ),
-            R.resultify_async_exc,
+            R.resultify_async_exc(self.resolve_one(d, {**a, **b} if a and b else None))
+            for d, i in defns_to_ids.items()
+            for a, b in ((list_items_by_id.get(i), details_items_by_id.get(i)),)
         )
         return dict(zip(defns, results))
 
     async def _resolve_one(self, defn: Defn, metadata: _WowiCombinedItem | None) -> PkgCandidate:
         if metadata is None:
             raise R.PkgNonexistent
```

### Comparing `instawow-4.0.0/src/instawow/catalogue/__init__.py` & `instawow-4.1.0/src/instawow/catalogue/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import datetime as dt
 import json
 from functools import lru_cache
 
-from loguru import logger
-
 from .. import manager_ctx
+from .._logging import logger
+from .._utils.perf import time_op
 from ..http import GenericDownloadTraceRequestCtx
-from ..utils import time_op
 from . import cataloguer
 
 _LOAD_CATALOGUE_LOCK = '_LOAD_CATALOGUE_'
 
 _base_catalogue_url = (
     f'https://raw.githubusercontent.com/layday/instawow-data/data/'
     f'base-catalogue-v{cataloguer.CATALOGUE_VERSION}.compact.json'
```

### Comparing `instawow-4.0.0/src/instawow/catalogue/cataloguer.py` & `instawow-4.1.0/src/instawow/catalogue/cataloguer.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 import attrs
 import cattrs
 import cattrs.preconf.json
 from typing_extensions import Self
 
 from .. import http
-from ..utils import bucketise, fauxfrozen, normalise_names
+from .._utils.compat import fauxfrozen
+from .._utils.iteration import bucketise
+from .._utils.text import normalise_names
 from ..wow_installations import Flavour
 
 CATALOGUE_VERSION = 7
 COMPUTED_CATALOGUE_VERSION = 4
 
 
 catalogue_converter = cattrs.Converter(
```

### Comparing `instawow-4.0.0/src/instawow/catalogue/search.py` & `instawow-4.1.0/src/instawow/catalogue/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Iterator, Set
 from datetime import datetime
 from typing import Literal
 
-from .. import manager_ctx, pkg_db
-from ..utils import bucketise, normalise_names
+from .. import manager_ctx
+from .._utils.iteration import bucketise
+from .._utils.text import normalise_names
 from . import cataloguer
 from . import synchronise as synchronise_catalogue
 
 _normalise_search_terms = normalise_names('')
 
 
 async def search(
@@ -39,20 +40,19 @@
         if unknown_sources:
             raise ValueError(f'Unknown sources: {", ".join(unknown_sources)}')
 
     if prefer_source and prefer_source not in manager_ctx.resolvers:
         raise ValueError(f'Unknown preferred source: {prefer_source}')
 
     def get_installed_pkg_keys():
-        with manager_ctx.database.connect() as connection:
-            return (
-                connection.execute(pkg_db.sa.select(pkg_db.pkg.c.source, pkg_db.pkg.c.id))
-                .tuples()
-                .all()
-            )
+        with (
+            manager_ctx.database.connect() as connection,
+            manager_ctx.database.use_tuple_factory(connection) as cursor,
+        ):
+            return cursor.execute('SELECT source, id FROM pkg').fetchall()
 
     def make_filter_fns() -> Iterator[Callable[[cataloguer.ComputedCatalogueEntry], bool]]:
         yield lambda e: manager_ctx.config.game_flavour in e.game_flavours
 
         if sources:
             yield lambda e: e.source in sources
```

### Comparing `instawow-4.0.0/src/instawow/http/__init__.py` & `instawow-4.1.0/src/instawow/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         cache_backend = CacheBackend(
             allowed_codes=(200, 206),
             allowed_methods=('GET', 'POST'),
             expire_after=_DEFAULT_EXPIRE,
             include_headers=True,
         )
-        with make_cache(cache_dir) as cache:
+        async with make_cache(cache_dir) as cache:
             cache_backend.responses = cache_backend.redirects = cache
             if no_cache:
                 cache_backend.disabled = True
 
             async with CachedSession(cache=cache_backend, **kwargs) as client_session:
                 yield client_session
```

### Comparing `instawow-4.0.0/src/instawow/http/_cache.py` & `instawow-4.1.0/src/instawow/http/_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 import diskcache
 from typing_extensions import ParamSpec
 
 _U = TypeVar('_U')
 _P = ParamSpec('_P')
 
 
-@contextlib.contextmanager
-def make_cache(cache_dir: os.PathLike[str]):
-    with (
-        concurrent.futures.ThreadPoolExecutor(1, '_http_cache') as executor,
-        diskcache.Cache(os.fspath(cache_dir)) as cache,
-    ):
+@contextlib.asynccontextmanager
+async def make_cache(cache_dir: os.PathLike[str]):
+    with concurrent.futures.ThreadPoolExecutor(1, '_http_cache') as executor:
         loop = asyncio.get_running_loop()
 
         def run_in_thread2(fn: Callable[_P, _U]) -> Callable[_P, Coroutine[Any, Any, _U]]:
             @wraps(fn)
             async def wrapper(*args: _P.args, **kwargs: _P.kwargs):
                 return await loop.run_in_executor(
                     executor, lambda: contextvars.copy_context().run(fn, *args, **kwargs)
                 )
 
             return wrapper
 
+        # diskcache will only close the sqlite connection if it was initialised
+        # in the same thread.
+        cache = await run_in_thread2(diskcache.Cache)(os.fspath(cache_dir))
+
         class Cache(aiohttp_client_cache.BaseCache):
             @run_in_thread2
             def bulk_delete(self, keys: Set[str]):
                 for key in keys:
                     cache.delete(key)
 
             @run_in_thread2
@@ -71,8 +72,11 @@
                 async for key in self.keys():
                     yield cast(aiohttp_client_cache.ResponseOrKey, run_in_thread2(cache.get)(key))
 
             @run_in_thread2
             def write(self, key: str, item: aiohttp_client_cache.ResponseOrKey):
                 cache[key] = item
 
-        yield Cache()
+        try:
+            yield Cache()
+        finally:
+            await run_in_thread2(cache.close)()
```

### Comparing `instawow-4.0.0/src/instawow/matchers/__init__.py` & `instawow-4.1.0/src/instawow/matchers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,23 @@
 from itertools import chain, product
 from pathlib import Path
 from typing import Protocol
 
 import attrs
 from typing_extensions import Self
 
-from .. import manager_ctx, pkg_db
+from .. import manager_ctx
+from .._utils.aio import gather
+from .._utils.compat import fauxfrozen
+from .._utils.iteration import bucketise, merge_intersecting_sets, uniq
 from ..catalogue import synchronise as synchronise_catalogue
 from ..definitions import Defn
-from ..utils import (
-    TocReader,
-    bucketise,
-    fauxfrozen,
-    gather,
-    merge_intersecting_sets,
-    uniq,
-)
 from ..wow_installations import Flavour
 from ._addon_hashing import generate_wowup_addon_hash
+from .addon_toc import TocReader
 
 
 class Matcher(Protocol):  # pragma: no cover
     def __call__(
         self, manager_ctx: manager_ctx.ManagerCtx, leftovers: frozenset[AddonFolder]
     ) -> Awaitable[list[tuple[list[AddonFolder], list[Defn]]]]: ...
 
@@ -49,15 +45,14 @@
     ),
     Flavour.CataclysmClassic: ('Cata',),
 }
 
 FLAVOUR_TOC_SUFFIXES = {
     k: tuple(f'{s}{f}.toc' for s, f in product('-_', v)) for k, v in FLAVOUR_TOC_IDS.items()
 }
-
 NORMALISED_FLAVOUR_TOC_SUFFIXES = {
     k: tuple(i.lower() for i in v) for k, v in FLAVOUR_TOC_SUFFIXES.items()
 }
 
 
 @fauxfrozen(order=True)
 class AddonFolder:
@@ -77,26 +72,27 @@
             except FileNotFoundError:
                 pass
 
     def hash_contents(self, __method: AddonHashMethod) -> str:
         return generate_wowup_addon_hash(self.path)
 
     def get_defns_from_toc_keys(self, keys_and_ids: Iterable[tuple[str, str]]) -> frozenset[Defn]:
-        return frozenset(Defn(s, i) for k, s in keys_and_ids for i in (self.toc_reader[k],) if i)
+        return frozenset(
+            Defn(s, i) for k, s in keys_and_ids for i in (self.toc_reader.get(k),) if i
+        )
 
     @cached_property
     def version(self) -> str:
-        return self.toc_reader['Version', 'X-Packaged-Version', 'X-Curse-Packaged-Version'] or ''
+        version_keys = ('Version', 'X-Packaged-Version', 'X-Curse-Packaged-Version')
+        return next(filter(None, map(self.toc_reader.get, version_keys)), '')
 
 
 def _get_unreconciled_folders(manager_ctx: manager_ctx.ManagerCtx):
     with manager_ctx.database.connect() as connection:
-        pkg_folders = (
-            connection.execute(pkg_db.sa.select(pkg_db.pkg_folder.c.name)).scalars().all()
-        )
+        pkg_folders = [n for (n,) in connection.execute('SELECT name FROM pkg_folder').fetchall()]
 
     unreconciled_folder_paths = (
         p
         for p in manager_ctx.config.addon_dir.iterdir()
         if p.name not in pkg_folders and p.is_dir() and not p.is_symlink()
     )
     for path in unreconciled_folder_paths:
```

### Comparing `instawow-4.0.0/src/instawow/matchers/_addon_hashing.py` & `instawow-4.1.0/src/instawow/matchers/_addon_hashing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import hashlib
 import os
 import re
 from collections.abc import Iterator
 from functools import lru_cache
 from pathlib import Path
 
-from loguru import logger
+from .._logging import logger
 
 _TOC_FILE_PATH_PATTERN = re.compile(
     r'^(?P<name>[^/]+)/(?P=name)(?:[-_](?:mainline|bcc|tbc|classic|vanilla|wrath|wotlkc))?\.toc$',
     flags=re.IGNORECASE,
 )
 _BINDINGS_XML_FILE_PATH_PATTERN = re.compile(
     r'^[^/]+/Bindings\.xml$',
```

### Comparing `instawow-4.0.0/src/instawow_wa_updater/_cli.py` & `instawow-4.1.0/src/instawow_wa_updater/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     mw.run_with_progress(WaCompanionBuilder(mw.manager.ctx).build())
 
 
 @wa_updater_command_group.command('list')
 @click.pass_obj
 def list_installed_wago_auras(mw: cli.CtxObjWrapper) -> None:
     "List WeakAuras installed from Wago."
-    from instawow.utils import tabulate
+    from instawow._utils.text import tabulate
 
     from ._core import WaCompanionBuilder
 
     aura_groups = WaCompanionBuilder(mw.manager.ctx).extract_installed_auras()
     installed_auras = sorted(
         (g.addon_name, a.id, a.url)
         for g in aura_groups
```

### Comparing `instawow-4.0.0/src/instawow_wa_updater/_core.py` & `instawow-4.1.0/src/instawow_wa_updater/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from __future__ import annotations
 
+import importlib.resources
 import json
 from collections.abc import Iterable, Iterator, Mapping, Sequence
 from datetime import timedelta
 from functools import reduce
 from itertools import chain, product
 from typing import Literal, TypeAlias, cast
 
 import cattrs
-from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
+from instawow._logging import logger
+from instawow._utils.aio import gather, run_in_thread
+from instawow._utils.compat import StrEnum, fauxfrozen
+from instawow._utils.iteration import bucketise
+from instawow._utils.perf import time_op
+from instawow._utils.text import shasum
 from instawow.http import CACHE_INDEFINITELY, GenericDownloadTraceRequestCtx
 from instawow.manager_ctx import ManagerCtx
-from instawow.utils import (
-    StrEnum,
-    bucketise,
-    fauxfrozen,
-    gather,
-    read_resource_as_text,
-    shasum,
-    time_op,
-)
-from instawow.utils import run_in_thread as t
 
 _LuaTable: TypeAlias = Mapping[str, '_LuaTable']
 _Auras: TypeAlias = 'WeakAuras | Plateroos'
 _Match: TypeAlias = tuple[Sequence['WeakAura | Plateroo'], '_WagoApiResponse', str]
 
 
 class _WagoApiResponse(TypedDict):
@@ -239,14 +235,16 @@
         ]
 
     def _generate_addon(self, auras: Iterable[tuple[type[_Auras], list[_Match]]]):
         from zipfile import ZipFile, ZipInfo
 
         from . import _templates
 
+        template_resources = importlib.resources.files(_templates)
+
         aura_dict = dict.fromkeys((WeakAuras, Plateroos), list[_Match]()) | dict(auras)
 
         self.addon_zip_path.parent.mkdir(exist_ok=True)
 
         with ZipFile(self.addon_zip_path, 'w') as file:
 
             def write_file(filename: str, content: str):
@@ -289,33 +287,35 @@
     }},"""
     for c, v in aura_dict.items()
 )}
 }}
 ''',
             )
 
-            init_output = write_file('init.lua', read_resource_as_text(_templates, 'init.lua'))
+            init_output = write_file(
+                'init.lua', template_resources.joinpath('init.lua').read_text()
+            )
 
             interface_version = self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
                 _TocNumber
             ).value
             addon_version = shasum(data_output, init_output, interface_version)[:7]
 
-            toc_tpl = read_resource_as_text(_templates, 'WeakAurasCompanion.toc')
+            toc_tpl = template_resources.joinpath('WeakAurasCompanion.toc').read_text()
             write_file(
                 'WeakAurasCompanion.toc',
                 toc_tpl.format(
                     interface=self._manager_ctx.config.game_flavour.to_flavour_keyed_enum(
                         _TocNumber
                     ).value,
                     version=addon_version,
                 ),
             )
 
-        changelog_tpl = read_resource_as_text(_templates, 'CHANGELOG.md')
+        changelog_tpl = template_resources.joinpath('CHANGELOG.md').read_text()
         self.changelog_path.write_text(
             '\n\n'.join(
                 changelog_tpl.format(
                     name=a.id,
                     url=a.url.parent,
                     version=metadata['version'],
                     changelog=metadata['changelog'].get('text') or 'n/a',
@@ -332,16 +332,16 @@
         self._version_txt_path.write_text(
             addon_version,
             encoding='utf-8',
         )
 
     async def build(self) -> None:
         installed_auras_by_type = _merge_auras(
-            await t(list[_Auras])(self.extract_installed_auras()),
+            await run_in_thread(list[_Auras])(self.extract_installed_auras()),
         )
         remote_auras = await gather(
             self.get_remote_auras(r) for r in installed_auras_by_type.values()
         )
-        await t(self._generate_addon)(zip(installed_auras_by_type, remote_auras))
+        await run_in_thread(self._generate_addon)(zip(installed_auras_by_type, remote_auras))
 
     def get_version(self) -> str:
         return self._version_txt_path.read_text(encoding='utf-8')
```

### Comparing `instawow-4.0.0/src/instawow_wa_updater/_custom_slpp.py` & `instawow-4.1.0/src/instawow_wa_updater/_custom_slpp.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow_wa_updater/_templates/COPYING.WeakAuras-Companion` & `instawow-4.1.0/src/instawow_wa_updater/_templates/COPYING.WeakAuras-Companion`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/src/instawow_wa_updater/_templates/init.lua` & `instawow-4.1.0/src/instawow_wa_updater/_templates/init.lua`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/conftest.py` & `instawow-4.1.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from typing import Any
 
 import aiohttp
 import aiohttp.web
 import pytest
 from aresponses import ResponsesMockServer
 from aresponses.errors import NoRouteFoundError
-from loguru import logger
+from yarl import URL
 
+from instawow._logging import logger
 from instawow.config import GlobalConfig, ProfileConfig
 from instawow.http import init_web_client
 from instawow.manager_ctx import ManagerCtx, contextualise
 from instawow.pkg_management import PkgManager
 from instawow.wow_installations import _DELECTABLE_DIR_NAMES, Flavour
 
 from .fixtures.http import ROUTES
@@ -117,17 +118,21 @@
 @pytest.fixture
 async def iw_web_client(iw_config: ProfileConfig):
     async with init_web_client(iw_config.global_config.cache_dir) as web_client:
         yield web_client
 
 
 @pytest.fixture
-def iw_manager_ctx(iw_config: ProfileConfig, iw_web_client: aiohttp.ClientSession):
-    contextualise(web_client=iw_web_client)
-    return ManagerCtx(iw_config)
+def iw_manager_ctx(
+    iw_config: ProfileConfig,
+    iw_web_client: aiohttp.ClientSession,
+):
+    with ManagerCtx(iw_config) as ctx:
+        contextualise(web_client=iw_web_client)
+        yield ctx
 
 
 @pytest.fixture
 def iw_manager(iw_manager_ctx: ManagerCtx):
     return PkgManager(iw_manager_ctx)
 
 
@@ -135,14 +140,15 @@
 @should_mock
 def _iw_mock_aiohttp_requests(
     request: pytest.FixtureRequest, iw_aresponses: _StrictResponsesMockServer
 ):
     if request.param == 'all':
         routes = ROUTES.values()
     else:
-        if not request.param.issubset(ROUTES.keys()):
+        urls = set(map(URL, request.param))
+        if not urls.issubset(ROUTES.keys()):
             raise ValueError('Supplied routes must be subset of all routes')
 
-        routes = (ROUTES[k] for k in ROUTES.keys() & request.param)
+        routes = (ROUTES[k] for k in ROUTES.keys() & urls)
 
     for route in routes:
         iw_aresponses.add(**route.to_aresponses_add_args())
```

### Comparing `instawow-4.0.0/tests/test_catalogue_search.py` & `instawow-4.1.0/tests/test_catalogue_search.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_cli.py` & `instawow-4.1.0/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 from __future__ import annotations
 
 import json
 import shutil
-from collections.abc import Callable as C
+from collections.abc import Callable
 from functools import partial
 from textwrap import dedent
+from typing import TypeAlias
 from unittest import mock
 
 import pytest
 from cattrs.preconf.json import make_converter as make_json_converter
 from click.testing import CliRunner, Result
 from prompt_toolkit.application import create_app_session
-from prompt_toolkit.input import create_pipe_input
+from prompt_toolkit.input import PipeInput, create_pipe_input
 from prompt_toolkit.output import DummyOutput
 
 from instawow import __version__
 from instawow.cli import cli
 from instawow.config import ProfileConfig
 from instawow.definitions import SourceMetadata
 
+Run: TypeAlias = Callable[[str], Result]
+
 
 @pytest.fixture(autouse=True, scope='module')
-def _iw_mock_pt_progress_bar():
+def _mock_pt_progress_bar():
     monkeypatch = pytest.MonkeyPatch()
     monkeypatch.setattr('prompt_toolkit.shortcuts.progress_bar.ProgressBar', mock.MagicMock())
     yield
     monkeypatch.undo()
 
 
 @pytest.fixture
-def feed_pt():
-    with create_pipe_input() as input_, create_app_session(input=input_, output=DummyOutput()):
-        yield input_.send_text
+def pt_input():
+    with (
+        create_pipe_input() as pipe_input,
+        create_app_session(input=pipe_input, output=DummyOutput()),
+    ):
+        yield pipe_input
 
 
 @pytest.fixture
 async def run(
     monkeypatch: pytest.MonkeyPatch,
     iw_config: ProfileConfig,
 ):
@@ -45,24 +51,24 @@
     monkeypatch.setattr('asyncio.run', loop.run_until_complete)
 
     return partial(CliRunner().invoke, cli, catch_exceptions=False)
 
 
 @pytest.fixture
 def install_molinari_and_run(
-    run: C[[str], Result],
+    run: Run,
 ):
     run('install curse:molinari')
     return run
 
 
 @pytest.fixture
 def pretend_install_molinari_and_run(
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
 ):
     molinari = iw_config.addon_dir / 'Molinari'
     molinari.mkdir()
     (molinari / 'Molinari.toc').write_text(
         """\
 ## X-Curse-Project-ID: 20338
 ## X-WoWI-ID: 13188
@@ -77,83 +83,83 @@
         'curse:molinari',
         'wowi:13188-molinari',
         'tukui:tukui',
         'github:p3lim-wow/Molinari',
     ],
 )
 def test_valid_pkg_lifecycle(
-    run: C[[str], Result],
+    run: Run,
     alias: str,
 ):
     assert run(f'install {alias}').output.startswith(f'✓ {alias}\n  installed')
     assert run(f'install {alias}').output == f'✗ {alias}\n  package already installed\n'
     assert run(f'update {alias}').output == f'✗ {alias}\n  package is up to date\n'
     assert run(f'remove {alias}').output == f'✓ {alias}\n  removed\n'
     assert run(f'update {alias}').output == f'✗ {alias}\n  package is not installed\n'
     assert run(f'remove {alias}').output == f'✗ {alias}\n  package is not installed\n'
 
 
 @pytest.mark.parametrize('alias', ['instawow:gargantuan-wigs'])
 def test_nonexistent_pkg_lifecycle(
-    run: C[[str], Result],
+    run: Run,
     alias: str,
 ):
     assert run(f'install {alias}').output == f'✗ {alias}\n  package does not exist\n'
     assert run(f'update {alias}').output == f'✗ {alias}\n  package is not installed\n'
     assert run(f'remove {alias}').output == f'✗ {alias}\n  package is not installed\n'
 
 
 @pytest.mark.parametrize('alias', ['foo:bar'])
 def test_invalid_source_lifecycle(
-    run: C[[str], Result],
+    run: Run,
     alias: str,
 ):
     assert run(f'install {alias}').output == f'✗ :{alias}\n  package source is invalid\n'
     assert run(f'update {alias}').output == f'✗ :{alias}\n  package is not installed\n'
     assert run(f'remove {alias}').output == f'✗ :{alias}\n  package is not installed\n'
 
 
 def test_reconciled_folder_conflict_on_install(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('install curse:molinari').output.startswith('✓ curse:molinari\n  installed')
     assert run('install wowi:13188-molinari').output == (
         '✗ wowi:13188-molinari\n'
         '  package folders conflict with installed package Molinari\n'
         '    (curse:20338)\n'
     )
 
 
 def test_unreconciled_folder_conflict_on_install(
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
 ):
     iw_config.addon_dir.joinpath('Molinari').mkdir()
     assert (
         run('install curse:molinari').output
         == "✗ curse:molinari\n  package folders conflict with 'Molinari'\n"
     )
     assert run('install --replace curse:molinari').output.startswith(
         '✓ curse:molinari\n  installed'
     )
 
 
 def test_keep_folders_on_remove(
     iw_config: ProfileConfig,
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     assert (
         install_molinari_and_run('remove --keep-folders curse:molinari').output
         == '✓ curse:molinari\n  removed\n'
     )
     assert iw_config.addon_dir.joinpath('Molinari').is_dir()
 
 
 def test_version_strategy_lifecycle(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('install curse:molinari').output.startswith(
         '✓ curse:molinari\n  installed 100205.111-Release'
     )
     assert (
         run('install curse:molinari#version_eq=foo').output
         == '✗ curse:molinari\n  package already installed\n'
@@ -186,27 +192,27 @@
             version_eq=None
         """
     )
     assert run('remove curse:molinari').output == '✓ curse:molinari\n  removed\n'
 
 
 def test_install_options(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('install curse:molinari#any_release_type,any_flavour').output == dedent(
         """\
         ✓ curse:molinari
           installed 100205.111-Release
         """
     )
 
 
 @pytest.mark.parametrize('step', [1, -1])
 def test_install_order_is_respected(
-    run: C[[str], Result],
+    run: Run,
     step: int,
 ):
     assert run(
         'install '
         + ' '.join(
             [
                 'curse:molinari',
@@ -221,144 +227,157 @@
           package folders conflict with installed package Molinari
             (curse:20338)
         """
     )
 
 
 def test_install_invalid_defn(
-    run: C[[str], Result],
+    run: Run,
 ):
     result = run('install foo')
     assert result.exit_code == 2
     assert result.output.endswith("Error: Invalid value for '[ADDONS]...': foo\n")
 
 
 def test_install_dry_run(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('install --dry-run curse:molinari').output == dedent(
         """\
         ✓ curse:molinari
           would have installed 100205.111-Release
         """
     )
 
 
-def test_debug(
+def test_debug_config(
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
 ):
-    assert run('debug').output == iw_config.encode_for_display() + '\n'
+    assert (
+        run('debug config').output
+        == json.dumps(iw_config.unstructure_for_display(), indent=2) + '\n'
+    )
+
+
+def test_debug_sources(
+    run: Run,
+):
+    json_converter = make_json_converter()
+
+    output = run('debug sources').output
+    source_metadata = json_converter.loads(output, list[SourceMetadata])
+    assert len(source_metadata) > 1
 
 
 @pytest.mark.parametrize('command', ['configure', 'list'], ids=['explicit', 'implicit'])
 def test_configure__create_new_profile(
     monkeypatch: pytest.MonkeyPatch,
-    feed_pt: C[[str], None],
+    pt_input: PipeInput,
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
     command: str,
 ):
     # In case there is a WoW installation in the test environment.
     monkeypatch.setattr('instawow.wow_installations.find_installations', lambda: iter([]))
 
-    feed_pt(f'{iw_config.addon_dir}\r\rY\r')
+    pt_input.send_text(f'{iw_config.addon_dir}\r\rY\r')
     assert run(f'-p foo {command}').output == (
         'Navigate to https://github.com/login/device and paste the code below:\n'
         '  WDJB-MJHT\n'
         'Waiting...\n'
         'Configuration written to:\n'
         f'  {iw_config.global_config.config_dir / "config.json"}\n'
         f'  {iw_config.global_config.config_dir / "profiles/foo/config.json"}\n'
     )
 
 
 def test_configure__update_existing_profile_interactively(
-    feed_pt: C[[str], None],
+    pt_input: PipeInput,
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
 ):
-    feed_pt('Y\r')
+    pt_input.send_text('Y\r')
     assert run('configure global_config.auto_update_check').output == (
         'Configuration written to:\n'
         f'  {iw_config.global_config.config_dir / "config.json"}\n'
         f'  {iw_config.global_config.config_dir / "profiles/__default__/config.json"}\n'
     )
 
 
 def test_configure__update_existing_profile_directly(
     iw_config: ProfileConfig,
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('configure global_config.auto_update_check=0').output == (
         'Configuration written to:\n'
         f'  {iw_config.global_config.config_dir / "config.json"}\n'
         f'  {iw_config.global_config.config_dir / "profiles/__default__/config.json"}\n'
     )
 
 
 @pytest.mark.parametrize('options', ['', '--undo'])
 def test_rollback__pkg_not_installed(
-    run: C[[str], Result],
+    run: Run,
     options: str,
 ):
     assert (
         run(f'rollback {options} curse:molinari').output
         == '✗ curse:molinari\n  package is not installed\n'
     )
 
 
 @pytest.mark.parametrize('options', ['', '--undo'])
 def test_rollback__unsupported(
-    run: C[[str], Result],
+    run: Run,
     options: str,
 ):
     assert run('install wowi:13188-molinari').exit_code == 0
     assert (
         run(f'rollback {options} wowi:13188-molinari').output
         == '✗ wowi:13188-molinari\n  strategies are not valid for source: version_eq\n'
     )
 
 
 def test_rollback__single_version(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('install curse:molinari').exit_code == 0
     assert (
         run('rollback curse:molinari').output == '✗ curse:molinari\n  cannot find older versions\n'
     )
 
 
 def test_rollback__multiple_versions(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
 ):
     assert run('install curse:molinari#version_eq=100005.97-Release').exit_code == 0
     assert run('remove curse:molinari').exit_code == 0
     assert run('install curse:molinari').exit_code == 0
-    feed_pt('\r\r')
+    pt_input.send_text('\r\r')
     assert run('rollback curse:molinari').output == dedent(
         """\
         ✓ curse:molinari
           updated 100205.111-Release to 100005.97-Release with new strategies:
             version_eq='100005.97-Release'
         """
     )
 
 
 @pytest.mark.parametrize('options', ['', '--undo'])
 def test_rollback__rollback_multiple_versions(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
     options: str,
 ):
     assert run('install curse:molinari').exit_code == 0
     assert run('remove curse:molinari').exit_code == 0
     assert run('install curse:molinari#version_eq=100005.97-Release').exit_code == 0
-    feed_pt('\r\r')
+    pt_input.send_text('\r\r')
     assert run(f'rollback {options} curse:molinari').output == dedent(
         """\
         ✓ curse:molinari
           updated 100005.97-Release to 100205.111-Release with new strategies:
             version_eq=None
         """
         if options == '--undo'
@@ -366,188 +385,188 @@
         ✓ curse:molinari
           updated 100005.97-Release to 100205.111-Release
         """
     )
 
 
 def test_reconcile__list_unreconciled(
-    pretend_install_molinari_and_run: C[[str], Result],
+    pretend_install_molinari_and_run: Run,
 ):
     assert (
         pretend_install_molinari_and_run('reconcile --list-unreconciled').output
         == (
             'unreconciled\n'  # fmt: skip
             '------------\n'
             'Molinari    \n'
         )
     )
 
 
 def test_reconcile_leftovers(
-    feed_pt: C[[str], None],
-    pretend_install_molinari_and_run: C[[str], Result],
+    pt_input: PipeInput,
+    pretend_install_molinari_and_run: Run,
 ):
-    feed_pt('sss')  # Skip
+    pt_input.send_text('sss')  # Skip
     assert pretend_install_molinari_and_run(
         'reconcile'
     ).output.endswith(
         'unreconciled\n'  # fmt: skip
         '------------\n'
         'Molinari    \n'
     )
 
 
 def test_reconcile__auto_reconcile(
-    pretend_install_molinari_and_run: C[[str], Result],
+    pretend_install_molinari_and_run: Run,
 ):
     assert pretend_install_molinari_and_run('reconcile --auto').output == dedent(
         """\
         ✓ github:p3lim-wow/molinari
           installed 100205.111-Release
         """
     )
 
 
 def test_reconcile__abort_interactive_reconciliation(
-    feed_pt: C[[str], None],
-    pretend_install_molinari_and_run: C[[str], Result],
+    pt_input: PipeInput,
+    pretend_install_molinari_and_run: Run,
 ):
-    feed_pt('\x03')  # ^C
+    pt_input.send_text('\x03')  # ^C
     assert pretend_install_molinari_and_run('reconcile').output.endswith('Aborted!\n')
 
 
 def test_reconcile__complete_interactive_reconciliation(
-    feed_pt: C[[str], None],
-    pretend_install_molinari_and_run: C[[str], Result],
+    pt_input: PipeInput,
+    pretend_install_molinari_and_run: Run,
 ):
-    feed_pt('\r\r')
+    pt_input.send_text('\ry')
     assert pretend_install_molinari_and_run('reconcile').output.endswith(
         dedent(
             """\
             ✓ github:p3lim-wow/molinari
               installed 100205.111-Release
             """
         )
     )
 
 
 def test_reconcile__reconciliation_complete(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('reconcile').output == 'No add-ons left to reconcile.\n'
 
 
 def test_reconcile__rereconcile(
-    feed_pt: C[[str], None],
-    install_molinari_and_run: C[[str], Result],
+    pt_input: PipeInput,
+    install_molinari_and_run: Run,
 ):
-    feed_pt('\r\r')
+    pt_input.send_text('\ry')
     assert install_molinari_and_run('reconcile --installed').output == dedent(
         """\
         ✓ curse:molinari
           removed
         ✓ github:p3lim-wow/molinari
           installed 100205.111-Release
         """
     )
 
 
 def test_reconcile__cannot_use_auto_with_installed(
-    run: C[[str], Result],
+    run: Run,
 ):
     result = run('reconcile --auto --installed')
     assert result.exit_code == 2
     assert 'Cannot use "--auto" with "--installed"' in result.output
 
 
 def test_search__no_results(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('search ∅').output == 'No results found.\n'
 
 
 def test_search__exit_without_selecting(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
 ):
-    feed_pt('\r')  # enter
+    pt_input.send_text('\r')  # enter
     assert run('search molinari').output == (
         'Nothing was selected; select add-ons with <space> and confirm by pressing <enter>.\n'
     )
 
 
 def test_search__exit_after_selection(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
 ):
-    feed_pt(' \rn')  # space, enter, "n"
+    pt_input.send_text(' \rn')  # space, enter, "n"
     assert run('search molinari').output == ''
 
 
 def test_search__install_one(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
 ):
-    feed_pt(' \r\r')  # space, enter, enter
+    pt_input.send_text(' \ry')  # space, enter, enter
     assert run('search molinari --source curse').output == dedent(
         """\
         ✓ curse:molinari
           installed 100205.111-Release
         """
     )
 
 
 def test_search__install_multiple_conflicting(
-    feed_pt: C[[str], None],
-    run: C[[str], Result],
+    pt_input: PipeInput,
+    run: Run,
 ):
-    feed_pt(' \x1b[B \r\r')  # space, arrow down, space, enter, enter
+    pt_input.send_text(' \x1b[B \ry')  # space, arrow down, space, enter, enter
     assert run('search molinari').output == dedent(
         """\
         ✓ github:p3lim-wow/molinari
           installed 100205.111-Release
         ✗ wowi:13188-molinari
           package folders conflict with installed package Molinari
             (github:388670)
         """
     )
 
 
 def test_changelog_output(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     output = (
         'curse:molinari:\n  Changes in 90200.82-Release:'
         if shutil.which('pandoc')
         else 'curse:molinari:\n  <h3>Changes in'
     )
     assert install_molinari_and_run('view-changelog curse:molinari').output.startswith(output)
 
 
 def test_changelog_output_no_convert(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     assert install_molinari_and_run(
         'view-changelog --no-convert curse:molinari'
     ).output.startswith('curse:molinari:\n  <h3>Changes in')
 
 
 def test_argless_changelog_output(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     output = (
         'curse:molinari:\n  Changes in 90200.82-Release:'
         if shutil.which('pandoc')
         else 'curse:molinari:\n  <h3>Changes in'
     )
     assert install_molinari_and_run('view-changelog').output.startswith(output)
 
 
 def test_argless_changelog_output_no_convert(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     assert install_molinari_and_run('view-changelog --no-convert').output.startswith(
         'curse:molinari:\n  <h3>Changes in'
     )
 
 
 @pytest.mark.parametrize(
@@ -557,53 +576,43 @@
         ('info foo', 0),
         ('reveal mol', 0),
         ('reveal foo', 1),
     ],
 )
 def test_exit_codes_with_substr_match(
     monkeypatch: pytest.MonkeyPatch,
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
     command: str,
     exit_code: int,
 ):
-    monkeypatch.setattr('instawow.cli.reveal_folder', lambda *_, **__: ...)
+    monkeypatch.setattr('instawow._utils.file.reveal_folder', lambda *_, **__: ...)
     assert install_molinari_and_run(command).exit_code == exit_code
 
 
 def test_can_list_with_substr_match(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     assert install_molinari_and_run('list mol').output == 'curse:molinari\n'
     assert install_molinari_and_run('list foo').output == ''
     assert install_molinari_and_run('list -f detailed mol').output.startswith('curse:molinari')
     (molinari,) = json.loads(install_molinari_and_run('list -f json mol').output)
     assert (molinari['source'], molinari['slug']) == ('curse', 'molinari')
 
 
 def test_json_export(
-    install_molinari_and_run: C[[str], Result],
+    install_molinari_and_run: Run,
 ):
     output = install_molinari_and_run('list -f json').output
     assert json.loads(output)[0]['name'] == 'Molinari'
 
 
-def test_list_sources(
-    run: C[[str], Result],
-):
-    json_converter = make_json_converter()
-
-    output = run('list-sources').output
-    source_metadata = json_converter.loads(output, list[SourceMetadata])
-    assert len(source_metadata) > 1
-
-
 def test_show_version(
-    run: C[[str], Result],
+    run: Run,
 ):
     assert run('--version').output == f'instawow, version {__version__}\n'
 
 
 def test_plugin_hook_command_can_be_invoked(
-    run: C[[str], Result],
+    run: Run,
 ):
     pytest.importorskip('instawow_test_plugin')
     assert run('plugins foo').output == 'success!\n'
```

### Comparing `instawow-4.0.0/tests/test_config.py` & `instawow-4.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_json_rpc_api.py` & `instawow-4.1.0/tests/test_json_rpc_api.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_matchers.py` & `instawow-4.1.0/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_pkg_archives.py` & `instawow-4.1.0/tests/test_pkg_archives.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_pkg_management.py` & `instawow-4.1.0/tests/test_pkg_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from aresponses import ResponsesMockServer
 
 from instawow import results as R
 from instawow.definitions import Defn, Strategy
 from instawow.pkg_management import PkgManager
 from instawow.pkg_models import Pkg
 
+from .fixtures.http import Route
+
 
 def test_auth_bound_resolvers_are_not_unloaded_if_tokens_set(
     iw_manager: PkgManager,
 ):
     assert {
         r.metadata.id for r in iw_manager.ctx.RESOLVERS if r.requires_access_token is not None
     }.issubset(iw_manager.ctx.resolvers)
@@ -167,18 +169,18 @@
 
 async def test_install_recognises_renamed_pkg_from_id(
     monkeypatch: pytest.MonkeyPatch,
     iw_aresponses: ResponsesMockServer,
     iw_manager: PkgManager,
 ):
     iw_aresponses.add(
-        'api.github.com',
-        '/repos/p3lim-wow/molinarifico',
-        'get',
-        iw_aresponses.Response(status=404),
+        **Route(
+            '//api.github.com/repos/p3lim-wow/molinarifico',
+            iw_aresponses.Response(status=404),
+        ).to_aresponses_add_args()
     )
 
     old_defn = Defn('github', 'p3lim-wow/molinari')
     new_defn = Defn('github', 'p3lim-wow/molinarifico')
 
     result = await iw_manager.install([old_defn], replace_folders=False)
     assert type(result[old_defn]) is R.PkgInstalled
```

### Comparing `instawow-4.0.0/tests/test_resolvers.py` & `instawow-4.1.0/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_source__curse.py` & `instawow-4.1.0/tests/test_source__curse.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_source__github.py` & `instawow-4.1.0/tests/test_source__github.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from __future__ import annotations
 
 import logging
 import re
 from io import BytesIO
+from typing import Literal
 from zipfile import ZipFile
 
 import aiohttp.hdrs
 import aiohttp.web
 import pytest
 from aresponses import ResponsesMockServer
 from yarl import URL
 
 from instawow._sources.github import GithubResolver
-from instawow.definitions import Defn
+from instawow.definitions import Defn, StrategyValues
 from instawow.manager_ctx import ManagerCtx
 from instawow.pkg_models import Pkg
 from instawow.results import PkgFilesMissing, PkgFilesNotMatching, PkgNonexistent
-from instawow.wow_installations import Flavour
+from instawow.wow_installations import Flavour, FlavourVersionRange
+
+from .fixtures.http import Route
 
 
 @pytest.fixture
 def github_resolver(
     iw_manager_ctx: ManagerCtx,
 ):
     return GithubResolver(iw_manager_ctx)
 
 
 zip_defn = Defn('github', '28/NoteworthyII')
 zip_addon_name = URL(zip_defn.alias).name
 
+packager_test_defn = Defn('github', 'nebularg/PackagerTest')
+
 
 ZIPS = {
     'flavoured-toc-only': {
         'toc_files': {
             '_Wrath': b'',
         },
         'flavours': {Flavour.Classic},
@@ -79,16 +84,16 @@
     return (addon.getvalue(), request.param['flavours'])
 
 
 @pytest.mark.parametrize(
     '_iw_mock_aiohttp_requests',
     [
         {
-            URL(f'//api.github.com/repos/{zip_defn.alias}'),
-            URL(f'//api.github.com/repos/{zip_defn.alias}/releases?per_page=10'),
+            f'//api.github.com/repos/{zip_defn.alias}',
+            f'//api.github.com/repos/{zip_defn.alias}/releases?per_page=10',
         }
     ],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'iw_config_values',
     Flavour,
@@ -105,19 +110,19 @@
             raise aiohttp.web.HTTPRequestRangeNotSatisfiable
 
         response = aiohttp.web.Response(body=addon)
         await response.prepare(request)
         return response
 
     iw_aresponses.add(
-        'api.github.com',
-        re.compile(r'^/repos(/[^/]*){2}/releases/assets/'),
-        'get',
-        handle_request,
-        repeat=iw_aresponses.INFINITY,
+        **Route(
+            '//api.github.com',
+            path_pattern=re.compile(r'^/repos(/[^/]*){2}/releases/assets/'),
+            response=handle_request,
+        ).to_aresponses_add_args()
     )
 
     addon, flavours = package_json_less_addon
     try:
         await github_resolver.resolve_one(zip_defn, None)
     except PkgFilesNotMatching:
         assert iw_manager_ctx.config.game_flavour not in flavours
@@ -138,26 +143,76 @@
     github_resolver: GithubResolver,
 ):
     defn = Defn('github', 'AdiAddons/AdiBags')
 
     with pytest.raises(PkgFilesMissing) as exc_info:
         await github_resolver.resolve_one(defn, None)
 
-    assert exc_info.value.message == 'release not found'
+    assert exc_info.value.message == 'no releases found'
 
 
 async def test_nonexistent_repo(
     github_resolver: GithubResolver,
 ):
     defn = Defn('github', 'layday/foobar')
 
     with pytest.raises(PkgNonexistent):
         await github_resolver.resolve_one(defn, None)
 
 
+@pytest.mark.parametrize(
+    '_iw_mock_aiohttp_requests',
+    [
+        {
+            f'//api.github.com/repos/{packager_test_defn.alias}',
+            f'//api.github.com/repos/{packager_test_defn.alias}/releases?per_page=10',
+        }
+    ],
+    indirect=True,
+)
+@pytest.mark.parametrize('any_flavour', [True, None])
+async def test_any_flavour_strategy(
+    iw_aresponses: ResponsesMockServer,
+    iw_manager_ctx: ManagerCtx,
+    github_resolver: GithubResolver,
+    any_flavour: Literal[True, None],
+):
+    opposite_flavour = next(f for f in Flavour if f is not iw_manager_ctx.config.game_flavour)
+    opposite_interface = next(
+        n for r in opposite_flavour.to_flavour_keyed_enum(FlavourVersionRange).value for n in r
+    )
+
+    iw_aresponses.add(
+        **Route(
+            '//api.github.com',
+            path_pattern=re.compile(r'^/repos/nebularg/PackagerTest/releases/assets/'),
+            response={
+                'releases': [
+                    {
+                        'filename': 'TestGit-v1.9.7.zip',
+                        'nolib': False,
+                        'metadata': [
+                            {
+                                'flavor': opposite_flavour,
+                                'interface': opposite_interface,
+                            }
+                        ],
+                    }
+                ]
+            },
+        ).to_aresponses_add_args()
+    )
+    defn = Defn(
+        'github', 'nebularg/PackagerTest', strategies=StrategyValues(any_flavour=any_flavour)
+    )
+
+    results = await github_resolver.resolve([defn])
+    assert type(results[defn]) is (Pkg if any_flavour else PkgFilesNotMatching)
+
+
 async def test_changelog_is_data_url(
     github_resolver: GithubResolver,
 ):
     defn = Defn('github', 'p3lim-wow/Molinari')
 
     result = await github_resolver.resolve_one(defn, None)
     assert result.changelog_url.startswith('data:,')
@@ -172,53 +227,53 @@
     ],
     indirect=('iw_config_values',),
 )
 @pytest.mark.parametrize(
     '_iw_mock_aiohttp_requests',
     [
         {
-            URL('//api.github.com/repos/nebularg/PackagerTest'),
-            URL('//api.github.com/repos/nebularg/PackagerTest/releases?per_page=10'),
+            f'//api.github.com/repos/{packager_test_defn.alias}',
+            f'//api.github.com/repos/{packager_test_defn.alias}/releases?per_page=10',
         }
     ],
     indirect=True,
 )
 async def test_mismatched_release_is_skipped_and_logged(
     caplog: pytest.LogCaptureFixture,
     iw_aresponses: ResponsesMockServer,
+    iw_manager_ctx: ManagerCtx,
     github_resolver: GithubResolver,
     flavor: str,
     interface: int,
 ):
     iw_aresponses.add(
-        'api.github.com',
-        re.compile(r'^/repos/nebularg/PackagerTest/releases/assets/'),
-        'GET',
-        {
-            'releases': [
-                {
-                    'filename': 'TestGit-v1.9.7.zip',
-                    'nolib': False,
-                    'metadata': [{'flavor': flavor, 'interface': interface}],
-                }
-            ]
-        },
+        **Route(
+            '//api.github.com',
+            path_pattern=re.compile(r'^/repos/nebularg/PackagerTest/releases/assets/'),
+            response={
+                'releases': [
+                    {
+                        'filename': 'TestGit-v1.9.7.zip',
+                        'nolib': False,
+                        'metadata': [{'flavor': flavor, 'interface': interface}],
+                    }
+                ]
+            },
+        ).to_aresponses_add_args()
     )
 
-    defn = Defn('github', 'nebularg/PackagerTest')
-
     with pytest.raises(PkgFilesNotMatching):
-        await github_resolver.resolve_one(defn, None)
+        await github_resolver.resolve_one(packager_test_defn, None)
 
-    (log_record,) = caplog.record_tuples
-    assert log_record == (
+    assert (
         'instawow._sources.github',
         logging.INFO,
-        f'interface number "{interface}" and flavor "{flavor}" mismatch',
-    )
+        f'flavor and interface mismatch: {interface} not found in '
+        f'{[iw_manager_ctx.config.game_flavour.to_flavour_keyed_enum(FlavourVersionRange).value]}',
+    ) in caplog.record_tuples
 
 
 @pytest.mark.parametrize(
     ('url', 'extracted_alias'),
     [
         (
             'https://github.com/AdiAddons/AdiButtonAuras',
```

### Comparing `instawow-4.0.0/tests/test_source__tukui.py` & `instawow-4.1.0/tests/test_source__tukui.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_source__wowi.py` & `instawow-4.1.0/tests/test_source__wowi.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_wa_updater.py` & `instawow-4.1.0/tests/test_wa_updater.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_wa_updater_parser.py` & `instawow-4.1.0/tests/test_wa_updater_parser.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/test_wow_installations.py` & `instawow-4.1.0/tests/test_wow_installations.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,19 +17,36 @@
 
 
 def test_can_convert_between_flavour_keyed_enum_and_flavour():
     class Foo(Enum):
         Retail = 1
         VanillaClassic = 2
         Classic = 3
+        CataclysmClassic = 4
 
     assert Flavour.from_flavour_keyed_enum(Foo.Retail) is Flavour.Retail
     assert Flavour.Retail.to_flavour_keyed_enum(Foo) is Foo.Retail
 
 
+@pytest.mark.parametrize('flavour', list(Flavour))
+@pytest.mark.parametrize('affine', [True, False])
+def test_flavour_groups_vary_by_flavour_and_affinity(
+    flavour: Flavour,
+    affine: bool,
+):
+    flavour_groups = flavour.get_flavour_groups(affine)
+    if affine:
+        if flavour is Flavour.CataclysmClassic:
+            assert flavour_groups == [(flavour, Flavour.Classic), None]
+        else:
+            assert flavour_groups == [(flavour,), None]
+    else:
+        assert flavour_groups == [(flavour,)]
+
+
 def test_can_extract_flavour_from_version_number():
     assert FlavourVersionRange.from_version(95000) is FlavourVersionRange.Retail
     assert FlavourVersionRange.from_version(34000) is FlavourVersionRange.Classic
     assert FlavourVersionRange.from_version(12300) is FlavourVersionRange.VanillaClassic
 
 
 def test_can_extract_flavour_from_version_string():
@@ -49,15 +66,15 @@
     [
         (
             'wowzerz/_classic_/Interface/AddOns',
             Flavour.Classic,
         ),
         (
             '/foo/bar/_classic_ptr_/Interface/AddOns',
-            Flavour.Classic,
+            Flavour.CataclysmClassic,
         ),
         (
             '_classic_era_/Interface/AddOns',
             Flavour.VanillaClassic,
         ),
         (
             '_classic_era_ptr_/Interface/AddOns',
```

### Comparing `instawow-4.0.0/tests/fixtures/http/__init__.py` & `instawow-4.1.0/tests/fixtures/http/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # pyright: strict
 
 from __future__ import annotations
 
+import importlib.resources
 import json
 import re
-from collections.abc import Callable
+from collections.abc import Awaitable, Callable
 from functools import cache
 from io import BytesIO
-from pathlib import Path
 from typing import Any
 from zipfile import ZipFile
 
-from aiohttp.web import Response
-from attr import frozen
+import attrs
+from aiohttp.web import Request, Response
 from yarl import URL
 
 from instawow import __version__
 
-_HERE = Path(__file__).parent
-
 _match_any = re.compile(r'.*')
 
 
 def _load_fixture(filename: str):
-    return (_HERE / filename).read_bytes()
+    return (importlib.resources.files(__spec__.parent) / filename).read_bytes()
 
 
 def _load_json_fixture(filename: str):
     return json.loads(_load_fixture(filename))
 
 
 @cache
@@ -36,18 +34,24 @@
     with ZipFile(buffer, 'w') as file:
         for folder in folders:
             file.writestr(f'{folder}/{folder}.toc', b'')
 
     return buffer.getvalue()
 
 
-@frozen
+@attrs.frozen
 class Route:
-    url: URL
-    response: Callable[[], Response] | dict[str, Any] | str
+    url: URL = attrs.field(converter=URL)
+    response: (
+        Response
+        | Callable[[Request], Response]
+        | Callable[[Request], Awaitable[Response]]
+        | dict[str, Any]
+        | str
+    )
     path_pattern: re.Pattern[str] | None = None
     method: str = 'GET'
     body_pattern: re.Pattern[str] | None = None
     match_querystring: bool = False
     repeat: float = float('inf')
     case_insensitive: bool = False
 
@@ -64,111 +68,109 @@
         return {
             'host_pattern': self.url.host,
             'path_pattern': self._make_path_pattern(),
             'method_pattern': self.method,
             'body_pattern': _match_any if self.body_pattern is None else self.body_pattern,
             'match_querystring': self.match_querystring,
             'repeat': self.repeat,
-            'response': self.response() if callable(self.response) else self.response,
+            'response': self.response,
         }
 
 
 def _make_route_dict_entry(route: Route):
     return (route.url, route)
 
 
 ROUTES = dict(
     map(
         _make_route_dict_entry,
         [
             Route(
-                URL('//pypi.org/pypi/instawow/json'),
+                '//pypi.org/pypi/instawow/json',
                 {'info': {'version': __version__}},
             ),
             Route(
-                URL(
-                    '//raw.githubusercontent.com/layday/instawow-data/data/base-catalogue-v7.compact.json'
-                ),
+                '//raw.githubusercontent.com/layday/instawow-data/data/base-catalogue-v7.compact.json',
                 _load_json_fixture('base-catalogue-v7.compact.json'),
             ),
             Route(
-                URL('//api.curseforge.com/v1/mods'),
+                '//api.curseforge.com/v1/mods',
                 _load_json_fixture('curse-addon--all.json'),
                 method='POST',
             ),
             Route(
-                URL('//api.curseforge.com/v1/mods/search?gameId=1&slug=molinari'),
+                '//api.curseforge.com/v1/mods/search?gameId=1&slug=molinari',
                 _load_json_fixture('curse-addon-slug-search.json'),
                 match_querystring=True,
             ),
             Route(
-                URL('//api.curseforge.com/v1/mods/20338/files'),
+                '//api.curseforge.com/v1/mods/20338/files',
                 _load_json_fixture('curse-addon-files.json'),
             ),
             Route(
-                URL('//api.curseforge.com/v1/mods/20338/files/{id}/changelog'),
+                '//api.curseforge.com/v1/mods/20338/files/{id}/changelog',
                 _load_json_fixture('curse-addon-changelog.json'),
                 path_pattern=re.compile(r'^/v1/mods/20338/files/(\d+)/changelog$'),
             ),
             Route(
-                URL('//edge.forgecdn.net'),
-                lambda: Response(body=_make_addon_zip('Molinari')),
+                '//edge.forgecdn.net',
+                lambda _: Response(body=_make_addon_zip('Molinari')),
                 path_pattern=_match_any,
             ),
             Route(
-                URL('//api.mmoui.com/v3/game/WOW/filelist.json'),
+                '//api.mmoui.com/v3/game/WOW/filelist.json',
                 _load_json_fixture('wowi-filelist.json'),
             ),
             Route(
-                URL('//api.mmoui.com/v3/game/WOW/filedetails/{id}.json'),
+                '//api.mmoui.com/v3/game/WOW/filedetails/{id}.json',
                 _load_json_fixture('wowi-filedetails.json'),
                 path_pattern=re.compile(r'^/v3/game/WOW/filedetails/(\d*)\.json$'),
             ),
             Route(
-                URL('//cdn.wowinterface.com'),
-                lambda: Response(body=_make_addon_zip('Molinari')),
+                '//cdn.wowinterface.com',
+                lambda _: Response(body=_make_addon_zip('Molinari')),
                 path_pattern=_match_any,
             ),
             Route(
-                URL('//api.tukui.org/v1/addon/tukui'),
+                '//api.tukui.org/v1/addon/tukui',
                 _load_json_fixture('tukui-ui--tukui.json'),
             ),
             Route(
-                URL('//api.tukui.org/v1/addon/elvui'),
+                '//api.tukui.org/v1/addon/elvui',
                 _load_json_fixture('tukui-ui--elvui.json'),
             ),
             Route(
-                URL('//api.tukui.org/v1/download/'),
-                lambda: Response(body=_make_addon_zip('Tukui')),
+                '//api.tukui.org/v1/download/',
+                lambda _: Response(body=_make_addon_zip('Tukui')),
                 path_pattern=re.compile(r'^/v1/download/'),
             ),
             Route(
-                URL('//api.github.com/repos/nebularg/PackagerTest'),
+                '//api.github.com/repos/nebularg/PackagerTest',
                 _load_json_fixture('github-repo-release-json.json'),
             ),
             Route(
-                URL('//api.github.com/repos/nebularg/PackagerTest/releases?per_page=10'),
+                '//api.github.com/repos/nebularg/PackagerTest/releases?per_page=10',
                 _load_json_fixture('github-release-release-json.json'),
                 match_querystring=True,
             ),
             Route(
-                URL('//api.github.com/repos/nebularg/PackagerTest/releases/assets/37156458'),
+                '//api.github.com/repos/nebularg/PackagerTest/releases/assets/37156458',
                 _load_json_fixture('github-release-release-json-release-json.json'),
             ),
             Route(
-                URL('//api.github.com/repositories/388670'),
+                '//api.github.com/repositories/388670',
                 _load_json_fixture('github-repo-molinari.json'),
             ),
             Route(
-                URL('//api.github.com/repos/p3lim-wow/Molinari'),
+                '//api.github.com/repos/p3lim-wow/Molinari',
                 _load_json_fixture('github-repo-molinari.json'),
                 case_insensitive=True,
             ),
             Route(
-                URL('//api.github.com/repos/p3lim-wow/Molinari/releases?per_page=10'),
+                '//api.github.com/repos/p3lim-wow/Molinari/releases?per_page=10',
                 _load_json_fixture('github-release-molinari.json'),
                 case_insensitive=True,
                 match_querystring=True,
             ),
             Route(
                 URL(
                     next(
@@ -177,55 +179,55 @@
                         if a['name'] == 'release.json'
                     )
                 ).with_scheme(''),
                 _load_json_fixture('github-release-molinari-release-json.json'),
                 case_insensitive=True,
             ),
             Route(
-                URL('//api.github.com/repos/AdiAddons/AdiBags'),
+                '//api.github.com/repos/AdiAddons/AdiBags',
                 _load_json_fixture('github-repo-no-releases.json'),
             ),
             Route(
-                URL('//api.github.com/repos/AdiAddons/AdiBags/releases?per_page=10'),
-                lambda: Response(body=b'', status=404),
+                '//api.github.com/repos/AdiAddons/AdiBags/releases?per_page=10',
+                lambda _: Response(body=b'', status=404),
                 match_querystring=True,
             ),
             Route(
-                URL('//api.github.com/repos/AdiAddons/AdiButtonAuras/releases/tags/2.0.19'),
+                '//api.github.com/repos/AdiAddons/AdiButtonAuras/releases/tags/2.0.19',
                 _load_json_fixture('github-release-no-assets.json'),
             ),
             Route(
-                URL('//api.github.com/repos/layday/foobar'),
-                lambda: Response(body=b'', status=404),
+                '//api.github.com/repos/layday/foobar',
+                lambda _: Response(body=b'', status=404),
             ),
             Route(
-                URL('//api.github.com/repos/{x}/{y}/releases/asssets/{z}'),
-                lambda: Response(body=_make_addon_zip('Molinari')),
+                '//api.github.com/repos/{x}/{y}/releases/asssets/{z}',
+                lambda _: Response(body=_make_addon_zip('Molinari')),
                 path_pattern=re.compile(r'^/repos(/[^/]*){2}/releases/assets/'),
             ),
             Route(
-                URL('//github.com/login/device/code'),
+                '//github.com/login/device/code',
                 _load_json_fixture('github-oauth-login-device-code.json'),
                 method='POST',
             ),
             Route(
-                URL('//github.com/login/oauth/access_token'),
+                '//github.com/login/oauth/access_token',
                 _load_json_fixture('github-oauth-login-access-token.json'),
                 method='POST',
             ),
             Route(
-                URL('//api.github.com/repos/28/NoteworthyII'),
+                '//api.github.com/repos/28/NoteworthyII',
                 _load_json_fixture('github-repo-no-release-json.json'),
             ),
             Route(
-                URL('//api.github.com/repos/28/NoteworthyII/releases?per_page=10'),
+                '//api.github.com/repos/28/NoteworthyII/releases?per_page=10',
                 _load_json_fixture('github-release-no-release-json.json'),
                 match_querystring=True,
             ),
             Route(
-                URL('//addons.wago.io/api/external/addons/_match'),
+                '//addons.wago.io/api/external/addons/_match',
                 _load_json_fixture('wago-match-addons.json'),
                 method='POST',
             ),
         ],
     )
 )
```

### Comparing `instawow-4.0.0/tests/fixtures/http/base-catalogue-v7.compact.json` & `instawow-4.1.0/tests/fixtures/http/base-catalogue-v7.compact.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/curse-addon--all.json` & `instawow-4.1.0/tests/fixtures/http/curse-addon--all.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/curse-addon-files.json` & `instawow-4.1.0/tests/fixtures/http/curse-addon-files.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/curse-addon-slug-search.json` & `instawow-4.1.0/tests/fixtures/http/curse-addon-slug-search.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-release-molinari.json` & `instawow-4.1.0/tests/fixtures/http/github-release-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-release-no-assets.json` & `instawow-4.1.0/tests/fixtures/http/github-release-no-assets.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-release-no-release-json.json` & `instawow-4.1.0/tests/fixtures/http/github-release-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-release-release-json.json` & `instawow-4.1.0/tests/fixtures/http/github-release-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-repo-molinari.json` & `instawow-4.1.0/tests/fixtures/http/github-repo-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-repo-no-release-json.json` & `instawow-4.1.0/tests/fixtures/http/github-repo-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-repo-no-releases.json` & `instawow-4.1.0/tests/fixtures/http/github-repo-no-releases.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/github-repo-release-json.json` & `instawow-4.1.0/tests/fixtures/http/github-repo-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/regen.sh` & `instawow-4.1.0/tests/fixtures/http/regen.sh`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/tukui-ui--elvui.json` & `instawow-4.1.0/tests/fixtures/http/tukui-ui--elvui.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/tukui-ui--tukui.json` & `instawow-4.1.0/tests/fixtures/http/tukui-ui--tukui.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/wago-match-addons.json` & `instawow-4.1.0/tests/fixtures/http/wago-match-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/wowi-filedetails.json` & `instawow-4.1.0/tests/fixtures/http/wowi-filedetails.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/fixtures/http/wowi-filelist.json` & `instawow-4.1.0/tests/fixtures/http/wowi-filelist.json`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/tests/plugin/instawow_test_plugin.py` & `instawow-4.1.0/tests/plugin/instawow_test_plugin.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/_plugin.py` & `instawow-4.1.0/instawow-gui/src/instawow_gui/_plugin.py`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/app.py` & `instawow-4.1.0/instawow-gui/src/instawow_gui/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from typing import cast
 
 import anyio.from_thread
 import anyio.to_thread
 import toga
 import toga.constants
 import toga.style.pack
-from loguru import logger
 
-from instawow.utils import StrEnum
+from instawow._logging import logger
+from instawow._utils.compat import StrEnum
 
 from . import json_rpc_server
 
 
 class _TogaSimulateKeypressAction(StrEnum):
     ToggleSearchFilter = 'toggleSearchFilter'
     ActivateViewInstalled = 'activateViewInstalled'
```

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/json_rpc_server.py` & `instawow-4.1.0/instawow-gui/src/instawow_gui/json_rpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import contextvars
+import importlib.resources
 import json
 import os
 from collections.abc import Awaitable, Callable, Iterator, Set
 from contextlib import AsyncExitStack, contextmanager
 from datetime import datetime
 from functools import partial
 from itertools import chain
@@ -17,42 +18,37 @@
 import aiohttp.web
 import anyio.from_thread
 import attrs
 import cattrs
 import cattrs.preconf.json
 import click
 import iso8601
-import sqlalchemy as sa
 from aiohttp_rpc import JsonRpcMethod
 from aiohttp_rpc import middlewares as rpc_middlewares
 from aiohttp_rpc.errors import InvalidParams, ServerError
 from aiohttp_rpc.server import WsJsonRpcServer
-from loguru import logger
 from typing_extensions import ParamSpec, TypedDict
 from yarl import URL
 
-from instawow import __version__, matchers, pkg_db, pkg_models
+from instawow import __version__, matchers, pkg_models
 from instawow import results as R
+from instawow._logging import logger
+from instawow._utils.aio import run_in_thread
+from instawow._utils.compat import StrEnum
+from instawow._utils.file import reveal_folder
+from instawow._utils.iteration import WeakValueDefaultDictionary, uniq
 from instawow._version_check import is_outdated
 from instawow.catalogue.cataloguer import ComputedCatalogueEntry
 from instawow.catalogue.search import search
 from instawow.config import GlobalConfig, ProfileConfig, SecretStr, config_converter
 from instawow.definitions import Defn, SourceMetadata
 from instawow.github_auth import get_codes, poll_for_access_token
 from instawow.http import TraceRequestCtx, init_web_client
 from instawow.manager_ctx import ManagerCtx, contextualise
 from instawow.pkg_management import PkgDownloadTraceRequestCtx, PkgManager, bucketise_results
-from instawow.utils import (
-    StrEnum,
-    WeakValueDefaultDictionary,
-    read_resource_as_text,
-    reveal_folder,
-    uniq,
-)
-from instawow.utils import run_in_thread as t
 from instawow.wow_installations import Flavour, infer_flavour_from_addon_dir
 
 from . import frontend
 
 _T = TypeVar('_T')
 _P = ParamSpec('_P')
 _ManagerBoundCoroFn: TypeAlias = Callable[Concatenate[PkgManager, _P], Awaitable[_T]]
@@ -131,21 +127,21 @@
     try:
         yield
     except BaseException as exc:
         logger.info(f'invalid request: {(values, exc)}')
         raise error_class(data=list(_transform_validation_errors(exc))) from exc
 
 
-@t
+@run_in_thread
 def _read_global_config() -> GlobalConfig:
     with _reraise_validation_errors(_ConfigError):
         return GlobalConfig.read().ensure_dirs()
 
 
-@t
+@run_in_thread
 def _read_config(global_config: GlobalConfig, profile: str) -> ProfileConfig:
     with _reraise_validation_errors(_ConfigError):
         return ProfileConfig.read(global_config, profile).ensure_dirs()
 
 
 _methods: list[tuple[str, type[BaseParams]]] = []
 
@@ -202,15 +198,15 @@
                 )
                 if self.infer_game_flavour:
                     config = attrs.evolve(
                         config,
                         game_flavour=infer_flavour_from_addon_dir(config.addon_dir)
                         or Flavour.Retail,
                     )
-                await t(config.write)()
+                await run_in_thread(config.write)()
 
             # Unload the corresponding ``Manager`` instance for the
             # config to be reloaded on the next request
             managers.unload_profile(config.profile)
 
             return config
 
@@ -221,24 +217,24 @@
         return await _read_config(managers.global_config, self.profile)
 
 
 @_register_method('config/delete_profile')
 class DeleteProfileConfigParams(_ProfileParamMixin, BaseParams):
     async def respond(self, managers: _ManagersManager) -> None:
         async def delete_profile(manager: PkgManager):
-            await t(manager.ctx.config.delete)()
+            await run_in_thread(manager.ctx.config.delete)()
             managers.unload_profile(self.profile)
 
         await managers.run(self.profile, delete_profile)
 
 
 @_register_method('config/list_profiles')
 class ListProfilesParams(BaseParams):
     async def respond(self, managers: _ManagersManager) -> list[str]:
-        return await t(list[str])(managers.global_config.iter_profiles())
+        return await run_in_thread(list[str])(managers.global_config.iter_profiles())
 
 
 @_register_method('config/update_global')
 class UpdateGlobalConfigParams(BaseParams):
     access_tokens: dict[str, str | None]
 
     async def respond(self, managers: _ManagersManager) -> GlobalConfig:
@@ -296,22 +292,18 @@
 
 @_register_method('list')
 class ListInstalledParams(_ProfileParamMixin, BaseParams):
     async def respond(self, managers: _ManagersManager) -> list[pkg_models.Pkg]:
         manager = await managers.get_manager(self.profile)
 
         with manager.ctx.database.connect() as connection:
-            installed_pkgs = (
-                connection.execute(
-                    sa.select(pkg_db.pkg).order_by(sa.func.lower(pkg_db.pkg.c.name))
-                )
-                .mappings()
-                .all()
-            )
-            return [manager.build_pkg_from_row_mapping(connection, p) for p in installed_pkgs]
+            return [
+                manager.build_pkg_from_row_mapping(connection, p)
+                for p in connection.execute('SELECT * FROM pkg ORDER BY lower(name)')
+            ]
 
 
 @_register_method('search')
 class SearchParams(_ProfileParamMixin, BaseParams):
     search_terms: str
     limit: int
     sources: set[str]
@@ -448,15 +440,15 @@
 @_register_method('reconcile')
 class ReconcileParams(_ProfileParamMixin, BaseParams):
     matcher: str
 
     async def respond(self, managers: _ManagersManager) -> list[AddonMatch]:
         manager = await managers.get_manager(self.profile)
 
-        leftovers = await t(matchers.get_unreconciled_folders)(manager.ctx)
+        leftovers = await run_in_thread(matchers.get_unreconciled_folders)(manager.ctx)
 
         match_groups = await matchers.DEFAULT_MATCHERS[self.matcher](
             manager.ctx, leftovers=leftovers
         )
 
         resolved_defns = await manager.resolve(uniq(d for _, b in match_groups for d in b))
         pkgs, _ = bucketise_results(resolved_defns.items())
@@ -483,19 +475,15 @@
 class GetReconcileInstalledCandidatesParams(_ProfileParamMixin, BaseParams):
     async def respond(self, managers: _ManagersManager) -> list[ReconcileInstalledCandidate]:
         manager = await managers.get_manager(self.profile)
 
         with manager.ctx.database.connect() as connection:
             installed_pkgs = [
                 manager.build_pkg_from_row_mapping(connection, p)
-                for p in connection.execute(
-                    sa.select(pkg_db.pkg).order_by(sa.func.lower(pkg_db.pkg.c.name))
-                )
-                .mappings()
-                .all()
+                for p in connection.execute('SELECT * FROM pkg ORDER BY lower(name)')
             ]
 
         defn_groups = await managers.run(
             self.profile, partial(PkgManager.find_equivalent_pkg_defns, pkgs=installed_pkgs)
         )
         resolved_defns = await managers.run(
             self.profile,
@@ -660,15 +648,15 @@
 
     async def update_global_config(
         self, update_cb: Callable[[GlobalConfig], GlobalConfig]
     ) -> GlobalConfig:
         async with self.locks[_LOCK_PREFIX, _LockOperation.UpdateGlobalConfig]:
             with _reraise_validation_errors(_ConfigError):
                 self.global_config = update_cb(self.global_config)
-                await t(self.global_config.write)()
+                await run_in_thread(self.global_config.write)()
 
             self._unload_all_profiles()
 
             return self.global_config
 
     async def run(self, profile: str, coro_fn: _ManagerBoundCoroFn[..., _T]) -> _T:
         try:
@@ -739,24 +727,26 @@
             self._github_auth_flow_task.cancel()
 
 
 async def create_app(toga_handle: tuple[Any, anyio.from_thread.BlockingPortal] | None = None):
     if toga_handle:
         _toga_handle.set(toga_handle)
 
+    frontend_resources = importlib.resources.files(frontend)
+
     managers = _ManagersManager()
 
     async def managers_listen(app: aiohttp.web.Application):
         async with managers:
             yield
 
     async def get_index(request: aiohttp.web.Request):
         return aiohttp.web.Response(
             content_type='text/html',
-            text=read_resource_as_text(frontend, 'index.html'),
+            text=frontend_resources.joinpath('index.html').read_text(),
         )
 
     async def get_static_file(request: aiohttp.web.Request):
         filename = request.path.lstrip('/')
 
         if filename.endswith('.js'):
             content_type = 'application/javascript'
@@ -765,15 +755,15 @@
         elif filename.endswith('.css'):
             content_type = 'text/css'
         else:
             raise aiohttp.web.HTTPNotFound
 
         return aiohttp.web.Response(
             content_type=content_type,
-            text=read_resource_as_text(frontend, filename),
+            text=frontend_resources.joinpath(filename).read_text(),
         )
 
     def json_serialize(value: dict[str, Any]):
         return json.dumps(_converter.unstructure(value))
 
     rpc_server = WsJsonRpcServer(
         json_serialize=json_serialize,
```

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/assets/index-BzfSzUDv.css` & `instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/assets/index-BzfSzUDv.css`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/frontend/assets/index-DqShBAqA.js` & `instawow-4.1.0/instawow-gui/src/instawow_gui/frontend/assets/index-DqShBAqA.js`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.icns` & `instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.icns`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.ico` & `instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.ico`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/instawow-gui/src/instawow_gui/resources/instawow_gui.png` & `instawow-4.1.0/instawow-gui/src/instawow_gui/resources/instawow_gui.png`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/COPYING` & `instawow-4.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `instawow-4.0.0/README.rst` & `instawow-4.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 You can install multiple add-ons directly from search.
 
 Install strategies
 ~~~~~~~~~~~~~~~~~~
 
 Add-ons take a number of options which determine how they are resolved:
 
-- ``any_flavour`` to ignore game version compatibility
+- ``any_flavour`` to ignore game version compatibility by prioriting "affine" game versions
 - ``any_release_type`` to ignore add-on stability
 - ``version_eq=[VERSION]`` to install a specific add-on version
 
 In the CLI, you can pass strategies in the fragment portion of the add-on URI,
 separated by a comma, e.g. ``instawow install curse:molinari#any_release_type,any_flavour``.
 Strategies are respected by ``install`` and ``update``.  To reset an add-on's strategies on update,
 you can pass a ``=`` fragment, e.g. ``instawow update curse:molinari#=``.
```

### Comparing `instawow-4.0.0/pyproject.toml` & `instawow-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 description = "World of Warcraft add-on manager"
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 authors = [{ name = "layday", email = "layday@protonmail.com" }]
 urls."homepage" = "http://github.com/layday/instawow"
 
 dependencies = [
-  "aiohttp >= 3.9.3, < 4",
+  "aiohttp >= 3.9.5, < 4",
   "aiohttp-client-cache >= 0.9.1",
   "attrs >= 23.2.0",
   "cattrs >= 23.2.3",
   "click >= 8.1.6",
   "diskcache >= 5.6.3",
   "iso8601 >= 1.0.2",
   "loguru >= 0.7.2",
   "packaging >= 23.2",
   "pluggy >= 1.4.0",
   "prompt-toolkit >= 3.0.29",
-  "questionary >= 2",
   "rapidfuzz >= 3.6.1",
-  "sqlalchemy >= 2.0.21",
   "truststore >= 0.7.0",
   "typing-extensions >= 4.6.0",
   "yarl >= 1.9.2",
 ]
 optional-dependencies."gui" = [
   "aiohttp-rpc >= 1.0.0",
   "anyio >= 4.3.0",
```

### Comparing `instawow-4.0.0/PKG-INFO` & `instawow-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.3
 Name: instawow
-Version: 4.0.0
+Version: 4.1.0
 Summary: World of Warcraft add-on manager
 Project-URL: homepage, http://github.com/layday/instawow
 Author-email: layday <layday@protonmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: COPYING
 Requires-Python: >=3.10
 Requires-Dist: aiohttp-client-cache>=0.9.1
-Requires-Dist: aiohttp<4,>=3.9.3
+Requires-Dist: aiohttp<4,>=3.9.5
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: cattrs>=23.2.3
 Requires-Dist: click>=8.1.6
 Requires-Dist: diskcache>=5.6.3
 Requires-Dist: iso8601>=1.0.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: packaging>=23.2
 Requires-Dist: pluggy>=1.4.0
 Requires-Dist: prompt-toolkit>=3.0.29
-Requires-Dist: questionary>=2
 Requires-Dist: rapidfuzz>=3.6.1
-Requires-Dist: sqlalchemy>=2.0.21
 Requires-Dist: truststore>=0.7.0
 Requires-Dist: typing-extensions>=4.6.0
 Requires-Dist: yarl>=1.9.2
 Provides-Extra: gui
 Requires-Dist: aiohttp-rpc>=1.0.0; extra == 'gui'
 Requires-Dist: anyio>=4.3.0; extra == 'gui'
 Requires-Dist: toga>=0.4.2; extra == 'gui'
@@ -132,15 +130,15 @@
 You can install multiple add-ons directly from search.
 
 Install strategies
 ~~~~~~~~~~~~~~~~~~
 
 Add-ons take a number of options which determine how they are resolved:
 
-- ``any_flavour`` to ignore game version compatibility
+- ``any_flavour`` to ignore game version compatibility by prioriting "affine" game versions
 - ``any_release_type`` to ignore add-on stability
 - ``version_eq=[VERSION]`` to install a specific add-on version
 
 In the CLI, you can pass strategies in the fragment portion of the add-on URI,
 separated by a comma, e.g. ``instawow install curse:molinari#any_release_type,any_flavour``.
 Strategies are respected by ``install`` and ``update``.  To reset an add-on's strategies on update,
 you can pass a ``=`` fragment, e.g. ``instawow update curse:molinari#=``.
```

