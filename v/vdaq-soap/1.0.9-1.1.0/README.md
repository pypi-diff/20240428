# Comparing `tmp/vdaq_soap-1.0.9.tar.gz` & `tmp/vdaq_soap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdaq_soap-1.0.9.tar", last modified: Fri Sep  1 15:18:30 2023, max compression
+gzip compressed data, was "vdaq_soap-1.1.0.tar", last modified: Sun Apr 28 08:52:30 2024, max compression
```

## Comparing `vdaq_soap-1.0.9.tar` & `vdaq_soap-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-09-01 15:18:30.727246 vdaq_soap-1.0.9/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-09-01 15:18:30.726924 vdaq_soap-1.0.9/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      408 2023-05-12 07:04:30.000000 vdaq_soap-1.0.9/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      957 2023-09-01 15:13:02.000000 vdaq_soap-1.0.9/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-09-01 15:18:30.727313 vdaq_soap-1.0.9/setup.cfg
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-09-01 15:18:30.724569 vdaq_soap-1.0.9/vdaq_soap/
--rw-r--r--   0 lacasta    (503) staff       (20)      334 2023-09-01 15:13:02.000000 vdaq_soap-1.0.9/vdaq_soap/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3237 2023-05-11 20:13:13.000000 vdaq_soap-1.0.9/vdaq_soap/analyzeHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4779 2023-05-11 20:06:02.000000 vdaq_soap-1.0.9/vdaq_soap/analyzeMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1645 2023-05-11 17:14:59.000000 vdaq_soap-1.0.9/vdaq_soap/data_utils.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    25791 2023-09-01 14:24:37.000000 vdaq_soap-1.0.9/vdaq_soap/soapCheckMadDaq.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3158 2023-09-01 14:58:29.000000 vdaq_soap-1.0.9/vdaq_soap/soapHoldDelay.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3121 2023-08-03 11:22:53.000000 vdaq_soap-1.0.9/vdaq_soap/soapMbias.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3153 2023-08-03 11:23:40.000000 vdaq_soap-1.0.9/vdaq_soap/soapTestChannel.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-09-01 15:18:30.726577 vdaq_soap-1.0.9/vdaq_soap.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      839 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      434 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      264 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       92 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-09-01 15:18:30.000000 vdaq_soap-1.0.9/vdaq_soap.egg-info/top_level.txt
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-28 08:52:30.053537 vdaq_soap-1.1.0/
+-rw-r--r--   0 lacasta    (501) staff       (20)     1024 2024-04-28 08:52:30.053357 vdaq_soap-1.1.0/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      409 2024-04-27 17:25:08.000000 vdaq_soap-1.1.0/README.md
+-rw-r--r--   0 lacasta    (501) staff       (20)      961 2024-04-27 17:37:07.000000 vdaq_soap-1.1.0/pyproject.toml
+-rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-04-28 08:52:30.053571 vdaq_soap-1.1.0/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-28 08:52:30.052384 vdaq_soap-1.1.0/vdaq_soap/
+-rw-r--r--   0 lacasta    (501) staff       (20)      336 2024-04-27 17:50:10.000000 vdaq_soap-1.1.0/vdaq_soap/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3227 2024-04-28 08:45:28.000000 vdaq_soap-1.1.0/vdaq_soap/analyzeHoldDelay.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4919 2024-04-27 21:19:12.000000 vdaq_soap-1.1.0/vdaq_soap/analyzeMbias.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1637 2024-04-27 21:19:29.000000 vdaq_soap-1.1.0/vdaq_soap/data_utils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    26417 2024-04-27 21:19:58.000000 vdaq_soap-1.1.0/vdaq_soap/soapCheckAliVATA.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3274 2024-04-27 17:33:45.000000 vdaq_soap-1.1.0/vdaq_soap/soapHoldDelay.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3574 2024-04-27 17:29:18.000000 vdaq_soap-1.1.0/vdaq_soap/soapMbias.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3295 2024-04-27 17:33:48.000000 vdaq_soap-1.1.0/vdaq_soap/soapTestChannel.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-28 08:52:30.053178 vdaq_soap-1.1.0/vdaq_soap.egg-info/
+-rw-r--r--   0 lacasta    (501) staff       (20)     1024 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      435 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      266 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       94 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       10 2024-04-28 08:52:30.000000 vdaq_soap-1.1.0/vdaq_soap.egg-info/top_level.txt
```

### Comparing `vdaq_soap-1.0.9/pyproject.toml` & `vdaq_soap-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vdaq_soap"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to control VDaq."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "daqpp>=2.0.3",
   "lmfit>=1.0.3",
