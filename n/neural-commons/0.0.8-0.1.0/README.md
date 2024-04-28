# Comparing `tmp/neural-commons-0.0.8.tar.gz` & `tmp/neural-commons-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.0.8.tar", last modified: Wed Apr 10 19:04:02 2024, max compression
+gzip compressed data, was "neural-commons-0.1.0.tar", last modified: Sun Apr 28 17:26:52 2024, max compression
```

## Comparing `neural-commons-0.0.8.tar` & `neural-commons-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 19:04:02.427176 neural-commons-0.0.8/
--rw-rw-rw-   0        0        0      455 2024-04-10 19:04:02.426176 neural-commons-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 19:04:02.404176 neural-commons-0.0.8/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:04:02.410176 neural-commons-0.0.8/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0    10089 2024-04-08 14:26:47.000000 neural-commons-0.0.8/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:04:02.425176 neural-commons-0.0.8/neural_commons/modules/
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.0.8/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0     2818 2024-04-08 14:36:12.000000 neural-commons-0.0.8/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      844 2024-04-10 16:44:22.000000 neural-commons-0.0.8/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.0.8/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0     1350 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/PreTrainedLayer.py
--rw-rw-rw-   0        0        0      886 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.0.8/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.0.8/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      410 2024-04-10 19:01:58.000000 neural-commons-0.0.8/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:04:02.409176 neural-commons-0.0.8/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-10 19:04:02.000000 neural-commons-0.0.8/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-04-10 19:04:02.000000 neural-commons-0.0.8/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 19:04:02.000000 neural-commons-0.0.8/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-10 19:04:02.000000 neural-commons-0.0.8/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 19:04:02.000000 neural-commons-0.0.8/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 19:04:02.427176 neural-commons-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      968 2024-04-10 19:03:58.000000 neural-commons-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/
+-rw-rw-rw-   0        0        0      745 2024-04-28 17:26:52.785545 neural-commons-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.752250 neural-commons-0.1.0/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3238 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1511 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0      305 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0     8322 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/cf_nn/CFTrainer.py
+-rw-rw-rw-   0        0        0      898 2024-04-28 16:00:09.000000 neural-commons-0.1.0/neural_commons/cf_nn/LRFunctions.py
+-rw-rw-rw-   0        0        0      168 2024-04-28 16:58:17.000000 neural-commons-0.1.0/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4887 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.1.0/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.1.0/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.1.0/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.1.0/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      548 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.785545 neural-commons-0.1.0/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.1.0/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 17:26:52.754289 neural-commons-0.1.0/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      745 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1307 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-28 17:26:52.000000 neural-commons-0.1.0/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 17:26:52.785545 neural-commons-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-04-28 15:00:31.000000 neural-commons-0.1.0/setup.py
```

### Comparing `neural-commons-0.0.8/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.1.0/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.8/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.1.0/neural_commons/modules/NeuralLayer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import math
-from dataclasses import dataclass
-
 import torch
+import torch.nn.functional as F
+from dataclasses import dataclass
 from huggingface_hub import PyTorchModelHubMixin
 from torch import nn, Tensor
 from torch.nn import Parameter, init
-import torch.nn.functional as F
-
-from neural_commons.helpers.torch_helper import get_torch_dtype
 
 
 @dataclass
 class NeuralLayerConfig:
     in_features: int
     out_features: int
     bias: bool = True
@@ -22,40 +19,29 @@
 class NeuralLayer(nn.Module, PyTorchModelHubMixin):
     __constants__ = ['in_features', 'out_features']
     in_features: int
     out_features: int
     weight: Tensor
     hp_params: Tensor
 
-    def __init__(self, config: NeuralLayerConfig) -> None:
-        if isinstance(config, dict):
-            config = NeuralLayerConfig(**config)
+    def __init__(self, in_features: int, out_features: int, bias: bool = True,
+                 slopes_log_std: float = 0.1) -> None:
         super().__init__()
-        dtype = get_torch_dtype(config.dtype)
-        self.config = config
-        self.convert_input = dtype != torch.float and dtype != torch.float32
-        self.in_features = config.in_features
-        self.out_features = config.out_features
-        slopes_t = torch.exp(torch.randn(self.out_features, dtype=dtype) * config.slopes_log_std)
+        self.in_features = in_features
+        self.out_features = out_features
+        slopes_t = torch.exp(torch.randn(self.out_features) * slopes_log_std)
         self.slopes = nn.Parameter(slopes_t.detach())
         setattr(self.slopes, "__skip_transplant__", True)
-        self.weight = Parameter(torch.empty((self.out_features, self.in_features,), dtype=dtype))
-        if config.bias:
-            self.bias = Parameter(torch.empty(self.out_features, dtype=dtype))
+        self.weight = Parameter(torch.empty((self.out_features, self.in_features,)))
+        if bias:
+            self.bias = Parameter(torch.empty(self.out_features))
         else:
             self.register_parameter('bias', None)
         self.reset_parameters()
 
-    @classmethod
-    def build(cls, in_features: int, out_features: int, bias: bool = True,
-              dtype: str = "float32"):
-        return cls(NeuralLayerConfig(in_features=in_features,
-                                     out_features=out_features,
-                                     bias=bias, dtype=dtype))
-
     def reset_parameters(self) -> None:
         # Setting a=sqrt(5) in kaiming_uniform is the same as initializing with
         # uniform(-1/sqrt(in_features), 1/sqrt(in_features)). For details, see
         # https://github.com/pytorch/pytorch/issues/57109
         init.kaiming_uniform_(self.weight, a=math.sqrt(5))
         if self.bias is not None:
             fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
```

### Comparing `neural-commons-0.0.8/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.1.0/neural_commons/modules/NeuralLayer2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Union
-
 import torch
+from typing import Union
 from torch import nn, Tensor
 
 
 class NeuralLayer2d(nn.Module):
     def __init__(self, in_channels: int, out_channels: int,
                  kernel_size: Union[int, tuple[int, int]],
                  slopes_log_std=0.1,
```

### Comparing `neural-commons-0.0.8/neural_commons/modules/RndProjection.py` & `neural-commons-0.1.0/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.8/neural_commons/modules/SMoE.py` & `neural-commons-0.1.0/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.8/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.1.0/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.8/setup.py` & `neural-commons-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.0.8'
+VERSION = '0.1.0'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
-    'torch>=2.0.0',
+    'torch>=2.1.0',
     'transformers>=4.28.0',
-    'mpmath==1.3.0'
+    'mpmath==1.3.0',
 ]
 
 # Long description comes from README
 with codecs.open('README.md', 'r', 'utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 packages = find_packages(".")
```

