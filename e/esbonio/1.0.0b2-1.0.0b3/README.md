# Comparing `tmp/esbonio-1.0.0b2.tar.gz` & `tmp/esbonio-1.0.0b3.tar.gz`

## Comparing `esbonio-1.0.0b2.tar` & `esbonio-1.0.0b3.tar`

### file list

```diff
@@ -1,90 +1,100 @@
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/__main__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/__main__.py
--rw-r--r--   0        0        0    15079 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/_configuration.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/cli.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/events.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/feature.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/py.typed
--rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/server.py
--rw-r--r--   0        0        0    11175 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/setup.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/testing.py
--rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/log.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/directives/__init__.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/directives/completion.py
--rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/preview_manager/__init__.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/preview_manager/webview.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/__init__.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/manager.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/project_manager/project.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client_subprocess.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/config.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/manager.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/diagnostics.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/directives.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/server/features/sphinx_support/symbols.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/__main__.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/app.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/config.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/database.py
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/log.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/patches.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/py.typed
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/server.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/transforms.py
--rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/types.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/util.py
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/__init__.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/diagnostics.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/directives.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/files.py
--rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/symbols.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/esbonio/sphinx_agent/static/webview.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/conftest.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_option_pattern.txt
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_pattern.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/doctests/example_directive_substitution_pattern.txt
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/conftest.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_diagnostics.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_directives.py
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_e2e_symbols.py
--rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/e2e/test_sphinx_manager.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/conftest.py
--rw-r--r--   0        0        0    13646 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/test_configuration.py
--rw-r--r--   0        0        0    19841 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/test_patterns.py
--rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_directive_completion.py
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_logging.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/server/features/test_sphinx_config.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/conftest.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_app.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_build.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_create_app.py
--rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_unit.py
--rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/test_sa_uri_class.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_database.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_diagnostics.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/LICENSE
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/README.md
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/conf.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/demo_myst.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/demo_rst.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/index.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/pyproject.toml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/diagnostics.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/directives.md
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/myst/symbols.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/diagnostics.rst
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/directives.rst
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo/rst/symbols.rst
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo-error/conf.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/tests/workspaces/demo-error-build/conf.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/hatch.toml
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 esbonio-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/__main__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/__main__.py
+-rw-r--r--   0        0        0    15079 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/_configuration.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/cli.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/events.py
+-rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/feature.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/py.typed
+-rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/server.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/setup.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/testing.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/log.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/directives/__init__.py
+-rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/directives/completion.py
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/preview_manager/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/preview_manager/config.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/preview_manager/preview.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/preview_manager/webview.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/project_manager/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/project_manager/manager.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/project_manager/project.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/roles/__init__.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/roles/completion.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/client.py
+-rw-r--r--   0        0        0    11459 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/client_subprocess.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/config.py
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/manager.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_support/diagnostics.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_support/directives.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_support/roles.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/server/features/sphinx_support/symbols.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/__main__.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/app.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/config.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/database.py
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/log.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/patches.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/py.typed
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/server.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/transforms.py
+-rw-r--r--   0        0        0    21027 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/types.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/util.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/__init__.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/diagnostics.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/directives.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/files.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/roles.py
+-rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/symbols.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/esbonio/sphinx_agent/static/webview.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/conftest.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/doctests/example_directive_option_pattern.txt
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/doctests/example_directive_pattern.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/doctests/example_directive_substitution_pattern.txt
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/conftest.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/test_e2e_diagnostics.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/test_e2e_directives.py
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/test_e2e_roles.py
+-rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/test_e2e_symbols.py
+-rw-r--r--   0        0        0    11609 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/e2e/test_sphinx_manager.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/conftest.py
+-rw-r--r--   0        0        0    13646 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/test_configuration.py
+-rw-r--r--   0        0        0    28162 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/test_patterns.py
+-rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/features/test_directive_completion.py
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/features/test_logging.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/features/test_role_completion.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/server/features/test_sphinx_config.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/conftest.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/test_app.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/test_sa_build.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/test_sa_create_app.py
+-rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/test_sa_unit.py
+-rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/test_sa_uri_class.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/handlers/test_database.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/sphinx-agent/handlers/test_diagnostics.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/LICENSE
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/README.md
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/conf.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/demo_myst.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/demo_rst.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/pyproject.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/myst/diagnostics.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/myst/directives.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/myst/roles.md
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/myst/symbols.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/rst/diagnostics.rst
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/rst/directives.rst
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/rst/roles.rst
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo/rst/symbols.rst
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo-error/conf.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/tests/workspaces/demo-error-build/conf.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/README.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/hatch.toml
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 esbonio-1.0.0b3/PKG-INFO
```

### Comparing `esbonio-1.0.0b2/esbonio/server/__init__.py` & `esbonio-1.0.0b3/esbonio/server/__init__.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/_configuration.py` & `esbonio-1.0.0b3/esbonio/server/_configuration.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/cli.py` & `esbonio-1.0.0b3/esbonio/server/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,19 @@
     # Order matters!
     modules = [
         "esbonio.server.features.log",
         "esbonio.server.features.project_manager",
         "esbonio.server.features.sphinx_manager",
         "esbonio.server.features.preview_manager",
         "esbonio.server.features.directives",
+        "esbonio.server.features.roles",
         "esbonio.server.features.sphinx_support.diagnostics",
         "esbonio.server.features.sphinx_support.symbols",
         "esbonio.server.features.sphinx_support.directives",
+        "esbonio.server.features.sphinx_support.roles",
     ]
 
     for mod in args.included_modules:
         modules.append(mod)
 
     for mod in args.excluded_modules:
         if mod in modules:
```

### Comparing `esbonio-1.0.0b2/esbonio/server/events.py` & `esbonio-1.0.0b3/esbonio/server/events.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/feature.py` & `esbonio-1.0.0b3/esbonio/server/feature.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/server.py` & `esbonio-1.0.0b3/esbonio/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from typing import Optional
     from typing import Set
     from typing import Tuple
     from typing import Type
 
     from .feature import LanguageFeature
 
-__version__ = "1.0.0b2"
+__version__ = "1.0.0b3"
 T = TypeVar("T")
 LF = TypeVar("LF", bound="LanguageFeature")
 
 
 class EsbonioWorkspace(Workspace):
     """A modified version of pygls' workspace that ensures uris are always resolved."""
