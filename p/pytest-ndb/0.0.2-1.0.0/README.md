# Comparing `tmp/pytest-ndb-0.0.2.tar.gz` & `tmp/pytest_ndb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ndb-0.0.2.tar", last modified: Sun Oct 15 15:14:55 2023, max compression
+gzip compressed data, was "pytest_ndb-1.0.0.tar", last modified: Sun Apr 28 14:00:40 2024, max compression
```

## Comparing `pytest-ndb-0.0.2.tar` & `pytest_ndb-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 15:14:55.134213 pytest-ndb-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2023-10-15 15:14:55.134213 pytest-ndb-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 15:14:55.130213 pytest-ndb-0.0.2/pytest_ndb/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/pytest_ndb/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/pytest_ndb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/pytest_ndb/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 15:14:55.134213 pytest-ndb-0.0.2/pytest_ndb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2023-10-15 15:14:55.000000 pytest-ndb-0.0.2/pytest_ndb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-15 15:14:55.000000 pytest-ndb-0.0.2/pytest_ndb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 15:14:55.000000 pytest-ndb-0.0.2/pytest_ndb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-15 15:14:55.000000 pytest-ndb-0.0.2/pytest_ndb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-15 15:14:55.000000 pytest-ndb-0.0.2/pytest_ndb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 15:14:55.134213 pytest-ndb-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 15:14:55.134213 pytest-ndb-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-10-15 15:14:43.000000 pytest-ndb-0.0.2/tests/test_pytest_ndb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:00:40.328460 pytest_ndb-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-28 14:00:40.328460 pytest_ndb-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:00:40.324459 pytest_ndb-1.0.0/pytest_ndb/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/pytest_ndb/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/pytest_ndb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:00:40.328460 pytest_ndb-1.0.0/pytest_ndb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-28 14:00:40.000000 pytest_ndb-1.0.0/pytest_ndb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-28 14:00:40.000000 pytest_ndb-1.0.0/pytest_ndb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 14:00:40.000000 pytest_ndb-1.0.0/pytest_ndb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-28 14:00:40.000000 pytest_ndb-1.0.0/pytest_ndb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 14:00:40.000000 pytest_ndb-1.0.0/pytest_ndb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 14:00:40.328460 pytest_ndb-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:00:40.328460 pytest_ndb-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-28 14:00:35.000000 pytest_ndb-1.0.0/tests/test_pytest_ndb.py
```

### Comparing `pytest-ndb-0.0.2/LICENSE` & `pytest_ndb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ndb-0.0.2/PKG-INFO` & `pytest_ndb-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pytest-ndb
-Version: 0.0.2
+Version: 1.0.0
 Summary: pytest notebook debugger
 Author-email: Richard Shadrach <rhshadrach@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rhshadrach/pytest-ndb
 Project-URL: documentation, https://github.com/rhshadrach/pytest-ndb
 Project-URL: repository, https://github.com/rhshadrach/pytest-ndb
 Project-URL: issues, https://github.com/rhshadrach/pytest-ndb/issues
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: codespell; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
@@ -29,23 +29,23 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest-ndb[doc,lint,test]; extra == "dev"
 
 # pytest-ndb
 
-Interactively debug a failing pytest test in a notebook or any REPL. See `Usage` below for examples.
+Interactively debug a failing pytest test in a notebook or REPL. See `Usage` below for examples.
 
-In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can often mean analyzing data, for which there is little support in a debugger and where notebooks truly shine.
+In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can mean having to analyze data, for which there is little support in a debugger and where notebooks truly shine.
 
 Traditionally to debug in a notebook, all of the code from the test, including fixtures and parametrizations, must be copied. For simple tests this might not be an issue, but for a complex test it can be quite time consuming. Instead, you can use `pytest-ndb`!
 
 ## Usage
 
