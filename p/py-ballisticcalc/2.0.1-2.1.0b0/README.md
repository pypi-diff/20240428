# Comparing `tmp/py_ballisticcalc-2.0.1.tar.gz` & `tmp/py_ballisticcalc-2.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-2.0.1.tar", last modified: Thu Apr 11 16:14:29 2024, max compression
+gzip compressed data, was "py_ballisticcalc-2.1.0b0.tar", last modified: Sun Apr 28 15:14:46 2024, max compression
```

## Comparing `py_ballisticcalc-2.0.1.tar` & `py_ballisticcalc-2.1.0b0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:14:29.094526 py_ballisticcalc-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22789 2024-04-11 16:14:29.094526 py_ballisticcalc-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:14:29.090526 py_ballisticcalc-2.0.1/py_ballisticcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/drag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/drag_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/munition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/trajectory_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/py_ballisticcalc/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:14:29.094526 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22789 2024-04-11 16:14:29.000000 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 16:14:29.000000 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:14:29.000000 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 16:14:29.000000 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 16:14:29.000000 py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:14:29.094526 py_ballisticcalc-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:14:29.094526 py_ballisticcalc-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_danger_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_mbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-11 16:14:14.000000 py_ballisticcalc-2.0.1/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:14:46.071256 py_ballisticcalc-2.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-28 15:14:46.071256 py_ballisticcalc-2.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:14:46.071256 py_ballisticcalc-2.1.0b0/py_ballisticcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/drag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22248 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/drag_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/munition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/profile_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/trajectory_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27292 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:14:46.071256 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 15:14:46.000000 py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:14:46.075256 py_ballisticcalc-2.1.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:14:46.071256 py_ballisticcalc-2.1.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_danger_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_mbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-28 15:14:31.000000 py_ballisticcalc-2.1.0b0/tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.1/LICENSE` & `py_ballisticcalc-2.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/PKG-INFO` & `py_ballisticcalc-2.1.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.1
+Version: 2.1.0b0
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.1; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.1.0b0; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.1/README.md` & `py_ballisticcalc-2.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/__init__.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,16 @@
                     if use_powder_sensitivity := calculator.get('use_powder_sensitivity'):
                         set_global_use_powder_sensitivity(use_powder_sensitivity)
                 else:
                     logger.warning("Config has not `pybc.calculator` section")
             else:
                 logger.warning("Config has not `pybc` section")
 
+    logger.debug("Calculator globals and PreferredUnits load success")
+
 
 def _basic_config(filename=None,
                   max_calc_step_size: [float, Distance] = None,
                   use_powder_sensitivity: bool = False,
                   preferred_units: dict[str, Unit] = None):
 
     """
@@ -131,24 +133,31 @@
     'HitResult',
     'TrajFlag',
     'Atmo',
     'Wind',
     'Shot',
     'Weapon',
     'Ammo',
+    'Sight',
     'Unit',
+    'UnitType',
+    'UnitAliases',
+    'UnitAliasError',
+    'UnitTypeError',
+    'UnitConversionError',
     'AbstractUnit',
     'AbstractUnitType',
     'UnitProps',
     'UnitPropsDict',
     'Distance',
     'Velocity',
     'Angular',
     'Temperature',
     'Pressure',
     'Energy',
     'Weight',
     'Dimension',
-    'PreferredUnits'
+    'PreferredUnits',
+    'get_drag_tables_names'
 ]
 
 __all__ += ["TableG%s" % n for n in (1, 7, 2, 5, 6, 8, 'I', 'S')]
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/backend.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     from py_ballisticcalc_exts import (TrajectoryCalc,
                                        get_global_max_calc_step_size,
                                        get_global_use_powder_sensitivity,
                                        set_global_max_calc_step_size,
                                        set_global_use_powder_sensitivity,
                                        reset_globals)
 
-    logger.info("Binary modules found, running in binary mode")
+    logger.debug("Binary modules found, running in binary mode")
 except ImportError as error:
     from .trajectory_calc import (TrajectoryCalc,
                                   get_global_max_calc_step_size,
                                   get_global_use_powder_sensitivity,
                                   set_global_max_calc_step_size,
                                   set_global_use_powder_sensitivity,
                                   reset_globals)
 
-    logger.warning("Library running in pure python mode. "
-                   "For better performance install 'py_ballisticcalc.exts' package")
+    logger.info("Library running in pure python mode. "
+                "For better performance install 'py_ballisticcalc.exts' package")
 
 __all__ = (
     'TrajectoryCalc',
     'get_global_max_calc_step_size',
     'get_global_use_powder_sensitivity',
     'set_global_max_calc_step_size',
     'set_global_use_powder_sensitivity',
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/conditions.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/conditions.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/drag_model.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/drag_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     V: Velocity = Dimension(prefer_units='velocity', compare=False)
 
     def __post_init__(self):
         # If Mach not defined then convert V using standard atmosphere
         if self.Mach < 0:
             self.Mach = (self.V >> Velocity.MPS) / cSpeedOfSoundMetric
         if self.BC <= 0:
-            raise ValueError('bc must be positive')
+            raise ValueError('Ballistic coefficient must be positive')
 
 
 DragTableDataType = [list[dict[str, float]], list[DragDataPoint]]
 
 
 class DragModel:
     """
