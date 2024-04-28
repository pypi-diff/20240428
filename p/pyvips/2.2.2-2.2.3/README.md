# Comparing `tmp/pyvips-2.2.2.tar.gz` & `tmp/pyvips-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvips-2.2.2.tar", last modified: Thu Jan  4 11:50:50 2024, max compression
+gzip compressed data, was "pyvips-2.2.3.tar", last modified: Sun Apr 28 11:19:44 2024, max compression
```

## Comparing `pyvips-2.2.2.tar` & `pyvips-2.2.3.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-04 11:50:50.910200 pyvips-2.2.2/
--rw-rw-r--   0 john      (1000) john      (1000)     1055 2022-06-12 09:56:30.000000 pyvips-2.2.2/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)       47 2022-06-12 09:56:30.000000 pyvips-2.2.2/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     7208 2024-01-04 11:50:50.910200 pyvips-2.2.2/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     5847 2023-09-30 17:02:57.000000 pyvips-2.2.2/README.rst
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-04 11:50:50.910200 pyvips-2.2.2/pyvips/
--rw-rw-r--   0 john      (1000) john      (1000)     5799 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3296 2022-10-18 15:58:45.000000 pyvips-2.2.2/pyvips/base.py
--rw-rw-r--   0 john      (1000) john      (1000)    26882 2023-10-09 09:40:18.000000 pyvips-2.2.2/pyvips/enums.py
--rw-rw-r--   0 john      (1000) john      (1000)     2006 2022-10-18 15:58:45.000000 pyvips-2.2.2/pyvips/error.py
--rw-rw-r--   0 john      (1000) john      (1000)     7018 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/gobject.py
--rw-rw-r--   0 john      (1000) john      (1000)    13220 2023-10-01 17:58:34.000000 pyvips-2.2.2/pyvips/gvalue.py
--rw-rw-r--   0 john      (1000) john      (1000)     1298 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/pyvips_build.py
--rw-rw-r--   0 john      (1000) john      (1000)     1130 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vconnection.py
--rw-rw-r--   0 john      (1000) john      (1000)    17052 2023-10-01 17:58:34.000000 pyvips-2.2.2/pyvips/vdecls.py
--rw-rw-r--   0 john      (1000) john      (1000)      111 2023-01-31 18:38:53.000000 pyvips-2.2.2/pyvips/version.py
--rw-rw-r--   0 john      (1000) john      (1000)    61705 2023-10-01 17:58:34.000000 pyvips-2.2.2/pyvips/vimage.py
--rw-rw-r--   0 john      (1000) john      (1000)     1100 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vinterpolate.py
--rw-rw-r--   0 john      (1000) john      (1000)     4093 2022-10-19 08:16:30.000000 pyvips-2.2.2/pyvips/vobject.py
--rw-rw-r--   0 john      (1000) john      (1000)    20282 2023-10-09 09:47:50.000000 pyvips-2.2.2/pyvips/voperation.py
--rw-rw-r--   0 john      (1000) john      (1000)     1779 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vregion.py
--rw-rw-r--   0 john      (1000) john      (1000)     3079 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vsource.py
--rw-rw-r--   0 john      (1000) john      (1000)     1887 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vsourcecustom.py
--rw-rw-r--   0 john      (1000) john      (1000)     2533 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vtarget.py
--rw-rw-r--   0 john      (1000) john      (1000)     3401 2022-06-12 09:56:30.000000 pyvips-2.2.2/pyvips/vtargetcustom.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-04 11:50:50.910200 pyvips-2.2.2/pyvips.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     7208 2024-01-04 11:50:50.000000 pyvips-2.2.2/pyvips.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      593 2024-01-04 11:50:50.000000 pyvips-2.2.2/pyvips.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-01-04 11:50:50.000000 pyvips-2.2.2/pyvips.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2022-10-03 11:46:13.000000 pyvips-2.2.2/pyvips.egg-info/not-zip-safe
--rw-rw-r--   0 john      (1000) john      (1000)       87 2024-01-04 11:50:50.000000 pyvips-2.2.2/pyvips.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       16 2024-01-04 11:50:50.000000 pyvips-2.2.2/pyvips.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      137 2024-01-04 11:50:50.910200 pyvips-2.2.2/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     3623 2023-09-30 17:02:57.000000 pyvips-2.2.2/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-28 11:19:44.582812 pyvips-2.2.3/
+-rw-rw-r--   0 john      (1000) john      (1000)     1055 2022-06-12 09:56:30.000000 pyvips-2.2.3/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       47 2022-06-12 09:56:30.000000 pyvips-2.2.3/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     7279 2024-04-28 11:19:44.582812 pyvips-2.2.3/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     5867 2024-01-05 20:02:19.000000 pyvips-2.2.3/README.rst
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-28 11:19:44.578812 pyvips-2.2.3/pyvips/
+-rw-rw-r--   0 john      (1000) john      (1000)     6375 2024-04-28 11:16:17.000000 pyvips-2.2.3/pyvips/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4029 2024-04-28 11:16:17.000000 pyvips-2.2.3/pyvips/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26480 2024-01-22 19:23:41.000000 pyvips-2.2.3/pyvips/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2006 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/error.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7018 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/gobject.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12350 2024-04-28 11:16:17.000000 pyvips-2.2.3/pyvips/gvalue.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1688 2024-04-28 11:16:17.000000 pyvips-2.2.3/pyvips/pyvips_build.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1130 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vconnection.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15589 2024-04-28 11:16:17.000000 pyvips-2.2.3/pyvips/vdecls.py
+-rw-rw-r--   0 john      (1000) john      (1000)      111 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/version.py
+-rw-rw-r--   0 john      (1000) john      (1000)    62010 2024-03-07 12:54:14.000000 pyvips-2.2.3/pyvips/vimage.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1100 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vinterpolate.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4093 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vobject.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20282 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/voperation.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1779 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vregion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3079 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vsource.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1887 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vsourcecustom.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2533 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vtarget.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3401 2024-01-05 20:02:19.000000 pyvips-2.2.3/pyvips/vtargetcustom.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-28 11:19:44.582812 pyvips-2.2.3/pyvips.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     7279 2024-04-28 11:19:44.000000 pyvips-2.2.3/pyvips.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      750 2024-04-28 11:19:44.000000 pyvips-2.2.3/pyvips.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-28 11:19:44.000000 pyvips-2.2.3/pyvips.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2022-10-03 11:46:13.000000 pyvips-2.2.3/pyvips.egg-info/not-zip-safe
+-rw-rw-r--   0 john      (1000) john      (1000)       87 2024-04-28 11:19:44.000000 pyvips-2.2.3/pyvips.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       16 2024-04-28 11:19:44.000000 pyvips-2.2.3/pyvips.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      137 2024-04-28 11:19:44.582812 pyvips-2.2.3/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     3669 2024-04-28 11:16:17.000000 pyvips-2.2.3/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-28 11:19:44.582812 pyvips-2.2.3/tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1396 2022-10-18 15:58:45.000000 pyvips-2.2.3/tests/test_block.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6052 2022-06-12 09:56:30.000000 pyvips-2.2.3/tests/test_connections.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3864 2022-06-12 09:56:30.000000 pyvips-2.2.3/tests/test_constants.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3584 2023-10-04 10:46:35.000000 pyvips-2.2.3/tests/test_gvalue.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10475 2022-06-12 09:56:30.000000 pyvips-2.2.3/tests/test_image.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2182 2024-01-05 20:02:19.000000 pyvips-2.2.3/tests/test_progress.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2216 2024-01-05 20:02:19.000000 pyvips-2.2.3/tests/test_saveload.py
```

### Comparing `pyvips-2.2.2/LICENSE.txt` & `pyvips-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/PKG-INFO` & `pyvips-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvips
-Version: 2.2.2
+Version: 2.2.3
 Summary: binding for the libvips image processing library, API mode
 Home-page: https://github.com/libvips/pyvips
 Author: John Cupitt
 Author-email: jcupitt@gmail.com
 License: MIT
 Keywords: image processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,17 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.txt
 
 README
 ======
 