-When tests fail, `pytest` will produce a summary of the failures such as follows.
+When tests fail, `pytest` will produce a summary of the failures.
 
 ```
 FAILED pytest_ndb/tests.py::test_fixture_single_fails - AssertionError: assert 'x' == 'y'
 FAILED pytest_ndb/tests.py::test_fixture_double_fails - AssertionError: assert 'y' == 'x'
 FAILED pytest_ndb/tests.py::test_parametrization_fails[5] - AssertionError: assert 'z' == 'w'
 ```
 
@@ -91,23 +91,23 @@
 test_locals = pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_parametrization_fails[5]")
 ```
 
 ## Requirements
 
 `pytest-ndb` requires:
 
- - At least Python 3.7.
- - pytest between versions `7.0.0` and `7.4.0`. Other versions **may** work.
+ - At least Python 3.8.
+ - pytest between versions `7.0` and `8.2` inclusive. Other versions **may** work.
  - The test path provided to `pytets-ndb` must identify a unique test (only one parametrization).
  - If parametrizations are used, they must be deterministic.
 
 ## Installation
 
 ```bash
 pip install pytest-ndb
 ```
 
 ## Development state
 
-`pytest-ndb` is largely a hack on the `pytest` internals, and likely always will be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
+`pytest-ndb` is largely a hack on the `pytest` internals, and likely will always be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
 
-This package is rather new, and so users should not be surprised to encounter issues. Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
+Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
```

### Comparing `pytest-ndb-0.0.2/README.md` & `pytest_ndb-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pytest-ndb
 
-Interactively debug a failing pytest test in a notebook or any REPL. See `Usage` below for examples.
+Interactively debug a failing pytest test in a notebook or REPL. See `Usage` below for examples.
 
-In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can often mean analyzing data, for which there is little support in a debugger and where notebooks truly shine.
+In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can mean having to analyze data, for which there is little support in a debugger and where notebooks truly shine.
 
 Traditionally to debug in a notebook, all of the code from the test, including fixtures and parametrizations, must be copied. For simple tests this might not be an issue, but for a complex test it can be quite time consuming. Instead, you can use `pytest-ndb`!
 
 ## Usage
 
-When tests fail, `pytest` will produce a summary of the failures such as follows.
+When tests fail, `pytest` will produce a summary of the failures.
 
 ```
 FAILED pytest_ndb/tests.py::test_fixture_single_fails - AssertionError: assert 'x' == 'y'
 FAILED pytest_ndb/tests.py::test_fixture_double_fails - AssertionError: assert 'y' == 'x'
 FAILED pytest_ndb/tests.py::test_parametrization_fails[5] - AssertionError: assert 'z' == 'w'
 ```
 
@@ -58,23 +58,23 @@
 test_locals = pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_parametrization_fails[5]")
 ```
 
 ## Requirements
 
 `pytest-ndb` requires:
 
- - At least Python 3.7.
- - pytest between versions `7.0.0` and `7.4.0`. Other versions **may** work.
+ - At least Python 3.8.
+ - pytest between versions `7.0` and `8.2` inclusive. Other versions **may** work.
  - The test path provided to `pytets-ndb` must identify a unique test (only one parametrization).
  - If parametrizations are used, they must be deterministic.
 
 ## Installation
 
 ```bash
 pip install pytest-ndb
 ```
 
 ## Development state
 
-`pytest-ndb` is largely a hack on the `pytest` internals, and likely always will be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
+`pytest-ndb` is largely a hack on the `pytest` internals, and likely will always be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
 
-This package is rather new, and so users should not be surprised to encounter issues. Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
+Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
```

### Comparing `pytest-ndb-0.0.2/pyproject.toml` & `pytest_ndb-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "pytest-ndb"
 authors = [
     {name = "Richard Shadrach", email = "rhshadrach@gmail.com"},
 ]
 description = "pytest notebook debugger"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = ["pytest"]
 dynamic = ["version"]
