# Comparing `tmp/hypothesis_torch-0.4.1.tar.gz` & `tmp/hypothesis_torch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.4.1.tar", last modified: Wed Apr 24 20:47:40 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.4.2.tar", last modified: Sat Apr 27 04:09:39 2024, max compression
```

## Comparing `hypothesis_torch-0.4.1.tar` & `hypothesis_torch-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:47:40.903942 hypothesis_torch-0.4.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 20:47:40.903942 hypothesis_torch-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:47:40.899942 hypothesis_torch-0.4.1/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-24 20:47:37.000000 hypothesis_torch-0.4.1/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2377 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:47:40.903942 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 20:47:40.000000 hypothesis_torch-0.4.1/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 20:45:02.000000 hypothesis_torch-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 20:47:40.903942 hypothesis_torch-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 04:09:39.204856 hypothesis_torch-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-27 04:09:39.204856 hypothesis_torch-0.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 04:09:39.200856 hypothesis_torch-0.4.2/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-27 04:09:36.000000 hypothesis_torch-0.4.2/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     8911 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 04:09:39.204856 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-27 04:09:39.000000 hypothesis_torch-0.4.2/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-27 04:09:05.000000 hypothesis_torch-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 04:09:39.204856 hypothesis_torch-0.4.2/setup.cfg
```

### Comparing `hypothesis_torch-0.4.1/LICENSE` & `hypothesis_torch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/PKG-INFO` & `hypothesis_torch-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.4.1/README.md` & `hypothesis_torch-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/__init__.py` & `hypothesis_torch-0.4.2/hypothesis_torch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
```

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/device.py` & `hypothesis_torch-0.4.2/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/dtype.py` & `hypothesis_torch-0.4.2/hypothesis_torch/dtype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Strategies for generating PyTorch dtypes."""
 
 from __future__ import annotations
 
 from collections.abc import Sequence
-from typing import Mapping
+from typing import Mapping, Literal
 
 from typing_extensions import Final
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from hypothesis import strategies as st
@@ -43,26 +43,34 @@
 
 numpy_dtype_map: Final[Mapping[torch.dtype, npt.DTypeLike]] = {
     torch.int8: np.int8,
     torch.int16: np.int16,
     torch.int32: np.int32,
     torch.int64: np.int64,
     torch.uint8: np.uint8,
-    torch.float16: float,
-    torch.float32: float,
-    torch.float64: float,
-    torch.bfloat16: float,
+    torch.float16: np.float16,
+    torch.float32: np.float32,
+    torch.float64: np.float64,
+    torch.bfloat16: np.float32,  # Numpy does not have a bf16, but it has the same dynamic range as f32
     torch.complex64: complex,
     torch.complex128: complex,
     torch.bool: np.bool_,
 }
 """A mapping from torch dtypes to numpy dtypes. Useful for generating tensors of arbitrary dtypes from the builtin
 numpy strategies."""
 
+float_width_map: Final[Mapping[torch.dtype, Literal[16, 32, 64]]] = {
+    torch.float16: 16,
+    torch.bfloat16: 32,  # Numpy does not have a bf16, but it has the same dynamic range as f32
+    torch.float32: 32,
+    torch.float64: 64,
+}
+
 assert set(numpy_dtype_map.keys()) == set(ALL_DTYPES)
+assert set(float_width_map.keys()) == set(FLOAT_DTYPES)
 
 
 def dtype_strategy(dtypes: Sequence[torch.dtype] | None = None) -> st.SearchStrategy[torch.dtype]:
     """Strategy for generating torch dtypes.
 
     Args:
         dtypes: A strategy for generating elements of the dtype. If `None`, all dtypes are sampled.
```

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.4.2/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.4.2/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/layout.py` & `hypothesis_torch-0.4.2/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.4.2/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/module.py` & `hypothesis_torch-0.4.2/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.4.2/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/tensor.py` & `hypothesis_torch-0.4.2/hypothesis_torch/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Strategies for generating PyTorch tensors."""
 
 from __future__ import annotations
 
 from collections.abc import Mapping
 from typing import Any, Sequence
+
+from hypothesis.internal.floats import float_of
 from typing_extensions import Final
 
 import hypothesis.extra.numpy as numpy_st
 import torch
-from hypothesis import strategies as st
+from hypothesis import strategies as st, reject
+from hypothesis.strategies._internal import numbers as st_numbers
 import hypothesis
 
 import hypothesis_torch
 from hypothesis_torch import dtype as dtype_module
 
 _NOT_MPS_DEVICES: Final[Sequence[torch.device]] = (
     hypothesis_torch.AVAILABLE_CPU_DEVICES + hypothesis_torch.AVAILABLE_CUDA_DEVICES
@@ -102,14 +105,40 @@
     hypothesis.assume(not (device is not None and device.type == "mps" and layout == torch.sparse_coo))
 
     # If the dtype is an integer, we need to make sure that the elements are integers within the dtype's range
     if dtype in dtype_module.INT_DTYPES and isinstance(elements, st.SearchStrategy):
         info = torch.iinfo(dtype)
         elements = elements.filter(lambda x: info.min <= x <= info.max)
 
+    # If the dtype is a float, then we need to make sure that only elements that can be represented exactly are
+    # generated
+    if dtype in dtype_module.FLOAT_DTYPES and elements is not None:
+        width = dtype_module.float_width_map[dtype]
+        if width < 64:
+
+            def downcast(x: float) -> float:
+                """Downcast a float to a smaller width.
+
+                This function is used to ensure that only floats that can be represented exactly are generated.
+
+                Adapted from `hypothesis.strategies.numbers.floats`.
+
+                Args:
+                    x: The float to downcast.
+
+                Returns:
+                    The downcasted float.
+                """
+                try:
+                    return float_of(x, width)
+                except OverflowError:  # pragma: no cover
+                    reject()
+
+            elements = elements.map(downcast)
+
     if isinstance(unique, st.SearchStrategy):
         unique = draw(unique)
 
     ndarray_strategy = numpy_st.arrays(numpy_dtype, shape, elements=elements, fill=fill, unique=unique)
     tensor = draw(ndarray_strategy.map(torch.from_numpy))
 
     if pin_memory is None:
```

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch/utils.py` & `hypothesis_torch-0.4.2/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.4.2/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.4.1/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.4.2/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.1/pyproject.toml` & `hypothesis_torch-0.4.2/pyproject.toml`

 * *Files identical despite different names*