```

### Comparing `esbonio-1.0.0b2/esbonio/server/setup.py` & `esbonio-1.0.0b3/esbonio/server/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,16 @@
         doc.saved_version = doc.version or 0
 
         await call_features(ls, "document_save", params)
 
     @server.feature(
         types.TEXT_DOCUMENT_COMPLETION,
         types.CompletionOptions(
-            trigger_characters=[">", ".", ":", "`", "<", "/"], resolve_provider=True
+            trigger_characters=[">", ".", ":", "`", "<", "/", "{", "}"],
+            resolve_provider=True,
         ),
     )
     async def on_completion(ls: EsbonioLanguageServer, params: types.CompletionParams):
         uri = params.text_document.uri
         pos = params.position
         doc = ls.workspace.get_text_document(uri)
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/log.py` & `esbonio-1.0.0b3/esbonio/server/features/log.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/directives/__init__.py` & `esbonio-1.0.0b3/esbonio/server/features/directives/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         Optional[List[Directive]], Coroutine[Any, Any, Optional[List[Directive]]]
     ]:
         """Given a completion context, suggest directives that may be used."""
         return None
 
 
 class DirectiveFeature(server.LanguageFeature):
+    """Support for directives."""
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._providers: Dict[int, DirectiveProvider] = {}
         self._insert_behavior = "replace"
 
     def add_provider(self, provider: DirectiveProvider):
@@ -76,15 +78,15 @@
     ):
         """Called when the user's configuration is updated."""
         self._insert_behavior = event.value.preferred_insert_behavior
 
     async def completion(
         self, context: server.CompletionContext
     ) -> Optional[List[types.CompletionItem]]:
-        """Provide auto-completion suggestions for directives."""
+        """Provide completion suggestions for directives."""
 
         groups = context.match.groupdict()
 
         # Are we completing a directive's options?
         if "directive" not in groups:
             return await self.complete_options(context)
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/directives/completion.py` & `esbonio-1.0.0b3/esbonio/server/features/directives/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,21 @@
 
     This implements the ``insert`` behavior for directives.
     Parameters
     ----------
     context
        The context in which the completion is being generated.
 
-    name
-       The name of the directive, as it appears in an rst file.
-
     directive
-       The class implementing the directive.
+       The directive.
 
+    Returns
+    -------
+    Optional[types.CompletionItem]
+       The rendered completion item, or ``None`` if the directive should be skipped
     """
     insert_text = f".. {directive.name}::"
     user_text = context.match.group(0).strip()
 
     # Since we can't replace any existing text, it only makes sense
     # to offer completions that align with what the user has already written.
     if not insert_text.startswith(user_text):
@@ -149,15 +150,15 @@
 
     directive
        The directive to render.
 
     Returns
     -------
     Optional[types.CompletionItem]
-       The rendered completion item
+       The rendered completion item, or ``None`` if the directive should be skipped
     """
     match = context.match
 
     # Calculate the range of text the CompletionItems should edit, we don't need to
     # touch indentation.
     start = match.span()[0] + match.group(0).find(".")
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/preview_manager/__init__.py` & `esbonio-1.0.0b3/esbonio/server/features/preview_manager/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,235 @@
-import asyncio
-import logging
-import sys
-from http.server import HTTPServer
-from http.server import SimpleHTTPRequestHandler
 from typing import Any
 from typing import Dict
 from typing import Optional
+from typing import Set
 from urllib.parse import urlencode
 
-import attrs
+from lsprotocol import types
+from pygls.capabilities import get_capability
 
-from esbonio.server import EsbonioLanguageServer
+from esbonio import server
 from esbonio.server import Uri
-from esbonio.server.feature import LanguageFeature
 from esbonio.server.features.project_manager import ProjectManager
 from esbonio.server.features.sphinx_manager import SphinxClient
 from esbonio.server.features.sphinx_manager import SphinxManager
 
+from .config import PreviewConfig
+from .preview import PreviewServer
+from .preview import make_http_server
 from .webview import WebviewServer
 from .webview import make_ws_server
 
 
-class RequestHandler(SimpleHTTPRequestHandler):
-    def __init__(self, *args, logger: logging.Logger, directory: str, **kwargs) -> None:
-        self.logger = logger
-        super().__init__(*args, directory=directory, **kwargs)
-
-    def translate_path(self, path: str) -> str:
-        result = super().translate_path(path)
-        # self.logger.debug("Translate: '%s' -> '%s'", path, result)
-        return result
-
-    def log_message(self, format: str, *args: Any) -> None:
-        self.logger.debug(format, *args)
-
-
-class RequestHandlerFactory:
-    """Class for dynamically producing request handlers.
-
-    ``HTTPServer`` works by taking a "request handler" class and creating an instance of
-    it for every request it receives. By making this class callable, we can dynamically
-    produce a request handler based on the current situation.
-    """
-
-    def __init__(self, logger: logging.Logger, build_uri: Optional[Uri] = None):
-        self.logger = logger
-        self.build_uri = build_uri
-
-    def __call__(self, *args, **kwargs):
-        if self.build_uri is None:
-            raise ValueError("No build directory set")
-
-        if (build_dir := self.build_uri.fs_path) is None:
-            raise ValueError(
-                "Unable to determine build dir from uri: '%s'", self.build_uri
-            )
-
-        return RequestHandler(*args, logger=self.logger, directory=build_dir, **kwargs)
-
-
-@attrs.define
-class PreviewConfig:
-    """Configuration settings for previews."""
-
-    bind: str = attrs.field(default="localhost")
-    """The network interface to bind to, defaults to ``localhost``"""
-
-    http_port: int = attrs.field(default=0)
-    """The port to host the HTTP server on. If ``0`` a random port number will be
-    chosen"""
-
-    ws_port: int = attrs.field(default=0)
-    """The port to host the WebSocket server on. If ``0`` a random port number will be
-    chosen"""
-
-    show_line_markers: bool = attrs.field(default=False)
-    """If set, render the source line markers in the preview"""
-
-
-class PreviewManager(LanguageFeature):
+class PreviewManager(server.LanguageFeature):
     """Language feature for managing previews."""
 
     def __init__(
         self,
-        server: EsbonioLanguageServer,
+        server: server.EsbonioLanguageServer,
         sphinx: SphinxManager,
         projects: ProjectManager,
     ):
         super().__init__(server)
         self.sphinx = sphinx
         self.sphinx.add_listener("build", self.on_build)
