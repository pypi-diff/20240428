# Comparing `tmp/einops-0.7.0rc2.tar.gz` & `tmp/einops-0.8.0.tar.gz`

## Comparing `einops-0.7.0rc2.tar` & `einops-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 einops-0.7.0rc2/mkdocs.yml
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 einops-0.7.0rc2/test.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/__init__.py
--rw-r--r--   0        0        0    19642 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/_backends.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/_torch_specific.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/array_api.py
--rw-r--r--   0        0        0    36794 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/einops.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/packing.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/experimental/__init__.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/experimental/data_api_packing.py
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/experimental/indexing.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/__init__.py
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/_einmix.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/chainer.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/flax.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/keras.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/oneflow.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/paddle.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/tensorflow.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 einops-0.7.0rc2/einops/layers/torch.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 einops-0.7.0rc2/scripts/convert_readme.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 einops-0.7.0rc2/scripts/setup.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/__init__.py
--rw-r--r--   0        0        0    11438 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_einsum.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_examples.py
--rw-r--r--   0        0        0    15495 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_layers.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_notebooks.py
--rw-r--r--   0        0        0    25195 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_ops.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_other.py
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_packing.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 einops-0.7.0rc2/tests/test_parsing.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 einops-0.7.0rc2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.7.0rc2/LICENSE
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 einops-0.7.0rc2/README.md
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 einops-0.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 einops-0.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 einops-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 einops-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 einops-0.8.0/test.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 einops-0.8.0/einops/__init__.py
+-rw-r--r--   0        0        0    21081 2020-02-02 00:00:00.000000 einops-0.8.0/einops/_backends.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 einops-0.8.0/einops/_torch_specific.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 einops-0.8.0/einops/array_api.py
+-rw-r--r--   0        0        0    37252 2020-02-02 00:00:00.000000 einops-0.8.0/einops/einops.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 einops-0.8.0/einops/packing.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 einops-0.8.0/einops/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.8.0/einops/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 einops-0.8.0/einops/experimental/__init__.py
+-rw-r--r--   0        0        0    14868 2020-02-02 00:00:00.000000 einops-0.8.0/einops/experimental/indexing.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/__init__.py
+-rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/_einmix.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/chainer.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/flax.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/keras.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/oneflow.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/paddle.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/tensorflow.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 einops-0.8.0/einops/layers/torch.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 einops-0.8.0/scripts/convert_readme.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 einops-0.8.0/scripts/setup.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 einops-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0    10983 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_einsum.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_examples.py
+-rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_layers.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0    27116 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_ops.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_other.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_packing.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 einops-0.8.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 einops-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 einops-0.8.0/LICENSE
+-rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 einops-0.8.0/README.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 einops-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 einops-0.8.0/PKG-INFO
```

### Comparing `einops-0.7.0rc2/mkdocs.yml` & `einops-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `einops-0.7.0rc2/test.py` & `einops-0.8.0/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,21 +31,23 @@
         have_cuda = True
 
 
 def main():
     _executable, *frameworks = sys.argv
     framework_name2installation = {
         "numpy": ["numpy"],
-        "torch": ["torch"],
-        "jax": ["jax", "jaxlib", "flax"],
+        "torch": ["torch --index-url https://download.pytorch.org/whl/cpu"],
+        "jax": ["jax[cpu]", "jaxlib", "flax"],
         "tensorflow": ["tensorflow"],
         "chainer": ["chainer"],
         "cupy": ["cupy"],
-        "paddle": ["paddlepaddle==0.0.0 -f https://www.paddlepaddle.org.cn/whl/linux/cpu-mkl/develop.html"],
-        "oneflow": ["oneflow==0.9.0+cpu -f https://release.oneflow.info"],
+        # switch to stable paddlepaddle, because of https://github.com/PaddlePaddle/Paddle/issues/63927
+        # "paddle": ["paddlepaddle==0.0.0 -f https://www.paddlepaddle.org.cn/whl/linux/cpu-mkl/develop.html"],
+        "paddle": ["paddlepaddle"],
+        "oneflow": ["oneflow==0.9.0"],
     }
 
     usage = f"""
     Usage:   python test.py <frameworks>
     Example: python test.py numpy pytorch
 
     Available frameworks: {list(framework_name2installation)}
```

### Comparing `einops-0.7.0rc2/einops/_backends.py` & `einops-0.8.0/einops/_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Backends in `einops` are organized to meet the following requirements
 - backends are not imported unless those are actually needed, because
     - backends may not be installed
     - importing all available backends will drive to significant memory footprint
-    - backends may by present but installed with errors (but never used),
+    - backends may be present but installed with errors (but never used),
       importing may drive to crashes
-- backend should be either symbolic or imperative (tensorflow is for both, but that causes problems)
+- backend should be either symbolic or imperative
     - this determines which methods (from_numpy/to_numpy or create_symbol/eval_symbol) should be defined
-- if backend can't (temporarily) provide symbols for shape dimensions, UnknownSize objects are used
+- if backend can't provide symbols for shape dimensions, UnknownSize objects are used
 """
 
 import sys
 
 __author__ = "Alex Rogozhnikov"
 
 _loaded_backends: dict = {}
@@ -25,15 +25,15 @@
     If needed, imports package and creates backend
     """
     _type = type(tensor)
     _result = _type2backend.get(_type, None)
     if _result is not None:
         return _result
 
-    for framework_name, backend in _loaded_backends.items():
+    for framework_name, backend in list(_loaded_backends.items()):
         if backend.is_appropriate_type(tensor):
             _type2backend[_type] = backend
             return backend
 
     # Find backend subclasses recursively
     backend_subclasses = []
     backends = AbstractBackend.__subclasses__()
@@ -241,17 +241,18 @@
             return x.amin(dim=reduced_axes)
         elif operation == "max":
             return x.amax(dim=reduced_axes)
         elif operation == "sum":
             return x.sum(dim=reduced_axes)
         elif operation == "mean":
             return x.mean(dim=reduced_axes)
-        elif operation == "prod":
+        elif operation in ("any", "all", "prod"):
+            # pytorch supports reducing only one operation at a time
             for i in list(sorted(reduced_axes))[::-1]:
-                x = x.prod(dim=i)
+                x = getattr(x, operation)(dim=i)
             return x
         else:
             raise NotImplementedError("Unknown reduction ", operation)
 
     def transpose(self, x, axes):
         return x.permute(axes)
 
@@ -424,15 +425,15 @@
             static_shape = x.shape.as_list()
             tf_shape = self.tf.shape(x)
             # use the static shape where known, otherwise use the TF shape components
             shape = tuple([s or tf_shape[dim] for dim, s in enumerate(static_shape)])
             try:
                 hash(shape)
                 return shape
-            except:
+            except BaseException:
                 # unhashable symbols in shape. Wrap tuple to be hashable.
                 return HashableTuple(shape)
 
     def reduce(self, x, operation, axes):
         return getattr(self.tf, "reduce_" + operation)(x, axis=axes)
 
     def reshape(self, x, shape):
@@ -461,15 +462,15 @@
 
         return tensorflow
 
     def einsum(self, pattern, *x):
         return self.tf.einsum(pattern, *x)
 
 
-class KerasBackend(AbstractBackend):
+class TFKerasBackend(AbstractBackend):
     framework_name = "tensorflow.keras"
 
     def __init__(self):
         import tensorflow as tf
 
         self.tf = tf
         self.keras = tf.keras
@@ -548,15 +549,15 @@
 
     def reduce(self, x, operation, reduced_axes):
         for axis in sorted(reduced_axes, reverse=True):
             if operation == "min":
                 x, _ = x.min(dim=axis)
             elif operation == "max":
                 x, _ = x.max(dim=axis)
-            elif operation in ["sum", "mean", "prod"]:
+            elif operation in ["sum", "mean", "prod", "any", "all"]:
                 x = getattr(x, operation)(dim=axis)
             else:
                 raise NotImplementedError("Unknown reduction ", operation)
         return x
 
     def transpose(self, x, axes):
         return x.permute(axes)
@@ -611,16 +612,16 @@
     def to_numpy(self, x):
         return x.detach().numpy()
 
     def arange(self, start, stop):
         return self.paddle.arange(start, stop, dtype=self.paddle.int64)
 
     def reduce(self, x, operation, axes):
-        # TODO: Support the reduce operation to output a 0D Tensor
         if len(axes) == x.ndim:
+            # currently paddle returns 1d tensor instead of 0d
             return super().reduce(x, operation, axes).squeeze(0)
         else:
             return super().reduce(x, operation, axes)
 
     def transpose(self, x, axes):
         return x.transpose(axes)
 
@@ -655,7 +656,60 @@
         return paddle
 
     def einsum(self, pattern, *x):
         return self.paddle.einsum(pattern, *x)
 
     def shape(self, x):
         return tuple(x.shape)
+
+
+class TinygradBackend(AbstractBackend):
+    framework_name = "tinygrad"
+
+    def __init__(self):
+        import tinygrad
+
+        self.tinygrad = tinygrad
+
+    def is_appropriate_type(self, tensor):
+        return isinstance(tensor, self.tinygrad.Tensor)
+
+    def from_numpy(self, x):
+        return self.tinygrad.Tensor(x)
+
+    def to_numpy(self, x):
+        return x.numpy()
+
+    def arange(self, start, stop):
+        return self.tinygrad.Tensor.arange(start, stop)
+
+    def shape(self, x):
+        return x.shape
+
+    def reshape(self, x, shape):
+        return x.reshape(shape)
+
+    def transpose(self, x, axes):
+        return x.permute(axes)
+
+    def reduce(self, x, operation, axes):
+        for axis in sorted(axes, reverse=True):
+            x = getattr(x, operation)(axis=axis)
+        return x
+
+    def stack_on_zeroth_dimension(self, tensors: list):
+        return self.tinygrad.Tensor.stack(tensors)
+
+    def add_axis(self, x, new_position):
+        return x.unsqueeze(new_position)
+
+    def tile(self, x, repeats):
+        return x.repeat(repeats)
+
+    def concat(self, tensors, axis: int):
+        return tensors[0].cat(tensors[1:], axis) if len(tensors) > 1 else tensors[0]
+
+    def is_float_type(self, x):
+        return self.tinygrad.dtypes.is_float(x.dtype)
+
+    def einsum(self, pattern, *x):
+        return self.tinygrad.Tensor.einsum(pattern, *x)
```

### Comparing `einops-0.7.0rc2/einops/_torch_specific.py` & `einops-0.8.0/einops/_torch_specific.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Specialization of einops for torch.
 
 Unfortunately, torch's jit scripting mechanism isn't strong enough,
 and to have scripting supported at least for layers,
 a number of additional moves is needed.
 
 Design of main operations (dynamic resolution by lookup) is unlikely
-to be implemented by torch.jit.script, 
+to be implemented by torch.jit.script,
 but torch.compile seems to work with operations just fine.
 """
+
 import warnings
 from typing import Dict, List, Tuple
 
 import torch
 from einops.einops import TransformRecipe, _reconstruct_from_shape_uncached
```

### Comparing `einops-0.7.0rc2/einops/array_api.py` & `einops-0.8.0/einops/array_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,75 +12,78 @@
     else:
         xp = tensor.__array_namespace__()
     try:
         hashable_axes_lengths = tuple(axes_lengths.items())
         recipe = _prepare_transformation_recipe(pattern, reduction, axes_names=tuple(axes_lengths), ndim=tensor.ndim)
         return _apply_recipe_array_api(
             xp,
-            recipe=recipe, tensor=tensor, reduction_type=reduction, axes_lengths=hashable_axes_lengths,
+            recipe=recipe,
+            tensor=tensor,
+            reduction_type=reduction,
+            axes_lengths=hashable_axes_lengths,
         )
     except EinopsError as e:
         message = ' Error while processing {}-reduction pattern "{}".'.format(reduction, pattern)
         if not isinstance(tensor, list):
             message += "\n Input tensor shape: {}. ".format(tensor.shape)
         else:
             message += "\n Input is list. "
         message += "Additional info: {}.".format(axes_lengths)
         raise EinopsError(message + "\n {}".format(e))
 
 
-
 def repeat(tensor: Tensor, pattern: str, **axes_lengths) -> Tensor:
     return reduce(tensor, pattern, reduction="repeat", **axes_lengths)
 
 
 def rearrange(tensor: Tensor, pattern: str, **axes_lengths) -> Tensor:
     return reduce(tensor, pattern, reduction="rearrange", **axes_lengths)
 
 
 def asnumpy(tensor: Tensor):
     import numpy as np
+
     return np.from_dlpack(tensor)
 
+
 Shape = Tuple
 
+
 def pack(tensors: Sequence[Tensor], pattern: str) -> Tuple[Tensor, List[Shape]]:
-    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, 'pack')
+    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, "pack")
     xp = tensors[0].__array_namespace__()
 
     reshaped_tensors: List[Tensor] = []
     packed_shapes: List[Shape] = []
     for i, tensor in enumerate(tensors):
         shape = tensor.shape
         if len(shape) < min_axes:
-            raise EinopsError(f'packed tensor #{i} (enumeration starts with 0) has shape {shape}, '
-                              f'while pattern {pattern} assumes at least {min_axes} axes')
+            raise EinopsError(
+                f"packed tensor #{i} (enumeration starts with 0) has shape {shape}, "
+                f"while pattern {pattern} assumes at least {min_axes} axes"
+            )
         axis_after_packed_axes = len(shape) - n_axes_after
         packed_shapes.append(shape[n_axes_before:axis_after_packed_axes])
         reshaped_tensors.append(xp.reshape(tensor, (*shape[:n_axes_before], -1, *shape[axis_after_packed_axes:])))
 
     return xp.concat(reshaped_tensors, axis=n_axes_before), packed_shapes
 
 
-
 def unpack(tensor: Tensor, packed_shapes: List[Shape], pattern: str) -> List[Tensor]:
     xp = tensor.__array_namespace__()
-    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, opname='unpack')
+    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, opname="unpack")
 
     # backend = get_backend(tensor)
     input_shape = tensor.shape
     if len(input_shape) != n_axes_before + 1 + n_axes_after:
-        raise EinopsError(f'unpack(..., {pattern}) received input of wrong dim with shape {input_shape}')
+        raise EinopsError(f"unpack(..., {pattern}) received input of wrong dim with shape {input_shape}")
 
     unpacked_axis: int = n_axes_before
 
-    lengths_of_composed_axes: List[int] = [
-        -1 if -1 in p_shape else prod(p_shape)
-        for p_shape in packed_shapes
-    ]
+    lengths_of_composed_axes: List[int] = [-1 if -1 in p_shape else prod(p_shape) for p_shape in packed_shapes]
 
     n_unknown_composed_axes = sum(x == -1 for x in lengths_of_composed_axes)
     if n_unknown_composed_axes > 1:
         raise EinopsError(
             f"unpack(..., {pattern}) received more than one -1 in {packed_shapes} and can't infer dimensions"
         )
 
@@ -98,22 +101,24 @@
         unknown_composed_axis: int = lengths_of_composed_axes.index(-1)
         for i in range(unknown_composed_axis):
             split_positions[i + 1] = split_positions[i] + lengths_of_composed_axes[i]
         for j in range(unknown_composed_axis + 1, len(lengths_of_composed_axes))[::-1]:
             split_positions[j] = split_positions[j + 1] - lengths_of_composed_axes[j]
 
     shape_start = input_shape[:unpacked_axis]
-    shape_end = input_shape[unpacked_axis + 1:]
+    shape_end = input_shape[unpacked_axis + 1 :]
     slice_filler = (slice(None, None),) * unpacked_axis
     try:
         return [
             xp.reshape(
                 # shortest way slice arbitrary axis
                 tensor[(*slice_filler, slice(split_positions[i], split_positions[i + 1]), ...)],
-                (*shape_start, *element_shape, *shape_end)
+                (*shape_start, *element_shape, *shape_end),
             )
             for i, element_shape in enumerate(packed_shapes)
         ]
     except BaseException:
         # this hits if there is an error during reshapes, which means passed shapes were incorrect
-        raise RuntimeError(f'Error during unpack(..., "{pattern}"): could not split axis of size {split_positions[-1]}'
-                           f' into requested {packed_shapes}')
+        raise RuntimeError(
+            f'Error during unpack(..., "{pattern}"): could not split axis of size {split_positions[-1]}'
+            f" into requested {packed_shapes}"
+        )
```

### Comparing `einops-0.7.0rc2/einops/einops.py` & `einops-0.8.0/einops/einops.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import string
 import typing
 from collections import OrderedDict
 from typing import Set, Tuple, List, Dict, Union, Callable, Optional, TypeVar, cast, Any
 
 if typing.TYPE_CHECKING:
     # for docstrings in pycharm
-    import numpy as np
+    import numpy as np  # noqa E401
 
 from . import EinopsError
 from ._backends import get_backend
 from .parsing import ParsedExpression, _ellipsis, AnonymousAxis
 
 Tensor = TypeVar("Tensor")
 ReductionCallable = Callable[[Tensor, Tuple[int, ...]], Tensor]
 Reduction = Union[str, ReductionCallable]
 
-_reductions = ("min", "max", "sum", "mean", "prod")
+_reductions = ("min", "max", "sum", "mean", "prod", "any", "all")
 
 # magic integers are required to stay within
 # traceable subset of language
 _unknown_axis_length = -999999
 _expected_axis_length = -99999
 
 
@@ -683,17 +683,27 @@
             exp.composition[:ellipsis_idx]
             + ["_"] * (len(shape) - len(exp.composition) + 1)
             + exp.composition[ellipsis_idx + 1 :]
         )
     else:
         composition = exp.composition
     result = {}
-    for (axis_name,), axis_length in zip(composition, shape):  # type: ignore
-        if axis_name != "_":
-            result[axis_name] = axis_length
+    for axes, axis_length in zip(composition, shape):  # type: ignore
+        # axes either [], or [AnonymousAxis] or ['axis_name']
+        if len(axes) == 0:
+            if axis_length != 1:
+                raise RuntimeError(f"Length of axis is not 1: {pattern} {shape}")
+        else:
+            [axis] = axes
+            if isinstance(axis, str):
+                if axis != "_":
+                    result[axis] = axis_length
+            else:
+                if axis.value != axis_length:
+                    raise RuntimeError(f"Length of anonymous axis does not match: {pattern} {shape}")
     return result
 
 
 # _enumerate_directions is not exposed in the public API
 def _enumerate_directions(x):
     """
     For an n-dimensional tensor, returns tensors to enumerate each axis.
@@ -800,35 +810,31 @@
 
         compact_pattern += axis_name_mapping[axis_name]
 
     return compact_pattern
 
 
 @typing.overload
-def einsum(tensor: Tensor, pattern: str, /) -> Tensor:
-    ...
+def einsum(tensor: Tensor, pattern: str, /) -> Tensor: ...
 
 
 @typing.overload
-def einsum(tensor1: Tensor, tensor2: Tensor, pattern: str, /) -> Tensor:
-    ...
+def einsum(tensor1: Tensor, tensor2: Tensor, pattern: str, /) -> Tensor: ...
 
 
 @typing.overload
-def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, pattern: str, /) -> Tensor:
-    ...
+def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, pattern: str, /) -> Tensor: ...
 
 
 @typing.overload
-def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, tensor4: Tensor, pattern: str, /) -> Tensor:
-    ...
+def einsum(tensor1: Tensor, tensor2: Tensor, tensor3: Tensor, tensor4: Tensor, pattern: str, /) -> Tensor: ...
 
 
 def einsum(*tensors_and_pattern: Union[Tensor, str]) -> Tensor:
-    """
+    r"""
     einops.einsum calls einsum operations with einops-style named
     axes indexing, computing tensor products with an arbitrary
     number of tensors. Unlike typical einsum syntax, here you must
     pass tensors first, and then the pattern.
 
     Also, note that rearrange operations such as `"(batch chan) out"`,
     or singleton axes `()`, are not currently supported.
```

### Comparing `einops-0.7.0rc2/einops/packing.py` & `einops-0.8.0/einops/packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from typing import List, Union, TypeVar, Tuple, Sequence
 
 from einops import EinopsError
 
 from einops._backends import get_backend
 from einops.parsing import ParsedExpression
 
