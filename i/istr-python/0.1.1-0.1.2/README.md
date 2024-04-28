# Comparing `tmp/istr_python-0.1.1.tar.gz` & `tmp/istr_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.1.tar", last modified: Fri Apr 26 12:45:20 2024, max compression
+gzip compressed data, was "istr_python-0.1.2.tar", last modified: Sat Apr 27 16:58:03 2024, max compression
```

## Comparing `istr_python-0.1.1.tar` & `istr_python-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.410875 istr_python-0.1.1/
--rw-rw-rw-   0        0        0    10334 2024-04-26 12:45:20.408875 istr_python-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9420 2024-04-26 11:01:42.000000 istr_python-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.376413 istr_python-0.1.1/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.1/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.1/istr/install istr.py
--rw-rw-rw-   0        0        0    15477 2024-04-26 12:43:24.000000 istr_python-0.1.1/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.406571 istr_python-0.1.1/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10334 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      616 2024-04-26 12:45:13.000000 istr_python-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 12:45:20.411875 istr_python-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.403564 istr_python-0.1.1/tests/
--rw-rw-rw-   0        0        0    11418 2024-04-25 11:05:24.000000 istr_python-0.1.1/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.589473 istr_python-0.1.2/
+-rw-rw-rw-   0        0        0    10334 2024-04-27 16:58:03.585523 istr_python-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9420 2024-04-26 11:01:42.000000 istr_python-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.537898 istr_python-0.1.2/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.2/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.2/istr/install istr.py
+-rw-rw-rw-   0        0        0    18172 2024-04-27 16:04:34.000000 istr_python-0.1.2/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.582447 istr_python-0.1.2/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10334 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-27 16:58:03.000000 istr_python-0.1.2/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      658 2024-04-27 16:57:58.000000 istr_python-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 16:58:03.591476 istr_python-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 16:58:03.579798 istr_python-0.1.2/tests/
+-rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.2/tests/test_istr.py
```

### Comparing `istr_python-0.1.1/PKG-INFO` & `istr_python-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-0.1.1/README.md` & `istr_python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.1/istr/install istr.py` & `istr_python-0.1.2/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.1/istr/istr.py` & `istr_python-0.1.2/istr/istr.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 import functools
 import math
 
 """
 changelog
 
+version 0.1.2  2024-04-26  
+-------------------------
+Added all relevant string methods to return istrs or data structures with istrs.
+Added corresponding tests.
+
 version 0.1.0  2024-04-22  
 -------------------------
-Changed the way istr.range is implemenented.
+Changed the way istr.range is implemennted.
 
 Changed the context manager istr.format() to be used directly without the with statement.
 Also, noww istr.format() works without any argument and then returns the current format.
 
 istr class now uses __slots__
 
 All internal values and methods now start with an underscore.
@@ -34,14 +39,15 @@
 
 
 version 0.0.8  2024-04-18  
 -------------------------
 initial version with changelog
 """
 
+
 class _range:
     """
     based on https://codereview.stackexchange.com/questions/229073/pure-python-range-implementation
     """
 
     def __init__(self, cls, start, stop=None, step=1):
         if stop is None:
@@ -243,26 +249,28 @@
             raise TypeError("no parameter given")
         if len(value) == 1:
             value = value[0]  # normal case of 1 parameter
         if isinstance(value, range):
             return cls.range(value.start, value.stop, value.step)
         if isinstance(value, _range):
             return value
+        if isinstance(value, cls):
+            return value
         if isinstance(value, dict):
             return type(value)((k, cls(v)) for k, v in value.items())
         if not isinstance(value, (str, type)) and hasattr(value, "__iter__"):
             if hasattr(value, "__next__"):
                 return map(functools.partial(cls), value)
             return type(value)(map(functools.partial(cls), value))
         if value == "":
             as_str = ""
             as_int = 0
         else:
             as_int = cls._to_int(value)
-            if (cls._format == "" or cls._base != 10) and not isinstance(value,istr):
+            if (cls._format == "" or cls._base != 10) and not isinstance(value, istr):
                 if isinstance(value, str):
                     as_str = value
                 else:
                     if cls._base == 10:
                         as_str = str(as_int)
                     else:
                         as_str = istr._to_base(as_int, cls._base)
@@ -402,18 +410,14 @@
 
     def is_even(self):
         return self._as_int % 2 == 0
 
     def is_odd(self):
         return self._as_int % 2 == 1
 
-    def join(self, iterable):
-        s = super().join(iterable)
-        return self.__class__(s)
-
     def reversed(self):
         return self[::-1]
 
     def __getitem__(self, key):
         return self.__class__(super().__getitem__(key))
 
     @classmethod
@@ -483,23 +487,98 @@
         def __enter__(self):
             ...
 
         def __exit__(self, exc_type, exc_value, exc_tb):
             self.saved_cls._base = self.saved_base
 
     @classmethod
