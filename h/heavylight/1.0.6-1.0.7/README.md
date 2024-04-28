# Comparing `tmp/heavylight-1.0.6.tar.gz` & `tmp/heavylight-1.0.7.tar.gz`

## Comparing `heavylight-1.0.6.tar` & `heavylight-1.0.7.tar`

### file list

```diff
@@ -1,74 +1,95 @@
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 heavylight-1.0.6/mkdocs.yml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 heavylight-1.0.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 heavylight-1.0.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 heavylight-1.0.6/.vscode/settings.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 heavylight-1.0.6/developer-setup/environment-notes.md
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/index.md
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/storage_function.md
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/tables.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/_static/custom_css.css
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.6/docs/_static/mathjax.js
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/basic_cashflow.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/readme.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/readme_example.py
--rw-r--r--   0        0        0    21406 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/memory_optimizations/example.ipynb
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/docs_check_tables_md.ipynb
--rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0    76024 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/string_lookup_investigation.ipynb
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/super_init_example.ipynb
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_bounds_check.ipynb
--rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation.ipynb
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation.md
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/using_dataclasses.ipynb
--rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/vectors.py
--rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
--rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/notebook/table_documentation_files/table_documentation_32_1.png
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/protection_model.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/run_model.py
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/covert_q_x_tables.ipynb
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/q_x_generic.csv
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/qx_generic_raw.csv
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model/tables/uk_zero_spot.csv
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/protection_model.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/run_model.py
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/covert_q_x_tables.ipynb
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/q_x_generic.csv
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/qx_generic_raw.csv
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.6/examples/std_model_numpy/tables/uk_zero_spot.csv
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/__init__.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/heavylight.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/heavytables.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/make_examples.py
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/memory_optimized_cache.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/memory_optimized_model.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_model_base.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_model_np.py
--rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/readme.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/run_model_base.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/run_model_np.py
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/tables/forward_rates.csv
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/protection/tables/q_x_generic.csv
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 heavylight-1.0.6/src/heavylight/examples/template/model.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_examples.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_heavylight.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_heavytables.py
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_lightmodel.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_lightmodel_df.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_memory_savings.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 heavylight-1.0.6/tests/test_optimized_cache.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.6/LICENSE
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 heavylight-1.0.6/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 heavylight-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 heavylight-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 heavylight-1.0.7/.python-version
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 heavylight-1.0.7/mkdocs.yml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 heavylight-1.0.7/requirements-dev.lock
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 heavylight-1.0.7/requirements.lock
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 heavylight-1.0.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 heavylight-1.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 heavylight-1.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 heavylight-1.0.7/developer-setup/environment-notes.md
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/index.md
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/storage_function.md
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/tables.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/custom_css.css
+-rw-r--r--   0        0        0   177915 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/dependency-graph-dark.svg
+-rw-r--r--   0        0        0   178414 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/dependency-graph-light.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/mathjax.js
+-rw-r--r--   0        0        0   176374 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-can-clear-dark.svg
+-rw-r--r--   0        0        0   177132 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-can-clear-light.svg
+-rw-r--r--   0        0        0   173374 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-last-needed-dark.svg
+-rw-r--r--   0        0        0   172658 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/_static/memopt-last-needed-light.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/heavylight_Model.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/heavylight_Table.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/api/lightmodel.md
+-rw-r--r--   0        0        0    56497 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/getting_started/heavylight_tables.ipynb
+-rw-r--r--   0        0        0   172293 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/getting_started/intro_to_heavylight.ipynb
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/memory_optimization.md
+-rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/recursive_life_insurance.ipynb
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 heavylight-1.0.7/docs/theory/vectorized_models.ipynb
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/basic_cashflow.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/readme.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/readme_example.py
+-rw-r--r--   0        0        0    21406 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/memory_optimizations/example.ipynb
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/docs_check_tables_md.ipynb
+-rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    76024 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/safe_string_table_lookup.ipynb
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/string_lookup_investigation.ipynb
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/super_init_example.ipynb
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_bounds_check.ipynb
+-rw-r--r--   0        0        0    70439 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation.ipynb
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation.md
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/test_tables_v1.0.7.ipynb
+-rw-r--r--   0        0        0    21245 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/using_dataclasses.ipynb
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/vectors.py
+-rw-r--r--   0        0        0  1491502 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/notebook/table_documentation_files/table_documentation_32_1.png
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/protection_model.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/run_model.py
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/covert_q_x_tables.ipynb
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/qx_generic_raw.csv
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 heavylight-1.0.7/examples/std_model_numpy/tables/uk_zero_spot.csv
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/heavytables.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/make_examples.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/memory_optimized_cache.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/memory_optimized_model.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_base.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_mo.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_model_np.py
+-rw-r--r--   0        0        0   380137 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/readme.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_base.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_mo.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/run_model_np.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/tables/forward_rates.csv
+-rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/protection/tables/q_x_generic.csv
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 heavylight-1.0.7/src/heavylight/examples/template/model.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_examples.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_heavylight.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_heavytables.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_lightmodel.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_lightmodel_df.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_memory_savings.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 heavylight-1.0.7/tests/test_optimized_cache.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 heavylight-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 heavylight-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 heavylight-1.0.7/README.md
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 heavylight-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 heavylight-1.0.7/PKG-INFO
```