@@ -51,21 +51,20 @@
     """
 
     def __init__(self, bc: float,
                  drag_table: DragTableDataType,
                  weight: [float, Weight] = 0,
                  diameter: [float, Distance] = 0,
                  length: [float, Distance] = 0):
-        error = ''
+
         if len(drag_table) <= 0:
-            error = 'Received empty drag table'
+            # TODO: maybe have to require minimum size, cause few values don't give a valid result
+            raise ValueError('Received empty drag table')
         elif bc <= 0:
-            error = 'Ballistic coefficient must be positive'
-        if error:
-            raise ValueError(error)
+            raise ValueError('Ballistic coefficient must be positive')
 
         self.drag_table = make_data_points(drag_table)
 
         self.BC = bc
         self.length = PreferredUnits.length(length)
         self.weight = PreferredUnits.weight(weight)
         self.diameter = PreferredUnits.diameter(diameter)
@@ -140,16 +139,15 @@
                          yp: Union[list[float], tuple[float]]) -> Union[list[float], tuple[float]]:
     """Piecewise linear interpolation
     :param x: List of points for which we want interpolated values
     :param xp: List of existing points (x coordinate), *sorted in ascending order*
     :param yp: List of values for existing points (y coordinate)
     :return: List of interpolated values y for inputs x
     """
-    if len(xp) != len(yp):
-        raise ValueError("xp and yp lists must have same length")
+    assert len(xp) == len(yp), "xp and yp lists must have same length"
 
     y = []
 
     for xi in x:
         if xi <= xp[0]:
             y.append(yp[0])
         elif xi >= xp[-1]:
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/drag_tables.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/drag_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,8 +665,13 @@
     {'Mach': 3.85, 'CD': 0.9325},
     {'Mach': 3.90, 'CD': 0.9310},
     {'Mach': 3.95, 'CD': 0.9295},
     {'Mach': 4.00, 'CD': 0.9280},
 ]
 
 
-__all__ = ["TableG%s" % n for n in (1, 7, 2, 5, 6, 8, 'I', 'S')]
+def get_drag_tables_names():
+    return ["TableG%s" % n for n in (1, 7, 2, 5, 6, 8, 'I', 'S')]
+
+
+__all__ = ['get_drag_tables_names']
+__all__ += get_drag_tables_names()
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/example.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/example.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/interface.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/interface.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/trajectory_calc.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/trajectory_calc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/trajectory_data.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc/unit.py` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc/unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,40 +4,55 @@
 
 import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, MISSING, Field
 from enum import IntEnum
 from math import pi, atan, tan
 from typing import NamedTuple, Union, TypeVar
+import re
 
 from py_ballisticcalc.logger import logger
 
-
-__all__ = ('Unit', 'AbstractUnit', 'AbstractUnitType', 'UnitProps',
+__all__ = ('Unit', 'UnitType',
+           'AbstractUnit', 'AbstractUnitType',
+           'UnitProps', 'UnitAliases',
            'UnitPropsDict', 'Distance',
            'Velocity', 'Angular', 'Temperature', 'Pressure',
-           'Energy', 'Weight', 'Dimension', 'PreferredUnits')
-
+           'Energy', 'Weight', 'Dimension', 'PreferredUnits',
+           'UnitAliasError', 'UnitTypeError', 'UnitConversionError')
 
+UnitType = TypeVar('UnitType', bound='Unit')
 AbstractUnitType = TypeVar('AbstractUnitType', bound='AbstractUnit')
 
 
+class UnitTypeError(TypeError):
+    pass
+
+
+class UnitConversionError(UnitTypeError):
+    pass
+
+
+class UnitAliasError(ValueError):
+    pass
+
+
 # pylint: disable=invalid-name
 class Unit(IntEnum):
     """
     Usage of IntEnum simplify data serializing for using it with databases etc.
     """
     Radian = 0
     Degree = 1
     MOA = 2
     Mil = 3
     MRad = 4
     Thousandth = 5
     InchesPer100Yd = 6
-    CmPer100M = 7
+    CmPer100m = 7
     OClock = 8
 
     Inch = 10
     Foot = 11
     Yard = 12
     Mile = 13
     NauticalMile = 14
@@ -94,15 +109,15 @@
         :return: short symbol of the unit of measure in CI
         """
         return UnitPropsDict[self].symbol
 
     def __repr__(self) -> str:
         return UnitPropsDict[self].name
 