-Tensor = TypeVar('Tensor')
+Tensor = TypeVar("Tensor")
 
 Shape = Union[Tuple[int, ...], List[int]]
 
 
 @lru_cache(maxsize=128)
 def analyze_pattern(pattern: str, opname: str) -> Tuple[int, int, int]:
     # Maybe some validation of identifiers?
     axes = pattern.split()
     axes_set = set(axes)
     if len(axes) != len(axes_set):
         raise EinopsError(f'Duplicates in axes names in {opname}(..., "{pattern}")')
-    if '*' not in axes_set:
+    if "*" not in axes_set:
         raise EinopsError(f'No *-axis in {opname}(..., "{pattern}")')
     for axis in axes:
-        if axis != '*':
+        if axis != "*":
             is_valid, reason = ParsedExpression.check_axis_name_return_reason(axis)
             if not is_valid:
                 raise EinopsError(f'Invalid axis name {axis} in {opname}(..., "{pattern}")')
-    n_axes_before = axes.index('*')
+    n_axes_before = axes.index("*")
     n_axes_after = len(axes) - n_axes_before - 1
     min_axes = n_axes_before + n_axes_after
     return n_axes_before, n_axes_after, min_axes
 
 
 def pack(tensors: Sequence[Tensor], pattern: str) -> Tuple[Tensor, List[Shape]]:
     """
@@ -63,31 +63,31 @@
     >>> inputs_unpacked = unpack(packed, ps, 'i j * k')
     >>> [x.shape for x in inputs_unpacked]
     [(2, 3, 5), (2, 3, 7, 5), (2, 3, 7, 9, 5)]
     ```
 
     Read the tutorial for introduction and application scenarios.
     """
-    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, 'pack')
+    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, "pack")
 
     # packing zero tensors is illegal
     backend = get_backend(tensors[0])
 
     reshaped_tensors: List[Tensor] = []
     packed_shapes: List[Shape] = []
     for i, tensor in enumerate(tensors):
         shape = backend.shape(tensor)
         if len(shape) < min_axes:
-            raise EinopsError(f'packed tensor #{i} (enumeration starts with 0) has shape {shape}, '
-                              f'while pattern {pattern} assumes at least {min_axes} axes')
+            raise EinopsError(
+                f"packed tensor #{i} (enumeration starts with 0) has shape {shape}, "
+                f"while pattern {pattern} assumes at least {min_axes} axes"
+            )
         axis_after_packed_axes = len(shape) - n_axes_after
         packed_shapes.append(shape[n_axes_before:axis_after_packed_axes])
-        reshaped_tensors.append(
-            backend.reshape(tensor, (*shape[:n_axes_before], -1, *shape[axis_after_packed_axes:]))
-        )
+        reshaped_tensors.append(backend.reshape(tensor, (*shape[:n_axes_before], -1, *shape[axis_after_packed_axes:])))
 
     return backend.concat(reshaped_tensors, axis=n_axes_before), packed_shapes
 
 
 def prod(x: Shape) -> int:
     result = 1
     for i in x:
@@ -132,29 +132,26 @@
     >>> inputs_unpacked = unpack(packed, ps, 'i j * k')
     >>> [x.shape for x in inputs_unpacked]
     [(2, 3, 5), (2, 3, 7, 5), (2, 3, 7, 9, 5)]
     ```
 
     Read the tutorial for introduction and application scenarios.
     """
-    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, opname='unpack')
+    n_axes_before, n_axes_after, min_axes = analyze_pattern(pattern, opname="unpack")
 
     backend = get_backend(tensor)
     input_shape = backend.shape(tensor)
     if len(input_shape) != n_axes_before + 1 + n_axes_after:
-        raise EinopsError(f'unpack(..., {pattern}) received input of wrong dim with shape {input_shape}')
+        raise EinopsError(f"unpack(..., {pattern}) received input of wrong dim with shape {input_shape}")
 
     unpacked_axis: int = n_axes_before
 
-    lengths_of_composed_axes: List[int] = [
-        -1 if -1 in p_shape else prod(p_shape)
-        for p_shape in packed_shapes
-    ]
+    lengths_of_composed_axes: List[int] = [-1 if -1 in p_shape else prod(p_shape) for p_shape in packed_shapes]
 
-    n_unknown_composed_axes = sum(x == -1 for x in lengths_of_composed_axes)
+    n_unknown_composed_axes = sum(int(x == -1) for x in lengths_of_composed_axes)
     if n_unknown_composed_axes > 1:
         raise EinopsError(
             f"unpack(..., {pattern}) received more than one -1 in {packed_shapes} and can't infer dimensions"
         )
 
     # following manipulations allow to skip some shape verifications
     # and leave it to backends
@@ -170,22 +167,24 @@
         unknown_composed_axis: int = lengths_of_composed_axes.index(-1)
         for i in range(unknown_composed_axis):
             split_positions[i + 1] = split_positions[i] + lengths_of_composed_axes[i]
         for j in range(unknown_composed_axis + 1, len(lengths_of_composed_axes))[::-1]:
             split_positions[j] = split_positions[j + 1] - lengths_of_composed_axes[j]
 
     shape_start = input_shape[:unpacked_axis]
-    shape_end = input_shape[unpacked_axis + 1:]
+    shape_end = input_shape[unpacked_axis + 1 :]
     slice_filler = (slice(None, None),) * unpacked_axis
     try:
         return [
             backend.reshape(
                 # shortest way slice arbitrary axis
                 tensor[(*slice_filler, slice(split_positions[i], split_positions[i + 1]))],
-                (*shape_start, *element_shape, *shape_end)
+                (*shape_start, *element_shape, *shape_end),
             )
             for i, element_shape in enumerate(packed_shapes)
         ]
     except BaseException:
         # this hits if there is an error during reshapes, which means passed shapes were incorrect
-        raise RuntimeError(f'Error during unpack(..., "{pattern}"): could not split axis of size {split_positions[-1]}'
-                           f' into requested {packed_shapes}')
+        raise RuntimeError(
+            f'Error during unpack(..., "{pattern}"): could not split axis of size {split_positions[-1]}'
+            f" into requested {packed_shapes}"
+        )
```

### Comparing `einops-0.7.0rc2/einops/parsing.py` & `einops-0.8.0/einops/parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from einops import EinopsError
 import keyword
 import warnings
 from typing import List, Optional, Set, Tuple, Union
 
-_ellipsis: str = '…'  # NB, this is a single unicode symbol. String is used as it is not a list, but can be iterated
+_ellipsis: str = "…"  # NB, this is a single unicode symbol. String is used as it is not a list, but can be iterated
 
 
 class AnonymousAxis(object):
-    """Important thing: all instances of this class are not equal to each other """
+    """Important thing: all instances of this class are not equal to each other"""
 
     def __init__(self, value: str):
         self.value = int(value)
         if self.value <= 1:
             if self.value == 1:
-                raise EinopsError('No need to create anonymous axis of length 1. Report this as an issue')
+                raise EinopsError("No need to create anonymous axis of length 1. Report this as an issue")
             else:
-                raise EinopsError('Anonymous axis should have positive length, not {}'.format(self.value))
+                raise EinopsError("Anonymous axis should have positive length, not {}".format(self.value))
 
     def __repr__(self):
         return "{}-axis".format(str(self.value))
 
 
 class ParsedExpression:
     """
     non-mutable structure that contains information about one side of expression (e.g. 'b c (h w)')
     and keeps some information important for downstream
     """
-    def __init__(self, expression: str, *, allow_underscore: bool = False,
-                 allow_duplicates: bool = False):
+
+    def __init__(self, expression: str, *, allow_underscore: bool = False, allow_duplicates: bool = False):
         self.has_ellipsis: bool = False
         self.has_ellipsis_parenthesized: Optional[bool] = None
         self.identifiers: Set[str] = set()
         # that's axes like 2, 3, 4 or 5. Axes with size 1 are exceptional and replaced with empty composition
         self.has_non_unitary_anonymous_axes: bool = False
         # composition keeps structure of composite axes, see how different corner cases are handled in tests
         self.composition: List[Union[List[str], str]] = []
-        if '.' in expression:
-            if '...' not in expression:
-                raise EinopsError('Expression may contain dots only inside ellipsis (...)')
-            if str.count(expression, '...') != 1 or str.count(expression, '.') != 3:
+        if "." in expression:
+            if "..." not in expression:
+                raise EinopsError("Expression may contain dots only inside ellipsis (...)")
+            if str.count(expression, "...") != 1 or str.count(expression, ".") != 3:
                 raise EinopsError(
-                    'Expression may contain dots only inside ellipsis (...); only one ellipsis for tensor ')
-            expression = expression.replace('...', _ellipsis)
+                    "Expression may contain dots only inside ellipsis (...); only one ellipsis for tensor "
+                )
+            expression = expression.replace("...", _ellipsis)
             self.has_ellipsis = True
 
         bracket_group: Optional[List[str]] = None
 
         def add_axis_name(x):
             if x in self.identifiers:
                 if not (allow_underscore and x == "_") and not allow_duplicates:
@@ -65,41 +66,41 @@
                     if bracket_group is None:
                         self.composition.append([])
                     else:
                         pass  # no need to think about 1s inside parenthesis
                     return
                 is_axis_name, reason = self.check_axis_name_return_reason(x, allow_underscore=allow_underscore)
                 if not (is_number or is_axis_name):
-                    raise EinopsError('Invalid axis identifier: {}\n{}'.format(x, reason))
+                    raise EinopsError("Invalid axis identifier: {}\n{}".format(x, reason))
                 if is_number:
                     x = AnonymousAxis(x)
                 self.identifiers.add(x)
                 if is_number:
                     self.has_non_unitary_anonymous_axes = True
                 if bracket_group is None:
                     self.composition.append([x])
                 else:
                     bracket_group.append(x)
 
         current_identifier = None
         for char in expression:
-            if char in '() ':
+            if char in "() ":
                 if current_identifier is not None:
                     add_axis_name(current_identifier)
                 current_identifier = None
-                if char == '(':
+                if char == "(":
                     if bracket_group is not None:
                         raise EinopsError("Axis composition is one-level (brackets inside brackets not allowed)")
                     bracket_group = []
-                elif char == ')':
+                elif char == ")":
                     if bracket_group is None:
-                        raise EinopsError('Brackets are not balanced')
+                        raise EinopsError("Brackets are not balanced")
                     self.composition.append(bracket_group)
                     bracket_group = None
-            elif str.isalnum(char) or char in ['_', _ellipsis]:
+            elif str.isalnum(char) or char in ["_", _ellipsis]:
                 if current_identifier is None:
                     current_identifier = char
                 else:
                     current_identifier += char
             else:
                 raise EinopsError("Unknown character '{}'".format(char))
 
@@ -107,41 +108,43 @@
             raise EinopsError('Imbalanced parentheses in expression: "{}"'.format(expression))
         if current_identifier is not None:
             add_axis_name(current_identifier)
 
     def flat_axes_order(self) -> List:
         result = []
         for composed_axis in self.composition:
-            assert isinstance(composed_axis, list), 'does not work with ellipsis'
+            assert isinstance(composed_axis, list), "does not work with ellipsis"
             for axis in composed_axis:
                 result.append(axis)
         return result
 
     def has_composed_axes(self) -> bool:
         # this will ignore 1 inside brackets
         for axes in self.composition:
             if isinstance(axes, list) and len(axes) > 1:
                 return True
         return False
 
     @staticmethod
     def check_axis_name_return_reason(name: str, allow_underscore: bool = False) -> Tuple[bool, str]:
         if not str.isidentifier(name):
-            return False, 'not a valid python identifier'
-        elif name[0] == '_' or name[-1] == '_':
-            if name == '_' and allow_underscore:
-                return True, ''
-            return False, 'axis name should should not start or end with underscore'
+            return False, "not a valid python identifier"
+        elif name[0] == "_" or name[-1] == "_":
+            if name == "_" and allow_underscore:
+                return True, ""
+            return False, "axis name should should not start or end with underscore"
         else:
             if keyword.iskeyword(name):
                 warnings.warn("It is discouraged to use axes names that are keywords: {}".format(name), RuntimeWarning)
-            if name in ['axis']:
-                warnings.warn("It is discouraged to use 'axis' as an axis name "
-                              "and will raise an error in future", FutureWarning)
-            return True, ''
+            if name in ["axis"]:
+                warnings.warn(
+                    "It is discouraged to use 'axis' as an axis name " "and will raise an error in future",
+                    FutureWarning,
+                )
+            return True, ""
 
     @staticmethod
     def check_axis_name(name: str) -> bool:
         """
         Valid axes names are python identifiers except keywords,
         and additionally should not start or end with underscore
         """
```

### Comparing `einops-0.7.0rc2/einops/experimental/indexing.py` & `einops-0.8.0/einops/experimental/indexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,22 +55,22 @@
 
 """
 
 from typing import List, Union, TypeVar, Tuple
 
 from einops import EinopsError
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class CompositionDecomposition:
     def __init__(
-            self,
-            decomposed_shape: List[str],
-            composed_shape: List[List[str]],
+        self,
+        decomposed_shape: List[str],
+        composed_shape: List[List[str]],
     ):
         flat_shape = []
         for x in composed_shape:
             flat_shape.extend(x)
 
         self.compose_transposition: Tuple[int, ...] = tuple([decomposed_shape.index(x) for x in flat_shape])
         self.decompose_transposition: Tuple[int, ...] = tuple([flat_shape.index(x) for x in decomposed_shape])
@@ -131,47 +131,46 @@
     shape = [1] * n_axes
     shape[axis] = axis_len
     x = xp.reshape(x, shape)
     return x
 
 
 class IndexingFormula:
-
     def __init__(self, pattern: str):
         """
         :param pattern: example 'b t c <- b hsel wsel c, [hsel, wsel] b t'
         """
         self.pattern = pattern
-        left, right = pattern.split('<-')
-        arg_split = right.index(',')
-        arr_pattern, ind_pattern = right[:arg_split], right[arg_split + 1:]
+        left, right = pattern.split("<-")
+        arg_split = right.index(",")
+        arr_pattern, ind_pattern = right[:arg_split], right[arg_split + 1 :]
         ind_pattern = ind_pattern.strip()
         # print(
         #     arr_pattern, '\n',
         #     ind_pattern,
         # )
-        assert ind_pattern.startswith('['), 'composition axis should go first in indexer (second argument) [h w] i j k'
-        composition_start = ind_pattern.index('[')
-        composition_end = ind_pattern.index(']')
-        composition = ind_pattern[composition_start + 1: composition_end]
-        ind_other_axes = ind_pattern[composition_end + 1:]
+        assert ind_pattern.startswith("["), "composition axis should go first in indexer (second argument) [h w] i j k"
+        composition_start = ind_pattern.index("[")
+        composition_end = ind_pattern.index("]")
+        composition = ind_pattern[composition_start + 1 : composition_end]
+        ind_other_axes = ind_pattern[composition_end + 1 :]
 
         self.result_axes_names = left.split()
         self.array_axes_names = arr_pattern.split()
-        self.indexing_axes_names = [x.strip() for x in composition.split(',')]
+        self.indexing_axes_names = [x.strip() for x in composition.split(",")]
         self.indexer_other_axes_names = ind_other_axes.split()
 
         for group_name, group in [
-            ('result', self.result_axes_names),
-            ('array', self.array_axes_names),
-            ('indexer', self.indexing_axes_names + self.indexer_other_axes_names),
+            ("result", self.result_axes_names),
+            ("array", self.array_axes_names),
+            ("indexer", self.indexing_axes_names + self.indexer_other_axes_names),
         ]:
             if len(set(group)) != len(group):
                 # need more verbosity, which axis, raise
-                raise EinopsError(f'{group_name} pattern ({group}) contains a duplicated axis')
+                raise EinopsError(f"{group_name} pattern ({group}) contains a duplicated axis")
 
         axis_groups = [
             self.result_axes_names,
             self.array_axes_names,
             self.indexing_axes_names,
             self.indexer_other_axes_names,
         ]
@@ -187,24 +186,24 @@
 
         for axis in all_axes:
             presence = tuple(axis in g for g in axis_groups)
             # want match-case here. sweet dreams
             if presence == (False, True, True, False):
                 self.indexer_axes.append(axis)
             elif presence[2]:
-                raise EinopsError(f'Wrong usage of indexer variable {axis}')
+                raise EinopsError(f"Wrong usage of indexer variable {axis}")
             elif presence == (True, True, False, True):
                 self.batch_axes.append(axis)
             elif presence == (True, False, False, True):
                 self.result_and_index_axes.append(axis)
             elif presence == (True, True, False, False):
                 self.result_and_array_axes.append(axis)
             else:
                 # TODO better categorization of wrong usage patterns
-                raise EinopsError(f'{axis} is used incorrectly in {pattern}')
+                raise EinopsError(f"{axis} is used incorrectly in {pattern}")
 
         assert set(self.indexer_axes) == set(self.indexing_axes_names)
         # order of these variables matters, since we can't lose mapping here
         self.indexer_axes = self.indexing_axes_names
 
         self.array_composition = CompositionDecomposition(
             decomposed_shape=self.array_axes_names,
@@ -244,18 +243,25 @@
 
         for axis_name, indexer in list(zip(self.indexing_axes_names, ind))[::-1]:
             full_index = full_index + shift * (indexer % known_axes_sizes[axis_name])
             shift *= known_axes_sizes[axis_name]
 
         for axis_name in self.batch_axes[::-1]:
             axis_id = self.indexer_other_axes_names.index(axis_name)
-            full_index = full_index + arange_at_position(
-                xp, len(self.indexer_other_axes_names), axis=axis_id, axis_len=known_axes_sizes[axis_name],
-                device=arr.device,
-            ) * shift
+            full_index = (
+                full_index
+                + arange_at_position(
+                    xp,
+                    len(self.indexer_other_axes_names),
+                    axis=axis_id,
+                    axis_len=known_axes_sizes[axis_name],
+                    device=arr.device,
+                )
+                * shift
+            )
             shift *= known_axes_sizes[axis_name]
 
         assert shift == arr_2d.shape[0]
 
         # step 3. Flatten index
         full_index = self.index_composition.compose(full_index, known_axes_sizes)
 
@@ -277,32 +283,33 @@
     """
     formula = IndexingFormula(pattern)
     return formula.apply_to_array_api(arr, ind)
 
 
 def test_composition_and_decomposition():
     import numpy.array_api as np
+
     x = np.arange(2 * 3 * 5 * 7)
     x = np.reshape(x, (2, 3, 5, 7))
     comp = CompositionDecomposition(
-        decomposed_shape=['a', 'b', 'c', 'd'],
-        composed_shape=[['a', 'b'], ['c', 'd']],
+        decomposed_shape=["a", "b", "c", "d"],
+        composed_shape=[["a", "b"], ["c", "d"]],
     )
     assert comp.compose(x, known_axes_lengths={}).shape == (2 * 3, 5 * 7)
 
     y = CompositionDecomposition(
-        decomposed_shape=['a', 'b', 'c', 'd'],
-        composed_shape=[['a', 'b'], [], ['c', 'd']],
+        decomposed_shape=["a", "b", "c", "d"],
+        composed_shape=[["a", "b"], [], ["c", "d"]],
     ).compose(x, {})
     assert y.shape == (2 * 3, 1, 5 * 7)
     assert np.all(np.reshape(x, (-1,)) == np.reshape(y, (-1,)))
 
     comp = CompositionDecomposition(
-        decomposed_shape=['a', 'b', 'e', 'c', 'd'],
-        composed_shape=[['e', 'c'], ['b'], ['a', 'd']],
+        decomposed_shape=["a", "b", "e", "c", "d"],
+        composed_shape=[["e", "c"], ["b"], ["a", "d"]],
     )
     x = np.arange(2 * 3 * 5 * 7 * 3)
     x = np.reshape(x, (2, 3, 5, 7, 3))
 
     axes = {}
     y = comp.compose(x, axes)
     x2 = comp.decompose(y, axes)
@@ -311,44 +318,44 @@
 
 def test_simple_indexing():
     import numpy.array_api as np
 
     # simple 2d test
     arr = np.reshape(np.arange(5 * 7), (5, 7))
     ind = np.arange(7) % 5
-    x = einindex('j <- i j, [i] j', arr, [ind])
+    x = einindex("j <- i j, [i] j", arr, [ind])
     for j, i in enumerate(ind):
         assert arr[i, j] == x[j]
 
