# Comparing `tmp/mlforge-0.1.0a0.tar.gz` & `tmp/mlforge-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforge-0.1.0a0.tar", last modified: Mon Mar 11 12:17:59 2024, max compression
+gzip compressed data, was "mlforge-0.1.0b0.tar", last modified: Sun Apr 28 10:29:28 2024, max compression
```

## Comparing `mlforge-0.1.0a0.tar` & `mlforge-0.1.0b0.tar`

### file list

```diff
@@ -1,15 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:17:59.925848 mlforge-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-11 12:17:53.000000 mlforge-0.1.0a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-11 12:17:59.921848 mlforge-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-11 12:17:53.000000 mlforge-0.1.0a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 12:17:53.000000 mlforge-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 12:17:59.925848 mlforge-0.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-11 12:17:53.000000 mlforge-0.1.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:17:59.921848 mlforge-0.1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:17:59.921848 mlforge-0.1.0a0/src/mlforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-11 12:17:59.000000 mlforge-0.1.0a0/src/mlforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-11 12:17:59.000000 mlforge-0.1.0a0/src/mlforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:17:59.000000 mlforge-0.1.0a0/src/mlforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:17:59.000000 mlforge-0.1.0a0/src/mlforge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:17:59.921848 mlforge-0.1.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-03-11 12:17:53.000000 mlforge-0.1.0a0/tests/test_forge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:28.895562 mlforge-0.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-28 10:29:28.895562 mlforge-0.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:28.891562 mlforge-0.1.0b0/mlforge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/mlforge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/mlforge/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34237 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/mlforge/mlforge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/mlforge/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:28.891562 mlforge-0.1.0b0/mlforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-28 10:29:28.000000 mlforge-0.1.0b0/mlforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-28 10:29:28.000000 mlforge-0.1.0b0/mlforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:29:28.000000 mlforge-0.1.0b0/mlforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 10:29:28.000000 mlforge-0.1.0b0/mlforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:29:28.895562 mlforge-0.1.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:29:28.891562 mlforge-0.1.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_add_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_build_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_callable_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_get_method_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_get_step_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_parse_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_pbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-28 10:29:22.000000 mlforge-0.1.0b0/tests/test_run.py
```

### Comparing `mlforge-0.1.0a0/LICENSE.txt` & `mlforge-0.1.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.0a0/setup.py` & `mlforge-0.1.0b0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlforge",
-    version="0.1.0-alpha",
+    version="0.1.0-beta",
     author="J. Renero",
     author_email="jesus.renero@gmail.com",
     description="A package to design and run sequential ML pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/renero/mlforge",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
+    # package_dir={"": "mlforge"},
+    # packages=setuptools.find_packages(where="mlforge"),
+    packages=setuptools.find_packages(),
     python_requires=">=3.6"
 )
```

### Comparing `mlforge-0.1.0a0/tests/test_forge.py` & `mlforge-0.1.0b0/tests/test_parse_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """
 
-Tests for the forge module.
+Tests for the parse_step method.
 
 """
 # pylint: disable=E1101:no-member, W0201:attribute-defined-outside-init, W0511:fixme
 # pylint: disable=C0103:invalid-name, W0212:protected-access
 # pylint: disable=C0116:missing-function-docstring, C0115:missing-class-docstring
 # pylint: disable=R0913:too-many-arguments, R0903:too-few-public-methods
 # pylint: disable=R0914:too-many-locals, R0915:too-many-statements
 # pylint: disable=W0106:expression-not-assigned, R1702:too-many-branches
+# pylint: disable=C0413:wrong-import-position
 
-from ..src.forge import Pipeline
+import os
+import sys
+import pytest
 
+sys.path.insert(0, os.path.abspath(
+    os.path.join(os.path.dirname(__file__), '../mlforge')))
+
+from mlforge import Pipeline
 
 # Used to test access to global classes
 class SomeClass:
     def __init__(self):
         pass
 
     def method_name(self):
@@ -23,162 +30,133 @@
 
 
 def global_method():
     # Used to test access to global methods
     pass
 
 
