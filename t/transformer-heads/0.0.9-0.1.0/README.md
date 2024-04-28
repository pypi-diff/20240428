# Comparing `tmp/transformer_heads-0.0.9.tar.gz` & `tmp/transformer_heads-0.1.0.tar.gz`

## Comparing `transformer_heads-0.0.9.tar` & `transformer_heads-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.readthedocs.yaml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0    66320 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/_images/example_architecture.svg
--rw-r--r--   0        0        0    64089 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/_images/multi_linear_probe.svg
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/make.bat
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/requirements.txt
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/conf.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/getting_started.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/images.rst
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/index.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/modules.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/readme.rst
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.model.rst
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.tests.rst
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/docs/source/transformer_heads.util.rst
--rw-r--r--   0        0        0    85722 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/joint_multitask_learning.ipynb
--rw-r--r--   0        0        0    48378 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/linear_probe.ipynb
--rw-r--r--   0        0        0    70663 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/multi_linear_probe.ipynb
--rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/saving_and_loading.ipynb
--rw-r--r--   0        0        0    74344 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_full_finetune.ipynb
--rw-r--r--   0        0        0   722448 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_linear_probe.ipynb
--rw-r--r--   0        0        0    79822 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/gpt2/text_classification_qlora.ipynb
--rw-r--r--   0        0        0    59619 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/llama/linear_probe.ipynb
--rw-r--r--   0        0        0    81976 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/notebooks/llama/multi_linear_probe.ipynb
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/other/pip_freeze.txt
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/paper_shredder.bash
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/remove_eval_spam.py
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/run_slurm.sh
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/scripts/shredder_papers.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/__init__.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/config.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/constants.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/__init__.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/head.py
--rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/model/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/__init__.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/test_load_model.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/tests/test_loss_compute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/evaluate.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/helpers.py
--rw-r--r--   0        0        0    10882 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/load_model.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/load_tokenizer.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/transformer_heads/util/model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/LICENSE
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 transformer_heads-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0    66320 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/_images/example_architecture.svg
+-rw-r--r--   0        0        0    64089 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/_images/multi_linear_probe.svg
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/getting_started.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/images.rst
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/modules.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/readme.rst
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/transformer_heads.model.rst
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/transformer_heads.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/transformer_heads.tests.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/docs/source/transformer_heads.util.rst
+-rw-r--r--   0        0        0    85722 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/joint_multitask_learning.ipynb
+-rw-r--r--   0        0        0    48378 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/linear_probe.ipynb
+-rw-r--r--   0        0        0    70663 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/multi_linear_probe.ipynb
+-rw-r--r--   0        0        0    15095 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/saving_and_loading.ipynb
+-rw-r--r--   0        0        0    74344 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/text_classification_full_finetune.ipynb
+-rw-r--r--   0        0        0    75081 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/text_classification_linear_probe.ipynb
+-rw-r--r--   0        0        0    79822 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/gpt2/text_classification_qlora.ipynb
+-rw-r--r--   0        0        0  2411412 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/llama/joint_multitask_learning.ipynb
+-rw-r--r--   0        0        0    59416 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/llama/linear_probe.ipynb
+-rw-r--r--   0        0        0    81976 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/notebooks/llama/multi_linear_probe.ipynb
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/other/pip_freeze.txt
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/scripts/paper_shredder.bash
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/scripts/remove_eval_spam.py
+-rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/scripts/run_slurm.sh
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/scripts/shredder_papers.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/__init__.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/config.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/constants.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/model/__init__.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/model/head.py
+-rw-r--r--   0        0        0    34144 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/model/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/tests/__init__.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/tests/test_generate.py
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/tests/test_load_model.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/tests/test_loss_compute.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/custom_loss.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/evaluate.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/helpers.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/load_model.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/load_tokenizer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/transformer_heads/util/model.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 transformer_heads-0.1.0/PKG-INFO
```

### Comparing `transformer_heads-0.0.9/.readthedocs.yaml` & `transformer_heads-0.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/.github/workflows/publish_to_pypi.yml` & `transformer_heads-0.1.0/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/_images/example_architecture.svg` & `transformer_heads-0.1.0/_images/example_architecture.svg`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/_images/multi_linear_probe.svg` & `transformer_heads-0.1.0/_images/multi_linear_probe.svg`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/Makefile` & `transformer_heads-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/make.bat` & `transformer_heads-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/conf.py` & `transformer_heads-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/getting_started.md` & `transformer_heads-0.1.0/docs/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/index.rst` & `transformer_heads-0.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/transformer_heads.model.rst` & `transformer_heads-0.1.0/docs/source/transformer_heads.model.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/transformer_heads.rst` & `transformer_heads-0.1.0/docs/source/transformer_heads.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/docs/source/transformer_heads.util.rst` & `transformer_heads-0.1.0/docs/source/transformer_heads.util.rst`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/joint_multitask_learning.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/joint_multitask_learning.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/linear_probe.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/multi_linear_probe.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/multi_linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/saving_and_loading.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/saving_and_loading.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/text_classification_full_finetune.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/text_classification_full_finetune.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/gpt2/text_classification_qlora.ipynb` & `transformer_heads-0.1.0/notebooks/gpt2/text_classification_qlora.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/notebooks/llama/linear_probe.ipynb` & `transformer_heads-0.1.0/notebooks/llama/linear_probe.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'cells'": "{17: {'source': ['The linear probe has vocab_size * hidden_size (32000*4096) "*

 * *            'parameters. So already quite a few, but nothing compared to 7 billion other '*

 * *            "parameters of the model.']}}"}*

```diff
@@ -526,15 +526,15 @@
                     "exception": false,
                     "start_time": "2024-03-24T04:29:38.658269",
                     "status": "completed"
                 },
                 "tags": []
             },
             "source": [
-                "Given that gpt2 is a fairly small model with a large vocab size, our single linear probe already has quite a lot of parameters compared to the rest of the model. Every parameter in the model that is not part of the linear probe is frozen (has requires_grad set to false)."
+                "The linear probe has vocab_size * hidden_size (32000*4096) parameters. So already quite a few, but nothing compared to 7 billion other parameters of the model."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "844c2225",
             "metadata": {
                 "papermill": {
```

### Comparing `transformer_heads-0.0.9/notebooks/llama/multi_linear_probe.ipynb` & `transformer_heads-0.1.0/notebooks/llama/multi_linear_probe.ipynb`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/scripts/paper_shredder.bash` & `transformer_heads-0.1.0/scripts/paper_shredder.bash`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/scripts/remove_eval_spam.py` & `transformer_heads-0.1.0/scripts/remove_eval_spam.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/scripts/shredder_papers.py` & `transformer_heads-0.1.0/scripts/shredder_papers.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/transformer_heads/config.py` & `transformer_heads-0.1.0/transformer_heads/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     pred_for_sequence: Optional[bool] = False
     is_regression: Optional[bool] = False
     output_bias: Optional[bool] = False
     loss_fct: Optional[str] = "cross_entropy"
     trainable: Optional[bool] = True
     loss_weight: Optional[float] = 1.0
     ignore_pads: Optional[bool] = None
+    block_gradients: Optional[bool] = False
 
     def __hash__(self):
         return hash(tuple(sorted(self.items())))
 
     # Make minimally serializable
     # Caveat: Won't work without indent specified in json.dumps
     def items(self):
```

### Comparing `transformer_heads-0.0.9/transformer_heads/constants.py` & `transformer_heads-0.1.0/transformer_heads/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 It includes `loss_fct_map`, a dictionary that maps loss function names to their corresponding PyTorch implementations, 
 and `model_type_map`, a dictionary that maps model type names to their corresponding transformers model classes.
 activation_map is a dictionary that maps activation function names to their corresponding PyTorch implementations.
 """
 
 import torch.nn as nn
 from transformers import GPT2Model, LlamaModel, MistralModel
+from transformer_heads.util.custom_loss import Masked_MSE_Loss
 
 activation_map = {"sigmoid": nn.Sigmoid, "linear": nn.Identity, "relu": nn.ReLU}
 loss_fct_map = {
     "mse": nn.MSELoss(),
+    "masked_mse": Masked_MSE_Loss(),
     "cross_entropy": nn.CrossEntropyLoss(),
     "bce": nn.BCELoss(),
     "bce_with_logits": nn.BCEWithLogitsLoss(),
 }
 
 # Map model type to base model class attribute name and base model class
 model_type_map = {
```

### Comparing `transformer_heads-0.0.9/transformer_heads/output.py` & `transformer_heads-0.1.0/transformer_heads/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,11 +29,24 @@
         past_key_values (Optional[Tuple[Tuple[torch.FloatTensor]]]): Tuple of key value states for transformer models.
         hidden_states (Optional[Tuple[torch.FloatTensor, ...]]): Tuple of hidden states for transformer models.
         attentions (Optional[Tuple[torch.FloatTensor, ...]]): Tuple of attention weights for transformer models.
     """
 
     loss: Optional[torch.FloatTensor] = None
     loss_by_head: Optional[dict[str, torch.FloatTensor]] = None
+    adapted_loss_by_head: Optional[dict[str, torch.FloatTensor]] = None
     preds_by_head: Optional[dict[str, torch.FloatTensor]] = None
     past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None
     hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
     attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+
+
+@dataclass
+class HeadedModelGenerateOutput(ModelOutput):
+    """
+    An generation output class for a model with multiple heads.
+    """
+
+    sequences: torch.LongTensor = None
+    logprobs: torch.FloatTensor = None
+    head_outputs: dict[str, torch.FloatTensor] = None
+    past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None
```

### Comparing `transformer_heads-0.0.9/transformer_heads/model/head.py` & `transformer_heads-0.1.0/transformer_heads/model/head.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,18 +36,20 @@
         in_size,
         hidden_size,
         num_layers,
         output_activation: str,
         num_outputs: int = 1,
         output_bias: bool = False,
         trainable: bool = True,
+        block_gradients: bool = False,
     ):
         super().__init__()
         self.name = name
         self.trainable = trainable
+        self.block_gradients = block_gradients
         self.lins = nn.ModuleList()
         if num_layers == 1:
             self.lins.append(nn.Linear(in_size, num_outputs, bias=output_bias))
         else:
             self.lins.append(nn.Linear(in_size, hidden_size, bias=True))
             for _ in range(num_layers - 2):
                 self.lins.append(nn.Linear(hidden_size, hidden_size, bias=True))
@@ -73,14 +75,15 @@
             head_config.in_size,
             head_config.hidden_size,
             head_config.num_layers,
             head_config.output_activation,
             head_config.num_outputs or 1,
             head_config.output_bias,
             head_config.trainable,
+            head_config.block_gradients,
         )
 
     def set_requires_grad(self, requires_grad):
         """
         Sets whether the parameters of the MLP head require gradients.
 
         Args:
@@ -118,13 +121,15 @@
 
         Args:
             x (torch.Tensor): The input tensor.
 
         Returns:
             torch.FloatTensor: The output tensor.
         """
+        if self.block_gradients:
+            x = x.detach()
         for i, lin in enumerate(self.lins):
             x = lin(x)
             if i < len(self.lins) - 1:
                 x = self.hidden_activation(x)
         x = self.output_activation(x)
         return x
```

### Comparing `transformer_heads-0.0.9/transformer_heads/tests/test_load_model.py` & `transformer_heads-0.1.0/transformer_heads/tests/test_load_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from transformer_heads.model.model import get_multi_head_transformer
 from transformer_heads.output import HeadedModelOutput
 from transformer_heads.util.load_model import (
     create_headed_qlora,
     load_headed,
     load_lora_with_heads,
 )
+from transformer_heads.util.helpers import get_model_params
 from transformer_heads.util.model import print_trainable_parameters
 
 heads = [
     HeadConfig(
         name="lm_head",
         layer_hook=-1,
         in_size=4096,
@@ -80,89 +81,93 @@
         probs1 = torch.softmax(logits1[0], dim=-1)
         probs2 = torch.softmax(logits2[0], dim=-1)
         print(torch.sum(probs1), torch.sum(probs2))
         print(torch.sum(torch.abs(probs1 - probs2)))
         assert probs1.allclose(probs2, atol=1e-4, rtol=1e-3)
 
 
-def get_test_inputs(device):
-    tk = AutoTokenizer.from_pretrained("mistralai/Mistral-7B-v0.1")
+def get_test_inputs(device, model_path="mistralai/Mistral-7B-v0.1"):
+    tk = AutoTokenizer.from_pretrained(model_path)
     inputs = tk("Paris is the capital of", return_tensors="pt")
     inputs["classes"] = torch.ones_like(inputs["input_ids"])
     inputs["seq"] = torch.tensor(1)
     inputs["regression_hook"] = torch.zeros_like(inputs["input_ids"])
     inputs["lm_head"] = torch.ones_like(inputs["input_ids"])
     inputs.to(device)
     return tk, inputs
 
 
-def test_load_model():
-    model = load_headed(
-        MistralForCausalLM, "mistralai/Mistral-7B-v0.1", heads, device_map="cpu"
-    )
-    print("Loaded headed Mistral model successfully!")
+def test_load_model(model_path="mistralai/Mistral-7B-v0.1"):
+    params = get_model_params(model_path)
+    heads[0].num_outputs = params["vocab_size"]
+    model = load_headed(params["model_class"], model_path, heads, device_map="cpu")
+    print("Loaded headed model successfully!")
 
-    tk, inputs = get_test_inputs(model.device)
+    tk, inputs = get_test_inputs(model.device, model_path=model_path)
     outputs: HeadedModelOutput = model(**inputs)
     print("loss_by_head", outputs["loss_by_head"])
     logits = outputs.preds_by_head["lm_head"]
     next_logits = logits[0, -1, :]
     pred_tk = tk.decode(next_logits.argmax().item())
     print("Model prediction:", pred_tk)
 
-    model.save_pretrained("mistral_headed")
-    print("Saved headed Mistral model successfully!")
+    model.save_pretrained("headed_model")
+    print("Saved headed model successfully!")
     del model
-    model = get_multi_head_transformer(MistralForCausalLM).from_pretrained(
-        "mistral_headed", device_map="cpu"
+    model = get_multi_head_transformer(params["model_class"]).from_pretrained(
+        "headed_model", device_map="cpu"
     )
-    print("Loaded saved headed Mistral model successfully!")
+    print("Loaded saved headed model successfully!")
     inputs.to(model.device)
     new_outputs: HeadedModelOutput = model(**inputs)
     new_logits = new_outputs.preds_by_head["lm_head"].to(logits.device)
     new_next_logits = logits[0, -1, :]
     pred_tk = tk.decode(new_next_logits.argmax().item())
     print("Model prediction:", pred_tk)
     check_consistency(outputs, new_outputs)
 
 
-def test_load_quantized():
+def test_load_quantized(model_path="mistralai/Mistral-7B-v0.1"):
+    params = get_model_params(model_path)
+    heads[0].num_outputs = params["vocab_size"]
     quantization_config = BitsAndBytesConfig(
         load_in_4bit=True,
         load_in_8bit=False,
         llm_int8_threshold=6.0,
         llm_int8_has_fp16_weight=False,
         bnb_4bit_compute_dtype=torch.float32,
         bnb_4bit_use_double_quant=True,
         bnb_4bit_quant_type="nf4",
     )
     model = load_headed(
-        MistralForCausalLM,
-        "mistralai/Mistral-7B-v0.1",
+        params["model_class"],
+        model_path,
         heads,
         device_map="cuda",
         quantization_config=quantization_config,
     )
-    tk, inputs = get_test_inputs(model.device)
+    tk, inputs = get_test_inputs(model.device, model_path=model_path)
     outputs1 = model(**inputs)
     print("loss_by_head", outputs1["loss_by_head"])
-    model.save_pretrained("mistral_heads")
+    model.save_pretrained("headed_model")
     del model
     model = load_headed(
-        MistralForCausalLM,
-        "mistralai/Mistral-7B-v0.1",
-        head_folder_path="mistral_heads",
+        params["model_class"],
+        model_path,
+        head_folder_path="headed_model",
         device_map="cuda",
         quantization_config=quantization_config,
     )
     outputs2 = model(**inputs)
     check_consistency(outputs1, outputs2)
 
 
-def test_qlora():
+def test_qlora(model_path="mistralai/Mistral-7B-v0.1"):
+    params = get_model_params(model_path)
+    heads[0].num_outputs = params["vocab_size"]
     quantization_config = BitsAndBytesConfig(
         load_in_4bit=True,
         load_in_8bit=False,
         llm_int8_threshold=6.0,
         llm_int8_has_fp16_weight=False,
         bnb_4bit_compute_dtype=torch.float32,
         bnb_4bit_use_double_quant=True,
@@ -173,41 +178,41 @@
         lora_alpha=16,
         target_modules=None,
         lora_dropout=0.0,
         bias="none",
         task_type="CAUSAL_LM",
     )
     model = create_headed_qlora(
-        MistralForCausalLM,
-        "mistralai/Mistral-7B-v0.1",
+        params["model_class"],
+        model_path,
         quantization_config=quantization_config,
         lora_config=lora_config,
         head_configs=heads,
         device_map="cuda",
     )
     print_trainable_parameters(model, use_4bit=quantization_config.load_in_4bit)
-    print("Loaded headed qlora Mistral model successfully!")
-    tk, inputs = get_test_inputs(model.device)
+    print("Loaded headed qlora model successfully!")
+    tk, inputs = get_test_inputs(model.device, model_path=model_path)
     print(inputs["input_ids"].dtype)
     outputs: HeadedModelOutput = model(**inputs)
     logits = outputs.preds_by_head["lm_head"]
     next_logits = logits[0, -1, :]
     pred_tk = tk.decode(next_logits.argmax().item())
     print("Model prediction:", pred_tk)
-    model.save_pretrained("mistral_headed_qlora")
-    print("Saved headed qlora Mistral model successfully!")
+    model.save_pretrained("headed_model_qlora")
+    print("Saved headed qlora model successfully!")
     del model
     model = load_lora_with_heads(
-        MistralForCausalLM,
-        "mistral_headed_qlora",
+        params["model_class"],
+        "headed_model_qlora",
         quantization_config,
         device_map="cuda",
     )
     print_trainable_parameters(model, use_4bit=quantization_config.load_in_4bit)
-    print("Loaded saved headed qlora Mistral model successfully!")
+    print("Loaded saved headed qlora model successfully!")
     print(inputs["input_ids"].dtype)
     new_outputs: HeadedModelOutput = model(**inputs)
     new_logits = new_outputs.preds_by_head["lm_head"]
     new_next_logits = new_logits[0, -1, :]
     pred_tk = tk.decode(new_next_logits.argmax().item())
     print("Model prediction:", pred_tk)
     check_consistency(outputs, new_outputs)
```

### Comparing `transformer_heads-0.0.9/transformer_heads/util/evaluate.py` & `transformer_heads-0.1.0/transformer_heads/util/evaluate.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/transformer_heads/util/helpers.py` & `transformer_heads-0.1.0/transformer_heads/util/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Functions:
     get_model_params(model_path: str): Get the parameters of a model based on its type.
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List
+from math import sqrt
 
 import torch
 from torch.nn.utils.rnn import pad_sequence
 from transformers import (
     GPT2LMHeadModel,
     LlamaForCausalLM,
     MistralForCausalLM,
@@ -30,15 +31,15 @@
     Attributes:
         feature_name_to_padding_value (dict[str, int]): A dictionary mapping feature names to their padding values.
 
     Methods:
         __call__(features: List[Dict[str, Any]]) -> Dict[str, Any]: Pad the sequences in the features to the same length.
     """
 
-    feature_name_to_padding_value: dict[str, int]
+    feature_name_to_padding_value: dict[str, int | float]
 
     def __call__(self, features: List[Dict[str, Any]]) -> Dict[str, Any]:
         """
         Pad the sequences in the features to the same length.
 
         Args:
             features (List[Dict[str, Any]]): A list of features, where each feature is a dictionary mapping feature names to sequences.
@@ -78,7 +79,25 @@
     cfg["model_class"] = getattr(
         __import__("transformers", fromlist=[cfg["architectures"][0]]),
         cfg["architectures"][0],
     )
     if model_path == "gpt2" and "hidden_size" not in cfg:
         cfg["hidden_size"] = 768
     return cfg
+
+
+class Welfords:
+    def __init__(self):
+        self.count: int = 0
+        self.mean: float = 0.0
+        self.M2: float = 0.0
+
+    def update(self, new_value):
+        self.count += 1
+        delta = new_value - self.mean
+        self.mean += delta / self.count
+        delta2 = new_value - self.mean
+        self.M2 += delta * delta2
+
+    @property
+    def std(self) -> float:
+        return sqrt(self.M2 / self.count) if self.count > 1 else 0.0
```

### Comparing `transformer_heads-0.0.9/transformer_heads/util/load_model.py` & `transformer_heads-0.1.0/transformer_heads/util/load_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,28 +46,30 @@
     model_name: str,
     head_configs=None,
     head_folder_path=None,
     only_inference: bool = False,
     device_map="auto",
     quantization_config: BitsAndBytesConfig = None,
     freeze_base_model: bool = True,
+    adaptive_loss: bool = False,
     **kwargs,
 ) -> HeadedModel:
     """
     Loads a transformer model with additional heads.
 
     Args:
         base_model_class (Type[PreTrainedModel]): The class of the base transformer model.
         model_name (str): The huggingface name of the model to load.
         head_configs (list, optional): A list of head configurations.
         head_folder_path (str, optional): The path to the folder containing the saved heads and head configurations.
         only_inference (bool, optional): Whether to load the model for inference only.
         device_map (str, optional): The device map to use when loading the model.
         quantization_config (BitsAndBytesConfig, optional): The quantization configuration to use when loading the model.
         freeze_base_model (bool, optional): Whether to freeze the base model during training.
+        adaptive_loss (bool, optional): Whether to use adaptive loss scaling.
         **kwargs: Additional keyword arguments to pass to from_pretrained.
     """
     assert head_configs is not None or head_folder_path is not None
     assert head_configs is None or head_folder_path is None
     assert (
         quantization_config is None or only_inference or freeze_base_model
     ), "You can only use quantization in inference mode or if you freeze the base model. Use qlora to modify the base model with quantization."
@@ -91,14 +93,15 @@
     model = model.from_pretrained(
         model_name,
         config=config,
         device_map=device_map,
         quantization_config=quantization_config,
         **kwargs,
     )
+    model.set_adaptive_loss(adaptive_loss)
     if freeze_base_model and quantization_config is None:
         for _name, param in model.named_parameters():
             param.requires_grad = False
     if quantization_config is not None and bits < 16:
         if not only_inference:
             model = prepare_model_for_kbit_training(model)
             model._hf_peft_config_loaded = (
@@ -109,14 +112,20 @@
     for head in model.heads.values():
         if head_folder_path is not None:
             head.load_from_safetensors(head_folder_path)
         if not only_inference:
             if head.trainable:
                 head.set_requires_grad(True)
             head.requires_individual_saving = True
+    if (
+        not only_inference
+        and model.lm_head is not None
+        and model.lm_head_config.trainable
+    ):
+        model.lm_head.requires_grad_(True)
     return model
 
 
 def load_lora_with_heads(
     base_model_class: Type[PreTrainedModel],
     path: str,
     quantization_config: BitsAndBytesConfig = None,
@@ -189,27 +198,35 @@
                 param.requires_grad = True
     head: MLPHead
     for head in model.heads.values():
         head.load_from_safetensors(path)
         if not only_inference and fully_trained_heads:
             head.set_requires_grad(True)
             head.requires_individual_saving = True
+
+    if (
+        not only_inference
+        and model.lm_head is not None
+        and model.lm_head_config.trainable
+    ):
+        model.lm_head.requires_grad_(True)
     patch_save_pretrained(model)
     return model
 
 
 def create_headed_qlora(
     base_model_class: Type[PreTrainedModel],
     model_name: str,
     quantization_config: BitsAndBytesConfig,
     lora_config: LoraConfig,
     head_configs: list[HeadConfig],
     fully_trained_heads: bool = True,
     device_map="auto",
     gradient_checkpointing: bool = False,
+    adaptive_loss: bool = False,
     **kwargs,
 ) -> HeadedModel:
     """
     Creates a quantized LoRA (Low Rank Adaptation) transformer model with additional heads.
 
     Args:
         base_model_class (Type[PreTrainedModel]): The class of the base transformer model.
@@ -239,25 +256,29 @@
     model: HeadedModel = model.from_pretrained(
         model_name,
         config=config,
         device_map=device_map,
         quantization_config=quantization_config,
         **kwargs,
     )
+    model.set_adaptive_loss(adaptive_loss)
 
     if lora_config.target_modules is None:
         lora_config.target_modules = find_all_linear_names(bits, model, noadd=["heads"])
 
     model = prepare_model_for_kbit_training(
         model, use_gradient_checkpointing=gradient_checkpointing
     )
 
     model = get_peft_model(model, lora_config)
 
     if fully_trained_heads:
         head: MLPHead
         for head in model.heads.values():
-            head.set_requires_grad(True)
-            head.requires_individual_saving = True
+            if head.trainable:
+                head.set_requires_grad(True)
+                head.requires_individual_saving = True
+        if model.lm_head is not None and model.lm_head_config.trainable:
+            model.lm_head.requires_grad_(True)
 
     patch_save_pretrained(model)
     return model
```

### Comparing `transformer_heads-0.0.9/transformer_heads/util/load_tokenizer.py` & `transformer_heads-0.1.0/transformer_heads/util/load_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/transformer_heads/util/model.py` & `transformer_heads-0.1.0/transformer_heads/util/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             names = name.split(".")
             for n in names:
                 if n in noadd:
                     break
             else:
                 lora_module_names.add(names[-1])
 
-    if "lm_head" in lora_module_names:  # needed for 16-bit
-        lora_module_names.remove("lm_head")
+    # if "lm_head" in lora_module_names:  # needed for 16-bit
+    #    lora_module_names.remove("lm_head")
     return list(lora_module_names)
 
 
 def print_trainable_parameters(model, use_4bit=False):
     """
     Print some information about the trainable parameters off a model.
```

### Comparing `transformer_heads-0.0.9/LICENSE` & `transformer_heads-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/README.md` & `transformer_heads-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/pyproject.toml` & `transformer_heads-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transformer_heads-0.0.9/PKG-INFO` & `transformer_heads-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: transformer_heads
-Version: 0.0.9
+Version: 0.1.0
 Summary: Attach custom heads to transformer models.
 Author-email: Yannik Keller <yannik@kelnet.de>
 License: MIT License
 License-File: LICENSE
 Keywords: Linear Probe,Qlora,Transformer
 Requires-Python: >=3.10
 Requires-Dist: bitsandbytes
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: transformer_heads Version: 0.0.9 Summary: Attach
+Metadata-Version: 2.3 Name: transformer_heads Version: 0.1.0 Summary: Attach
 custom heads to transformer models. Author-email: Yannik Keller
 kelnet.de> License: MIT License License-File: LICENSE Keywords: Linear
 Probe,Qlora,Transformer Requires-Python: >=3.10 Requires-Dist: bitsandbytes
 Requires-Dist: datasets Requires-Dist: fire Requires-Dist: pandas Requires-
 Dist: peft Requires-Dist: torch Requires-Dist: tqdm Requires-Dist: transformers
 Description-Content-Type: text/markdown
      ****** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd || _RR_ee_dd_dd_ii_tt_ _PP_oo_ss_tt_ _ww_ii_tt_hh_ _mm_oo_rr_ee_ _ii_nn_ff_oo ******
```