```

### Comparing `pytest-ndb-0.0.2/pytest_ndb/__init__.py` & `pytest_ndb-1.0.0/pytest_ndb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,20 +72,22 @@
     Returns:
         Local variables from the test, regardless if the test succeeds or fails.
     """
     from _pytest.config import _prepareconfig
     from _pytest.config.exceptions import UsageError
     from _pytest.fixtures import FixtureRequest
     from _pytest.main import Session
+    from _pytest.runner import SetupState
 
     # We don't understand what finalizers do, and they seem to cause issues. So far
     # disabling them entirely has worked.
     def disable_finalizers(*args, **kwargs):
         pass
 
+    SetupState.addfinalizer = disable_finalizers
     FixtureRequest._schedule_finalizers = disable_finalizers
 
     path = (Path(package.__file__).parent / "..").resolve()
     if path.parts[-1] == "src":
         # Go up one more level
         path = path / ".."
     path = path / test
@@ -108,30 +110,24 @@
 
     # Only one test is supported
     if len(session.items) == 0:
         raise ValueError(f"No tests found with for {test}")
     elif len(session.items) > 1:
         raise ValueError(f"Multiple tests found for {test}")
 
-    session_test = session.items[0]
-    request = session_test._request
+    item = session.items[0]
+    request = item._request
 
     kwargs = {}
-    for name in session_test.fixturenames:
-        # The request fixture doesn't require any setup
-        if name != "request":
-            fixturedef = session_test._fixtureinfo.name2fixturedefs[name][0]
-            request._compute_fixture_value(fixturedef)
+    for name in item.fixturenames:
         kwargs[name] = request.getfixturevalue(name)
 
-    test_function = _persistent_locals(session_test.function)
+    test_function = _persistent_locals(item.function)
     try:
-        test_function(
-            **{arg: kwargs[arg] for arg in session_test._fixtureinfo.argnames}
-        )
+        test_function(**{arg: kwargs[arg] for arg in item._fixtureinfo.argnames})
     except Exception:
         traceback.print_exc()
     finally:
         result = {
             k: v for k, v in test_function.locals.items() if not _is_pytest_internal(k)
         }
         return result
```

### Comparing `pytest-ndb-0.0.2/pytest_ndb.egg-info/PKG-INFO` & `pytest_ndb-1.0.0/pytest_ndb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pytest-ndb
-Version: 0.0.2
+Version: 1.0.0
 Summary: pytest notebook debugger
 Author-email: Richard Shadrach <rhshadrach@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rhshadrach/pytest-ndb
 Project-URL: documentation, https://github.com/rhshadrach/pytest-ndb
 Project-URL: repository, https://github.com/rhshadrach/pytest-ndb
 Project-URL: issues, https://github.com/rhshadrach/pytest-ndb/issues
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: codespell; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
@@ -29,23 +29,23 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest-ndb[doc,lint,test]; extra == "dev"
 
 # pytest-ndb
 
-Interactively debug a failing pytest test in a notebook or any REPL. See `Usage` below for examples.
+Interactively debug a failing pytest test in a notebook or REPL. See `Usage` below for examples.
 
-In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can often mean analyzing data, for which there is little support in a debugger and where notebooks truly shine.
+In our opinion, developers should often prefer to debug failing tests using a debugger such as `pdb`. However for certain applications, such as those that occur in data science with large complex data sets or long running models, this is can be quite difficult. Debugging a failing test can mean having to analyze data, for which there is little support in a debugger and where notebooks truly shine.
 
 Traditionally to debug in a notebook, all of the code from the test, including fixtures and parametrizations, must be copied. For simple tests this might not be an issue, but for a complex test it can be quite time consuming. Instead, you can use `pytest-ndb`!
 
 ## Usage
 
-When tests fail, `pytest` will produce a summary of the failures such as follows.
+When tests fail, `pytest` will produce a summary of the failures.
 
 ```
 FAILED pytest_ndb/tests.py::test_fixture_single_fails - AssertionError: assert 'x' == 'y'
 FAILED pytest_ndb/tests.py::test_fixture_double_fails - AssertionError: assert 'y' == 'x'
 FAILED pytest_ndb/tests.py::test_parametrization_fails[5] - AssertionError: assert 'z' == 'w'
 ```
 
@@ -91,23 +91,23 @@
 test_locals = pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_parametrization_fails[5]")
 ```
 
 ## Requirements
 
 `pytest-ndb` requires:
 
- - At least Python 3.7.
- - pytest between versions `7.0.0` and `7.4.0`. Other versions **may** work.
+ - At least Python 3.8.
+ - pytest between versions `7.0` and `8.2` inclusive. Other versions **may** work.
  - The test path provided to `pytets-ndb` must identify a unique test (only one parametrization).
  - If parametrizations are used, they must be deterministic.
 
 ## Installation
 
 ```bash
 pip install pytest-ndb
 ```
 
 ## Development state
 
-`pytest-ndb` is largely a hack on the `pytest` internals, and likely always will be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
+`pytest-ndb` is largely a hack on the `pytest` internals, and likely will always be. In addition, we must guess at the root path of your package, and in certain cases we may guess wrong. While we test this package using parametrizations and fixtures, other `pytest` features may not work.
 
-This package is rather new, and so users should not be surprised to encounter issues. Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
+Is something not working? Report an issue on our [GitHub issue tracker](https://github.com/rhshadrach/pytest-ndb/issues)!
```

### Comparing `pytest-ndb-0.0.2/tests/test_pytest_ndb.py` & `pytest_ndb-1.0.0/tests/test_pytest_ndb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 import pytest
 
 import pytest_ndb
 
+from . import package
+
 
 def test_basic_passes():
     expected = {"x": 5}
-    result = pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_basic_passes")
+    result = pytest_ndb.run(package, "package/tests.py::test_basic_passes")
     assert result == expected
 
 
 def test_basic_fails():
     expected = {"x": 5}
-    result = pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_basic_fails")
+    result = pytest_ndb.run(package, "package/tests.py::test_basic_fails")
     assert result == expected
 
 
 def test_incorrect_path():
-    msg = "No tests found for pytest_ndb/tests.py::test_foo"
+    msg = "No tests found for package/tests.py::test_foo"
     with pytest.raises(ValueError, match=msg):
-        pytest_ndb.run(pytest_ndb, "pytest_ndb/tests.py::test_foo")
+        pytest_ndb.run(package, "package/tests.py::test_foo")
 
 
 def test_fixture_single_passes():
-    path = "pytest_ndb/tests.py::test_fixture_single_passes"
+    path = "package/tests.py::test_fixture_single_passes"
     expected = {"fixture_1": "x", "x": 5}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
 
 
 def test_fixture_single_fails():
-    path = "pytest_ndb/tests.py::test_fixture_single_fails"
+    path = "package/tests.py::test_fixture_single_fails"
     expected = {"fixture_1": "x", "x": 5}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
 
 
 def test_fixture_double_passes():
-    path = "pytest_ndb/tests.py::test_fixture_double_passes"
+    path = "package/tests.py::test_fixture_double_passes"
     expected = {"fixture_1": "x", "fixture_2": "y", "x": 5}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
 
 
 def test_fixture_double_fails():
-    path = "pytest_ndb/tests.py::test_fixture_double_fails"
+    path = "package/tests.py::test_fixture_double_fails"
     expected = {"fixture_1": "x", "fixture_2": "y", "x": 5}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
 
 
 def test_parametrization_passes():
-    path = "pytest_ndb/tests.py::test_parametrization_passes[5]"
+    path = "package/tests.py::test_parametrization_passes[5]"
     expected = {"x": 5, "y": "z"}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
 
 
 def test_parametrization_fails():
-    path = "pytest_ndb/tests.py::test_parametrization_fails[5]"
+    path = "package/tests.py::test_parametrization_fails[5]"
     expected = {"x": 5, "y": "z"}
-    result = pytest_ndb.run(pytest_ndb, path)
+    result = pytest_ndb.run(package, path)
     assert result == expected
```