-    def __call__(self: 'Unit', value: [int, float, AbstractUnitType] = None) -> AbstractUnitType:
+    def __call__(self: UnitType, value: [int, float, AbstractUnitType] = None) -> AbstractUnitType:
         """Creates new unit instance by dot syntax
         :param self: unit as Unit enum
         :param value: numeric value of the unit
         :return: AbstractUnit instance
         """
 
         # if value is None:
@@ -121,34 +136,87 @@
         elif 50 <= self < 60:
             obj = Temperature(value, self)
         elif 60 <= self < 70:
             obj = Velocity(value, self)
         elif 70 <= self < 80:
             obj = Weight(value, self)
         else:
-            raise TypeError(f"{self} Unit is not supported")
+            raise UnitTypeError(f"{self} Unit is not supported")
         return obj
 
+    @staticmethod
+    def find_unit_by_alias(string_to_find, aliases):
+        # Iterate over the keys of the dictionary
+        for aliases_tuple in aliases.keys():
+            # Check if the string is present in any of the tuples
+            # if any(string_to_find in alias for alias in aliases_tuple):
+            if string_to_find in (each.lower() for each in aliases_tuple):
+                return aliases[aliases_tuple]
+        return None  # If not found, return None or handle it as needed
+
+    @staticmethod
+    def parse_unit(input_: str) -> UnitType:
+        input_ = input_.strip().lower()
+        if not isinstance(input_, str):
+            raise TypeError(f"type str expected for 'input_', got {type(input_)}")
+        if hasattr(PreferredUnits, input_):
+            return getattr(PreferredUnits, input_)
+        try:
+            return Unit[input_]
+        except KeyError:
+            return Unit.find_unit_by_alias(input_, UnitAliases)
+
+    @staticmethod
+    def parse_value(input_: [str, float, int], preferred: [UnitType, str]) -> AbstractUnitType:
+
+        def create_as_preferred(value):
+            if isinstance(preferred, Unit):
+                return preferred(float(value))
+            if isinstance(preferred, str):
+                if units := Unit.parse_unit(preferred):
+                    return units(float(value))
+            raise UnitAliasError(f"Unsupported {preferred=} unit alias")
+
+        if isinstance(input_, (float, int)):
+            return create_as_preferred(input_)
+
+        if not isinstance(input_, str):
+            raise TypeError(f"type, [str, float, int] expected for 'input_', got {type(input_)}")
+
+        input_string = input_.replace(" ", "")
+        if match := re.match(r'^-?(?:\d+\.\d*|\.\d+|\d+\.?)$', input_string):
+            value = match.group()
+            return create_as_preferred(value)
+
+        if match := re.match(r'(^-?(?:\d+\.\d*|\.\d+|\d+\.?))(.*$)', input_string):
+            value, alias = match.groups()
+            if units := Unit.parse_unit(alias):
+                return units(float(value))
+            else:
+                raise UnitAliasError(f"Unsupported unit {alias=}")
+
+        raise UnitAliasError(f"Can't parse unit {input_=}")
+
 
 class UnitProps(NamedTuple):
     """Properties of unit measure"""
     name: str
     accuracy: int
     symbol: str
 
 
 UnitPropsDict = {
     Unit.Radian: UnitProps('radian', 6, 'rad'),
     Unit.Degree: UnitProps('degree', 4, '°'),
     Unit.MOA: UnitProps('MOA', 2, 'MOA'),
-    Unit.Mil: UnitProps('mil', 2, 'mil'),
+    Unit.Mil: UnitProps('mil', 3, 'mil'),
     Unit.MRad: UnitProps('mrad', 2, 'mrad'),
     Unit.Thousandth: UnitProps('thousandth', 2, 'ths'),
     Unit.InchesPer100Yd: UnitProps('inch/100yd', 2, 'in/100yd'),
-    Unit.CmPer100M: UnitProps('cm/100m', 2, 'cm/100m'),
+    Unit.CmPer100m: UnitProps('cm/100m', 2, 'cm/100m'),
     Unit.OClock: UnitProps('hour', 2, 'h'),
 
     Unit.Inch: UnitProps("inch", 1, "inch"),
     Unit.Foot: UnitProps("foot", 2, "ft"),
     Unit.Yard: UnitProps("yard", 1, "yd"),
     Unit.Mile: UnitProps("mile", 3, "mi"),
     Unit.NauticalMile: UnitProps("nautical mile", 3, "nm"),
@@ -182,14 +250,65 @@
     Unit.Ounce: UnitProps('ounce', 1, 'oz'),
     Unit.Gram: UnitProps('gram', 1, 'g'),
     Unit.Pound: UnitProps('pound', 0, 'lb'),
     Unit.Kilogram: UnitProps('kilogram', 3, 'kg'),
     Unit.Newton: UnitProps('newton', 3, 'N'),
 }
 