+        """The sphinx manager."""
+
+        self.built_clients: Set[str] = set()
+        """Keeps track of which clients run a build at least once."""
+
+        self.build_path: Optional[str] = None
+        """The filepath we are currently displaying."""
+
+        self.build_uri: Optional[Uri] = None
+        """The uri of the build dir we are currently serving from."""
+
+        self.config = PreviewConfig()
+        """The current configuration."""
 
         self.projects = projects
+        """The project manager."""
 
-        logger = server.logger.getChild("PreviewServer")
-        self._request_handler_factory = RequestHandlerFactory(logger)
-        self._http_server: Optional[HTTPServer] = None
-        self._http_future: Optional[asyncio.Future] = None
+        self.preview: Optional[PreviewServer] = None
+        """The http server for serving the built files"""
 
-        self._ws_server: Optional[WebviewServer] = None
-        self._ws_task: Optional[asyncio.Task] = None
+        self.webview: Optional[WebviewServer] = None
+        """The server for controlling the webview."""
+
+    @property
+    def supports_show_document(self):
+        """Indicates if the client supports the `window/showDocument` request."""
+        return get_capability(
+            self.server.client_capabilities, "window.show_document.support", False
+        )
+
+    def initialized(self, params: types.InitializedParams):
+        """Called once the initial handshake between client and server has finished."""
+        self.configuration.subscribe(
+            "esbonio.preview", PreviewConfig, self.update_configuration
+        )
 
     def shutdown(self, params: None):
         """Called when the client instructs the server to ``shutdown``."""
-        args = {}
-        if sys.version_info.minor > 8:
-            args["msg"] = "Server is shutting down."
-
-        if self._http_server:
-            self.logger.debug("Shutting down preview HTTP server")
-            self._http_server.shutdown()
-
-        if self._ws_task:
-            self.logger.debug("Shutting down preview WebSocket server")
-            self._ws_task.cancel(**args)
+
+        if self.preview is not None:
+            self.preview.stop()
+
+        if self.webview is not None:
+            self.webview.stop()
 
     @property
     def preview_active(self) -> bool:
         """Return true if the preview is active.
 
         i.e. there is a HTTP server hosting the build result."""
-        return self._http_server is not None
+        return self.preview is not None
 
     @property
     def preview_controllable(self) -> bool:
         """Return true if the preview is controllable.
 
         i.e. there is a web socket server available to control the webview.
         """
-        return self._ws_server is not None
+        return self.webview is not None
 
-    async def get_preview_config(self) -> PreviewConfig:
-        """Return the user's preview server configuration."""
-        config = self.server.configuration.get("esbonio.preview", PreviewConfig)
-        if config is None:
-            self.logger.info(
-                "Unable to obtain preview configuration, proceeding with defaults"
-            )
-            config = PreviewConfig()
-
-        return config
-
-    async def get_http_server(self, config: PreviewConfig) -> HTTPServer:
-        """Return the http server instance hosting the previews.
+    def update_configuration(self, event: server.ConfigChangeEvent[PreviewConfig]):
+        """Called when the user's configuration is updated."""
+        config = event.value
+
+        # (Re)create the websocket server
+        if self.webview is None:
+            self.webview = make_ws_server(self.server, config)
+
+        elif (
+            config.bind != self.webview.config.bind
+            or config.ws_port != self.webview.config.ws_port
+        ):
+            self.webview.stop()
+            self.webview = make_ws_server(self.server, config)
+
+        # (Re)create the http server
+        if self.preview is None:
+            self.preview = make_http_server(self.server, config)
+            self.preview.build_uri = self.build_uri
+
+        elif (
+            config.bind != self.preview.config.bind
+            or config.http_port != self.preview.config.http_port
+        ):
+            self.preview.stop()
+            self.preview = make_http_server(self.server, config)
+            self.preview.build_uri = self.build_uri
 