-    y = einindex('j <- j i, [i] j', np.permute_dims(arr, (1, 0)), [ind])
+    y = einindex("j <- j i, [i] j", np.permute_dims(arr, (1, 0)), [ind])
     for j, i in enumerate(ind):
         assert arr[i, j] == y[j]
 
 
 def test_multidimensional_indexing():
     import numpy.array_api as np
 
     embedding_bhwc = (
-            + arange_at_position(np, 4, 0, 2) * 1000
-            + arange_at_position(np, 4, 1, 3) * 100
-            + arange_at_position(np, 4, 2, 5) * 10
-            + arange_at_position(np, 4, 3, 7) * 1
+        +arange_at_position(np, 4, 0, 2) * 1000
+        + arange_at_position(np, 4, 1, 3) * 100
+        + arange_at_position(np, 4, 2, 5) * 10
+        + arange_at_position(np, 4, 3, 7) * 1
     )
 
     hindices_bt = np.reshape(np.arange(6), (2, 3)) % 3
     windices_bt = np.reshape(np.arange(6), (2, 3)) % 5
 
     # imagine that you have pairs of image <> sentence
     # your goal is to get most suitable token from image for every token in sentence
     # thus for every token in sentence you compute best k and v
 
-    result = einindex('c t b <- b h w c, [h, w] b t', embedding_bhwc, [hindices_bt, windices_bt])
+    result = einindex("c t b <- b h w c, [h, w] b t", embedding_bhwc, [hindices_bt, windices_bt])
     # example of using a single array for indexing multiple axes
     hw_indices_bt = np.stack([hindices_bt, windices_bt])
-    result2 = einindex('c t b <- b h w c, [h, w] b t', embedding_bhwc, hw_indices_bt)
+    result2 = einindex("c t b <- b h w c, [h, w] b t", embedding_bhwc, hw_indices_bt)
     assert np.all(result == result2)
 
     # check vs manual element computation
     result_manual = result * 0
     for b in range(2):
         for t in range(3):
             for c in range(7):
@@ -365,29 +372,27 @@
     C, T, B = 2, 3, 5
     # G = GPU, batch-like varaible
     G = 4
     H = 7
     W = 9
 
     arr_gtbc = (
-            + arange_at_position(np, 4, 0, G) * 1000
-            + arange_at_position(np, 4, 1, T) * 100
-            + arange_at_position(np, 4, 2, B) * 10
-            + arange_at_position(np, 4, 3, C) * 1
+        +arange_at_position(np, 4, 0, G) * 1000
+        + arange_at_position(np, 4, 1, T) * 100
+        + arange_at_position(np, 4, 2, B) * 10
+        + arange_at_position(np, 4, 3, C) * 1
     )
 
     t_indices_gbhw = np.reshape(np.arange(G * B * H * W), (G, B, H, W)) % T
 
-    result = einindex('g b c h w <- g t b c, [t] g b h w', arr_gtbc, [t_indices_gbhw])
+    result = einindex("g b c h w <- g t b c, [t] g b h w", arr_gtbc, [t_indices_gbhw])
 
     result_manual = result * 0
     for g in range(G):
         for b in range(B):
             for c in range(C):
                 for h in range(H):
                     for w in range(W):
                         t = t_indices_gbhw[g, b, h, w]
                         result_manual[g, b, c, h, w] = arr_gtbc[g, t, b, c]
 
     assert np.all(result == result_manual)
-
-
```

### Comparing `einops-0.7.0rc2/einops/layers/__init__.py` & `einops-0.8.0/einops/layers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 from typing import Any, Dict
 
 
 from ..einops import TransformRecipe, _apply_recipe, _prepare_recipes_for_all_dims, get_backend
 from .. import EinopsError
 
@@ -24,40 +24,40 @@
         # self._recipe = self.recipe()  # checking parameters
         self._multirecipe = self.multirecipe()
         self._axes_lengths = tuple(self.axes_lengths.items())
 
     def __repr__(self) -> str:
         params = repr(self.pattern)
         for axis, length in self.axes_lengths.items():
-            params += ', {}={}'.format(axis, length)
-        return '{}({})'.format(self.__class__.__name__, params)
+            params += ", {}={}".format(axis, length)
+        return "{}({})".format(self.__class__.__name__, params)
 
     def multirecipe(self) -> Dict[int, TransformRecipe]:
         try:
             return _prepare_recipes_for_all_dims(
-                self.pattern, operation='rearrange', axes_names=tuple(self.axes_lengths)
+                self.pattern, operation="rearrange", axes_names=tuple(self.axes_lengths)
             )
         except EinopsError as e:
-            raise EinopsError(' Error while preparing {!r}\n {}'.format(self, e))
+            raise EinopsError(" Error while preparing {!r}\n {}".format(self, e))
 
     def _apply_recipe(self, x):
         backend = get_backend(x)
         return _apply_recipe(
             backend=backend,
             recipe=self._multirecipe[len(x.shape)],
             tensor=x,
-            reduction_type='rearrange',
+            reduction_type="rearrange",
             axes_lengths=self._axes_lengths,
         )
 
     def __getstate__(self):
-        return {'pattern': self.pattern, 'axes_lengths': self.axes_lengths}
+        return {"pattern": self.pattern, "axes_lengths": self.axes_lengths}
 
     def __setstate__(self, state):
-        self.__init__(pattern=state['pattern'], **state['axes_lengths'])
+        self.__init__(pattern=state["pattern"], **state["axes_lengths"])
 
 
 class ReduceMixin:
     """
     Reduce layer behaves identically to einops.reduce operation.
 
     :param pattern: str, rearrangement pattern
@@ -72,35 +72,35 @@
         self.pattern = pattern
         self.reduction = reduction
         self.axes_lengths = axes_lengths
         self._multirecipe = self.multirecipe()
         self._axes_lengths = tuple(self.axes_lengths.items())
 
     def __repr__(self):
-        params = '{!r}, {!r}'.format(self.pattern, self.reduction)
+        params = "{!r}, {!r}".format(self.pattern, self.reduction)
         for axis, length in self.axes_lengths.items():
-            params += ', {}={}'.format(axis, length)
-        return '{}({})'.format(self.__class__.__name__, params)
+            params += ", {}={}".format(axis, length)
+        return "{}({})".format(self.__class__.__name__, params)
 
     def multirecipe(self) -> Dict[int, TransformRecipe]:
         try:
             return _prepare_recipes_for_all_dims(
                 self.pattern, operation=self.reduction, axes_names=tuple(self.axes_lengths)
             )
         except EinopsError as e:
-            raise EinopsError(' Error while preparing {!r}\n {}'.format(self, e))
+            raise EinopsError(" Error while preparing {!r}\n {}".format(self, e))
 
     def _apply_recipe(self, x):
         backend = get_backend(x)
         return _apply_recipe(
             backend=backend,
             recipe=self._multirecipe[len(x.shape)],
             tensor=x,
             reduction_type=self.reduction,
             axes_lengths=self._axes_lengths,
         )
 
     def __getstate__(self):
-        return {'pattern': self.pattern, 'reduction': self.reduction, 'axes_lengths': self.axes_lengths}
+        return {"pattern": self.pattern, "reduction": self.reduction, "axes_lengths": self.axes_lengths}
 
     def __setstate__(self, state):
-        self.__init__(pattern=state['pattern'], reduction=state['reduction'], **state['axes_lengths'])
+        self.__init__(pattern=state["pattern"], reduction=state["reduction"], **state["axes_lengths"])
```

### Comparing `einops-0.7.0rc2/einops/layers/_einmix.py` & `einops-0.8.0/einops/layers/_einmix.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def _report_axes(axes: set, report_message: str):
     if len(axes) > 0:
         raise EinopsError(report_message.format(axes))
 
 
 class _EinmixMixin:
-    def __init__(self, pattern: str, weight_shape: str, bias_shape: Optional[str]=None, **axes_lengths: Any):
+    def __init__(self, pattern: str, weight_shape: str, bias_shape: Optional[str] = None, **axes_lengths: Any):
         """
         EinMix - Einstein summation with automated tensor management and axis packing/unpacking.
 
         EinMix is an advanced tool, helpful tutorial:
         https://github.com/arogozhnikov/einops/blob/master/docs/3-einmix-layer.ipynb
 
         Imagine taking einsum with two arguments, one of each input, and one - tensor with weights
@@ -32,103 +32,101 @@
         There is no restriction to mix the last axis. Let's mix along height
         >>> EinMix('h w c-> hout w c', weight_shape='h hout', bias_shape='hout', h=32, hout=32)
         Channel-wise multiplication (like one used in normalizations)
         >>> EinMix('t b c -> t b c', weight_shape='c', c=128)
         Multi-head linear layer (each head is own linear layer):
         >>> EinMix('t b (head cin) -> t b (head cout)', weight_shape='head cin cout', ...)
 
-        ... ah yes, you need to specify all dimensions of weight shape/bias shape in parameters.
+        ... and yes, you need to specify all dimensions of weight shape/bias shape in parameters.
 
         Use cases:
         - when channel dimension is not last, use EinMix, not transposition
         - patch/segment embeddings
         - when need only within-group connections to reduce number of weights and computations
         - perfect as a part of sequential models
-        - next-gen MLPs (follow tutorial to learn more)
+        - next-gen MLPs (follow tutorial to learn more!)
 
-        Uniform He initialization is applied to weight tensor and encounters for number of elements mixed.
+        Uniform He initialization is applied to weight tensor. This accounts for number of elements mixed.
 
         Parameters
         :param pattern: transformation pattern, left side - dimensions of input, right side - dimensions of output
         :param weight_shape: axes of weight. A tensor of this shape is created, stored, and optimized in a layer
         :param bias_shape: axes of bias added to output. Weights of this shape are created and stored. If `None` (the default), no bias is added.
         :param axes_lengths: dimensions of weight tensor
         """
         super().__init__()
         self.pattern = pattern
         self.weight_shape = weight_shape
         self.bias_shape = bias_shape
         self.axes_lengths = axes_lengths
-        self.initialize_einmix(pattern=pattern, weight_shape=weight_shape, bias_shape=bias_shape, axes_lengths=axes_lengths)
+        self.initialize_einmix(
+            pattern=pattern, weight_shape=weight_shape, bias_shape=bias_shape, axes_lengths=axes_lengths
+        )
 
     def initialize_einmix(self, pattern: str, weight_shape: str, bias_shape: Optional[str], axes_lengths: dict):
-        left_pattern, right_pattern = pattern.split('->')
+        left_pattern, right_pattern = pattern.split("->")
         left = ParsedExpression(left_pattern)
         right = ParsedExpression(right_pattern)
         weight = ParsedExpression(weight_shape)
         _report_axes(
             set.difference(right.identifiers, {*left.identifiers, *weight.identifiers}),
-            'Unrecognized identifiers on the right side of EinMix {}'
+            "Unrecognized identifiers on the right side of EinMix {}",
         )
 
         if left.has_ellipsis or right.has_ellipsis or weight.has_ellipsis:
-            raise EinopsError('Ellipsis is not supported in EinMix (right now)')
+            raise EinopsError("Ellipsis is not supported in EinMix (right now)")
         if any(x.has_non_unitary_anonymous_axes for x in [left, right, weight]):
-            raise EinopsError('Anonymous axes (numbers) are not allowed in EinMix')
-        if '(' in weight_shape or ')' in weight_shape:
-            raise EinopsError(f'Parenthesis is not allowed in weight shape: {weight_shape}')
+            raise EinopsError("Anonymous axes (numbers) are not allowed in EinMix")
+        if "(" in weight_shape or ")" in weight_shape:
+            raise EinopsError(f"Parenthesis is not allowed in weight shape: {weight_shape}")
 
         pre_reshape_pattern = None
         pre_reshape_lengths = None
         post_reshape_pattern = None
         if any(len(group) != 1 for group in left.composition):
             names: List[str] = []
             for group in left.composition:
                 names += group
-            composition = ' '.join(names)
-            pre_reshape_pattern = f'{left_pattern}->{composition}'
+            composition = " ".join(names)
+            pre_reshape_pattern = f"{left_pattern}->{composition}"
             pre_reshape_lengths = {name: length for name, length in axes_lengths.items() if name in names}
 
         if any(len(group) != 1 for group in right.composition):
             names = []
             for group in right.composition:
                 names += group
-            composition = ' '.join(names)
-            post_reshape_pattern = f'{composition}->{right_pattern}'
+            composition = " ".join(names)
+            post_reshape_pattern = f"{composition}->{right_pattern}"
 
         self._create_rearrange_layers(pre_reshape_pattern, pre_reshape_lengths, post_reshape_pattern, {})
 
         for axis in weight.identifiers:
             if axis not in axes_lengths:
-                raise EinopsError('Dimension {} of weight should be specified'.format(axis))
+                raise EinopsError("Dimension {} of weight should be specified".format(axis))
         _report_axes(
             set.difference(set(axes_lengths), {*left.identifiers, *weight.identifiers}),
-            'Axes {} are not used in pattern',
+            "Axes {} are not used in pattern",
         )
         _report_axes(
-            set.difference(weight.identifiers, {*left.identifiers, *right.identifiers}),
-            'Weight axes {} are redundant'
+            set.difference(weight.identifiers, {*left.identifiers, *right.identifiers}), "Weight axes {} are redundant"
         )
         if len(weight.identifiers) == 0:
-            warnings.warn('EinMix: weight has no dimensions (means multiplication by a number)')
+            warnings.warn("EinMix: weight has no dimensions (means multiplication by a number)")
 
-        _weight_shape = [axes_lengths[axis] for axis, in weight.composition]
+        _weight_shape = [axes_lengths[axis] for (axis,) in weight.composition]
         # single output element is a combination of fan_in input elements
-        _fan_in = _product([axes_lengths[axis] for axis, in weight.composition if axis not in right.identifiers])
+        _fan_in = _product([axes_lengths[axis] for (axis,) in weight.composition if axis not in right.identifiers])
         if bias_shape is not None:
             if not isinstance(bias_shape, str):
-                raise EinopsError('bias shape should be string specifying which axes bias depends on')
+                raise EinopsError("bias shape should be string specifying which axes bias depends on")
             bias = ParsedExpression(bias_shape)
-            _report_axes(
-                set.difference(bias.identifiers, right.identifiers),
-                'Bias axes {} not present in output'
-            )
+            _report_axes(set.difference(bias.identifiers, right.identifiers), "Bias axes {} not present in output")
             _report_axes(
                 set.difference(bias.identifiers, set(axes_lengths)),
-                'Sizes not provided for bias axes {}',
+                "Sizes not provided for bias axes {}",
             )
 
             _bias_shape = []
             for axes in right.composition:
                 for axis in axes:
                     if axis in bias.identifiers:
                         _bias_shape.append(axes_lengths[axis])
@@ -143,34 +141,36 @@
 
         # rewrite einsum expression with single-letter latin identifiers so that
         # expression will be understood by any framework
         mapped_identifiers = {*left.identifiers, *right.identifiers, *weight.identifiers}
         mapping2letters = {k: letter for letter, k in zip(string.ascii_lowercase, mapped_identifiers)}
 
         def write_flat(axes: list):
-            return ''.join(mapping2letters[axis] for axis in axes)
+            return "".join(mapping2letters[axis] for axis in axes)
 
-        self.einsum_pattern: str = '{},{}->{}'.format(
+        self.einsum_pattern: str = "{},{}->{}".format(
             write_flat(left.flat_axes_order()),
             write_flat(weight.flat_axes_order()),
             write_flat(right.flat_axes_order()),
         )
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict]):
-        raise NotImplementedError('Should be defined in framework implementations')
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
+        raise NotImplementedError("Should be defined in framework implementations")
 
     def _create_parameters(self, weight_shape, weight_bound, bias_shape, bias_bound):
-        """ Shape and implementations """
-        raise NotImplementedError('Should be defined in framework implementations')
+        """Shape and implementations"""
+        raise NotImplementedError("Should be defined in framework implementations")
 
     def __repr__(self):
         params = repr(self.pattern)
         params += f", '{self.weight_shape}'"
         if self.bias_shape is not None:
             params += f", '{self.bias_shape}'"
         for axis, length in self.axes_lengths.items():
-            params += ', {}={}'.format(axis, length)
-        return '{}({})'.format(self.__class__.__name__, params)
+            params += ", {}={}".format(axis, length)
+        return "{}({})".format(self.__class__.__name__, params)
```

### Comparing `einops-0.7.0rc2/einops/layers/chainer.py` & `einops-0.8.0/einops/layers/chainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Dict, cast
 
 import chainer
 
 from . import RearrangeMixin, ReduceMixin
 from ._einmix import _EinmixMixin
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 
 class Rearrange(RearrangeMixin, chainer.Link):
     def __call__(self, x):
         return self._apply_recipe(x)
 
 
@@ -24,20 +24,21 @@
         with self.init_scope():
             self.weight = chainer.variable.Parameter(uniform(weight_bound), weight_shape)
             if bias_shape is not None:
                 self.bias = chainer.variable.Parameter(uniform(bias_bound), bias_shape)
             else:
                 self.bias = None
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict],
-                                 ):
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
         self.pre_rearrange = None
         if pre_reshape_pattern is not None:
             self.pre_rearrange = Rearrange(pre_reshape_pattern, **cast(dict, pre_reshape_lengths))
 
         self.post_rearrange = None
         if post_reshape_pattern is not None:
             self.post_rearrange = Rearrange(post_reshape_pattern, **cast(dict, post_reshape_lengths))
```

### Comparing `einops-0.7.0rc2/einops/layers/flax.py` & `einops-0.8.0/einops/layers/flax.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
 from . import RearrangeMixin, ReduceMixin
 from ._einmix import _EinmixMixin
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 
 class Reduce(nn.Module):
     pattern: str
     reduction: str
     sizes: dict = field(default_factory=lambda: {})
 
@@ -52,19 +52,21 @@
         self.weight = self.param("weight", jax.nn.initializers.uniform(weight_bound), weight_shape)
 
         if bias_shape is not None:
             self.bias = self.param("bias", jax.nn.initializers.uniform(bias_bound), bias_shape)
         else:
             self.bias = None
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict]):
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
         self.pre_rearrange = None
         if pre_reshape_pattern is not None:
             self.pre_rearrange = Rearrange(pre_reshape_pattern, sizes=cast(dict, pre_reshape_lengths))
 
         self.post_rearrange = None
         if post_reshape_pattern is not None:
             self.post_rearrange = Rearrange(post_reshape_pattern, sizes=cast(dict, post_reshape_lengths))
```

### Comparing `einops-0.7.0rc2/einops/layers/oneflow.py` & `einops-0.8.0/einops/layers/oneflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from typing import Optional, Dict, cast
 
 import oneflow as flow
 
 from . import RearrangeMixin, ReduceMixin
 from ._einmix import _EinmixMixin
 
-__author__ = 'Tianhe Ren & Depeng Liang'
+__author__ = "Tianhe Ren & Depeng Liang"
 
 
 class Rearrange(RearrangeMixin, flow.nn.Module):
     def forward(self, input):
         return self._apply_recipe(input)
 
 
 class Reduce(ReduceMixin, flow.nn.Module):
     def forward(self, input):
         return self._apply_recipe(input)
 
 
 class EinMix(_EinmixMixin, flow.nn.Module):
     def _create_parameters(self, weight_shape, weight_bound, bias_shape, bias_bound):
-        self.weight = flow.nn.Parameter(flow.zeros(weight_shape).uniform_(-weight_bound, weight_bound),
-                                         requires_grad=True)
+        self.weight = flow.nn.Parameter(
+            flow.zeros(weight_shape).uniform_(-weight_bound, weight_bound), requires_grad=True
+        )
         if bias_shape is not None:
-            self.bias = flow.nn.Parameter(flow.zeros(bias_shape).uniform_(-bias_bound, bias_bound),
-                                           requires_grad=True)
+            self.bias = flow.nn.Parameter(flow.zeros(bias_shape).uniform_(-bias_bound, bias_bound), requires_grad=True)
         else:
             self.bias = None
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict],
-                                 ):
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
         self.pre_rearrange = None
         if pre_reshape_pattern is not None:
             self.pre_rearrange = Rearrange(pre_reshape_pattern, **cast(dict, pre_reshape_lengths))
 
         self.post_rearrange = None
         if post_reshape_pattern is not None:
             self.post_rearrange = Rearrange(post_reshape_pattern, **cast(dict, post_reshape_lengths))
```

### Comparing `einops-0.7.0rc2/einops/layers/paddle.py` & `einops-0.8.0/einops/layers/paddle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Dict, cast
 
 import paddle
 
 from . import RearrangeMixin, ReduceMixin
 from ._einmix import _EinmixMixin
 
-__author__ = 'PaddlePaddle'
+__author__ = "PaddlePaddle"
 
 
 class Rearrange(RearrangeMixin, paddle.nn.Layer):
     def forward(self, input):
         return self._apply_recipe(input)
 
 
@@ -17,43 +17,42 @@
     def forward(self, input):
         return self._apply_recipe(input)
 
 
 class EinMix(_EinmixMixin, paddle.nn.Layer):
     def _create_parameters(self, weight_shape, weight_bound, bias_shape, bias_bound):
         self.weight = self.create_parameter(
-            weight_shape, 
-            default_initializer=paddle.nn.initializer.Uniform(-weight_bound, weight_bound)
+            weight_shape, default_initializer=paddle.nn.initializer.Uniform(-weight_bound, weight_bound)
         )
 
         if bias_shape is not None:
             self.bias = self.create_parameter(
-                bias_shape,
-                default_initializer=paddle.nn.initializer.Uniform(-bias_bound, bias_bound)
+                bias_shape, default_initializer=paddle.nn.initializer.Uniform(-bias_bound, bias_bound)
             )
         else:
             self.bias = None
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict],
-                                 ):
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
         self.pre_rearrange = None
         if pre_reshape_pattern is not None:
             self.pre_rearrange = Rearrange(pre_reshape_pattern, **cast(dict, pre_reshape_lengths))
 
         self.post_rearrange = None
         if post_reshape_pattern is not None:
             self.post_rearrange = Rearrange(post_reshape_pattern, **cast(dict, post_reshape_lengths))
 
     def forward(self, input):
         if self.pre_rearrange is not None:
             input = self.pre_rearrange(input)
-        
+
         result = paddle.einsum(self.einsum_pattern, input, self.weight)
         if self.bias is not None:
             result += self.bias
         if self.post_rearrange is not None:
             result = self.post_rearrange(result)
-        return result
+        return result
```

### Comparing `einops-0.7.0rc2/einops/layers/tensorflow.py` & `einops-0.8.0/einops/layers/torch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,67 @@
-from typing import List, Optional, Dict, cast
+from typing import Optional, Dict, cast
 
-import tensorflow as tf
-from tensorflow.keras.layers import Layer
+import torch
 
-from .._backends import UnknownSize
 from . import RearrangeMixin, ReduceMixin
 from ._einmix import _EinmixMixin
-from ..einops import TransformRecipe, _reconstruct_from_shape_uncached
+from .._torch_specific import apply_for_scriptable_torch
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 
-def _compute_output_shape(recipe: TransformRecipe, input_shape) -> List[Optional[int]]:
-    input_shape = [UnknownSize() if d is None else int(d) for d in input_shape]
-    init_shapes, reduced_axes, axes_reordering, added_axes, final_shape = \
-        _reconstruct_from_shape_uncached(recipe, input_shape)
-    output_shape: List[Optional[int]] = [None if isinstance(d, UnknownSize) else int(d) for d in final_shape]
-    return output_shape
-
-
-class Rearrange(RearrangeMixin, Layer):
-    def compute_output_shape(self, input_shape):
-        return _compute_output_shape(self.recipe(), input_shape)
-
-    def call(self, inputs):
-        return self._apply_recipe(inputs)
-
-    def get_config(self):
-        return {'pattern': self.pattern, **self.axes_lengths}
+class Rearrange(RearrangeMixin, torch.nn.Module):
+    def forward(self, input):
+        recipe = self._multirecipe[input.ndim]
+        return apply_for_scriptable_torch(recipe, input, reduction_type="rearrange", axes_dims=self._axes_lengths)
 
+    def _apply_recipe(self, x):
+        # overriding parent method to prevent it's scripting
+        pass
 
-class Reduce(ReduceMixin, Layer):
-    def compute_output_shape(self, input_shape):
-        return _compute_output_shape(self.recipe(), input_shape)
 
-    def call(self, inputs):
-        return self._apply_recipe(inputs)
+class Reduce(ReduceMixin, torch.nn.Module):
+    def forward(self, input):
+        recipe = self._multirecipe[input.ndim]
+        return apply_for_scriptable_torch(recipe, input, reduction_type=self.reduction, axes_dims=self._axes_lengths)
 
-    def get_config(self):
-        return {'pattern': self.pattern, 'reduction': self.reduction, **self.axes_lengths}
+    def _apply_recipe(self, x):
+        # overriding parent method to prevent it's scripting
+        pass
 
 
-class EinMix(_EinmixMixin, Layer):
+class EinMix(_EinmixMixin, torch.nn.Module):
     def _create_parameters(self, weight_shape, weight_bound, bias_shape, bias_bound):
-        self.weight = tf.Variable(tf.random_uniform_initializer(-weight_bound, weight_bound)(shape=weight_shape),
-                                  trainable=True)
+        self.weight = torch.nn.Parameter(
+            torch.zeros(weight_shape).uniform_(-weight_bound, weight_bound), requires_grad=True
+        )
         if bias_shape is not None:
-            self.bias = tf.Variable(tf.random_uniform_initializer(-bias_bound, bias_bound)(shape=bias_shape),
-                                    trainable=True)
+            self.bias = torch.nn.Parameter(
+                torch.zeros(bias_shape).uniform_(-bias_bound, bias_bound), requires_grad=True
+            )
         else:
             self.bias = None
 
-    def _create_rearrange_layers(self,
-                                 pre_reshape_pattern: Optional[str],
-                                 pre_reshape_lengths: Optional[Dict],
-                                 post_reshape_pattern: Optional[str],
-                                 post_reshape_lengths: Optional[Dict],
-                                 ):
+    def _create_rearrange_layers(
+        self,
+        pre_reshape_pattern: Optional[str],
+        pre_reshape_lengths: Optional[Dict],
+        post_reshape_pattern: Optional[str],
+        post_reshape_lengths: Optional[Dict],
+    ):
         self.pre_rearrange = None
         if pre_reshape_pattern is not None:
             self.pre_rearrange = Rearrange(pre_reshape_pattern, **cast(dict, pre_reshape_lengths))
 
         self.post_rearrange = None
         if post_reshape_pattern is not None:
             self.post_rearrange = Rearrange(post_reshape_pattern, **cast(dict, post_reshape_lengths))
 
-    def build(self, input_shape):
-        pass
-
-    def call(self, inputs):
+    def forward(self, input):
         if self.pre_rearrange is not None:
-            inputs = self.pre_rearrange(inputs)
-        result = tf.einsum(self.einsum_pattern, inputs, self.weight)
+            input = self.pre_rearrange(input)
+        result = torch.einsum(self.einsum_pattern, input, self.weight)
         if self.bias is not None:
-            result = result + self.bias
+            result += self.bias
         if self.post_rearrange is not None:
             result = self.post_rearrange(result)
         return result
-
-    def get_config(self):
-        return {'pattern': self.pattern,
-                'weight_shape': self.weight_shape,
-                'bias_shape': self.bias_shape,
-                **self.axes_lengths}
```

### Comparing `einops-0.7.0rc2/scripts/convert_readme.py` & `einops-0.8.0/scripts/convert_readme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """
 Converts readme from github repo page to mkdocs-friendly
 """
+
 from pathlib import Path
 
-original_text = Path(__file__).parent.parent.joinpath('README.md').read_text(encoding='utf-8')
+original_text = Path(__file__).parent.parent.joinpath("README.md").read_text(encoding="utf-8")
 
 
 def replace_with_video_tag(line: str):
-    if line.startswith('https://') and line.endswith('.mp4') and ' ' not in line:
+    if line.startswith("https://") and line.endswith(".mp4") and " " not in line:
         # treating as link to mp4 file.
         return ""
         # return f"""
         # <video width="800" controls><source src="{line}" type="video/mp4">
         # Your browser does not support the video </video>\n\n<br />\n\n<br />
         # """.strip()
     else:
         # other lines are not touched
         return line
 
 