+UnitAliases = {
+    ('radian', 'rad'): Unit.Radian,
+    ('degree', 'deg'): Unit.Degree,
+    ('moa',): Unit.MOA,
+    ('mil',): Unit.Mil,
+    ('mrad',): Unit.MRad,
+    ('thousandth', 'ths'): Unit.Thousandth,
+    ('inch/100yd', 'in/100yd', 'inch/100yd', 'in/100yard, inper100yd'): Unit.InchesPer100Yd,
+    ('centimeter/100m', 'cm/100m', 'cm/100meter', 'centimeter/100meter', 'cmper100m'): Unit.CmPer100m,
+    ('hour', 'h'): Unit.OClock,
+
+    ('inch', 'in'): Unit.Inch,
+    ('foot', 'ft'): Unit.Foot,
+    ('yard', 'yd'): Unit.Yard,
+    ('mile', 'mi', 'mi.'): Unit.Mile,
+    ('nauticalmile', 'nm', 'nmi'): Unit.NauticalMile,
+    ('millimeter', 'mm'): Unit.Millimeter,
+    ('centimeter', 'cm'): Unit.Centimeter,
+    ('meter', 'm'): Unit.Meter,
+    ('kilometer', 'km'): Unit.Kilometer,
+    ('line', 'ln', 'liniа'): Unit.Line,
+
+    ('footpound', 'foot-pound', 'ft⋅lbf', 'ft⋅lbf', 'ft⋅lb',
+     'foot*pound', 'ft*lbf', 'ft*lbf', 'ft*lb'): Unit.FootPound,
+    ('joule', 'J'): Unit.Joule,
+
+    ('mmHg',): Unit.MmHg,
+    ('inHg', '″Hg'): Unit.InHg,
+    ('bar',): Unit.Bar,
+    ('hectopascal', 'hPa'): Unit.hPa,
+    ('psi', 'lbf/in2'): Unit.PSI,
+
+    ('fahrenheit', '°F', 'F', 'degF'): Unit.Fahrenheit,
+    ('celsius', '°C', 'C', 'degC'): Unit.Celsius,
+    ('kelvin', '°K', 'K', 'degK'): Unit.Kelvin,
+    ('rankin', '°R', 'R', 'degR'): Unit.Rankin,
+
+    ('meter/second', 'm/s', 'meter/s', 'm/second', 'mps'): Unit.MPS,
+    ('kilometer/hour', 'km/h', 'kilometer/h', 'km/hour', 'kmh'): Unit.KMH,
+    ('foot/second', 'ft/s', 'foot/s', 'ft/second', 'fps'): Unit.FPS,
+    ('mile/hour', 'mi/h', 'mile/h', 'mi/hour', 'mph'): Unit.MPH,
+    ('knot', 'kn', 'kt'): Unit.KT,
+
+    ('grain', 'gr', 'grn'): Unit.Grain,
+    ('ounce', 'oz'): Unit.Ounce,
+    ('gram', 'g'): Unit.Gram,
+    ('pound', 'lb'): Unit.Pound,
+    ('kilogram', 'kilogramme', 'kg'): Unit.Kilogram,
+    ('newton', 'N'): Unit.Kilogram,
+}
+
 
 class AbstractUnit:
     """Abstract class for unit of measure instance definition
     Stores defined unit and value, applies conversions to other prefer_units
     """
     __slots__ = ('_value', '_defined_units')
 