-        This will also handle the creation of the server the first time it is called.
-        """
-        # TODO: Recreate the server if the configuration changes?
-        if self._http_server is not None:
-            return self._http_server
-
-        self._http_server = HTTPServer(
-            (config.bind, config.http_port), self._request_handler_factory
-        )
-
-        loop = asyncio.get_running_loop()
-        self._http_future = loop.run_in_executor(
-            self.server.thread_pool_executor,
-            self._http_server.serve_forever,
-        )
-
-        return self._http_server
-
-    async def get_webview_server(self, config: PreviewConfig) -> WebviewServer:
-        """Return the websocket server used to communicate with the webview."""
-
-        # TODO: Recreate the server if the configuration changes?
-        if self._ws_server is not None:
-            return self._ws_server
-
-        logger = self.server.logger.getChild("WebviewServer")
-        self._ws_server = make_ws_server(self.server, logger)
-        self._ws_task = asyncio.create_task(
-            self._ws_server.start_ws(config.bind, config.ws_port)
-        )
-
-        # HACK: we need to yield control to the event loop to give the ws_server time to
-        #       spin up and allocate a port number.
-        await asyncio.sleep(1)
-
-        return self._ws_server
+        self.config = config
+        self.server.run_task(self.show_preview_uri())
 
     async def on_build(self, client: SphinxClient, result):
         """Called whenever a sphinx build completes."""
+        self.built_clients.add(client.id)
 
-        if self._ws_server is None:
+        if self.webview is None or self.preview is None:
             return
 
         # Only refresh the view if the project we are previewing was built.
-        if client.build_uri != self._request_handler_factory.build_uri:
+        if client.build_uri != self.preview.build_uri:
             return
 
         self.logger.debug("Refreshing preview")
-        self._ws_server.reload()
+        self.webview.reload()
 
     async def scroll_view(self, line: int):
         """Scroll the webview to the given line number."""
 
-        if self._ws_server is None:
+        if self.webview is None:
             return
 
-        self._ws_server.scroll(line)
+        self.webview.scroll(line)
+
+    async def preview_file(self, params, retry=True):
+
+        if self.preview is None:
+            return None
 
-    async def preview_file(self, params):
         # Always check the fully resolved uri.
         src_uri = Uri.parse(params["uri"]).resolve()
         self.logger.debug("Previewing file: '%s'", src_uri)
 
         if (client := await self.sphinx.get_client(src_uri)) is None:
             return None
 
         if (project := self.projects.get_project(src_uri)) is None:
             return None
 
         if (build_path := await project.get_build_path(src_uri)) is None:
-            self.logger.debug(
-                "Unable to preview file '%s', not included in build output.", src_uri
-            )
+
+            # The client might not have built the project yet.
+            if client.id not in self.built_clients and retry is True:
+
+                # Only retry this once.
+                await self.sphinx.trigger_build(src_uri)
+                return await self.preview_file(params, retry=False)
+            else:
+
+                self.logger.debug(
+                    "Unable to preview file '%s', not included in build output.",
+                    src_uri,
+                )
+                return None
+
+        self.build_path = build_path
+        self.build_uri = self.preview.build_uri = client.build_uri
+
+        if (uri := await self.show_preview_uri()) is None:
             return None
 
-        config = await self.get_preview_config()
-        server = await self.get_http_server(config)
-        webview = await self.get_webview_server(config)
+        return {"uri": uri.as_string(encode=False)}
+
+    async def show_preview_uri(self) -> Optional[Uri]:
+        """Show the preview uri in the client using a ``window/showDocument`` request.
+        Also return the final uri."""
+
+        if self.webview is None or self.preview is None or self.build_path is None:
+            return None
+
+        server = await self.preview
+        webview = await self.webview
 
-        self._request_handler_factory.build_uri = client.build_uri
         query_params: Dict[str, Any] = dict(ws=webview.port)
 
-        if config.show_line_markers:
+        if self.config.show_line_markers:
             query_params["show-markers"] = True
 
         uri = Uri.create(
             scheme="http",
-            authority=f"localhost:{server.server_port}",
-            path=build_path,
+            authority=f"localhost:{server.port}",
+            path=self.build_path,
             query=urlencode(query_params),
         )
-
         self.logger.info("Preview available at: %s", uri.as_string(encode=False))
-        return {"uri": uri.as_string(encode=False)}
+
+        if self.supports_show_document:
+            result = await self.server.show_document_async(
+                types.ShowDocumentParams(
+                    uri=uri.as_string(encode=False), external=True, take_focus=False
+                )
+            )
+            self.logger.debug("window/showDocument: %s", result)
+
+        return uri
 
 
 def esbonio_setup(
-    server: EsbonioLanguageServer, sphinx: SphinxManager, projects: ProjectManager
+    esbonio: server.EsbonioLanguageServer,
+    sphinx: SphinxManager,
+    projects: ProjectManager,
 ):
-    manager = PreviewManager(server, sphinx, projects)
-    server.add_feature(manager)
+    manager = PreviewManager(esbonio, sphinx, projects)
+    esbonio.add_feature(manager)
 
-    @server.feature("view/scroll")
-    async def on_scroll(ls: EsbonioLanguageServer, params):
+    @esbonio.feature("view/scroll")
+    async def on_scroll(ls: server.EsbonioLanguageServer, params):
         await manager.scroll_view(params.line)
 
-    @server.command("esbonio.server.previewFile")
-    async def preview_file(ls: EsbonioLanguageServer, *args):
+    @esbonio.command("esbonio.server.previewFile")
+    async def preview_file(ls: server.EsbonioLanguageServer, *args):
         return await manager.preview_file(args[0][0])
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/preview_manager/webview.py` & `esbonio-1.0.0b3/esbonio/server/features/preview_manager/webview.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,75 @@
-"""This module implements the websocket server used to communicate with preivew
- windows."""
+from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import socket
-from typing import Optional
+import typing
 
 from pygls.protocol import JsonRPCProtocol
 from pygls.protocol import default_converter
 from pygls.server import Server
 from pygls.server import WebSocketTransportAdapter
 from websockets.server import serve
 
-from esbonio.server import EsbonioLanguageServer
+from esbonio import server
+
+if typing.TYPE_CHECKING:
+    from typing import Optional
+
+    from websockets import WebSocketServer
+
+    from .config import PreviewConfig
 
 
 class WebviewServer(Server):
     """The webview server controlls the webpage hosting the preview.
 
     Used to implement automatic reloads and features like sync scrolling.
     """
 
     lsp: JsonRPCProtocol
 
-    def __init__(self, logger: logging.Logger, *args, **kwargs):
+    def __init__(self, logger: logging.Logger, config: PreviewConfig, *args, **kwargs):
         super().__init__(JsonRPCProtocol, default_converter, *args, **kwargs)
-        self.logger = logger
+
+        self.config = config
+        self.logger = logger.getChild("WebviewServer")
         self.lsp._send_only_body = True
-        self.port = None
 
         self._connected = False
+        self._ws_server: Optional[WebSocketServer] = None
+
+        self._startup_task: Optional[asyncio.Task] = None
+        """The task that resolves once startup is complete."""
+
+        self._server_task: Optional[asyncio.Task] = None
+        """The task hosting the server itself."""
+
         self._editor_in_control: Optional[asyncio.Task] = None
+        """If set, the editor is in control and the view should not emit scroll events"""
+
         self._view_in_control: Optional[asyncio.Task] = None
+        """If set, the view is in control and the editor should not emit scroll events"""
+
+    def __await__(self):
+        """Makes the server await-able"""
+        if self._startup_task is None:
+            self._startup_task = asyncio.create_task(self.start())
+
+        return self._startup_task.__await__()
+
+    @property
+    def port(self):
+        if self._ws_server is None:
+            return None
+
+        sock = list(self._ws_server.sockets)[0]
+        return sock.getsockname()[1]
 
     @property
     def connected(self) -> bool:
         """Indicates when we have an active connection to the client."""
         return self._connected
 
     def feature(self, feature_name: str, options=None):
@@ -63,16 +96,34 @@
         """Create a cooldown."""
         await asyncio.sleep(1)
 
         # Unset the cooldown
         self.logger.debug("%s cooldown ended", name)
         setattr(self, f"_{name}_in_control", None)
 
-    async def start_ws(self, host: str, port: int) -> None:  # type: ignore[override]
-        """Start the server."""
+    async def start(self):
+        """Start the server and wrap the server coroutine in a task."""
+        self._server_task = asyncio.create_task(
+            self._start_ws(self.config.bind, self.config.ws_port)
+        )
+
+        # HACK: we need to yield control to the event loop to give the ws_server time to
+        #       spin up and allocate a port number.
+        await asyncio.sleep(1)
+        return self
+
+    def stop(self):
+        """Stop the server."""
+        self.logger.debug("Shutting down preview WebSocket server")
+
+        if self._server_task is not None:
+            self._server_task.cancel()
+
+    async def _start_ws(self, host: str, port: int) -> None:
+        """Actually, start the server."""
 
         async def connection(websocket):
             loop = asyncio.get_running_loop()
             transport = WebSocketTransportAdapter(websocket, loop)
 
             self.lsp.connection_made(transport)  # type: ignore[arg-type]
             self._connected = True
@@ -89,23 +140,22 @@
         async with serve(
             connection,
             host,
             port,
             # logger=self.logger.getChild("ws"),
             family=socket.AF_INET,  # Use IPv4 only.
         ) as ws_server:
-            sock = list(ws_server.sockets)[0]
-            self.port = sock.getsockname()[1]
+            self._ws_server = ws_server
             await asyncio.Future()  # run forever
 
 
 def make_ws_server(
-    esbonio: EsbonioLanguageServer, logger: logging.Logger
+    esbonio: server.EsbonioLanguageServer, config: PreviewConfig
 ) -> WebviewServer:
-    server = WebviewServer(logger)
+    server = WebviewServer(esbonio.logger, config)
 
     @server.feature("editor/scroll")
     def on_scroll(ls: WebviewServer, params):
         """Called by the webview to scroll the editor."""
         if not server.connected or server._editor_in_control:
             return
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/project_manager/manager.py` & `esbonio-1.0.0b3/esbonio/server/features/project_manager/manager.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/project_manager/project.py` & `esbonio-1.0.0b3/esbonio/server/features/project_manager/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,22 @@
         """Get the directives known to Sphinx."""
         db = await self.get_db()
 
         query = "SELECT name, implementation FROM directives"
         cursor = await db.execute(query)
         return await cursor.fetchall()  # type: ignore[return-value]
 
+    async def get_roles(self) -> List[Tuple[str, Optional[str]]]:
+        """Get the roles known to Sphinx."""
+        db = await self.get_db()
+
+        query = "SELECT name, implementation FROM roles"
+        cursor = await db.execute(query)
+        return await cursor.fetchall()  # type: ignore[return-value]
+
     async def get_document_symbols(self, src_uri: Uri) -> List[types.Symbol]:
         """Get the symbols for the given file."""
         db = await self.get_db()
         query = (
             "SELECT id, name, kind, detail, range, parent_id, order_id "
             "FROM symbols WHERE uri = ?"
         )
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/__init__.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/client.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/client_subprocess.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/client_subprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
 async def forward_stderr(server: asyncio.subprocess.Process):
     if server.stderr is None:
         return
 
     # EOF is signalled with an empty bytestring
     while (line := await server.stderr.readline()) != b"":
-        sphinx_logger.info(line.decode())
+        sphinx_logger.info(line.decode().strip())
 
 
 def make_subprocess_sphinx_client(
     manager: SphinxManager, config: SphinxConfig
 ) -> SphinxClient:
     """Factory function for creating a ``SubprocessSphinxClient`` instance.
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/config.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/config.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_manager/manager.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,31 +207,40 @@
 
         scope = self.server.configuration.scope_for(uri)
         if scope not in self.clients:
             self.logger.debug("No client found, creating new subscription")
             self.server.configuration.subscribe(
                 "esbonio.sphinx",
                 SphinxConfig,
-                self._create_or_replace_client,
+                partial(self._create_or_replace_client, uri),
                 scope=uri,
             )
             # The first few callers in a given scope will miss out, but that shouldn't matter
             # too much
             return None
 
         if (client := self.clients[scope]) is None:
             self.logger.debug("No applicable client for uri: %s", uri)
             return None
 
         return await client
 
     async def _create_or_replace_client(
-        self, event: server.ConfigChangeEvent[SphinxConfig]
+        self, uri: Uri, event: server.ConfigChangeEvent[SphinxConfig]
     ):