-new_content = '\n'.join([
-    replace_with_video_tag(line)
-    for line in original_text.splitlines()
-])
+new_content = "\n".join([replace_with_video_tag(line) for line in original_text.splitlines()])
 # save contents
-docs_index = Path(__file__).parent.parent.joinpath('docs_src', 'index.md')
+docs_index = Path(__file__).parent.parent.joinpath("docs_src", "index.md")
 assert docs_index.parent.exists()
-docs_index.write_bytes(
-    new_content.encode('utf-8')
-)
-print('Converted README.md')
+docs_index.write_bytes(new_content.encode("utf-8"))
+print("Converted README.md")
```

### Comparing `einops-0.7.0rc2/scripts/setup.py` & `einops-0.8.0/scripts/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 This is a fake script, it is not used.
 Seems github does not count contributions unless you have a setup.py
 """
+
 __author__ = "Alex Rogozhnikov"
 
 from setuptools import setup
 
 setup(
     name="einops",
-    version="0.7.0rc2",
+    version="0.7.0",
     description="A new flavour of deep learning operations",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/arogozhnikov/einops",
     author="Alex Rogozhnikov",
     classifiers=[
         "Intended Audience :: Science/Research",
```

### Comparing `einops-0.7.0rc2/tests/__init__.py` & `einops-0.8.0/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 __author__ = "Alex Rogozhnikov"
 
 
 # minimize noise in tests logging
 logging.getLogger("tensorflow").disabled = True
 logging.getLogger("matplotlib").disabled = True
 
+FLOAT_REDUCTIONS = ("min", "max", "sum", "mean", "prod")  # not includes any/all
+
 
 def find_names_of_all_frameworks() -> List[str]:
     backend_subclasses = []
     backends = _backends.AbstractBackend.__subclasses__()
     while backends:
         backend = backends.pop()
         backends += backend.__subclasses__()
@@ -35,17 +37,18 @@
     _known_backends = find_names_of_all_frameworks()
     for backend_name in parsed_backends:
         if backend_name not in _known_backends:
             raise RuntimeError(f"Unknown framework: {backend_name}")
 
     return parsed_backends
 
+
 def is_backend_tested(backend: str) -> bool:
     if backend not in find_names_of_all_frameworks():
-        raise RuntimeError(f'Unknown framework {backend}')
+        raise RuntimeError(f"Unknown framework {backend}")
     return backend in parse_backends_to_test()
 
 
 def unparse_backends(backend_names: List[str]) -> Tuple[str, str]:
     _known_backends = find_names_of_all_frameworks()
     for backend_name in backend_names:
         if backend_name not in _known_backends:
@@ -79,15 +82,15 @@
                 _backends.PaddleBackend,
             ]
     else:
         if not layers:
             backend_types = []
         else:
             backend_types = [
-                _backends.KerasBackend,
+                _backends.TFKerasBackend,
             ]
 
     backend_names_to_test = parse_backends_to_test()
     result = []
     for backend_type in backend_types:
         if backend_type.framework_name not in backend_names_to_test:
             continue
```

### Comparing `einops-0.7.0rc2/tests/test_einsum.py` & `einops-0.8.0/tests/test_einsum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Any, Callable
-from venv import create
 from . import collect_test_backends
 from einops.einops import _compactify_pattern_for_einsum, einsum, EinopsError
 import numpy as np
 import pytest
 import string
 
 
@@ -14,35 +13,35 @@
 
     def __call__(self, function: Callable):
         return function(*self.args, **self.kwargs)
 
 
 test_layer_cases = [
     (
-        Arguments('b c_in h w -> w c_out h b', 'c_in c_out', bias_shape=None, c_out=13, c_in=12),
+        Arguments("b c_in h w -> w c_out h b", "c_in c_out", bias_shape=None, c_out=13, c_in=12),
         (2, 12, 3, 4),
         (4, 13, 3, 2),
     ),
     (
-        Arguments('b c_in h w -> w c_out h b', 'c_in c_out', bias_shape='c_out', c_out=13, c_in=12),
+        Arguments("b c_in h w -> w c_out h b", "c_in c_out", bias_shape="c_out", c_out=13, c_in=12),
         (2, 12, 3, 4),
         (4, 13, 3, 2),
     ),
     (
-        Arguments('b c_in h w -> w c_in h b', '', bias_shape=None, c_in=12),
+        Arguments("b c_in h w -> w c_in h b", "", bias_shape=None, c_in=12),
         (2, 12, 3, 4),
         (4, 12, 3, 2),
     ),
     (
-        Arguments('b c_in h w -> b c_out', 'c_in h w c_out', bias_shape=None, c_in=12, h=3, w=4, c_out=5),
+        Arguments("b c_in h w -> b c_out", "c_in h w c_out", bias_shape=None, c_in=12, h=3, w=4, c_out=5),
         (2, 12, 3, 4),
         (2, 5),
     ),
     (
-        Arguments('b t head c_in -> b t head c_out', 'head c_in c_out', bias_shape=None, head=4, c_in=5, c_out=6),
+        Arguments("b t head c_in -> b t head c_out", "head c_in c_out", bias_shape=None, head=4, c_in=5, c_out=6),
         (2, 3, 4, 5),
         (2, 3, 4, 6),
     ),
 ]
 
 
 # Each of the form:
@@ -163,115 +162,114 @@
         (()),
     ),
 ]
 
 
 def test_layer():
     for backend in collect_test_backends(layers=True, symbolic=False):
-        if backend.framework_name in ['tensorflow', 'torch', 'chainer', 'oneflow', 'paddle']:
+        if backend.framework_name in ["tensorflow", "torch", "chainer", "oneflow", "paddle"]:
             layer_type = backend.layers().EinMix
             for args, in_shape, out_shape in test_layer_cases:
                 layer = args(layer_type)
-                print('Running', layer.einsum_pattern, 'for', backend.framework_name)
-                input = np.random.uniform(size=in_shape).astype('float32')
+                print("Running", layer.einsum_pattern, "for", backend.framework_name)
+                input = np.random.uniform(size=in_shape).astype("float32")
                 input_framework = backend.from_numpy(input)
                 output_framework = layer(input_framework)
                 output = backend.to_numpy(output_framework)
                 assert output.shape == out_shape
 
 
-valid_backends_functional = ['tensorflow', 'torch', 'jax', 'numpy',
-                             'chainer', 'oneflow', 'cupy', 'tensorflow.keras', 'paddle']
+valid_backends_functional = [
+    "tensorflow",
+    "torch",
+    "jax",
+    "numpy",
+    "chainer",
+    "oneflow",
+    "cupy",
+    "tensorflow.keras",
+    "paddle",
+]
+
 
 def test_functional():
     # Functional tests:
-    backends = filter(lambda x: x.framework_name in valid_backends_functional,
-                      collect_test_backends())
+    backends = filter(lambda x: x.framework_name in valid_backends_functional, collect_test_backends())
     for backend in backends:
         for einops_pattern, true_pattern, in_shapes, out_shape in test_functional_cases:
             print(f"Running '{einops_pattern}' for {backend.framework_name}")
-            
+
             # Create pattern:
             predicted_pattern = _compactify_pattern_for_einsum(einops_pattern)
             assert predicted_pattern == true_pattern
 
             # Generate example data:
             rstate = np.random.RandomState(0)
-            in_arrays = [
-                rstate.uniform(size=shape).astype('float32')
-                for shape in in_shapes
-            ]
-            in_arrays_framework = [
-                backend.from_numpy(array) for array in in_arrays
-            ]
-            
+            in_arrays = [rstate.uniform(size=shape).astype("float32") for shape in in_shapes]
+            in_arrays_framework = [backend.from_numpy(array) for array in in_arrays]
+
             # Loop over whether we call it manually with the backend,
             # or whether we use `einops.einsum`.
             for do_manual_call in [True, False]:
                 # Actually run einsum:
                 if do_manual_call:
                     out_array = backend.einsum(predicted_pattern, *in_arrays_framework)
                 else:
                     out_array = einsum(*in_arrays_framework, einops_pattern)
 
                 # Check shape:
                 if tuple(out_array.shape) != out_shape:
-                    raise ValueError(
-                        f"Expected output shape {out_shape} but got {out_array.shape}"
-                    )
+                    raise ValueError(f"Expected output shape {out_shape} but got {out_array.shape}")
 
                 # Check values:
                 true_out_array = np.einsum(true_pattern, *in_arrays)
                 predicted_out_array = backend.to_numpy(out_array)
-                np.testing.assert_array_almost_equal(predicted_out_array,
-                                                        true_out_array,
-                                                        decimal=5)
+                np.testing.assert_array_almost_equal(predicted_out_array, true_out_array, decimal=5)
 
 
 def test_functional_symbolic():
-    backends = filter(lambda x: x.framework_name in valid_backends_functional,
-                      collect_test_backends(symbolic=True, layers=False))
+    backends = filter(
+        lambda x: x.framework_name in valid_backends_functional, collect_test_backends(symbolic=True, layers=False)
+    )
     for backend in backends:
         for einops_pattern, true_pattern, in_shapes, out_shape in test_functional_cases:
             print(f"Running '{einops_pattern}' for symbolic {backend.framework_name}")
             # Create pattern:
             predicted_pattern = _compactify_pattern_for_einsum(einops_pattern)
             assert predicted_pattern == true_pattern
 
             rstate = np.random.RandomState(0)
             in_syms = [backend.create_symbol(in_shape) for in_shape in in_shapes]
-            in_data = [rstate.uniform(size=in_shape).astype('float32') for in_shape in in_shapes]
+            in_data = [rstate.uniform(size=in_shape).astype("float32") for in_shape in in_shapes]
 
             expected_out_data = np.einsum(true_pattern, *in_data)
 
             for do_manual_call in [True, False]:
                 if do_manual_call:
                     predicted_out_symbol = backend.einsum(predicted_pattern, *in_syms)
                 else:
                     predicted_out_symbol = einsum(*in_syms, einops_pattern)
 
                 predicted_out_data = backend.eval_symbol(
                     predicted_out_symbol,
                     list(zip(in_syms, in_data)),
                 )
                 if predicted_out_data.shape != out_shape:
-                    raise ValueError(
-                        f"Expected output shape {out_shape} but got {predicted_out_data.shape}"
-                    )
-                assert np.testing.assert_array_almost_equal(predicted_out_data,
-                                                            expected_out_data,
-                                                            decimal=5)
+                    raise ValueError(f"Expected output shape {out_shape} but got {predicted_out_data.shape}")
+                assert np.testing.assert_array_almost_equal(predicted_out_data, expected_out_data, decimal=5)
 
 
 def test_functional_errors():
     # Specific backend does not matter, as errors are raised
     # during the pattern creation.
 
     rstate = np.random.RandomState(0)
-    create_tensor = lambda *shape: rstate.uniform(size=shape).astype('float32')
+
+    def create_tensor(*shape):
+        return rstate.uniform(size=shape).astype("float32")
 
     # raise NotImplementedError("Singleton () axes are not yet supported in einsum.")
     with pytest.raises(NotImplementedError, match="^Singleton"):
         einsum(
             create_tensor(5, 1),
             "i () -> i",
         )
```

### Comparing `einops-0.7.0rc2/tests/test_examples.py` & `einops-0.8.0/tests/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,257 +5,293 @@
 from tests import is_backend_tested
 from tests.test_ops import imp_op_backends
 
 
 def test_rearrange_examples():
     def test1(x):
         # transpose
-        y = rearrange(x, 'b c h w -> b h w c')
+        y = rearrange(x, "b c h w -> b h w c")
         assert tuple(y.shape) == (10, 30, 40, 20)
         return y
 
     def test2(x):
         # view / reshape
-        y = rearrange(x, 'b c h w -> b (c h w)')
+        y = rearrange(x, "b c h w -> b (c h w)")
         assert tuple(y.shape) == (10, 20 * 30 * 40)
         return y
 
     def test3(x):
         # depth-to-space
-        y = rearrange(x, 'b (c h1 w1) h w -> b c (h h1) (w w1)', h1=2, w1=2)
+        y = rearrange(x, "b (c h1 w1) h w -> b c (h h1) (w w1)", h1=2, w1=2)
         assert tuple(y.shape) == (10, 5, 30 * 2, 40 * 2)
         return y
 
     def test4(x):
         # space-to-depth
-        y = rearrange(x, 'b c (h h1) (w w1) -> b (h1 w1 c) h w', h1=2, w1=2)
+        y = rearrange(x, "b c (h h1) (w w1) -> b (h1 w1 c) h w", h1=2, w1=2)
         assert tuple(y.shape) == (10, 20 * 4, 30 // 2, 40 // 2)
         return y
 
     def test5(x):
         # simple transposition
-        y = rearrange(x, 'b1 sound b2 letter -> b1 b2 sound letter')
+        y = rearrange(x, "b1 sound b2 letter -> b1 b2 sound letter")
         assert tuple(y.shape) == (10, 30, 20, 40)
         return y
 
     def test6(x):
         # parsing parameters
-        t = rearrange(x, 'b c h w -> (b h w) c')
+        t = rearrange(x, "b c h w -> (b h w) c")
         t = t[:, ::2]  # replacement for dot-product, just changes size of second axis
         assert tuple(t.shape) == (10 * 30 * 40, 10)
 
-        y = rearrange(t, '(b h w) c2 -> b c2 h w', **parse_shape(x, 'b _ h w'))
+        y = rearrange(t, "(b h w) c2 -> b c2 h w", **parse_shape(x, "b _ h w"))
         assert tuple(y.shape) == (10, 10, 30, 40)
         return y
 
     def test7(x):
         # split of embedding into groups
-        y1, y2 = rearrange(x, 'b (c g) h w -> g b c h w', g=2)
+        y1, y2 = rearrange(x, "b (c g) h w -> g b c h w", g=2)
         assert tuple(y1.shape) == (10, 10, 30, 40)
         assert tuple(y2.shape) == (10, 10, 30, 40)
         return y1 + y2  # only one tensor is expected in output
 
     def test8(x):
         # max-pooling
-        y = reduce(x, 'b c (h h1) (w w1) -> b c h w', reduction='max', h1=2, w1=2)
+        y = reduce(x, "b c (h h1) (w w1) -> b c h w", reduction="max", h1=2, w1=2)
         assert tuple(y.shape) == (10, 20, 30 // 2, 40 // 2)
         return y
 
     def test9(x):
         # squeeze - unsqueeze
-        y = reduce(x, 'b c h w -> b c () ()', reduction='max')
+        y = reduce(x, "b c h w -> b c () ()", reduction="max")
         assert tuple(y.shape) == (10, 20, 1, 1)
-        y = rearrange(y, 'b c () () -> c b')
+        y = rearrange(y, "b c () () -> c b")
         assert tuple(y.shape) == (20, 10)
         return y
 
     def test10(x):
         # stack
         tensors = list(x + 0)  # 0 is needed https://github.com/tensorflow/tensorflow/issues/23185
-        tensors = rearrange(tensors, 'b c h w -> b h w c')
+        tensors = rearrange(tensors, "b c h w -> b h w c")
         assert tuple(tensors.shape) == (10, 30, 40, 20)
         return tensors
 
     def test11(x):
         # concatenate
         tensors = list(x + 0)  # 0 is needed https://github.com/tensorflow/tensorflow/issues/23185
-        tensors = rearrange(tensors, 'b c h w -> h (b w) c')
+        tensors = rearrange(tensors, "b c h w -> h (b w) c")
         assert tuple(tensors.shape) == (30, 10 * 40, 20)
         return tensors
 
     def shufflenet(x, convolve, c1, c2):
         # shufflenet reordering example
         x = convolve(x)
-        x = rearrange(x, 'b (c1 c2) h w-> b (c2 c1) h w', c1=c1, c2=c2)
+        x = rearrange(x, "b (c1 c2) h w-> b (c2 c1) h w", c1=c1, c2=c2)
         x = convolve(x)
         return x
 
     def convolve_strided_1d(x, stride, usual_convolution):
-        x = rearrange(x, 'b c t1 t2 -> b c (t1 t2)')  # reduce dimensionality
-        x = rearrange(x, 'b c (t stride) -> (stride b) c t', stride=stride)
+        x = rearrange(x, "b c t1 t2 -> b c (t1 t2)")  # reduce dimensionality
+        x = rearrange(x, "b c (t stride) -> (stride b) c t", stride=stride)
         x = usual_convolution(x)
-        x = rearrange(x, '(stride b) c t -> b c (t stride)', stride=stride)
+        x = rearrange(x, "(stride b) c t -> b c (t stride)", stride=stride)
         return x
 
     def convolve_strided_2d(x, h_stride, w_stride, usual_convolution):
-        x = rearrange(x, 'b c (h hs) (w ws) -> (hs ws b) c h w', hs=h_stride, ws=w_stride)
+        x = rearrange(x, "b c (h hs) (w ws) -> (hs ws b) c h w", hs=h_stride, ws=w_stride)
         x = usual_convolution(x)
-        x = rearrange(x, '(hs ws b) c h w -> b c (h hs) (w ws)', hs=h_stride, ws=w_stride)
+        x = rearrange(x, "(hs ws b) c h w -> b c (h hs) (w ws)", hs=h_stride, ws=w_stride)
         return x
 
     def unet_like_1d(x, usual_convolution):
         # u-net like steps for increasing / reducing dimensionality
-        x = rearrange(x, 'b c t1 t2 -> b c (t1 t2)')  # reduce dimensionality
-        y = rearrange(x, 'b c (t dt) -> b (dt c) t', dt=2)
+        x = rearrange(x, "b c t1 t2 -> b c (t1 t2)")  # reduce dimensionality
+        y = rearrange(x, "b c (t dt) -> b (dt c) t", dt=2)
         y = usual_convolution(y)
-        x = x + rearrange(y, 'b (dt c) t -> b c (t dt)', dt=2)
+        x = x + rearrange(y, "b (dt c) t -> b c (t dt)", dt=2)
         return x
 
     # mock for convolution (works for all backends)
-    convolve_mock = lambda x: x
+    def convolve_mock(x):
+        return x
 
-    tests = [test1, test2, test3, test4, test5, test6, test7, test8, test9, test10, test11,
-             lambda x: shufflenet(x, convolve=convolve_mock, c1=4, c2=5),
-             lambda x: convolve_strided_1d(x, stride=2, usual_convolution=convolve_mock),
-             lambda x: convolve_strided_2d(x, h_stride=2, w_stride=2, usual_convolution=convolve_mock),
-             lambda x: unet_like_1d(x, usual_convolution=convolve_mock),
-             ]
+    tests = [
+        test1,
+        test2,
+        test3,
+        test4,
+        test5,
+        test6,
+        test7,
+        test8,
+        test9,
+        test10,
+        test11,
+        lambda x: shufflenet(x, convolve=convolve_mock, c1=4, c2=5),
+        lambda x: convolve_strided_1d(x, stride=2, usual_convolution=convolve_mock),
+        lambda x: convolve_strided_2d(x, h_stride=2, w_stride=2, usual_convolution=convolve_mock),
+        lambda x: unet_like_1d(x, usual_convolution=convolve_mock),
+    ]
 
     for backend in imp_op_backends:
-        print('testing source_examples for ', backend.framework_name)
+        print("testing source_examples for ", backend.framework_name)
         for test in tests:
             x = numpy.arange(10 * 20 * 30 * 40).reshape([10, 20, 30, 40])
             result1 = test(x)
             result2 = backend.to_numpy(test(backend.from_numpy(x)))
             assert numpy.array_equal(result1, result2)
 
             # now with strides
             x = numpy.arange(10 * 2 * 20 * 3 * 30 * 1 * 40).reshape([10 * 2, 20 * 3, 30 * 1, 40 * 1])
             # known torch bug - torch doesn't support negative steps
-            last_step = -1 if (backend.framework_name != 'torch' and backend.framework_name != 'oneflow') else 1
+            last_step = -1 if (backend.framework_name != "torch" and backend.framework_name != "oneflow") else 1
             indexing_expression = numpy.index_exp[::2, ::3, ::1, ::last_step]
             result1 = test(x[indexing_expression])
             result2 = backend.to_numpy(test(backend.from_numpy(x)[indexing_expression]))
             assert numpy.array_equal(result1, result2)
 
 
 def tensor_train_example_numpy():
     # kept here just for a collection, only tested for numpy
     # https://arxiv.org/pdf/1509.06569.pdf, (5)
     x = numpy.ones([3, 4, 5, 6])
     rank = 4
-    if numpy.__version__ < '1.15.0':
+    if numpy.__version__ < "1.15.0":
         # numpy.einsum fails here, skip test
         return
     # creating appropriate Gs
     Gs = [numpy.ones([d, d, rank, rank]) for d in x.shape]
     Gs[0] = Gs[0][:, :, :1, :]
     Gs[-1] = Gs[-1][:, :, :, :1]
 
     # einsum way
     y = x.reshape((1,) + x.shape)
     for G in Gs:
         # taking partial results left-to-right
         # y = numpy.einsum('i j alpha beta, alpha i ...  -> beta ... j', G, y)
-        y = numpy.einsum('i j a b, a i ...  -> b ... j', G, y)
+        y = numpy.einsum("i j a b, a i ...  -> b ... j", G, y)
     y1 = y.reshape(-1)
 
     # alternative way
     y = x.reshape(-1)
     for G in Gs:
         i, j, alpha, beta = G.shape
-        y = rearrange(y, '(i rest alpha) -> rest (alpha i)', alpha=alpha, i=i)
-        y = y @ rearrange(G, 'i j alpha beta -> (alpha i) (j beta)')
-        y = rearrange(y, 'rest (beta j) -> (beta rest j)', beta=beta, j=j)
+        y = rearrange(y, "(i rest alpha) -> rest (alpha i)", alpha=alpha, i=i)
+        y = y @ rearrange(G, "i j alpha beta -> (alpha i) (j beta)")
+        y = rearrange(y, "rest (beta j) -> (beta rest j)", beta=beta, j=j)
     y2 = y
     assert numpy.allclose(y1, y2)
 
     # yet another way
     y = x
     for G in Gs:
         i, j, alpha, beta = G.shape
-        y = rearrange(y, 'i ... (j alpha) -> ... j (alpha i)', alpha=alpha, i=i)
-        y = y @ rearrange(G, 'i j alpha beta -> (alpha i) (j beta)')
+        y = rearrange(y, "i ... (j alpha) -> ... j (alpha i)", alpha=alpha, i=i)
+        y = y @ rearrange(G, "i j alpha beta -> (alpha i) (j beta)")
     y3 = y.reshape(-1)
     assert numpy.allclose(y1, y3)
 
 
 def test_pytorch_yolo_fragment():
-    if not is_backend_tested('torch'):
+    if not is_backend_tested("torch"):
         pytest.skip()
 
     import torch
+
     def old_way(input, num_classes, num_anchors, anchors, stride_h, stride_w):
         # https://github.com/BobLiu20/YOLOv3_PyTorch/blob/c6b483743598b5f64d520d81e7e5f47ba936d4c9/nets/yolo_loss.py#L28-L44
         bs = input.size(0)
         in_h = input.size(2)
         in_w = input.size(3)
         scaled_anchors = [(a_w / stride_w, a_h / stride_h) for a_w, a_h in anchors]
 
-        prediction = input.view(bs, num_anchors,
-                                5 + num_classes, in_h, in_w).permute(0, 1, 3, 4, 2).contiguous()
+        prediction = input.view(bs, num_anchors, 5 + num_classes, in_h, in_w).permute(0, 1, 3, 4, 2).contiguous()
         # Get outputs
         x = torch.sigmoid(prediction[..., 0])  # Center x
         y = torch.sigmoid(prediction[..., 1])  # Center y
         w = prediction[..., 2]  # Width
         h = prediction[..., 3]  # Height
         conf = torch.sigmoid(prediction[..., 4])  # Conf
         pred_cls = torch.sigmoid(prediction[..., 5:])  # Cls pred.
 
         # https://github.com/BobLiu20/YOLOv3_PyTorch/blob/c6b483743598b5f64d520d81e7e5f47ba936d4c9/nets/yolo_loss.py#L70-L92
         FloatTensor = torch.cuda.FloatTensor if x.is_cuda else torch.FloatTensor
         LongTensor = torch.cuda.LongTensor if x.is_cuda else torch.LongTensor
         # Calculate offsets for each grid
-        grid_x = torch.linspace(0, in_w - 1, in_w).repeat(in_w, 1).repeat(
-            bs * num_anchors, 1, 1).view(x.shape).type(FloatTensor)
-        grid_y = torch.linspace(0, in_h - 1, in_h).repeat(in_h, 1).t().repeat(
-            bs * num_anchors, 1, 1).view(y.shape).type(FloatTensor)
+        grid_x = (
+            torch.linspace(0, in_w - 1, in_w)
+            .repeat(in_w, 1)
+            .repeat(bs * num_anchors, 1, 1)
+            .view(x.shape)
+            .type(FloatTensor)
+        )
+        grid_y = (
+            torch.linspace(0, in_h - 1, in_h)
+            .repeat(in_h, 1)
+            .t()
+            .repeat(bs * num_anchors, 1, 1)
+            .view(y.shape)
+            .type(FloatTensor)
+        )
         # Calculate anchor w, h
         anchor_w = FloatTensor(scaled_anchors).index_select(1, LongTensor([0]))
         anchor_h = FloatTensor(scaled_anchors).index_select(1, LongTensor([1]))
         anchor_w = anchor_w.repeat(bs, 1).repeat(1, 1, in_h * in_w).view(w.shape)
         anchor_h = anchor_h.repeat(bs, 1).repeat(1, 1, in_h * in_w).view(h.shape)
         # Add offset and scale with anchors
         pred_boxes = FloatTensor(prediction[..., :4].shape)
         pred_boxes[..., 0] = x.data + grid_x
         pred_boxes[..., 1] = y.data + grid_y
         pred_boxes[..., 2] = torch.exp(w.data) * anchor_w
         pred_boxes[..., 3] = torch.exp(h.data) * anchor_h
         # Results
         _scale = torch.Tensor([stride_w, stride_h] * 2).type(FloatTensor)
-        output = torch.cat((pred_boxes.view(bs, -1, 4) * _scale,
-                            conf.view(bs, -1, 1), pred_cls.view(bs, -1, num_classes)), -1)
+        output = torch.cat(
+            (pred_boxes.view(bs, -1, 4) * _scale, conf.view(bs, -1, 1), pred_cls.view(bs, -1, num_classes)), -1
+        )
         return output
 
     def new_way(input, num_classes, num_anchors, anchors, stride_h, stride_w):
-        raw_predictions = rearrange(input, ' b (anchor prediction) h w -> prediction b anchor h w', anchor=num_anchors)
+        raw_predictions = rearrange(input, " b (anchor prediction) h w -> prediction b anchor h w", anchor=num_anchors)
 
         anchors = torch.FloatTensor(anchors).to(input.device)
-        anchor_sizes = rearrange(anchors, 'anchor dim -> dim () anchor () ()')
+        anchor_sizes = rearrange(anchors, "anchor dim -> dim () anchor () ()")
 
         _, _, _, in_h, in_w = raw_predictions.shape
-        grid_h = rearrange(torch.arange(in_h).float(), 'h -> () () h ()').to(input.device)
-        grid_w = rearrange(torch.arange(in_w).float(), 'w -> () () () w').to(input.device)
+        grid_h = rearrange(torch.arange(in_h).float(), "h -> () () h ()").to(input.device)
+        grid_w = rearrange(torch.arange(in_w).float(), "w -> () () () w").to(input.device)
 
         predicted_bboxes = torch.zeros_like(raw_predictions)
         predicted_bboxes[0] = (raw_predictions[0].sigmoid() + grid_h) * stride_h  # center y
         predicted_bboxes[1] = (raw_predictions[1].sigmoid() + grid_w) * stride_w  # center x
         predicted_bboxes[2:4] = (raw_predictions[2:4].exp()) * anchor_sizes  # bbox width and height
         predicted_bboxes[4] = raw_predictions[4].sigmoid()  # confidence
         predicted_bboxes[5:] = raw_predictions[5:].sigmoid()  # class predictions
         # only to match results of original code, not needed
-        return rearrange(predicted_bboxes, 'prediction b anchor h w -> b anchor h w prediction')
+        return rearrange(predicted_bboxes, "prediction b anchor h w -> b anchor h w prediction")
 
     stride_h = 4
     stride_w = 4
     batch_size = 5
     num_classes = 12
     anchors = [[50, 100], [100, 50], [75, 75]]
     num_anchors = len(anchors)
 
     input = torch.randn([batch_size, num_anchors * (5 + num_classes), 1, 1])
-    result1 = old_way(input=input, num_anchors=num_anchors, num_classes=num_classes,
-                      stride_h=stride_h, stride_w=stride_w, anchors=anchors)
-    result2 = new_way(input=input, num_anchors=num_anchors, num_classes=num_classes,
-                      stride_h=stride_h, stride_w=stride_w, anchors=anchors)
+    result1 = old_way(
+        input=input,
+        num_anchors=num_anchors,
+        num_classes=num_classes,
+        stride_h=stride_h,
+        stride_w=stride_w,
+        anchors=anchors,
+    )
+    result2 = new_way(
+        input=input,
+        num_anchors=num_anchors,
+        num_classes=num_classes,
+        stride_h=stride_h,
+        stride_w=stride_w,
+        anchors=anchors,
+    )
     result1 = result1.reshape(result2.shape)
-    assert torch.allclose(result1, result2)
+    assert torch.allclose(result1, result2)
```

### Comparing `einops-0.7.0rc2/tests/test_layers.py` & `einops-0.8.0/tests/test_layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import tempfile
 from collections import namedtuple
 
 import numpy
 import pytest
 
 from einops import rearrange, reduce
-from einops.einops import _reductions
-from . import collect_test_backends, is_backend_tested
+from . import collect_test_backends, is_backend_tested, FLOAT_REDUCTIONS as REDUCTIONS
 
 __author__ = "Alex Rogozhnikov"
 
 testcase = namedtuple("testcase", ["pattern", "axes_lengths", "input_shape", "wrong_shapes"])
 
 rearrangement_patterns = [
     testcase(
@@ -42,15 +41,15 @@
         for pattern, axes_lengths, input_shape, wrong_shapes in rearrangement_patterns:
             x = numpy.arange(numpy.prod(input_shape), dtype="float32").reshape(input_shape)
             result_numpy = rearrange(x, pattern, **axes_lengths)
             layer = backend.layers().Rearrange(pattern, **axes_lengths)
             for shape in wrong_shapes:
                 try:
                     layer(backend.from_numpy(numpy.zeros(shape, dtype="float32")))
-                except:
+                except BaseException:
                     pass
                 else:
                     raise AssertionError("Failure expected")
 
             # simple pickling / unpickling
             layer2 = pickle.loads(pickle.dumps(layer))
             result1 = backend.to_numpy(layer(backend.from_numpy(x)))
@@ -106,25 +105,25 @@
     testcase("b ... c -> b", dict(b=10), (10, 20, 30, 40), [(10,), (11, 10)]),
 ]
 
 
 def test_reduce_imperative():
     for backend in collect_test_backends(symbolic=False, layers=True):
         print("Test layer for ", backend.framework_name)
-        for reduction in _reductions:
+        for reduction in REDUCTIONS:
             for pattern, axes_lengths, input_shape, wrong_shapes in reduction_patterns:
                 print(backend, reduction, pattern, axes_lengths, input_shape, wrong_shapes)
                 x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype="float32").reshape(input_shape)
                 x /= x.mean()
                 result_numpy = reduce(x, pattern, reduction, **axes_lengths)
                 layer = backend.layers().Reduce(pattern, reduction, **axes_lengths)
                 for shape in wrong_shapes:
                     try:
                         layer(backend.from_numpy(numpy.zeros(shape, dtype="float32")))
-                    except:
+                    except BaseException:
                         pass
                     else:
                         raise AssertionError("Failure expected")
 
                 # simple pickling / unpickling
                 layer2 = pickle.loads(pickle.dumps(layer))
                 result1 = backend.to_numpy(layer(backend.from_numpy(x)))
@@ -147,15 +146,15 @@
                     assert numpy.all(numpy.in1d(grad, [0, 1]))
                     assert numpy.sum(grad) > 0.5
 
 
 def test_reduce_symbolic():
     for backend in collect_test_backends(symbolic=True, layers=True):
         print("Test layer for ", backend.framework_name)
-        for reduction in _reductions:
+        for reduction in REDUCTIONS:
             for pattern, axes_lengths, input_shape, wrong_shapes in reduction_patterns:
                 x = numpy.arange(1, 1 + numpy.prod(input_shape), dtype="float32").reshape(input_shape)
                 x /= x.mean()
                 result_numpy = reduce(x, pattern, reduction, **axes_lengths)
                 layer = backend.layers().Reduce(pattern, reduction, **axes_lengths)
                 input_shape_of_nones = [None] * len(input_shape)
                 shapes = [input_shape, input_shape_of_nones]
@@ -241,14 +240,18 @@
 
 
 def test_keras_layer():
     if not is_backend_tested("tensorflow"):
         pytest.skip()
     else:
         import tensorflow as tf
+
+        if tf.__version__ < "2.16.":
+            # current implementation of layers follows new TF interface
+            pytest.skip()
         from tensorflow.keras.models import Sequential
         from tensorflow.keras.layers import Conv2D as Conv2d, Dense as Linear, ReLU
         from einops.layers.keras import Rearrange, Reduce, EinMix, keras_custom_objects
 
         def create_keras_model():
             return Sequential(
                 [
@@ -265,33 +268,39 @@
                     EinMix("(b c2) -> b c3", weight_shape="c2 c3", bias_shape="c3", c2=84, c3=84),
                     Linear(10),
                 ]
             )
 
         model1 = create_keras_model()
         model2 = create_keras_model()
+
         input = numpy.random.normal(size=[10, 32, 32, 3]).astype("float32")
+        # two randomly init models should provide different outputs
         assert not numpy.allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
 
         # get some temp filename
-        with tempfile.NamedTemporaryFile(mode="r+b") as f:
-            tmp_filename = f.name
+        tmp_model_filename = "/tmp/einops_tf_model.h5"
         # save arch + weights
-        print("temp_path_keras1", tmp_filename)
-        tf.keras.models.save_model(model1, tmp_filename)
-        model3 = tf.keras.models.load_model(tmp_filename, custom_objects=keras_custom_objects)
-        assert numpy.allclose(model1.predict_on_batch(input), model3.predict_on_batch(input))
+        print("temp_path_keras1", tmp_model_filename)
+        tf.keras.models.save_model(model1, tmp_model_filename)
+        model3 = tf.keras.models.load_model(tmp_model_filename, custom_objects=keras_custom_objects)
 
+        numpy.testing.assert_allclose(model1.predict_on_batch(input), model3.predict_on_batch(input))
+
+        weight_filename = "/tmp/einops_tf_model.weights.h5"
         # save arch as json
         model4 = tf.keras.models.model_from_json(model1.to_json(), custom_objects=keras_custom_objects)
-        model1.save_weights(tmp_filename)
-        model4.load_weights(tmp_filename)
-        model2.load_weights(tmp_filename)
-        assert numpy.allclose(model1.predict_on_batch(input), model4.predict_on_batch(input))
-        assert numpy.allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
+        model1.save_weights(weight_filename)
+        model4.load_weights(weight_filename)
+        model2.load_weights(weight_filename)
+        # check that differently-inialized model receives same weights
+        numpy.testing.assert_allclose(model1.predict_on_batch(input), model2.predict_on_batch(input))
+        # ulimate test
+        # save-load architecture, and then load weights - should return same result
+        numpy.testing.assert_allclose(model1.predict_on_batch(input), model4.predict_on_batch(input))
 
 
 def test_chainer_layer():
     chainer_is_present = any(
         "chainer" in backend.framework_name for backend in collect_test_backends(symbolic=False, layers=True)
     )
     if chainer_is_present:
@@ -356,15 +365,17 @@
                 x = Rearrange("b h w c -> b (w h c)", sizes=dict(c=5))(x)
                 x = Reduce("b hwc -> b", "mean", dict(hwc=2 * 3 * 5))(x)
                 return x
 
         model = NN()
         fixed_input = jnp.ones([10, 2 * 2, 3 * 3, 4])
         params = model.init(jax.random.PRNGKey(0), fixed_input)
-        eval_at_point = lambda params: jnp.linalg.norm(model.apply(params, fixed_input))
+
+        def eval_at_point(params):
+            return jnp.linalg.norm(model.apply(params, fixed_input))
 
         vandg = jax.value_and_grad(eval_at_point)
         value0 = eval_at_point(params)
         value1, grad1 = vandg(params)
         assert jnp.allclose(value0, value1)
 
         params2 = jax.tree_map(lambda x1, x2: x1 - x2 * 0.001, params, grad1)
```

### Comparing `einops-0.7.0rc2/tests/test_notebooks.py` & `einops-0.8.0/tests/test_notebooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
 from io import StringIO
 
-from tests import parse_backends_to_test, is_backend_tested
+from tests import is_backend_tested
 
 __author__ = "Alex Rogozhnikov"
 
 from pathlib import Path
 import nbformat
 import pytest
 from nbconvert.preprocessors import ExecutePreprocessor
@@ -17,18 +17,19 @@
     :param filename: notebook
     :param replacements: dictionary with text replacements done before executing
     :return: notebook, rendered as string
     """
     with filename.open("r") as f:
         nb_as_str = f.read()
     for original, replacement in replacements.items():
