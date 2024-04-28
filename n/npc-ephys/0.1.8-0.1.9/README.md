# Comparing `tmp/npc-ephys-0.1.8.tar.gz` & `tmp/npc-ephys-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc-ephys-0.1.8.tar", last modified: Fri Feb  9 02:35:38 2024, max compression
+gzip compressed data, was "npc-ephys-0.1.9.tar", last modified: Thu Mar  7 01:02:06 2024, max compression
```

## Comparing `npc-ephys-0.1.8.tar` & `npc-ephys-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:38.389384 npc-ephys-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-02-09 02:35:38.385383 npc-ephys-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-09 02:35:35.000000 npc-ephys-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 02:35:38.389384 npc-ephys-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:38.385383 npc-ephys-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:38.385383 npc-ephys-0.1.8/src/npc_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-02-09 02:35:32.000000 npc-ephys-0.1.8/src/npc_ephys/barcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/openephys.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/settings_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14655 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/spikeinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/src/npc_ephys/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:38.385383 npc-ephys-0.1.8/src/npc_ephys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-02-09 02:35:38.000000 npc-ephys-0.1.8/src/npc_ephys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-09 02:35:38.000000 npc-ephys-0.1.8/src/npc_ephys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 02:35:38.000000 npc-ephys-0.1.8/src/npc_ephys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-09 02:35:38.000000 npc-ephys-0.1.8/src/npc_ephys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 02:35:38.000000 npc-ephys-0.1.8/src/npc_ephys.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 02:35:38.385383 npc-ephys-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-09 02:35:11.000000 npc-ephys-0.1.8/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 01:02:06.143088 npc-ephys-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-03-07 01:02:06.143088 npc-ephys-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-07 01:02:03.000000 npc-ephys-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 01:02:06.143088 npc-ephys-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 01:02:06.139088 npc-ephys-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 01:02:06.139088 npc-ephys-0.1.9/src/npc_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/barcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/settings_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17021 2024-03-07 01:02:00.000000 npc-ephys-0.1.9/src/npc_ephys/spikeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/src/npc_ephys/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 01:02:06.143088 npc-ephys-0.1.9/src/npc_ephys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-03-07 01:02:06.000000 npc-ephys-0.1.9/src/npc_ephys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-07 01:02:06.000000 npc-ephys-0.1.9/src/npc_ephys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 01:02:06.000000 npc-ephys-0.1.9/src/npc_ephys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-07 01:02:06.000000 npc-ephys-0.1.9/src/npc_ephys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 01:02:06.000000 npc-ephys-0.1.9/src/npc_ephys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 01:02:06.143088 npc-ephys-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-07 01:01:37.000000 npc-ephys-0.1.9/tests/test_core.py
```

### Comparing `npc-ephys-0.1.8/LICENSE` & `npc-ephys-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/PKG-INFO` & `npc-ephys-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-ephys
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for accessing and processing raw ephys data, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_ephys
 Project-URL: Issues, https://github.com/AllenInstitute/npc_ephys/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `npc-ephys-0.1.8/README.md` & `npc-ephys-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/pyproject.toml` & `npc-ephys-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "zarr>=2.16.1",
     "pandas>=2.2.0",
     "tqdm>=4.66.1",
     "npc-lims>=0.1.115",
     "wavpack-numcodecs>=0.1.5",
     "npc-io>=0.1.23",
 ]
-version = "0.1.8"
+version = "0.1.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc-ephys-0.1.8/src/npc_ephys/__init__.py` & `npc-ephys-0.1.9/src/npc_ephys/__init__.py`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/src/npc_ephys/barcodes.py` & `npc-ephys-0.1.9/src/npc_ephys/barcodes.py`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/src/npc_ephys/openephys.py` & `npc-ephys-0.1.9/src/npc_ephys/openephys.py`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/src/npc_ephys/settings_xml.py` & `npc-ephys-0.1.9/src/npc_ephys/settings_xml.py`

 * *Files identical despite different names*

### Comparing `npc-ephys-0.1.8/src/npc_ephys/spikeinterface.py` & `npc-ephys-0.1.9/src/npc_ephys/spikeinterface.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 from typing import Union
 
 import npc_io
 import npc_lims
 import npc_session
 import numpy as np
 import numpy.typing as npt
+import packaging.version
 import pandas as pd
 import upath
+import zarr
 from typing_extensions import TypeAlias
 
 logger = logging.getLogger(__name__)
 
 SpikeInterfaceData: TypeAlias = Union[
     str, npc_session.SessionRecord, npc_io.PathLike, "SpikeInterfaceKS25Data"
 ]
