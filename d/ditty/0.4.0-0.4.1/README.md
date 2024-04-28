# Comparing `tmp/ditty-0.4.0.tar.gz` & `tmp/ditty-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.4.0.tar", last modified: Tue May 30 22:17:13 2023, max compression
+gzip compressed data, was "ditty-0.4.1.tar", last modified: Sun Apr 28 04:17:56 2024, max compression
```

## Comparing `ditty-0.4.0.tar` & `ditty-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.4.0/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-30 22:17:13.466307 ditty-0.4.0/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     3138 2023-05-29 11:53:59.000000 ditty-0.4.0/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.462308 ditty-0.4.0/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/lib/ditty/
--rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.4.0/lib/ditty/__init__.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.4.0/lib/ditty/data.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     7408 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/pipeline.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     8324 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/trainer.py
--rw-rw-r--   0 crow      (1000) crow      (1000)      311 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/utils.py
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      302 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-30 22:17:13.466307 ditty-0.4.0/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-30 22:16:23.000000 ditty-0.4.0/setup.py
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.312009 ditty-0.4.1/
+-rw-r--r--   0 crow       (501) staff       (20)    11357 2023-12-10 02:25:24.000000 ditty-0.4.1/LICENSE
+-rw-r--r--   0 crow       (501) staff       (20)     3616 2024-04-28 04:17:56.311943 ditty-0.4.1/PKG-INFO
+-rw-r--r--   0 crow       (501) staff       (20)     3173 2023-12-10 08:48:25.000000 ditty-0.4.1/README.md
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.307612 ditty-0.4.1/lib/
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.310674 ditty-0.4.1/lib/ditty/
+-rw-r--r--   0 crow       (501) staff       (20)        0 2023-12-10 02:25:24.000000 ditty-0.4.1/lib/ditty/__init__.py
+-rw-r--r--   0 crow       (501) staff       (20)     5366 2023-12-10 09:23:34.000000 ditty-0.4.1/lib/ditty/data.py
+-rw-r--r--   0 crow       (501) staff       (20)     7440 2023-12-10 08:46:51.000000 ditty-0.4.1/lib/ditty/pipeline.py
+-rw-r--r--   0 crow       (501) staff       (20)     9272 2023-12-10 21:22:42.000000 ditty-0.4.1/lib/ditty/trainer.py
+-rw-r--r--   0 crow       (501) staff       (20)      311 2023-12-10 02:25:24.000000 ditty-0.4.1/lib/ditty/utils.py
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.311682 ditty-0.4.1/lib/ditty.egg-info/
+-rw-r--r--   0 crow       (501) staff       (20)     3616 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/PKG-INFO
+-rw-r--r--   0 crow       (501) staff       (20)      302 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/SOURCES.txt
+-rw-r--r--   0 crow       (501) staff       (20)        1 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/dependency_links.txt
+-rw-r--r--   0 crow       (501) staff       (20)       56 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/requires.txt
+-rw-r--r--   0 crow       (501) staff       (20)        6 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/top_level.txt
+-rw-r--r--   0 crow       (501) staff       (20)      103 2024-04-28 04:17:56.312256 ditty-0.4.1/setup.cfg
+-rw-r--r--   0 crow       (501) staff       (20)      639 2024-04-28 04:14:49.000000 ditty-0.4.1/setup.py
```

### Comparing `ditty-0.4.0/LICENSE` & `ditty-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.4.0/PKG-INFO` & `ditty-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: accelerate
+Requires-Dist: transformers
+Requires-Dist: datasets
+Requires-Dist: bitsandbytes
+Requires-Dist: fire
+Requires-Dist: peft
 
 # Ditty
 
 A simple fine-tune.
 
 ## What
 A very simple library for finetuning Huggingface Pretrained AutoModelForCausalLM such as GPTNeoX, leveraging Huggingface Accelerate, Transformers, Datasets and Peft
@@ -52,15 +58,16 @@
 Data wraps an HF Dataset and can configure length grouped sampling and random sampling, as well as handling collation, batching, seeds, removing unused columns and a few other things.
 
 The primary way of using this class is through the `prepare` method which takes a list of operations to perform against the dataset. These are normal operations like `map` and `filter`.
 
 Example:
 ```python
 data = Data(
-    load_args=(self.dataset_name, self.dataset_language),
+    load_kwargs={"path": self.dataset_name, "name":
+                 self.dataset_language},
     tokenizer=self.tokenizer,
     seed=self.seed,
     batch_size=self.batch_size,
     grad_accum=self.grad_accum,
 )
 
 ....sic
```