-  "maddaq>=0.7.7",
+  "vdaq_ana>=0.7.7",
   "matplotlib>=3.3.0",
   "numpy>=1.19.0",
   "python_docx>=0.8.11"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.gui-scripts]
-soapCheckMadDaq = "vdaq_soap:soapCheckMadDaq"
+soapCheckAliVata = "vdaq_soap:soapCheckAliVata"
 soapHoldDelay = "vdaq_soap:soapHoldDelay"
 soapMbias = "vdaq_soap:soapMbias"
 soapTestChannel = "vdaq_soap:soapTestChannel"
 analyzeHoldDelay = "vdaq_soap:do_analyzeHoldDelay"
 analyzeMbias = "vdaq_soap:do_analyzeMbias"
 
 [project.urls]
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/analyzeHoldDelay.py` & `vdaq_soap-1.1.0/vdaq_soap/analyzeHoldDelay.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 import pathlib
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
-from maddaq import ShowProgress
+from vdaq_ana import ShowProgress
 
 from vdaq_soap.data_utils import open_data_file
 
 
-def read_hold_delay_data(fname, mod_id, thrs=-1, document=None):
+def read_hold_delay_data(fname, mod_id, emin=-1, document=None):
     """Read the scan data."""
     print(":> Opening {} for hold_delay analysis".format(fname))
-    maddaq = open_data_file(fname)
-    if maddaq is None:
+    vdaq = open_data_file(fname)
+    if vdaq is None:
         return
 
     # get the iterator of the Scan data
-    scan_iter = maddaq.scan_iter()
+    scan_iter = vdaq.scan_iter()
     scan_point = next(scan_iter)
     point_values = [scan_point.values[11]]
     point_mean = []
     point_data = []
 
-    prg = ShowProgress(maddaq.nevts, width=24)
+    prg = ShowProgress(vdaq.nevts, width=24)
     prg.start()
-    for evt in maddaq:
+    for evt in vdaq:
         # Get the module id
         mid = evt.mod_id
 
         if evt.evt_time > scan_point.end:
             # Next point
             try:
                 scan_point = next(scan_iter)
@@ -50,19 +50,19 @@
                 print("Stop iteration")
                 print(evt.evt_time, scan_point.end)
                 break
 
         if mid != mod_id:
             continue
 
-        md = maddaq.modules[mid]
+        md = vdaq.modules[mid]
         data = md.process_event(evt)
         if data is not None:
             for C, E in data:
-                if E > thrs:
+                if E > emin:
                     point_data.append(E)
 
         prg.increase(show=True)
 
     print("")
     point_mean.append(np.mean(point_data))
 
@@ -90,23 +90,23 @@
 
 def analyzeHoldDelay(files, options):
     """main entry."""
     ifile = Path(files[0]).expanduser().resolve()
     if not ifile.exists():
         return
 
-    read_hold_delay_data(ifile, options.mid, options.thrs, None)
+    read_hold_delay_data(ifile, options.mid, options.emin, None)
     plt.show()
 
 
 def do_analyzeHoldDelay():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
-    parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
+    parser.add_argument("--emin", default=0.0, type=float, help="Min E to show in histogram")
 
     parser.add_argument("--mid", dest="mid", default=11, type=int, help="The slot ID")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/analyzeMbias.py` & `vdaq_soap-1.1.0/vdaq_soap/analyzeMbias.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,53 @@
 import pathlib
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
-from maddaq import ShowProgress
+from vdaq_ana import ShowProgress
 
 from vdaq_soap.data_utils import open_data_file
 
 
-def read_mbias_scan(fname, mod_id, thrs=-1, document=None):
+def read_mbias_scan(fname, mod_id, emin=-1, document=None):
     """Read the mbias scan data.
 
     Args:
     ----
         fname: The file name
         mod_id: The modile ID
         document (optional): The word document. Defaults to None.
 
     """
     print(":> Opening {} for mbias analysis".format(fname))
-    maddaq = open_data_file(fname)
-    if maddaq is None:
+    vdaq = open_data_file(fname)
+    if vdaq is None:
         return
 
     # get the iterator of the Scan data
