# Comparing `tmp/npc-stim-0.1.6.tar.gz` & `tmp/npc_stim-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc-stim-0.1.6.tar", last modified: Wed Mar 20 18:48:51 2024, max compression
+gzip compressed data, was "npc_stim-0.1.7.tar", last modified: Sat Apr 27 18:56:56 2024, max compression
```

## Comparing `npc-stim-0.1.6.tar` & `npc_stim-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:51.148310 npc-stim-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-20 18:48:22.000000 npc-stim-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-20 18:48:51.148310 npc-stim-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-20 18:48:22.000000 npc-stim-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-20 18:48:48.000000 npc-stim-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:48:51.148310 npc-stim-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:51.144310 npc-stim-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:51.148310 npc-stim-0.1.6/src/npc_stim/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-20 18:48:22.000000 npc-stim-0.1.6/src/npc_stim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:22.000000 npc-stim-0.1.6/src/npc_stim/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-20 18:48:22.000000 npc-stim-0.1.6/src/npc_stim/running.py
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-03-20 18:48:22.000000 npc-stim-0.1.6/src/npc_stim/stim.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-20 18:48:22.000000 npc-stim-0.1.6/src/npc_stim/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:51.148310 npc-stim-0.1.6/src/npc_stim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-20 18:48:51.000000 npc-stim-0.1.6/src/npc_stim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-20 18:48:51.000000 npc-stim-0.1.6/src/npc_stim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:48:51.000000 npc-stim-0.1.6/src/npc_stim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-20 18:48:51.000000 npc-stim-0.1.6/src/npc_stim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 18:48:51.000000 npc-stim-0.1.6/src/npc_stim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:51.148310 npc-stim-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-20 18:48:22.000000 npc-stim-0.1.6/tests/test_core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:56:56.862512 npc_stim-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2024-02-01 20:36:32.000000 npc_stim-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2154 2024-04-27 18:56:56.860513 npc_stim-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2024-02-01 21:15:50.000000 npc_stim-0.1.7/README.md
+-rw-rw-rw-   0        0        0     4508 2024-04-27 18:56:45.000000 npc_stim-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 18:56:56.862512 npc_stim-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 18:56:56.764942 npc_stim-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 18:56:56.816215 npc_stim-0.1.7/src/npc_stim/
+-rw-rw-rw-   0        0        0     1062 2024-04-26 18:01:23.000000 npc_stim-0.1.7/src/npc_stim/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-01 20:36:32.000000 npc_stim-0.1.7/src/npc_stim/py.typed
+-rw-rw-rw-   0        0        0     5741 2024-04-27 18:56:25.000000 npc_stim-0.1.7/src/npc_stim/running.py
+-rw-rw-rw-   0        0        0    19096 2024-04-26 18:01:23.000000 npc_stim-0.1.7/src/npc_stim/stim.py
+-rw-rw-rw-   0        0        0      349 2024-04-26 18:01:23.000000 npc_stim-0.1.7/src/npc_stim/types.py
+drwxrwxrwx   0        0        0        0 2024-04-27 18:56:56.858512 npc_stim-0.1.7/src/npc_stim.egg-info/
+-rw-rw-rw-   0        0        0     2154 2024-04-27 18:56:56.000000 npc_stim-0.1.7/src/npc_stim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-04-27 18:56:56.000000 npc_stim-0.1.7/src/npc_stim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 18:56:56.000000 npc_stim-0.1.7/src/npc_stim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-27 18:56:56.000000 npc_stim-0.1.7/src/npc_stim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 18:56:56.000000 npc_stim-0.1.7/src/npc_stim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 18:56:56.855513 npc_stim-0.1.7/tests/
+-rw-rw-rw-   0        0        0       54 2024-02-01 20:36:32.000000 npc_stim-0.1.7/tests/test_core.py
```

### Comparing `npc-stim-0.1.6/LICENSE` & `npc_stim-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `npc-stim-0.1.6/PKG-INFO` & `npc_stim-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1
-Name: npc-stim
-Version: 0.1.6
-Summary: Tools for accessing and processing stim data, compatible with data in the cloud.
-Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
-License: MIT
-Project-URL: Repository, https://github.com/AllenInstitute/npc_stim
-Project-URL: Issues, https://github.com/AllenInstitute/npc_stim/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: npc-sync>=0.1.3
-Requires-Dist: npc_io>=0.1.26
-Requires-Dist: npc-session>=0.1.33
-Requires-Dist: scipy>=1.12.0
-
-# npc_stim
-
-Tools for accessing and processing stim data, compatible with data in the cloud.
-
-[![PyPI](https://img.shields.io/pypi/v/npc_stim.svg?label=PyPI&color=blue)](https://pypi.org/project/npc_stim/)
-[![Python version](https://img.shields.io/pypi/pyversions/npc_stim)](https://pypi.org/project/npc_stim/)
-
-[![Coverage](https://img.shields.io/codecov/c/github/AllenInstitute/npc_stim?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_stim)
-[![CI/CD](https://img.shields.io/github/actions/workflow/status/AllenInstitute/npc_stim/publish.yml?label=CI/CD&logo=github)](https://github.com/AllenInstitute/npc_stim/actions/workflows/publish.yml)
-[![GitHub issues](https://img.shields.io/github/issues/AllenInstitute/npc_stim?logo=github)](https://github.com/AllenInstitute/npc_stim/issues)
-
-# Usage
-```bash
-conda create -n npc_stim python>=3.9
-conda activate npc_stim
-pip install npc_stim
-```
-
-## Python
-```python
->>> import npc_stim
-```
-
-# Development
-See instructions in https://github.com/AllenInstitute/npc_stim/CONTRIBUTING.md and the original template: https://github.com/AllenInstitute/copier-pdm-npc/blob/main/README.md
+Metadata-Version: 2.1
+Name: npc-stim
+Version: 0.1.7
+Summary: Tools for accessing and processing stim data, compatible with data in the cloud.
+Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
+License: MIT
+Project-URL: Repository, https://github.com/AllenInstitute/npc_stim
+Project-URL: Issues, https://github.com/AllenInstitute/npc_stim/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: npc-sync>=0.1.3
+Requires-Dist: npc_io>=0.1.26
+Requires-Dist: npc-session>=0.1.33
+Requires-Dist: scipy>=1.12.0
+
+# npc_stim
+
+Tools for accessing and processing stim data, compatible with data in the cloud.
+
+[![PyPI](https://img.shields.io/pypi/v/npc_stim.svg?label=PyPI&color=blue)](https://pypi.org/project/npc_stim/)
+[![Python version](https://img.shields.io/pypi/pyversions/npc_stim)](https://pypi.org/project/npc_stim/)
+
+[![Coverage](https://img.shields.io/codecov/c/github/AllenInstitute/npc_stim?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_stim)
+[![CI/CD](https://img.shields.io/github/actions/workflow/status/AllenInstitute/npc_stim/publish.yml?label=CI/CD&logo=github)](https://github.com/AllenInstitute/npc_stim/actions/workflows/publish.yml)
+[![GitHub issues](https://img.shields.io/github/issues/AllenInstitute/npc_stim?logo=github)](https://github.com/AllenInstitute/npc_stim/issues)
+
+# Usage
+```bash
+conda create -n npc_stim python>=3.9
+conda activate npc_stim
+pip install npc_stim
+```
+
+## Python
+```python
+>>> import npc_stim
+```
+
+# Development
+See instructions in https://github.com/AllenInstitute/npc_stim/CONTRIBUTING.md and the original template: https://github.com/AllenInstitute/copier-pdm-npc/blob/main/README.md
```

