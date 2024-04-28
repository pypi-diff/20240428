# Comparing `tmp/accmt-0.0.9.tar.gz` & `tmp/accmt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-0.0.9.tar", last modified: Wed Apr 10 06:54:47 2024, max compression
+gzip compressed data, was "accmt-1.0.0.tar", last modified: Sun Apr 28 01:05:15 2024, max compression
```

## Comparing `accmt-0.0.9.tar` & `accmt-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.353626 accmt-0.0.9/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.9/LICENSE
--rw-rw-rw-   0        0        0    12238 2024-04-10 06:54:47.351626 accmt-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    11517 2024-04-09 02:52:21.000000 accmt-0.0.9/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      837 2024-04-10 06:54:47.356627 accmt-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.299448 accmt-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.320440 accmt-0.0.9/src/accmt/
--rw-rw-rw-   0        0        0       96 2024-04-09 02:00:37.000000 accmt-0.0.9/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    23935 2024-04-10 06:51:48.000000 accmt-0.0.9/src/accmt/accmt.py
--rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-0.0.9/src/accmt/collate_fns.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.9/src/accmt/config.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:54:47.349629 accmt-0.0.9/src/accmt.egg-info/
--rw-rw-rw-   0        0        0    12238 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 06:54:47.000000 accmt-0.0.9/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 01:05:15.641313 accmt-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    13859 2024-04-28 01:05:15.640310 accmt-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13146 2024-04-21 20:01:57.000000 accmt-1.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      829 2024-04-28 01:05:15.644308 accmt-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 01:05:15.590314 accmt-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 01:05:15.610874 accmt-1.0.0/src/accmt/
+-rw-rw-rw-   0        0        0       96 2024-04-24 04:46:41.000000 accmt-1.0.0/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    24318 2024-04-28 01:02:19.000000 accmt-1.0.0/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.0/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.0/src/accmt/config.py
+drwxrwxrwx   0        0        0        0 2024-04-28 01:05:15.638308 accmt-1.0.0/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    13859 2024-04-28 01:05:15.000000 accmt-1.0.0/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-28 01:05:15.000000 accmt-1.0.0/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 01:05:15.000000 accmt-1.0.0/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-28 01:05:15.000000 accmt-1.0.0/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-28 01:05:15.000000 accmt-1.0.0/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-0.0.9/LICENSE` & `accmt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-0.0.9/PKG-INFO` & `accmt-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.9
+Version: 1.0.0
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
-Home-page: https://github.com/MartinPC-uls/AcceleratorModule
+Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
-Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
+Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
@@ -239,9 +239,52 @@
 ```
 
 This collator will handle padding to the longest example in a batch, as well as adding special tokens for padding in labels to compute loss without learning pad tokens. This is optimal to optimize training, since you're going to have tensors with the adecuated shape, and not a fixed one.
 
 The current implementation is quite similar to **transformers** library.
 
 
+## Teacher-Student support
+A Teacher-Student approach let's you mimic the behaviour of a bigger model (teacher) in a smaller model (student). This is a method for model distillation, useful to save computational resources and accelerate inference.
+
+To load teacher and student models, we can do the following in the module constructor:
+```python
+class TeacherStudentExampleModule(AcceleratorModule):
+    def __init__(self):
+        self.teacher = ... # teacher model
+        self.model = ...   # student model
+
+        self.teacher.eval() # set teacher to evaluation mode
+```
+
+During training, the teacher model will only provide outputs, and will not have its parameters updated.
+
+**NOTE**: In order to successfully load models into hardware, we must use **self.teacher** for teacher model, and **self.model** for student model.
+
+If using KL Divergence approach for the loss function, our **step** method will look something like this:
+```python
+import torch
+import torch.nn.functional as F
+# other imports...
+
+# other logic for module...
+
+def step(self, batch):
+    x = batch
+    with torch.no_grad(): # no gradients required for teacher model
+        teacher_logits = self.teacher(**x).logits
+
+    student_output = self.model(**x)
+    student_logits = student_output.logits
+
+    soft_prob = F.log_softmax(student_logits / self.T, dim=-1)
+    soft_targets = F.softmax(teacher_logits / self.T, dim=-1)
+
+    kd_loss = F.kl_div(soft_prob, soft_targets, reduction="batchmean") * (self.T**2)
+    loss = self.alpha * student_output.loss + (1. - self.alpha) * kd_loss
+
+    return loss
+```
+
+
 ## Notes
 I will continue to update this repository to add more features overtime. If you want to contribute to this little project, feel free to make a PR 🤗.
```

