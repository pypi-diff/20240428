# Comparing `tmp/axidence-0.1.0.tar.gz` & `tmp/axidence-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axidence-0.1.0.tar", last modified: Wed Apr 24 15:15:20 2024, max compression
+gzip compressed data, was "axidence-0.2.0.tar", last modified: Sat Apr 27 15:42:10 2024, max compression
```

## Comparing `axidence-0.1.0.tar` & `axidence-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.695610 axidence-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 15:15:13.000000 axidence-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-24 15:15:20.691610 axidence-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 15:15:13.000000 axidence-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/isolated/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/isolated_s1.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/isolated_s2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/pairing/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/paired_events.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/paired_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/salting/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/event_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/event_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/peak_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/salting_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/salting_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 15:15:13.000000 axidence-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 15:15:20.695610 axidence-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_deps_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_exhaust_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_salting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.028913 axidence-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-27 15:42:06.000000 axidence-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-27 15:42:10.028913 axidence-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-27 15:42:06.000000 axidence-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.024913 axidence-0.2.0/axidence/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.024913 axidence-0.2.0/axidence/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.024913 axidence-0.2.0/axidence/plugins/cuts/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/cuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/cuts/cut_event_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/cuts/cut_isolated_s1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/cuts/cut_isolated_s2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/cuts/cut_pairing_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.024913 axidence-0.2.0/axidence/plugins/isolated/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/isolated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/isolated/isolated_s1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/isolated/isolated_s2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.028913 axidence-0.2.0/axidence/plugins/pairing/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/pairing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/pairing/events_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19628 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/pairing/peaks_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.028913 axidence-0.2.0/axidence/plugins/salting/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/event_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/event_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/events_salting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/peak_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/plugins/salting/peaks_salted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-27 15:42:06.000000 axidence-0.2.0/axidence/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.028913 axidence-0.2.0/axidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-27 15:42:10.000000 axidence-0.2.0/axidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-27 15:42:10.000000 axidence-0.2.0/axidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:42:10.000000 axidence-0.2.0/axidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 15:42:10.000000 axidence-0.2.0/axidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 15:42:10.000000 axidence-0.2.0/axidence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 15:42:06.000000 axidence-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 15:42:10.028913 axidence-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:42:10.028913 axidence-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-27 15:42:06.000000 axidence-0.2.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-27 15:42:06.000000 axidence-0.2.0/tests/test_exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-27 15:42:06.000000 axidence-0.2.0/tests/test_salting.py
```

### Comparing `axidence-0.1.0/LICENSE` & `axidence-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axidence-0.1.0/PKG-INFO` & `axidence-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.1.0
+Version: 0.2.0
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Author-email: Dacheng Xu <dx2227@columbia.edu>
 Maintainer-email: Dacheng Xu <dx2227@columbia.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, axidence contributors.
         All rights reserved.