### Comparing `npc-stim-0.1.6/README.md` & `npc_stim-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `npc-stim-0.1.6/pyproject.toml` & `npc_stim-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "npc-sync>=0.1.3",
     "npc_io>=0.1.26",
     "npc-session>=0.1.33",
     "scipy>=1.12.0",
 ]
-version = "0.1.6"
+version = "0.1.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc-stim-0.1.6/src/npc_stim/running.py` & `npc_stim-0.1.7/src/npc_stim/running.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,156 @@
-from __future__ import annotations
-
-import logging
-from typing import Callable, Literal
-
-import npc_sync
-import numpy as np
-import numpy.typing as npt
-import scipy.signal
-
-import npc_stim.stim
-from npc_stim.types import StimPathOrDataset
-
-logger = logging.getLogger(__name__)
-
-RUNNING_SAMPLE_RATE = 60
-"""Visual stim f.p.s - assumed to equal running wheel sampling rate. i.e. one
-running wheel sample per camstim vsync"""
-
-RUNNING_SPEED_UNITS: Literal["cm/s", "m/s"] = "cm/s"
-"""How to report in NWB - NWB expects SI, SDK might have previously reported cm/s"""
-
-RUNNING_LOWPASS_FILTER_HZ = 4
-"""Frequency for filtering running speed - filtered data stored in NWB `processing`, unfiltered
-in `acquisition`"""
-
-
-def get_running_speed_from_stim_files(
-    *stim_path_or_dataset: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset | None = None,
-    filt: Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]] | None = None,
-) -> tuple[npt.NDArray, npt.NDArray]:
-    """Pools running speeds across files. Returns arrays of running speed and
-    corresponding timestamps."""
-    if not sync and len(stim_path_or_dataset) > 1:
-        raise ValueError(
-            "Must pass sync file to coordinate data from multiple stim files."
-        )
-
-    running_speed = np.array([])
-    timestamps = np.array([])
-
-    def _append(values, times):
-        if len(times) + 1 == len(values):
-            values = values[1:]
-
-        if len(times) == len(values):
-            times = times[1:]
-            values = values[1:]
-            times = times + 0.5 * np.median(np.diff(times))
-        else:
-            raise ValueError(
-                f"Length mismatch between running speed ({len(values)}) and timestamps ({len(times)})"
-            )
-        nonlocal running_speed, timestamps
-        # we need to filter before pooling discontiguous blocks of samples
-        running_speed = np.concatenate(
-            [running_speed, filt(values) if filt else values]
-        )
-        timestamps = np.concatenate([timestamps, times])
-
-    if sync is None:
-        _append(
-            get_running_speed_from_hdf5(*stim_path_or_dataset),
-            get_frame_times_from_stim_file(*stim_path_or_dataset),
-        )
-    else:
-        # we need timestamps for each frame's nidaq-read time (wheel encoder is read before frame's
-        # flip time)
-        # there may be multiple h5 files with encoder
-        # data per sync file: vsyncs are in blocks with a separating gap
-        for hdf5 in stim_path_or_dataset:
-            read_times = npc_stim.stim.get_input_data_times(hdf5, sync)
-            h5_data = get_running_speed_from_hdf5(hdf5)
-            if h5_data is None:
-                continue
-            _append(h5_data, read_times)
-
-    assert len(running_speed) == len(timestamps)
-    return running_speed, timestamps
-
-
-def get_frame_times_from_stim_file(
-    stim_path_or_dataset: StimPathOrDataset,
-) -> npt.NDArray:
-    return np.concatenate(
-        (
-            [0],
-            np.cumsum(
-                npc_stim.stim.get_stim_data(stim_path_or_dataset)["frameIntervals"][:]
-            ),
-        )
-    )
-
-
-def get_running_speed_from_hdf5(
-    stim_path_or_dataset: StimPathOrDataset,
-) -> npt.NDArray | None:
-    """
-    Running speed in m/s or cm/s (see `UNITS`).
-
-
-    To align with timestamps, remove timestamp[0] and sample[0] and shift
-    timestamps by half a frame (speed is estimated from difference between
-    timestamps)
-
-    See
-    https://github.com/samgale/DynamicRoutingTask/blob/main/Analysis/DynamicRoutingAnalysisUtils.py
-
-    >>> get_running_speed_from_hdf5('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
-    array([        nan, 26.76305601, 26.33139382, ..., 37.12294866, 38.20210414, 39.49709072])
-    """
-    d = npc_stim.stim.get_stim_data(stim_path_or_dataset)
-    if (
-        "rotaryEncoder" in d
-        and isinstance(d["rotaryEncoder"][()], bytes)
-        and d["rotaryEncoder"].asstr()[()] == "digital"
-    ):
-        if "frameRate" in d:
-            assert d["frameRate"][()] == RUNNING_SAMPLE_RATE
-        wheel_revolutions = (
-            d["rotaryEncoderCount"][:] / d["rotaryEncoderCountsPerRev"][()]
-        )
-        if not any(wheel_revolutions):
-            return None
-        wheel_radius_cm = d["wheelRadius"][()]
-        if RUNNING_SPEED_UNITS == "m/s":
-            running_disk_radius = wheel_radius_cm / 100
-        elif RUNNING_SPEED_UNITS == "cm/s":
-            running_disk_radius = wheel_radius_cm
-        else:
-            raise ValueError(
-                f"Unexpected units for running speed: {RUNNING_SPEED_UNITS}"
-            )
-        speed = np.diff(
-            wheel_revolutions * 2 * np.pi * running_disk_radius * RUNNING_SAMPLE_RATE
-        )
-        # we lost one sample due to diff: pad with nan to keep same number of samples
-        return np.concatenate([[np.nan], speed])
-    return None
-
-
-def lowpass_filter(running_speed: npt.NDArray) -> npt.NDArray:
-    """
-    Careful not to filter discontiguous blocks of samples.
-    See
-    https://github.com/AllenInstitute/AllenSDK/blob/36e784d007aed079e3cad2b255ca83cdbbeb1330/allensdk/brain_observatory/behavior/data_objects/running_speed/running_processing.py
-    """
-    b, a = scipy.signal.butter(
-        3, Wn=RUNNING_LOWPASS_FILTER_HZ, fs=RUNNING_SAMPLE_RATE, btype="lowpass"
-    )
-    return scipy.signal.filtfilt(b, a, np.nan_to_num(running_speed))
-
-
-if __name__ == "__main__":
-    from npc_stim import testmod
-
-    testmod()
+from __future__ import annotations
+
+import logging
+from typing import Callable, Literal
+
+import npc_sync
+import numpy as np
+import numpy.typing as npt
+import scipy.signal
+
+import npc_stim.stim
+from npc_stim.types import StimPathOrDataset
+
+logger = logging.getLogger(__name__)
+
+RUNNING_SAMPLE_RATE = 60
+"""Visual stim f.p.s - assumed to equal running wheel sampling rate. i.e. one
+running wheel sample per camstim vsync"""
+
+RUNNING_SPEED_UNITS: Literal["cm/s", "m/s"] = "cm/s"
+"""How to report in NWB - NWB expects SI, SDK might have previously reported cm/s"""
+
+RUNNING_LOWPASS_FILTER_HZ = 4
+"""Frequency for filtering running speed - filtered data stored in NWB `processing`, unfiltered
+in `acquisition`"""
+
+
+def get_running_speed_from_stim_files(
+    *stim_path_or_dataset: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset | None = None,
+    filt: Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]] | None = None,
+) -> tuple[npt.NDArray, npt.NDArray]:
+    """Pools running speeds across files. Returns arrays of running speed and
+    corresponding timestamps."""
+    if not sync and len(stim_path_or_dataset) > 1:
+        raise ValueError(
+            "Must pass sync file to coordinate data from multiple stim files."
+        )
+
+    running_speed = np.array([])
+    timestamps = np.array([])
+
+    def _append(values, times):
+        if len(times) + 1 == len(values):
+            values = values[1:]
+
+        if len(times) == len(values):
+            times = times[1:]
+            values = values[1:]
+            times = times + 0.5 * np.median(np.diff(times))
+        else:
+            raise ValueError(
+                f"Length mismatch between running speed ({len(values)}) and timestamps ({len(times)})"
+            )
+        nonlocal running_speed, timestamps
+        # we need to filter before pooling discontiguous blocks of samples
+        running_speed = np.concatenate(
+            [running_speed, filt(values) if filt else values]
+        )
+        timestamps = np.concatenate([timestamps, times])
+
+    if sync is None:
+        _append(
+            get_running_speed_from_hdf5(*stim_path_or_dataset),
+            get_frame_times_from_stim_file(*stim_path_or_dataset),
+        )
+    else:
+        # we need timestamps for each frame's nidaq-read time (wheel encoder is read before frame's
+        # flip time)
+        # there may be multiple h5 files with encoder
+        # data per sync file: vsyncs are in blocks with a separating gap
+        for hdf5 in stim_path_or_dataset:
+            read_times = npc_stim.stim.get_input_data_times(hdf5, sync)
+            h5_data = get_running_speed_from_hdf5(hdf5)
+            if h5_data is None:
+                continue
+            _append(h5_data, read_times)
+
+    assert len(running_speed) == len(timestamps)
+    return running_speed, timestamps
+
+
+def get_frame_times_from_stim_file(
+    stim_path_or_dataset: StimPathOrDataset,
+) -> npt.NDArray:
+    return np.concatenate(
+        (
+            [0],
+            np.cumsum(
+                npc_stim.stim.get_stim_data(stim_path_or_dataset)["frameIntervals"][:]
+            ),
+        )
+    )
+
+
+def get_running_speed_from_hdf5(
+    stim_path_or_dataset: StimPathOrDataset,
+) -> npt.NDArray | None:
+    """
+    Running speed in m/s or cm/s (see `UNITS`).
+
+
+    To align with timestamps, remove timestamp[0] and sample[0] and shift
+    timestamps by half a frame (speed is estimated from difference between
+    timestamps)
+
+    See
+    https://github.com/samgale/DynamicRoutingTask/blob/main/Analysis/DynamicRoutingAnalysisUtils.py
+
+    >>> get_running_speed_from_hdf5('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
+    array([        nan, 26.76305601, 26.33139382, ..., 37.12294866, 38.20210414, 39.49709072])
+    """
+    d = npc_stim.stim.get_stim_data(stim_path_or_dataset)
+    if not (
+        "rotaryEncoder" in d
+        and isinstance(d["rotaryEncoder"][()], bytes)
+        and d["rotaryEncoder"].asstr()[()] == "digital"
+    ):
+        raise ValueError(
+            f"No rotary encoder data found (or not the expected format) in {stim_path_or_dataset}"
+        )
+    if "frameRate" in d:
+        assert d["frameRate"][()] == RUNNING_SAMPLE_RATE
+    wheel_revolutions = d["rotaryEncoderCount"][:] / d["rotaryEncoderCountsPerRev"][()]
+    if not any(wheel_revolutions):
+        logger.warning(f"No wheel revolutions found in {stim_path_or_dataset}")
+    wheel_radius_cm = d["wheelRadius"][()]
+    if RUNNING_SPEED_UNITS == "m/s":
+        running_disk_radius = wheel_radius_cm / 100
+    elif RUNNING_SPEED_UNITS == "cm/s":
+        running_disk_radius = wheel_radius_cm
+    else:
+        raise ValueError(f"Unexpected units for running speed: {RUNNING_SPEED_UNITS}")
+    speed = np.diff(
+        wheel_revolutions * 2 * np.pi * running_disk_radius * RUNNING_SAMPLE_RATE
+    )
+    # we lost one sample due to diff: pad with nan to keep same number of samples
+    return np.concatenate([[np.nan], speed])
+
+
+def lowpass_filter(running_speed: npt.NDArray) -> npt.NDArray:
+    """
+    Careful not to filter discontiguous blocks of samples.
+    See
+    https://github.com/AllenInstitute/AllenSDK/blob/36e784d007aed079e3cad2b255ca83cdbbeb1330/allensdk/brain_observatory/behavior/data_objects/running_speed/running_processing.py
+    """
+    b, a = scipy.signal.butter(
+        3, Wn=RUNNING_LOWPASS_FILTER_HZ, fs=RUNNING_SAMPLE_RATE, btype="lowpass"
+    )
+    return scipy.signal.filtfilt(b, a, np.nan_to_num(running_speed))
+
+
+if __name__ == "__main__":
+    from npc_stim import testmod
+
+    testmod()
```

### Comparing `npc-stim-0.1.6/src/npc_stim/stim.py` & `npc_stim-0.1.7/src/npc_stim/stim.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,451 +1,451 @@
-from __future__ import annotations
-
-import datetime
-import io
-import logging
-import pickle
-from collections.abc import Iterable, Mapping
-from typing import Literal, SupportsFloat
-
-import h5py
-import npc_io
-import npc_session
-import npc_sync
-import numpy as np
-import numpy.typing as npt
-
-from npc_stim.types import StimPathOrDataset
-
-logger = logging.getLogger(__name__)
-
-
-def get_stim_data(stim_path: StimPathOrDataset, **kwargs) -> h5py.File | dict:
-    if isinstance(stim_path, h5py.File):
-        return stim_path
-    if isinstance(stim_path, Mapping):  # ie. from pkl file
-        return dict(stim_path)
-    path = npc_io.from_pathlike(stim_path)
-    if path.suffix in (".hdf5", ".h5"):
-        return get_h5_stim_data(path, **kwargs)
-    if path.suffix == ".pkl":
-        return get_pkl_stim_data(path, **kwargs)
-    raise ValueError(f"Unknown stim file type: {path}")
-
-
-def get_h5_stim_data(stim_path: StimPathOrDataset, **kwargs) -> h5py.File:
-    if isinstance(stim_path, h5py.File):
-        return stim_path
-    if isinstance(stim_path, Mapping):
-        raise ValueError("Susepcted pickle date encountered: use `get_pkl_stim_data`")
-    kwargs.setdefault("mode", "r")
-    path = npc_io.from_pathlike(stim_path)
-    if path.protocol in ("", "file"):
-        return h5py.File(io.BytesIO(path.read_bytes()), **kwargs)
-    else:
-        return h5py.File(path.open(mode="rb", cache_type="first"), **kwargs)
-
-
-def get_pkl_stim_data(stim_path: StimPathOrDataset, **kwargs) -> dict:
-    if isinstance(stim_path, Mapping):
-        return dict(stim_path)
-    if isinstance(stim_path, h5py.File):
-        raise ValueError("Susepcted hdf5 date encountered: use `get_h5_stim_data`")
-    kwargs.setdefault("encoding", "latin1")
-    return pickle.loads(npc_io.from_pathlike(stim_path).read_bytes())
-
-
-def get_input_data_times(
-    stim: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset | None = None,
-) -> npt.NDArray[np.float64]:
-    """Best-estimate time of `getInputData()` in psychopy event loop, in seconds, from start
-    of experiment. Uses preceding frame's vsync time if sync provided"""
-    stim = get_stim_data(stim)
-    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now"
-    if not sync:
-        return np.concatenate(([0], np.cumsum(stim["frameIntervals"][:])))
-    return np.concatenate(
-        [
-            [np.nan],
-            assert_stim_times(
-                get_stim_frame_times(stim, sync=sync, frame_time_type="vsync")[stim]
-            )[:-1],
-        ]
-    )
-
-
-def get_flip_times(
-    stim: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset | None = None,
-) -> npt.NDArray[np.float64]:
-    """Best-estimate time of `flip()` at end of psychopy event loop, in seconds, from start
-    of experiment. Uses frame's vsync time sync provided."""
-    stim = get_stim_data(stim)
-    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now"
-    if not sync:
-        return np.concatenate(
-            (
-                (c := np.cumsum(f := stim["frameIntervals"][:])),
-                [c[-1] + np.median(np.diff(f))],
-            )
-        )
-    return assert_stim_times(
-        get_stim_frame_times(stim, sync=sync, frame_time_type="vsync")[stim]
-    )
-
-
-def get_vis_display_times(
-    stim: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset | None = None,
-) -> npt.NDArray[np.float64]:
-    """Best-estimate time of monitor update. Uses photodiode if sync provided. Without sync, this equals frame times."""
-    stim = get_stim_data(stim)
-    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now "
-    if not sync:
-        return get_flip_times(stim)
-    return assert_stim_times(
-        get_stim_frame_times(stim, sync=sync, frame_time_type="display_time")[stim]
-    )
-
-
-def get_stim_frame_times(
-    *stim_paths: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset,
-    frame_time_type: Literal["display_time", "vsync"] = "display_time",
-) -> dict[StimPathOrDataset, Exception | npt.NDArray[np.float64]]:
-    """
-    - keys are the stim paths provided as inputs
-
-    >>> bad_stim = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
-    >>> good_stim_1 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/Spontaneous_670248_20230802_114611.hdf5'
-    >>> good_stim_2 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/SpontaneousRewards_670248_20230802_130736.hdf5'
-    >>> sync = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/20230802T113053.h5'
-
-    Returns the frame times for each stim file based on start time and number
-    of frames - can be provided in any order:
-    >>> frame_times = get_stim_frame_times(good_stim_2, good_stim_1, sync=sync)
-    >>> len(frame_times[good_stim_1])
-    36000
-
-    Returns Exception if the stim file can't be opened, or it has no frames.
-    Should be used with `assert_stim_times` to raise a possible exception:
-    >>> frame_times = get_stim_frame_times(bad_stim, sync=sync)
-    >>> assert_stim_times(frame_times[bad_stim])
-    Traceback (most recent call last):
-    ...
-    FileNotFoundError: aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5
-    """
-
-    # load sync file once
-    sync_data = npc_sync.get_sync_data(sync)
-    # get vsync_times_in_blocks
-    if "vsync" in frame_time_type:
-        frame_times_in_blocks = sync_data.vsync_times_in_blocks
-    # get frame_display_time_blocks
-    elif "display" in frame_time_type:
-        frame_times_in_blocks = sync_data.frame_display_time_blocks
-    else:
-        raise ValueError(f"Unexpected value: {frame_time_type = }")
-    # get num frames in each block
-    n_frames_per_block = np.asarray([len(x) for x in frame_times_in_blocks])
-    # get first frame time in each block
-    first_frame_per_block = np.asarray([x[0] for x in frame_times_in_blocks])
-
-    stim_frame_times: dict[StimPathOrDataset, Exception | npt.NDArray[np.float64]] = {}
-
-    exception: Exception | None = None
-    # loop through stim files
-    for stim_path in stim_paths:
-        # load each stim file once - may fail if file wasn't saved correctly
-        try:
-            stim_data = get_h5_stim_data(stim_path)
-        except OSError as exc:
-            exception = exc
-            stim_frame_times[stim_path] = exception
-            continue
-
-        # get number of frames
-        n_stim_frames = get_total_stim_frames(stim_data)
-        if n_stim_frames == 0:
-            exception = ValueError(f"No frames found in {stim_path = }")
-            stim_frame_times[stim_path] = exception
-            continue
-
-        # get first stimulus frame relative to sync start time
-        stim_start_time: datetime.datetime = get_stim_start_time(stim_data)
-        if abs((stim_start_time - sync_data.start_time).days > 0):
-            logger.error(
-                f"Skipping {stim_path =}, sync data is from a different day: {stim_start_time = }, {sync_data.start_time = }"
-            )
-            continue
-
-        # try to match to vsyncs by start time
-        stim_start_time_on_sync = (stim_start_time - sync_data.start_time).seconds
-        matching_block_idx_by_start_time = np.argmin(
-            abs(first_frame_per_block - stim_start_time_on_sync)
-        )
-        matching_block_idx_by_len = np.argmin(abs(n_frames_per_block - n_stim_frames))
-        start_and_len_match_disagree: bool = (
-            (matching_block_idx_by_start_time != matching_block_idx_by_len)
-            and (
-                len(
-                    [
-                        same_len_stims
-                        for same_len_stims in n_frames_per_block
-                        if same_len_stims
-                        == n_frames_per_block[matching_block_idx_by_len]
-                    ]
-                )
-                == 1
-            )
-            # if multiple blocks have the same number of frames, then we can't
-            # use the number of frames to disambiguate
-        )
-        num_frames_match: bool = (
-            n_stim_frames == n_frames_per_block[matching_block_idx_by_start_time]
-        )
-        # use first frame time for actual matching
-        if not num_frames_match and not start_and_len_match_disagree:
-            frame_diff = (
-                n_stim_frames - n_frames_per_block[matching_block_idx_by_start_time]
-            )
-            exception = IndexError(
-                f"Closest match with {stim_path} has a mismatch of {frame_diff} frames."
-            )
-            stim_frame_times[stim_path] = exception
-            continue
-        elif start_and_len_match_disagree:
-            # if frame len gets the right match, and there's only one stim with that
-            # number of frames (checked earlier), then we take it as the
-            # correct match - however it indicates a problem with time info on
-            # sync or in the stim files that we should log
-            msg = f"failed to match frame times using {stim_start_time = } with {sync_data.start_time = }, expected {stim_start_time_on_sync = }. Sync or stim file may have the wrong start-time info."
-            if n_stim_frames == n_frames_per_block[matching_block_idx_by_len]:
-                logger.warning(
-                    f"{stim_path = } matched to sync block using {n_stim_frames = }, but {msg}"
-                )
-                stim_frame_times[stim_path] = frame_times_in_blocks[
-                    matching_block_idx_by_len
-                ]
-                continue
-            # otherwise, we have a mismatch that we can't resolve
-            time_diff_len = (
-                stim_start_time_on_sync
-                - first_frame_per_block[matching_block_idx_by_len]
-            )
-            time_diff_start = (
-                stim_start_time_on_sync
-                - first_frame_per_block[matching_block_idx_by_start_time]
-            )
-            exception = IndexError(
-                f"{matching_block_idx_by_start_time=} != {matching_block_idx_by_len=} for {stim_path}: {msg} Closest match by start time has a mismatch of {time_diff_start:.1f} seconds. Closest match by number of frames has a mismatch of {time_diff_len:.1f} seconds."
-            )
-            stim_frame_times[stim_path] = exception
-            continue
-        stim_frame_times[stim_path] = frame_times_in_blocks[
-            matching_block_idx_by_start_time
-        ]
-    sorted_keys = sorted(stim_frame_times.keys(), key=lambda x: 0 if isinstance(stim_frame_times[x], Exception) else stim_frame_times[x][0])  # type: ignore[index]
-    return {k: stim_frame_times[k] for k in sorted_keys}
-
-
-def assert_stim_times(result: Exception | npt.NDArray) -> npt.NDArray:
-    """Raise exception if result is an exception, otherwise return result"""
-    if isinstance(result, Exception):
-        raise result from None
-    return result
-
-
-def get_num_trials(
-    stim_path_or_data: npc_io.PathLike | h5py.File,
-) -> int:
-    """
-    >>> get_num_trials('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
-    524
-    """
-    stim_data = get_h5_stim_data(stim_path_or_data)
-    return len(
-        stim_data.get("trialEndFrame")
-        or stim_data.get("trialOptoOnsetFrame")
-        or stim_data.get("stimStartFrame")
-    )
-
-
-def get_stim_start_time(
-    stim_path_or_data: npc_io.PathLike | h5py.File,
-) -> datetime.datetime:
-    """Absolute datetime of the first frame, according to the stim file
-    >>> get_stim_start_time('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
-    datetime.datetime(2023, 8, 31, 13, 14, 18)
-    """
-    # TODO make compatible with pkl files
-    stim_data = get_h5_stim_data(stim_path_or_data)
-    # get stim start time & convert to datetime
-    return npc_session.DatetimeRecord(stim_data["startTime"][()].decode()).dt
-
-
-def get_total_stim_frames(stim_path_or_data: npc_io.PathLike | h5py.File) -> int:
-    """
-    >>> get_total_stim_frames('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
-    217261
-    """
-    # TODO make compatible with pkl files
-    stim_data = get_h5_stim_data(stim_path_or_data)
-    frame_intervals = stim_data["frameIntervals"][:]
-    if len(frame_intervals) == 0:
-        return 0
-    return len(frame_intervals) + 1
-
-
-def get_stim_duration(stim_path_or_data: npc_io.PathLike | h5py.File) -> float:
-    """
-    >>> get_stim_duration('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
-    3647.0994503999827
-    """
-    # TODO make compatible with pkl files
-    stim_data = get_h5_stim_data(stim_path_or_data)
-    return np.sum(stim_data["frameIntervals"][:])
-
-
-def get_stim_trigger_frames(
-    stim_path_or_data: npc_io.PathLike | h5py.File,
-    stim_type: str | Literal["opto"] = "stim",
-) -> tuple[int | None, ...]:
-    """Frame index of stim command being sent. len() == num trials.
-
-    - for DynamicRouting1 files, use `stim_type='opto'` to get the trigger frames for opto
-
-    >>> path = 's3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5'
-    >>> frames = get_stim_trigger_frames(path)
-    >>> len(frames)
-    524
-
-    >>> frames = get_stim_trigger_frames(path, stim_type='opto')
-    >>> len(frames)
-    0
-    """
-    stim_data = get_h5_stim_data(stim_path_or_data)
-    start_frames = (
-        (stim_data.get("trialStimStartFrame") or stim_data.get("stimStartFrame"))
-        if stim_type != "opto"
-        else (opto := stim_data.get("trialOptoOnsetFrame"))
-    )
-
-    if start_frames is None and opto is not None:
-        # optoTagging experiments use "trialOptoOnsetFrame" instead of
-        # "trialStimStartFrame" - should be safe to switch.. the stim_type
-        # parameter just wasn't set to 'opto' when the function was called
-        start_frames = opto
-        if stim_data.get("optoTaggingLocs") is None:
-            logger.warning(
-                'Using "trialOptoOnsetFrame" instead of "trialStimStartFrame" - this is likely an old optoTagging experiment, and `stim_type` was specified as `stim` instead of `opto`.'
-            )
-
-    start_frames = start_frames[: get_num_trials(stim_data)].squeeze()
-    monotonic_increase = np.all(
-        (without_nans := start_frames[~np.isnan(start_frames)])[1:] > without_nans[:-1]
-    )
-    if not monotonic_increase:
-        # behavior files with opto report the onset frame of opto relative to stim onset for
-        # each trial. OptoTagging files specify absolute frame index
-        start_frames += stim_data.get("trialStimStartFrame")[
-            : get_num_trials(stim_data)
-        ].squeeze()
-
-    return tuple(
-        int(v) if ~np.isnan(v) else None
-        for v in safe_index(start_frames, np.arange(len(start_frames)))
-    )
-
-
-def safe_index(
-    array: npt.ArrayLike, indices: SupportsFloat | Iterable[SupportsFloat]
-) -> npt.NDArray:
-    """Checks `indices` can be safely used as array indices (i.e. all
-    numerical float values are integers), then indexes into `array` using `np.where`.
-
-    - returns nans where `indices` is nan
-    - returns a scalar if `indices` is a scalar #TODO use @overload: current type annotation is insufficient
-
-    >>> safe_index([1, 2], 0)
-    1
-    >>> safe_index([1., 2.], 0)
-    1.0
-    >>> safe_index([1., 2.], np.nan)
-    nan
-    >>> safe_index([1., 2., 3.1], [0, np.nan, 2.0])
-    array([1. , nan, 3.1])
-
-    Type of array is preserved, if possible:
-    >>> safe_index([1, 2, 3], [0., 1., 2.])
-    array([1, 2, 3])
-
-    Type of array can't be preserved if any indices are nan:
-    >>> safe_index([1, 2, 3], [0, np.nan, 2.0])
-    array([ 1., nan,  3.])
-    """
-    idx: npt.NDArray = np.array(indices)  # copy
-    if not all(idx[~np.isnan(idx)] == idx[~np.isnan(idx)].astype(np.int32)):
-        raise TypeError(
-            f"Non-integer numerical values cannot be used as indices: {idx[np.isnan(idx)][0]}"
-        )
-    array = np.array(array)  # copy/make sure array can be fancy-indexed
-    int_idx = np.where(np.isnan(idx), -1, idx)
-    result = np.where(np.isnan(idx), np.nan, array[int_idx.astype(np.int32)])
-    # np.where casts indexed array to floats just because of the
-    # possibility of nans being in result, even if they aren't:
-    # cast back if appropriate
-    if not np.isnan(result).any():
-        result = result.astype(array.dtype)
-    # if indices was a scalar, return a scalar instead of a 0d array
-    if not isinstance(indices, Iterable):
-        assert result.size == 1
-        return result.item()
-    return result
-
-
-def validate_stim(
-    *stim_paths: StimPathOrDataset,
-    sync: npc_sync.SyncPathOrDataset,
-) -> None:
-    """
-    Check that the stim files can be opened and have valid data that corresponds
-    to the sync file. Raises an AssertionError if any of the stim files fail to
-    open or can't be identified on sync.
-
-    - validation of other properties (trial starts, display times, etc.) is
-      specific to the type of stim and file format
-
-    >>> good_stim_1 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/Spontaneous_670248_20230802_114611.hdf5'
-    >>> good_stim_2 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/SpontaneousRewards_670248_20230802_130736.hdf5'
-    >>> sync = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/20230802T113053.h5'
-    >>> validate_stim(good_stim_1, good_stim_2, sync=sync)
-
-    # stim file that doesn't open or has bad data:
-    >>> bad_stim = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
-    >>> validate_stim(bad_stim, sync=sync)
-    Traceback (most recent call last):
-    ...
-    AssertionError: Failed to validate stim_path = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
-    """
-
-    def validate_single_stim(stim_path, sync=sync) -> None:
-        for v in get_stim_frame_times(
-            stim_path, sync=sync
-        ).values():  # should be only one entry
-            assert_stim_times(v)
-
-    logger.info(f"Validating {len(stim_paths)} stim files with sync data")
-    for stim_path in stim_paths:
-        logger.debug(f"Validating {stim_path = }")
-        try:
-            validate_single_stim(stim_path)
-        except Exception as exc:
-            raise AssertionError(f"Failed to validate {stim_path = }") from exc
-        logger.info(f"Validated {stim_path = }")
-
-
-if __name__ == "__main__":
-    from npc_stim import testmod
-
-    testmod()
+from __future__ import annotations
+
+import datetime
+import io
+import logging
+import pickle
+from collections.abc import Iterable, Mapping
+from typing import Literal, SupportsFloat
+
+import h5py
+import npc_io
+import npc_session
+import npc_sync
+import numpy as np
+import numpy.typing as npt
+
+from npc_stim.types import StimPathOrDataset
+
+logger = logging.getLogger(__name__)
+
+
+def get_stim_data(stim_path: StimPathOrDataset, **kwargs) -> h5py.File | dict:
+    if isinstance(stim_path, h5py.File):
+        return stim_path
+    if isinstance(stim_path, Mapping):  # ie. from pkl file
+        return dict(stim_path)
+    path = npc_io.from_pathlike(stim_path)
+    if path.suffix in (".hdf5", ".h5"):
+        return get_h5_stim_data(path, **kwargs)
+    if path.suffix == ".pkl":
+        return get_pkl_stim_data(path, **kwargs)
+    raise ValueError(f"Unknown stim file type: {path}")
+
+
+def get_h5_stim_data(stim_path: StimPathOrDataset, **kwargs) -> h5py.File:
+    if isinstance(stim_path, h5py.File):
+        return stim_path
+    if isinstance(stim_path, Mapping):
+        raise ValueError("Susepcted pickle date encountered: use `get_pkl_stim_data`")
+    kwargs.setdefault("mode", "r")
+    path = npc_io.from_pathlike(stim_path)
+    if path.protocol in ("", "file"):
+        return h5py.File(io.BytesIO(path.read_bytes()), **kwargs)
+    else:
+        return h5py.File(path.open(mode="rb", cache_type="first"), **kwargs)
+
+
+def get_pkl_stim_data(stim_path: StimPathOrDataset, **kwargs) -> dict:
+    if isinstance(stim_path, Mapping):
+        return dict(stim_path)
+    if isinstance(stim_path, h5py.File):
+        raise ValueError("Susepcted hdf5 date encountered: use `get_h5_stim_data`")
+    kwargs.setdefault("encoding", "latin1")
+    return pickle.loads(npc_io.from_pathlike(stim_path).read_bytes())
+
+
+def get_input_data_times(
+    stim: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset | None = None,
+) -> npt.NDArray[np.float64]:
+    """Best-estimate time of `getInputData()` in psychopy event loop, in seconds, from start
+    of experiment. Uses preceding frame's vsync time if sync provided"""
+    stim = get_stim_data(stim)
+    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now"
+    if not sync:
+        return np.concatenate(([0], np.cumsum(stim["frameIntervals"][:])))
+    return np.concatenate(
+        [
+            [np.nan],
+            assert_stim_times(
+                get_stim_frame_times(stim, sync=sync, frame_time_type="vsync")[stim]
+            )[:-1],
+        ]
+    )
+
+
+def get_flip_times(
+    stim: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset | None = None,
+) -> npt.NDArray[np.float64]:
+    """Best-estimate time of `flip()` at end of psychopy event loop, in seconds, from start
+    of experiment. Uses frame's vsync time sync provided."""
+    stim = get_stim_data(stim)
+    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now"
+    if not sync:
+        return np.concatenate(
+            (
+                (c := np.cumsum(f := stim["frameIntervals"][:])),
+                [c[-1] + np.median(np.diff(f))],
+            )
+        )
+    return assert_stim_times(
+        get_stim_frame_times(stim, sync=sync, frame_time_type="vsync")[stim]
+    )
+
+
+def get_vis_display_times(
+    stim: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset | None = None,
+) -> npt.NDArray[np.float64]:
+    """Best-estimate time of monitor update. Uses photodiode if sync provided. Without sync, this equals frame times."""
+    stim = get_stim_data(stim)
+    assert isinstance(stim, h5py.File), "Only hdf5 stim files supported for now "
+    if not sync:
+        return get_flip_times(stim)
+    return assert_stim_times(
+        get_stim_frame_times(stim, sync=sync, frame_time_type="display_time")[stim]
+    )
+
+
+def get_stim_frame_times(
+    *stim_paths: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset,
+    frame_time_type: Literal["display_time", "vsync"] = "display_time",
+) -> dict[StimPathOrDataset, Exception | npt.NDArray[np.float64]]:
+    """
+    - keys are the stim paths provided as inputs
+
+    >>> bad_stim = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
+    >>> good_stim_1 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/Spontaneous_670248_20230802_114611.hdf5'
+    >>> good_stim_2 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/SpontaneousRewards_670248_20230802_130736.hdf5'
+    >>> sync = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/20230802T113053.h5'
+
+    Returns the frame times for each stim file based on start time and number
+    of frames - can be provided in any order:
+    >>> frame_times = get_stim_frame_times(good_stim_2, good_stim_1, sync=sync)
+    >>> len(frame_times[good_stim_1])
+    36000
+
+    Returns Exception if the stim file can't be opened, or it has no frames.
+    Should be used with `assert_stim_times` to raise a possible exception:
+    >>> frame_times = get_stim_frame_times(bad_stim, sync=sync)
+    >>> assert_stim_times(frame_times[bad_stim])
+    Traceback (most recent call last):
+    ...
+    FileNotFoundError: aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5
+    """
+
+    # load sync file once
+    sync_data = npc_sync.get_sync_data(sync)
+    # get vsync_times_in_blocks
+    if "vsync" in frame_time_type:
+        frame_times_in_blocks = sync_data.vsync_times_in_blocks
+    # get frame_display_time_blocks
+    elif "display" in frame_time_type:
+        frame_times_in_blocks = sync_data.frame_display_time_blocks
+    else:
+        raise ValueError(f"Unexpected value: {frame_time_type = }")
+    # get num frames in each block
+    n_frames_per_block = np.asarray([len(x) for x in frame_times_in_blocks])
+    # get first frame time in each block
+    first_frame_per_block = np.asarray([x[0] for x in frame_times_in_blocks])
+
+    stim_frame_times: dict[StimPathOrDataset, Exception | npt.NDArray[np.float64]] = {}
+
+    exception: Exception | None = None
+    # loop through stim files
+    for stim_path in stim_paths:
+        # load each stim file once - may fail if file wasn't saved correctly
+        try:
+            stim_data = get_h5_stim_data(stim_path)
+        except OSError as exc:
+            exception = exc
+            stim_frame_times[stim_path] = exception
+            continue
+
+        # get number of frames
+        n_stim_frames = get_total_stim_frames(stim_data)
+        if n_stim_frames == 0:
+            exception = ValueError(f"No frames found in {stim_path = }")
+            stim_frame_times[stim_path] = exception
+            continue
+
+        # get first stimulus frame relative to sync start time
+        stim_start_time: datetime.datetime = get_stim_start_time(stim_data)
+        if abs((stim_start_time - sync_data.start_time).days > 0):
+            logger.error(
+                f"Skipping {stim_path =}, sync data is from a different day: {stim_start_time = }, {sync_data.start_time = }"
+            )
+            continue
+
+        # try to match to vsyncs by start time
+        stim_start_time_on_sync = (stim_start_time - sync_data.start_time).seconds
+        matching_block_idx_by_start_time = np.argmin(
+            abs(first_frame_per_block - stim_start_time_on_sync)
+        )
+        matching_block_idx_by_len = np.argmin(abs(n_frames_per_block - n_stim_frames))
+        start_and_len_match_disagree: bool = (
+            (matching_block_idx_by_start_time != matching_block_idx_by_len)
+            and (
+                len(
+                    [
+                        same_len_stims
+                        for same_len_stims in n_frames_per_block
+                        if same_len_stims
+                        == n_frames_per_block[matching_block_idx_by_len]
+                    ]
+                )
+                == 1
+            )
+            # if multiple blocks have the same number of frames, then we can't
+            # use the number of frames to disambiguate
+        )
+        num_frames_match: bool = (
+            n_stim_frames == n_frames_per_block[matching_block_idx_by_start_time]
+        )
+        # use first frame time for actual matching
+        if not num_frames_match and not start_and_len_match_disagree:
+            frame_diff = (
+                n_stim_frames - n_frames_per_block[matching_block_idx_by_start_time]
+            )
+            exception = IndexError(
+                f"Closest match with {stim_path} has a mismatch of {frame_diff} frames."
+            )
+            stim_frame_times[stim_path] = exception
+            continue
+        elif start_and_len_match_disagree:
+            # if frame len gets the right match, and there's only one stim with that
+            # number of frames (checked earlier), then we take it as the
+            # correct match - however it indicates a problem with time info on
+            # sync or in the stim files that we should log
+            msg = f"failed to match frame times using {stim_start_time = } with {sync_data.start_time = }, expected {stim_start_time_on_sync = }. Sync or stim file may have the wrong start-time info."
+            if n_stim_frames == n_frames_per_block[matching_block_idx_by_len]:
+                logger.warning(
+                    f"{stim_path = } matched to sync block using {n_stim_frames = }, but {msg}"
+                )
+                stim_frame_times[stim_path] = frame_times_in_blocks[
+                    matching_block_idx_by_len
+                ]
+                continue
+            # otherwise, we have a mismatch that we can't resolve
+            time_diff_len = (
+                stim_start_time_on_sync
+                - first_frame_per_block[matching_block_idx_by_len]
+            )
+            time_diff_start = (
+                stim_start_time_on_sync
+                - first_frame_per_block[matching_block_idx_by_start_time]
+            )
+            exception = IndexError(
+                f"{matching_block_idx_by_start_time=} != {matching_block_idx_by_len=} for {stim_path}: {msg} Closest match by start time has a mismatch of {time_diff_start:.1f} seconds. Closest match by number of frames has a mismatch of {time_diff_len:.1f} seconds."
+            )
+            stim_frame_times[stim_path] = exception
+            continue
+        stim_frame_times[stim_path] = frame_times_in_blocks[
+            matching_block_idx_by_start_time
+        ]
+    sorted_keys = sorted(stim_frame_times.keys(), key=lambda x: 0 if isinstance(stim_frame_times[x], Exception) else stim_frame_times[x][0])  # type: ignore[index]
+    return {k: stim_frame_times[k] for k in sorted_keys}
+
+
+def assert_stim_times(result: Exception | npt.NDArray) -> npt.NDArray:
+    """Raise exception if result is an exception, otherwise return result"""
+    if isinstance(result, Exception):
+        raise result from None
+    return result
+
+
+def get_num_trials(
+    stim_path_or_data: npc_io.PathLike | h5py.File,
+) -> int:
+    """
+    >>> get_num_trials('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
+    524
+    """
+    stim_data = get_h5_stim_data(stim_path_or_data)
+    return len(
+        stim_data.get("trialEndFrame")
+        or stim_data.get("trialOptoOnsetFrame")
+        or stim_data.get("stimStartFrame")
+    )
+
+
+def get_stim_start_time(
+    stim_path_or_data: npc_io.PathLike | h5py.File,
+) -> datetime.datetime:
+    """Absolute datetime of the first frame, according to the stim file
+    >>> get_stim_start_time('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
+    datetime.datetime(2023, 8, 31, 13, 14, 18)
+    """
+    # TODO make compatible with pkl files
+    stim_data = get_h5_stim_data(stim_path_or_data)
+    # get stim start time & convert to datetime
+    return npc_session.DatetimeRecord(stim_data["startTime"][()].decode()).dt
+
+
+def get_total_stim_frames(stim_path_or_data: npc_io.PathLike | h5py.File) -> int:
+    """
+    >>> get_total_stim_frames('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
+    217261
+    """
+    # TODO make compatible with pkl files
+    stim_data = get_h5_stim_data(stim_path_or_data)
+    frame_intervals = stim_data["frameIntervals"][:]
+    if len(frame_intervals) == 0:
+        return 0
+    return len(frame_intervals) + 1
+
+
+def get_stim_duration(stim_path_or_data: npc_io.PathLike | h5py.File) -> float:
+    """
+    >>> get_stim_duration('s3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5')
+    3647.0994503999827
+    """
+    # TODO make compatible with pkl files
+    stim_data = get_h5_stim_data(stim_path_or_data)
+    return np.sum(stim_data["frameIntervals"][:])
+
+
+def get_stim_trigger_frames(
+    stim_path_or_data: npc_io.PathLike | h5py.File,
+    stim_type: str | Literal["opto"] = "stim",
+) -> tuple[int | None, ...]:
+    """Frame index of stim command being sent. len() == num trials.
+
+    - for DynamicRouting1 files, use `stim_type='opto'` to get the trigger frames for opto
+
+    >>> path = 's3://aind-ephys-data/ecephys_668755_2023-08-31_12-33-31/behavior/DynamicRouting1_668755_20230831_131418.hdf5'
+    >>> frames = get_stim_trigger_frames(path)
+    >>> len(frames)
+    524
+
+    >>> frames = get_stim_trigger_frames(path, stim_type='opto')
+    >>> len(frames)
+    0
+    """
+    stim_data = get_h5_stim_data(stim_path_or_data)
+    start_frames = (
+        (stim_data.get("trialStimStartFrame") or stim_data.get("stimStartFrame"))
+        if stim_type != "opto"
+        else (opto := stim_data.get("trialOptoOnsetFrame"))
+    )
+
+    if start_frames is None and opto is not None:
+        # optoTagging experiments use "trialOptoOnsetFrame" instead of
+        # "trialStimStartFrame" - should be safe to switch.. the stim_type
+        # parameter just wasn't set to 'opto' when the function was called
+        start_frames = opto
+        if stim_data.get("optoTaggingLocs") is None:
+            logger.warning(
+                'Using "trialOptoOnsetFrame" instead of "trialStimStartFrame" - this is likely an old optoTagging experiment, and `stim_type` was specified as `stim` instead of `opto`.'
+            )
+
+    start_frames = start_frames[: get_num_trials(stim_data)].squeeze()
+    monotonic_increase = np.all(
+        (without_nans := start_frames[~np.isnan(start_frames)])[1:] > without_nans[:-1]
+    )
+    if not monotonic_increase:
+        # behavior files with opto report the onset frame of opto relative to stim onset for
+        # each trial. OptoTagging files specify absolute frame index
+        start_frames += stim_data.get("trialStimStartFrame")[
+            : get_num_trials(stim_data)
+        ].squeeze()
+
+    return tuple(
+        int(v) if ~np.isnan(v) else None
+        for v in safe_index(start_frames, np.arange(len(start_frames)))
+    )
+
+
+def safe_index(
+    array: npt.ArrayLike, indices: SupportsFloat | Iterable[SupportsFloat]
+) -> npt.NDArray:
+    """Checks `indices` can be safely used as array indices (i.e. all
+    numerical float values are integers), then indexes into `array` using `np.where`.
+
+    - returns nans where `indices` is nan
+    - returns a scalar if `indices` is a scalar #TODO use @overload: current type annotation is insufficient
+
+    >>> safe_index([1, 2], 0)
+    1
+    >>> safe_index([1., 2.], 0)
+    1.0
+    >>> safe_index([1., 2.], np.nan)
+    nan
+    >>> safe_index([1., 2., 3.1], [0, np.nan, 2.0])
+    array([1. , nan, 3.1])
+
+    Type of array is preserved, if possible:
+    >>> safe_index([1, 2, 3], [0., 1., 2.])
+    array([1, 2, 3])
+
+    Type of array can't be preserved if any indices are nan:
+    >>> safe_index([1, 2, 3], [0, np.nan, 2.0])
+    array([ 1., nan,  3.])
+    """
+    idx: npt.NDArray = np.array(indices)  # copy
+    if not all(idx[~np.isnan(idx)] == idx[~np.isnan(idx)].astype(np.int32)):
+        raise TypeError(
+            f"Non-integer numerical values cannot be used as indices: {idx[np.isnan(idx)][0]}"
+        )
+    array = np.array(array)  # copy/make sure array can be fancy-indexed
+    int_idx = np.where(np.isnan(idx), -1, idx)
+    result = np.where(np.isnan(idx), np.nan, array[int_idx.astype(np.int32)])
+    # np.where casts indexed array to floats just because of the
+    # possibility of nans being in result, even if they aren't:
+    # cast back if appropriate
+    if not np.isnan(result).any():
+        result = result.astype(array.dtype)
+    # if indices was a scalar, return a scalar instead of a 0d array
+    if not isinstance(indices, Iterable):
+        assert result.size == 1
+        return result.item()
+    return result
+
+
+def validate_stim(
+    *stim_paths: StimPathOrDataset,
+    sync: npc_sync.SyncPathOrDataset,
+) -> None:
+    """
+    Check that the stim files can be opened and have valid data that corresponds
+    to the sync file. Raises an AssertionError if any of the stim files fail to
+    open or can't be identified on sync.
+
+    - validation of other properties (trial starts, display times, etc.) is
+      specific to the type of stim and file format
+
+    >>> good_stim_1 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/Spontaneous_670248_20230802_114611.hdf5'
+    >>> good_stim_2 = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/SpontaneousRewards_670248_20230802_130736.hdf5'
+    >>> sync = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/20230802T113053.h5'
+    >>> validate_stim(good_stim_1, good_stim_2, sync=sync)
+
+    # stim file that doesn't open or has bad data:
+    >>> bad_stim = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
+    >>> validate_stim(bad_stim, sync=sync)
+    Traceback (most recent call last):
+    ...
+    AssertionError: Failed to validate stim_path = 's3://aind-ephys-data/ecephys_670248_2023-08-02_11-30-53/behavior/DynamicRouting1_670248_20230802_120703.hdf5'
+    """
+
+    def validate_single_stim(stim_path, sync=sync) -> None:
+        for v in get_stim_frame_times(
+            stim_path, sync=sync
+        ).values():  # should be only one entry
+            assert_stim_times(v)
+
+    logger.info(f"Validating {len(stim_paths)} stim files with sync data")
+    for stim_path in stim_paths:
+        logger.debug(f"Validating {stim_path = }")
+        try:
+            validate_single_stim(stim_path)
+        except Exception as exc:
+            raise AssertionError(f"Failed to validate {stim_path = }") from exc
+        logger.info(f"Validated {stim_path = }")
+
+
+if __name__ == "__main__":
+    from npc_stim import testmod
+
+    testmod()
```

### Comparing `npc-stim-0.1.6/src/npc_stim.egg-info/PKG-INFO` & `npc_stim-0.1.7/src/npc_stim.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1
-Name: npc-stim
-Version: 0.1.6
-Summary: Tools for accessing and processing stim data, compatible with data in the cloud.
-Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
-License: MIT
-Project-URL: Repository, https://github.com/AllenInstitute/npc_stim
-Project-URL: Issues, https://github.com/AllenInstitute/npc_stim/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: npc-sync>=0.1.3
-Requires-Dist: npc_io>=0.1.26
-Requires-Dist: npc-session>=0.1.33
-Requires-Dist: scipy>=1.12.0
-
-# npc_stim
-
-Tools for accessing and processing stim data, compatible with data in the cloud.
-
-[![PyPI](https://img.shields.io/pypi/v/npc_stim.svg?label=PyPI&color=blue)](https://pypi.org/project/npc_stim/)
-[![Python version](https://img.shields.io/pypi/pyversions/npc_stim)](https://pypi.org/project/npc_stim/)
-
-[![Coverage](https://img.shields.io/codecov/c/github/AllenInstitute/npc_stim?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_stim)
-[![CI/CD](https://img.shields.io/github/actions/workflow/status/AllenInstitute/npc_stim/publish.yml?label=CI/CD&logo=github)](https://github.com/AllenInstitute/npc_stim/actions/workflows/publish.yml)
-[![GitHub issues](https://img.shields.io/github/issues/AllenInstitute/npc_stim?logo=github)](https://github.com/AllenInstitute/npc_stim/issues)
-
-# Usage
-```bash
-conda create -n npc_stim python>=3.9
-conda activate npc_stim
-pip install npc_stim
-```
-
-## Python
-```python
->>> import npc_stim
-```
-
-# Development
-See instructions in https://github.com/AllenInstitute/npc_stim/CONTRIBUTING.md and the original template: https://github.com/AllenInstitute/copier-pdm-npc/blob/main/README.md
+Metadata-Version: 2.1
+Name: npc-stim
+Version: 0.1.7
+Summary: Tools for accessing and processing stim data, compatible with data in the cloud.
+Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
+License: MIT
+Project-URL: Repository, https://github.com/AllenInstitute/npc_stim
+Project-URL: Issues, https://github.com/AllenInstitute/npc_stim/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: npc-sync>=0.1.3
+Requires-Dist: npc_io>=0.1.26
+Requires-Dist: npc-session>=0.1.33
+Requires-Dist: scipy>=1.12.0
+
+# npc_stim
+
+Tools for accessing and processing stim data, compatible with data in the cloud.
+
+[![PyPI](https://img.shields.io/pypi/v/npc_stim.svg?label=PyPI&color=blue)](https://pypi.org/project/npc_stim/)
+[![Python version](https://img.shields.io/pypi/pyversions/npc_stim)](https://pypi.org/project/npc_stim/)
+
+[![Coverage](https://img.shields.io/codecov/c/github/AllenInstitute/npc_stim?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_stim)
+[![CI/CD](https://img.shields.io/github/actions/workflow/status/AllenInstitute/npc_stim/publish.yml?label=CI/CD&logo=github)](https://github.com/AllenInstitute/npc_stim/actions/workflows/publish.yml)
+[![GitHub issues](https://img.shields.io/github/issues/AllenInstitute/npc_stim?logo=github)](https://github.com/AllenInstitute/npc_stim/issues)
+
+# Usage
+```bash
+conda create -n npc_stim python>=3.9
+conda activate npc_stim
+pip install npc_stim
+```
+
+## Python
+```python
+>>> import npc_stim
+```
+
+# Development
+See instructions in https://github.com/AllenInstitute/npc_stim/CONTRIBUTING.md and the original template: https://github.com/AllenInstitute/copier-pdm-npc/blob/main/README.md
```

