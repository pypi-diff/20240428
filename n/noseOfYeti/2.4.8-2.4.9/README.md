# Comparing `tmp/noseofyeti-2.4.8.tar.gz` & `tmp/noseofyeti-2.4.9.tar.gz`

## Comparing `noseofyeti-2.4.8.tar` & `noseofyeti-2.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/pytest.ini
--rwxr-xr-x   0        0        0     1273 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/run.sh
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/test.sh
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/example/converted.test.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/example/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/version.py
--rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/black/Grammar.noy.txt
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/black/noy_black.pth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/__init__.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/black_compat.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/mypy.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/nosetests.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/pylama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/pyls.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/plugins/pytest.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/chooser.py
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/containers.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/spec_codec.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/support.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/tokeniser.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/tokens.py
--rw-r--r--   0        0        0    21768 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/noseOfYeti/tokeniser/tracker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/__init__.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/conftest.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_chooser_test.py
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_complex_tokeniser.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_formatting.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_mismatched_brackets.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_nesting_tokeniser.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_pylama.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_spec_codec.py
--rw-r--r--   0        0        0    18605 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_translation_tokeniser.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/test_using_pytest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_formatting_and_pylama/failing_pylama_spec.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_formatting_and_pylama/formatted_normal.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_formatting_and_pylama/formatted_spec.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_formatting_and_pylama/unformatted_normal.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_formatting_and_pylama/unformatted_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_pytest_plugin/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_pytest_plugin/conftest.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_pytest_plugin/test_one.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tests/for_pytest_plugin/test_two.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tools/bootstrap_venvstarter.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tools/devtools.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tools/requirements.dev.txt
--rwxr-xr-x   0        0        0     1470 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/tools/venv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/README.rst
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/pyproject.toml
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 noseofyeti-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/pytest.ini
+-rwxr-xr-x   0        0        0     1273 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/run.sh
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/test.sh
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/example/converted.test.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/example/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/version.py
+-rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/black/Grammar.noy.txt
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/black/noy_black.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/__init__.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/black_compat.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/mypy.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/nosetests.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/pylama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/pyls.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/plugins/pytest.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/chooser.py
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/containers.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/spec_codec.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/support.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/tokeniser.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/tokens.py
+-rw-r--r--   0        0        0    21768 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/noseOfYeti/tokeniser/tracker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/__init__.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/conftest.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_chooser_test.py
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_complex_tokeniser.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_formatting.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_mismatched_brackets.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_nesting_tokeniser.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_pylama.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_spec_codec.py
+-rw-r--r--   0        0        0    18605 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_translation_tokeniser.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/test_using_pytest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_formatting_and_pylama/failing_pylama_spec.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_formatting_and_pylama/formatted_normal.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_formatting_and_pylama/formatted_spec.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_formatting_and_pylama/unformatted_normal.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_formatting_and_pylama/unformatted_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_pytest_plugin/conftest.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_pytest_plugin/test_one.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tests/for_pytest_plugin/test_two.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tools/bootstrap_venvstarter.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tools/devtools.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tools/requirements.dev.txt
+-rwxr-xr-x   0        0        0     1470 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/tools/venv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/README.rst
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 noseofyeti-2.4.9/PKG-INFO
```

### Comparing `noseofyeti-2.4.8/run.sh` & `noseofyeti-2.4.9/run.sh`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/example/converted.test.py` & `noseofyeti-2.4.9/example/converted.test.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/example/test.py` & `noseofyeti-2.4.9/example/test.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/black/Grammar.noy.txt` & `noseofyeti-2.4.9/noseOfYeti/black/Grammar.noy.txt`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/plugins/black_compat.py` & `noseofyeti-2.4.9/noseOfYeti/plugins/black_compat.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/plugins/nosetests.py` & `noseofyeti-2.4.9/noseOfYeti/plugins/nosetests.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/plugins/pylama.py` & `noseofyeti-2.4.9/noseOfYeti/plugins/pylama.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/plugins/pyls.py` & `noseofyeti-2.4.9/noseOfYeti/plugins/pyls.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/plugins/pytest.py` & `noseofyeti-2.4.9/noseOfYeti/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/chooser.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/chooser.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/containers.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/containers.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/spec_codec.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/spec_codec.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/support.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/support.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/tokeniser.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/tokeniser.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/tokens.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/tokens.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/noseOfYeti/tokeniser/tracker.py` & `noseofyeti-2.4.9/noseOfYeti/tokeniser/tracker.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/conftest.py` & `noseofyeti-2.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_chooser_test.py` & `noseofyeti-2.4.9/tests/test_chooser_test.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_complex_tokeniser.py` & `noseofyeti-2.4.9/tests/test_complex_tokeniser.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_formatting.py` & `noseofyeti-2.4.9/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_mismatched_brackets.py` & `noseofyeti-2.4.9/tests/test_mismatched_brackets.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_nesting_tokeniser.py` & `noseofyeti-2.4.9/tests/test_nesting_tokeniser.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_pylama.py` & `noseofyeti-2.4.9/tests/test_pylama.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_spec_codec.py` & `noseofyeti-2.4.9/tests/test_spec_codec.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_translation_tokeniser.py` & `noseofyeti-2.4.9/tests/test_translation_tokeniser.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/test_using_pytest.py` & `noseofyeti-2.4.9/tests/test_using_pytest.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/for_pytest_plugin/test_one.py` & `noseofyeti-2.4.9/tests/for_pytest_plugin/test_one.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tests/for_pytest_plugin/test_two.py` & `noseofyeti-2.4.9/tests/for_pytest_plugin/test_two.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tools/bootstrap_venvstarter.py` & `noseofyeti-2.4.9/tools/bootstrap_venvstarter.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tools/devtools.py` & `noseofyeti-2.4.9/tools/devtools.py`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/tools/venv` & `noseofyeti-2.4.9/tools/venv`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/LICENSE` & `noseofyeti-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/README.rst` & `noseofyeti-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `noseofyeti-2.4.8/pyproject.toml` & `noseofyeti-2.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 [project.optional-dependencies]
 black = [
     "black==24.2.0",
     "importlib-resources==5.10.0",
 ]
 tests = [
     "alt-pytest-asyncio==0.6.0",
-    "asynctest==0.13.0",
     "pytest-helpers-namespace==2021.4.29",
     "pytest>=7.0.1",
 ]
 
 [project.entry-points."nose.plugins"]
 noseOfYeti = "noseOfYeti.plugins.nosetests:Plugin"
```

### Comparing `noseofyeti-2.4.8/PKG-INFO` & `noseofyeti-2.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: noseOfYeti
-Version: 2.4.8
+Version: 2.4.9
 Summary: A custom python codec that provides an RSpec style dsl for python
 Project-URL: Homepage, https://github.com/delfick/nose-of-yeti
 Author-email: Stephen Moore <stephen@delfick.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bdd,rspec,spec
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Provides-Extra: black
 Requires-Dist: black==24.2.0; extra == 'black'
 Requires-Dist: importlib-resources==5.10.0; extra == 'black'
 Provides-Extra: tests
 Requires-Dist: alt-pytest-asyncio==0.6.0; extra == 'tests'
-Requires-Dist: asynctest==0.13.0; extra == 'tests'
 Requires-Dist: pytest-helpers-namespace==2021.4.29; extra == 'tests'
 Requires-Dist: pytest>=7.0.1; extra == 'tests'
 Description-Content-Type: text/x-rst
 
 Nose of Yeti
 ============
```

