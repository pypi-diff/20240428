# Comparing `tmp/hnn_utils-0.3.0.tar.gz` & `tmp/hnn_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnn_utils-0.3.0.tar", max compression
+gzip compressed data, was "hnn_utils-0.3.1.tar", max compression
```

## Comparing `hnn_utils-0.3.0.tar` & `hnn_utils-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1068 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0      137 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/__init__.py
--rw-r--r--   0        0        0       48 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/callbacks/__init__.py
--rw-r--r--   0        0        0     6438 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/callbacks/ema.py
--rw-r--r--   0        0        0     1370 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/ALiBi.py
--rw-r--r--   0        0        0     1655 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/RotaryEmbedding.py
--rw-r--r--   0        0        0    14366 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/Transformer.py
--rw-r--r--   0        0        0      164 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/ffn.py
--rw-r--r--   0        0        0     1961 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/functional.py
--rw-r--r--   0        0        0      800 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/hnn_utils/nn/normalization.py
--rw-r--r--   0        0        0      448 2024-04-25 03:42:44.890258 hnn_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 hnn_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-28 17:40:00.813072 hnn_utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0      137 2024-04-28 17:40:00.813072 hnn_utils-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     6566 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/callbacks/ema.py
+-rw-r--r--   0        0        0      178 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/guacamol.py
+-rw-r--r--   0        0        0     3119 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/utils.py
+-rw-r--r--   0        0        0     1730 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac.json
+-rw-r--r--   0        0        0     1843 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac_random.json
+-rw-r--r--   0        0        0     5297 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/zinc20.json
+-rw-r--r--   0        0        0     2721 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/zinc.py
+-rw-r--r--   0        0        0     1370 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/ALiBi.py
+-rw-r--r--   0        0        0     1677 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/RotaryEmbedding.py
+-rw-r--r--   0        0        0    14366 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/Transformer.py
+-rw-r--r--   0        0        0      164 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/ffn.py
+-rw-r--r--   0        0        0     2000 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/functional.py
+-rw-r--r--   0        0        0      800 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/normalization.py
+-rw-r--r--   0        0        0      516 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 hnn_utils-0.3.1/PKG-INFO
```

### Comparing `hnn_utils-0.3.0/LICENSE` & `hnn_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.0/hnn_utils/callbacks/ema.py` & `hnn_utils-0.3.1/hnn_utils/callbacks/ema.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,31 @@
         super().__init__()
 
         self.tau = tau
 
         self.every_n_steps = update_every_n_steps
 
         if start_on_step is not None and start_on_epoch is not None:
-            raise ValueError("Only one of `update_after_n_steps` and `update_after_n_epochs` can be set.")
+            raise ValueError(
+                "Only one of `update_after_n_steps` and `update_after_n_epochs` can be set."
+            )
 
         if start_on_step is not None:
             self.update_start = UpdateAfter.STEP
             self.update_time = start_on_step
         elif start_on_epoch is not None:
             self.update_start = UpdateAfter.EPOCH
             self.update_time = start_on_epoch
         else:
             self.update_start = UpdateAfter.STEP
             self.update_time = 0
 
-        self.excluded_parameters = set(excluded_parameters) if excluded_parameters else set()
+        self.excluded_parameters = (
+            set(excluded_parameters) if excluded_parameters else set()
+        )
 
         self.ema_weights = None
 
         # We track the step instead of using the trainer's global_step because
         # multiple optimizers can increment the global step multiple times per batch
         self.step = 0
 
@@ -71,15 +75,17 @@
         self._cached_sd = None
         self.use_for_val = use_for_val
 
         # If we restore from a checkpoint, we need to know if we've transferred the weights
         # to the device yet or not
         self.on_device = False
 
-    def on_before_optimizer_step(self, trainer: Trainer, pl_module: LightningModule, optimizer: Optimizer) -> None:
+    def on_before_optimizer_step(
+        self, trainer: Trainer, pl_module: LightningModule, optimizer: Optimizer
+    ) -> None:
         if not self.should_update(trainer):
             return
 
         self.step += 1
 
         self._init(trainer, pl_module)
 
@@ -96,15 +102,17 @@
 
     def _init(self, trainer: Trainer, pl_module: LightningModule):
         if self.ema_weights is None:
             self.ema_weights = sd_copy(pl_module.state_dict())
             self.step = 0
             self.on_device = True
         elif not self.on_device:
-            self.ema_weights = {k: v.to(pl_module.device) for k, v in self.ema_weights.items()}
+            self.ema_weights = {
+                k: v.to(pl_module.device) for k, v in self.ema_weights.items()
+            }
             self.on_device = True
 
     def should_update(self, trainer: Trainer):
         if self.step % self.every_n_steps != 0:
             return False
 
         if self.update_start == UpdateAfter.STEP:
@@ -130,15 +138,17 @@
         """Swap the weights back after validation"""
         if self.use_for_val and self._cached_sd is not None:
             pl_module.load_state_dict(self._cached_sd)
             self._cached_sd = None
 
     def setup(self, trainer: Trainer, pl_module: LightningModule, stage: str) -> None:
         if isinstance(trainer.strategy, (FSDPStrategy, DeepSpeedStrategy, DDPStrategy)):
-            raise MisconfigurationException("I haven't tested this with FSDP, DeepSpeed, or DDP. Don't use it.")
+            raise MisconfigurationException(
+                "I haven't tested this with FSDP, DeepSpeed, or DDP. Don't use it."
+            )
 
     def state_dict(self) -> Dict[str, Any]:
         return {
             "state_dict": self.ema_weights,
             "step": self.step,
             "update_start": self.update_start,
             "update_time": self.update_time,
```

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/ALiBi.py` & `hnn_utils-0.3.1/hnn_utils/nn/ALiBi.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/RotaryEmbedding.py` & `hnn_utils-0.3.1/hnn_utils/nn/RotaryEmbedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 class XPOS(nn.Module):
     def __init__(self, head_dim: int, scale_base: int = 512):
         super().__init__()
 
         self.head_dim = head_dim
         self.scale_base = scale_base
 
-        self.register_buffer("scale", (torch.arange(0, head_dim, 2) + 0.4 * head_dim) / (1.4 * head_dim))
+        self.register_buffer(
+            "scale", (torch.arange(0, head_dim, 2) + 0.4 * head_dim) / (1.4 * head_dim)
+        )
         inv_freq = 1.0 / (10000 ** (torch.arange(0, head_dim, 2).float() / head_dim))
         self.register_buffer("inv_freq", inv_freq.unsqueeze(0))
 
     def forward(self, q: torch.Tensor, k: torch.Tensor):
         SL = q.shape[-2]
 
         seq = torch.arange(SL, device=q.device, dtype=q.dtype).unsqueeze(-1)
```

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/Transformer.py` & `hnn_utils-0.3.1/hnn_utils/nn/Transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,18 +331,18 @@
         dtype = query.dtype
 
         attn = flash_attn_kvpacked_func(
             q=q.bfloat16(),
             kv=kv.bfloat16(),
             causal=is_causal,
             alibi_slopes=slopes,
-        )
+        ).type(dtype)
 
         attn = rearrange(attn, "... h d -> ... (h d)")
-        return self.out_proj(attn).type(dtype)
+        return self.out_proj(attn)
 
 
 class SelfAttention(nn.Module):
     def __init__(
         self,
         embed_dim: int,
         heads: int,
@@ -405,18 +405,18 @@
         if hasattr(self, "alibi"):
             slopes = self.alibi.slopes.float().squeeze()
 
         dtype = x.dtype
 
         attn = flash_attn_qkvpacked_func(
             qkv=qkv.bfloat16(), causal=is_causal, alibi_slopes=slopes
-        )
+        ).type(dtype)
 
         attn = rearrange(attn, "... h d -> ... (h d)")
-        return self.out_proj(attn).type(dtype)
+        return self.out_proj(attn)
 
 
 def combine_masks(
     attn_mask: Optional[Tensor],
     pad_mask: Optional[Tensor],
     heads: int = 1,
     dtype: Optional[torch.dtype] = None,
@@ -465,9 +465,9 @@
     pad_mask: Optional[Tensor] = None,
     attn_mask: Optional[Tensor] = None,
 ):
     return (
         pad_mask is None
         and attn_mask is None
         and FLASH_AVAILABLE
-        and x.device.type != "cpu"
+        and x.device.type == "gpu"
     )
```

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/ffn.py` & `hnn_utils-0.3.1/hnn_utils/nn/ffn.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/functional.py` & `hnn_utils-0.3.1/hnn_utils/nn/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,10 +72,15 @@
     return ce
 
 
 def causal_mask(embed: Tensor) -> Tensor:
     """
     Creates a causal mask for self-attention.
     """
-    mask = torch.full((embed.shape[1], embed.shape[1]), -torch.inf, device=embed.device, dtype=embed.dtype)
+    mask = torch.full(
+        (embed.shape[1], embed.shape[1]),
+        -torch.inf,
+        device=embed.device,
+        dtype=embed.dtype,
+    )
     mask = torch.triu(mask, diagonal=1)
     return mask
```

### Comparing `hnn_utils-0.3.0/hnn_utils/nn/normalization.py` & `hnn_utils-0.3.1/hnn_utils/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.0/PKG-INFO` & `hnn_utils-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hnn_utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Various utilities used throughout my research
 Author: Haydn Jones
 Author-email: haydnjonest@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: einops (>=0.7.0,<0.8.0)
+Requires-Dist: lightning (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # hnn_utils
 Various utils / layers that might be used throughout my research.
 
 `pip install hnn-utils`
```

