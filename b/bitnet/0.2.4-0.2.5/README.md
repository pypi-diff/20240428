# Comparing `tmp/bitnet-0.2.4.tar.gz` & `tmp/bitnet-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitnet-0.2.4.tar", max compression
+gzip compressed data, was "bitnet-0.2.5.tar", max compression
```

## Comparing `bitnet-0.2.4.tar` & `bitnet-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-10-18 16:19:28.150325 bitnet-0.2.4/LICENSE
--rw-r--r--   0        0        0     9404 2024-04-04 18:13:01.988695 bitnet-0.2.4/README.md
--rw-r--r--   0        0        0      664 2024-04-04 18:13:01.989393 bitnet-0.2.4/bitnet/__init__.py
--rw-r--r--   0        0        0     3465 2024-03-01 19:18:43.112600 bitnet-0.2.4/bitnet/at.py
--rw-r--r--   0        0        0    12739 2024-03-01 20:29:44.095925 bitnet-0.2.4/bitnet/bit_attention.py
--rw-r--r--   0        0        0     4077 2024-03-01 21:13:33.168128 bitnet-0.2.4/bitnet/bit_ffn.py
--rw-r--r--   0        0        0     1531 2024-04-01 03:23:11.454392 bitnet-0.2.4/bitnet/bit_linear_new.py
--rw-r--r--   0        0        0    17973 2024-03-25 01:48:38.566685 bitnet-0.2.4/bitnet/bit_llama.py
--rw-r--r--   0        0        0     3034 2024-04-03 00:23:27.023230 bitnet-0.2.4/bitnet/bit_lora.py
--rw-r--r--   0        0        0    18667 2024-04-04 18:13:01.989661 bitnet-0.2.4/bitnet/bit_mamba.py
--rw-r--r--   0        0        0    10070 2024-04-03 00:14:20.060186 bitnet-0.2.4/bitnet/bit_moe.py
--rw-r--r--   0        0        0     3909 2024-03-04 04:15:41.162906 bitnet-0.2.4/bitnet/bit_transformer.py
--rw-r--r--   0        0        0     1528 2024-04-01 03:24:00.785922 bitnet-0.2.4/bitnet/bitlinear.py
--rw-r--r--   0        0        0     1980 2024-03-01 20:30:11.205701 bitnet-0.2.4/bitnet/inference.py
--rw-r--r--   0        0        0     1708 2024-03-13 04:11:00.313804 bitnet-0.2.4/bitnet/replace_hf.py
--rw-r--r--   0        0        0     1233 2024-04-04 18:14:11.580798 bitnet-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    10359 1970-01-01 00:00:00.000000 bitnet-0.2.4/setup.py
--rw-r--r--   0        0        0    10531 1970-01-01 00:00:00.000000 bitnet-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-10-18 16:19:28.150325 bitnet-0.2.5/LICENSE
+-rw-r--r--   0        0        0     9798 2024-04-28 02:19:26.111816 bitnet-0.2.5/README.md
+-rw-r--r--   0        0        0      712 2024-04-28 02:18:20.858300 bitnet-0.2.5/bitnet/__init__.py
+-rw-r--r--   0        0        0     3465 2024-03-01 19:18:43.112600 bitnet-0.2.5/bitnet/at.py
+-rw-r--r--   0        0        0    12739 2024-03-01 20:29:44.095925 bitnet-0.2.5/bitnet/bit_attention.py
+-rw-r--r--   0        0        0     4077 2024-03-01 21:13:33.168128 bitnet-0.2.5/bitnet/bit_ffn.py
+-rw-r--r--   0        0        0     1531 2024-04-01 03:23:11.454392 bitnet-0.2.5/bitnet/bit_linear_new.py
+-rw-r--r--   0        0        0    17973 2024-03-25 01:48:38.566685 bitnet-0.2.5/bitnet/bit_llama.py
+-rw-r--r--   0        0        0     3034 2024-04-03 00:23:27.023230 bitnet-0.2.5/bitnet/bit_lora.py
+-rw-r--r--   0        0        0    19488 2024-04-28 02:11:35.945778 bitnet-0.2.5/bitnet/bit_mamba.py
+-rw-r--r--   0        0        0     4609 2024-04-28 02:27:19.326015 bitnet-0.2.5/bitnet/bit_moe.py
+-rw-r--r--   0        0        0     3909 2024-03-04 04:15:41.162906 bitnet-0.2.5/bitnet/bit_transformer.py
+-rw-r--r--   0        0        0     1528 2024-04-01 03:24:00.785922 bitnet-0.2.5/bitnet/bitlinear.py
+-rw-r--r--   0        0        0     1980 2024-03-01 20:30:11.205701 bitnet-0.2.5/bitnet/inference.py
+-rw-r--r--   0        0        0     1708 2024-03-13 04:11:00.313804 bitnet-0.2.5/bitnet/replace_hf.py
+-rw-r--r--   0        0        0     1234 2024-04-28 04:23:08.157532 bitnet-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    10774 1970-01-01 00:00:00.000000 bitnet-0.2.5/setup.py
+-rw-r--r--   0        0        0    10726 1970-01-01 00:00:00.000000 bitnet-0.2.5/PKG-INFO
```

### Comparing `bitnet-0.2.4/LICENSE` & `bitnet-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/README.md` & `bitnet-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -269,28 +269,48 @@
 
 
 ## BitMamba
 ```python
 import torch
 from bitnet import BitMamba
 
-# Create a random tensor of shape (2, 10, 512)
-x = torch.randn(2, 10, 512)
+# Create a tensor of size (2, 10) with random values between 0 and 100
+x = torch.randint(0, 100, (2, 10))
 
-# Create an instance of the BitMamba model with input size 512 and output size 6
-model = BitMamba(512, 6)
+# Create an instance of the BitMamba model with input size 512, hidden size 100, output size 10, and depth size 6
+model = BitMamba(512, 100, 10, 6, return_tokens=True)
 
-# Pass the input tensor through the model to get the output
+# Pass the input tensor through the model and get the output
 output = model(x)
 
 # Print the output tensor
 print(output)
 
 # Print the shape of the output tensor
 print(output.shape)
+
+```
+
+## `BitMoE`
+
+```python
+import torch
+from bitnet.bit_moe import BitMoE
+
+# Create input tensor
+x = torch.randn(2, 4, 8)
+
+# Create BitMoE model with specified input and output dimensions
+model = BitMoE(8, 4, 2)
+
+# Forward pass through the model
+output = model(x)
+
+# Print the output
+print(output)
 ```
 
 # License
 MIT
 
 # Citation
 ```bibtex
```

