# Comparing `tmp/py_win_task_scheduler-0.2.0.tar.gz` & `tmp/py_win_task_scheduler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_win_task_scheduler-0.2.0.tar", last modified: Wed Jan 10 19:21:55 2024, max compression
+gzip compressed data, was "py_win_task_scheduler-0.2.1.tar", last modified: Sun Apr 28 20:06:08 2024, max compression
```

## Comparing `py_win_task_scheduler-0.2.0.tar` & `py_win_task_scheduler-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 19:21:55.521282 py_win_task_scheduler-0.2.0/
--rw-rw-rw-   0        0        0     1092 2023-03-04 08:13:23.000000 py_win_task_scheduler-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1905 2024-01-10 19:21:55.521282 py_win_task_scheduler-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1086 2023-03-04 08:39:56.000000 py_win_task_scheduler-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-10 19:21:55.517305 py_win_task_scheduler-0.2.0/py_win_task_scheduler/
--rw-rw-rw-   0        0        0    84833 2024-01-10 19:12:52.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 19:21:55.520310 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/
--rw-rw-rw-   0        0        0     1905 2024-01-10 19:21:55.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-01-10 19:21:55.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 19:21:55.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-10 19:21:55.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-01-10 19:21:55.000000 py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      876 2024-01-10 19:21:55.522279 py_win_task_scheduler-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-04-25 19:06:18.000000 py_win_task_scheduler-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:06:08.330071 py_win_task_scheduler-0.2.1/
+-rw-rw-rw-   0        0        0     1092 2023-03-04 08:13:23.000000 py_win_task_scheduler-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1878 2024-04-28 20:06:08.330071 py_win_task_scheduler-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1086 2023-03-04 08:39:56.000000 py_win_task_scheduler-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 20:06:08.299983 py_win_task_scheduler-0.2.1/py_win_task_scheduler/
+-rw-rw-rw-   0        0        0    84732 2024-04-28 20:01:13.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:06:08.330071 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/
+-rw-rw-rw-   0        0        0     1878 2024-04-28 20:06:07.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-28 20:06:07.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:06:07.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:06:07.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-28 20:06:07.000000 py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      878 2024-04-28 20:06:08.331325 py_win_task_scheduler-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       75 2022-04-25 19:06:18.000000 py_win_task_scheduler-0.2.1/setup.py
```

### Comparing `py_win_task_scheduler-0.2.0/LICENSE` & `py_win_task_scheduler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_win_task_scheduler-0.2.0/PKG-INFO` & `py_win_task_scheduler-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: py_win_task_scheduler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Script to work with Windows Task Scheduler 2.0 from SaltStack
 Home-page: https://github.com/dolamroth/py_win_task_scheduler
-Download-URL: https://github.com/dolamroth/py_win_task_scheduler/archive/refs/tags/0.2.tar.gz
+Download-URL: https://github.com/dolamroth/py_win_task_scheduler/archive/refs/tags/0.2.1.tar.gz
 Author: Sergey Sayamov
 Author-email: dolamroth71@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: pywin32>=306
 
 ## Python scripts for Windows Task Scheduler 2.0 from SaltStack
 
 This is a copy of a `https://github.com/saltstack/salt/blob/master/salt/modules/win_task.py`
 from `https://github.com/saltstack/salt` (Apache 2.0 Licence) as a separate repository.
 
 ## Installation and usage
```

### Comparing `py_win_task_scheduler-0.2.0/README.md` & `py_win_task_scheduler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py_win_task_scheduler-0.2.0/py_win_task_scheduler/__init__.py` & `py_win_task_scheduler-0.2.1/py_win_task_scheduler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,16 +311,14 @@
             password,
             logon_type,
         )
 
         return True
 
     except pythoncom.com_error as error:
