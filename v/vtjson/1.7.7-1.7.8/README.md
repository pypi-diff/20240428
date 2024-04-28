# Comparing `tmp/vtjson-1.7.7.tar.gz` & `tmp/vtjson-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.7.tar", last modified: Mon Apr 22 15:19:02 2024, max compression
+gzip compressed data, was "vtjson-1.7.8.tar", last modified: Sun Apr 28 05:42:54 2024, max compression
```

## Comparing `vtjson-1.7.7.tar` & `vtjson-1.7.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:19:02.207346 vtjson-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 15:18:57.000000 vtjson-1.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-22 15:19:02.207346 vtjson-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-22 15:18:57.000000 vtjson-1.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-22 15:18:57.000000 vtjson-1.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:19:02.207346 vtjson-1.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:19:02.207346 vtjson-1.7.7/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-22 15:19:02.000000 vtjson-1.7.7/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-22 15:19:02.000000 vtjson-1.7.7/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:19:02.000000 vtjson-1.7.7/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 15:19:02.000000 vtjson-1.7.7/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 15:19:02.000000 vtjson-1.7.7/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    29722 2024-04-22 15:18:57.000000 vtjson-1.7.7/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:42:54.975399 vtjson-1.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-28 05:42:50.000000 vtjson-1.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 05:42:54.975399 vtjson-1.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19109 2024-04-28 05:42:50.000000 vtjson-1.7.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 05:42:50.000000 vtjson-1.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:42:54.975399 vtjson-1.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:42:54.975399 vtjson-1.7.8/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 05:42:54.000000 vtjson-1.7.8/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30742 2024-04-28 05:42:50.000000 vtjson-1.7.8/vtjson.py
```

### Comparing `vtjson-1.7.7/LICENSE` & `vtjson-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.7/PKG-INFO` & `vtjson-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.7
+Version: 1.7.8
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dnspython
 Requires-Dist: email_validator
 Requires-Dist: idna
+Requires-Dist: python-magic
 
 # vtjson
 A lightweight package for validating JSON like Python objects.
 
 ## Schemas
 
 Validation of JSON like Python objects is done according to a `schema` which is somewhat inspired by a typescript type. The format of a schema is more or less self explanatory as the following example shows.
@@ -225,14 +226,15 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
```

### Comparing `vtjson-1.7.7/README.md` & `vtjson-1.7.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
```

### Comparing `vtjson-1.7.7/pyproject.toml` & `vtjson-1.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "vtjson"
 dynamic = ["version"]
 authors = [
   { name="Michel Van den Bergh", email="michel.vandenbergh@uhasselt.be" },
 ]
 description = "A lightweight package for validating JSON like Python objects"
 readme = "README.md"
-dependencies = ["dnspython", "email_validator", "idna"]
+dependencies = ["dnspython", "email_validator", "idna", "python-magic"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `vtjson-1.7.7/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.8/vtjson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.7
+Version: 1.7.8
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dnspython
 Requires-Dist: email_validator
 Requires-Dist: idna
+Requires-Dist: python-magic
 
 # vtjson
 A lightweight package for validating JSON like Python objects.
 
 ## Schemas
 
 Validation of JSON like Python objects is done according to a `schema` which is somewhat inspired by a typescript type. The format of a schema is more or less self explanatory as the following example shows.
@@ -225,14 +226,15 @@
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
+- `magic(mime_type, name=None)`. Checks if a buffer (for example a string or a byte array) has the given mime type. This is implemented using the `python-magic` package.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
 - `email`. Checks if the object is a valid email address. This uses the package `email_validator`. The `email` schema accepts the same options as `validate_email` in loc. cit.
 - `ip_address` and `url`. These are similar to `email`.
 - `domain_name(ascii_only=True, resolve=False)`. Checks if the object is a valid domain name. If `ascii_only=False` then allow IDNA domain names. If `resolve=True` check if the domain name resolves.
 - `date_time(format=None)`. Without argument this represents an ISO 8601 date-time. The `format` argument represents a format string for `strftime`.
 - `date` and `time`. These represent an ISO 8601 date and an ISO 8601 time.
```

### Comparing `vtjson-1.7.7/vtjson.py` & `vtjson-1.7.8/vtjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 import re
 import urllib.parse
 
 import dns.resolver
 import email_validator
 import idna
 
+MAGIC_AVAILABLE = True
+try:
+    import magic as magic_
+except Exception:
+    MAGIC_AVAILABLE = False
+
 
 class ValidationError(Exception):
     pass
 
 
 class SchemaError(Exception):
     pass
@@ -23,15 +29,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.7"
+__version__ = "1.7.8"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -300,14 +306,42 @@
                 return ""
             else:
                 return _wrong_type_message(object, name, self.__name__)
         except Exception as e:
             return _wrong_type_message(object, name, self.__name__, str(e))
 
 
+class magic:
+    def __init__(self, mime_type, name=None):
+        if not MAGIC_AVAILABLE:
+            raise SchemaError("Failed to load python-magic")
+
+        if not isinstance(mime_type, str):
+            raise SchemaError(f"{repr(mime_type)} is not a string")
+
+        self.mime_type = mime_type
+
+        if name is None:
+            self.__name__ = f"magic({repr(mime_type)})"
+        else:
+            self.__name__ = name
+
+    def __validate__(self, object, name, strict):
+        try:
+            object_mime_type = magic_.from_buffer(object, mime=True)
+        except Exception as e:
+            return _wrong_type_message(object, name, self.__name__, str(e))
+        if object_mime_type != self.mime_type:
+            return (
+                f"The mime type of {name} is equal to {repr(object_mime_type)} "
+                f"which is different from {repr(self.mime_type)}"
+            )
+        return ""
+
+
 class div:
     def __init__(self, divisor, remainder=0, name=None):
         if not isinstance(divisor, int):
             raise SchemaError(f"The divisor {repr(divisor)} is not an integer")
         if divisor == 0:
             raise SchemaError("The divisor cannot be zero")
         if not isinstance(remainder, int):
```