### Comparing `accmt-0.0.9/README.md` & `accmt-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -221,9 +221,52 @@
 ```
 
 This collator will handle padding to the longest example in a batch, as well as adding special tokens for padding in labels to compute loss without learning pad tokens. This is optimal to optimize training, since you're going to have tensors with the adecuated shape, and not a fixed one.
 
 The current implementation is quite similar to **transformers** library.
 
 
+## Teacher-Student support
+A Teacher-Student approach let's you mimic the behaviour of a bigger model (teacher) in a smaller model (student). This is a method for model distillation, useful to save computational resources and accelerate inference.
+
+To load teacher and student models, we can do the following in the module constructor:
+```python
+class TeacherStudentExampleModule(AcceleratorModule):
+    def __init__(self):
+        self.teacher = ... # teacher model
+        self.model = ...   # student model
+
+        self.teacher.eval() # set teacher to evaluation mode
+```
+
+During training, the teacher model will only provide outputs, and will not have its parameters updated.
+
+**NOTE**: In order to successfully load models into hardware, we must use **self.teacher** for teacher model, and **self.model** for student model.
+
+If using KL Divergence approach for the loss function, our **step** method will look something like this:
+```python
+import torch
+import torch.nn.functional as F
+# other imports...
+
+# other logic for module...
+
+def step(self, batch):
+    x = batch
+    with torch.no_grad(): # no gradients required for teacher model
+        teacher_logits = self.teacher(**x).logits
+
+    student_output = self.model(**x)
+    student_logits = student_output.logits
+
+    soft_prob = F.log_softmax(student_logits / self.T, dim=-1)
+    soft_targets = F.softmax(teacher_logits / self.T, dim=-1)
+
+    kd_loss = F.kl_div(soft_prob, soft_targets, reduction="batchmean") * (self.T**2)
+    loss = self.alpha * student_output.loss + (1. - self.alpha) * kd_loss
+
+    return loss
+```
+
+
 ## Notes
 I will continue to update this repository to add more features overtime. If you want to contribute to this little project, feel free to make a PR 🤗.
```

### Comparing `accmt-0.0.9/setup.cfg` & `accmt-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 302e 302e 390d 0a61 7574 686f  n = 0.0.9..autho
+00000020: 6e20 3d20 312e 302e 300d 0a61 7574 686f  n = 1.0.0..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
@@ -16,38 +16,37 @@
 000000f0: 6e69 6e67 2e0d 0a6c 6f6e 675f 6465 7363  ning...long_desc
 00000100: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000110: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000120: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000130: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
 00000140: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
 00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000160: 6f6d 2f4d 6172 7469 6e50 432d 756c 732f  om/MartinPC-uls/