-    def range(cls, start,stop=None,step=1):
-        return _range(cls,start,stop,step) 
+    def range(cls, start, stop=None, step=1):
+        return _range(cls, start, stop, step)
+
+    def capitalize1(self, *args, **kwargs):
+        return self.__class__(super().capitalize(*args, **kwargs))
+
+    def casefold(self, *args, **kwargs):
+        return self.__class__(super().casefold(*args, **kwargs))
+
+    def center(self, *args, **kwargs):
+        return self.__class__(super().center(*args, **kwargs))
+
+    def expandtabs(self, *args, **kwargs):
+        return self.__class__(super().expandtabs(*args, **kwargs))
+
+    def join(self, *args, **kwargs):
+        return self.__class__(super().join(*args, **kwargs))
+
+    def ljust(self, *args, **kwargs):
+        return self.__class__(super().ljust(*args, **kwargs))
+
+    def lower(self, *args, **kwargs):
+        return self.__class__(super().lower(*args, **kwargs))
+
+    def lstrip(self, *args, **kwargs):
+        return self.__class__(super().lstrip(*args, **kwargs))
+
+    def partition(self, *args, **kwargs):
+        return self.__class__(super().partition(*args, **kwargs))
+
+    def removeprefix(self, *args, **kwargs):
+        return self.__class__(super().removeprefix(*args, **kwargs))
 
+    def removesuffix(self, *args, **kwargs):
+        return self.__class__(super().removesuffix(*args, **kwargs))
+
+    def replace(self, *args, **kwargs):
+        return self.__class__(super().replace(*args, **kwargs))
+
+    def rjust(self, *args, **kwargs):
+        return self.__class__(super().rjust(*args, **kwargs))
+
+    def rpartition(self, *args, **kwargs):
+        return self.__class__(super().rpartition(*args, **kwargs))
+
+    def rsplit(self, *args, **kwargs):
+        return self.__class__(super().rsplit(*args, **kwargs))
+
+    def rstrip(self, *args, **kwargs):
+        return self.__class__(super().rstrip(*args, **kwargs))
+
+    def split(self, *args, **kwargs):
+        return self.__class__(super().split(*args, **kwargs))
+
+    def strip(self, *args, **kwargs):
+        return self.__class__(super().strip(*args, **kwargs))
+
+    def swapcase(self, *args, **kwargs):
+        return self.__class__(super().swapcase(*args, **kwargs))
+
+    def title(self, *args, **kwargs):
+        return self.__class__(super().title(*args, **kwargs))
+
+    def translate(self, *args, **kwargs):
+        return self.__class__(super().translate(*args, **kwargs))
+
+    def upper(self, *args, **kwargs):
+        return self.__class__(super().upper(*args, **kwargs))
+
+    def zfill(self, *args, **kwargs):
+        return self.__class__(super().zfill(*args, **kwargs))
+
+    f = "capitalize"
+    exec(
+        f"""
+def {f}(self, *args, **kwargs):
+        return self.__class__(super(istr,self).{f}(*args, **kwargs)) 
+""",
+        globals(),
+        locals(),
+    )
 
 
 def main():
-    with istr.base(16):
-        a = istr(15)
-    b = a * a
-    print(b)
-    c=istr(a)
-    print(repr(c))
+    a = istr("123123")
+    print(repr(a.capitalize()))
 
 
 if __name__ == "__main__":
-    main()
+    main()
+
```

### Comparing `istr_python-0.1.1/istr_python.egg-info/PKG-INFO` & `istr_python-0.1.2/istr_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-0.1.1/pyproject.toml` & `istr_python-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only"
 ]
 [project.urls]
 Homepage = "https://github.com/salabim/istr"
 Repository = "https://github.com/salabim/istr"
+
+[tool.setuptools]
+packages = ["istr"]
```

### Comparing `istr_python-0.1.1/tests/test_istr.py` & `istr_python-0.1.2/tests/test_istr.py`

 * *Files 4% similar despite different names*

```diff
@@ -404,14 +404,41 @@
     assert repr(hundred) == "istr('100')"
 
     assert istr.repr_mode() == "istr"
 
     with pytest.raises(TypeError):
         istr.repr_mode("no")
 
+def test_str_methods():
+    a=istr("   123123 ")
+    b=istr("123123")
+    assert a.capitalize().equals(a)
+    assert a.casefold().equals(a)
+    assert a.center(20).equals(istr('        123123      '))
+    assert a.expandtabs(4).equals(a)
+    assert istr("").join(("0","1","2")).equals(istr("012"))
+    assert a.ljust(20).equals(istr('   123123           '))
+    assert a.lower().equals(a)
+    assert a.lstrip().equals(istr('123123 '))
+    assert a.partition("3")==(istr('   12'), istr('3'), istr('123 '))
+    assert a.removeprefix("   12").equals(istr("3123 "))
+    assert a.removesuffix("23 ").equals(istr("   1231"))
+    assert a.replace("1","9").equals(istr("   923923 "))
+    assert a.rjust(20).equals(istr('             123123 '))
+    assert b.partition("2")==(istr('1'), istr('2'), istr('3123'))
+    assert b.rpartition("2")==(istr('1231'), istr('2'), istr('3'))
+    assert b.rsplit("1")==[istr(''), istr('23'), istr('23')]
+    assert a.rstrip().equals(istr('   123123'))
+    assert b.split("1")==[istr(''), istr('23'), istr('23')]
+    assert a.strip().equals(istr('123123'))
+    assert a.swapcase().equals(a)
+    assert a.title().equals(a)
+    assert a.translate({49:  52}).equals(istr('   423423 '))
+    assert a.upper().equals(a)
+    assert b.zfill(10).equals(istr('0000123123'))
 
 def test_base():
     assert istr.base() == 10
     with istr.base(16):
         a = istr("7fff")
         assert a == 32767
         assert a == "7fff"
```