-        """Create or replace thesphinx client instance for the given config."""
+        """Create or replace thesphinx client instance for the given config.
+
+        Parameters
+        ----------
+        uri
+           The uri for which the sphinx client was originally created for
+
+        event
+           The configuration change event
+        """
 
         config = event.value
 
         # Do not try and create clients in the global scope
         if event.scope == "":
             return
 
@@ -239,17 +248,15 @@
         if (previous_client := self.clients.pop(event.scope, None)) is not None:
             self.server.lsp.notify(
                 "sphinx/clientDestroyed",
                 ClientDestroyedNotification(id=previous_client.id),
             )
             self.server.run_task(previous_client.stop())
 
-        resolved = config.resolve(
-            Uri.parse(event.scope), self.server.workspace, self.logger
-        )
+        resolved = config.resolve(uri, self.server.workspace, self.logger)
         if resolved is None:
             self.clients[event.scope] = None
             return
 
         self.clients[event.scope] = client = self.client_factory(self, resolved)
         client.add_listener("state-change", partial(self._on_state_change, event.scope))
```

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_support/diagnostics.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_support/diagnostics.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_support/directives.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_support/directives.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/server/features/sphinx_support/symbols.py` & `esbonio-1.0.0b3/esbonio/server/features/sphinx_support/symbols.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/__init__.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/app.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/app.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/config.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/config.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/database.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/database.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/log.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/log.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/patches.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/patches.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/server.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/server.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/types.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,60 @@
 )
 """A regular expression to detect and parse partial and complete MyST directives.
 
 This does **not** include any options or content that may be included with the
 initial declaration.
 """
 
+MYST_ROLE: "re.Pattern" = re.compile(
+    r"""
+    ([^\w`]|^\s*)                     # roles cannot be preceeded by letter chars
+    (?P<role>
+      {                               # roles start with a '{'
+      (?P<name>[:\w-]+)?              # roles have a name
+      }?                              # roles end with a '}'
+    )
+    (?P<target>
+      `                               # targets begin with a '`' character
+      ((?P<alias>[^<`>]*?)<)?         # targets may specify an alias
+      (?P<modifier>[!~])?             # targets may have a modifier
+      (?P<label>[^<`>]*)?             # targets contain a label
+      >?                              # labels end with a '>' when there's an alias
+      `?                              # targets end with a '`' character
+    )?
+    """,
+    re.VERBOSE,
+)
+"""A regular expression to detect and parse parial and complete roles.
+
+I'm not sure if there are offical names for the components of a role, but the
+language server breaks a role down into a number of parts::
+
+                 vvvvvv label
+                v modifier(optional)
+               vvvvvvvv target
+   {c:function}`!malloc`
+   ^^^^^^^^^^^^ role
+    ^^^^^^^^^^ name
+
+The language server sometimes refers to the above as a "plain" role, in that the
+role's target contains just the label of the object it is linking to. However it's
+also possible to define "aliased" roles, where the link text in the final document
+is overriden, for example::
+
+                vvvvvvvvvvvvvvvvvvvvvvvv alias
+                                          vvvvvv label
+                                         v modifier (optional)
+               vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv target
+   {c:function}`used to allocate memory <~malloc>`
+   ^^^^^^^^^^^^ role
+    ^^^^^^^^^^ name
+
+"""
+
 
 RST_DIRECTIVE: "re.Pattern" = re.compile(
     r"""
     (\s*)                             # directives can be indented
     (?P<directive>
       \.\.                            # directives start with a comment
       [ ]?                            # followed by a space
@@ -110,16 +156,15 @@
 
 RST_ROLE = re.compile(
     r"""
     ([^\w:]|^\s*)                     # roles cannot be preceeded by letter chars
     (?P<role>
       :                               # roles begin with a ':' character
       (?!:)                           # the next character cannot be a ':'
-      ((?P<domain>[\w]+):(?=\w))?     # roles may include a domain (that must be followed by a word character)
-      ((?P<name>[\w-]+):?)?           # roles have a name
+      ((?P<name>\w([:\w-]*\w)?):?)?   # roles have a name
     )
     (?P<target>
       `                               # targets begin with a '`' character
       ((?P<alias>[^<`>]*?)<)?         # targets may specify an alias
       (?P<modifier>[!~])?             # targets may have a modifier
       (?P<label>[^<`>]*)?             # targets contain a label
       >?                              # labels end with a '>' when there's an alias
@@ -134,30 +179,28 @@
 language server breaks a role down into a number of parts::
 
                  vvvvvv label
                 v modifier(optional)
                vvvvvvvv target
    :c:function:`!malloc`
    ^^^^^^^^^^^^ role
-      ^^^^^^^^ name
-    ^ domain (optional)
+    ^^^^^^^^^^ name
 
 The language server sometimes refers to the above as a "plain" role, in that the
 role's target contains just the label of the object it is linking to. However it's
 also possible to define "aliased" roles, where the link text in the final document
 is overriden, for example::
 
                 vvvvvvvvvvvvvvvvvvvvvvvv alias
                                           vvvvvv label
                                          v modifier (optional)
-               vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv target
+               vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv target
    :c:function:`used to allocate memory <~malloc>`
    ^^^^^^^^^^^^ role
-      ^^^^^^^^ name
-    ^ domain (optional)
+    ^^^^^^^^^^ name
 
 """
 
 
 RST_DEFAULT_ROLE = re.compile(
     r"""
     (?<![:`])
```

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/util.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/util.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/__init__.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 # Inject our own 'core' extensions into Sphinx
 sphinx.application.builtin_extensions += (
     f"{__name__}.files",
     f"{__name__}.diagnostics",
     f"{__name__}.symbols",
     f"{__name__}.directives",
+    f"{__name__}.roles",
 )
 
 
 class SphinxHandler:
     """Responsible for implementing the JSON-RPC API exposed by the Sphinx agent."""
 
     def __init__(self):
```

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/diagnostics.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/directives.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/directives.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/files.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/files.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/handlers/symbols.py` & `esbonio-1.0.0b3/esbonio/sphinx_agent/handlers/symbols.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/esbonio/sphinx_agent/static/webview.js` & `esbonio-1.0.0b3/esbonio/sphinx_agent/static/webview.js`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/e2e/conftest.py` & `esbonio-1.0.0b3/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/e2e/test_e2e_diagnostics.py` & `esbonio-1.0.0b3/tests/e2e/test_e2e_diagnostics.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/e2e/test_e2e_directives.py` & `esbonio-1.0.0b3/tests/e2e/test_e2e_directives.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/e2e/test_e2e_symbols.py` & `esbonio-1.0.0b3/tests/e2e/test_e2e_symbols.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/e2e/test_sphinx_manager.py` & `esbonio-1.0.0b3/tests/e2e/test_sphinx_manager.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/server/conftest.py` & `esbonio-1.0.0b3/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/server/test_configuration.py` & `esbonio-1.0.0b3/tests/server/test_configuration.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/server/test_patterns.py` & `esbonio-1.0.0b3/tests/server/test_patterns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from esbonio.sphinx_agent.types import MYST_DIRECTIVE
+from esbonio.sphinx_agent.types import MYST_ROLE
 from esbonio.sphinx_agent.types import RST_DEFAULT_ROLE
 from esbonio.sphinx_agent.types import RST_DIRECTIVE
 from esbonio.sphinx_agent.types import RST_DIRECTIVE_OPTION
 from esbonio.sphinx_agent.types import RST_ROLE
 
 
 @pytest.mark.parametrize(
@@ -58,14 +59,288 @@
         for name, value in expected.items():
             assert match.groupdict().get(name, None) == value, name
 
 
 @pytest.mark.parametrize(
     "string, expected",
     [
+        ("`{", None),
+        ("d{", None),
+        ("{", {"role": "{"}),
+        ("{ref", {"name": "ref", "role": "{ref"}),
+        # The pattern should still work if the user adds a role in the middle of a line
+        ("{ref for more details", {"name": "ref", "role": "{ref"}),
+        ("{ref} for more details", {"name": "ref", "role": "{ref}"}),
+        ("{code-block", {"name": "code-block", "role": "{code-block"}),
+        ("{c:func}", {"name": "c:func", "role": "{c:func}"}),
+        ("{cpp:func}", {"name": "cpp:func", "role": "{cpp:func}"}),
+        ("{ref}`", {"name": "ref", "role": "{ref}", "target": "`"}),
+        (
+            "{code-block}`",
+            {"name": "code-block", "role": "{code-block}", "target": "`"},
+        ),
+        (
+            "{c:func}`",
+            {"name": "c:func", "role": "{c:func}", "target": "`"},
+        ),
+        (
+            "{ref}`some_label",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "label": "some_label",
+                "target": "`some_label",
+            },
+        ),
+        (
+            "{ref}`!some_label",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "label": "some_label",
+                "target": "`!some_label",
+                "modifier": "!",
+            },
+        ),
+        (
+            "{ref}`~some_label",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "label": "some_label",
+                "target": "`~some_label",
+                "modifier": "~",
+            },
+        ),
+        (
+            "{code-block}`some_label",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "label": "some_label",
+                "target": "`some_label",
+            },
+        ),
+        (
+            "{c:func}`some_label",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "label": "some_label",
+                "target": "`some_label",
+            },
+        ),
+        (
+            "{ref}`some_label`",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "label": "some_label",
+                "target": "`some_label`",
+            },
+        ),
+        (
+            "{code-block}`some_label`",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "label": "some_label",
+                "target": "`some_label`",
+            },
+        ),
+        (
+            "{c:func}`some_label`",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "label": "some_label",
+                "target": "`some_label`",
+            },
+        ),
+        (
+            "{ref}`see more <",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "alias": "see more ",
+                "target": "`see more <",
+            },
+        ),
+        (
+            "{code-block}`see more <",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "alias": "see more ",
+                "target": "`see more <",
+            },
+        ),
+        (
+            "{c:func}`see more <",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "alias": "see more ",
+                "target": "`see more <",
+            },
+        ),
+        (
+            "{ref}`see more <some_label",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label",
+            },
+        ),
+        (
+            "{code-block}`see more <some_label",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label",
+            },
+        ),
+        (
+            "{ref}`see more <!some_label",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <!some_label",
+                "modifier": "!",
+            },
+        ),
+        (
+            "{code-block}`see more <~some_label",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <~some_label",
+                "modifier": "~",
+            },
+        ),
+        (
+            "{c:func}`see more <some_label",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label",
+            },
+        ),
+        (
+            "{ref}`see more <some_label>",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>",
+            },
+        ),
+        (
+            "{code-block}`see more <some_label>",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>",
+            },
+        ),
+        (
+            "{c:func}`see more <some_label>",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>",
+            },
+        ),
+        (
+            "{ref}`see more <some_label>`",
+            {
+                "name": "ref",
+                "role": "{ref}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>`",
+            },
+        ),
+        (
+            "{code-block}`see more <some_label>`",
+            {
+                "name": "code-block",
+                "role": "{code-block}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>`",
+            },
+        ),
+        (
+            "{c:func}`see more <some_label>`",
+            {
+                "name": "c:func",
+                "role": "{c:func}",
+                "alias": "see more ",
+                "label": "some_label",
+                "target": "`see more <some_label>`",
+            },
+        ),
+    ],
+)
+def test_myst_role_regex(string, expected):
+    """Ensure that the regular expression we use to detect and parse roles works as
+    expected.
+
+    As a general rule, it's better to write tests at the LSP protocol level as that
+    decouples the test cases from the implementation. However, roles and the
+    corresponding regular expression are complex enough to warrant a test case on its
+    own.
+
+    As with most test cases, this one is parameterized with the following arguments::
+
+        (":ref:", {"name": "ref"}),
+        (".. directive::", None)
+
+    The first argument is the string to test the pattern against, the second a
+    dictionary containing the groups we expect to see in the resulting match object.
+    Groups that appear in the resulting match object but not in the expected result will
+    **not** fail the test.
+
+    To test situations where the pattern should **not** match the input, pass ``None``
+    as the second argument.
+
+    To test situations where the pattern should match, but we don't expect to see any
+    groups pass an empty dictionary as the second argument.
+    """
+
+    match = MYST_ROLE.search(string)
+
+    if expected is None:
+        assert match is None
+    else:
+        assert match is not None
+
+        for name, value in expected.items():
+            assert match.groupdict().get(name, None) == value
+
+
+@pytest.mark.parametrize(
+    "string, expected",
+    [
         (".", None),
         ("..", {"directive": ".."}),
         (".. d", {"directive": ".. d"}),
         (".. image::", {"name": "image", "directive": ".. image::"}),
         (".. c:", {"name": "c:", "directive": ".. c:"}),
         (".. |", {"directive": ".. |", "substitution": "|"}),
         (
@@ -163,15 +438,15 @@
                 "name": "rst:directive:option",
                 "directive": ".. rst:directive:option::",
                 "argument": "height",
             },
         ),
     ],
 )
-def test_directive_regex(string, expected):
+def test_rst_directive_regex(string, expected):
     """Ensure that the regular expression we use to detect and parse directives
     works as expected.
 
     As with most test cases, this one is parameterized with the following arguments::
 
        (".. figure::", {"name": "figure"})
 
@@ -247,25 +522,28 @@
 
 @pytest.mark.parametrize(
     "string, expected",
     [
         ("::", None),
         (":", {"role": ":"}),
         (":ref", {"name": "ref", "role": ":ref"}),
+        # The pattern should still work if the user adds a role in the middle of a line
+        (":ref for more details", {"name": "ref", "role": ":ref"}),
+        (":ref: for more details", {"name": "ref", "role": ":ref:"}),
         (":code-block", {"name": "code-block", "role": ":code-block"}),
-        (":c:func:", {"name": "func", "domain": "c", "role": ":c:func:"}),
-        (":cpp:func:", {"name": "func", "domain": "cpp", "role": ":cpp:func:"}),
+        (":c:func:", {"name": "c:func", "role": ":c:func:"}),
+        (":cpp:func:", {"name": "cpp:func", "role": ":cpp:func:"}),
         (":ref:`", {"name": "ref", "role": ":ref:", "target": "`"}),
         (
             ":code-block:`",
             {"name": "code-block", "role": ":code-block:", "target": "`"},
         ),
         (
             ":c:func:`",
-            {"name": "func", "domain": "c", "role": ":c:func:", "target": "`"},
+            {"name": "c:func", "role": ":c:func:", "target": "`"},
         ),
         (
             ":ref:`some_label",
             {
                 "name": "ref",
                 "role": ":ref:",
                 "label": "some_label",
@@ -300,16 +578,15 @@
                 "label": "some_label",
                 "target": "`some_label",
             },
         ),
         (
             ":c:func:`some_label",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "label": "some_label",
                 "target": "`some_label",
             },
         ),
         (
             ":ref:`some_label`",
@@ -328,16 +605,15 @@
                 "label": "some_label",
                 "target": "`some_label`",
             },
         ),
         (
             ":c:func:`some_label`",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "label": "some_label",
                 "target": "`some_label`",
             },
         ),
         (
             ":ref:`see more <",
@@ -356,16 +632,15 @@
                 "alias": "see more ",
                 "target": "`see more <",
             },
         ),
         (
             ":c:func:`see more <",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "alias": "see more ",
                 "target": "`see more <",
             },
         ),
         (
             ":ref:`see more <some_label",
@@ -408,16 +683,15 @@
                 "target": "`see more <~some_label",
                 "modifier": "~",
             },
         ),
         (
             ":c:func:`see more <some_label",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "alias": "see more ",
                 "label": "some_label",
                 "target": "`see more <some_label",
             },
         ),
         (
@@ -439,16 +713,15 @@
                 "label": "some_label",
                 "target": "`see more <some_label>",
             },
         ),
         (
             ":c:func:`see more <some_label>",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "alias": "see more ",
                 "label": "some_label",
                 "target": "`see more <some_label>",
             },
         ),
         (
@@ -470,25 +743,24 @@
                 "label": "some_label",
                 "target": "`see more <some_label>`",
             },
         ),
         (
             ":c:func:`see more <some_label>`",
             {
-                "name": "func",
-                "domain": "c",
+                "name": "c:func",
                 "role": ":c:func:",
                 "alias": "see more ",
                 "label": "some_label",
                 "target": "`see more <some_label>`",
             },
         ),
     ],
 )