-    scan_iter = maddaq.scan_iter()
+    scan_iter = vdaq.scan_iter()
     scan_point = next(scan_iter)
     point_values = [scan_point.values[4]]
     point_mean = []
     point_rms = []
     point_data = []
     point_good = []
     good_chan = 0
     n_evts = 0
-    the_chan = scan_point.values[0]
 
-    prg = ShowProgress(maddaq.nevts, width=24)
+    try:
+        the_chan = scan_point.values[0]
+    except KeyError:
+        the_chan = -1
+
+    prg = ShowProgress(vdaq.nevts, width=24)
     prg.start()
-    for evt in maddaq:
+    for evt in vdaq:
         # Get the module id
         mid = evt.mod_id
 
         if evt.evt_time > scan_point.end:
             # Next point
             try:
                 scan_point = next(scan_iter)
@@ -59,37 +63,41 @@
                 if len(point_data) > 3:
                     point_mean.append(np.mean(point_data))
                     point_rms.append(np.std(point_data))
                 else:
                     point_mean.append(0)
                     point_rms.append(0)
 
-                the_chan = scan_point.values[0]
+                try:
+                    the_chan = scan_point.values[0]
+                except KeyError:
+                    the_chan = -1
+
                 n_evts = 0
                 good_chan = 0
                 point_data = []
 
             except StopIteration:
                 print("Stop iteration")
                 print(evt.evt_time, scan_point.end)
                 break
 
         if mid != mod_id:
             continue
 
         n_evts += 1
-        md = maddaq.modules[mid]
+        md = vdaq.modules[mid]
         data = md.process_event(evt)
         if data is not None:
             ng = 0
             for C, E in data:
                 if C == the_chan:
                     ng += 1
 
-                if E > thrs:
+                if E > emin:
                     point_data.append(E)
 
             if ng > 0:
                 good_chan += 1
 
         prg.increase(show=True)
 
@@ -136,23 +144,23 @@
 
 def analyzeMbias(files, options):
     """main entry."""
     ifile = Path(files[0]).expanduser().resolve()
     if not ifile.exists():
         return
 
-    read_mbias_scan(ifile, options.mid, options.thrs, None)
+    read_mbias_scan(ifile, options.mid, options.emin, None)
     plt.show()
 
 
 def do_analyzeMbias():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument('files', nargs='*', help="Input files")
-    parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
+    parser.add_argument("--emin", default=0.0, type=float, help="Min E to show in histogram")
 
     parser.add_argument("--mid", dest="mid", default=11, type=int, help="The slot ID")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/data_utils.py` & `vdaq_soap-1.1.0/vdaq_soap/data_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """Collection of utilities for data."""
 
 import time
-from maddaq import MadDAQData, ShowProgress, GTimer
+from vdaq_ana import VDaqData, GTimer, ShowProgress
 import numpy as np
 from lmfit.models import GaussianModel
 
 
 def fit_gaussian(n, X, center, width=5.0, amplitude=1):
     """Fit a gaussion.
 
@@ -42,19 +42,19 @@
 def open_data_file(ifile):
     """Open a data file."""
     ntry = 10
     while True:
         try:
             if ntry <= 0:
                 print("### Could not open the data file\n {}".format(ifile))
-                maddaq = None
+                vdaq = None
                 break
 
-            maddaq = MadDAQData(ifile)
+            vdaq = VDaqData(ifile)
             break
 
         except Exception:
             print("...Problems opening data file. Waiting for a new try.")
             time.sleep(1.0)
             ntry -= 1
 
-    return maddaq
+    return vdaq
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/soapCheckMadDaq.py` & `vdaq_soap-1.1.0/vdaq_soap/soapCheckAliVATA.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 """Create a run and execute it."""
 
 import sys
 import os
 import json
 import zlib
 import math
+import pathlib
+import time
 from argparse import ArgumentParser
 import numpy as np
 import matplotlib.pyplot as plt
-import pathlib
-import time
 import docx
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 
 try:
     import daqpp.soap
 except ModuleNotFoundError:
     pass
 
-from maddaq import MadDAQData, ShowProgress, GTimer
+from vdaq_ana import GTimer, ShowProgress
 
 from vdaq_soap.data_utils import fit_gaussian, draw_best_fit, open_data_file
 from vdaq_soap.analyzeHoldDelay import read_hold_delay_data
 from vdaq_soap.analyzeMbias import read_mbias_scan
 
 
 def set_module_param(runm, par_name, value):
@@ -38,24 +38,24 @@
     """
     kkk = runm.getModules()
     kkk = kkk.values()
     for md in runm.getModules().values():
         try:
             md.parameters[par_name].set_value(value)
         except IndexError:
-            print("parameter {} does not exist for module {]".format(par_name, md.name))
+            print("parameter {} does not exist for module {}]".format(par_name, md.name))
 
 
-def set_default_parameters(run_manager, hold_delay=175, polarity=0, mbias=600):
+def set_default_parameters(run_manager, hold_delay=200, polarity=0, mbias=600, threshold=50):
     """Set default module parameters."""
     # print("Def. parameters. Setting HD to {} Mbias {}".format(hold_delay, mbias))
-    set_module_param(run_manager, "channel", -1)
+    set_module_param(run_manager, "channel", -9999)
     set_module_param(run_manager, "coincidence", False)
     set_module_param(run_manager, "ro_mode", 4)      # sparse
-    set_module_param(run_manager, "threshold", 70)  # threshold
+    set_module_param(run_manager, "threshold", threshold)  # threshold
     set_module_param(run_manager, "polarity", polarity)
     set_module_param(run_manager, "nadj", 5)
     set_module_param(run_manager, "trg_type", 1)
     set_module_param(run_manager, "hold_delay", hold_delay)
 
     try:
         version = run_manager.getParameter("version")
@@ -265,26 +265,27 @@
 
     # Restore the values
     the_module.parameters['trg_type'].set_value(old_trg_type)
     the_module.parameters['ro_mode'].set_value(old_ro_mode)
     the_module.parameters['coincidence'].set_value(old_coinc)
 
 
-def test_hold_delay_scan(server, the_module, chan, npts=32, first=0, last=255, nsec=1, thrs=-1, document=None):
+def test_hold_delay_scan(server, the_module, chan, npts=32, first=0, last=255, nsec=1, emin=-1, document=None):
     """Make a HoldDelay scan.
 
     Args:
     ----
         server: The SOAP server
         the_module: The module to test
         chan: The channel tto send teh calib pulse to.
         npts: number of points.
         first: First hold_delay value. Defaults to 0.
         last: Last hold_delay value. Defaults to 255.
         nsec: number of seconds per scan point
+        emin (optional): min value to store in histrogram.
         document: the word document
 
     """
     print("\n:> Hold delay scan (chan {}: {}, {}, {}".format(chan, first, last, npts))
 
     # Create a new scan run
     server.createRunManager("scan", "main")
@@ -319,15 +320,15 @@
     time.sleep(0.5)
 
     # restore hold_delay value
     the_module.parameters['hold_delay'].set_value(old_hold_delay)
 
     # read the data
     ofile = pathlib.Path.cwd().joinpath("hold_delay_{}_000.h5".format(the_module.name))
-    hd_max = read_hold_delay_data(ofile, int(the_module.name), thrs=thrs, document=document)
+    hd_max = read_hold_delay_data(ofile, int(the_module.name), emin=emin, document=document)
     return hd_max
 
 
 def test_channel_change(server, the_module, nchan, first_chan, last_chan, nevts=1000, document=None):
     """Make a channel scan.
 
     Args:
@@ -416,24 +417,24 @@
 
         plt.draw()
         plt.pause(0.001)
 
     return run_status
 
 
-def test_TDCs(server, the_module, channel, nsec=5, thrs=0.0, document=None):
+def test_TDCs(server, the_module, channel, nsec=5, emin=0.0, document=None):
     """Test the TDC or clock counter.
 
     Args:
     ----
         server: The soap client
         the_module: the Module
         channel: the channel
         nsec (optional): Acquisition time. Defaults to 5 sec.