```

### Comparing `axidence-0.1.0/README.md` & `axidence-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `axidence-0.1.0/axidence/plugins/salting/event_building.py` & `axidence-0.2.0/axidence/plugins/salting/events_salting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,178 +1,233 @@
 from typing import Tuple
 import numpy as np
-from tqdm import tqdm
 import strax
 import straxen
-from straxen import Events, EventBasics
+from straxen import units, EventBasics, EventPositions
 
-from ...utils import needed_dtype, merge_salting_real
-from axidence.plugin import ExhaustPlugin
+from ...utils import copy_dtype
+from ...plugin import RunMetaPlugin
 
 
-class SaltedEvents(Events, ExhaustPlugin):
+class EventsSalting(EventPositions, EventBasics, RunMetaPlugin):
     __version__ = "0.0.0"
-    depends_on = ("salting_peaks", "salting_peak_proximity", "peak_basics", "peak_proximity")
-    provides = "events"
-    data_kind = "events"
+    depends_on: Tuple = tuple()
+    provides = "events_salting"
+    data_kind = "events_salting"
     save_when = strax.SaveWhen.EXPLICIT
 
-    n_drift_time_window = straxen.URLConfig(
-        default=5,
-        type=int,
-        track=True,
-        help="How many max drift time will the event builder extend",
+    salting_seed = straxen.URLConfig(
+        default=None,
+        type=(int, None),
+        help="Seed for salting",
     )
 
-    disable_tqdm = straxen.URLConfig(
-        default=True,
-        type=bool,
-        track=False,
-        help="Whether to disable tqdm",
+    salting_rate = straxen.URLConfig(
+        default=10,
+        type=(int, float),
+        help="Rate of salting in Hz",
     )
 
-    def __init__(self):
-        super().__init__()
-        self.dtype = super().dtype + [
-            (("Salting number of events", "salt_number"), np.int64),
-            (("Whether the salting event can trigger", "is_triggering"), bool),
-        ]
-
-    def setup(self):
-        super().setup()
-        self.needed_fields, self._peaks_dtype = needed_dtype(
-            self.deps, self.dependencies_by_kind, set.intersection
-        )
+    real_run_start = straxen.URLConfig(
+        default=None,
+        type=(int, None),
+        help="Real start time of run [ns]",
+    )
 
-        self.window = self.n_drift_time_window * self.drift_time_max
+    real_run_end = straxen.URLConfig(
+        default=None,
+        type=(int, None),
+        help="Real start time of run [ns]",
+    )
 
-        if self.window < self.left_extension + self.right_extension:
-            raise ValueError(
-                f"The window {self.window}ns is too small to extend the event "
-                f"while the gap_threshold is about {self.left_extension + self.right_extension}!"
-            )
+    strict_real_run_time_check = straxen.URLConfig(
+        default=True,
+        type=bool,
+        help="Whether to strictly check the real run time is provided",
+    )
 
-    def get_window_size(self):
-        return max(super().get_window_size(), self.window * 10)
+    s1_area_range = straxen.URLConfig(
+        default=(1, 150),
+        type=(list, tuple),
+        help="Range of S1 area",
+    )
 
-    def compute(self, salting_peaks, peaks, start, end):
-        if salting_peaks["salt_number"][0] != 0:
-            raise ValueError(
-                "Expected salt_number to start from 0 because "
-                f"{self.__class__.__name__} is a ExhaustPlugin plugin!"
-            )
+    s2_area_range = straxen.URLConfig(
+        default=(1e2, 2e4),
+        type=(list, tuple),
+        help="Range of S2 area",
+    )
 
-        _peaks = merge_salting_real(salting_peaks, peaks, self._peaks_dtype)
+    s1_distribution = straxen.URLConfig(
+        default="",
+        type=str,
+        help="S1 distribution shape",
+    )
 
-        # use S2s as anchors
-        anchor_peaks = salting_peaks[1::2]
-        windows = strax.touching_windows(_peaks, anchor_peaks, window=self.window)
-
-        n_events = len(salting_peaks) // 2
-        if np.unique(salting_peaks["salt_number"]).size != n_events:
-            raise ValueError("Expected salt_number to be half of the input peaks number!")
-
-        _is_triggering = self._is_triggering(anchor_peaks)
-
-        # check if the salting event can trigger
-        # for now, only S2 can trigger
-        if not self.exclude_s1_as_triggering_peaks:
-            raise NotImplementedError("Only S2 can trigger for now!")
-        result = np.empty(n_events, self.dtype)
-        if np.unique(anchor_peaks["type"]).size != 1:
-            raise ValueError("Expected only one type of anchor peaks!")
-
-        # prepare for an empty event
-        empty_event = np.empty(1, dtype=self.dtype)
-        EventBasics.set_nan_defaults(empty_event)
-
-        # iterate through all anchor peaks
-        _result = []
-        for i in tqdm(range(n_events), disable=self.disable_tqdm):
-            left_i, right_i = windows[i]
-            _events = super().compute(_peaks[left_i:right_i], start, end)
-            _events = strax.split_touching_windows(_events, anchor_peaks[i : i + 1])
-            if _is_triggering[i]:
-                if len(_events) != 1 or len(_events[0]) != 1:
-                    raise ValueError(f"Expected 1 event, got {_events}!")
-                _result.append(_events[0])
-            else:
-                empty_event["time"] = anchor_peaks["time"][i]
-                empty_event["endtime"] = anchor_peaks["endtime"][i]
-                _result.append(empty_event.copy())
-        _result = np.hstack(_result)
-
-        for n in _result.dtype.names:
-            result[n] = _result[n]
-
-        # assign the most important parameters
-        result["is_triggering"] = _is_triggering
-        result["salt_number"] = salting_peaks["salt_number"][::2]
-        result["event_number"] = salting_peaks["salt_number"][::2]
-
-        if np.any(np.diff(result["time"]) < 0):
-            raise ValueError("Expected time to be sorted!")
-        return result
+    s2_distribution = straxen.URLConfig(
+        default="",
+        type=str,
+        help="S2 distribution shape",
+    )
 
+    veto_length_run_start = straxen.URLConfig(
+        default=10**9,
+        type=int,
+        help="Min time delay in [ns] for events towards the run start boundary",
+    )
 
-class SaltedEventBasics(EventBasics, ExhaustPlugin):
-    __version__ = "0.0.0"
-    depends_on: Tuple[str, ...] = (
-        "events",
-        "salting_peaks",
-        "salting_peak_proximity",
-        "peak_basics",
-        "peak_proximity",
-        "peak_positions",
+    veto_length_run_end = straxen.URLConfig(
+        default=10**8,
+        type=int,
+        help="Min time delay in [ns] for events towards the run end boundary",
     )
-    provides = "event_basics"
-    data_kind = "events"
-    save_when = strax.SaveWhen.EXPLICIT
 
-    def infer_dtype(self):
-        dtype = super().infer_dtype()
-        dtype += [
-            (("Salting number of main S1", "s1_salt_number"), np.int64),
-            (("Salting number of main S2", "s2_salt_number"), np.int64),
-            (("Salting number of alternative S1", "alt_s1_salt_number"), np.int64),
-            (("Salting number of alternative S2", "alt_s2_salt_number"), np.int64),
-            (("Salting number of events", "salt_number"), np.int64),
-            (("Whether the salting event can trigger", "is_triggering"), bool),
-        ]
-        return dtype
+    s1_n_hits_tight_coincidence = straxen.URLConfig(
+        default=2,
+        type=int,
+        help="Will assign the events's ``s1_n_hits`` and ``s1_tight_coincidence`` by this",
+    )
 
-    def setup(self):
-        super().setup()
+    n_drift_time_window = straxen.URLConfig(
+        default=5,
+        type=int,
+        help="How many max drift time will the event builder extend",
+    )
 
-        self.needed_fields, self._peaks_dtype = needed_dtype(
-            self.deps, self.dependencies_by_kind, set.union
+    def _set_posrec_save(self):
+        self.posrec_save = []
+        self.pos_rec_labels = []
+
+    def refer_dtype(self):
+        return strax.merged_dtype(
+            [
+                strax.to_numpy_dtype(super(EventPositions, self).infer_dtype()),
+                strax.to_numpy_dtype(super(EventsSalting, self).infer_dtype()),
+            ]
         )
 
-        self.peak_properties = tuple(
-            list(self.peak_properties) + [("salt_number", np.int64, "Salting number of peaks")]
-        )
+    def infer_dtype(self):
+        dtype_reference = self.refer_dtype()
+        required_names = ["time", "endtime", "s1_center_time", "s2_center_time"]
+        required_names += ["s1_area", "s2_area", "s1_n_hits", "s1_tight_coincidence"]
+        required_names += ["x", "y", "z", "drift_time", "s2_x", "s2_y", "z_naive"]
+        dtype = copy_dtype(dtype_reference, required_names)
+        # since event_number is int64 in event_basics
+        dtype += [(("Salting number of events", "salt_number"), np.int64)]
+        return dtype
 
-    def compute(self, events, salting_peaks, peaks):
-        if salting_peaks["salt_number"][0] != 0:
-            raise ValueError(
-                "Expected salt_number to start from 0 because "
-                f"{self.__class__.__name__} is a ExhaustPlugin plugin!"
+    def init_rng(self):
+        if self.salting_seed is None:
+            self.rng = np.random.default_rng(seed=int(self.run_id))
+        else:
+            self.rng = np.random.default_rng(seed=self.salting_seed)
+
+    def sample_time(self):
+        """Sample the time according to the start and end of the run."""
+        self.event_time_interval = units.s // self.salting_rate
+
+        if units.s / self.salting_rate < self.drift_time_max * self.n_drift_time_window * 2:
+            raise ValueError("Salting rate is too high according the drift time window!")
+
+        time = np.arange(
+            self.run_start + self.veto_length_run_start,
+            self.run_end - self.veto_length_run_end,
+            self.event_time_interval,
+        ).astype(np.int64)
+        self.time_left = self.event_time_interval // 2
+        self.time_right = self.event_time_interval - self.time_left
+        return time
+
+    def inverse_field_distortion(self, x, y, z):
+        # TODO: implement detailed inverse field distortion
+        return x, y, z
+
+    def set_chunk_splitting(self):
+        """Split the rujn into chunks to prevent oversize chunk."""
+        self.max_n_events_in_chunk = round(
+            self.chunk_target_size_mb * 1e6 / self.dtype.itemsize * 0.9
+        )
+        slices_idx = np.unique(
+            np.append(
+                np.arange(self.n_events, dtype=int)[:: self.max_n_events_in_chunk], self.n_events
             )
+        )
+        self.slices = np.vstack([slices_idx[:-1], slices_idx[1:]]).T.astype(int).tolist()
 
-        _peaks = merge_salting_real(salting_peaks, peaks, self._peaks_dtype)
-
-        result = np.zeros(len(events), dtype=self.dtype)
-        self.set_nan_defaults(result)
+        self.time_left = self.event_time_interval // 2
+        self.time_right = self.event_time_interval - self.time_left
 
-        split_peaks = strax.split_by_containment(_peaks, events)
+    def setup(self):
+        """Sample the features of events."""
+        super(EventPositions, self).setup()
+        super(EventsSalting, self).setup()
+
+        self.init_rng()
+        self.init_run_meta()
+
+        time = self.sample_time()
+        self.n_events = len(time)
+        self.events_salting = np.empty(self.n_events, dtype=self.dtype)
+        self.events_salting["salt_number"] = np.arange(self.n_events)
+        self.events_salting["time"] = time
+        self.events_salting["endtime"] = time
+
+        self.events_salting["s1_n_hits"] = self.s1_n_hits_tight_coincidence
+        self.events_salting["s1_tight_coincidence"] = self.s1_n_hits_tight_coincidence
+
+        theta = self.rng.random(size=self.n_events) * 2 * np.pi - np.pi
+        r = np.sqrt(self.rng.random(size=self.n_events)) * straxen.tpc_r
+        self.events_salting["x"] = np.cos(theta) * r
+        self.events_salting["y"] = np.sin(theta) * r
+        self.events_salting["z"] = -self.rng.random(size=self.n_events) * straxen.tpc_z
+        s2_x, s2_y, z_naive = self.inverse_field_distortion(
+            self.events_salting["x"],
+            self.events_salting["y"],
+            self.events_salting["z"],
+        )
+        self.events_salting["s2_x"] = s2_x
+        self.events_salting["s2_y"] = s2_y
+        self.events_salting["z_naive"] = z_naive
+        self.events_salting["drift_time"] = (
+            self.electron_drift_velocity * self.electron_drift_time_gate
+            - self.events_salting["z_naive"]
+        ) / self.electron_drift_velocity
+
+        self.events_salting["s1_center_time"] = time - self.events_salting["drift_time"]
+        self.events_salting["s2_center_time"] = time
+
+        s1_area_range = (float(self.s1_area_range[0]), float(self.s1_area_range[1]))
+        s2_area_range = (float(self.s2_area_range[0]), float(self.s2_area_range[1]))
+        self.events_salting["s1_area"] = np.exp(
+            self.rng.uniform(np.log(s1_area_range[0]), np.log(s1_area_range[1]), size=self.n_events)
+        )
+        self.events_salting["s1_area"] = np.clip(self.events_salting["s1_area"], *s1_area_range)
+        self.events_salting["s2_area"] = np.exp(
+            self.rng.uniform(np.log(s2_area_range[0]), np.log(s2_area_range[1]), size=self.n_events)
+        )
+        self.events_salting["s2_area"] = np.clip(self.events_salting["s2_area"], *s2_area_range)
 
-        result["time"] = events["time"]
-        result["endtime"] = events["endtime"]
-        result["salt_number"] = events["salt_number"]
-        result["event_number"] = events["event_number"]
+        self.set_chunk_splitting()
 
-        self.fill_events(result, events, split_peaks)
-        result["is_triggering"] = events["is_triggering"]
+    def compute(self, chunk_i):
+        """Copy and assign the salting events into chunk."""
+        indices = self.slices[chunk_i]
+
+        if chunk_i == 0:
+            start = self.run_start
+        else:
+            start = self.events_salting["time"][indices[0]] - self.time_left
+
+        if chunk_i == len(self.slices) - 1:
+            end = self.run_end
+        else:
+            end = self.events_salting["time"][indices[1] - 1] + self.time_right
+        return self.chunk(start=start, end=end, data=self.events_salting[indices[0] : indices[1]])
+
+    def is_ready(self, chunk_i):
+        if chunk_i < len(self.slices):
+            return True
+        else:
+            return False
 
-        if np.all(result["s1_salt_number"] < 0) or np.all(result["s2_salt_number"] < 0):
-            raise ValueError("Found zero triggered salting peaks!")
-        return result
+    def source_finished(self):
+        return True
```