-def test_parse_step():
-    """
-    Depending on the length, we can have different scenarios:
-
-        'method_name'
-        ClassHolder
-        ('method_name')
-        (ClassHolder)
-
-        ('method_name', ClassHolder)
-        ('new_attribute', 'method_name')
-        ('new_attribute', ClassHolder)
-        ('method_name', {'param1': 'value1'})
-
-        ('new_attribute', 'method_name', {'param1': 'value1'})
-        ('new_attribute', ClassHolder, {'param1': 'value1'})
-        ('method_name', ClassHolder, {'param1': 'value1'})
-
-        ('new_attribute', 'method_name', ClassHolder, {'param1': 'value1'})
-
-    """
-    forge = Pipeline()
-
-    # Test case 1: step_name is a string
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        "step_name")
-    assert attribute_name is None
-    assert method_name == "step_name"
-    assert class_name is None
-    assert arguments is None
-
-    # Test case 1b: step_name is a string
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("method_name"))
-    assert attribute_name is None
-    assert method_name == "method_name"
-    assert class_name is None
-    assert arguments is None
-
-    # Test case 1b: step_name is a string
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        (SomeClass))
-    assert attribute_name is None
-    assert method_name is None
-    assert class_name == SomeClass
-    assert arguments is None
-
-    # Test case 2: step_name is a tuple with length 2
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("attribute_name", "method_name"))
-    assert attribute_name == "attribute_name"
-    assert method_name == "method_name"
-    assert class_name is None
-    assert arguments is None
-
-    # Test case 2: step_name is a tuple with length 2
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("attribute_name", SomeClass))
-    assert attribute_name == "attribute_name"
-    assert method_name is None
-    assert class_name == SomeClass
-    assert arguments is None
-
-    # Test case 2b: step_name is a tuple with length 2
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("method_name", SomeClass))
-    assert attribute_name is None
-    assert method_name == "method_name"
-    assert class_name == SomeClass
-    assert arguments is None
-
-    # Test case 2c: step_name is a tuple with length 2
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("method_name", {"param": "value"}))
-    assert attribute_name is None
-    assert method_name == "method_name"
-    assert class_name is None
-    assert arguments == {"param": "value"}
-
-    # Test case 3: step_name is a tuple with length 3
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("method_name", SomeClass, {"param": "value"}))
-    assert attribute_name is None
-    assert method_name == "method_name"
-    assert class_name == SomeClass
-    assert arguments == {"param": "value"}
-
-    # Test case 3b: step_name is a tuple with length 3
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("attribute_name", "method_name", {"param": "value"}))
-    assert attribute_name == "attribute_name"
-    assert method_name == "method_name"
-    assert class_name is None
-    assert arguments == {"param": "value"}
-
-    # Test case 3c: step_name is a tuple with length 3
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("attribute_name", SomeClass, {"param": "value"}))
-    assert attribute_name == "attribute_name"
-    assert method_name is None
-    assert class_name == SomeClass
-    assert arguments == {"param": "value"}
-
-    # Test case 4: step_name is a tuple with length 4
-    attribute_name, method_name, class_name, arguments = forge._parse_step(
-        ("attribute_name", "method_name", SomeClass, {"param": "value"}))
-    assert attribute_name == "attribute_name"
-    assert method_name == "method_name"
-    assert class_name == SomeClass
-    assert arguments == {"param": "value"}
-
-
-def test_get_callable_method():
-    # Pipeline without host
-    forge = Pipeline()
-
-    # method_name is a method of SomeClass
-    method = forge._get_callable_method("method_name", SomeClass)
-    assert method is not None
-
-    # wrong_method is NOT a method of SomeClass
-    method = forge._get_callable_method("wrong_method", SomeClass)
-    assert method is None
-
-    # The class sent does not exist
-    try:
-        method = forge._get_callable_method(
-            "method_name", test_get_callable_method)
-        catch = False
-    except AttributeError:
-        catch = True
-    assert catch
-
-    # Now, with a host object
-    forge = Pipeline(host=SomeClass())
-
-    # Test case 1: method_name is a method of the host object
-    method = forge._get_callable_method("method_name")
-    assert method is not None
-
-    # Test case 2: method_name is a method in the pipeline object
-    # Create a method in the pipeline object
-    setattr(forge, "local_method", lambda: None)
-    method = forge._get_callable_method("local_method")
-    assert method is not None
-
-    # CANNOT test this since tests are in a different namespace
-    # Test case 3: method_name is a function in globals
-    # globals()["global_method"] = global_function
-    # method = forge._get_callable_method("global_method")
-    # assert method is not None
-
-    # Test case 4: method_name is not found
-    method = forge._get_callable_method("nonexistent_method")
-    assert method is None
+class Test_ParseStep:
+    def test_parse_step(self):
+        """
+        Depending on the length, we can have different scenarios:
+
+            'method_name'
+            ClassHolder
+            ('method_name')
+            (ClassHolder)
+
+            ('method_name', ClassHolder)
+            ('new_attribute', 'method_name')
+            ('new_attribute', ClassHolder)
+            ('method_name', {'param1': 'value1'})
+
+            ('new_attribute', 'method_name', {'param1': 'value1'})
+            ('new_attribute', ClassHolder, {'param1': 'value1'})
+            ('method_name', ClassHolder, {'param1': 'value1'})
+
+            ('new_attribute', 'method_name', ClassHolder, {'param1': 'value1'})
+
+        """
+        forge = Pipeline()
+
+        # Test case 1: step_name is a string
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            "step_name")
+        assert attribute_name is None
+        assert method_name == "step_name"
+        assert class_name is None
+        assert arguments is None
+
+        # Test case 1b: step_name is a string
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("method_name"))
+        assert attribute_name is None
+        assert method_name == "method_name"
+        assert class_name is None
+        assert arguments is None
+
+        # Test case 1b: step_name is a string
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            (SomeClass))
+        assert attribute_name is None
+        assert method_name is None
+        assert class_name == SomeClass
+        assert arguments is None
+
+        # Test case 2: step_name is a tuple with length 2
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("attribute_name", "method_name"))
+        assert attribute_name == "attribute_name"
+        assert method_name == "method_name"
+        assert class_name is None
+        assert arguments is None
+
+        # Test case 2: the method does not exists, so the __init__ method should be called.
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("attribute_name", SomeClass))
+        assert attribute_name == "attribute_name"
+        assert method_name is None
+        assert class_name == SomeClass
+        assert arguments is None
+
+        # Test case 2b: step_name is a tuple with length 2
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("method_name", SomeClass))
+        assert attribute_name is None
+        assert method_name == "method_name"
+        assert class_name == SomeClass
+        assert arguments is None
+
+        # Test case 2c: step_name is a tuple with length 2
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("method_name", {"param": "value"}))
+        assert attribute_name is None
+        assert method_name == "method_name"
+        assert class_name is None
+        assert arguments == {"param": "value"}
+
+        # Test case 3: step_name is a tuple with length 3
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("method_name", SomeClass, {"param": "value"}))
+        assert attribute_name is None
+        assert method_name == "method_name"
+        assert class_name == SomeClass
+        assert arguments == {"param": "value"}
+
+        # Test case 3b: step_name is a tuple with length 3
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("attribute_name", "method_name", {"param": "value"}))
+        assert attribute_name == "attribute_name"
+        assert method_name == "method_name"
+        assert class_name is None
+        assert arguments == {"param": "value"}
+
+        # Test case 3c: step_name is a tuple with length 3
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("attribute_name", SomeClass, {"param": "value"}))
+        assert attribute_name == "attribute_name"
+        assert method_name is None
+        assert class_name == SomeClass
+        assert arguments == {"param": "value"}
+
+        # Test case 4: step_name is a tuple with length 4
+        attribute_name, method_name, class_name, arguments = forge._parse_step(
+            ("attribute_name", "method_name", SomeClass, {"param": "value"}))
+        assert attribute_name == "attribute_name"
+        assert method_name == "method_name"
+        assert class_name == SomeClass
+        assert arguments == {"param": "value"}
+
+    def test_parse_step_raises_value_error(self):
+        forge = Pipeline()
+
+        # Test case 1: step_name is empty
+        with pytest.raises(AssertionError):
+            forge._parse_step(())
+
+        # Test case 2: step_name is a tuple with length 5
+        with pytest.raises(AssertionError):
+            forge._parse_step(("attribute_name", "method_name", SomeClass, {"param": "value"}, "extra"))
+
+        # Test case 3: step_name is a tuple with length 3, but the class does not exist
+        with pytest.raises(ValueError):
+            forge._parse_step(("attribute_name", "method_name", "SomeClass"))
```