-        thrs (optional): min value to store in histrogram.
+        emin (optional): min value to store in histrogram.
         document (optional): The report document. Defaults to None.
 
     """
     # do a channel scan for this
     ofile = pathlib.Path.cwd().joinpath("channel_TDC_{}.h5".format(the_module.name))
     server.createRunManager("data", "main")
     run_manager = daqpp.soap.RunManager("main", server)
@@ -449,29 +450,29 @@
     status = run_manager.getStatus()
     rate = status.rate
 
     # Now we have to read back the data
     ifile = pathlib.Path.cwd().joinpath("channel_TDC_{}_000.h5".format(the_module.name))
 
     print(":> Opening {} for TDC analysis".format(ifile))
-    maddaq = open_data_file(ifile)
+    vdaq = open_data_file(ifile)
 
-    if maddaq is None:
+    if vdaq is None:
         return
 
     last_time = {}
     last_event = {}
     nlost = 0
     mod_id = int(the_module.name)
     values = []
     amplitude = []
 
-    prg = ShowProgress(maddaq.nevts, width=24)
+    prg = ShowProgress(vdaq.nevts, width=24)
     prg.start()
-    for evt in maddaq:
+    for evt in vdaq:
         evt_time = int(evt.time)
         mid = evt.mod_id
         if mid != mod_id:
             continue
 
         ltim = last_time.get(mid, -1)
         if ltim > 0:
@@ -489,19 +490,19 @@
 
         last_event[mid] = evt.evtcnt
         dt = (dt*25.0)/1000.0
         if dt > 0 and dt < 1000:
             values.append(dt)
 
         # The single channel amplitude
-        md = maddaq.modules[mid]
+        md = vdaq.modules[mid]
         data = md.process_event(evt)
         if data is not None:
             for C, E in data:
-                if E > thrs:
+                if E > emin:
                     amplitude.append(E)
 
         prg.increase(show=True)
 
     print("\nNumber of events lost: {}".format(nlost))
     if rate > 0:
         print("Expected rate: {:.2f} Hz. Period {:.6f} us.".format(rate, 1.0e6/rate))
@@ -580,15 +581,15 @@
     wait_for_end_of_run(run_manager, 6)
     print("Done")
 
 
 def test_mbias_scan(server, the_module,
                     nchan, first_chan, last_chan,
                     npts, first, last,
-                    nsec=1, thrs=-1, document=None):
+                    nsec=1, emin=-1, document=None):
     """Make a mbias scan.
 
     Args:
     ----
         server: the SOAP client
         the_module: The module to test
         nchan: number of channels