### Comparing `bitnet-0.2.4/bitnet/__init__.py` & `bitnet-0.2.5/bitnet/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from bitnet.bit_linear_new import BitLinearNew
 from bitnet.bit_transformer import BitNetTransformer
 from bitnet.bitlinear import BitLinear
 from bitnet.inference import BitNetInference
 from bitnet.replace_hf import replace_linears_in_hf, replace_linears_in_pytorch_model
 from bitnet.bit_lora import BitLora
 from bitnet.bit_mamba import BitMamba
+from bitnet.bit_moe import BitMoE
 
 __all__ = [
     "BitFeedForward",
     "BitNetInference",
     "replace_linears_in_hf",
     "replace_linears_in_pytorch_model",
     "BitNetTransformer",
     "BitMGQA",
     "BitLinearNew",
     "BitLinear",
     "BitLora",
     "BitMamba",
+    "BitMoE",
 ]
```

### Comparing `bitnet-0.2.4/bitnet/at.py` & `bitnet-0.2.5/bitnet/at.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_attention.py` & `bitnet-0.2.5/bitnet/bit_attention.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_ffn.py` & `bitnet-0.2.5/bitnet/bit_ffn.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_linear_new.py` & `bitnet-0.2.5/bitnet/bit_linear_new.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_llama.py` & `bitnet-0.2.5/bitnet/bit_llama.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_lora.py` & `bitnet-0.2.5/bitnet/bit_lora.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bit_mamba.py` & `bitnet-0.2.5/bitnet/bit_mamba.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,15 @@
 from dataclasses import dataclass
 from typing import Union
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 from bitnet.bitlinear import BitLinear
-
-"""
-
-An implementation of the parallel scan operation in PyTorch (Blelloch version).
-This code follows the skeleton proposed by Francois Fleuret in his pscan. However, the keys differences are :
--it has been written in an iterative way (rather than recursive)
--the backward pass has been rewritten
-
-Please see docs/pscan.ipynb for a detailed explanation of what happens here.
-
-"""
+from zeta.nn import OutputHead
 
 
 # taken straight from https://github.com/johnma2006/mamba-minimal/blob/master/model.py
 class RMSNorm(nn.Module):
     def __init__(self, dim: int, eps: float = 1e-5):
         super().__init__()
 
@@ -491,35 +481,58 @@
         y = y + D * x
 
         # todo : pq h.squeeze(1) ??
         return y, h.squeeze(1)
 
 
 class Mamba(nn.Module):
-    def __init__(self, config: MambaConfig):
+    def __init__(
+        self,
+        num_tokens: int,
+        sequence_length: int,
+        config: MambaConfig,
+        return_embeddings: bool = True,
+        return_tokens: bool = True,
+    ):
         super().__init__()
-
+        self.num_tokens = num_tokens
+        self.sequence_length = sequence_length
         self.config = config