### Comparing `heavylight-1.0.6/.devcontainer/devcontainer.json` & `heavylight-1.0.7/.devcontainer/devcontainer.json`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 		"ghcr.io/hspaans/devcontainer-features/pytest:1": {},
 		"ghcr.io/meaningful-ooo/devcontainer-features/fish:1": {},
 		"ghcr.io/stuartleeks/dev-container-features/shell-history:0": {},
 		"ghcr.io/devcontainers/features/github-cli:1": {}
 	},
 
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
-	// "forwardPorts": [],
+	"forwardPorts": [8000], // for mkdocs
 
 	// Use 'postCreateCommand' to pip install the editable
-	"postCreateCommand": "pip install -e .[dev]",
+	"postCreateCommand": "pip install -e .[dev,docs]",
 	"customizations": {
 		"vscode": {
 			"extensions": [
 				"ms-python.python",
 				"github.vscode-github-actions",
 				"ms-toolsai.jupyter",
 				"ms-python.black-formatter",
```

### Comparing `heavylight-1.0.6/.github/workflows/docs.yml` & `heavylight-1.0.7/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,9 +22,9 @@
       - run: echo "cache_id=$(date --utc '+%V')" >> $GITHUB_ENV 
       - uses: actions/cache@v4
         with:
           key: mkdocs-material-${{ env.cache_id }}
           path: .cache
           restore-keys: |
             mkdocs-material-
-      - run: pip install mkdocs-material 
-      - run: mkdocs gh-deploy --force
+      - run: pip install -e .[docs]
+      - run: mkdocs gh-deploy --force
```

### Comparing `heavylight-1.0.6/.github/workflows/python-package.yml` & `heavylight-1.0.7/.github/workflows/python-package.yml`

 * *Files 21% similar despite different names*

```diff
@@ -30,12 +30,10 @@
         python -m pip install pytest
         python -m pip install -e .[dev]
     - name: Test with pytest
       run: |
         pytest --cov=src tests/
     - run: ls
     - name: Upload coverage to codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
-        slug: lewisfogden/heavylight
-        fail_ci_if_error: true
```

### Comparing `heavylight-1.0.6/developer-setup/environment-notes.md` & `heavylight-1.0.7/developer-setup/environment-notes.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/docs/index.md` & `heavylight-1.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/docs/storage_function.md` & `heavylight-1.0.7/docs/storage_function.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/docs/tables.md` & `heavylight-1.0.7/docs/tables.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/docs/_static/custom_css.css` & `heavylight-1.0.7/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/basic_cashflow.py` & `heavylight-1.0.7/examples/basic_cashflow.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/readme_example.py` & `heavylight-1.0.7/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/memory_optimizations/example.ipynb` & `heavylight-1.0.7/examples/memory_optimizations/example.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/docs_check_tables_md.ipynb` & `heavylight-1.0.7/examples/notebook/docs_check_tables_md.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.7/examples/notebook/heavylight_basic.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.7/examples/notebook/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.7/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/string_lookup_investigation.ipynb` & `heavylight-1.0.7/examples/notebook/string_lookup_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/super_init_example.ipynb` & `heavylight-1.0.7/examples/notebook/super_init_example.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/table_bounds_check.ipynb` & `heavylight-1.0.7/examples/notebook/table_bounds_check.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/table_documentation.ipynb` & `heavylight-1.0.7/examples/notebook/table_documentation.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/table_documentation.md` & `heavylight-1.0.7/examples/notebook/table_documentation.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/table_maker.ipynb` & `heavylight-1.0.7/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/using_dataclasses.ipynb` & `heavylight-1.0.7/examples/notebook/using_dataclasses.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/vectors.ipynb` & `heavylight-1.0.7/examples/notebook/vectors.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/vectors.py` & `heavylight-1.0.7/examples/notebook/vectors.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv` & `heavylight-1.0.7/examples/notebook/example_tables/2017_loaded_CSO_mortality_rates_heavytable.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/notebook/table_documentation_files/table_documentation_32_1.png` & `heavylight-1.0.7/examples/notebook/table_documentation_files/table_documentation_32_1.png`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/protection_model.py` & `heavylight-1.0.7/examples/std_model/protection_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/protection_risk_model_generic.xlsx` & `heavylight-1.0.7/examples/std_model/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/run_model.py` & `heavylight-1.0.7/examples/std_model/run_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/tables/covert_q_x_tables.ipynb` & `heavylight-1.0.7/examples/std_model/tables/covert_q_x_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/tables/forward_rates.csv` & `heavylight-1.0.7/examples/std_model/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/tables/q_x_generic.csv` & `heavylight-1.0.7/examples/std_model/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/tables/qx_generic_raw.csv` & `heavylight-1.0.7/examples/std_model/tables/qx_generic_raw.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model/tables/uk_zero_spot.csv` & `heavylight-1.0.7/examples/std_model/tables/uk_zero_spot.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/protection_model.py` & `heavylight-1.0.7/examples/std_model_numpy/protection_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/protection_risk_model_generic.xlsx` & `heavylight-1.0.7/examples/std_model_numpy/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/run_model.py` & `heavylight-1.0.7/examples/std_model_numpy/run_model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/tables/covert_q_x_tables.ipynb` & `heavylight-1.0.7/examples/std_model_numpy/tables/covert_q_x_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/tables/forward_rates.csv` & `heavylight-1.0.7/examples/std_model_numpy/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/tables/q_x_generic.csv` & `heavylight-1.0.7/examples/std_model_numpy/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/tables/qx_generic_raw.csv` & `heavylight-1.0.7/examples/std_model_numpy/tables/qx_generic_raw.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/examples/std_model_numpy/tables/uk_zero_spot.csv` & `heavylight-1.0.7/examples/std_model_numpy/tables/uk_zero_spot.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/heavylight.py` & `heavylight-1.0.7/src/heavylight/heavylight.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,20 @@
         # cacheify
         self._cache_funcs()
 
         if do_run and proj_len > 0:
             self.RunModel(proj_len)
 
     def RunModel(self, proj_len: int):
+        """
+        Run the model if not already run.
+
+        Parameters
+        ----------
+        - proj_len: length of projection to run"""
         if self._is_run:
             # TODO: replace this with ability to run further, but warn that earlier values not recalculated?
             raise ValueError("Run has already been completed.")
         
         if hasattr(self, "BeforeRun"):
             self.BeforeRun()
 
@@ -140,21 +146,27 @@
     
     def _info(self):
         """Print info about the model"""
         for name, func in self._funcs.items():
             print(f"{name}: {func}")
         
     def ToDataFrame(self, param = 't'):
-        """return a pandas dataframe of all single parameter columns"""
+        """return a pandas dataframe of all single parameter columns
+        
+        Parameters
+        ----------
+        - param: parameter to filter on.  Default: `t`
+        """
         df = pd.DataFrame()
         for func in self._funcs:
             if self._funcs[func].has_one_param and self._funcs[func].param_names[0] == param:
                 df[func] = pd.Series(self._funcs[func].values)
 
         # if t is in the dataframe, move it to first position
         if "t" in df.columns:
             df.insert(0, "t", df.pop("t"))
         return df
     
     @property
     def df(self):
+        """return a pandas dataframe of all single parameter columns parameterised with `t`"""
         return self.ToDataFrame()
```

### Comparing `heavylight-1.0.6/src/heavylight/heavytables.py` & `heavylight-1.0.7/src/heavylight/heavytables.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 import numpy as np
 
 # Lookup classes
 # Each key column requires an input class which maps from the source datatype to an integer
 
 class IntegerLookup:
+    """An integer lookup - unsafe as doesn't check bounds"""
     def get(self, values):
         return values
 
 class IntegerLookupSafe:
     """An integer lookup that checks bounds"""
     def __init__(self, lower, upper):
         self.lower = lower
@@ -21,22 +22,38 @@
     def get(self, values):
         # TODO: replace np.all with np.any for faster failing (probably doesn't improve performance)
         if not np.all((self.lower <= values) & (values <= self.upper)):
             raise KeyError(f'values are not between table minimum ({self.lower}) and maximum ({self.upper})')
         return values
 
 class BoundIntLookup:
+    """An integer lookup that clips to the lowest and highest keys"""
     def __init__(self, lower, upper):
         self.lower = int(lower)
         self.upper = int(upper)
     
     def get(self, numpy_array):
         return np.clip(numpy_array, self.lower, self.upper)
 
+class StringLookup:
+    """A string lookup that include validation that the string match is exact"""
+    def __init__(self, string_vals):
+        self.string_vals = np.array(string_vals)
+    
+    def get(self, keys):
+        if isinstance(keys, np.ndarray):
+            if not all(np.isin(keys, self.string_vals)):
+                raise KeyError("invalid string key(s) passed into table lookup.")
+        else:
+            if not keys in self.string_vals:
+                raise KeyError("invalid string key(s) passed into table lookup.")   
+        return np.searchsorted(self.string_vals, keys)          
+
 class BandLookup:
+    """A lookup that matches on bands, using the np.searchsorted function"""
     def __init__(self, upper_bounds, labels):
         """Inputs must be sorted"""
         self.upper_bounds = np.array(upper_bounds)
         self.labels = np.array(labels)
 
     def get(self, numpy_array):
         """get the labels for vector"""
@@ -148,15 +165,21 @@
                 else:
                     self.mappers.append(IntegerLookup())
             elif col_type == "int_bound":
                 # bound integer forces values to be between the lowest and highest value in the table, for example maximum durations in mortality tables.
                 lower = df[col].min()
                 upper = df[col].max()
                 self.mappers.append(BoundIntLookup(lower=lower, upper=upper))
-            elif col_type in ["str", "band"]:
+            elif col_type == "str":
+                cols = df[col].unique()
+                string_mapper = StringLookup(cols)
+                self.mappers.append(string_mapper)
+                df_int_keys[col] = string_mapper.get(df_int_keys[col])
+
+            elif col_type in ["str_unsafe", "band"]:
                 df_col = pd.DataFrame(df[col].unique(), columns=["band_name"]).reset_index().sort_values("band_name")
 
                 # add a nan on the end so we get errors if the lookup fails
                 # as by default the BandLookup will return last item if no earlier matches
                 # commented out as it converts the datatype - we need these to be integers
                 # df_col.loc[len(df_col)] = len(df_col), np.nan
                 band_mapper = BandLookup.from_dataframe(df_col, "band_name", "index")
@@ -173,17 +196,16 @@
     def get(self, *keys):
         assert len(keys) == len(self.mappers)
         # TODO: if just one key then this doesn't work?  (needs fixed throughout)
         int_keys = [mapper.get(key) for key, mapper in zip(keys, self.mappers)]
         return self._int_key_table.get_value(*int_keys)
 
     def __getitem__(self, keys):
-        # print(keys, type(keys))
         if not isinstance(keys, tuple):
-            keys = keys, #force to be a tuple
+            keys = keys,    #force to be a tuple
         return self.get(*keys)
 
     def __repr__(self):
         # TODO: return a nice representation of the table, e.g. head/keys etc.
         return self.df.__repr__()
     
     @staticmethod
@@ -213,15 +235,16 @@
 
         # replace gaps with the fill value.
         df_rect[val_col] = df_rect[val_col] .fillna(fill)
         return df_rect
 
     @classmethod
     def read_excel(cls, spreadsheet_path, sheet_name):
-        """Read in a table from an excel sheet"""
+        """Read in a table from an excel sheet, for more control pass in the dataframe using `__init__`"""
         df = pd.read_excel(spreadsheet_path, sheet_name=sheet_name)
         return cls(df)
     
     @classmethod
     def read_csv(cls, csv_path):
+        """Read in a table from an csv file, for more control pass in the dataframe using `__init__`"""
         df = pd.read_csv(csv_path)
         return cls(df)
```

### Comparing `heavylight-1.0.6/src/heavylight/make_examples.py` & `heavylight-1.0.7/src/heavylight/make_examples.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/memory_optimized_cache.py` & `heavylight-1.0.7/src/heavylight/memory_optimized_cache.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/memory_optimized_model.py` & `heavylight-1.0.7/src/heavylight/memory_optimized_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,105 +10,128 @@
     """Default aggregation function for storing results."""
     if isinstance(x, np.ndarray) and issubclass(x.dtype.type, np.number):
         return np.sum(x)
     return x
 
 
 class LightModel:
-    """Base class to subclass from for recursive actuarial models.
-
-    Inheriting from this class causes functions starting with a lowercase letter to be cached.
-    A cached function will only be called once for each unique set of arguments.
-    Caching is necessary for recursive actuarial calculations to be efficient.
-
-    This means that the function will only be called once for each unique set of arguments, important for recursive actuarial models.
-
-    Parameters
-    ----------
-    agg_function: Callable[[int], Any], optional
-        This function is applied to the results of methods starting with a lowercase letter.
-
-    Class level methods:
-        RunModel(proj_len):
-        if the model has not been auto-run at initialisation, run it for projection length.
-
-    methods/variables to avoid:
-    methods/variables starting with an underscore `_` are treated as internal.  You may break functionality if you create your own.
+    """Inheriting from this class causes functions starting with a lowercase letter to be cached. 
+    The caches can be cleared to rerun the same instance with different data. 
+    This model can be memory optimized to reduce the memory requirements of the model without impacting results or performance. 
     """
 
     def __init__(self, agg_function: Union[Callable, None] = default_agg_function):
-        self.cache_graph = CacheGraph()
+        """**Arguments**
+
+        `agg_function`: Aggregation function for storing results. This function is applied to the return values of each method.
+         In memory optimized models the cache is cleared but the aggregated results are stored for reporting. 
+         If `agg_function` is not provided, the default aggregation function is used.
+         If `agg_function` is `None`, no aggregated results will be provided unless overridden at a method level with `agg`.
+
+        The implementation of the default aggregation function is as follows:
+
+        ```python
+        def default_agg_function(x: Any):
+            if isinstance(x, np.ndarray) and issubclass(x.dtype.type, np.number):
+                return np.sum(x)
+            return x
+        ```
+        """
+        self._cache_graph = CacheGraph()
         self._single_param_timestep_funcs: List[CacheMethod] = []
         self._funcs: Dict[MethodType, CacheMethod] = {}
+        self._ran_to: Union[int, None] = None
         # happens after setting up attributes
         for method_name, method in getmembers(self):
             if (
                 not method_name[0].islower()
                 or method_name.startswith("_")
                 or not isinstance(method, MethodType)
             ):
                 continue
             method_agg_function = getattr(method, "agg_function", None)
             if not hasattr(method, "agg_function"): # only provide class-level agg_function if method-level is not provided
                 method_agg_function = agg_function
-            cached_method = self.cache_graph(method_agg_function)(method)
+            cached_method = self._cache_graph(method_agg_function)(method)
             self._funcs[method] = cached_method
             is_single_param_t = check_single_parameter_name(method, "t")
             if is_single_param_t:
                 self._single_param_timestep_funcs.append(cached_method)
             setattr(self, method_name, cached_method)
 
     def RunModel(self, proj_len: int):
+        """**Arguments**
+
+        - `proj_len`: Projection length. All single parameter timestep functions will be run for each timestep in `range(proj_len + 1)`.
         """
-        Run the model for a projection length.
-        All single parameter timestep functions will be run for each timestep.
-        """
+        self.Clear()
+        self._ran_to = proj_len
+        self._run_model(proj_len)
+
+    def RunOptimized(self):
+        if self._ran_to is None:
+            raise ValueError("Model has not been run yet.")
+        self.ClearOptimize()
+        self._run_model(self._ran_to)
+
+    def _run_model(self, proj_len: int):
+        """shared logic between RunModel and RunOptimized"""
         for t in range(proj_len + 1):
             for func in self._single_param_timestep_funcs:
                 # We avoid recalling any functions that have already been cached, resolves issue #15 lewisfogden/heavylight
                 if (
                     not FunctionCall(func.func.__name__, (t,), frozenset())
-                    in self.cache_graph.all_calls
+                    in self._cache_graph.all_calls
                 ):
                     func(t)
 
-    def ResetCache(self):
-        """Reset the cache, useful if you want to run the model again with different parameters."""
-        self.cache_graph.reset()
 
-    def OptimizeMemoryAndReset(self):
-        """
-        Calling this clears the cache, and causes the cache to be optimized.
-        Optimizing the cache means that only needed results are stored, and intermediate results are cleared.
-        """
-        self.cache_graph.optimize_and_reset()
+    def Clear(self):
+        """Clears the cache. If the model was memory optimized, it is no longer memory optimized."""
+        self._cache_graph.reset()
+
+    def ClearOptimize(self):
+        """Clears the cache. The model is memory optimized after this function is called."""
+        self._cache_graph.optimize_and_reset()
 
     @property
-    def timestep_functions(self):
+    def _timestep_functions(self):
         """List the cached functions that have a single parameter `t`."""
         return [cache.func.__name__ for cache in self._single_param_timestep_funcs]
 
     @property
     def cache(self):
-        return self.cache_graph.cache
+        """
+        This is the cache of the model. It is a dictionary of dictionaries. 
+        The outer dictionary is keyed by the function name and the inner dictionary is keyed by the arguments.
+        """
+        return self._cache_graph.cache
 
     @property
     def cache_agg(self):
-        return self.cache_graph.cache_agg
+        """
+        The `cache` property with the `agg_function` applied to the results.
+        """
+        return self._cache_graph.cache_agg
 
     @property
     def df(self):
-        return self.ToDataFrame(is_agg=False)
+        """
+        A dataframe with the `cache` values of all functions that have a single parameter `t`.
+        """
+        return self._ToDataFrame(is_agg=False)
 
     @property
     def df_agg(self):
-        return self.ToDataFrame(is_agg=True)
+        """
+        The `df` property dataframe with the `agg_function` applied to the results.
+        """
+        return self._ToDataFrame(is_agg=True)
 
-    def ToDataFrame(self, param_name="t", is_agg=False):
-        """Return a pandas dataframe of all single parameter timestep results."""
+    def _ToDataFrame(self, param_name="t", is_agg=False):
         get_method_cache = _get_method_cache_factory(is_agg)
         filtered_cache = {}
         for method, cache_method in self._funcs.items():
             if not check_single_parameter_name(method, param_name):
                 continue
             if is_agg and cache_method.agg_func is None:
                 continue
@@ -122,16 +145,16 @@
 
 def check_single_parameter_name(func: Callable, name: str):
     sig = signature(func)
     return len(sig.parameters) == 1 and name in sig.parameters
 
 
 def agg(agg_function: Union[Callable, None]):
-    """
-    Register the storage function on a function.
+    """Register the storage function of a method.
+    
     Used for storing aggregated results before cache eviction to reduce memory consumption.
     """
 
     def decorator(func: Callable):
         func.agg_function = agg_function # type: ignore
         return func
```

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/protection_model_base.py` & `heavylight-1.0.7/src/heavylight/examples/protection/protection_model_base.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/protection_model_np.py` & `heavylight-1.0.7/src/heavylight/examples/protection/protection_model_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/protection_risk_model_generic.xlsx` & `heavylight-1.0.7/src/heavylight/examples/protection/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/run_model_base.py` & `heavylight-1.0.7/src/heavylight/examples/protection/run_model_base.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/run_model_np.py` & `heavylight-1.0.7/src/heavylight/examples/protection/run_model_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/tables/forward_rates.csv` & `heavylight-1.0.7/src/heavylight/examples/protection/tables/forward_rates.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/protection/tables/q_x_generic.csv` & `heavylight-1.0.7/src/heavylight/examples/protection/tables/q_x_generic.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/src/heavylight/examples/template/model.py` & `heavylight-1.0.7/src/heavylight/examples/template/model.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/tests/test_heavylight.py` & `heavylight-1.0.7/tests/test_heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/tests/test_lightmodel.py` & `heavylight-1.0.7/tests/test_lightmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,25 +46,25 @@
             return t
         return mult_factor * self.fib(t - 1, mult_factor) + self.fib(t - 2, mult_factor)
 
 def test_method_call_and_cache_retrievals():
     sm = SimpleModel(np.linspace(.1, 1, 10))
     sm.forward_rate(0)
     assert sm.forward_rate.cache[0] == .04
-    assert sm.cache_graph._caches['forward_rate'][((0,), frozenset())] == .04
-    assert sm.cache_graph.cache['forward_rate'][0] == .04
-    assert len(sm.cache_graph.cache) == 1
+    assert sm._cache_graph._caches['forward_rate'][((0,), frozenset())] == .04
+    assert sm._cache_graph.cache['forward_rate'][0] == .04
+    assert len(sm._cache_graph.cache) == 1
     assert len(sm.forward_rate.cache) == 1
     sm.forward_rate(5)
     assert len(sm.forward_rate.cache) == 2
-    assert len(sm.cache_graph.cache) == 1
+    assert len(sm._cache_graph.cache) == 1
 
 def test_timestep_functions():
     sm = SimpleModel(np.linspace(.1, 1, 10))
-    timestep_functions = sm.timestep_functions
+    timestep_functions = sm._timestep_functions
     expected_functions = ['t', 'num_pols_if', 'pols_death', 'cashflow', 'v', 'pv_cashflow', 'forward_rate']
     assert set(timestep_functions) == set(expected_functions) # no duplicates
 
 @pytest.mark.timeout(4)
 def test_caching_speedups():
     sm = SimpleModel(np.linspace(.1, 1, 10))
     assert len(sm.num_pols_if.cache) == 0
@@ -78,35 +78,32 @@
 
 def test_reset_cache():
     sm = SimpleModel(np.linspace(.1, 1, 10))
     sm.RunModel(5)
     assert round(np.sum(sm.pols_death.cache[0]), 10) == .055
     sm.mortality_rate = .02
     sm.RunModel(5)
-    assert round(np.sum(sm.pols_death.cache[0]), 10) == .055
-    sm.ResetCache()
-    sm.RunModel(5)
     assert round(np.sum(sm.pols_death.cache[0]), 10) == .11
 
 class TestPrettyCacheModel(LightModel):
     def __init__(self):
         super().__init__()
     def t(self, t):
         return self.wowee(t, 1) + self.zowee(t, x=1)
     def wowee(self, t, x):
         return 1
     def zowee(self, t, x):
         return 2
     
 def test_pretty_cache():
     pretty_model = TestPrettyCacheModel()
-    pretty_model.ResetCache()
+    pretty_model.Clear()
     pretty_model.RunModel(0)
-    assert pretty_model.cache_graph.cache['wowee'][(0,1)] == 1
+    assert pretty_model._cache_graph.cache['wowee'][(0,1)] == 1
     assert pretty_model.wowee.cache[(0,1)] == 1
-    assert pretty_model.cache_graph.cache['zowee'][((0,),frozenset({'x': 1}.items()))] == 2
+    assert pretty_model._cache_graph.cache['zowee'][((0,),frozenset({'x': 1}.items()))] == 2
     assert pretty_model.zowee.cache[((0,),frozenset({'x': 1}.items()))] == 2
-    assert pretty_model.cache_graph.cache['t'][0] == 3
+    assert pretty_model._cache_graph.cache['t'][0] == 3
     assert pretty_model.t.cache[0] == 3
     # can inject into the cache
     pretty_model.zowee[1] = 'hello cache'
     assert pretty_model.zowee.cache[1] == 'hello cache'
```

### Comparing `heavylight-1.0.6/tests/test_lightmodel_df.py` & `heavylight-1.0.7/tests/test_lightmodel_df.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/tests/test_memory_savings.py` & `heavylight-1.0.7/tests/test_memory_savings.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,42 +34,69 @@
     def forward_rate(self, t):
         return np.float64(0.04)
     
     def pv_cashflow(self, t):
         return self.cashflow(t) * self.v(t)
 
 def calculate_cache_graph_size(model: LightModel):
-    cg = model.cache_graph
+    cg = model._cache_graph
     return sum(val.nbytes for cache in cg._caches.values() for val in cache.values())
 
 def run_model_calculate_max_cache(model: SimpleModel, max_time: int):
     max_cache_size = 0
     for t in range(max_time+1):
         model.pv_cashflow(t)
         cache_size = calculate_cache_graph_size(model)
         max_cache_size = max(max_cache_size, cache_size)
     return max_cache_size
 
 def get_memory_savings_ratio(model: SimpleModel, max_time: int):
-    model.ResetCache()
+    model.Clear()
     max_cache_size = run_model_calculate_max_cache(model, max_time)
-    model.OptimizeMemoryAndReset()
+    model.ClearOptimize()
     optimized_max_cache_graph_size = run_model_calculate_max_cache(model, max_time)
     return optimized_max_cache_graph_size / max_cache_size
 
 @pytest.mark.timeout(4)
 def test_memory_savings():
     model = SimpleModel(np.ones((1000,)))
     assert get_memory_savings_ratio(model, 100) < .01
-    assert sum(model.cache_graph.cache_misses.values()) > 0 # verify that misses are being tracked
-    assert all(misses == 1 for misses in model.cache_graph.cache_misses.values())
+    assert sum(model._cache_graph.cache_misses.values()) > 0 # verify that misses are being tracked
+    assert all(misses == 1 for misses in model._cache_graph.cache_misses.values())
 
 def test_cache_misses():
     sm = SimpleModel(np.linspace(.1, 1, 10))
     sm.RunModel(5)
-    assert len(sm.cache_graph.cache_misses.values()) > 0
-    assert all(x == 1 for x in sm.cache_graph.cache_misses.values())
-    sm.OptimizeMemoryAndReset()
-    assert len(sm.cache_graph.cache_misses.values()) == 0
+    assert len(sm._cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm._cache_graph.cache_misses.values())
+    sm.ClearOptimize()
+    assert len(sm._cache_graph.cache_misses.values()) == 0
     sm.RunModel(5)
-    assert len(sm.cache_graph.cache_misses.values()) > 0
-    assert all(x == 1 for x in sm.cache_graph.cache_misses.values())
+    assert len(sm._cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm._cache_graph.cache_misses.values())
+
+def test_run_before_optimize():
+    sm = SimpleModel(
+        initial_pols_if=np.linspace(.1, 1, 10),
+        mortality_rate=.01)
+    with pytest.raises(ValueError):
+        sm.RunOptimized()
+
+def test_run_optimize():
+    sm = SimpleModel(
+        initial_pols_if=np.linspace(.1, 1, 10),
+        mortality_rate=.01)
+    sm.RunModel(5)
+    # optimized run works after normal run
+    sm.initial_pols_if = np.ones((10,))
+    sm.RunOptimized()
+    assert len(sm._cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm._cache_graph.cache_misses.values())
+    assert sm.num_pols_if.cache_agg[1] == 9.9
+    assert len(sm.num_pols_if.cache) == 0
+    # do it again
+    sm.initial_pols_if = np.ones((100,))
+    sm.RunOptimized()
+    assert len(sm._cache_graph.cache_misses.values()) > 0
+    assert all(x == 1 for x in sm._cache_graph.cache_misses.values())
+    assert round(sm.num_pols_if.cache_agg[1], 10) == 99
+    assert len(sm.num_pols_if.cache) == 0
```

### Comparing `heavylight-1.0.6/tests/test_optimized_cache.py` & `heavylight-1.0.7/tests/test_optimized_cache.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/.gitignore` & `heavylight-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/LICENSE` & `heavylight-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/README.md` & `heavylight-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.6/pyproject.toml` & `heavylight-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool]
+rye = { dev-dependencies = [
+    "pytest>=8.1.2",
+    "pytest-cov>=5.0.0",
+    "pytest-timeout>=2.3.1",
+    "numpy>=1.26.4",
+] }
+
 [tool.hatch.build.targets.wheel]
 src-dir = "src"
 
 [project]
 name = "heavylight"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
   { name="Matthew Caseres", email="matthewcaseres@outlook.com"}
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -27,14 +35,15 @@
     "pytest-timeout",
     "numpy"
 ]
 docs = [
     "mkdocs",
     "mkdocstrings[python]",
     "mkdocs-material",
+    "mkdocs-jupyter"
 ]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 testpaths = [
```

### Comparing `heavylight-1.0.6/PKG-INFO` & `heavylight-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: heavylight
-Version: 1.0.6
+Version: 1.0.7
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
 Project-URL: Documentation, https://lewisfogden.github.io/heavylight/
 Author-email: Lewis Fogden <lewisfogden@gmail.com>, Matthew Caseres <matthewcaseres@outlook.com>
 License-File: LICENSE
 Requires-Python: >=3.8
@@ -12,14 +12,15 @@
 Provides-Extra: dev
 Requires-Dist: numpy; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest==7.4.3; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
+Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/lewisfogden/heavylight/graph/badge.svg?token=P81UIDV4FZ)](https://codecov.io/gh/lewisfogden/heavylight)
 
 # heavylight
```