@@ -239,45 +358,45 @@
 
     def __rshift__(self, other: Unit):
         return self.get_in(other)
 
     def __rlshift__(self, other: Unit):
         return self.convert(other)
 
-    def _unit_support_error(self, value: float, units: Unit):
+    def _validate_unit_type(self, value: float, units: Unit):
         """Validates the prefer_units
         :param value: value of the instance
         :param units: Unit enum type
         :return: value in specified prefer_units
         """
         if not isinstance(units, Unit):
             err_msg = f"Type expected: {Unit}, {type(Unit).__name__} " \
                       f"found: {type(units).__name__} ({value})"
             raise TypeError(err_msg)
         if units not in self.__dict__.values():
-            raise ValueError(f'{self.__class__.__name__}: unit {units} is not supported')
+            raise UnitConversionError(f'{self.__class__.__name__}: unit {units} is not supported')
         return 0
 
     def to_raw(self, value: float, units: Unit) -> float:
         """Converts value with specified prefer_units to raw value
         :param value: value of the instance
         :param units: Unit enum type
         :return: value in specified prefer_units
         """
-        return self._unit_support_error(value, units)
+        return self._validate_unit_type(value, units)
 
     def from_raw(self, value: float, units: Unit) -> float:
         """Converts raw value to specified prefer_units
         :param value: raw value of the unit
         :param units: Unit enum type
         :return: value in specified prefer_units
         """
-        return self._unit_support_error(value, units)
+        return self._validate_unit_type(value, units)
 
-    def convert(self, units: Unit) -> 'AbstractUnit':
+    def convert(self, units: Unit) -> AbstractUnitType:
         """Returns new unit instance in specified prefer_units
         :param units: Unit enum type
         :return: new unit instance in specified prefer_units
         """
         value = self.get_in(units)
         return self.__class__(value, units)
 
@@ -507,15 +626,15 @@
             result = value / 3200 * pi
         elif units == Angular.MRad:
             result = value / 1000
         elif units == Angular.Thousandth:
             result = value / 3000 * pi
         elif units == Angular.InchesPer100Yd:
             result = atan(value / 3600)
-        elif units == Angular.CmPer100M:
+        elif units == Angular.CmPer100m:
             result = atan(value / 10000)
         elif units == Angular.OClock:
             result = value / 6 * pi
         else:
             return super().to_raw(value, units)
         if result > 2 * pi:
             result = result % (2 * pi)
@@ -532,30 +651,30 @@
             result = value * 3200 / pi
         elif units == Angular.MRad:
             result = value * 1000
         elif units == Angular.Thousandth:
             result = value * 3000 / pi
         elif units == Angular.InchesPer100Yd:
             result = tan(value) * 3600