@@ -597,15 +598,15 @@
         npts: number of mbias points
         first: first mbias value
         last: last mbias value
         nsec: Tiem on each scanpoint. Defaults to 1.
         document (optional): the word document
 
     """
-    print("\n:> mbias scan (chan {} {}-{}: {}, {}, {}".format(nchan, first_chan, last_chan, first, last, npts))
+    print("\n:> mbias scan (chan {} {}-{}, sec {}): mbias from {} to {} npts {}".format(nchan, first_chan, last_chan, nsec, first, last, npts))
 
     # Create a new scan run
     server.createRunManager("scan", "main")
     run_manager = daqpp.soap.RunManager("main", server)
 
     # Reset all monitor data
     the_module.resetMonitorData()
@@ -624,33 +625,39 @@
     if nchan > 1:
         step = math.floor((last_chan-first_chan)/(nchan-1))
         last_chan = first_chan + (nchan-1) * step
     else:
         last_chan = first_chan
 
     # Define the scan
-    run_manager.getParameter("command").set_value(
-        "scan|nevt={}:is_time=true:points=(1,1,0,0);(0,{},{},{});(4,{},{},{})".format(
-            nsec, nchan, first_chan, last_chan, npts, first, last)
-    )
+    if nchan == 1 and first_chan < 0:
+        run_manager.getParameter("command").set_value(
+            "scan|nevt={}:is_time=true:points=(4,{},{},{})".format(
+                nsec, npts, first, last)
+        )
+    else:
+        run_manager.getParameter("command").set_value(
+            "scan|nevt={}:is_time=true:points=(1,1,0,0);(0,{},{},{});(4,{},{},{})".format(
+                nsec, nchan, first_chan, last_chan, npts, first, last)
+        )
 
     # Set the output file name
     ofile = pathlib.Path.cwd().joinpath("mbias_{}.h5".format(the_module.name))
     run_manager.getParameter("command").set_value("logData|file={}".format(ofile))
 
     # start the run
     run_manager.startRun()
     wait_for_end_of_run(run_manager)
 
     # Wait to have data file closed
     time.sleep(0.5)
 
     # read the data
     ofile = pathlib.Path.cwd().joinpath("mbias_{}_000.h5".format(the_module.name))
-    read_mbias_scan(ofile, int(the_module.name), thrs=thrs, document=document)
+    read_mbias_scan(ofile, int(the_module.name), emin=emin, document=document)
 
 
 def restore_default_state(server, options):
     """Restore state and parameters."""
     # BAck to normal Data RunManager.
     server.createRunManager("data", "main")
     run_manager = daqpp.soap.RunManager("main", server)
@@ -702,65 +709,65 @@
             md.setLocal(True, "")
             in_local.append(md)
         else:
             md.setLocal(False, "main")
             the_module = md
 
     if the_module is None:
-        print("### CheckMadDaq Error: module {} not present")
+        print("### CheckAliVATA Error: module {} not present")
         return
 
     # Set some module parameters like adjacent, polarity and threshold.
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     run_manager.GetReady()
 
     # Test the pedestals
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     test_pedestals(server, the_module, save_data=True, document=document)
 
     # Test Ext Trigger
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     test_ext_trigger(server, the_module, nsec=5, document=document)
 
     # Do a channel scan
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     nchan = options.nchip*8
     first_chan = 8
     last_chan = options.nchip*128 - 8
     test_channel_change(server, the_module, nchan, first_chan, last_chan, 5000, document=document)
 
     # test TDCs
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
-    test_TDCs(server, the_module, channel, nsec=5, thrs=options.thrs, document=document)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
+    test_TDCs(server, the_module, channel, nsec=5, emin=options.emin, document=document)
 
     # Do a hold delay scan
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
-    test_hold_delay_scan(server, the_module, channel, 64, 0, 255, nsec=1, thrs=options.thrs, document=document)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
+    test_hold_delay_scan(server, the_module, channel, 64, 0, 255, nsec=1, emin=options.emin, document=document)
 
     # Do a mbias scan
-    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, hold_delay=options.hold_delay, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     test_mbias_scan(server, the_module,
                     1, channel, channel,
                     64, 100, 4096,
-                    nsec=1, thrs=options.thrs, document=document)
+                    nsec=1, emin=options.emin, document=document)
 
     # Now we move back to a data run
     # test_FOR_run(server, 10000)
 
     # Set all settings in the default state
     restore_default_state(server, options)
     document.save(options.out)
 
 
-def soapCheckMadDaq():
+def soapCheckAliVATA():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument("--mid", dest="mid", default="11",
                         type=str, help="The slot ID")
-    parser.add_argument("--out", dest="out", default="maddaq_report.docx",
+    parser.add_argument("--out", dest="out", default="vdaq_report.docx",
                         type=str, help="The output fiel name")
     parser.add_argument("--title", dest="title", default=None,
                         type=str, help="Document title")
     parser.add_argument("--firmware", dest="firmware", default="XX.XX.XX",
                         type=str, help="Firmware")
     parser.add_argument("--host", dest="host", default="localhost",
                         type=str, help="The soap server")
@@ -772,15 +779,17 @@
                         type=float, help="Cal. pulse amplitude")
     parser.add_argument("--mbias", dest="mbias", default=300,
                         type=int, help="Chip Main bias")
     parser.add_argument("--hold_delay", dest="hold_delay", default=175,
                         type=int, help="Chip Hold delay")
     parser.add_argument("--polarity", dest="polarity", default=0,
                         type=int, help="Signal polarity")
-    parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
+    parser.add_argument("--threshold", default=50, type=int, help="GPx threshold")
+    
+    parser.add_argument("--emin", default=0.0, type=float, help="Min E to show in histogram")
     parser.add_argument("--nchip", help="Number of chips", default=1, type=int)
     parser.add_argument("--debug", dest="debug", action="store_true",
                         help="Debug server I/O",
                         default=False)
 
     options = parser.parse_args()
 
@@ -790,8 +799,8 @@
 
     print("\n### All tests done ###")
     plt.ioff()
     # plt.show()
 
 
 if __name__ == "__main__":
-    soapCheckMadDaq()
+    soapCheckAliVATA()
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/soapHoldDelay.py` & `vdaq_soap-1.1.0/vdaq_soap/soapHoldDelay.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 """Do a Hold delay scan."""
 import sys
 from argparse import ArgumentParser
 
 import daqpp.soap
 import matplotlib.pyplot as plt
 
-from vdaq_soap.soapCheckMadDaq import restore_default_state
-from vdaq_soap.soapCheckMadDaq import set_default_parameters
-from vdaq_soap.soapCheckMadDaq import test_hold_delay_scan
+from vdaq_soap.soapCheckAliVATA import restore_default_state
+from vdaq_soap.soapCheckAliVATA import set_default_parameters
+from vdaq_soap.soapCheckAliVATA import test_hold_delay_scan
 
 
 def soapHoldDelay():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument("--host", dest="host", default="localhost",
                         type=str, help="The soap server")
@@ -27,16 +27,17 @@
     parser.add_argument("--hold_delay", dest="hold_delay", default=175,
                         type=int, help="Chip hold delay")
     parser.add_argument("--polarity", dest="polarity", default=0,
                         type=int, help="Signal polarity")
     parser.add_argument("--nsec", dest="nsec", default=10,
                         type=int, help="Chip Main bias")
     parser.add_argument("--step", type=int, help="Scan step", default=4)
-    parser.add_argument("--thrs", default=0.0, type=float,
+    parser.add_argument("--emin", default=0.0, type=float,
                         help="Min E to show in histogram")
+    parser.add_argument("--threshold", default=50, type=int, help="GPx threshold")
     parser.add_argument("--debug", dest="debug", action="store_true",
                         help="Debug server I/O",
                         default=False)
     options = parser.parse_args()
 
     # This is where we connect with the server
     try:
@@ -64,21 +65,21 @@
         else:
             md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
-        print("### CheckMadDaq Error: module {} not present")
+        print("### CheckAliVATA Error: module {} not present")
         sys.exit()
 
     npts = int(256.0/float(options.step))
 
     plt.ion()
-    set_default_parameters(run_manager, polarity=options.polarity, mbias=options.mbias)
+    set_default_parameters(run_manager, polarity=options.polarity, mbias=options.mbias, threshold=options.threshold)
     test_hold_delay_scan(server, the_module, options.channel, npts, 0, 255, nsec=options.nsec)
 
     # Set all settings in the default state
     restore_default_state(server, options)
 
     plt.ioff()
     plt.show()
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/soapMbias.py` & `vdaq_soap-1.1.0/vdaq_soap/soapTestChannel.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 """Do a Hold delay scan."""
 import sys
 from argparse import ArgumentParser
 
 import daqpp.soap
 import matplotlib.pyplot as plt
 
-from vdaq_soap.soapCheckMadDaq import restore_default_state
-from vdaq_soap.soapCheckMadDaq import set_default_parameters
-from vdaq_soap.soapCheckMadDaq import test_mbias_scan
+from vdaq_soap.soapCheckAliVATA import restore_default_state
+from vdaq_soap.soapCheckAliVATA import set_default_parameters
+from vdaq_soap.soapCheckAliVATA import test_TDCs
 
 
-def soapMbias():
+def soapTestChannel():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument("--host", dest="host", default="localhost",
                         type=str, help="The soap server")
     parser.add_argument("--port", dest="port", default=50000,
                         type=int, help="The soap port")
     parser.add_argument("--mid", dest="mid", default="11",
                         type=str, help="The slot ID")
     parser.add_argument("--channel", dest="channel", default=32,
                         type=int, help="The test channel")
-    parser.add_argument("--hold_delay", dest="mbias", default=175,
+    parser.add_argument("--mbias", dest="mbias", default=300,
                         type=int, help="Chip Main bias")
+    parser.add_argument("--hold_delay", dest="hold_delay", default=175,
+                        type=int, help="Chip hold delay")
     parser.add_argument("--polarity", dest="polarity", default=0,
                         type=int, help="Signal polarity")
     parser.add_argument("--nsec", dest="nsec", default=10,
                         type=int, help="Chip Main bias")
-    parser.add_argument("--step", type=int, help="Scan step", default=64)
-    parser.add_argument("--thrs", default=0.0, type=float,
+    parser.add_argument("--emin", default=0.0, type=float,
                         help="Min E to show in histogram")
+    parser.add_argument("--threshold", default=50, type=int, help="GPx threshold")
     parser.add_argument("--debug", dest="debug", action="store_true",
                         help="Debug server I/O",
                         default=False)
     options = parser.parse_args()
 
     # This is where we connect with the server
     try:
@@ -62,28 +64,27 @@
         else:
             md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
-        print("### CheckMadDaq Error: module {} not present")
+        print("### CheckAliVATAq Error: module {} not present")
         sys.exit()
 
-    npts = int((4096-64)/float(options.step))
-
     plt.ion()
-    set_default_parameters(run_manager, polarity=options.polarity, mbias=options.mbias)
-    test_mbias_scan(server, the_module,
-                    1, options.channel, options.channel,
-                    npts, 64, 4096,
-                    nsec=options.nsec, thrs=options.thrs)
+    set_default_parameters(run_manager, 
+                           polarity=options.polarity, 
+                           hold_delay=options.hold_delay,
+                           threshold=options.threshold,
+                           mbias=options.mbias)
+    test_TDCs(server, the_module, channel=options.channel, nsec=options.nsec, emin=options.emin)
 
     # Set all settings in the default state
     restore_default_state(server, options)
 
     plt.ioff()
     plt.show()
 
 
 if __name__ == "__main__":
-    soapMbias()
+    soapTestChannel()
```

### Comparing `vdaq_soap-1.0.9/vdaq_soap/soapTestChannel.py` & `vdaq_soap-1.1.0/vdaq_soap/soapMbias.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,40 +2,44 @@
 """Do a Hold delay scan."""
 import sys
 from argparse import ArgumentParser
 
 import daqpp.soap
 import matplotlib.pyplot as plt
 
-from vdaq_soap.soapCheckMadDaq import restore_default_state
-from vdaq_soap.soapCheckMadDaq import set_default_parameters
-from vdaq_soap.soapCheckMadDaq import test_TDCs
+from vdaq_soap.soapCheckAliVATA import restore_default_state
+from vdaq_soap.soapCheckAliVATA import set_default_parameters
+from vdaq_soap.soapCheckAliVATA import test_mbias_scan
 
 
-def soapTestChannel():
+def soapMbias():
     """Main entry."""
     parser = ArgumentParser()
     parser.add_argument("--host", dest="host", default="localhost",
                         type=str, help="The soap server")
     parser.add_argument("--port", dest="port", default=50000,
                         type=int, help="The soap port")
     parser.add_argument("--mid", dest="mid", default="11",
                         type=str, help="The slot ID")
     parser.add_argument("--channel", dest="channel", default=32,
                         type=int, help="The test channel")
-    parser.add_argument("--mbias", dest="mbias", default=300,
-                        type=int, help="Chip Main bias")
     parser.add_argument("--hold_delay", dest="hold_delay", default=175,
-                        type=int, help="Chip hold delay")
+                        type=int, help="Chip Hold Delay")
+    parser.add_argument("--mbias", dest="mbias", default=600,
+                        type=int, help="Chip Main bias")
     parser.add_argument("--polarity", dest="polarity", default=0,
                         type=int, help="Signal polarity")
     parser.add_argument("--nsec", dest="nsec", default=10,
                         type=int, help="Chip Main bias")
-    parser.add_argument("--thrs", default=0.0, type=float,
+    parser.add_argument("--step", type=int, help="Scan step", default=64)
+    parser.add_argument("--min_val", type=int, help="Minimum value of scan", default=64)
+    parser.add_argument("--max_val", type=int, help="Minimum value of scan", default=4096)
+    parser.add_argument("--emin", default=0.0, type=float,
                         help="Min E to show in histogram")
+    parser.add_argument("--threshold", default=50, type=int, help="GPx threshold")
 
     parser.add_argument("--debug", dest="debug", action="store_true",
                         help="Debug server I/O",
                         default=False)
     options = parser.parse_args()
 
     # This is where we connect with the server
@@ -64,26 +68,28 @@
         else:
             md.setLocal(True, "")
 
     if the_module is None:
         the_module = modules[0]
 
     if the_module is None:
-        print("### CheckMadDaq Error: module {} not present")
+        print("### soapMbias Error: module {} not present")
         sys.exit()
 
+    npts = int((4096-64)/float(options.step))
+
     plt.ion()
-    set_default_parameters(run_manager, 
-                           polarity=options.polarity, 
-                           hold_delay=options.hold_delay, 
-                           mbias=options.mbias)
-    test_TDCs(server, the_module, channel=options.channel, nsec=options.nsec, thrs=options.thrs)
+    set_default_parameters(run_manager, polarity=options.polarity, hold_delay=options.hold_delay, threshold=options.threshold)
+    test_mbias_scan(server, the_module,
+                    1, options.channel, options.channel,
+                    npts, options.min_val, options.max_val,
+                    nsec=options.nsec, emin=options.emin)
 
     # Set all settings in the default state
     restore_default_state(server, options)
 
     plt.ioff()
     plt.show()
 
 
 if __name__ == "__main__":
-    soapTestChannel()
+    soapMbias()
```