+        self.return_embeddings = return_embeddings
+        self.return_tokens = return_tokens
+
+        # Embedding
+        self.token_embed = nn.Embedding(num_tokens, config.dim)
+        self.norm = nn.LayerNorm(config.dim)
 
         self.layers = nn.ModuleList(
             [ResidualBlock(config) for _ in range(config.depth)]
         )
         # self.norm_f = RMSNorm(config.dim)
 
     def forward(self, x):
         # x : (B, L, D)
 
         # y : (B, L, D)
+        # Embedding
+        x = self.token_embed(x)
+        x = self.norm(x)
 
         for layer in self.layers:
             x = layer(x)
 
-        # x = self.norm_f(x)
+        x = self.norm(x)
 
-        return x
+        # Return embeddings or Logits
+        # Return Tokens
+        if self.return_tokens:
+            x = OutputHead(self.config.dim, -1)(x)
+            return x
+        else:
+            return x
 
     def step(self, x, caches):
         # x : (B, L, D)
         # caches : [cache(layer) for all layers], cache : (h, inputs)
 
         # y : (B, L, D)
         # caches : [cache(layer) for all layers], cache : (h, inputs)
@@ -550,43 +563,53 @@
         conv_bias (bool, optional): Whether to include bias terms in the convolutional layers. Defaults to True.
         pscan (bool, optional): Whether to use parallel scan mode or sequential mode when training. Defaults to True.
     """
 
     def __init__(
         self,
         dim: int,  # D
+        num_tokens: int,
+        sequence_length: int,
         depth: int,
         dt_rank: Union[int, str] = "auto",
         d_state: int = 16,  # N in paper/comments
         expand_factor: int = 2,  # E in paper/comments
         d_conv: int = 4,
         dt_min: float = 0.001,
         dt_max: float = 0.1,
         dt_init: str = "random",  # "random" or "constant"
         dt_scale: float = 1.0,
         dt_init_floor=1e-4,
         bias: bool = False,
         conv_bias: bool = True,
         pscan: bool = True,  # use parallel scan mode or sequential mode when training
+        return_embeddings: bool = True,
+        return_tokens: bool = True,
+        *args,
+        **kwargs
     ):
-        super().__init__()
+        super().__init__(*args, **kwargs)
         self.dim = dim
+        self.num_token = num_tokens
+        self.sequence_length = sequence_length
         self.depth = depth
         self.dt_rank = dt_rank
         self.d_state = d_state
         self.expand_factor = expand_factor
         self.d_conv = d_conv
         self.dt_min = dt_min
         self.dt_max = dt_max
         self.dt_init = dt_init
         self.dt_scale = dt_scale
         self.dt_init_floor = dt_init_floor
         self.bias = bias
         self.conv_bias = conv_bias
         self.pscan = pscan
+        self.return_embeddings = return_embeddings
+        self.return_tokens = return_tokens
 
         self.d_inner = self.expand_factor * self.dim
 
         if self.dt_rank == "auto":
             self.dt_rank = math.ceil(self.dim / 16)
 
         # Mamba
@@ -602,20 +625,17 @@
             dt_init=self.dt_init,
             dt_scale=self.dt_scale,
             # dt_init_floor=self.dt_init_floor,
             bias=self.bias,
             conv_bias=self.conv_bias,
             pscan=self.pscan,
         )
-        self.mamba = Mamba(config)
+        self.mamba = Mamba(
+            num_tokens=self.num_token,
+            sequence_length=self.sequence_length,
+            config=config,
+            return_embeddings=self.return_embeddings,
+            return_tokens=self.return_tokens,
+        )
 
     def forward(self, x):
         return self.mamba(x)
-
-
-# x = torch.randn(2, 10, 512)
-
-# model = BitMamba(512, 6)
-
-# output = model(x)
-# print(output)
-# print(output.shape)
```

### Comparing `bitnet-0.2.4/bitnet/bit_transformer.py` & `bitnet-0.2.5/bitnet/bit_transformer.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/bitlinear.py` & `bitnet-0.2.5/bitnet/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/inference.py` & `bitnet-0.2.5/bitnet/inference.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/bitnet/replace_hf.py` & `bitnet-0.2.5/bitnet/replace_hf.py`

 * *Files identical despite different names*

### Comparing `bitnet-0.2.4/pyproject.toml` & `bitnet-0.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bitnet"
-version = "0.2.4"
+version = "0.2.5"
 description = "bitnet - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/bitnet"
 documentation = "https://github.com/kyegomez/bitnet"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/bitnet"
@@ -18,15 +18,15 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.10"
 torch = "*"
 einops = "*"
 zetascale = "*"
 
 
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `bitnet-0.2.4/setup.py` & `bitnet-0.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['einops', 'torch', 'zetascale']
 
 setup_kwargs = {
     'name': 'bitnet',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'bitnet - Pytorch',
-    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# BitNet\n![bitnet](/bitnet.png)\nPyTorch Implementation of the linear methods and model from the paper "BitNet: Scaling 1-bit Transformers for Large Language Models"\n\n[Paper link:](https://arxiv.org/pdf/2310.11453.pdf)\n\nBitLinear = tensor -> layernorm -> Binarize -> abs max quantization -> dequant\n\n"The implementation of the BitNet architecture is quite simple, requiring only the replacement of linear projections (i.e., nn.Linear in PyTorch) in the Transformer. " -- BitNet is really easy to implement just swap out the linears with the BitLinear modules! \n\n## **NEWS**\n- **New Iteration** 🔥 There is an all-new iteration from the paper "[The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits](https://arxiv.org/abs/2402.17764)", we\'re implementing it now. Join the Agora discord and contribute! [Join Here](https://discord.gg/hFzevCjG8c)\n- **New Optimizations** The first `BitLinear` has been optimized and we now have a Bit Attention `BitMGQA` That implements BitLinear into the attention mechanism. Multi Grouped Query Attention is also widely recognized as the best attention for its fast decoding and long context handling, thanks to Frank for his easy to use implementation!\n- **BitLinear 1.5 Launch 🔥**: The new BitLinear 1.5 is still in progress 🔥 [Here is the file]() There are still some bugs like with the dequantization algorithm and we still need to replace the multiplication with elementwisw addition, if you could help with this, this would be amazing.\n- **NOTICE**: A model obviously needs to be finetuned from scratch to use BitLinear, just changing the linear methods in an already trained model isn\'t going to work. Finetune or train from scratch.\n\n## Appreciation\n- Dimitry, Nullonix for analysis and code review and revision\n- Vyom, for providing 4080 to train!\n\n## Installation\n`pip install bitnet`\n\n## Usage:\n\n### `BitLinear`\n- Example of the BitLinear layer which is the main innovation of the paper!\n```python\nimport torch\n\nfrom bitnet import BitLinear\n\n# Input\nx = torch.randn(10, 1000, 512)\n\n# BitLinear layer\nlayer = BitLinear(512, 400)\n\n# Output\ny = layer(x)\n\nprint(y)\n\n```\n\n### BitLinearNew\n```python\nimport torch\nfrom bitnet import BitLinearNew\n\n# Create a random tensor of shape (16, 10)\nx = torch.randn(16, 1000, 512)\n\n# Create an instance of the BitLinearNew class with input size 10, output size 20, and 2 groups\nlayer = BitLinearNew(\n    512,\n    20,\n)\n\n# Perform a forward pass through the BitLinearNew layer with input x\noutput = layer(x)\n\n# Print the output tensor\nprint(output)\nprint(output.shape)\n```\n----\n\n### `BitNetTransformer`\n- Fully implemented Transformer as described in the diagram with MHA, and BitFeedforwards\n- Can be utilized not just for text but for images and maybe even video or audio processing\n- Complete with residuals and skip connections for gradient flow\n\n```python\n# Import the necessary libraries\nimport torch\nfrom bitnet import BitNetTransformer\n\n# Create a random tensor of integers\nx = torch.randint(0, 20000, (1, 1024))\n\n# Initialize the BitNetTransformer model\nbitnet = BitNetTransformer(\n    num_tokens=20000,  # Number of unique tokens in the input\n    dim=1024,  # Dimension of the input and output embeddings\n    depth=6,  # Number of transformer layers\n    heads=8,  # Number of attention heads\n    ff_mult=4,  # Multiplier for the hidden dimension in the feed-forward network\n)\n\n# Pass the tensor through the transformer model\nlogits = bitnet(x)\n\n# Print the shape of the output\nprint(logits)\n\n```\n\n\n### `BitAttention`\nThis Attention has been modified to use BitLinear instead of the default linear projection. It\'s also using Multi-Grouped Query Attention instead of regular multi-head attention for faster decoding and longer context handling.\n\n```python\nimport torch\nfrom bitnet import BitMGQA\n\n# Create a random tensor of shape (1, 10, 512)\nx = torch.randn(1, 10, 512)\n\n# Create an instance of the BitMGQA model with input size 512, 8 attention heads, and 4 layers\ngqa = BitMGQA(512, 8, 4)\n\n# Pass the input tensor through the BitMGQA model and get the output and attention weights\nout, _ = gqa(x, x, x, need_weights=True)\n\n# Print the shapes of the output tensor and attention tensor\nprint(out)\n```\n\n### `BitFeedForward`\n- Feedforward as shown in the diagram with BitLinear and a GELU:\n- Linear -> GELU -> Linear\n- You can add dropouts, or layernorms, or other layers for a better ffn\n\n```python\nimport torch\nfrom bitnet import BitFeedForward\n\n# Create a random input tensor of shape (10, 512)\nx = torch.randn(10, 512)\n\n# Create an instance of the BitFeedForward class with the following parameters:\n# - input_dim: 512\n# - hidden_dim: 512\n# - num_layers: 4\n# - swish: True (use Swish activation function)\n# - post_act_ln: True (apply Layer Normalization after each activation)\n# - dropout: 0.1 (apply dropout with a probability of 0.1)\nff = BitFeedForward(512, 512, 4, swish=True, post_act_ln=True, dropout=0.1)\n\n# Apply the BitFeedForward network to the input tensor x\ny = ff(x)\n\n# Print the shape of the output tensor y\nprint(y)  # torch.Size([10, 512])\n```\n\n## Inference\n```python\nfrom bitnet import BitNetInference\n\nbitnet = BitNetInference()\nbitnet.load_model("../model_checkpoint.pth")  # Download model\noutput_str = bitnet.generate("The dog jumped over the ", 512)\nprint(output_str)\n```\n\n## Huggingface Usage\n```python\nimport torch\nfrom transformers import AutoModelForSequenceClassification, AutoTokenizer\n\nfrom bitnet import replace_linears_in_hf\n\n# Load a model from Hugging Face\'s Transformers\nmodel_name = "bert-base-uncased"\ntokenizer = AutoTokenizer.from_pretrained(model_name)\nmodel = AutoModelForSequenceClassification.from_pretrained(model_name)\n\n# Replace Linear layers with BitLinear\nreplace_linears_in_hf(model)\n\n# Example text to classify\ntext = "Replace this with your text"\ninputs = tokenizer(\n    text, return_tensors="pt", padding=True, truncation=True, max_length=512\n)\n\n# Perform inference\nmodel.eval()  # Set the model to evaluation mode\nwith torch.no_grad():\n    outputs = model(**inputs)\n    predictions = torch.nn.functional.softmax(outputs.logits, dim=-1)\n    print(predictions)\n\n# Process predictions\npredicted_class_id = predictions.argmax().item()\nprint(f"Predicted class ID: {predicted_class_id}")\n\n# Optionally, map the predicted class ID to a label, if you know the classification labels\n# labels = ["Label 1", "Label 2", ...]  # Define your labels corresponding to the model\'s classes\n# print(f"Predicted label: {labels[predicted_class_id]}")\n```\n\n\n## Drop in Replacement for Pytorch Models\n```python\nimport torch\nfrom torch import nn\nfrom bitnet import replace_linears_in_pytorch_model\n\n# Define a simple model\nmodel = nn.Sequential(\n    nn.Linear(10, 20),\n    nn.ReLU(),\n    nn.Linear(20, 30),\n)\n\nprint("Before replacement:")\nprint(model)\n\n# Replace nn.Linear with BitLinear\nreplace_linears_in_pytorch_model(model)\n\nprint("After replacement:")\nprint(model)\n\n# Now you can use the model for training or inference\n# For example, pass a random input through the model\ninput = torch.randn(1, 10)\noutput = model(input)\n```\n\n\n### Optimized Cuda Kernel\n`python setup.py build_ext --inplace`\n\n```python\nimport torch\nimport gemm_lowbit_ext  # This imports the compiled module\n\n# Example usage\na = torch.randn(10, 20, dtype=torch.half, device=\'cuda\')  # Example tensor\nb = torch.randn(20, 30, dtype=torch.half, device=\'cuda\')  # Example tensor\nc = torch.empty(10, 30, dtype=torch.half, device=\'cuda\')  # Output tensor\n\nw_scale = 1.0  # Example scale factor\nx_scale = 1.0  # Example scale factor\n\n# Call the custom CUDA GEMM operation\ngemm_lowbit_ext.gemm_lowbit(a, b, c, w_scale, x_scale)\n\nprint(c)  # View the result\n\n```\n\n\n## `BitLora`\nImplementation of BitLora!\n\n```python\nimport torch\nfrom bitnet import BitLora\n\n# Random text tensor\nx = torch.randn(1, 12, 200)\n\n# Create an instance of the BitLora model\nmodel = BitLora(in_features=200, out_features=200, rank=4, lora_alpha=1)\n\n# Perform the forward pass\nout = model(x)\n\n# Print the shape of the output tensor\nprint(out.shape)\n```\n\n\n## BitMamba\n```python\nimport torch\nfrom bitnet import BitMamba\n\n# Create a random tensor of shape (2, 10, 512)\nx = torch.randn(2, 10, 512)\n\n# Create an instance of the BitMamba model with input size 512 and output size 6\nmodel = BitMamba(512, 6)\n\n# Pass the input tensor through the model to get the output\noutput = model(x)\n\n# Print the output tensor\nprint(output)\n\n# Print the shape of the output tensor\nprint(output.shape)\n```\n\n# License\nMIT\n\n# Citation\n```bibtex\n@misc{2310.11453,\nAuthor = {Hongyu Wang and Shuming Ma and Li Dong and Shaohan Huang and Huaijie Wang and Lingxiao Ma and Fan Yang and Ruiping Wang and Yi Wu and Furu Wei},\nTitle = {BitNet: Scaling 1-bit Transformers for Large Language Models},\nYear = {2023},\nEprint = {arXiv:2310.11453},\n}\n\n```\n\n\n# Todo\n- [x] Double check BitLinear implementation and make sure it works exactly as in paper \n- [x] Implement training script for `BitNetTransformer`\n- [x] Train on Enwiki8, copy and past code and data from Lucidrains repos\n- [x] Benchmark performance\n- [x] Look into Straight Through Estimator for non-differentiable backprop\n- [x] Implement BitFeedForward\n- [x] Clean up codebase \n- [x] Add unit tests for each module\n- [x] Implement the new BitNet1.5b from the [paper](https://arxiv.org/abs/2402.17764)\n- [ ] Implement the BitNet15b in Cuda',
+    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# BitNet\n![bitnet](/bitnet.png)\nPyTorch Implementation of the linear methods and model from the paper "BitNet: Scaling 1-bit Transformers for Large Language Models"\n\n[Paper link:](https://arxiv.org/pdf/2310.11453.pdf)\n\nBitLinear = tensor -> layernorm -> Binarize -> abs max quantization -> dequant\n\n"The implementation of the BitNet architecture is quite simple, requiring only the replacement of linear projections (i.e., nn.Linear in PyTorch) in the Transformer. " -- BitNet is really easy to implement just swap out the linears with the BitLinear modules! \n\n## **NEWS**\n- **New Iteration** 🔥 There is an all-new iteration from the paper "[The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits](https://arxiv.org/abs/2402.17764)", we\'re implementing it now. Join the Agora discord and contribute! [Join Here](https://discord.gg/hFzevCjG8c)\n- **New Optimizations** The first `BitLinear` has been optimized and we now have a Bit Attention `BitMGQA` That implements BitLinear into the attention mechanism. Multi Grouped Query Attention is also widely recognized as the best attention for its fast decoding and long context handling, thanks to Frank for his easy to use implementation!\n- **BitLinear 1.5 Launch 🔥**: The new BitLinear 1.5 is still in progress 🔥 [Here is the file]() There are still some bugs like with the dequantization algorithm and we still need to replace the multiplication with elementwisw addition, if you could help with this, this would be amazing.\n- **NOTICE**: A model obviously needs to be finetuned from scratch to use BitLinear, just changing the linear methods in an already trained model isn\'t going to work. Finetune or train from scratch.\n\n## Appreciation\n- Dimitry, Nullonix for analysis and code review and revision\n- Vyom, for providing 4080 to train!\n\n## Installation\n`pip install bitnet`\n\n## Usage:\n\n### `BitLinear`\n- Example of the BitLinear layer which is the main innovation of the paper!\n```python\nimport torch\n\nfrom bitnet import BitLinear\n\n# Input\nx = torch.randn(10, 1000, 512)\n\n# BitLinear layer\nlayer = BitLinear(512, 400)\n\n# Output\ny = layer(x)\n\nprint(y)\n\n```\n\n### BitLinearNew\n```python\nimport torch\nfrom bitnet import BitLinearNew\n\n# Create a random tensor of shape (16, 10)\nx = torch.randn(16, 1000, 512)\n\n# Create an instance of the BitLinearNew class with input size 10, output size 20, and 2 groups\nlayer = BitLinearNew(\n    512,\n    20,\n)\n\n# Perform a forward pass through the BitLinearNew layer with input x\noutput = layer(x)\n\n# Print the output tensor\nprint(output)\nprint(output.shape)\n```\n----\n\n### `BitNetTransformer`\n- Fully implemented Transformer as described in the diagram with MHA, and BitFeedforwards\n- Can be utilized not just for text but for images and maybe even video or audio processing\n- Complete with residuals and skip connections for gradient flow\n\n```python\n# Import the necessary libraries\nimport torch\nfrom bitnet import BitNetTransformer\n\n# Create a random tensor of integers\nx = torch.randint(0, 20000, (1, 1024))\n\n# Initialize the BitNetTransformer model\nbitnet = BitNetTransformer(\n    num_tokens=20000,  # Number of unique tokens in the input\n    dim=1024,  # Dimension of the input and output embeddings\n    depth=6,  # Number of transformer layers\n    heads=8,  # Number of attention heads\n    ff_mult=4,  # Multiplier for the hidden dimension in the feed-forward network\n)\n\n# Pass the tensor through the transformer model\nlogits = bitnet(x)\n\n# Print the shape of the output\nprint(logits)\n\n```\n\n\n### `BitAttention`\nThis Attention has been modified to use BitLinear instead of the default linear projection. It\'s also using Multi-Grouped Query Attention instead of regular multi-head attention for faster decoding and longer context handling.\n\n```python\nimport torch\nfrom bitnet import BitMGQA\n\n# Create a random tensor of shape (1, 10, 512)\nx = torch.randn(1, 10, 512)\n\n# Create an instance of the BitMGQA model with input size 512, 8 attention heads, and 4 layers\ngqa = BitMGQA(512, 8, 4)\n\n# Pass the input tensor through the BitMGQA model and get the output and attention weights\nout, _ = gqa(x, x, x, need_weights=True)\n\n# Print the shapes of the output tensor and attention tensor\nprint(out)\n```\n\n### `BitFeedForward`\n- Feedforward as shown in the diagram with BitLinear and a GELU:\n- Linear -> GELU -> Linear\n- You can add dropouts, or layernorms, or other layers for a better ffn\n\n```python\nimport torch\nfrom bitnet import BitFeedForward\n\n# Create a random input tensor of shape (10, 512)\nx = torch.randn(10, 512)\n\n# Create an instance of the BitFeedForward class with the following parameters:\n# - input_dim: 512\n# - hidden_dim: 512\n# - num_layers: 4\n# - swish: True (use Swish activation function)\n# - post_act_ln: True (apply Layer Normalization after each activation)\n# - dropout: 0.1 (apply dropout with a probability of 0.1)\nff = BitFeedForward(512, 512, 4, swish=True, post_act_ln=True, dropout=0.1)\n\n# Apply the BitFeedForward network to the input tensor x\ny = ff(x)\n\n# Print the shape of the output tensor y\nprint(y)  # torch.Size([10, 512])\n```\n\n## Inference\n```python\nfrom bitnet import BitNetInference\n\nbitnet = BitNetInference()\nbitnet.load_model("../model_checkpoint.pth")  # Download model\noutput_str = bitnet.generate("The dog jumped over the ", 512)\nprint(output_str)\n```\n\n## Huggingface Usage\n```python\nimport torch\nfrom transformers import AutoModelForSequenceClassification, AutoTokenizer\n\nfrom bitnet import replace_linears_in_hf\n\n# Load a model from Hugging Face\'s Transformers\nmodel_name = "bert-base-uncased"\ntokenizer = AutoTokenizer.from_pretrained(model_name)\nmodel = AutoModelForSequenceClassification.from_pretrained(model_name)\n\n# Replace Linear layers with BitLinear\nreplace_linears_in_hf(model)\n\n# Example text to classify\ntext = "Replace this with your text"\ninputs = tokenizer(\n    text, return_tensors="pt", padding=True, truncation=True, max_length=512\n)\n\n# Perform inference\nmodel.eval()  # Set the model to evaluation mode\nwith torch.no_grad():\n    outputs = model(**inputs)\n    predictions = torch.nn.functional.softmax(outputs.logits, dim=-1)\n    print(predictions)\n\n# Process predictions\npredicted_class_id = predictions.argmax().item()\nprint(f"Predicted class ID: {predicted_class_id}")\n\n# Optionally, map the predicted class ID to a label, if you know the classification labels\n# labels = ["Label 1", "Label 2", ...]  # Define your labels corresponding to the model\'s classes\n# print(f"Predicted label: {labels[predicted_class_id]}")\n```\n\n\n## Drop in Replacement for Pytorch Models\n```python\nimport torch\nfrom torch import nn\nfrom bitnet import replace_linears_in_pytorch_model\n\n# Define a simple model\nmodel = nn.Sequential(\n    nn.Linear(10, 20),\n    nn.ReLU(),\n    nn.Linear(20, 30),\n)\n\nprint("Before replacement:")\nprint(model)\n\n# Replace nn.Linear with BitLinear\nreplace_linears_in_pytorch_model(model)\n\nprint("After replacement:")\nprint(model)\n\n# Now you can use the model for training or inference\n# For example, pass a random input through the model\ninput = torch.randn(1, 10)\noutput = model(input)\n```\n\n\n### Optimized Cuda Kernel\n`python setup.py build_ext --inplace`\n\n```python\nimport torch\nimport gemm_lowbit_ext  # This imports the compiled module\n\n# Example usage\na = torch.randn(10, 20, dtype=torch.half, device=\'cuda\')  # Example tensor\nb = torch.randn(20, 30, dtype=torch.half, device=\'cuda\')  # Example tensor\nc = torch.empty(10, 30, dtype=torch.half, device=\'cuda\')  # Output tensor\n\nw_scale = 1.0  # Example scale factor\nx_scale = 1.0  # Example scale factor\n\n# Call the custom CUDA GEMM operation\ngemm_lowbit_ext.gemm_lowbit(a, b, c, w_scale, x_scale)\n\nprint(c)  # View the result\n\n```\n\n\n## `BitLora`\nImplementation of BitLora!\n\n```python\nimport torch\nfrom bitnet import BitLora\n\n# Random text tensor\nx = torch.randn(1, 12, 200)\n\n# Create an instance of the BitLora model\nmodel = BitLora(in_features=200, out_features=200, rank=4, lora_alpha=1)\n\n# Perform the forward pass\nout = model(x)\n\n# Print the shape of the output tensor\nprint(out.shape)\n```\n\n\n## BitMamba\n```python\nimport torch\nfrom bitnet import BitMamba\n\n# Create a tensor of size (2, 10) with random values between 0 and 100\nx = torch.randint(0, 100, (2, 10))\n\n# Create an instance of the BitMamba model with input size 512, hidden size 100, output size 10, and depth size 6\nmodel = BitMamba(512, 100, 10, 6, return_tokens=True)\n\n# Pass the input tensor through the model and get the output\noutput = model(x)\n\n# Print the output tensor\nprint(output)\n\n# Print the shape of the output tensor\nprint(output.shape)\n\n```\n\n## `BitMoE`\n\n```python\nimport torch\nfrom bitnet.bit_moe import BitMoE\n\n# Create input tensor\nx = torch.randn(2, 4, 8)\n\n# Create BitMoE model with specified input and output dimensions\nmodel = BitMoE(8, 4, 2)\n\n# Forward pass through the model\noutput = model(x)\n\n# Print the output\nprint(output)\n```\n\n# License\nMIT\n\n# Citation\n```bibtex\n@misc{2310.11453,\nAuthor = {Hongyu Wang and Shuming Ma and Li Dong and Shaohan Huang and Huaijie Wang and Lingxiao Ma and Fan Yang and Ruiping Wang and Yi Wu and Furu Wei},\nTitle = {BitNet: Scaling 1-bit Transformers for Large Language Models},\nYear = {2023},\nEprint = {arXiv:2310.11453},\n}\n\n```\n\n\n# Todo\n- [x] Double check BitLinear implementation and make sure it works exactly as in paper \n- [x] Implement training script for `BitNetTransformer`\n- [x] Train on Enwiki8, copy and past code and data from Lucidrains repos\n- [x] Benchmark performance\n- [x] Look into Straight Through Estimator for non-differentiable backprop\n- [x] Implement BitFeedForward\n- [x] Clean up codebase \n- [x] Add unit tests for each module\n- [x] Implement the new BitNet1.5b from the [paper](https://arxiv.org/abs/2402.17764)\n- [ ] Implement the BitNet15b in Cuda',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/bitnet',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `bitnet-0.2.4/PKG-INFO` & `bitnet-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: bitnet
-Version: 0.2.4
+Version: 0.2.5
 Summary: bitnet - Pytorch
 Home-page: https://github.com/kyegomez/bitnet
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
 Requires-Dist: torch
 Requires-Dist: zetascale
@@ -298,28 +294,48 @@
 
 
 ## BitMamba
 ```python
 import torch
 from bitnet import BitMamba
 
-# Create a random tensor of shape (2, 10, 512)
-x = torch.randn(2, 10, 512)
+# Create a tensor of size (2, 10) with random values between 0 and 100
+x = torch.randint(0, 100, (2, 10))
 
-# Create an instance of the BitMamba model with input size 512 and output size 6
-model = BitMamba(512, 6)
+# Create an instance of the BitMamba model with input size 512, hidden size 100, output size 10, and depth size 6
+model = BitMamba(512, 100, 10, 6, return_tokens=True)
 
-# Pass the input tensor through the model to get the output
+# Pass the input tensor through the model and get the output
 output = model(x)
 
 # Print the output tensor
 print(output)
 
 # Print the shape of the output tensor
 print(output.shape)
+
+```
+
+## `BitMoE`
+
+```python
+import torch
+from bitnet.bit_moe import BitMoE
+
+# Create input tensor
+x = torch.randn(2, 4, 8)
+
+# Create BitMoE model with specified input and output dimensions
+model = BitMoE(8, 4, 2)
+
+# Forward pass through the model
+output = model(x)
+
+# Print the output
+print(output)
 ```
 
 # License
 MIT
 
 # Citation
 ```bibtex
```