-        elif units == Angular.CmPer100M:
+        elif units == Angular.CmPer100m:
             result = tan(value) * 10000
         elif units == Angular.OClock:
             result = value * 6 / pi
         else:
             return super().from_raw(value, units)
         return result
 
     Radian = Unit.Radian
     Degree = Unit.Degree
     MOA = Unit.MOA
     Mil = Unit.Mil
     MRad = Unit.MRad
     Thousandth = Unit.Thousandth
     InchesPer100Yd = Unit.InchesPer100Yd
-    CmPer100M = Unit.CmPer100M
+    CmPer100m = Unit.CmPer100m
     OClock = Unit.OClock
 
 
 class Velocity(AbstractUnit):
     """Velocity unit"""
 
     def to_raw(self, value: float, units: Unit):
@@ -658,17 +777,20 @@
             if (_field := _fields.get(key)) and value is not None and not isinstance(value, AbstractUnit):
 
                 if units := _field.metadata.get('prefer_units'):
 
                     if isinstance(units, Unit):
                         value = units(value)
                     elif isinstance(units, str):
-                        value = PreferredUnits.__dict__[units](value)
+                        if _units := Unit.parse_unit(units):
+                            value = _units(value)
+                        else:
+                            raise UnitTypeError(f"Unsupported unit or dimension, use one of {PreferredUnits}")
                     else:
-                        raise TypeError(f"Unsupported unit or dimension use one of {PreferredUnits}")
+                        raise UnitTypeError(f"Unsupported unit or dimension, use one of {PreferredUnits}")
 
             super().__setattr__(key, value)
 
     @classmethod
     def defaults(self):
         """resets preferred units to defaults"""
         self.angular = Unit.Degree
@@ -692,34 +814,34 @@
         """set preferred units from Mapping"""
         for attribute, value in kwargs.items():
 
             if hasattr(PreferredUnits, attribute):
                 if isinstance(value, Unit):
                     setattr(PreferredUnits, attribute, value)
                 elif isinstance(value, str):
-                    try:
-                        setattr(PreferredUnits, attribute, Unit[value])
-                    except KeyError:
+                    if _unit := Unit.parse_unit(value):
+                        setattr(PreferredUnits, attribute, _unit)
+                    else:
                         logger.warning(f"{value=} not a member of Unit")
                 else:
                     logger.warning(f"type of {value=} have not been converted to a member of Unit")
             else:
                 logger.warning(f"{attribute=} not found in preferred_units")
 
 
-
 # pylint: disable=redefined-builtin,too-few-public-methods,too-many-arguments
 class Dimension(Field):
     """
     Definition of measure units specified field for
     PreferredUnits.Mixin based dataclasses
     """
 
     def __init__(self, prefer_units: Union[str, Unit], init=True, repr_=True,
                  hash_=None, compare=True, metadata=None):
+
         if metadata is None:
             metadata = {}
         metadata['prefer_units'] = prefer_units
 
         major, minor = sys.version_info.major, sys.version_info.minor
 
         if major >= 3 and minor > 9:
@@ -730,14 +852,18 @@
             raise RuntimeError("Unsupported python version")
 
         super().__init__(default=None, default_factory=MISSING,
                          init=init, repr=repr_,
                          hash=hash_, compare=compare,
                          metadata=metadata, **extra)
 
+    @property
+    def raw_value(self):
+        raise NotImplementedError
+
     @abstractmethod
     def __rshift__(self, other):
         ...
 
     @abstractmethod
     def __lshift__(self, other):
         ...
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.1
+Version: 2.1.0b0
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.1; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.1.0b0; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.1/py_ballisticcalc.egg-info/SOURCES.txt` & `py_ballisticcalc-2.1.0b0/py_ballisticcalc.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 py_ballisticcalc/__init__.py
+py_ballisticcalc/__main__.py
 py_ballisticcalc/backend.py
 py_ballisticcalc/conditions.py
 py_ballisticcalc/drag_model.py
 py_ballisticcalc/drag_tables.py
 py_ballisticcalc/example.py
 py_ballisticcalc/interface.py
 py_ballisticcalc/logger.py
 py_ballisticcalc/munition.py