-def test_role_regex(string, expected):
+def test_rst_role_regex(string, expected):
     """Ensure that the regular expression we use to detect and parse roles works as
     expected.
 
     As a general rule, it's better to write tests at the LSP protocol level as that
     decouples the test cases from the implementation. However, roles and the
     corresponding regular expression are complex enough to warrant a test case on its
     own.
```

### Comparing `esbonio-1.0.0b2/tests/server/features/test_directive_completion.py` & `esbonio-1.0.0b3/tests/server/features/test_directive_completion.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/server/features/test_logging.py` & `esbonio-1.0.0b3/tests/server/features/test_logging.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/server/features/test_sphinx_config.py` & `esbonio-1.0.0b3/tests/server/features/test_sphinx_config.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/conftest.py` & `esbonio-1.0.0b3/tests/sphinx-agent/conftest.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/test_app.py` & `esbonio-1.0.0b3/tests/sphinx-agent/test_app.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_build.py` & `esbonio-1.0.0b3/tests/sphinx-agent/test_sa_build.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_create_app.py` & `esbonio-1.0.0b3/tests/sphinx-agent/test_sa_create_app.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_unit.py` & `esbonio-1.0.0b3/tests/sphinx-agent/test_sa_unit.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/test_sa_uri_class.py` & `esbonio-1.0.0b3/tests/sphinx-agent/test_sa_uri_class.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_database.py` & `esbonio-1.0.0b3/tests/sphinx-agent/handlers/test_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,21 +23,23 @@
     db = await project.get_db()
     cursor = await db.execute("SELECT * FROM files")
     results = await cursor.fetchall()
     actual = {r for r in results if "badfile" not in r[1]}
 
     expected = {
         (anuri(src, "index.rst"), "index", "index.html"),
+        (anuri(src, "rst", "roles.rst"), "rst/roles", "rst/roles.html"),
         (anuri(src, "rst", "directives.rst"), "rst/directives", "rst/directives.html"),
         (
             anuri(src, "rst", "diagnostics.rst"),
             "rst/diagnostics",
             "rst/diagnostics.html",
         ),
         (anuri(src, "rst", "symbols.rst"), "rst/symbols", "rst/symbols.html"),
+        (anuri(src, "myst", "roles.md"), "myst/roles", "myst/roles.html"),
         (
             anuri(src, "myst", "directives.md"),
             "myst/directives",
             "myst/directives.html",
         ),
         (
             anuri(src, "myst", "diagnostics.md"),
```

### Comparing `esbonio-1.0.0b2/tests/sphinx-agent/handlers/test_diagnostics.py` & `esbonio-1.0.0b3/tests/sphinx-agent/handlers/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/LICENSE` & `esbonio-1.0.0b3/tests/workspaces/demo/LICENSE`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/README.md` & `esbonio-1.0.0b3/tests/workspaces/demo/README.md`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/conf.py` & `esbonio-1.0.0b3/tests/workspaces/demo/conf.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/index.rst` & `esbonio-1.0.0b3/tests/workspaces/demo/index.rst`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/myst/symbols.md` & `esbonio-1.0.0b3/tests/workspaces/demo/myst/symbols.md`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo/rst/symbols.rst` & `esbonio-1.0.0b3/tests/workspaces/demo/rst/symbols.rst`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo-error/conf.py` & `esbonio-1.0.0b3/tests/workspaces/demo-error/conf.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/tests/workspaces/demo-error-build/conf.py` & `esbonio-1.0.0b3/tests/workspaces/demo-error-build/conf.py`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/LICENSE` & `esbonio-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/README.md` & `esbonio-1.0.0b3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 ![Completion Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/completion-demo.gif)
 
 ## Definitions
 
 ![Definition Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/definition-demo.gif)
 
-
 ## Diagnostics
 
 ![Diagnostics Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/diagnostic-sphinx-errors-demo.png)
 
 ## Document Links
 
 ![Document Link Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/document-links-demo.png)
```

### Comparing `esbonio-1.0.0b2/pyproject.toml` & `esbonio-1.0.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbonio-1.0.0b2/PKG-INFO` & `esbonio-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbonio
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A language server for sphinx/docutils based documentation projects.
 Project-URL: Bug Tracker, https://github.com/swyddfa/esbonio/issues
 Project-URL: Documentation, https://swyddfa.github.io/esbonio/
 Project-URL: Source Code, https://github.com/swyddfa/esbonio
 Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -54,15 +54,14 @@
 
 ![Completion Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/completion-demo.gif)
 
 ## Definitions
 
 ![Definition Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/definition-demo.gif)
 
-
 ## Diagnostics
 
 ![Diagnostics Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/diagnostic-sphinx-errors-demo.png)
 
 ## Document Links
 
 ![Document Link Demo](https://github.com/swyddfa/esbonio/raw/release/resources/images/document-links-demo.png)
```

