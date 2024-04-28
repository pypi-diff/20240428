# Comparing `tmp/moltx-0.9.7.tar.gz` & `tmp/moltx-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-0.9.7.tar", last modified: Thu Apr 25 09:06:39 2024, max compression
+gzip compressed data, was "moltx-0.9.8.tar", last modified: Fri Apr 26 13:18:08 2024, max compression
```

## Comparing `moltx-0.9.7.tar` & `moltx-0.9.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:39.762081 moltx-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 09:06:33.000000 moltx-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-25 09:06:39.762081 moltx-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-25 09:06:33.000000 moltx-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:39.762081 moltx-0.9.7/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:39.762081 moltx-0.9.7/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-25 09:06:33.000000 moltx-0.9.7/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:39.762081 moltx-0.9.7/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-25 09:06:39.000000 moltx-0.9.7/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 09:06:39.000000 moltx-0.9.7/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:06:39.000000 moltx-0.9.7/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 09:06:39.000000 moltx-0.9.7/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 09:06:39.000000 moltx-0.9.7/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 09:06:33.000000 moltx-0.9.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 09:06:39.766081 moltx-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:06:33.000000 moltx-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:06:39.762081 moltx-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-25 09:06:33.000000 moltx-0.9.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-25 09:06:33.000000 moltx-0.9.7/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-25 09:06:33.000000 moltx-0.9.7/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-25 09:06:33.000000 moltx-0.9.7/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.931977 moltx-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 13:18:03.000000 moltx-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 13:18:08.931977 moltx-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-26 13:18:03.000000 moltx-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-26 13:18:03.000000 moltx-0.9.8/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.931977 moltx-0.9.8/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 13:18:08.000000 moltx-0.9.8/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 13:18:03.000000 moltx-0.9.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 13:18:08.931977 moltx-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:18:03.000000 moltx-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:18:08.927977 moltx-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-26 13:18:03.000000 moltx-0.9.8/tests/test_tokenizer.py
```

### Comparing `moltx-0.9.7/LICENSE` & `moltx-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/PKG-INFO` & `moltx-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.7
+Version: 0.9.8
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.7/README.md` & `moltx-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/data/spe_safe.txt` & `moltx-0.9.8/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/data/spe_smiles.txt` & `moltx-0.9.8/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/data/tks_safe.json` & `moltx-0.9.8/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/data/tks_smiles.json` & `moltx-0.9.8/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/datasets.py` & `moltx-0.9.8/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/models.py` & `moltx-0.9.8/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/nets.py` & `moltx-0.9.8/moltx/nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx/pipelines.py` & `moltx-0.9.8/moltx/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,38 +101,32 @@
         if s2 is None:
             tgt = self._tokenize(self.tokenizer.BOS)
             return src, tgt
         tgt = self._tokenize(f"{self.tokenizer.BOS}{s2}")
         return src, tgt
 
     # gentype: greedy, beam
-    def __call__(self, smiles: str, k: int = 1, gentype: str = 'greedy') -> typing.Mapping:
-        assert k <= 10
+    def __call__(self, smiles: str, gentype: str = 'greedy') -> typing.Mapping:
         src, tgt = self._model_args(smiles)
         m = getattr(self, f"_call_{gentype}")
-        smis, probs = m(src, tgt, k)
+        smi, prob = m(src, tgt)
         return {
-            'smiles': smis,
-            'probabilities': probs
+            'smiles': smi,
+            'probability': prob
         }
 
-    def _call_greedy(self, src: torch.Tensor, tgt: torch.Tensor, k: int) -> typing.Mapping:
-        smiles, probs = [], []
-        for _ in range(k):
-            smi, prob = self._greedy_search(src=src, tgt=tgt)
-            smiles.append(smi)
-            probs.append(prob)
-        return smiles, probs
+    def _call_greedy(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
+        return self._greedy_search(src=src, tgt=tgt)
 
-    def _call_beam(self, src: torch.Tensor, tgt: torch.Tensor, k: int) -> typing.Mapping:
-        beam_k = max(k, 3)
+    def _call_beam(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
+        beam_k = 3
         src = src.unsqueeze(0).repeat(beam_k, 1)
         tgt = tgt.unsqueeze(0).repeat(beam_k, 1)
         smiles, probs = self._beam_search(src=src, tgt=tgt)
-        return smiles[:k], probs[:k]
+        return smiles[0], probs[0]
 
 
 class AdaMRClassifier(AdaMR):
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
         return super()._model_args(smiles, f"{smiles}{self.tokenizer.EOS}")
 
     def __call__(self, smiles: str) -> typing.Mapping:
```

### Comparing `moltx-0.9.7/moltx/tokenizers.py` & `moltx-0.9.8/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/moltx.egg-info/PKG-INFO` & `moltx-0.9.8/moltx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.7
+Version: 0.9.8
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.7/moltx.egg-info/SOURCES.txt` & `moltx-0.9.8/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/setup.cfg` & `moltx-0.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/tests/test_datasets.py` & `moltx-0.9.8/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/tests/test_nets.py` & `moltx-0.9.8/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.7/tests/test_pipelines.py` & `moltx-0.9.8/tests/test_pipelines.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 import pytest
 from moltx import pipelines, models
 
 
 def test_AdaMR(tokenizer, model_conf):
     pipeline = pipelines.AdaMR(tokenizer, models.AdaMR(model_conf))
-    out = pipeline("CC[N+](C)(C)Br", k=1)
-    assert 'smiles' in out and 'probabilities' in out
-    assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
-    assert isinstance(out['probabilities'], list) and len(
-        out['probabilities']) == 1
-
-    out = pipeline("CC[N+](C)(C)Br", k=2, gentype='beam')
-    assert 'smiles' in out and 'probabilities' in out
-    assert isinstance(out['smiles'], list) and len(out['smiles']) == 2 and isinstance(out['smiles'][0], str)
-    assert isinstance(out['probabilities'], list) and len(
-        out['probabilities']) == 2
+    out = pipeline("CC[N+](C)(C)Br")
+    assert 'smiles' in out and 'probability' in out
+    assert isinstance(out['smiles'], str)
 
-    out = pipeline("CC[N+](C)(C)Br", k=1, gentype='beam')
-    assert 'smiles' in out and 'probabilities' in out
-    assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
-    assert isinstance(out['probabilities'], list) and len(
-        out['probabilities']) == 1
+    out = pipeline("CC[N+](C)(C)Br", gentype='beam')
+    assert 'smiles' in out and 'probability' in out
+    assert isinstance(out['smiles'], str)
 
 
 def test_AdaMRClassifier(tokenizer, model_conf):
     pipeline = pipelines.AdaMRClassifier(
         tokenizer, models.AdaMRClassifier(num_classes=2, conf=model_conf))
     out = pipeline("CC[N+](C)(C)Br")
     assert 'label' in out and 'probability' in out
```

### Comparing `moltx-0.9.7/tests/test_tokenizer.py` & `moltx-0.9.8/tests/test_tokenizer.py`

 * *Files identical despite different names*