@@ -276,11 +277,11 @@
     $ vi doc/conf.py
 
 Update pypi package:
 
 .. code-block:: shell
 
     $ python3 setup.py sdist
-    $ twine upload dist/*
+    $ twine upload --repository pyvips dist/*
     $ git tag -a v2.2.0 -m "as uploaded to pypi"
     $ git push origin v2.2.0
```

### Comparing `pyvips-2.2.2/README.rst` & `pyvips-2.2.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -243,11 +243,11 @@
     $ vi doc/conf.py
 
 Update pypi package:
 
 .. code-block:: shell
 
     $ python3 setup.py sdist
-    $ twine upload dist/*
+    $ twine upload --repository pyvips dist/*
     $ git tag -a v2.2.0 -m "as uploaded to pypi"
     $ git push origin v2.2.0
```

### Comparing `pyvips-2.2.2/pyvips/__init__.py` & `pyvips-2.2.3/pyvips/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
     ffi = _libvips.ffi
     vips_lib = _libvips.lib
     glib_lib = _libvips.lib
     gobject_lib = _libvips.lib
 
     # now check that the binary wrapper is for the same version of libvips that
-    # we find ourseleves linking to at runtime ... if it isn't, we must fall 
+    # we find ourseleves linking to at runtime ... if it isn't, we must fall
     # back to ABI mode
     lib_major = vips_lib.vips_version(0)
     lib_minor = vips_lib.vips_version(1)
     wrap_major = vips_lib.VIPS_MAJOR_VERSION
     wrap_minor = vips_lib.VIPS_MINOR_VERSION
-    logger.debug('Module generated for libvips %s.%s' % 
-                 (wrap_major, wrap_minor)) 
-    logger.debug('Linked to libvips %s.%s' % (lib_major, lib_minor)) 
+    logger.debug('Module generated for libvips %s.%s' %
+                 (wrap_major, wrap_minor))
+    logger.debug('Linked to libvips %s.%s' % (lib_major, lib_minor))
 
     if wrap_major != lib_major or wrap_minor != lib_minor:
         raise Exception('bad wrapper version')
 
     API_mode = True
 
 except Exception as e:
@@ -50,36 +50,43 @@
     ffi = FFI()
 
     _is_windows = os.name == 'nt'
     _is_mac = sys.platform == 'darwin'
 
     # yuk
     if _is_windows:
-        _glib_libname = 'libglib-2.0-0.dll'
-        _gobject_libname = 'libgobject-2.0-0.dll'
-        _vips_libname = 'libvips-42.dll'
+        vips_lib = ffi.dlopen('libvips-42.dll')
     elif _is_mac:
-        _glib_libname = None
-        _vips_libname = 'libvips.42.dylib'
-        _gobject_libname = 'libgobject-2.0.dylib'
+        vips_lib = ffi.dlopen('libvips.42.dylib')
     else:
-        _glib_libname = None
-        _vips_libname = 'libvips.so.42'
-        _gobject_libname = 'libgobject-2.0.so.0'
-
-    # possibly use ctypes.util.find_library() to locate the lib?
-    gobject_lib = ffi.dlopen(_gobject_libname)
-    vips_lib = ffi.dlopen(_vips_libname)
-    if _glib_libname:
-        glib_lib = ffi.dlopen(_glib_libname)
-    else:
-        glib_lib = gobject_lib
+        vips_lib = ffi.dlopen('libvips.so.42')
 
     logger.debug('Loaded lib %s', vips_lib)
-    logger.debug('Loaded lib %s', gobject_lib)
+
+    if _is_windows:
+        # On Windows, `GetProcAddress()` can only search in a specified DLL and
+        # doesn't look into its dependent libraries for symbols. Therefore, we
+        # check if the GLib DLLs are available. If these can not be found, we
+        # assume that GLib is statically linked into libvips.
+        try:
+            glib_lib = ffi.dlopen('libglib-2.0-0.dll')
+            gobject_lib = ffi.dlopen('libgobject-2.0-0.dll')
+
+            logger.debug('Loaded lib %s', glib_lib)
+            logger.debug('Loaded lib %s', gobject_lib)
+        except Exception:
+            glib_lib = vips_lib
+            gobject_lib = vips_lib
+    else:
+        # macOS and *nix uses `dlsym()`, which also searches for named symbols
+        # in the dependencies of the shared library. Therefore, we can support
+        # a single shared libvips library with all dependencies statically
+        # linked.
+        glib_lib = vips_lib
+        gobject_lib = vips_lib
 
     ffi.cdef('''
         int vips_init (const char* argv0);
         int vips_version (int flag);
     ''')
 
 if vips_lib.vips_init(sys.argv[0].encode()) != 0:
@@ -98,40 +105,42 @@
         'minor': minor,
         'micro': micro,
         'api': False,
     }
 
     ffi.cdef(cdefs(features))
 
+
 from .error import *
 
 # redirect all vips warnings to logging
 
 class GLogLevelFlags(object):
-    # log flags 
+    # log flags
     FLAG_RECURSION          = 1 << 0
     FLAG_FATAL              = 1 << 1
 
-    # GLib log levels 
+    # GLib log levels
     LEVEL_ERROR             = 1 << 2       # always fatal 
     LEVEL_CRITICAL          = 1 << 3
     LEVEL_WARNING           = 1 << 4
     LEVEL_MESSAGE           = 1 << 5
     LEVEL_INFO              = 1 << 6
     LEVEL_DEBUG             = 1 << 7
 
     LEVEL_TO_LOGGER = {
-        LEVEL_DEBUG : 10,
-        LEVEL_INFO : 20,
-        LEVEL_MESSAGE : 20,
-        LEVEL_WARNING : 30,
-        LEVEL_ERROR : 40,
-        LEVEL_CRITICAL : 50,
+        LEVEL_DEBUG: 10,
+        LEVEL_INFO: 20,
+        LEVEL_MESSAGE: 20,
+        LEVEL_WARNING: 30,
+        LEVEL_ERROR: 40,
+        LEVEL_CRITICAL: 50,
     }
 
+
 if API_mode:
     @ffi.def_extern()
     def _log_handler_callback(domain, level, message, user_data):
         logger.log(GLogLevelFlags.LEVEL_TO_LOGGER[level],
                    '{0}: {1}'.format(_to_string(domain), _to_string(message)))
 
     # keep a ref to the cb to stop it being GCd
@@ -140,24 +149,24 @@
     def _log_handler_callback(domain, level, message, user_data):
         logger.log(GLogLevelFlags.LEVEL_TO_LOGGER[level],
                    '{0}: {1}'.format(_to_string(domain), _to_string(message)))
 
     # keep a ref to the cb to stop it being GCd
     _log_handler_cb = ffi.callback('GLogFunc', _log_handler_callback)
 
-_log_handler_id = glib_lib.g_log_set_handler(_to_bytes('VIPS'), 
-                           GLogLevelFlags.LEVEL_DEBUG | 
-                           GLogLevelFlags.LEVEL_INFO | 
-                           GLogLevelFlags.LEVEL_MESSAGE | 
-                           GLogLevelFlags.LEVEL_WARNING | 
-                           GLogLevelFlags.LEVEL_CRITICAL | 
-                           GLogLevelFlags.LEVEL_ERROR | 
-                           GLogLevelFlags.FLAG_FATAL | 
-                           GLogLevelFlags.FLAG_RECURSION,
-                           _log_handler_cb, ffi.NULL)
+_log_handler_id = glib_lib.g_log_set_handler(_to_bytes('VIPS'),
+                                             GLogLevelFlags.LEVEL_DEBUG |
+                                             GLogLevelFlags.LEVEL_INFO |
+                                             GLogLevelFlags.LEVEL_MESSAGE |
+                                             GLogLevelFlags.LEVEL_WARNING |
+                                             GLogLevelFlags.LEVEL_CRITICAL |
+                                             GLogLevelFlags.LEVEL_ERROR |
+                                             GLogLevelFlags.FLAG_FATAL |
+                                             GLogLevelFlags.FLAG_RECURSION,
+                                             _log_handler_cb, ffi.NULL)
 
 # ffi doesn't like us looking up methods during shutdown: make a note of the
 # remove handler here
 _remove_handler = glib_lib.g_log_remove_handler
 
 # we must remove the handler on exit or libvips may try to run the callback
 # during shutdown
@@ -165,14 +174,15 @@
     global _log_handler_id
     global _remove_handler
 
     if _log_handler_id:
         _remove_handler(_to_bytes('VIPS'), _log_handler_id)
         _log_handler_id = None
 
+
 atexit.register(_remove_log_handler)
 
 from .enums import *
 from .base import *
 from .gobject import *
 from .gvalue import *
 from .vobject import *
```

### Comparing `pyvips-2.2.2/pyvips/enums.py` & `pyvips-2.2.3/pyvips/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1313,27 +1313,14 @@
 
     """
 
     SET = 'set'
     ADD = 'add'
 
 
-class Token(object):
-    """Token.
-
-Attributes:
-
-    """
-
-    LEFT = 'left'
-    RIGHT = 'right'
-    STRING = 'string'
-    EQUALS = 'equals'
-
-
 class Saveable(object):
     """Saveable.
 
 See also: #VipsForeignSave.
 
 Attributes:
 
@@ -1355,31 +1342,14 @@
     RGB = 'rgb'
     RGBA = 'rgba'
     RGBA_ONLY = 'rgba-only'
     RGB_CMYK = 'rgb-cmyk'
     ANY = 'any'
 
 
-class ImageType(object):
-    """ImageType.
-
-Attributes:
-
-    """
-
-    ERROR = 'error'
-    NONE = 'none'
-    SETBUF = 'setbuf'
-    SETBUF_FOREIGN = 'setbuf-foreign'
-    OPENIN = 'openin'
-    MMAPIN = 'mmapin'
-    MMAPINRW = 'mmapinrw'
-    OPENOUT = 'openout'
-
-
 class ForeignKeep(object):
     """ForeignKeep.
 
 Which metadata to retain.
 
 Attributes:
```

### Comparing `pyvips-2.2.2/pyvips/error.py` & `pyvips-2.2.3/pyvips/error.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/gobject.py` & `pyvips-2.2.3/pyvips/gobject.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/gvalue.py` & `pyvips-2.2.3/pyvips/gvalue.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,44 +222,25 @@
                 array[i] = image.pointer
         elif gtype == GValue.blob_type:
             # we need to set the blob to a copy of the string that vips_lib
             # can own
             memory = glib_lib.g_malloc(len(value))
             ffi.memmove(memory, value, len(value))
 
-            # this is horrible!
-            #
-            # * in API mode, we must have 8.6+ and use set_blob_free to
-            #   attach the metadata to avoid leaks
-            # * pre-8.6, we just pass a NULL free pointer and live with the
-            #   leak
-            #
-            # this is because in API mode you can't pass a builtin (what
-            # vips_lib.g_free() becomes) as a parameter to ffi.callback(), and
-            # vips_value_set_blob() needs a callback for arg 2
-            #
-            # additionally, you can't make a py def which calls g_free() and
-            # then use the py def in the callback, since libvips will trigger
-            # these functions during cleanup, and py will have shut down by
-            # then and you'll get a segv
-
-            if at_least_libvips(8, 6):
+            # In API mode, we use set_blob_free in a backwards compatible way.
+            # For pre-8.6 libvipses, in ABI mode, we declare the type of the
+            # free func in set_blob incorrectly so that we can pass g_free
+            # at runtime without triggering an exception.
+            if pyvips.API_mode or at_least_libvips(8, 6):
                 vips_lib.vips_value_set_blob_free(self.gvalue,
                                                   memory, len(value))
             else:
-                # we declare the type of the free func in set_blob incorrectly
-                # so that we can pass g_free at runtime without triggering an
-                # exception
-                if pyvips.API_mode:
-                    vips_lib.vips_value_set_blob(self.gvalue,
-                                                 ffi.NULL, memory, len(value))
-                else:
-                    vips_lib.vips_value_set_blob(self.gvalue,
-                                                 glib_lib.g_free,
-                                                 memory, len(value))
+                vips_lib.vips_value_set_blob(self.gvalue,
+                                             glib_lib.g_free,
+                                             memory, len(value))
         else:
             raise Error('unsupported gtype for set {0}, fundamental {1}'.
                         format(type_name(gtype), type_name(fundamental)))
 
     def get(self):
         """Get the contents of a GValue.
```

### Comparing `pyvips-2.2.2/pyvips/vconnection.py` & `pyvips-2.2.3/pyvips/vconnection.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vdecls.py` & `pyvips-2.2.3/pyvips/vdecls.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,53 +41,56 @@
             typedef guint64 GType;
         '''
     else:
         code += '''
             typedef guint32 GType;
         '''
 
+    # ... means opaque
     code += '''
         typedef void (*GLogFunc) (const char* log_domain,
             int log_level,
             const char* message, void* user_data);
         int g_log_set_handler (const char* log_domain,
             int log_levels,
             GLogFunc log_func, void* user_data);
 
         extern "Python" void _log_handler_callback (const char*, int,
             const char*, void*);
 
         void g_log_remove_handler (const char* log_domain, int handler_id);
 
-        typedef struct _VipsImage VipsImage;
-        typedef struct _VipsProgress VipsProgress;
-        typedef struct _GValue GValue;
+        typedef ... VipsImage;
 
         void* g_malloc (size_t size);
         void g_free (void* data);
 
         void vips_leak_set (int leak);
 
         GType vips_type_find (const char* basename, const char* nickname);
         const char* vips_nickname_find (GType type);
 
         const char* g_type_name (GType gtype);
         GType g_type_from_name (const char* name);
 
-        typedef void* (*VipsTypeMap2Fn) (GType type, void* a, void* b);
+        typedef ... VipsTypeMap2Fn;
         void* vips_type_map (GType base, VipsTypeMap2Fn fn, void* a, void* b);
 
         const char* vips_error_buffer (void);
         void vips_error_clear (void);
         void vips_error_freeze (void);
         void vips_error_thaw (void);
 
         typedef struct _GValue {
             GType g_type;
-            guint64 data[2];
+            union {
+                guint64 v_uint64;
+
+                // more
+            } data[2];
         } GValue;
 
         void g_value_init (GValue* value, GType gtype);
         void g_value_unset (GValue* value);
         GType g_type_fundamental (GType gtype);
 
         int vips_enum_from_nick (const char* domain,
@@ -106,17 +109,14 @@
         void vips_value_set_ref_string (GValue* value, const char* str);
         void g_value_set_object (GValue* value, void* object);
         void vips_value_set_array_double (GValue* value,
             const double* array, int n );
         void vips_value_set_array_int (GValue* value,
             const int* array, int n );
         void vips_value_set_array_image (GValue *value, int n);
-        typedef void (*FreeFn)(void* a);
-        void vips_value_set_blob (GValue* value,
-            FreeFn free_fn, void* data, size_t length);
 
         int g_value_get_boolean (const GValue* value);
         int g_value_get_int (GValue* value);
         guint64 g_value_get_uint64 (GValue* value);
         double g_value_get_double (GValue* value);
         int g_value_get_enum (GValue* value);
         unsigned int g_value_get_flags (GValue* value);
@@ -133,24 +133,27 @@
         GType vips_interpretation_get_type (void);
         GType vips_operation_flags_get_type (void);
         GType vips_band_format_get_type (void);
         GType vips_token_get_type (void);
         GType vips_saveable_get_type (void);
         GType vips_image_type_get_type (void);
 
-        typedef struct _GData GData;
+        typedef ... GData;
 
-        typedef struct _GTypeClass GTypeClass;
+        typedef struct _GTypeClass {
+            GType g_type;
+        } GTypeClass;
 
         typedef struct _GTypeInstance {
             GTypeClass *g_class;
         } GTypeInstance;
 
         typedef struct _GObject {
             GTypeInstance g_type_instance;
+
             unsigned int ref_count;
             GData *qdata;
         } GObject;
 
         typedef struct _GParamSpec {
             GTypeInstance g_type_instance;
 
@@ -172,15 +175,15 @@
             int value;
 
             const char *value_name;
             const char *value_nick;
         } GEnumValue;
 
         typedef struct _GEnumClass {
-            GTypeClass *g_type_class;
+            GTypeClass g_type_class;
 
             int minimum;
             int maximum;
             unsigned int n_values;
             GEnumValue *values;
         } GEnumClass;
 
@@ -188,15 +191,15 @@
             unsigned int value;
 
             const char *value_name;
             const char *value_nick;
         } GFlagsValue;
 
         typedef struct _GFlagsClass {
-            GTypeClass *g_type_class;
+            GTypeClass g_type_class;
 
             unsigned int mask;
             unsigned int n_values;
             GFlagsValue *values;
         } GFlagsClass;
 
         void* g_type_class_ref (GType type);
@@ -223,51 +226,30 @@
 
         extern "Python" void _marshal_image_progress (VipsImage*,
             void*, void*);
 
         void vips_image_set_progress (VipsImage* image, int progress);
         void vips_image_set_kill (VipsImage* image, int kill);
 
+        typedef ... GTimer;
+
         typedef struct _VipsProgress {
             VipsImage* im;
 
             int run;
             int eta;
             gint64 tpels;
             gint64 npels;
             int percent;
-            void* start;
+            GTimer* start;
         } VipsProgress;
 
-        typedef struct _VipsObject {
-    '''
+        typedef ... VipsObject;
 
-    # this field changed name in libvips 8.4
-    if _at_least(features, 8, 4):
-        code += '''
-            GObject parent_instance;
-        '''
-    else:
-        code += '''
-            GObject parent_object;
-        '''
-
-    code += '''
-            int constructed;
-            int static_object;
-            void *argument_table;
-            char *nickname;
-            char *description;
-            int preclose;
-            int close;
-            int postclose;
-            size_t local_memory;
-        } VipsObject;
-
-        typedef struct _VipsObjectClass VipsObjectClass;
+        typedef ... VipsObjectClass;
 
         typedef struct _VipsArgument {
             GParamSpec *pspec;
         } VipsArgument;
 
         typedef struct _VipsArgumentInstance {
             VipsArgument parent;
@@ -306,31 +288,14 @@
         int vips_object_set_from_string (VipsObject* object,
             const char* options);
 
         const char* vips_object_get_description (VipsObject* object);
 
         const char* g_param_spec_get_blurb (GParamSpec* pspec);
 
-        typedef struct _VipsImage {
-    '''
-
-    # this field changed name in libvips 8.4
-    if _at_least(features, 8, 4):
-        code += '''
-            VipsObject parent_instance;
-        '''
-    else:
-        code += '''
-            VipsObject parent_object;
-        '''
-
-    code += '''
-            // more
-        } VipsImage;
-
         const char* vips_foreign_find_load (const char* name);
         const char* vips_foreign_find_load_buffer (const void* data,
             size_t size);
         const char* vips_foreign_find_save (const char* name);
         const char* vips_foreign_find_save_buffer (const char* suffix);
 
         VipsImage* vips_image_new_matrix_from_array (int width, int height,
@@ -352,44 +317,32 @@
         char* vips_filename_get_options (const char* vips_filename);
 
         VipsImage* vips_image_new_temp_file (const char* format);
 
         int vips_image_write (VipsImage* image, VipsImage* out);
         void* vips_image_write_to_memory (VipsImage* in, size_t* size_out);
 
-        typedef struct _VipsInterpolate {
-            VipsObject parent_object;
-
-            // more
-        } VipsInterpolate;
+        typedef ... VipsInterpolate;
 
         VipsInterpolate* vips_interpolate_new (const char* name);
 
-        typedef struct _VipsOperation {
-            VipsObject parent_instance;
-
-            // more
-        } VipsOperation;
+        typedef ... VipsOperation;
 
         VipsOperation* vips_operation_new (const char* name);
 
         typedef void* (*VipsArgumentMapFn) (VipsObject* object,
             GParamSpec* pspec,
             VipsArgumentClass* argument_class,
             VipsArgumentInstance* argument_instance,
             void* a, void* b);
 
         void* vips_argument_map (VipsObject* object,
             VipsArgumentMapFn fn, void* a, void* b);
 
-        typedef struct _VipsRegion {
-            VipsObject parent_object;
-
-            // more
-        } VipsRegion;
+        typedef ... VipsRegion;
 
         VipsRegion* vips_region_new (VipsImage*);
 
         VipsOperation* vips_cache_operation_build (VipsOperation* operation);
         void vips_object_unref_outputs (VipsObject* object);
 
         int vips_operation_get_flags (VipsOperation* operation);
@@ -401,14 +354,23 @@
 
         int vips_cache_get_max();
         int vips_cache_get_size();
         size_t vips_cache_get_max_mem();
         int vips_cache_get_max_files();
     '''
 
+    # we must only define this in ABI mode ... in API mode we use
+    # vips_value_set_blob_free in a backwards compatible way
+    if not features['api']:
+        code += '''
+            typedef void (*FreeFn)(void* a);
+            void vips_value_set_blob (GValue* value,
+                FreeFn free_fn, void* data, size_t length);
+        '''
+
     if _at_least(features, 8, 5):
         code += '''
             char** vips_image_get_fields (VipsImage* image);
             int vips_image_hasalpha (VipsImage* image);
 
         '''
 
@@ -438,62 +400,42 @@
             int vips_image_get_page_height (VipsImage*);
             int vips_image_get_n_pages (VipsImage*);
 
         '''
 
     if _at_least(features, 8, 9):
         code += '''
-            typedef struct _VipsConnection {
-                VipsObject parent_object;
-
-                // more
-            } VipsConnection;
+            typedef ... VipsConnection;
 
             const char* vips_connection_filename (VipsConnection* stream);
             const char* vips_connection_nick (VipsConnection* stream);
 
-            typedef struct _VipsSource {
-                VipsConnection parent_object;
-
-                // more
-            } VipsSource;
+            typedef ... VipsSource;
 
             VipsSource* vips_source_new_from_descriptor (int descriptor);
             VipsSource* vips_source_new_from_file (const char* filename);
             VipsSource* vips_source_new_from_memory (const void* data,
                 size_t size);
 
-            typedef struct _VipsSourceCustom {
-                VipsSource parent_object;
-
-                // more
-            } VipsSourceCustom;
+            typedef ... VipsSourceCustom;
 
             VipsSourceCustom* vips_source_custom_new (void);
 
             extern "Python" gint64 _marshal_read (VipsSource*,
                 void*, gint64, void*);
             extern "Python" gint64 _marshal_seek (VipsSource*,
                 gint64, int, void*);
 
-            typedef struct _VipsTarget {
-                VipsConnection parent_object;
-
-                // more
-            } VipsTarget;
+            typedef ... VipsTarget;
 
             VipsTarget* vips_target_new_to_descriptor (int descriptor);
             VipsTarget* vips_target_new_to_file (const char* filename);
             VipsTarget* vips_target_new_to_memory (void);
 
-            typedef struct _VipsTargetCustom {
-                VipsTarget parent_object;
-
-                // more
-            } VipsTargetCustom;
+            typedef ... VipsTargetCustom;
 
             VipsTargetCustom* vips_target_custom_new (void);
 
             extern "Python" gint64 _marshal_write (VipsTarget*,
                 void*, gint64, void*);
             extern "Python" void _marshal_finish (VipsTarget*,
                 void*);
@@ -518,17 +460,19 @@
     if features['api']:
         code += '''
             int vips_init (const char* argv0);
             int vips_version (int flag);
         '''
 
     # ... means inherit from C defines
-    code += '#define VIPS_MAJOR_VERSION ...\n'
-    code += '#define VIPS_MINOR_VERSION ...\n'
-    code += '#define VIPS_MICRO_VERSION ...\n'
+    code += '''
+        #define VIPS_MAJOR_VERSION ...
+        #define VIPS_MINOR_VERSION ...
+        #define VIPS_MICRO_VERSION ...
+    '''
 
     # add contents of features as a comment ... handy for debugging
     for key, value in features.items():
         code += '//%s = %s\n' % (key, value)
 
     return code
```

### Comparing `pyvips-2.2.2/pyvips/vimage.py` & `pyvips-2.2.3/pyvips/vimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,16 +660,23 @@
 
         """
         pointer = vips_lib.vips_foreign_find_load_source(source.pointer)
         if pointer == ffi.NULL:
             raise Error('unable to load from source')
         name = _to_string(pointer)
 
-        return pyvips.Operation.call(name, source,
-                                     string_options=options, **kwargs)
+        image = pyvips.Operation.call(name, source,
+                                      string_options=options, **kwargs)
+
+        # keep a secret ref to the source object .. we need that to stay
+        # alive, since it might be a custom source that triggers a python
+        # callback
+        image._references.append(source)
+
+        return image
 
     @staticmethod
     def new_temp_file(format):
         """Make a new temporary image.
 
         Returns an image backed by a temporary file. When written to with
         :func:`Image.write`, a temporary file will be created on disc in the
@@ -1875,14 +1882,16 @@
         """True if the image has an alpha channel."""
         return vips_lib.vips_image_hasalpha(self.pointer)
 
     def addalpha(self):
         """Add an alpha channel."""
         if self.interpretation == 'grey16' or self.interpretation == 'rgb16':
             max_alpha = 65535
+        elif self.interpretation == 'scrgb':
+            max_alpha = 1.0
         else:
             max_alpha = 255
         return self.bandjoin(max_alpha)
 
     # we need different _imageize rules for this operator ... we need to
     # _imageize in1 and in2 to match each other first
     @_add_doc('ifthenelse')
```

### Comparing `pyvips-2.2.2/pyvips/vinterpolate.py` & `pyvips-2.2.3/pyvips/vinterpolate.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vobject.py` & `pyvips-2.2.3/pyvips/vobject.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/voperation.py` & `pyvips-2.2.3/pyvips/voperation.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vregion.py` & `pyvips-2.2.3/pyvips/vregion.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vsource.py` & `pyvips-2.2.3/pyvips/vsource.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vsourcecustom.py` & `pyvips-2.2.3/pyvips/vsourcecustom.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vtarget.py` & `pyvips-2.2.3/pyvips/vtarget.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips/vtargetcustom.py` & `pyvips-2.2.3/pyvips/vtargetcustom.py`

 * *Files identical despite different names*

### Comparing `pyvips-2.2.2/pyvips.egg-info/PKG-INFO` & `pyvips-2.2.3/pyvips.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvips
-Version: 2.2.2
+Version: 2.2.3
 Summary: binding for the libvips image processing library, API mode
 Home-page: https://github.com/libvips/pyvips
 Author: John Cupitt
 Author-email: jcupitt@gmail.com
 License: MIT
 Keywords: image processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,17 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.txt
 
 README
 ======
 
@@ -276,11 +277,11 @@
     $ vi doc/conf.py
 
 Update pypi package:
 
 .. code-block:: shell
 
     $ python3 setup.py sdist
-    $ twine upload dist/*
+    $ twine upload --repository pyvips dist/*
     $ git tag -a v2.2.0 -m "as uploaded to pypi"
     $ git push origin v2.2.0
```

### Comparing `pyvips-2.2.2/pyvips.egg-info/SOURCES.txt` & `pyvips-2.2.3/pyvips.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,15 @@
 pyvips/vtarget.py
 pyvips/vtargetcustom.py
 pyvips.egg-info/PKG-INFO
 pyvips.egg-info/SOURCES.txt
 pyvips.egg-info/dependency_links.txt
 pyvips.egg-info/not-zip-safe
 pyvips.egg-info/requires.txt
-pyvips.egg-info/top_level.txt
+pyvips.egg-info/top_level.txt
+tests/test_block.py
+tests/test_connections.py
+tests/test_constants.py
+tests/test_gvalue.py
+tests/test_image.py
+tests/test_progress.py
+tests/test_saveload.py
```

### Comparing `pyvips-2.2.2/setup.py` & `pyvips-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
-    'Programming Language :: Python :: Implementation :: PyPy',
+    'Programming Language :: Python :: 3.12',
     'Programming Language :: Python :: Implementation :: CPython',
+    'Programming Language :: Python :: Implementation :: PyPy',
 ]
 
 setup_deps = [
     'cffi>=1.0.0',
 ]
 
 install_deps = [
```

