# Comparing `tmp/quantiphy-2.8.0.tar.gz` & `tmp/quantiphy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quantiphy-2.8.0.tar", last modified: Wed Jan  8 19:02:30 2020, max compression
+gzip compressed data, was "dist/quantiphy-2.9.0.tar", last modified: Tue Jan 28 17:49:56 2020, max compression
```

## Comparing `quantiphy-2.8.0.tar` & `quantiphy-2.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-01-08 19:02:30.000000 quantiphy-2.8.0/
--rw-rw-r--   0 ken       (1000) ken       (1000)     8033 2020-01-08 19:02:30.000000 quantiphy-2.8.0/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1000)     5414 2020-01-08 18:58:40.000000 quantiphy-2.8.0/README.rst
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/
--rw-rw-r--   0 ken       (1000) ken       (1000)     8033 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1000)      224 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/SOURCES.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)        4 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)       10 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/top_level.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-01-08 19:02:30.000000 quantiphy-2.8.0/quantiphy.egg-info/zip-safe
--rw-rw-r--   0 ken       (1000) ken       (1000)   115304 2020-01-08 18:58:40.000000 quantiphy-2.8.0/quantiphy.py
--rw-rw-r--   0 ken       (1000) ken       (1000)       38 2020-01-08 19:02:30.000000 quantiphy-2.8.0/setup.cfg
--rw-rw-r--   0 ken       (1000) ken       (1000)     1829 2020-01-08 18:58:40.000000 quantiphy-2.8.0/setup.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-01-28 17:49:56.652261 quantiphy-2.9.0/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     8033 2020-01-28 17:49:56.651261 quantiphy-2.9.0/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)     5414 2020-01-28 17:40:44.000000 quantiphy-2.9.0/README.rst
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2020-01-28 17:49:56.649261 quantiphy-2.9.0/quantiphy.egg-info/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     8033 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)      224 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)        4 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/requires.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       10 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/top_level.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)        1 2020-01-28 17:49:56.000000 quantiphy-2.9.0/quantiphy.egg-info/zip-safe
+-rw-rw-r--   0 ken       (1000) ken       (1000)   116003 2020-01-28 17:40:44.000000 quantiphy-2.9.0/quantiphy.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)       38 2020-01-28 17:49:56.652261 quantiphy-2.9.0/setup.cfg
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1829 2020-01-28 17:40:44.000000 quantiphy-2.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `quantiphy-2.8.0/PKG-INFO` & `quantiphy-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: quantiphy
-Version: 2.8.0
+Version: 2.9.0
 Summary: physical quantities (numbers with units)
 Home-page: https://quantiphy.readthedocs.io
 Author: Ken Kundert
 Author-email: quantiphy@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/quantiphy/tarball/master
 Description: QuantiPhy — Physical Quantities
@@ -23,16 +23,16 @@
             :target: https://pypi.python.org/pypi/quantiphy/
         
         .. IGNORE: pypi statistics are broken and unlikely to be fixed
             .. image:: https://img.shields.io/pypi/dm/quantiphy.svg
                 :target: https://pypi.python.org/pypi/quantiphy/
         
         :Author: Ken Kundert
-        :Version: 2.8.0
-        :Released: 2020-01-08
+        :Version: 2.9.0
+        :Released: 2020-01-28
         
         
         What?
         -----
         
         *QuantiPhy* is a Python library that offers support for physical quantities.  
         A quantity is the pairing of a number and a unit of measure that indicates the
```

### Comparing `quantiphy-2.8.0/README.rst` & `quantiphy-2.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     :target: https://pypi.python.org/pypi/quantiphy/
 
 .. IGNORE: pypi statistics are broken and unlikely to be fixed
     .. image:: https://img.shields.io/pypi/dm/quantiphy.svg
         :target: https://pypi.python.org/pypi/quantiphy/
 
 :Author: Ken Kundert
-:Version: 2.8.0
-:Released: 2020-01-08
+:Version: 2.9.0
+:Released: 2020-01-28
 
 
 What?
 -----
 
 *QuantiPhy* is a Python library that offers support for physical quantities.  
 A quantity is the pairing of a number and a unit of measure that indicates the