+        assert original in nb_as_str, f"not found in notebook: {original}"
         nb_as_str = nb_as_str.replace(original, replacement)
 
     nb = nbformat.read(StringIO(nb_as_str), nbformat.NO_CONVERT)
-    ep = ExecutePreprocessor(timeout=60, kernel_name="python3")
+    ep = ExecutePreprocessor(timeout=120, kernel_name="python3")
     ep.preprocess(nb, {"metadata": {"path": str(filename.parent.absolute())}})
 
     result_as_stream = StringIO()
     nbformat.write(nb, result_as_stream)
     return result_as_stream.getvalue()
```

### Comparing `einops-0.7.0rc2/tests/test_ops.py` & `einops-0.8.0/tests/test_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 
 import numpy
 import pytest
 
 from einops import EinopsError
-from einops.einops import rearrange, reduce, repeat, _enumerate_directions, _reductions
-from . import collect_test_backends, is_backend_tested
+from einops.einops import rearrange, reduce, repeat, _enumerate_directions
+from . import collect_test_backends, is_backend_tested, FLOAT_REDUCTIONS as REDUCTIONS
 
 imp_op_backends = collect_test_backends(symbolic=False, layers=False)
 sym_op_backends = collect_test_backends(symbolic=True, layers=False)
 
 identity_patterns = [
     "...->...",
     "a b c d e-> a b c d e",
@@ -199,15 +199,15 @@
 
         assert numpy.array_equal(result, expected_result)
 
 
 def test_reduction_imperatives():
     for backend in imp_op_backends:
         print("Reduction tests for ", backend.framework_name)
-        for reduction in _reductions:
+        for reduction in REDUCTIONS:
             # slight redundancy for simpler order - numpy version is evaluated multiple times
             input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype="int64").reshape([2, 3, 4, 5, 6])
             if reduction in ["mean", "prod"]:
                 input = input / input.astype("float64").mean()
             test_cases = [
                 ["a b c d e -> ", {}, getattr(input, reduction)()],
                 ["a ... -> ", {}, getattr(input, reduction)()],
@@ -235,15 +235,15 @@
                 result = backend.to_numpy(result)
                 assert numpy.allclose(result, expected_result), f"Failed at {pattern}"
 
 
 def test_reduction_symbolic():
     for backend in sym_op_backends:
         print("Reduction tests for ", backend.framework_name)
-        for reduction in _reductions:
+        for reduction in REDUCTIONS:
             input = numpy.arange(2 * 3 * 4 * 5 * 6, dtype="int64").reshape([2, 3, 4, 5, 6])
             input = input / input.astype("float64").mean()
             # slight redundancy for simpler order - numpy version is evaluated multiple times
             test_cases = [
                 ["a b c d e -> ", {}, getattr(input, reduction)()],
                 ["a ... -> ", {}, getattr(input, reduction)()],
                 ["(a a2) ... (e e2) -> ", dict(a2=1, e2=1), getattr(input, reduction)()],
@@ -288,15 +288,15 @@
                     result = backend.eval_symbol(result_sym, [(sym, input)])
                     assert numpy.allclose(result, expected_numpy_result)
 
 
 def test_reduction_stress_imperatives():
     for backend in imp_op_backends:
         print("Stress-testing reduction for ", backend.framework_name)
-        for reduction in _reductions + ("rearrange",):
+        for reduction in REDUCTIONS + ("rearrange",):
             dtype = "int64"
             coincide = numpy.array_equal
             if reduction in ["mean", "prod"]:
                 dtype = "float64"
                 coincide = numpy.allclose
             max_dim = 11
             if "oneflow" in backend.framework_name:
@@ -347,21 +347,21 @@
         # very naive logsumexp to compare to
         minused = x.max(tuple_of_axes)
         y = x - x.max(tuple_of_axes, keepdims=True)
         y = numpy.exp(y)
         y = numpy.sum(y, axis=tuple_of_axes)
         return numpy.log(y) + minused
 
-    from einops._backends import TorchBackend, ChainerBackend, TensorflowBackend, KerasBackend, NumpyBackend
+    from einops._backends import TorchBackend, ChainerBackend, TensorflowBackend, TFKerasBackend, NumpyBackend
 
     backend2callback = {
         TorchBackend.framework_name: logsumexp_torch,
         ChainerBackend.framework_name: logsumexp_chainer,
         TensorflowBackend.framework_name: logsumexp_tf,
-        KerasBackend.framework_name: logsumexp_keras,
+        TFKerasBackend.framework_name: logsumexp_keras,
         NumpyBackend.framework_name: logsumexp_numpy,
     }
 
     for backend in imp_op_backends:
         if backend.framework_name not in backend2callback:
             continue
 
@@ -409,15 +409,17 @@
                 result1 = rearrange(arrays1, "b ... -> ... b")
                 result2 = rearrange(arrays2, "b ... -> ... b")
                 assert numpy.array_equal(result1, backend.to_numpy(result2))
 
 
 def test_gradients_imperatives():
     # lazy - just checking reductions
-    for reduction in _reductions:
+    for reduction in REDUCTIONS:
+        if reduction in ("any", "all"):
+            continue  # non-differentiable ops
         x = numpy.arange(1, 1 + 2 * 3 * 4).reshape([2, 3, 4]).astype("float32")
         results = {}
         for backend in imp_op_backends:
             y0 = backend.from_numpy(x)
             if not hasattr(y0, "grad"):
                 continue
 
@@ -581,27 +583,67 @@
     )
 
 
 def test_torch_compile_with_dynamic_shape():
     if not is_backend_tested("torch"):
         pytest.skip()
     import torch
+
     # somewhat reasonable debug messages
     torch._dynamo.config.verbose = True
+
     def func1(x):
         # test contains ellipsis
         a, b, c, *other = x.shape
-        x = rearrange(x, '(a a2) b c ... -> b (c a2) (a ...)', a2=2)
+        x = rearrange(x, "(a a2) b c ... -> b (c a2) (a ...)", a2=2)
         # test contains passing expression as axis length
-        x = reduce(x, 'b ca2 A -> b A', 'sum', ca2=c * 2)
+        x = reduce(x, "b ca2 A -> b A", "sum", ca2=c * 2)
         return x
 
     # seems can't test static and dynamic in the same test run.
     # func1_compiled_static = torch.compile(func1, dynamic=False, fullgraph=True, backend='aot_eager')
-    func1_compiled_dynamic = torch.compile(func1, dynamic=True, fullgraph=True, backend='aot_eager')
+    func1_compiled_dynamic = torch.compile(func1, dynamic=True, fullgraph=True, backend="aot_eager")
 
     x = torch.randn(size=[4, 5, 6, 3])
     assert torch.equal(func1_compiled_dynamic(x), func1(x))
     # check with input of different dimensionality, and with all shape elements changed
     x = torch.randn(size=[6, 3, 4, 2, 3])
     assert torch.equal(func1_compiled_dynamic(x), func1(x))
 
+
+def bit_count(x):
+    return sum((x >> i) & 1 for i in range(20))
+
+
+def test_reduction_imperatives_booleans():
+    """Checks that any/all reduction works in all frameworks"""
+    x_np = numpy.asarray([(bit_count(x) % 2) == 0 for x in range(2**6)]).reshape([2] * 6)
+    for backend in imp_op_backends:
+        if backend.framework_name == "chainer":
+            continue  # no support for bools
+        print("Reduction any/all tests for ", backend.framework_name)
+
+        for axis in range(6):
+            expected_result_any = numpy.any(x_np, axis=axis, keepdims=True)
+            expected_result_all = numpy.all(x_np, axis=axis, keepdims=True)
+            assert not numpy.array_equal(expected_result_any, expected_result_all)
+
+            axes = list("abcdef")
+            axes_in = list(axes)
+            axes_out = list(axes)
+            axes_out[axis] = "1"
+            pattern = (" ".join(axes_in)) + " -> " + (" ".join(axes_out))
+
+            res_any = reduce(backend.from_numpy(x_np), pattern, reduction="any")
+            res_all = reduce(backend.from_numpy(x_np), pattern, reduction="all")
+
+            assert numpy.array_equal(expected_result_any, backend.to_numpy(res_any))
+            assert numpy.array_equal(expected_result_all, backend.to_numpy(res_all))
+
+        # expected result: any/all
+        expected_result_any = numpy.any(x_np, axis=(0, 1), keepdims=True)
+        expected_result_all = numpy.all(x_np, axis=(0, 1), keepdims=True)
+        pattern = "a b ... -> 1 1 ..."
+        res_any = reduce(backend.from_numpy(x_np), pattern, reduction="any")
+        res_all = reduce(backend.from_numpy(x_np), pattern, reduction="all")
+        assert numpy.array_equal(expected_result_any, backend.to_numpy(res_any))
+        assert numpy.array_equal(expected_result_all, backend.to_numpy(res_all))
```

### Comparing `einops-0.7.0rc2/tests/test_other.py` & `einops-0.8.0/tests/test_other.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     for backend_type in AbstractBackend.__subclasses__():
         if backend_type.framework_name not in backends_to_test:
             continue
         try:
             # instantiate
             backend_type()
         except Exception as e:
-            errors.append(e)
+            errors.append((backend_type.framework_name, e))
     assert len(errors) == 0, errors
 
 
 def test_optimize_transformations_numpy():
     print("Testing optimizations")
     shapes = [[2] * n_dimensions for n_dimensions in range(14)]
     shapes += [[3] * n_dimensions for n_dimensions in range(6)]
@@ -117,34 +117,57 @@
     def test_repeating(self):
         with pytest.raises(einops.EinopsError):
             parse_shape(self.x, "a a b b")
 
         with pytest.raises(einops.EinopsError):
             parse_shape(self.backend.from_numpy(self.x), "a a b b")
 
-    @parameterized.expand(
-        [
+    def test_ellipsis(self):
+        for shape, pattern, expected in [
             ([10, 20], "...", dict()),
             ([10], "... a", dict(a=10)),
             ([10, 20], "... a", dict(a=20)),
             ([10, 20, 30], "... a", dict(a=30)),
             ([10, 20, 30, 40], "... a", dict(a=40)),
             ([10], "a ...", dict(a=10)),
             ([10, 20], "a ...", dict(a=10)),
             ([10, 20, 30], "a ...", dict(a=10)),
             ([10, 20, 30, 40], "a ...", dict(a=10)),
             ([10, 20, 30, 40], " a ... b", dict(a=10, b=40)),
             ([10, 40], " a ... b", dict(a=10, b=40)),
-        ]
-    )
-    def test_ellipsis(self, shape: List[int], pattern: str, expected: Dict[str, int]):
-        x = numpy.ones(shape)
-        parsed1 = parse_shape(x, pattern)
-        parsed2 = parse_shape(self.backend.from_numpy(x), pattern)
-        assert parsed1 == parsed2 == expected
+        ]:
+            x = numpy.ones(shape)
+            parsed1 = parse_shape(x, pattern)
+            parsed2 = parse_shape(self.backend.from_numpy(x), pattern)
+            assert parsed1 == parsed2 == expected
+
+    def test_parse_with_anonymous_axes(self):
+        for shape, pattern, expected in [
+            ([1, 2, 3, 4], "1 2 3 a", dict(a=4)),
+            ([10, 1, 2], "a 1 2", dict(a=10)),
+            ([10, 1, 2], "a () 2", dict(a=10)),
+        ]:
+            x = numpy.ones(shape)
+            parsed1 = parse_shape(x, pattern)
+            parsed2 = parse_shape(self.backend.from_numpy(x), pattern)
+            assert parsed1 == parsed2 == expected
+
+    def test_failures(self):
+        # every test should fail
+        for shape, pattern in [
+            ([1, 2, 3, 4], "a b c"),
+            ([1, 2, 3, 4], "2 a b c"),
+            ([1, 2, 3, 4], "a b c ()"),
+            ([1, 2, 3, 4], "a b c d e"),
+            ([1, 2, 3, 4], "a b c d e ..."),
+            ([1, 2, 3, 4], "a b c ()"),
+        ]:
+            with pytest.raises(RuntimeError):
+                x = numpy.ones(shape)
+                parse_shape(self.backend.from_numpy(x), pattern)
 
 
 _SYMBOLIC_BACKENDS = [
     {"backend": backend}
     for backend in (
         collect_test_backends(symbolic=True, layers=False) + collect_test_backends(symbolic=True, layers=True)
     )
@@ -232,44 +255,46 @@
     """
     Test ensures that allow_ops_in_compiled_graph allows compiling in a single graph
     Additionally we ensure that after compilation cache works properly
      (by changing shapes and patterns)
     We additionally check that pack/unpack still can be handled
      despite variable number of inputs/outputs
     """
-    if not is_backend_tested('torch'):
+    if not is_backend_tested("torch"):
         pytest.skip()
     import torch
     from torch import nn
     from einops import repeat, reduce, pack, unpack, einsum
     from einops._torch_specific import allow_ops_in_compiled_graph
 
     allow_ops_in_compiled_graph()
+
     class TorchModuleWithOperations(nn.Module):
         def __init__(self) -> None:
             super().__init__()
 
-        def forward(self, x_abc, suffix=''):
+        def forward(self, x_abc, suffix=""):
             a, b, c = x_abc.shape
 
             def suf(pattern):
                 parts = pattern.split()
-                return ' '.join([p if p[-1] not in 'acd' else p + suffix for p in parts])
+                return " ".join([p if p[-1] not in "acd" else p + suffix for p in parts])
+
             # patterns look a bit strange because names a, c, d will be modified on every run
             # by suf function
-            x_abcd = repeat(x_abc, suf('a b c -> a b c 4'))
-            x_abc = reduce(x_abcd, suf('a b c d -> a b c'), 'min')
-            x_abdc, ps = pack([x_abc] * (2 + len(suffix)), suf('a b * c'))
-            x_array = unpack(rearrange(x_abdc, suf('a b d c -> (a b ) 1 c d')), ps, 'ab one1 c *')
+            x_abcd = repeat(x_abc, suf("a b c -> a b c 4"))
+            x_abc = reduce(x_abcd, suf("a b c d -> a b c"), "min")
+            x_abdc, ps = pack([x_abc] * (2 + len(suffix)), suf("a b * c"))
+            x_array = unpack(rearrange(x_abdc, suf("a b d c -> (a b ) 1 c d")), ps, "ab one1 c *")
             x1 = x_array[0] + len(x_array)
-            x1 = rearrange(x1, suf('(a b ) 1 c -> a b c'), b=b)
-            addition = einsum(x_abc, x_abcd, suf('a b c , a b c d -> d'))[0]
+            x1 = rearrange(x1, suf("(a b ) 1 c -> a b c"), b=b)
+            addition = einsum(x_abc, x_abcd, suf("a b c , a b c d -> d"))[0]
             return x1 + addition
 
     original = TorchModuleWithOperations()
-    compiled = torch.compile(original, fullgraph=True, backend='aot_eager')
+    compiled = torch.compile(original, fullgraph=True, backend="aot_eager")
     for size in [10, 20, 40]:
         x = torch.rand([size, size + 1, size + 2])
-        for suffix in ['', 'suf1', 'other_suffix']:
+        for suffix in ["", "suf1", "other_suffix"]:
             result1 = compiled(x, suffix)
             result2 = original(x, suffix)
             assert torch.allclose(result1, result2)
```

### Comparing `einops-0.7.0rc2/tests/test_packing.py` & `einops-0.8.0/tests/test_packing.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         packed, ps2 = pack(unpacked, pattern=pattern)
 
     with capturer_numpy:
         x_np = asnumpy(x)
         unpacked_np = unpack(x_np, ps, pattern)
         packed_np, ps3 = pack(unpacked_np, pattern=pattern)
 
-    assert type(capturer_numpy.exception) == type(capturer_backend.exception)
+    assert type(capturer_numpy.exception) == type(capturer_backend.exception)  # noqa E721
     if capturer_numpy.exception is not None:
         # both failed
         return
     else:
         # neither failed, check results are identical
         assert np.allclose(asnumpy(packed), asnumpy(x))
         assert np.allclose(asnumpy(packed_np), asnumpy(x))
@@ -265,15 +265,14 @@
                 unpack_and_pack(x, [[0], [-1], [5]], pattern)
                 unpack_and_pack(x, [[-1], [5], [0]], pattern)
 
                 # -1 takes zero, -1
                 unpack_and_pack(x, [[2, -1], [1, 5]], pattern)
 
 
-
 def test_pack_unpack_array_api():
     from einops import array_api as AA
     import numpy.array_api as xp
 
     for case in cases:
         shape = case.shape
         pattern = case.pattern
@@ -282,15 +281,14 @@
 
         for ps in [
             [[2], [1], [2]],
             [[1], [1], [-1]],
             [[1], [1], [-1, 3]],
             [[2, 1], [1, 1, 1], [-1]],
         ]:
-
             x_np_split = unpack(x_np, ps, pattern)
             x_xp_split = AA.unpack(x_xp, ps, pattern)
             for a, b in zip(x_np_split, x_xp_split):
                 assert np.allclose(a, AA.asnumpy(b + 0))
 
             x_agg_np, ps1 = pack(x_np_split, pattern)
             x_agg_xp, ps2 = AA.pack(x_xp_split, pattern)
@@ -302,8 +300,7 @@
             [[1], [5]],
             [[1], [5], [-1]],
             [[1], [2, 3]],
             [[1], [5], [-1, 2]],
         ]:
             with pytest.raises(BaseException):
                 unpack(x_np, ps, pattern)
-
```

### Comparing `einops-0.7.0rc2/tests/test_parsing.py` & `einops-0.8.0/tests/test_parsing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,126 @@
 import pytest
 
 from einops import EinopsError
 from einops.parsing import ParsedExpression, AnonymousAxis, _ellipsis
 
-__author__ = 'Alex Rogozhnikov'
+__author__ = "Alex Rogozhnikov"
 
 
 class AnonymousAxisPlaceholder:
     def __init__(self, value: int):
         self.value = value
         assert isinstance(self.value, int)
 
     def __eq__(self, other):
         return isinstance(other, AnonymousAxis) and self.value == other.value
 
 
 def test_anonymous_axes():
-    a, b = AnonymousAxis('2'), AnonymousAxis('2')
+    a, b = AnonymousAxis("2"), AnonymousAxis("2")
     assert a != b
     c, d = AnonymousAxisPlaceholder(2), AnonymousAxisPlaceholder(3)
     assert a == c and b == c
     assert a != d and b != d
     assert [a, 2, b] == [c, 2, c]
 
 
 def test_elementary_axis_name():
-    for name in ['a', 'b', 'h', 'dx', 'h1', 'zz', 'i9123', 'somelongname',
-                 'Alex', 'camelCase', 'u_n_d_e_r_score', 'unreasonablyLongAxisName']:
+    for name in [
+        "a",
+        "b",
+        "h",
+        "dx",
+        "h1",
+        "zz",
+        "i9123",
+        "somelongname",
+        "Alex",
+        "camelCase",
+        "u_n_d_e_r_score",
+        "unreasonablyLongAxisName",
+    ]:
         assert ParsedExpression.check_axis_name(name)
 
-    for name in ['', '2b', '12', '_startWithUnderscore', 'endWithUnderscore_', '_', '...', _ellipsis]:
+    for name in ["", "2b", "12", "_startWithUnderscore", "endWithUnderscore_", "_", "...", _ellipsis]:
         assert not ParsedExpression.check_axis_name(name)
 
 
 def test_invalid_expressions():
     # double ellipsis should raise an error
-    ParsedExpression('... a b c d')
+    ParsedExpression("... a b c d")
     with pytest.raises(EinopsError):
-        ParsedExpression('... a b c d ...')
+        ParsedExpression("... a b c d ...")
     with pytest.raises(EinopsError):
-        ParsedExpression('... a b c (d ...)')
+        ParsedExpression("... a b c (d ...)")
     with pytest.raises(EinopsError):
-        ParsedExpression('(... a) b c (d ...)')
+        ParsedExpression("(... a) b c (d ...)")
 
     # double/missing/enclosed parenthesis
-    ParsedExpression('(a) b c (d ...)')
+    ParsedExpression("(a) b c (d ...)")
     with pytest.raises(EinopsError):
-        ParsedExpression('(a)) b c (d ...)')
+        ParsedExpression("(a)) b c (d ...)")
     with pytest.raises(EinopsError):
-        ParsedExpression('(a b c (d ...)')
+        ParsedExpression("(a b c (d ...)")
     with pytest.raises(EinopsError):
-        ParsedExpression('(a) (()) b c (d ...)')
+        ParsedExpression("(a) (()) b c (d ...)")
     with pytest.raises(EinopsError):
-        ParsedExpression('(a) ((b c) (d ...))')
+        ParsedExpression("(a) ((b c) (d ...))")
 
     # invalid identifiers
-    ParsedExpression('camelCase under_scored cApiTaLs ß ...')
+    ParsedExpression("camelCase under_scored cApiTaLs ß ...")
     with pytest.raises(EinopsError):
-        ParsedExpression('1a')
+        ParsedExpression("1a")
     with pytest.raises(EinopsError):
-        ParsedExpression('_pre')
+        ParsedExpression("_pre")
     with pytest.raises(EinopsError):
-        ParsedExpression('...pre')
+        ParsedExpression("...pre")
     with pytest.raises(EinopsError):
-        ParsedExpression('pre...')
+        ParsedExpression("pre...")
 
 
 def test_parse_expression():
-    parsed = ParsedExpression('a1  b1   c1    d1')
-    assert parsed.identifiers == {'a1', 'b1', 'c1', 'd1'}
-    assert parsed.composition == [['a1'], ['b1'], ['c1'], ['d1']]
+    parsed = ParsedExpression("a1  b1   c1    d1")
+    assert parsed.identifiers == {"a1", "b1", "c1", "d1"}
+    assert parsed.composition == [["a1"], ["b1"], ["c1"], ["d1"]]
     assert not parsed.has_non_unitary_anonymous_axes
     assert not parsed.has_ellipsis
 
-    parsed = ParsedExpression('() () () ()')
+    parsed = ParsedExpression("() () () ()")
     assert parsed.identifiers == set()
     assert parsed.composition == [[], [], [], []]
     assert not parsed.has_non_unitary_anonymous_axes
     assert not parsed.has_ellipsis
 
-    parsed = ParsedExpression('1 1 1 ()')
+    parsed = ParsedExpression("1 1 1 ()")
     assert parsed.identifiers == set()
     assert parsed.composition == [[], [], [], []]
     assert not parsed.has_non_unitary_anonymous_axes
     assert not parsed.has_ellipsis
 
     aap = AnonymousAxisPlaceholder
 
-    parsed = ParsedExpression('5 (3 4)')
+    parsed = ParsedExpression("5 (3 4)")
     assert len(parsed.identifiers) == 3 and {i.value for i in parsed.identifiers} == {3, 4, 5}
     assert parsed.composition == [[aap(5)], [aap(3), aap(4)]]
     assert parsed.has_non_unitary_anonymous_axes
     assert not parsed.has_ellipsis
 
-    parsed = ParsedExpression('5 1 (1 4) 1')
+    parsed = ParsedExpression("5 1 (1 4) 1")
     assert len(parsed.identifiers) == 2 and {i.value for i in parsed.identifiers} == {4, 5}
     assert parsed.composition == [[aap(5)], [], [aap(4)], []]
 
-    parsed = ParsedExpression('name1 ... a1 12 (name2 14)')
+    parsed = ParsedExpression("name1 ... a1 12 (name2 14)")
     assert len(parsed.identifiers) == 6
-    assert parsed.identifiers.difference({'name1', _ellipsis, 'a1', 'name2'}).__len__() == 2
-    assert parsed.composition == [['name1'], _ellipsis, ['a1'], [aap(12)], ['name2', aap(14)]]
+    assert parsed.identifiers.difference({"name1", _ellipsis, "a1", "name2"}).__len__() == 2
+    assert parsed.composition == [["name1"], _ellipsis, ["a1"], [aap(12)], ["name2", aap(14)]]
     assert parsed.has_non_unitary_anonymous_axes
     assert parsed.has_ellipsis
     assert not parsed.has_ellipsis_parenthesized
 
-    parsed = ParsedExpression('(name1 ... a1 12) name2 14')
+    parsed = ParsedExpression("(name1 ... a1 12) name2 14")
     assert len(parsed.identifiers) == 6
-    assert parsed.identifiers.difference({'name1', _ellipsis, 'a1', 'name2'}).__len__() == 2
-    assert parsed.composition == [['name1', _ellipsis, 'a1', aap(12)], ['name2'], [aap(14)]]
+    assert parsed.identifiers.difference({"name1", _ellipsis, "a1", "name2"}).__len__() == 2
+    assert parsed.composition == [["name1", _ellipsis, "a1", aap(12)], ["name2"], [aap(14)]]
     assert parsed.has_non_unitary_anonymous_axes
     assert parsed.has_ellipsis
     assert parsed.has_ellipsis_parenthesized
```

### Comparing `einops-0.7.0rc2/.gitignore` & `einops-0.8.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
 # logo and video generation
 logo
 
 # code of internal checks
 _uncommited_explorations
 trash_notebooks
+*.personal*
 
 # oneflow's output trash
 log
 
 # this file is auto-generated
 docs_src/index.md
```

### Comparing `einops-0.7.0rc2/LICENSE` & `einops-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `einops-0.7.0rc2/README.md` & `einops-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
-- 0.7.0rc1: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
-- 10'000: github reports that more than 10k project use einops 🎂
-- see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
+- 0.7.0: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
+- 10'000🎉: github reports that more than 10k project use einops
 - einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
 - [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
   Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
 
 
@@ -48,24 +47,25 @@
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
 
+
 ## Tweets 
 
 > In case you need convincing arguments for setting aside time to learn about einsum and einops...
-[Tim Rocktäschel, FAIR](https://twitter.com/_rockt/status/1230818967205425152)
+[Tim Rocktäschel](https://twitter.com/_rockt/status/1230818967205425152)
 
 > Writing better code with PyTorch and einops 👌
-[Andrej Karpathy, AI at Tesla](https://twitter.com/karpathy/status/1290826075916779520)
+[Andrej Karpathy](https://twitter.com/karpathy/status/1290826075916779520)
 
 > Slowly but surely, einops is seeping in to every nook and cranny of my code. If you find yourself shuffling around bazillion dimensional tensors, this might change your life
-[Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/1216022614755463169)
+[Nasim Rahaman](https://twitter.com/nasim_rahaman/status/1216022614755463169)
 
 [More testimonials](https://einops.rocks/pages/testimonials/)
 
 <!--
 ## Recordings of talk at ICLR 2022
 
 <a href='https://iclr.cc/virtual/2022/oral/6603'>
@@ -158,15 +158,14 @@
 Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
 
 ```python
 from einops.layers.torch      import Rearrange, Reduce
 from einops.layers.tensorflow import Rearrange, Reduce
 from einops.layers.flax       import Rearrange, Reduce
 from einops.layers.paddle     import Rearrange, Reduce
-from einops.layers.keras      import Rearrange, Reduce
 from einops.layers.chainer    import Rearrange, Reduce
 ```
 
 <details markdown="1">
 <summary>Example of using layers within a pytorch model</summary>
 Example given for pytorch, but code in other frameworks is almost identical
 
@@ -314,17 +313,18 @@
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
 - [tensorflow](https://www.tensorflow.org/)
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
-- [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
+- [oneflow](https://github.com/Oneflow-Inc/oneflow) (community)
+- [tinygrad](https://github.com/tinygrad/tinygrad) (community)
 
 Additionally, starting from einops 0.7.0 einops can be used with any framework that supports [Python array API standard](https://data-apis.org/array-api/latest/API_specification/index.html)
 
 ## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
```

#### html2text {}

```diff
@@ -5,79 +5,76 @@
 badge.fury.io/py/einops.svg)](https://badge.fury.io/py/einops) [!
 [Documentation](https://img.shields.io/badge/documentation-link-blue.svg)]
 (https://einops.rocks/) ![Supported python versions](https://
 raw.githubusercontent.com/arogozhnikov/einops/master/docs/resources/
 python_badge.svg) Flexible and powerful tensor operations for readable and
 reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - 0.7.0rc1: no-hassle `torch.compile`, support of [array api
+## Recent updates: - 0.7.0: no-hassle `torch.compile`, support of [array api
 standard](https://data-apis.org/array-api/latest/API_specification/index.html)
-and more - 10'000: github reports that more than 10k project use einops ð -
-see how to use einops with [torch.compile](https://github.com/arogozhnikov/
-einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1: paddle backend
-added - einops 0.6 introduces [packing and unpacking](https://github.com/
-arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - einops 0.5:
-einsum is now a part of einops - [Einops paper](https://openreview.net/
-pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it
-worth reading). Talk recordings are [available](https://iclr.cc/virtual/2022/
-oral/6603) Previous updates - flax and oneflow backend added - torch.jit.script
-is supported for pytorch layers - powerful EinMix added to einops. [Einmix
-tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-
-einmix-layer.ipynb) ## Tweets > In case you need convincing arguments for
-setting aside time to learn about einsum and einops... [Tim RocktÃ¤schel, FAIR]
-(https://twitter.com/_rockt/status/1230818967205425152) > Writing better code
-with PyTorch and einops ð [Andrej Karpathy, AI at Tesla](https://
+and more - 10'000ð: github reports that more than 10k project use einops -
+einops 0.6.1: paddle backend added - einops 0.6 introduces [packing and
+unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-
+unpack.ipynb) - einops 0.5: einsum is now a part of einops - [Einops paper]
+(https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation
+at ICLR 2022 (yes, it worth reading). Talk recordings are [available](https://
+iclr.cc/virtual/2022/oral/6603) Previous updates - flax and oneflow backend
+added - torch.jit.script is supported for pytorch layers - powerful EinMix
+added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/
+einops/blob/master/docs/3-einmix-layer.ipynb) ## Tweets > In case you need
+convincing arguments for setting aside time to learn about einsum and einops...
+[Tim RocktÃ¤schel](https://twitter.com/_rockt/status/1230818967205425152) >
+Writing better code with PyTorch and einops ð [Andrej Karpathy](https://
 twitter.com/karpathy/status/1290826075916779520) > Slowly but surely, einops is
 seeping in to every nook and cranny of my code. If you find yourself shuffling
 around bazillion dimensional tensors, this might change your life [Nasim
-Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/
-1216022614755463169) [More testimonials](https://einops.rocks/pages/
-testimonials/) ## Contents - [Installation](#Installation) - [Documentation]
-(https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-reference](#API)
-- [Why using einops](#Why-using-einops-notation) - [Supported frameworks]
-(#Supported-frameworks) - [Citing](#Citing) - [Repository](https://github.com/
-arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
-discussions) ## Installation Plain and simple: ```bash pip install einops ```
-## Tutorials Tutorials are the most convenient way to see `einops` in action -
-part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
-master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
-/github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
-learning.ipynb) - part 3: [packing and unpacking](https://github.com/
-arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - part 4:
-[improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)
-Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/
-watch?v=xGy75Pjsqzo). ## API `einops` has a minimalistic yet powerful API.
-Three core operations provided ([einops tutorial](https://github.com/
-arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
-transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
-reductions) ```python from einops import rearrange, reduce, repeat # rearrange
-elements according to the pattern output_tensor = rearrange(input_tensor, 't b
-c -> b c t') # combine rearrangement and reduction output_tensor = reduce
-(input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
-a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` Later
-additions to the family are `pack` and `unpack` functions (better than stack/
-split/concatenate): ```python from einops import pack, unpack # pack and unpack
-allow reversibly 'packing' multiple tensors into one. # Packed tensors may be
-of different dimensionality: packed, ps = pack([class_token_bc,
-image_tokens_bhwc, text_tokens_btc], 'b * c') class_emb_bc, image_emb_bhwc,
-text_emb_btc = unpack(transformer(packed), ps, 'b * c') ``` Finally, einops
-provides einsum with a support of multi-lettered names: ```python from einops
-import einsum, pack, unpack # einsum is like ... einsum, generic and flexible
-dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
-with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
-t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
-Mixers and similar architectures. ### Layers Einops provides layers (`einops`
-keeps a separate version for each framework) that reflect corresponding
-functions ```python from einops.layers.torch import Rearrange, Reduce from
-einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
-import Rearrange, Reduce from einops.layers.paddle import Rearrange, Reduce
-from einops.layers.keras import Rearrange, Reduce from einops.layers.chainer
-import Rearrange, Reduce ``` Example of using layers within a pytorch model
-Example given for pytorch, but code in other frameworks is almost identical
-```python from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+Rahaman](https://twitter.com/nasim_rahaman/status/1216022614755463169) [More
+testimonials](https://einops.rocks/pages/testimonials/) ## Contents -
+[Installation](#Installation) - [Documentation](https://einops.rocks/) -
+[Tutorial](#Tutorials) - [API micro-reference](#API) - [Why using einops](#Why-
+using-einops-notation) - [Supported frameworks](#Supported-frameworks) -
+[Citing](#Citing) - [Repository](https://github.com/arogozhnikov/einops) and
+[discussions](https://github.com/arogozhnikov/einops/discussions) ##
+Installation Plain and simple: ```bash pip install einops ``` ## Tutorials
+Tutorials are the most convenient way to see `einops` in action - part 1:
+[einops fundamentals](https://github.com/arogozhnikov/einops/blob/master/docs/
+1-einops-basics.ipynb) - part 2: [einops for deep learning](https://github.com/
+arogozhnikov/einops/blob/master/docs/2-einops-for-deep-learning.ipynb) - part
+3: [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/
+docs/4-pack-and-unpack.ipynb) - part 4: [improve pytorch code with einops]
+(http://einops.rocks/pytorch-examples.html) Kapil Sachdeva recorded a small
+[intro to einops](https://www.youtube.com/watch?v=xGy75Pjsqzo). ## API `einops`
+has a minimalistic yet powerful API. Three core operations provided ([einops
+tutorial](https://github.com/arogozhnikov/einops/blob/master/docs/) shows those
+cover stacking, reshape, transposition, squeeze/unsqueeze, repeat, tile,
+concatenate, view and numerous reductions) ```python from einops import
+rearrange, reduce, repeat # rearrange elements according to the pattern
+output_tensor = rearrange(input_tensor, 't b c -> b c t') # combine
+rearrangement and reduction output_tensor = reduce(input_tensor, 'b c (h h2) (w
+w2) -> b h w c', 'mean', h2=2, w2=2) # copy along a new axis output_tensor =
+repeat(input_tensor, 'h w -> h w c', c=3) ``` Later additions to the family are
+`pack` and `unpack` functions (better than stack/split/concatenate): ```python
+from einops import pack, unpack # pack and unpack allow reversibly 'packing'
+multiple tensors into one. # Packed tensors may be of different dimensionality:
+packed, ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b *
+c') class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed),
+ps, 'b * c') ``` Finally, einops provides einsum with a support of multi-
+lettered names: ```python from einops import einsum, pack, unpack # einsum is
+like ... einsum, generic and flexible dot-product # but 1) axes can be multi-
+lettered 2) pattern goes last 3) works with multiple frameworks C = einsum(A,
+B, 'b t1 head c, b t2 head c -> b head t1 t2') ``` ### EinMix `EinMix` is a
+generic linear layer, perfect for MLP Mixers and similar architectures. ###
+Layers Einops provides layers (`einops` keeps a separate version for each
+framework) that reflect corresponding functions ```python from
+einops.layers.torch import Rearrange, Reduce from einops.layers.tensorflow
+import Rearrange, Reduce from einops.layers.flax import Rearrange, Reduce from
+einops.layers.paddle import Rearrange, Reduce from einops.layers.chainer import
+Rearrange, Reduce ``` Example of using layers within a pytorch model Example
+given for pytorch, but code in other frameworks is almost identical ```python
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
 einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
 kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
 forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
 (120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
 from layers as those are script-able and compile-able. ## Naming `einops`
 stands for Einstein-Inspired Notation for operations (though "Einstein
 operations" is more attractive and easier to remember). Notation was loosely
@@ -125,19 +122,19 @@
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
 [Testimonials](https://einops.rocks/pages/testimonials/) provide users'
 perspective on the same question. ## Supported frameworks Einops works with ...
 - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
 [tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
 jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
-[tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
-github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
+[tf.keras](https://www.tensorflow.org/guide/keras) - [flax](https://github.com/
 google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
-(experimental) Additionally, starting from einops 0.7.0 einops can be used with
-any framework that supports [Python array API standard](https://data-apis.org/
-array-api/latest/API_specification/index.html) ## Citing einops Please use the
-following bibtex record ```text @inproceedings{ rogozhnikov2022einops, title=
-{Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
-author={Alex Rogozhnikov}, booktitle={International Conference on Learning
-Representations}, year={2022}, url={https://openreview.net/
-forum?id=oapKSVM2bcj} } ``` ## Supported python versions `einops` works with
-python 3.8 or later.
+(experimental) - [oneflow](https://github.com/Oneflow-Inc/oneflow) (community)
+- [tinygrad](https://github.com/tinygrad/tinygrad) (community) Additionally,
+starting from einops 0.7.0 einops can be used with any framework that supports
+[Python array API standard](https://data-apis.org/array-api/latest/
+API_specification/index.html) ## Citing einops Please use the following bibtex
+record ```text @inproceedings{ rogozhnikov2022einops, title={Einops: Clear and
+Reliable Tensor Manipulations with Einstein-like Notation}, author={Alex
+Rogozhnikov}, booktitle={International Conference on Learning Representations},
+year={2022}, url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ##
+Supported python versions `einops` works with python 3.8 or later.
```

### Comparing `einops-0.7.0rc2/pyproject.toml` & `einops-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     "ignore:Call to deprecated create function Descriptor",
     "ignore:Call to deprecated create function EnumDescriptor",
     "ignore:Call to deprecated create function EnumValueDescriptor",
     "ignore:Call to deprecated create function FileDescriptor",
     "ignore:Call to deprecated create function OneofDescriptor",
 ]
 
-[tool.black]
-line-length = 120
-target-version = ['py311']
-
 
 [tool.ruff]
+
 line-length = 120
+target-version = 'py311'
+
+cache-dir = "/tmp/ruff_cache" # move cache out of workdir
+
+lint.select = ["E4", "E7", "E9", "F", "W"]
+
+[tool.ruff.format]
+docstring-code-format = false
```

### Comparing `einops-0.7.0rc2/PKG-INFO` & `einops-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: einops
-Version: 0.7.0rc2
+Version: 0.8.0
 Summary: A new flavour of deep learning operations
 Project-URL: Homepage, https://github.com/arogozhnikov/einops
 Author: Alex Rogozhnikov
 License: MIT
 License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific computations,tensor manipulation
 Classifier: Intended Audience :: Science/Research
@@ -40,17 +40,16 @@
 
 
 Flexible and powerful tensor operations for readable and reliable code. <br />
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
 
 ## Recent updates:
 
-- 0.7.0rc1: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
-- 10'000: github reports that more than 10k project use einops 🎂
-- see how to use einops with [torch.compile](https://github.com/arogozhnikov/einops/wiki/Using-torch.compile-with-einops)
+- 0.7.0: no-hassle `torch.compile`, support of [array api standard](https://data-apis.org/array-api/latest/API_specification/index.html) and more
+- 10'000🎉: github reports that more than 10k project use einops
 - einops 0.6.1: paddle backend added
 - einops 0.6 introduces [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb)
 - einops 0.5: einsum is now a part of einops
 - [Einops paper](https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it worth reading).
   Talk recordings are [available](https://iclr.cc/virtual/2022/oral/6603)
 
 
@@ -63,24 +62,25 @@
 
 <!--<div align="center">
   <img src="http://arogozhnikov.github.io/images/einops/einops_logo_350x350.png" 
   alt="einops package logo" width="250" height="250" />
   <br><br>
 </div> -->
 
+
 ## Tweets 
 
 > In case you need convincing arguments for setting aside time to learn about einsum and einops...
-[Tim Rocktäschel, FAIR](https://twitter.com/_rockt/status/1230818967205425152)
+[Tim Rocktäschel](https://twitter.com/_rockt/status/1230818967205425152)
 
 > Writing better code with PyTorch and einops 👌
-[Andrej Karpathy, AI at Tesla](https://twitter.com/karpathy/status/1290826075916779520)
+[Andrej Karpathy](https://twitter.com/karpathy/status/1290826075916779520)
 
 > Slowly but surely, einops is seeping in to every nook and cranny of my code. If you find yourself shuffling around bazillion dimensional tensors, this might change your life
-[Nasim Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/1216022614755463169)
+[Nasim Rahaman](https://twitter.com/nasim_rahaman/status/1216022614755463169)
 
 [More testimonials](https://einops.rocks/pages/testimonials/)
 
 <!--
 ## Recordings of talk at ICLR 2022
 
 <a href='https://iclr.cc/virtual/2022/oral/6603'>
@@ -173,15 +173,14 @@
 Einops provides layers (`einops` keeps a separate version for each framework) that reflect corresponding functions
 
 ```python
 from einops.layers.torch      import Rearrange, Reduce
 from einops.layers.tensorflow import Rearrange, Reduce
 from einops.layers.flax       import Rearrange, Reduce
 from einops.layers.paddle     import Rearrange, Reduce
-from einops.layers.keras      import Rearrange, Reduce
 from einops.layers.chainer    import Rearrange, Reduce
 ```
 
 <details markdown="1">
 <summary>Example of using layers within a pytorch model</summary>
 Example given for pytorch, but code in other frameworks is almost identical
 
@@ -329,17 +328,18 @@
 - [numpy](http://www.numpy.org/)
 - [pytorch](https://pytorch.org/)
 - [tensorflow](https://www.tensorflow.org/)
 - [jax](https://github.com/google/jax)
 - [cupy](https://cupy.chainer.org/)
 - [chainer](https://chainer.org/)
 - [tf.keras](https://www.tensorflow.org/guide/keras)
-- [oneflow](https://github.com/Oneflow-Inc/oneflow) (experimental)
 - [flax](https://github.com/google/flax) (experimental)
 - [paddle](https://github.com/PaddlePaddle/Paddle) (experimental)
+- [oneflow](https://github.com/Oneflow-Inc/oneflow) (community)
+- [tinygrad](https://github.com/tinygrad/tinygrad) (community)
 
 Additionally, starting from einops 0.7.0 einops can be used with any framework that supports [Python array API standard](https://data-apis.org/array-api/latest/API_specification/index.html)
 
 ## Citing einops <a name="Citing"></a>
 
 Please use the following bibtex record
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: einops Version: 0.7.0rc2 Summary: A new flavour of
+Metadata-Version: 2.3 Name: einops Version: 0.8.0 Summary: A new flavour of
 deep learning operations Project-URL: Homepage, https://github.com/
 arogozhnikov/einops Author: Alex Rogozhnikov License: MIT License-File: LICENSE
 Keywords: deep learning,einops,machine learning,neural networks,scientific
 computations,tensor manipulation Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown https://user-images.githubusercontent.com/6318811/
@@ -12,79 +12,76 @@
 run_tests.yml) [![PyPI version](https://badge.fury.io/py/einops.svg)](https://
 badge.fury.io/py/einops) [![Documentation](https://img.shields.io/badge/
 documentation-link-blue.svg)](https://einops.rocks/) ![Supported python
 versions](https://raw.githubusercontent.com/arogozhnikov/einops/master/docs/
 resources/python_badge.svg) Flexible and powerful tensor operations for
 readable and reliable code.
 Supports numpy, pytorch, tensorflow, jax, and [others](#supported-frameworks).
-## Recent updates: - 0.7.0rc1: no-hassle `torch.compile`, support of [array api
+## Recent updates: - 0.7.0: no-hassle `torch.compile`, support of [array api
 standard](https://data-apis.org/array-api/latest/API_specification/index.html)
-and more - 10'000: github reports that more than 10k project use einops ð -
-see how to use einops with [torch.compile](https://github.com/arogozhnikov/
-einops/wiki/Using-torch.compile-with-einops) - einops 0.6.1: paddle backend
-added - einops 0.6 introduces [packing and unpacking](https://github.com/
-arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - einops 0.5:
-einsum is now a part of einops - [Einops paper](https://openreview.net/
-pdf?id=oapKSVM2bcj) is accepted for oral presentation at ICLR 2022 (yes, it
-worth reading). Talk recordings are [available](https://iclr.cc/virtual/2022/
-oral/6603) Previous updates - flax and oneflow backend added - torch.jit.script
-is supported for pytorch layers - powerful EinMix added to einops. [Einmix
-tutorial notebook](https://github.com/arogozhnikov/einops/blob/master/docs/3-
-einmix-layer.ipynb) ## Tweets > In case you need convincing arguments for
-setting aside time to learn about einsum and einops... [Tim RocktÃ¤schel, FAIR]
-(https://twitter.com/_rockt/status/1230818967205425152) > Writing better code
-with PyTorch and einops ð [Andrej Karpathy, AI at Tesla](https://
+and more - 10'000ð: github reports that more than 10k project use einops -
+einops 0.6.1: paddle backend added - einops 0.6 introduces [packing and
+unpacking](https://github.com/arogozhnikov/einops/blob/master/docs/4-pack-and-
+unpack.ipynb) - einops 0.5: einsum is now a part of einops - [Einops paper]
+(https://openreview.net/pdf?id=oapKSVM2bcj) is accepted for oral presentation
+at ICLR 2022 (yes, it worth reading). Talk recordings are [available](https://
+iclr.cc/virtual/2022/oral/6603) Previous updates - flax and oneflow backend
+added - torch.jit.script is supported for pytorch layers - powerful EinMix
+added to einops. [Einmix tutorial notebook](https://github.com/arogozhnikov/
+einops/blob/master/docs/3-einmix-layer.ipynb) ## Tweets > In case you need
+convincing arguments for setting aside time to learn about einsum and einops...
+[Tim RocktÃ¤schel](https://twitter.com/_rockt/status/1230818967205425152) >
+Writing better code with PyTorch and einops ð [Andrej Karpathy](https://
 twitter.com/karpathy/status/1290826075916779520) > Slowly but surely, einops is
 seeping in to every nook and cranny of my code. If you find yourself shuffling
 around bazillion dimensional tensors, this might change your life [Nasim
-Rahaman, MILA (Montreal)](https://twitter.com/nasim_rahaman/status/
-1216022614755463169) [More testimonials](https://einops.rocks/pages/
-testimonials/) ## Contents - [Installation](#Installation) - [Documentation]
-(https://einops.rocks/) - [Tutorial](#Tutorials) - [API micro-reference](#API)
-- [Why using einops](#Why-using-einops-notation) - [Supported frameworks]
-(#Supported-frameworks) - [Citing](#Citing) - [Repository](https://github.com/
-arogozhnikov/einops) and [discussions](https://github.com/arogozhnikov/einops/
-discussions) ## Installation Plain and simple: ```bash pip install einops ```
-## Tutorials Tutorials are the most convenient way to see `einops` in action -
-part 1: [einops fundamentals](https://github.com/arogozhnikov/einops/blob/
-master/docs/1-einops-basics.ipynb) - part 2: [einops for deep learning](https:/
-/github.com/arogozhnikov/einops/blob/master/docs/2-einops-for-deep-
-learning.ipynb) - part 3: [packing and unpacking](https://github.com/
-arogozhnikov/einops/blob/master/docs/4-pack-and-unpack.ipynb) - part 4:
-[improve pytorch code with einops](http://einops.rocks/pytorch-examples.html)
-Kapil Sachdeva recorded a small [intro to einops](https://www.youtube.com/
-watch?v=xGy75Pjsqzo). ## API `einops` has a minimalistic yet powerful API.
-Three core operations provided ([einops tutorial](https://github.com/
-arogozhnikov/einops/blob/master/docs/) shows those cover stacking, reshape,
-transposition, squeeze/unsqueeze, repeat, tile, concatenate, view and numerous
-reductions) ```python from einops import rearrange, reduce, repeat # rearrange
-elements according to the pattern output_tensor = rearrange(input_tensor, 't b
-c -> b c t') # combine rearrangement and reduction output_tensor = reduce
-(input_tensor, 'b c (h h2) (w w2) -> b h w c', 'mean', h2=2, w2=2) # copy along
-a new axis output_tensor = repeat(input_tensor, 'h w -> h w c', c=3) ``` Later
-additions to the family are `pack` and `unpack` functions (better than stack/
-split/concatenate): ```python from einops import pack, unpack # pack and unpack
-allow reversibly 'packing' multiple tensors into one. # Packed tensors may be
-of different dimensionality: packed, ps = pack([class_token_bc,
-image_tokens_bhwc, text_tokens_btc], 'b * c') class_emb_bc, image_emb_bhwc,
-text_emb_btc = unpack(transformer(packed), ps, 'b * c') ``` Finally, einops
-provides einsum with a support of multi-lettered names: ```python from einops
-import einsum, pack, unpack # einsum is like ... einsum, generic and flexible
-dot-product # but 1) axes can be multi-lettered 2) pattern goes last 3) works
-with multiple frameworks C = einsum(A, B, 'b t1 head c, b t2 head c -> b head
-t1 t2') ``` ### EinMix `EinMix` is a generic linear layer, perfect for MLP
-Mixers and similar architectures. ### Layers Einops provides layers (`einops`
-keeps a separate version for each framework) that reflect corresponding
-functions ```python from einops.layers.torch import Rearrange, Reduce from
-einops.layers.tensorflow import Rearrange, Reduce from einops.layers.flax
-import Rearrange, Reduce from einops.layers.paddle import Rearrange, Reduce
-from einops.layers.keras import Rearrange, Reduce from einops.layers.chainer
-import Rearrange, Reduce ``` Example of using layers within a pytorch model
-Example given for pytorch, but code in other frameworks is almost identical
-```python from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
+Rahaman](https://twitter.com/nasim_rahaman/status/1216022614755463169) [More
+testimonials](https://einops.rocks/pages/testimonials/) ## Contents -
+[Installation](#Installation) - [Documentation](https://einops.rocks/) -
+[Tutorial](#Tutorials) - [API micro-reference](#API) - [Why using einops](#Why-
+using-einops-notation) - [Supported frameworks](#Supported-frameworks) -
+[Citing](#Citing) - [Repository](https://github.com/arogozhnikov/einops) and
+[discussions](https://github.com/arogozhnikov/einops/discussions) ##
+Installation Plain and simple: ```bash pip install einops ``` ## Tutorials
+Tutorials are the most convenient way to see `einops` in action - part 1:
+[einops fundamentals](https://github.com/arogozhnikov/einops/blob/master/docs/
+1-einops-basics.ipynb) - part 2: [einops for deep learning](https://github.com/
+arogozhnikov/einops/blob/master/docs/2-einops-for-deep-learning.ipynb) - part
+3: [packing and unpacking](https://github.com/arogozhnikov/einops/blob/master/
+docs/4-pack-and-unpack.ipynb) - part 4: [improve pytorch code with einops]
+(http://einops.rocks/pytorch-examples.html) Kapil Sachdeva recorded a small
+[intro to einops](https://www.youtube.com/watch?v=xGy75Pjsqzo). ## API `einops`
+has a minimalistic yet powerful API. Three core operations provided ([einops
+tutorial](https://github.com/arogozhnikov/einops/blob/master/docs/) shows those
+cover stacking, reshape, transposition, squeeze/unsqueeze, repeat, tile,
+concatenate, view and numerous reductions) ```python from einops import
+rearrange, reduce, repeat # rearrange elements according to the pattern
+output_tensor = rearrange(input_tensor, 't b c -> b c t') # combine
+rearrangement and reduction output_tensor = reduce(input_tensor, 'b c (h h2) (w
+w2) -> b h w c', 'mean', h2=2, w2=2) # copy along a new axis output_tensor =
+repeat(input_tensor, 'h w -> h w c', c=3) ``` Later additions to the family are
+`pack` and `unpack` functions (better than stack/split/concatenate): ```python
+from einops import pack, unpack # pack and unpack allow reversibly 'packing'
+multiple tensors into one. # Packed tensors may be of different dimensionality:
+packed, ps = pack([class_token_bc, image_tokens_bhwc, text_tokens_btc], 'b *
+c') class_emb_bc, image_emb_bhwc, text_emb_btc = unpack(transformer(packed),
+ps, 'b * c') ``` Finally, einops provides einsum with a support of multi-
+lettered names: ```python from einops import einsum, pack, unpack # einsum is
+like ... einsum, generic and flexible dot-product # but 1) axes can be multi-
+lettered 2) pattern goes last 3) works with multiple frameworks C = einsum(A,
+B, 'b t1 head c, b t2 head c -> b head t1 t2') ``` ### EinMix `EinMix` is a
+generic linear layer, perfect for MLP Mixers and similar architectures. ###
+Layers Einops provides layers (`einops` keeps a separate version for each
+framework) that reflect corresponding functions ```python from
+einops.layers.torch import Rearrange, Reduce from einops.layers.tensorflow
+import Rearrange, Reduce from einops.layers.flax import Rearrange, Reduce from
+einops.layers.paddle import Rearrange, Reduce from einops.layers.chainer import
+Rearrange, Reduce ``` Example of using layers within a pytorch model Example
+given for pytorch, but code in other frameworks is almost identical ```python
+from torch.nn import Sequential, Conv2d, MaxPool2d, Linear, ReLU from
 einops.layers.torch import Rearrange model = Sequential( ..., Conv2d(6, 16,
 kernel_size=5), MaxPool2d(kernel_size=2), # flattening without need to write
 forward Rearrange('b c h w -> b (c h w)'), Linear(16*5*5, 120), ReLU(), Linear
 (120, 10), ) ``` No more flatten needed! Additionally, torch users will benefit
 from layers as those are script-able and compile-able. ## Naming `einops`
 stands for Einstein-Inspired Notation for operations (though "Einstein
 operations" is more attractive and easier to remember). Notation was loosely
@@ -132,19 +129,19 @@
 'h w -> h (tile w)', tile=2) # in tf repeat(image, 'h w -> h (tile w)', tile=2)
 # in jax repeat(image, 'h w -> h (tile w)', tile=2) # in cupy ... (etc.) ```
 [Testimonials](https://einops.rocks/pages/testimonials/) provide users'
 perspective on the same question. ## Supported frameworks Einops works with ...
 - [numpy](http://www.numpy.org/) - [pytorch](https://pytorch.org/) -
 [tensorflow](https://www.tensorflow.org/) - [jax](https://github.com/google/
 jax) - [cupy](https://cupy.chainer.org/) - [chainer](https://chainer.org/) -
-[tf.keras](https://www.tensorflow.org/guide/keras) - [oneflow](https://
-github.com/Oneflow-Inc/oneflow) (experimental) - [flax](https://github.com/
+[tf.keras](https://www.tensorflow.org/guide/keras) - [flax](https://github.com/
 google/flax) (experimental) - [paddle](https://github.com/PaddlePaddle/Paddle)
-(experimental) Additionally, starting from einops 0.7.0 einops can be used with
-any framework that supports [Python array API standard](https://data-apis.org/
-array-api/latest/API_specification/index.html) ## Citing einops Please use the
-following bibtex record ```text @inproceedings{ rogozhnikov2022einops, title=
-{Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
-author={Alex Rogozhnikov}, booktitle={International Conference on Learning
-Representations}, year={2022}, url={https://openreview.net/
-forum?id=oapKSVM2bcj} } ``` ## Supported python versions `einops` works with
-python 3.8 or later.
+(experimental) - [oneflow](https://github.com/Oneflow-Inc/oneflow) (community)
+- [tinygrad](https://github.com/tinygrad/tinygrad) (community) Additionally,
+starting from einops 0.7.0 einops can be used with any framework that supports
+[Python array API standard](https://data-apis.org/array-api/latest/
+API_specification/index.html) ## Citing einops Please use the following bibtex
+record ```text @inproceedings{ rogozhnikov2022einops, title={Einops: Clear and
+Reliable Tensor Manipulations with Einstein-like Notation}, author={Alex
+Rogozhnikov}, booktitle={International Conference on Learning Representations},
+year={2022}, url={https://openreview.net/forum?id=oapKSVM2bcj} } ``` ##
+Supported python versions `einops` works with python 3.8 or later.
```