### Comparing `axidence-0.1.0/axidence/plugins/salting/peak_correlation.py` & `axidence-0.2.0/axidence/plugins/salting/peak_correlation.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,118 +2,118 @@
 import numpy as np
 import strax
 from straxen import PeakProximity, PeakShadow, PeakAmbience, PeakSEDensity
 
 from ...utils import copy_dtype
 
 
-class SaltingPeakProximity(PeakProximity):
+class PeakProximitySalted(PeakProximity):
     __version__ = "0.0.0"
-    depends_on = ("salting_peaks", "peak_basics")
-    provides = "salting_peak_proximity"
-    data_kind = "salting_peaks"
+    depends_on = ("peaks_salted", "peak_basics")
+    provides = "peak_proximity_salted"
+    data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def refer_dtype(self):
-        return strax.merged_dtype([strax.to_numpy_dtype(super(SaltingPeakProximity, self).dtype)])
+        return strax.unpack_dtype(strax.to_numpy_dtype(super(PeakProximitySalted, self).dtype))
 
     def infer_dtype(self):
         dtype_reference = self.refer_dtype()
         required_names = ["time", "endtime", "n_competing", "n_competing_left"]
         dtype = copy_dtype(dtype_reference, required_names)
         # since event_number is int64 in event_basics
         dtype += [
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
         return dtype
 
-    def compute(self, salting_peaks, peaks):
-        windows = strax.touching_windows(peaks, salting_peaks, window=self.nearby_window)
+    def compute(self, peaks_salted, peaks):
+        windows = strax.touching_windows(peaks, peaks_salted, window=self.nearby_window)
         n_left, n_tot = self.find_n_competing(
-            peaks, salting_peaks, windows, fraction=self.min_area_fraction
+            peaks, peaks_salted, windows, fraction=self.min_area_fraction
         )
         return dict(
-            time=salting_peaks["time"],
-            endtime=strax.endtime(salting_peaks),
+            time=peaks_salted["time"],
+            endtime=strax.endtime(peaks_salted),
             n_competing=n_tot,
             n_competing_left=n_left,
-            salt_number=salting_peaks["salt_number"],
+            salt_number=peaks_salted["salt_number"],
         )
 
     @staticmethod
     @numba.jit(nopython=True, nogil=True, cache=True)
-    def find_n_competing(peaks, salting_peaks, windows, fraction):
-        n_left = np.zeros(len(salting_peaks), dtype=np.int32)
+    def find_n_competing(peaks, peaks_salted, windows, fraction):
+        n_left = np.zeros(len(peaks_salted), dtype=np.int32)
         n_tot = n_left.copy()
         areas = peaks["area"]
-        salting_areas = salting_peaks["area"]
+        areas_salted = peaks_salted["area"]
 
-        dig = np.searchsorted(peaks["center_time"], salting_peaks["center_time"])
+        dig = np.searchsorted(peaks["center_time"], peaks_salted["center_time"])
 
-        for i, peak in enumerate(salting_peaks):
+        for i, peak in enumerate(peaks_salted):
             left_i, right_i = windows[i]
-            threshold = salting_areas[i] * fraction
+            threshold = areas_salted[i] * fraction
             n_left[i] = np.sum(areas[left_i : dig[i]] > threshold)
             n_tot[i] = n_left[i] + np.sum(areas[dig[i] : right_i] > threshold)
 
         return n_left, n_tot
 
 
-class SaltingPeakShadow(PeakShadow):
+class PeakShadowSalted(PeakShadow):
     __version__ = "0.0.0"
-    depends_on = ("salting_peaks", "peak_basics", "peak_positions")
-    provides = "salting_peak_shadow"
-    data_kind = "salting_peaks"
+    depends_on = ("peaks_salted", "peak_basics", "peak_positions")
+    provides = "peak_shadow_salted"
+    data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
         dtype += [
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
         return dtype
 
-    def compute(self, salting_peaks, peaks):
-        result = self.compute_shadow(peaks, salting_peaks)
-        result["salt_number"] = salting_peaks["salt_number"]
+    def compute(self, peaks_salted, peaks):
+        result = self.compute_shadow(peaks, peaks_salted)
+        result["salt_number"] = peaks_salted["salt_number"]
         return result
 
 
-class SaltingPeakAmbience(PeakAmbience):
+class PeakAmbienceSalted(PeakAmbience):
     __version__ = "0.0.0"
-    depends_on = ("salting_peaks", "lone_hits", "peak_basics", "peak_positions")
-    provides = "salting_peak_ambience"
-    data_kind = "salting_peaks"
+    depends_on = ("peaks_salted", "lone_hits", "peak_basics", "peak_positions")
+    provides = "peak_ambience_salted"
+    data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
         dtype += [
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
         return dtype
 
-    def compute(self, salting_peaks, lone_hits, peaks):
-        result = self.compute_ambience(lone_hits, peaks, salting_peaks)
-        result["salt_number"] = salting_peaks["salt_number"]
+    def compute(self, peaks_salted, lone_hits, peaks):
+        result = self.compute_ambience(lone_hits, peaks, peaks_salted)
+        result["salt_number"] = peaks_salted["salt_number"]
         return result
 
 
-class SaltingPeakSEDensity(PeakSEDensity):
+class PeakSEDensitySalted(PeakSEDensity):
     __version__ = "0.0.0"
-    depends_on = ("salting_peaks", "peak_basics", "peak_positions")
-    provides = "salting_peak_se_density"
-    data_kind = "salting_peaks"
+    depends_on = ("peaks_salted", "peak_basics", "peak_positions")
+    provides = "peak_se_density_salted"
+    data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
         dtype += [
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
         return dtype
 
-    def compute(self, salting_peaks, peaks):
-        se_density = self.compute_se_density(peaks, salting_peaks)
+    def compute(self, peaks_salted, peaks):
+        se_density = self.compute_se_density(peaks, peaks_salted)
         return dict(
-            time=salting_peaks["time"], endtime=strax.endtime(salting_peaks), se_density=se_density
+            time=peaks_salted["time"], endtime=strax.endtime(peaks_salted), se_density=se_density
         )
```

### Comparing `axidence-0.1.0/axidence/utils.py` & `axidence-0.2.0/axidence/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,49 @@
     Args:
         dtype_reference (list): dtype reference to copy from
         required_names (list or tuple): names to copy
 
     Returns:
         list: copied dtype
     """
+    if not isinstance(required_names, (set, list, tuple)):
+        raise ValueError(
+            "required_names must be set, list or tuple, "
+            f"not {type(required_names)}, got {required_names}!"
+        )
+    if not isinstance(dtype_reference, list):
+        raise ValueError(
+            f"dtype_reference must be list, not {type(dtype_reference)}, got {dtype_reference}!"
+        )
     dtype = []
     for n in required_names:
         for x in dtype_reference:
             found = False
             if (x[0][1] == n) and (not found):
                 dtype.append(x)
                 found = True
                 break
         if not found:
-            raise ValueError(f"Could not find {n} in dtype_reference!")
+            raise ValueError(f"Could not find {n} in {dtype_reference}!")
     return dtype
 
 
 def needed_dtype(deps, dependencies_by_kind, func):
     # intersection depends_on's dtype.names will be needed in event building
     needed_fields = func(
         *tuple(
             set.union(*tuple(set(deps[d].dtype_for(d).names) for d in dk))
-            for dk in dependencies_by_kind().values()
+            for dk in dependencies_by_kind
         )
     )
     dtype_reference = list(
         func(
             *tuple(
                 set.union(*tuple(set(deps[d].dtype_for(d).descr) for d in dk))
-                for dk in dependencies_by_kind().values()
+                for dk in dependencies_by_kind
             )
         )
     )
     _peaks_dtype = copy_dtype(dtype_reference, needed_fields)
     if len(_peaks_dtype) != len(needed_fields):
         raise ValueError(
             f"Weird! Could not find all needed fields {needed_fields} in {dtype_reference}!"
@@ -55,16 +64,16 @@
         if np.issubdtype(peaks_dtype[field], np.integer):
             _field = np.full(len(peaks), -1)
         else:
             _field = np.full(len(peaks), np.nan)
     return _field
 
 
-def merge_salting_real(salting_peaks, real_peaks, peaks_dtype):
-    # combine salting_peaks and peaks
-    _peaks = np.empty(len(salting_peaks) + len(real_peaks), dtype=peaks_dtype)
+def merge_salted_real(peaks_salted, real_peaks, peaks_dtype):
+    # combine peaks_salted and peaks
+    _peaks = np.empty(len(peaks_salted) + len(real_peaks), dtype=peaks_dtype)
     for n in _peaks.dtype.names:
         _peaks[n] = np.hstack(
-            [_pick_fields(n, salting_peaks, peaks_dtype), _pick_fields(n, real_peaks, peaks_dtype)]
+            [_pick_fields(n, peaks_salted, peaks_dtype), _pick_fields(n, real_peaks, peaks_dtype)]
         )
     _peaks = np.sort(_peaks, order="time")
     return _peaks
```

### Comparing `axidence-0.1.0/axidence.egg-info/PKG-INFO` & `axidence-0.2.0/axidence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.1.0
+Version: 0.2.0
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Author-email: Dacheng Xu <dx2227@columbia.edu>
 Maintainer-email: Dacheng Xu <dx2227@columbia.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, axidence contributors.
         All rights reserved.
```

### Comparing `axidence-0.1.0/axidence.egg-info/SOURCES.txt` & `axidence-0.2.0/axidence.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 axidence/utils.py
 axidence.egg-info/PKG-INFO
 axidence.egg-info/SOURCES.txt
 axidence.egg-info/dependency_links.txt
 axidence.egg-info/requires.txt
 axidence.egg-info/top_level.txt
 axidence/plugins/__init__.py
+axidence/plugins/cuts/__init__.py
+axidence/plugins/cuts/cut_event_building.py
+axidence/plugins/cuts/cut_isolated_s1.py
+axidence/plugins/cuts/cut_isolated_s2.py
+axidence/plugins/cuts/cut_pairing_exists.py
 axidence/plugins/isolated/__init__.py
 axidence/plugins/isolated/isolated_s1.py
 axidence/plugins/isolated/isolated_s2.py
 axidence/plugins/pairing/__init__.py
-axidence/plugins/pairing/paired_events.py
-axidence/plugins/pairing/paired_peaks.py
+axidence/plugins/pairing/events_paired.py
+axidence/plugins/pairing/peaks_paired.py
 axidence/plugins/salting/__init__.py
 axidence/plugins/salting/event_building.py
 axidence/plugins/salting/event_fields.py
+axidence/plugins/salting/events_salting.py
 axidence/plugins/salting/peak_correlation.py
-axidence/plugins/salting/salting_events.py
-axidence/plugins/salting/salting_peaks.py
-tests/test_deps_tree.py
+axidence/plugins/salting/peaks_salted.py
+tests/test_context.py
 tests/test_exhaust_plugin.py
 tests/test_salting.py
```

### Comparing `axidence-0.1.0/pyproject.toml` & `axidence-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axidence"
-version = "0.1.0"
+version = "0.2.0"
 description = "strax-based data-driven accidental coincidence background simulation and peak-level salting"
 readme = "README.md"
 license.file = "LICENSE"
 authors = [
   { name = "Dacheng Xu", email = "dx2227@columbia.edu" },
 ]
 maintainers = [
```

### Comparing `axidence-0.1.0/tests/test_exhaust_plugin.py` & `axidence-0.2.0/tests/test_exhaust_plugin.py`

 * *Files identical despite different names*

### Comparing `axidence-0.1.0/tests/test_salting.py` & `axidence-0.2.0/tests/test_salting.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def setUpClass(cls) -> None:
         # Maybe keeping one temp dir is a bit overkill
         temp_folder = uuid.uuid4().hex
         cls.tempdir = os.path.join(tempfile.gettempdir(), temp_folder)
         assert not os.path.exists(cls.tempdir)
 
         cls.run_id = "0" * 6
-        cls.st = axidence.unsalted_context(output_folder=cls.tempdir)
+        cls.st = axidence.ordinary_context(output_folder=cls.tempdir)
         cls.st.salt_to_context()
 
         cls.st.set_config(
             {
                 "real_run_start": 0,
                 "real_run_end": units.s * 10,
             }
@@ -30,10 +30,10 @@
     @classmethod
     def tearDownClass(cls):
         # Make sure to only cleanup this dir after we have done all the tests
         if os.path.exists(cls.tempdir):
             shutil.rmtree(cls.tempdir)
 
     # def test_salting(self):
-    #     """Test the computing of salting_events and salting_peaks."""
-    #     self.st.make(self.run_id, "salting_events", save="salting_events")
-    #     self.st.make(self.run_id, "salting_peaks", save="salting_peaks")
+    #     """Test the computing of events_salting and peaks_salted."""
+    #     self.st.make(self.run_id, "events_salting", save="events_salting")
+    #     self.st.make(self.run_id, "peaks_salted", save="peaks_salted")
```