```

### Comparing `quantiphy-2.8.0/quantiphy.egg-info/PKG-INFO` & `quantiphy-2.9.0/quantiphy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: quantiphy
-Version: 2.8.0
+Version: 2.9.0
 Summary: physical quantities (numbers with units)
 Home-page: https://quantiphy.readthedocs.io
 Author: Ken Kundert
 Author-email: quantiphy@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/quantiphy/tarball/master
 Description: QuantiPhy — Physical Quantities
@@ -23,16 +23,16 @@
             :target: https://pypi.python.org/pypi/quantiphy/
         
         .. IGNORE: pypi statistics are broken and unlikely to be fixed
             .. image:: https://img.shields.io/pypi/dm/quantiphy.svg
                 :target: https://pypi.python.org/pypi/quantiphy/
         
         :Author: Ken Kundert
-        :Version: 2.8.0
-        :Released: 2020-01-08
+        :Version: 2.9.0
+        :Released: 2020-01-28
         
         
         What?
         -----
         
         *QuantiPhy* is a Python library that offers support for physical quantities.  
         A quantity is the pairing of a number and a unit of measure that indicates the
```

### Comparing `quantiphy-2.8.0/quantiphy.py` & `quantiphy-2.9.0/quantiphy.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
 # Exceptions {{{1
 class QuantiPhyError(Exception):
     """QuantiPhy base exception.
 
     All of the specific QuantiPhy exceptions subclass this exception.
     """
