# Comparing `tmp/generate_sequences-0.0.3.tar.gz` & `tmp/generate_sequences-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.3.tar", last modified: Tue Apr 23 06:23:22 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.4.tar", last modified: Sun Apr 28 15:32:10 2024, max compression
```

## Comparing `generate_sequences-0.0.3.tar` & `generate_sequences-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.913272 generate_sequences-0.0.3/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.917271 generate_sequences-0.0.3/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:32:10.798162 generate_sequences-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-28 15:32:10.798162 generate_sequences-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:32:10.794162 generate_sequences-0.0.4/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:32:10.794162 generate_sequences-0.0.4/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-28 15:32:10.000000 generate_sequences-0.0.4/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-28 15:32:10.000000 generate_sequences-0.0.4/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:32:10.000000 generate_sequences-0.0.4/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-28 15:32:10.000000 generate_sequences-0.0.4/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 15:32:10.000000 generate_sequences-0.0.4/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-28 15:28:53.000000 generate_sequences-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:32:10.798162 generate_sequences-0.0.4/setup.cfg
```

### Comparing `generate_sequences-0.0.3/LICENSE` & `generate_sequences-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.3/PKG-INFO` & `generate_sequences-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `generate_sequences-0.0.3/generate_sequences/generate.py` & `generate_sequences-0.0.4/generate_sequences/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,25 @@
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda",
         temperature: float = 1.0,
         use_tqdm: bool = True,
+        multinomial_sampling: bool = False,
     ) -> None:
         self.device = device
         self.use_tqdm = use_tqdm
         self.max_length = max_length
         self.batch_size = batch_size
         self.generate_fn = generate_fn
         self.eos_token_id = eos_token_id
         self.decoder_start_token_id = decoder_start_token_id
         self.temperature = temperature
+        self.multinomial_sampling = multinomial_sampling
 
     def get_batches(self, inputs: Union[List[torch.Tensor], List[str]]) -> Iterator[List[str]]:
         for i in tqdm(
             range(0, len(inputs), self.batch_size),
             disable=not self.use_tqdm,
             desc="Generating Sequences",
             total=len(inputs) // self.batch_size,
@@ -43,16 +45,18 @@
 
 
 class GreedyGenerator(BaseGenerator):
     @torch.no_grad()
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         outputs = []
         # add user warning if temperature is not 1.0 that greedy search is not appropriate
-        if self.temperature != 1.0:
-            warnings.warn("Temperature does not have an affect on Greedy search!")
+        if self.temperature != 1.0 and not self.multinomial_sampling:
+            warnings.warn(
+                "Temperature does not have an affect on Greedy search if multinomial sampling is set to False! If forgot to add multinomail sampling, set `multinomial_sampling=True` to the generator."
+            )
 
         for batch_inputs in self.get_batches(inputs):
             batch_size = len(batch_inputs)
             decoder_inputs = torch.full(
                 (batch_size, self.max_length),
                 self.eos_token_id,  # Pre-fill with EOS; only overwrite if generating
                 dtype=torch.long,
@@ -64,15 +68,22 @@
             for step in range(1, self.max_length):
                 if finished_mask.all():
                     break  # Stop if all sequences are finished
                 batch_outputs = self.generate_fn(batch_inputs, decoder_inputs[:, :step])
                 batch_outputs = batch_outputs[:, -1, :]  # Get last tokens' outputs for the batch
                 next_tokens = batch_outputs / self.temperature
                 next_tokens = F.softmax(next_tokens, dim=-1)
-                next_tokens = torch.argmax(next_tokens, dim=-1)
+                # check for multinomial sampling
+                if self.multinomial_sampling:
+                    next_tokens = torch.multinomial(
+                        next_tokens,
+                        num_samples=1,
+                    ).squeeze()
+                else:
+                    next_tokens = torch.argmax(next_tokens, dim=-1)
                 not_finished = ~finished_mask
                 decoder_inputs[not_finished, step] = next_tokens[not_finished]
                 finished_mask |= next_tokens == self.eos_token_id  # Update finished sequences
             outputs += decoder_inputs
         return outputs
 
 
@@ -145,14 +156,15 @@
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda",
         temperature: float = 1.0,
         use_tqdm: bool = True,
+        multinomial_sampling: bool = False,
         beam_width: int = 4,
         length_penalty: float = 1.0,
         beam_nodes_ordering_function: Callable[
             [BeamNode, int, float], float
         ] = default_beam_nodes_ordering_fn,
     ) -> None:
         super().__init__(
@@ -160,14 +172,15 @@
             eos_token_id,
             generate_fn,
             max_length,
             batch_size,
             device,
             temperature,
             use_tqdm,
+            multinomial_sampling,
         )
         self.beam_width = beam_width
         self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
     @torch.no_grad
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
@@ -205,15 +218,24 @@
                     decoder_input_ids = torch.LongTensor(
                         [topk_nodes[k].tokens for topk_nodes in best_beams_nodes]
                     ).to(self.device)
                     batch_outputs = self.generate_fn(batch, decoder_input_ids)
                     batch_outputs = batch_outputs[:, -1, :]
                     batch_outputs = batch_outputs / self.temperature
                     batch_outputs = F.log_softmax(batch_outputs, dim=-1)
-                    topk_scores, topk_indices = torch.topk(batch_outputs, self.beam_width)
+                    # check for multinomial sampling
+                    if self.multinomial_sampling:
+                        topk_indices = torch.multinomial(
+                            torch.exp(batch_outputs),
+                            self.beam_width,
+                            replacement=True,
+                        )
+                        topk_scores = batch_outputs.gather(1, topk_indices)
+                    else:
+                        topk_scores, topk_indices = torch.topk(batch_outputs, self.beam_width)
                     for beam_index, beam in enumerate(next_beams):
                         # Check if this sequence has already reached eos token
                         if best_beams_nodes[beam_index][k].tokens[-1] == self.eos_token_id:
                             beam.add(
                                 BeamNode(
                                     tokens=best_beams_nodes[beam_index][k].tokens
                                     + [self.eos_token_id],
```

### Comparing `generate_sequences-0.0.3/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.4/generate_sequences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `generate_sequences-0.0.3/pyproject.toml` & `generate_sequences-0.0.4/pyproject.toml`

 * *Files identical despite different names*