@@ -35,15 +37,15 @@
 
 def get_spikeinterface_data(
     session_or_root_path: SpikeInterfaceData,
 ) -> SpikeInterfaceKS25Data:
     """Return a SpikeInterfaceKS25Data object for a session.
 
     >>> paths = get_spikeinterface_data('668759_20230711')
-    >>> paths.root == get_spikeinterface_data('s3://codeocean-s3datasetsbucket-1u41qdg42ur9/4797cab2-9ea2-4747-8d15-5ba064837c1c').root
+    >>> paths.root == get_spikeinterface_data('s3://codeocean-s3datasetsbucket-1u41qdg42ur9/83754308-0a91-4b54-af79-3c42f6bc831b').root
     True
     """
     if isinstance(session_or_root_path, SpikeInterfaceKS25Data):
         return session_or_root_path
     try:
         session = npc_session.SessionRecord(str(session_or_root_path))
         root = None
@@ -59,34 +61,40 @@
     KS2.5 sorting capsule contains `processing.json`, `postprocessed`,
     `spikesorted`, etc. This class just simplifies access to the data in those
     files and dirs.
 
     Provide a session ID or a root path:
     >>> si = SpikeInterfaceKS25Data('668759_20230711')
     >>> si.root
-    S3Path('s3://codeocean-s3datasetsbucket-1u41qdg42ur9/4797cab2-9ea2-4747-8d15-5ba064837c1c')
+    S3Path('s3://codeocean-s3datasetsbucket-1u41qdg42ur9/83754308-0a91-4b54-af79-3c42f6bc831b')
 
     >>> si.template_metrics_dict('probeA')
-    {'metric_names': ['peak_to_valley', 'peak_trough_ratio', 'half_width', 'repolarization_slope', 'recovery_slope'], 'sparsity': None, 'peak_sign': 'neg', 'upsampling_factor': 10, 'window_slope_ms': 0.7}
+    {'metric_names': ['exp_decay', 'half_width', 'num_negative_peaks', 'num_positive_peaks', 'peak_to_valley', 'peak_trough_ratio', 'recovery_slope', 'repolarization_slope', 'spread', 'velocity_above', 'velocity_below'], 'sparsity': None, 'peak_sign': 'neg', 'upsampling_factor': 10, 'metrics_kwargs': {'recovery_window_ms': 0.7, 'peak_relative_threshold': 0.2, 'peak_width_ms': 0.1, 'depth_direction': 'y', 'min_channels_for_velocity': 5, 'min_r2_velocity': 0.5, 'exp_peak_function': 'ptp',
+    'min_r2_exp_decay': 0.5, 'spread_threshold': 0.2, 'spread_smooth_um': 20, 'column_range': None}}
 
     >>> si.quality_metrics_df('probeA').columns