+    _template = "{}"
 
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
 
     def render(self, template=None):
         """Convert exception to a string under guidance of format string.
@@ -211,14 +212,20 @@
 class UnknownUnitSystem(QuantiPhyError, KeyError):
     """
     The name given does not correspond to a known unit system.
     """
     _template = "{}: unknown unit system."
 
 
+class IncompatiblePreferences(QuantiPhyError, ValueError):
+    """
+    Two preferences are not compatible
+    """
+
+
 # Unit Conversions {{{1
 _unit_conversions = {}
 def _convert_units(to_units, from_units, value):
     if to_units == from_units:
         return value
     try:
         return _unit_conversions[(to_units, from_units)](value)
@@ -651,16 +658,16 @@
         for a in aliases:
             _constants[None][a] = value
         if value.name:
             _constants[None][value.name] = value
 
 
 # Globals {{{1
-__version__ = '2.8.0'
-__released__ = '2020-01-08'
+__version__ = '2.9.0'
+__released__ = '2020-01-28'
 
 # These mappings are only used when reading numbers
 # The key for these mappings must be a single character
 MAPPINGS = {
     'Y': 'e24',
     'Z': 'e21',
     'E': 'e18',
@@ -845,14 +852,18 @@
 
     :raises UnknownScaleFactor(QuantiPhyError, ValueError):
         Unknown scale factor.
 
     :raises InvalidNumber(QuantiPhyError, ValueError, TypeError):
         Not a valid number.
 
+    :raises IncompatiblePreferences(QuantiPhyError, ValueError):
+        *radix* and *comma* must differ.
+
+    You can use *Quantity* to create quantities from floats, strings, or other
     You can use *Quantity* to create quantities from floats, strings, or other
     quantities.  If a float is given, *model* or *units* would be used to
     specify the units.
 
     Examples::
 
         >>> from quantiphy import Quantity
@@ -1121,15 +1132,15 @@
             scale factors. The default is 'TGMkmunpfa', which gets rid or the
             very large ('YZEP') and very small ('zy') scale factors that many
             people do not recognize.
 
         :arg str radix:
             The character to be used as the radix.  By default it is '.'.
 
-        :arg str radix:
+        :arg str plus:
             The text to be used as the plus sign.  By default it is '+',
             but is sometimes '＋' (the unicode full width plus sign) or '' to
             simply eliminate plus signs from numbers.  You can access the
             Unicode full width plus sign using Quantity.plus_sign.
 
         :arg int prec:
             Default precision  in digits where 0 corresponds to 1 digit.  Must
@@ -1367,40 +1378,39 @@
     # _combine {{{2
     def _combine(self, mantissa, sf, units, spacer, sf_is_exp=False):
         if self.number_fmt:
             parts = mantissa.split('.')
             whole_part = parts[0]
             frac_part = ''.join(parts[1:])
             if frac_part:
-                frac_part = '.' + frac_part
+                frac_part = self.radix + frac_part
             if units in CURRENCY_SYMBOLS:
                 whole_part = self._map_leading_sign(whole_part, units)
                 units = ''
             if sf_is_exp:
                 frac_part += sf
                 sf = ''
             if callable(self.number_fmt):
                 return self.number_fmt(whole_part, frac_part, sf+units)
             return self.number_fmt.format(
                 whole=whole_part, frac=frac_part, units=sf+units
             )
 
-        mantissa = mantissa.lstrip('+')
+        mantissa = self._fix_punct(mantissa.lstrip('+'))
         if units:
             if units in CURRENCY_SYMBOLS:
                 # prefix the value with the units
                 return self._map_leading_sign(mantissa + sf, units)
             mantissa = self._map_leading_sign(mantissa)
             if sf_is_exp:
                 # has an exponent
                 return mantissa + sf + spacer + units
             # has a scale factor
             return mantissa + spacer + sf + units
         mantissa = self._map_leading_sign(mantissa)
-        mantissa = self._fix_punct(mantissa)
         return mantissa + sf
 
     # recognizers {{{2
     @classmethod
     def _initialize_recognizers(cls):
         # Build regular expressions used to recognize quantities
 
@@ -1606,33 +1616,41 @@
                         data['desc'] = components[2]
             else:
                 # data['name'] = getattr(model, 'name', '')
                 data['units'] = getattr(model, 'units', '')
                 # data['desc'] = getattr(model, 'desc', '')
 
         def recognize_number(value, ignore_sf):
+            comma = cls.get_pref('comma')
+            radix = cls.get_pref('radix')
+            if comma == radix:
+                raise IncompatiblePreferences('comma and radix must differ.')
             if binary and not ignore_sf:
                 number_converters = cls.binary_number_converters
                 for pattern, get_mant, get_sf, get_units in number_converters:
-                    match = pattern.match(value.replace(',', ''))
+                    match = pattern.match(
+                        value.replace(comma, '').replace(radix, '.')
+                    )
                     if match:
                         mantissa = get_mant(match)
                         sf = get_sf(match)
                         units = get_units(match)
                         if sf+units in cls.get_pref('known_units'):
                             sf, units = '', sf+units
                         mantissa = mantissa.replace('_', '')
                         number = float(mantissa) * BINARY_MAPPINGS.get(sf, 1)
                         return number, units, None, ''
             if ignore_sf:
                 number_converters = cls.sf_free_number_converters
             else:
                 number_converters = cls.all_number_converters
             for pattern, get_mant, get_sf, get_units in number_converters:
-                match = pattern.match(value.replace(',', ''))
+                match = pattern.match(
+                    value.replace(comma, '').replace(radix, '.')
+                )
                 if match:
                     mantissa = get_mant(match)
                     sf = get_sf(match)
                     units = get_units(match)
                     if sf+units in cls.get_pref('known_units'):
                         sf, units = '', sf+units
                     mantissa = mantissa.replace('_', '')
@@ -2733,20 +2751,22 @@
                         units = components[-1][1:-1]
                         value = ' '.join(components[:-1])
                     else:
                         units = ''
                     symbols = ChainMap(
                         quantities, predefined, _active_constants, CONSTANTS
                     )
-                    value = eval(value, None, symbols)
                     try:
+                        value = eval(value, None, symbols)
                         quantity = cls(value, units=units, name=qname, desc=desc)
                     except InvalidNumber:
                         # not suitable to be a quantity, so just save value
                         quantity = value
+                    except SyntaxError:
+                        continue
                 quantities[name] = quantity
         return quantities
 
     # map_sf_to_sci_notation() {{{2
     # The explicit references to unicode here are for backward compatibility
     # with python2. It can be removed when python2 support is dropped.
     _SCI_NOTATION_MAPPER = {
```

### Comparing `quantiphy-2.8.0/setup.py` & `quantiphy-2.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
-import sys
 from codecs import open
+import sys
 
 with open('README.rst', encoding="UTF-8") as f:
     readme = f.read()
 
 if sys.version_info < (3,3):
     dependencies='six chainmap'
 else:
@@ -15,15 +15,15 @@
 keywords='''
     quantities physical quantity units SI scale factors engineering notation
     mks cgs
 '''
 
 setup(
     name='quantiphy',
-    version='2.8.0',
+    version='2.9.0',
     description='physical quantities (numbers with units)',
     long_description=readme,
     author="Ken Kundert",
     author_email='quantiphy@nurdletech.com',
     url='https://quantiphy.readthedocs.io',
     download_url='https://github.com/kenkundert/quantiphy/tarball/master',
     license='GPLv3+',
```