-00000170: 4163 6365 6c65 7261 746f 724d 6f64 756c  AcceleratorModul
-00000180: 650d 0a70 726f 6a65 6374 5f75 726c 7320  e..project_urls 
-00000190: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-000001a0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000001b0: 622e 636f 6d2f 4d61 7274 696e 5043 2d75  b.com/MartinPC-u
-000001c0: 6c73 2f41 6363 656c 6572 6174 6f72 4d6f  ls/AcceleratorMo
-000001d0: 6475 6c65 2f69 7373 7565 730d 0a63 6c61  dule/issues..cla
-000001e0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000200: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000210: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000220: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-00000230: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-00000240: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-00000250: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000260: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-00000270: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000280: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000290: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-000002a0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-000002b0: 7265 7320 3d20 3e3d 332e 3130 0d0a 696e  res = >=3.10..in
-000002c0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000002d0: 200d 0a09 6163 6365 6c65 7261 7465 0d0a   ...accelerate..
-000002e0: 096e 756d 7079 0d0a 0950 7959 414d 4c0d  .numpy...PyYAML.
-000002f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000300: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000310: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-00000320: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000330: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000340: 300d 0a0d 0a                             0....
+00000160: 6f6d 2f67 6861 6e76 6572 742f 4163 6365  om/ghanvert/Acce
+00000170: 6c65 7261 746f 724d 6f64 756c 650d 0a70  leratorModule..p
+00000180: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000190: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001b0: 6d2f 6768 616e 7665 7274 2f41 6363 656c  m/ghanvert/Accel
+000001c0: 6572 6174 6f72 4d6f 6475 6c65 2f69 7373  eratorModule/iss
+000001d0: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
+000001e0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000200: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+00000210: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000220: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+00000230: 6674 7761 7265 204c 6963 656e 7365 0d0a  ftware License..
+00000240: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000250: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000260: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000270: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000280: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+00000290: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000002a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002b0: 332e 3130 0d0a 696e 7374 616c 6c5f 7265  3.10..install_re
+000002c0: 7175 6972 6573 203d 200d 0a09 6163 6365  quires = ...acce
+000002d0: 6c65 7261 7465 0d0a 096e 756d 7079 0d0a  lerate...numpy..
+000002e0: 0950 7959 414d 4c0d 0a0d 0a5b 6f70 7469  .PyYAML....[opti
+000002f0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000300: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000310: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000320: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000330: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `accmt-0.0.9/src/accmt/accmt.py` & `accmt-1.0.0/src/accmt/accmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import torch
-import warnings
 
 from abc import ABC
 from accelerate import Accelerator
 from accelerate.utils import LoggerType, ProjectConfiguration, tqdm
 from .config import read, save_status, read_status
 import torch.optim
 import torch.optim.lr_scheduler as lr_scheduler
@@ -223,14 +222,19 @@
                 Whether to shuffle validation DataLoader or not.
             model_saving_below_loss (`float`, *optional*, defaults to `float("inf")`):
                 Start saving model on this loss (based on `model_saving`). Default is always.
             collate_fn (`function`, *optional*, defaults to `None`):
                 Collate function to be implemented in dataloaders. If `module` overrides `collate_fn` from
                 `AcceleratorModule` class, then that function will be used instead of the one specified on
                 this constructor.
+            max_shard_size (`str`, *optional*, defaults to `10GB`):
+                Max model shard size to be used.
+            safe_serializartion (`bool`, *optional*, defaults to `False`):
+                Whether to save model using safe tensors or the traditional PyTorch way. If `True`, some tensors
+                will be lost.
         """
 
         self.hps_config = hps_file_config
         self.checkpoint = checkpoint
         self.resume = resume
         self.model_path = model_path
         self.model_saving = model_saving.lower()
@@ -278,14 +282,16 @@
         if self.hps_config is None:
             raise AttributeError("Cannot train without HPS file config.")
 
         model = getattr(module, "model", None)
         if model is None:
             raise AttributeError("'self.model' needs to be declared in the AcceleratorModule class.")
         
+        teacher = getattr(module, "teacher", None)
+        
         cfg = read(self.hps_config)
         hps = cfg["hps"]
         optim = hps["optim"]
         schlr = hps["scheduler"] if "scheduler" in hps else None
 
         if self.model_path is None:
             self.model_path = cfg["version"]
@@ -319,23 +325,18 @@
 
         optimizer = self._get_optimizer(optim, model)
         scheduler = None
         if schlr is not None:
             scheduler = self._get_scheduler(schlr, optimizer, -1, len(train_dataloader), hps["epochs"])
             # -1 for last_epoch since Accelerate will take care of recovering the progress
 
-        if "log_every" in cfg:
-            self.log_every = cfg["log_every"]
-            warnings.warn("'log_every' parameter in HPS config file is deprecated and it'll be removed in v1.0.0 "
-                          "Use 'log_every' in Trainer constructor instead.\n"
-                          "Using 'log_every' from HPS config file.")
-
-        model, train_dataloader, val_dataloader, optimizer, scheduler = self.accelerator.prepare(
-            model, train_dataloader, val_dataloader, optimizer, scheduler
+        model, train_dataloader, val_dataloader, optimizer, scheduler, teacher = self.accelerator.prepare(
+            model, train_dataloader, val_dataloader, optimizer, scheduler, teacher
         )
+
         if scheduler:
             self.accelerator.register_for_checkpointing(scheduler)
         self.accelerator.init_trackers(self.model_path.split("/")[-1])
 
         if self.resume:
             if os.path.exists(self.checkpoint):
                 self.accelerator.load_state(self.checkpoint)
@@ -453,22 +454,29 @@
         eval_global_step += eval_step
 
         return eval_global_step
 
     def _save_model(self, model, best_valid_loss, best_train_loss):
         state_dict = self.accelerator.get_state_dict(model)
         unwrapped_model = self.accelerator.unwrap_model(model)
-        unwrapped_model.save_pretrained(
-            self.model_path,
-            is_main_process=self.accelerator.is_main_process,
-            state_dict=state_dict,
-            max_shard_size=self.max_shard_size,
-            save_function=self.accelerator.save,
-            safe_serialization=self.safe_serialization
-        )
+        if getattr(unwrapped_model, "save_pretrained", None) is not None:
+            unwrapped_model.save_pretrained(
+                self.model_path,
+                is_main_process=self.accelerator.is_main_process,
+                state_dict=state_dict,
+                max_shard_size=self.max_shard_size,
+                save_function=self.accelerator.save,
+                safe_serialization=self.safe_serialization
+            )
+        else:
+            self.accelerator.save(
+                unwrapped_model,
+                f"{self.model_path}/pytorch_model.bin",
+                safe_serialization=self.safe_serialization
+            )
 
         save_status({
             "best_valid_loss": best_valid_loss,
             "best_train_loss": best_train_loss,
         }, to=f"{self.model_path}/status.json")
```

### Comparing `accmt-0.0.9/src/accmt/collate_fns.py` & `accmt-1.0.0/src/accmt/collate_fns.py`

 * *Files identical despite different names*

### Comparing `accmt-0.0.9/src/accmt.egg-info/PKG-INFO` & `accmt-1.0.0/src/accmt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.9
+Version: 1.0.0
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
-Home-page: https://github.com/MartinPC-uls/AcceleratorModule
+Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
-Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
+Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate
@@ -239,9 +239,52 @@
 ```
 
 This collator will handle padding to the longest example in a batch, as well as adding special tokens for padding in labels to compute loss without learning pad tokens. This is optimal to optimize training, since you're going to have tensors with the adecuated shape, and not a fixed one.
 
 The current implementation is quite similar to **transformers** library.
 
 
+## Teacher-Student support
+A Teacher-Student approach let's you mimic the behaviour of a bigger model (teacher) in a smaller model (student). This is a method for model distillation, useful to save computational resources and accelerate inference.
+
+To load teacher and student models, we can do the following in the module constructor:
+```python
+class TeacherStudentExampleModule(AcceleratorModule):
+    def __init__(self):
+        self.teacher = ... # teacher model
+        self.model = ...   # student model
+
+        self.teacher.eval() # set teacher to evaluation mode
+```
+
+During training, the teacher model will only provide outputs, and will not have its parameters updated.
+
+**NOTE**: In order to successfully load models into hardware, we must use **self.teacher** for teacher model, and **self.model** for student model.
+
+If using KL Divergence approach for the loss function, our **step** method will look something like this:
+```python
+import torch
+import torch.nn.functional as F
+# other imports...
+
+# other logic for module...
+
+def step(self, batch):
+    x = batch
+    with torch.no_grad(): # no gradients required for teacher model
+        teacher_logits = self.teacher(**x).logits
+
+    student_output = self.model(**x)
+    student_logits = student_output.logits
+
+    soft_prob = F.log_softmax(student_logits / self.T, dim=-1)
+    soft_targets = F.softmax(teacher_logits / self.T, dim=-1)
+
+    kd_loss = F.kl_div(soft_prob, soft_targets, reduction="batchmean") * (self.T**2)
+    loss = self.alpha * student_output.loss + (1. - self.alpha) * kd_loss
+
+    return loss
+```
+
+
 ## Notes
 I will continue to update this repository to add more features overtime. If you want to contribute to this little project, feel free to make a PR 🤗.
```