+py_ballisticcalc/profile_loader.py
 py_ballisticcalc/trajectory_calc.py
 py_ballisticcalc/trajectory_data.py
 py_ballisticcalc/unit.py
 py_ballisticcalc.egg-info/PKG-INFO
 py_ballisticcalc.egg-info/SOURCES.txt
 py_ballisticcalc.egg-info/dependency_links.txt
+py_ballisticcalc.egg-info/entry_points.txt
 py_ballisticcalc.egg-info/requires.txt
 py_ballisticcalc.egg-info/top_level.txt
 tests/test_.py
 tests/test_atmosphere.py
 tests/test_computer.py
 tests/test_config_loader.py
 tests/test_danger_space.py
 tests/test_mbc.py
+tests/test_sight.py
 tests/test_trajectory.py
 tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.1/pyproject.toml` & `py_ballisticcalc-2.1.0b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc"
-version = "2.0.1"
+version = "2.1.0b0"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
@@ -50,10 +50,13 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["py_ballisticcalc*"]  # alternatively: `exclude = ["additional*"]`
 exclude = ["py_ballisticcalc_exts*"]
 
 
 [project.optional-dependencies]
-exts = ['py_ballisticcalc.exts==2.0.1']
+exts = ['py_ballisticcalc.exts==2.1.0b0']
 lint = ['pylint', 'flake8']
 charts = ['matplotlib', 'pandas']
+
+[project.scripts]
+pybc = "py_ballisticcalc.__main__:main"
```

### Comparing `py_ballisticcalc-2.0.1/tests/test_atmosphere.py` & `py_ballisticcalc-2.1.0b0/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_computer.py` & `py_ballisticcalc-2.1.0b0/tests/test_computer.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_config_loader.py` & `py_ballisticcalc-2.1.0b0/tests/test_config_loader.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_danger_space.py` & `py_ballisticcalc-2.1.0b0/tests/test_danger_space.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_mbc.py` & `py_ballisticcalc-2.1.0b0/tests/test_mbc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_trajectory.py` & `py_ballisticcalc-2.1.0b0/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.1/tests/test_units.py` & `py_ballisticcalc-2.1.0b0/tests/test_units.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,49 @@
         PreferredUnits.sight_height = Unit.Centimeter
 
         tc3 = TestClass(1, 1)
         self.assertEqual(tc3.as_metadata_str.units, Unit.Centimeter)
         self.assertEqual(tc3.as_metadata_unit.units, Unit.Meter)
 
 
+class TestUnitsParser(unittest.TestCase):
+    def test_parse_values(self):
+
+        valid_cases = [
+            '10', '10.2', '.2', '0.', '10ft*lb', '10footpound'
+        ]
+
+        for case in valid_cases:
+
+            with self.subTest(case):
+                ret = Unit.parse_value(case, Unit.FootPound)
+                self.assertIsInstance(ret, Energy)
+                self.assertEqual(ret.units, Unit.FootPound)
+
+            with self.subTest(case):
+                ret = Unit.parse_value(case, 'footpound')
+                self.assertIsInstance(ret, Energy)
+                self.assertEqual(ret.units, Unit.FootPound)
+
+            with self.subTest(case):
+                ret = Unit.parse_value(case, 'ft*lb')
+                self.assertIsInstance(ret, Energy)
+                self.assertEqual(ret.units, Unit.FootPound)
+
+            with self.subTest(case):
+                ret = Unit.parse_value(case, 'energy')
+                self.assertIsInstance(ret, Energy)
+                self.assertEqual(ret.units, Unit.FootPound)
+
+    def test_parse_units(self):
+
+        ret = Unit.parse_unit('ft*lb')
+        self.assertIsInstance(ret, Unit)
+
+
 class TestAngular(unittest.TestCase):
 
     def setUp(self) -> None:
         self.unit_class = Angular
         self.unit_list = [
             Angular.Degree,
             Angular.MOA,
```