### Comparing `ditty-0.4.0/README.md` & `ditty-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 Data wraps an HF Dataset and can configure length grouped sampling and random sampling, as well as handling collation, batching, seeds, removing unused columns and a few other things.
 
 The primary way of using this class is through the `prepare` method which takes a list of operations to perform against the dataset. These are normal operations like `map` and `filter`.
 
 Example:
 ```python
 data = Data(
-    load_args=(self.dataset_name, self.dataset_language),
+    load_kwargs={"path": self.dataset_name, "name":
+                 self.dataset_language},
     tokenizer=self.tokenizer,
     seed=self.seed,
     batch_size=self.batch_size,
     grad_accum=self.grad_accum,
 )
 
 ....sic
```

### Comparing `ditty-0.4.0/lib/ditty/data.py` & `ditty-0.4.1/lib/ditty/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,51 +4,62 @@
 from torch.utils.data import DataLoader, RandomSampler
 import datasets
 from transformers.trainer_pt_utils import (
     LabelSmoother,
     LengthGroupedSampler,
 )
 from transformers.trainer_utils import RemoveColumnsCollator, set_seed
-from transformers.data.data_collator import DataCollator, DataCollatorWithPadding, DataCollatorForLanguageModeling, default_data_collator
+from transformers.data.data_collator import (
+    DataCollator,
+    DataCollatorWithPadding,
+    DataCollatorForLanguageModeling,
+    default_data_collator,
+)
 from transformers import PreTrainedTokenizerBase
 from typing import Callable
 
 from logging import getLogger
 
 logger = getLogger()
 
+
 @dataclass(kw_only=True)
 class Data:
     dataset: datasets.Dataset | None = None
     split: str = "train"
     tokenizer: PreTrainedTokenizerBase
     seed: Optional[int] = None
     batch_size: int = 8
     grad_accum: int = 1
     length_column_name: Optional[str] = None
     group_by_length: bool = False
     dataloader_num_workers: int = 0
     dataloader_pin_memory: bool = True
     dataloader_drop_last: bool = False
-    load_args: Optional[list] = None
+    load_kwargs: Optional[dict] = None
     collator: Optional[DataCollator] = None
     remove_unused_columns: bool = False
 
     def __post_init__(self):
-        if self.dataset is None and self.load_args is None:
-            raise ValueError("Dataset and load_args cannot both be None. Please either pass an instance of Dataset or a list of args to load the dataset with.")
-        
+        if self.dataset is None and self.load_kwargs is None:
+            raise ValueError(
+                "dataset and load_kwargs cannot both be None.  Please either pass an instance of Dataset or a dict of args to load the dataset with."
+            )
+
         if self.dataset is None:
-            self.dataset = datasets.load_dataset(*self.load_args)[self.split]
+            kwargs = self.load_kwargs or {}
+
+            self.dataset = datasets.load_dataset(**kwargs)[self.split]
 
         if not self.collator:
-            collator = DataCollatorForLanguageModeling(tokenizer=self.tokenizer, return_tensors="pt", mlm=False)
+            collator = DataCollatorForLanguageModeling(
+                tokenizer=self.tokenizer, return_tensors="pt", mlm=False
+            )
             self.collator = collator
 
-
     def _get_sampler(self) -> Optional[torch.utils.data.Sampler]:
         generator = torch.Generator()
 
         if self.seed:
             generator.manual_seed(self.seed)
 
         # Build the sampler.