-        import traceback_with_variables
-        print(traceback_with_variables.format_exc(error, num_skipped_frames=0))
         hr, msg, exc, arg = error.args  # pylint: disable=W0633
         fc = {
             -2147024773: "The filename, directory name, or volume label "
             "syntax is incorrect",
             -2147024894: "The system cannot find the file specified",
             -2147216615: "Required element or attribute missing",
             -2147216616: "Value incorrectly formatted or out of range",
@@ -582,25 +580,25 @@
         # Add Trigger
         add_trigger(task_definition=task_definition, **kwargs)
 
         # get the folder to create the task in
         task_folder = task_service.GetFolder(location)
 
         # Save the task
-        _save_task_definition(
+        ret_val = _save_task_definition(
             name=name,
             task_folder=task_folder,
             task_definition=task_definition,
             user_name=task_definition.Principal.UserID,
             password=password,
             logon_type=task_definition.Principal.LogonType,
         )
 
     # Verify task was created
-    return name in list_tasks(location)
+    return (name in list_tasks(location), ret_val)
 
 
 def create_task_from_xml(
     name, location="\\", xml_text=None, xml_path=None, user_name="System", password=None
 ):
     r"""
     Create a task based on XML. Source can be a file or a string of XML.
```

### Comparing `py_win_task_scheduler-0.2.0/py_win_task_scheduler.egg-info/PKG-INFO` & `py_win_task_scheduler-0.2.1/py_win_task_scheduler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: py_win_task_scheduler
-Version: 0.2.0
+Name: py-win-task-scheduler
+Version: 0.2.1
 Summary: Script to work with Windows Task Scheduler 2.0 from SaltStack
 Home-page: https://github.com/dolamroth/py_win_task_scheduler
-Download-URL: https://github.com/dolamroth/py_win_task_scheduler/archive/refs/tags/0.2.tar.gz
+Download-URL: https://github.com/dolamroth/py_win_task_scheduler/archive/refs/tags/0.2.1.tar.gz
 Author: Sergey Sayamov
 Author-email: dolamroth71@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: pywin32>=306
 
 ## Python scripts for Windows Task Scheduler 2.0 from SaltStack
 
 This is a copy of a `https://github.com/saltstack/salt/blob/master/salt/modules/win_task.py`
 from `https://github.com/saltstack/salt` (Apache 2.0 Licence) as a separate repository.
 
 ## Installation and usage
```

### Comparing `py_win_task_scheduler-0.2.0/setup.cfg` & `py_win_task_scheduler-0.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 795f 7769 6e5f 7461 736b 5f73   = py_win_task_s
 00000020: 6368 6564 756c 6572 0d0a 7665 7273 696f  cheduler..versio
-00000030: 6e20 3d20 302e 322e 300d 0a64 6573 6372  n = 0.2.0..descr
+00000030: 6e20 3d20 302e 322e 310d 0a64 6573 6372  n = 0.2.1..descr
 00000040: 6970 7469 6f6e 203d 2053 6372 6970 7420  iption = Script 
 00000050: 746f 2077 6f72 6b20 7769 7468 2057 696e  to work with Win
 00000060: 646f 7773 2054 6173 6b20 5363 6865 6475  dows Task Schedu
 00000070: 6c65 7220 322e 3020 6672 6f6d 2053 616c  ler 2.0 from Sal
 00000080: 7453 7461 636b 0d0a 6c6f 6e67 5f64 6573  tStack..long_des
 00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
 000000a0: 2052 4541 444d 452e 6d64 0d0a 7572 6c20   README.md..url 
@@ -17,39 +17,39 @@
 00000100: 7574 686f 725f 656d 6169 6c20 3d20 646f  uthor_email = do
 00000110: 6c61 6d72 6f74 6837 3140 676d 6169 6c2e  lamroth71@gmail.
 00000120: 636f 6d0d 0a64 6f77 6e6c 6f61 645f 7572  com..download_ur
 00000130: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000140: 7562 2e63 6f6d 2f64 6f6c 616d 726f 7468  ub.com/dolamroth
 00000150: 2f70 795f 7769 6e5f 7461 736b 5f73 6368  /py_win_task_sch
 00000160: 6564 756c 6572 2f61 7263 6869 7665 2f72  eduler/archive/r
-00000170: 6566 732f 7461 6773 2f30 2e32 2e74 6172  efs/tags/0.2.tar
-00000180: 2e67 7a0d 0a6c 6963 656e 7365 203d 204d  .gz..license = M
-00000190: 4954 204c 6963 656e 7365 0d0a 636c 6173  IT License..clas
-000001a0: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
-000001b0: 6972 6f6e 6d65 6e74 203a 3a20 5769 6e33  ironment :: Win3
-000001c0: 3220 284d 5320 5769 6e64 6f77 7329 0d0a  2 (MS Windows)..
-000001d0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001f0: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000210: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-00000220: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
-00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000240: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 2e31 300d 0a09 5072 6f67 7261 6d6d 696e  .10...Programmin
-00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000290: 7468 6f6e 203a 3a20 332e 3131 0d0a 0950  thon :: 3.11...P
-000002a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002c0: 2033 2e31 320d 0a0d 0a5b 6f70 7469 6f6e   3.12....[option
-000002d0: 735d 0d0a 7079 7468 6f6e 5f72 6571 7569  s]..python_requi
-000002e0: 7265 7320 3d20 3e3d 332e 390d 0a70 6163  res = >=3.9..pac
-000002f0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
-00000300: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000310: 6174 6120 3d20 5472 7565 0d0a 696e 7374  ata = True..inst
-00000320: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000330: 0a09 7079 7769 6e33 323e 3d33 3036 0d0a  ..pywin32>=306..
-00000340: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000350: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000360: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000170: 6566 732f 7461 6773 2f30 2e32 2e31 2e74  efs/tags/0.2.1.t
+00000180: 6172 2e67 7a0d 0a6c 6963 656e 7365 203d  ar.gz..license =
+00000190: 204d 4954 204c 6963 656e 7365 0d0a 636c   MIT License..cl
+000001a0: 6173 7369 6669 6572 7320 3d20 0d0a 0945  assifiers = ...E
+000001b0: 6e76 6972 6f6e 6d65 6e74 203a 3a20 5769  nvironment :: Wi
+000001c0: 6e33 3220 284d 5320 5769 6e64 6f77 7329  n32 (MS Windows)
+000001d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001f0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+00000200: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000210: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+00000220: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000240: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
+00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000270: 2033 2e31 300d 0a09 5072 6f67 7261 6d6d   3.10...Programm
+00000280: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000290: 5079 7468 6f6e 203a 3a20 332e 3131 0d0a  Python :: 3.11..
+000002a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002c0: 3a3a 2033 2e31 320d 0a0d 0a5b 6f70 7469  :: 3.12....[opti
+000002d0: 6f6e 735d 0d0a 7079 7468 6f6e 5f72 6571  ons]..python_req
+000002e0: 7569 7265 7320 3d20 3e3d 332e 390d 0a70  uires = >=3.9..p
+000002f0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000300: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000310: 5f64 6174 6120 3d20 5472 7565 0d0a 696e  _data = True..in
+00000320: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000330: 200d 0a09 7079 7769 6e33 323e 3d33 3036   ...pywin32>=306
+00000340: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000350: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000360: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