-    Index(['num_spikes', 'firing_rate', 'presence_ratio', 'snr',
-           'isi_violations_ratio', 'isi_violations_count', 'rp_contamination',
-           'rp_violations', 'sliding_rp_violation', 'amplitude_cutoff',
-           'drift_ptp', 'drift_std', 'drift_mad', 'isolation_distance', 'l_ratio',
-           'd_prime'],
+    Index(['amplitude_cutoff', 'amplitude_cv_median', 'amplitude_cv_range',
+           'amplitude_median', 'drift_ptp', 'drift_std', 'drift_mad',
+           'firing_range', 'firing_rate', 'isi_violations_ratio',
+           'isi_violations_count', 'num_spikes', 'presence_ratio',
+           'rp_contamination', 'rp_violations', 'sliding_rp_violation', 'snr',
+           'sync_spike_2', 'sync_spike_4', 'sync_spike_8', 'd_prime',
+           'isolation_distance', 'l_ratio', 'silhouette', 'nn_hit_rate',
+           'nn_miss_rate'],
           dtype='object')
     >>> si.version
-    '0.97.1'
+    '0.100.0'
     >>> ''.join(si.probes)
-    'ABCEF'
+    'ABCDEF'
     >>> si.spike_indexes('probeA')
-    array([      491,       738,       835, ..., 143124925, 143125165, 143125201])
+    array([      145,       491,       738, ..., 143124925, 143125165, 143125201])
     >>> si.unit_indexes('probeA')
-    array([ 56,  61, 161, ..., 151,  72,  59])
+    array([ 36,  50,  55, ...,  52, 132,  53])
+    >>> len(si.original_cluster_id('probeA'))
+    139
     """
 
     session: str | npc_session.SessionRecord | None = None
     root: upath.UPath | None = None
 
     def __post_init__(self) -> None:
         if self.root is None and self.session is None:
@@ -100,20 +108,32 @@
         probes = set()
         for path in self.spikesorted().iterdir():
             with contextlib.suppress(ValueError):
                 probes.add(npc_session.ProbeRecord(path.name))
         return tuple(sorted(probes))
 
     @property
+    def is_nextflow_pipeline(self) -> bool:
+        if self.root is not None:
+            return any(f.name == "nextflow" for f in self.root.iterdir())
+
+        return False
+
+    @property
     def version(self) -> str:
-        return self.provenance(self.probes[0])["kwargs"]["parent_sorting"]["version"]
+        if not self.is_nextflow_pipeline:
+            return self.provenance(self.probes[0])["kwargs"]["parent_sorting"][
+                "version"
+            ]
+
+        return self.provenance(self.probes[0])["version"]
 
     @property
     def is_pre_v0_99(self) -> bool:
-        return self.version < "0.99"
+        return packaging.version.parse(self.version) < packaging.version.parse("0.99")
 
     @staticmethod
     @functools.cache
     def get_correct_path(*path_components: npc_io.PathLike) -> upath.UPath:
         """SpikeInterface makes paths with '#' in them, which is not allowed in s3
         paths in general - run paths through this function to fix them."""
         if not path_components:
@@ -315,30 +335,68 @@
     def cluster_indexes(self, probe: str) -> npt.NDArray[np.int64]:
         return np.take_along_axis(
             self.unit_indexes(probe, de_duplicated=False),
             self.original_cluster_id(probe),
             axis=0,
         )
 
+    def device_indices_in_nwb_units(
+        self, probe: str | npc_session.ProbeRecord
+    ) -> npt.NDArray:
+        probe = npc_session.ProbeRecord(probe)
+        devices = np.array(
+            [
+                npc_session.ProbeRecord(device)
+                for device in self.nwb["units/device_name"][:]
+            ]
+        )
+
+        return np.argwhere(devices == probe).squeeze()
+
+    def get_nwb_units_device_property(self, metric: str, probe: str) -> npt.NDArray:
+        return self.nwb[f"units/{metric}"][
+            self.device_indices_in_nwb_units(probe)
+        ].squeeze()
+
     @functools.cache
     def original_cluster_id(self, probe: str) -> npt.NDArray[np.int64]:
         """Array of cluster IDs, one per unit in unique('unit_indexes')"""
+        if self.is_nextflow_pipeline:
+            return self.get_nwb_units_device_property("ks_unit_id", probe).astype(
+                np.int64
+            )
+
+        with contextlib.suppress(FileNotFoundError):
+            return np.array(
+                io.BytesIO(
+                    self.get_correct_path(
+                        self.curated(probe),
+                        "properties",
+                        "original_cluster_id.npy",
+                    ).read_bytes()
+                )
+            )
+
         if self.is_pre_v0_99:
             # TODO! verify this is correct
             return self.sorting_cached(probe)["unit_ids"]
-        return np.load(
-            io.BytesIO(
-                self.get_correct_path(
-                    self.curated(probe),
-                    "properties",
-                    "original_cluster_id.npy",
-                ).read_bytes()
-            )
+
+        raise ValueError(
+            f"Unknown format of sorted output for SI {self.version=}, {self.is_nextflow_pipeline=}. As of March 2024 only handles 0.100 and lower"
         )
 
+    @property
+    def nwb(self) -> zarr.Group:
+        if not self.is_nextflow_pipeline:
+            raise ValueError("NWB not part of output from stand alone capsule")
+
+        assert self.root is not None
+
+        return zarr.open(next((self.root / "nwb").glob("*.nwb")))
+
     @functools.cache
     def default_qc(self, probe: str) -> npt.NDArray[np.floating]:
         return np.load(
             io.BytesIO(
                 self.get_correct_path(
                     self.curated(probe), "properties", "default_qc.npy"
                 ).read_bytes()
```

### Comparing `npc-ephys-0.1.8/src/npc_ephys/units.py` & `npc-ephys-0.1.9/src/npc_ephys/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     include_waveform_arrays: bool = False,
 ) -> pd.DataFrame:
     """
     >>> import npc_lims
     >>> device_timing_on_sync = npc_ephys.openephys.get_ephys_timing_on_sync(npc_lims.get_h5_sync_from_s3('662892_20230821'), npc_lims.get_recording_dirs_experiment_path_from_s3('662892_20230821'), only_devices_including='ProbeA')
     >>> units = make_units_table_from_spike_interface_ks25('662892_20230821', device_timing_on_sync)
     >>> len(units[units['electrode_group_name'] == 'probeA'])
-    237
+    225
     """
     spike_interface_data = npc_ephys.spikeinterface.get_spikeinterface_data(
         session_or_spikeinterface_data_or_path
     )
 
     devices_timing = tuple(
         timing for timing in device_timing_on_sync if timing.device.name.endswith("-AP")
```

### Comparing `npc-ephys-0.1.8/src/npc_ephys.egg-info/PKG-INFO` & `npc-ephys-0.1.9/src/npc_ephys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-ephys
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for accessing and processing raw ephys data, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_ephys
 Project-URL: Issues, https://github.com/AllenInstitute/npc_ephys/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