@@ -66,15 +77,16 @@
                 model_input_name=model_input_name,
                 generator=generator,
             )
         else:
             return RandomSampler(self.dataset, generator=generator)
 
     def _get_collator_with_removed_columns(
-        self, data_collator: Callable,
+        self,
+        data_collator: Callable,
     ) -> Callable:
         """Wrap the data collator in a callable removing unused columns."""
         if not self.remove_unused_columns:
             return data_collator
 
         remove_columns_collator = RemoveColumnsCollator(
             data_collator=data_collator,
@@ -101,24 +113,24 @@
             op = getattr(self.dataset, op_name)
 
             if not func:
                 self.dataset = op(**kwargs)
             else:
                 self.dataset = op(func, **kwargs)
 
-        return self._get_dataloader()        
+        return self._get_dataloader()
 
     def _seed_worker(self):
         if not self.seed:
             worker_seed = torch.initial_seed() % 2**32
         else:
             worker_seed = self.seed
 
         set_seed(worker_seed)
-    
+
     def _get_dataloader(self) -> DataLoader:
         """
         Returns a [`~torch.utils.data.DataLoader`].
 
         Will use no sampler if `dataset` does not implement `__len__`, a random sampler (adapted to distributed
         training if necessary) otherwise.
 
@@ -146,8 +158,8 @@
             batch_size=self.batch_size,
             sampler=sampler,
             collate_fn=data_collator,
             drop_last=self.dataloader_drop_last,
             num_workers=self.dataloader_num_workers,
             pin_memory=self.dataloader_pin_memory,
             worker_init_fn=self._seed_worker,
-        )
+        )
```

### Comparing `ditty-0.4.0/lib/ditty/pipeline.py` & `ditty-0.4.1/lib/ditty/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         fp32_cpu_offload=False,
         load_checkpoint=True,
         checkpoint_every=1000,
         gradient_checkpointing=True,
         experimental=False,
         block_size=2048,
         use_bfloat16=False,
-        model_load_kwargs={},
+        model_load_kwargs={"device_map": "auto"},
     ):
         self.output_dir = output_dir
         self.dataset_name = dataset_name
         self.dataset_language = dataset_language
         self.model_name_or_path = model_name_or_path
         self.hf_hub_token = hf_hub_token
         self.hf_hub_model_id = hf_hub_model_id
@@ -89,15 +89,16 @@
 
     def dataset(self) -> DataLoader:
         """
         Subclass Pipeline and customize for your own dataset.
         """
 
         data = Data(
-            load_args=(self.dataset_name, self.dataset_language),
+            load_kwargs={"path": self.dataset_name, "name":
+                         self.dataset_language},
             tokenizer=self.tokenizer,
             seed=self.seed,
             batch_size=self.batch_size,
             grad_accum=self.grad_accum,
         )
 
         columns = data.dataset.features
@@ -134,15 +135,14 @@
         if self.tokenizer.pad_token_id is None:
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
 
         data = self.dataset()
 
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_name_or_path,
-            device_map="auto",
             quantization_config=self.bnb_config,
             **self.model_load_kwargs,
         )
 
         target_modules = None
 
         print(self.model)
```

### Comparing `ditty-0.4.0/lib/ditty/trainer.py` & `ditty-0.4.1/lib/ditty/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,44 +17,52 @@
 import contextlib
 
 from peft import PeftModelForCausalLM
 from logging import getLogger
 from typing import Optional
 import os
 
-from transformers import (
-    PreTrainedModel
-)
+from transformers import PreTrainedModel
+
 
 def default_scheduler_factory(optimizer):
     return torch.optim.lr_scheduler.StepLR(optimizer, step_size=30, gamma=0.1)
 
+
+def get_number_from_checkpoint(filename):
+    parts = filename.split("_")
+    if len(parts) != 2 or not parts[1].isdigit():
+        return None
+    return int(parts[1])
+
+
 logger = getLogger()
 
+
 @dataclass(kw_only=True)
-class TrainerState():
+class TrainerState:
     epoch: int = 0
     steps: int = 0
     global_loss: int = 0
 
     def state_dict(self):
         return {
             "epoch": self.epoch,
             "steps": self.steps,
             "global_loss": self.global_loss,
         }
-    
+
     def load_state_dict(self, state_dict):
         self.epoch = state_dict["epoch"]
         self.steps = state_dict["steps"]
         self.global_loss = state_dict["global_loss"]
 
 
 @dataclass(kw_only=True)
-class Trainer():
+class Trainer:
     model: nn.Module
     optimizer: torch.optim.Optimizer
     dataset: DataLoader
     device: torch.device
     scheduler: torch.optim.lr_scheduler._LRScheduler | None = None
     use_scheduler: bool = True
     grad_accum: int = 1
@@ -84,121 +92,158 @@
 
         acc_kwargs = {
             "gradient_accumulation_steps": self.grad_accum,
             "project_dir": self.output_dir,
             "project_config": ProjectConfiguration(
                 project_dir=self.output_dir,
                 automatic_checkpoint_naming=True,
-            )
+            ),
         }
 
         acc_kwargs = {**acc_kwargs, **self.accelerator_kwargs}
 
         self.accelerator = Accelerator(**acc_kwargs)
         device = self.accelerator.device
         self.device = device
 
         if self.use_scheduler:
-            self.model, self.optimizer, self.dataset, self.scheduler = self.accelerator.prepare(self.model, self.optimizer, self.dataset, self.scheduler)
+            (
+                self.model,
+                self.optimizer,
+                self.dataset,
+                self.scheduler,
+            ) = self.accelerator.prepare(
+                self.model, self.optimizer, self.dataset, self.scheduler
+            )
 
             self.accelerator.register_for_checkpointing(self.scheduler)
         else:
-            self.model, self.optimizer, self.dataset = self.accelerator.prepare(self.model, self.optimizer, self.dataset)
+            self.model, self.optimizer, self.dataset = self.accelerator.prepare(
+                self.model, self.optimizer, self.dataset
+            )
 
         self.state = TrainerState()
         self.accelerator.register_for_checkpointing(self.state)
 
     def _save_dist(self):
         model = self.accelerator.unwrap_model(self.model)
         model_state = model.state_dict()
         model.save_pretrained(f"{self.output_dir}/dist", state_dict=model_state)
 
     def _save(self, no_dist=False):
-        self.accelerator.wait_for_everyone() 
+        self.accelerator.wait_for_everyone()
         self.accelerator.save_state()
         if not no_dist:
             self._save_dist()
 
+    def _load_last_checkpoint(self):
+        try:
+            checkpoints_dir = f"{self.output_dir}/checkpoints/"
+
+            if os.path.exists(checkpoints_dir) and os.listdir(checkpoints_dir):
+                files = os.listdir(checkpoints_dir)
+                checkpoint_files = [
+                    f
+                    for f in files
+                    if f.startswith("checkpoint_")
+                    and get_number_from_checkpoint(f) is not None
+                ]
+                checkpoint_files_sorted = sorted(
+                    checkpoint_files, key=get_number_from_checkpoint
+                )
+
+                if checkpoint_files_sorted:
+                    last_cp = checkpoint_files_sorted[-1]
+                    logger.info(f"Trying to load checkpoint: {last_cp}....")
+                    self.accelerator.load_state(
+                        f"{self.output_dir}/checkpoints/{last_cp}"
+                    )
+
+                    # Update the iteration number so that the next checkpoint name is increased by 1
+                    last_cp_num = last_cp.split("_")[-1]
+                    self.accelerator.project_configuration.iteration = (
+                        int(last_cp_num) + 1
+                    )
+                    return last_cp
+
+        except FileNotFoundError as e:
+            logger.warning(e)
+        return None
+
     def _train_accelerate(self, epochs=1, max_steps=None):
-        context_manager =  contextlib.nullcontext()
+        context_manager = contextlib.nullcontext()
 
         if self.fp16:
-            context_manager = torch.cuda.amp.autocast(cache_enabled=False, dtype=self.f16_dtype)
-
+            context_manager = torch.cuda.amp.autocast(
+                cache_enabled=False, dtype=self.f16_dtype
+            )
 
         self.model.train()
         total_batches = len(self.dataset) * epochs
         start_time = time.time()
-        
-        
-       
-        if self.load_checkpoint:
-            try:
-                checkpoints_dir = f"{self.output_dir}/checkpoints/"
-                
-                if os.path.exists(checkpoints_dir) and os.listdir(checkpoints_dir):
-                    last_cp = sorted(os.listdir(checkpoints_dir))[-1]
-                    logger.info(f"Trying to load checkpoint: {last_cp}....")
-                    last_cp = sorted(os.listdir(f"{self.output_dir}/checkpoints/"))[-1]
-                    logger.info(f"Trying to load checkpoint: {last_cp}....")
-                    self.accelerator.load_state(f"{self.output_dir}/checkpoints/{last_cp}")
 
-                    # Update the iteration number so that the next checkpoint name is increased by 1
-                    last_cp_num = last_cp.split("_")[-1]
-                    self.accelerator.project_configuration.iteration = int(last_cp_num) + 1
-                    logger.info("Checkpoint loaded.")
-                else:
-                    logger.warning("No checkpoint found, starting from scratch.")
-                    self._save(no_dist=True)
-                    
-            except FileNotFoundError as e:
-                logger.warning(e)
+        if self.load_checkpoint:
+            last_cp = self._load_last_checkpoint()
+            if last_cp:
+                logger.info(f"Checkpoint loaded: {last_cp}.")
+            else:
                 logger.warning("No checkpoint found, starting from scratch.")
                 self._save(no_dist=True)
+
         else:
             self._save(no_dist=True)
 
         atexit.register(self._save)
         for ep in range(self.state.epoch, epochs):
             dataset = self.dataset
 
             if self.state.steps > 0:
-                dataset = self.accelerator.skip_first_batches(self.dataset, self.state.steps)
+                dataset = self.accelerator.skip_first_batches(
+                    self.dataset, self.state.steps
+                )
 
             for batch_idx, batch in enumerate(dataset):
                 with self.accelerator.accumulate(self.model):
                     with context_manager:
                         outputs = self.model(**batch)
-                        loss = outputs["loss"] if isinstance(outputs, dict) else outputs[0]
+                        loss = (
+                            outputs["loss"] if isinstance(outputs, dict) else outputs[0]
+                        )
 
                     self.accelerator.backward(loss)
-
+                    batch_loss = loss.item()
                     self.optimizer.step()
                     if self.use_scheduler:
                         self.scheduler.step()
                     self.optimizer.zero_grad()
 
-                    batch_loss = loss.item() / self.grad_accum
-
                     # calculate current epoch as decimal
                     total_batches_done = ep * len(self.dataset) + batch_idx
                     current_epoch_decimal = total_batches_done / total_batches
 
                     # calculate time elapsed and estimate remaining time
                     time_elapsed = time.time() - start_time
                     batches_remaining = total_batches - total_batches_done
-                    estimated_time_remaining = (time_elapsed / total_batches_done) * batches_remaining if total_batches_done > 0 else 0
+                    estimated_time_remaining = (
+                        (time_elapsed / total_batches_done) * batches_remaining
+                        if total_batches_done > 0
+                        else 0
+                    )
 
                     # convert estimated_time_remaining to format: dd days, hh hours, mm minutes, ss seconds
-                    estimated_time_remaining_ddhhmmss = convert_seconds_to_string_time(estimated_time_remaining)
+                    estimated_time_remaining_ddhhmmss = convert_seconds_to_string_time(
+                        estimated_time_remaining
+                    )
 
                     # calculate percentage done
                     percent_done = (total_batches_done / total_batches) * 100
 
-                    print(f"Epoch {current_epoch_decimal:.2f} | Batch {batch_idx}/{len(self.dataset)} | Loss {batch_loss} | {percent_done:.2f}% done | Estimated time remaining: {estimated_time_remaining_ddhhmmss}")
+                    print(
+                        f"Epoch {current_epoch_decimal:.2f} | Batch {batch_idx}/{len(self.dataset)} | Loss {batch_loss} | {percent_done:.2f}% done | Estimated time remaining: {estimated_time_remaining_ddhhmmss}"
+                    )
 
                     self.state.global_loss += batch_loss
 
                 self.state.steps += 1
                 if max_steps is not None and batch_idx >= max_steps:
                     break
 
@@ -215,11 +260,12 @@
         logger.info("***** Running training *****")
         logger.info(f"  Num examples = {len(self.dataset):,}")
         logger.info(f"  Num Epochs = {epochs:,}")
         if max_steps:
             logger.info(f"  Total optimization steps = {max_steps:,}")
         logger.info(f"  Instantaneous batch size per device = {self.batch_size:,}")
         logger.info(f"  Gradient Accumulation steps = {self.grad_accum}")
-        logger.info(f"  Number of trainable parameters = {get_model_param_count(self.model, trainable_only=True):,}")
+        logger.info(
+            f"  Number of trainable parameters = {get_model_param_count(self.model, trainable_only=True):,}"
+        )
 
         return self._train_accelerate(epochs=epochs, max_steps=max_steps)
-
```

### Comparing `ditty-0.4.0/lib/ditty.egg-info/PKG-INFO` & `ditty-0.4.1/lib/ditty.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: accelerate
+Requires-Dist: transformers
+Requires-Dist: datasets
+Requires-Dist: bitsandbytes
+Requires-Dist: fire
+Requires-Dist: peft
 
 # Ditty
 
 A simple fine-tune.
 
 ## What
 A very simple library for finetuning Huggingface Pretrained AutoModelForCausalLM such as GPTNeoX, leveraging Huggingface Accelerate, Transformers, Datasets and Peft
@@ -52,15 +58,16 @@
 Data wraps an HF Dataset and can configure length grouped sampling and random sampling, as well as handling collation, batching, seeds, removing unused columns and a few other things.
 
 The primary way of using this class is through the `prepare` method which takes a list of operations to perform against the dataset. These are normal operations like `map` and `filter`.
 
 Example:
 ```python
 data = Data(
-    load_args=(self.dataset_name, self.dataset_language),
+    load_kwargs={"path": self.dataset_name, "name":
+                 self.dataset_language},
     tokenizer=self.tokenizer,
     seed=self.seed,
     batch_size=self.batch_size,
     grad_accum=self.grad_accum,
 )
 
 ....sic
```

### Comparing `ditty-0.4.0/setup.py` & `ditty-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.4.0',
+    version='0.4.1',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

