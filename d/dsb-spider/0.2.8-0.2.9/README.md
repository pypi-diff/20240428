# Comparing `tmp/dsb_spider-0.2.8.tar.gz` & `tmp/dsb_spider-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsb_spider-0.2.8.tar", last modified: Fri Dec  6 08:00:10 2019, max compression
+gzip compressed data, was "dist/dsb_spider-0.2.9.tar", last modified: Fri Dec  6 08:19:06 2019, max compression
```

## Comparing `dsb_spider-0.2.8.tar` & `dsb_spider-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/
--rw-r--r--   0 chen       (501) staff       (20)      296 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/dsb_spider/
--rw-r--r--   0 chen       (501) staff       (20)      355 2019-12-05 10:26:37.000000 dsb_spider-0.2.8/dsb_spider/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1633 2019-11-27 03:53:07.000000 dsb_spider-0.2.8/dsb_spider/checker.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/dsb_spider/log/
--rw-r--r--   0 chen       (501) staff       (20)     2438 2019-12-06 07:28:40.000000 dsb_spider-0.2.8/dsb_spider/log/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      664 2019-11-26 09:48:29.000000 dsb_spider-0.2.8/dsb_spider/log/color_codes.py
--rw-r--r--   0 chen       (501) staff       (20)      328 2019-12-06 07:40:42.000000 dsb_spider-0.2.8/dsb_spider/log/ex.py
--rw-r--r--   0 chen       (501) staff       (20)     1767 2019-11-26 09:48:29.000000 dsb_spider-0.2.8/dsb_spider/log/formatter.py
--rw-r--r--   0 chen       (501) staff       (20)     9411 2019-12-06 02:40:57.000000 dsb_spider-0.2.8/dsb_spider/req.py
--rw-r--r--   0 chen       (501) staff       (20)     1248 2019-12-05 11:51:41.000000 dsb_spider-0.2.8/dsb_spider/sched.py
--rw-r--r--   0 chen       (501) staff       (20)     5998 2019-12-06 07:56:02.000000 dsb_spider-0.2.8/dsb_spider/tasker.py
--rw-r--r--   0 chen       (501) staff       (20)     1419 2019-12-04 09:36:58.000000 dsb_spider-0.2.8/dsb_spider/timer.py
--rw-r--r--   0 chen       (501) staff       (20)     1375 2019-12-05 10:03:25.000000 dsb_spider-0.2.8/dsb_spider/utils.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/dsb_spider.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      296 2019-12-06 08:00:09.000000 dsb_spider-0.2.8/dsb_spider.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      427 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/dsb_spider.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2019-12-06 08:00:09.000000 dsb_spider-0.2.8/dsb_spider.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       56 2019-12-06 08:00:09.000000 dsb_spider-0.2.8/dsb_spider.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       11 2019-12-06 08:00:09.000000 dsb_spider-0.2.8/dsb_spider.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2019-12-06 08:00:10.000000 dsb_spider-0.2.8/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      479 2019-12-06 07:59:29.000000 dsb_spider-0.2.8/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/
+-rw-r--r--   0 chen       (501) staff       (20)      296 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/PKG-INFO
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider/
+-rw-r--r--   0 chen       (501) staff       (20)      355 2019-12-05 10:26:37.000000 dsb_spider-0.2.9/dsb_spider/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1633 2019-11-27 03:53:07.000000 dsb_spider-0.2.9/dsb_spider/checker.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider/log/
+-rw-r--r--   0 chen       (501) staff       (20)     2438 2019-12-06 07:28:40.000000 dsb_spider-0.2.9/dsb_spider/log/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      664 2019-11-26 09:48:29.000000 dsb_spider-0.2.9/dsb_spider/log/color_codes.py
+-rw-r--r--   0 chen       (501) staff       (20)      328 2019-12-06 07:40:42.000000 dsb_spider-0.2.9/dsb_spider/log/ex.py
+-rw-r--r--   0 chen       (501) staff       (20)     1767 2019-11-26 09:48:29.000000 dsb_spider-0.2.9/dsb_spider/log/formatter.py
+-rw-r--r--   0 chen       (501) staff       (20)     9411 2019-12-06 02:40:57.000000 dsb_spider-0.2.9/dsb_spider/req.py
+-rw-r--r--   0 chen       (501) staff       (20)     1248 2019-12-05 11:51:41.000000 dsb_spider-0.2.9/dsb_spider/sched.py
+-rw-r--r--   0 chen       (501) staff       (20)     6016 2019-12-06 08:18:49.000000 dsb_spider-0.2.9/dsb_spider/tasker.py
+-rw-r--r--   0 chen       (501) staff       (20)     1419 2019-12-04 09:36:58.000000 dsb_spider-0.2.9/dsb_spider/timer.py
+-rw-r--r--   0 chen       (501) staff       (20)     1375 2019-12-05 10:03:25.000000 dsb_spider-0.2.9/dsb_spider/utils.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      296 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      427 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       56 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       11 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/dsb_spider.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2019-12-06 08:19:06.000000 dsb_spider-0.2.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      479 2019-12-06 08:19:02.000000 dsb_spider-0.2.9/setup.py
```

### Comparing `dsb_spider-0.2.8/dsb_spider/checker.py` & `dsb_spider-0.2.9/dsb_spider/checker.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/log/__init__.py` & `dsb_spider-0.2.9/dsb_spider/log/__init__.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/log/color_codes.py` & `dsb_spider-0.2.9/dsb_spider/log/color_codes.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/log/formatter.py` & `dsb_spider-0.2.9/dsb_spider/log/formatter.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/req.py` & `dsb_spider-0.2.9/dsb_spider/req.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/sched.py` & `dsb_spider-0.2.9/dsb_spider/sched.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/tasker.py` & `dsb_spider-0.2.9/dsb_spider/tasker.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,30 +74,30 @@
     except KeyError:
         register = _TASK_FUNC_REGISTERS[name] = _FuncRegistry(name)
         return register
 
 exRegistry = getTaskFuncRegister('ex')
 
 @exRegistry
-def default(ex, *args, **kwargs):
+def default(self, ex, *args, **kwargs):
     logger.errorx(ex)
     pass
 
 def exhandler(ignore:bool=True, interrupt:bool=False):
     def deco_func(func):
         def deco_args(self, *args, **kwargs):
             try:
                 return func(self, *args, **kwargs)
             except TaskStateError as _ex:
                 logger.debug(_ex)
             except Exception as _ex:
                 if hasattr(_ex, 'handle_name'):
-                    exRegistry[_ex.handle_name](_ex, *args, *kwargs)
+                    exRegistry[_ex.handle_name](self, _ex, *args, *kwargs)
                 else:
-                    exRegistry['default'](_ex, *args, *kwargs)
+                    exRegistry['default'](self, _ex, *args, *kwargs)
                 if interrupt:
                     self.finish()
                 if not ignore:
                     raise
         return deco_args
     return deco_func
```

### Comparing `dsb_spider-0.2.8/dsb_spider/timer.py` & `dsb_spider-0.2.9/dsb_spider/timer.py`

 * *Files identical despite different names*

### Comparing `dsb_spider-0.2.8/dsb_spider/utils.py` & `dsb_spider-0.2.9/dsb_spider/utils.py`

 * *Files identical despite different names*

