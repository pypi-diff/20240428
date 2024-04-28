# Comparing `tmp/fuxictr-2.2.3.tar.gz` & `tmp/fuxictr-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.2.3.tar", last modified: Fri Apr 19 13:06:21 2024, max compression
+gzip compressed data, was "dist/fuxictr-2.3.0.tar", last modified: Sun Apr 28 01:53:43 2024, max compression
```

## Comparing `fuxictr-2.2.3.tar` & `fuxictr-2.3.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-19 13:06:21.000000 fuxictr-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-19 13:06:19.000000 fuxictr-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/autotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/avazu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/kkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18058 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/feature_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/rank_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/multitask_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/model_zoo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/model_zoo/multitask/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 13:06:19.000000 fuxictr-2.2.3/model_zoo/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:06:21.000000 fuxictr-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-19 13:06:19.000000 fuxictr-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    29890 2024-04-28 01:53:43.000000 fuxictr-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-28 01:53:38.000000 fuxictr-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/autotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/datasets/avazu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/datasets/kkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/preprocess/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18767 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/preprocess/feature_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/preprocess/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/preprocess/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/npz_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/parquet_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/parquet_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/dataloaders/rank_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/models/multitask_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/pytorch/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/tensorflow/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 01:53:38.000000 fuxictr-2.3.0/fuxictr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29890 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 01:53:43.000000 fuxictr-2.3.0/fuxictr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/model_zoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:53:43.000000 fuxictr-2.3.0/model_zoo/multitask/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 01:53:38.000000 fuxictr-2.3.0/model_zoo/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 01:53:43.000000 fuxictr-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-28 01:53:38.000000 fuxictr-2.3.0/setup.py
```

### Comparing `fuxictr-2.2.3/PKG-INFO` & `fuxictr-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.3
+Version: 2.3.0
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
         <img src="https://cdn.jsdelivr.net/gh/reczoo/FuxiCTR@main/docs/img/logo.png" alt="Logo" width="260"/>
         </div>
         
         <div align="center">
-        <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
+        <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.9+-blue" style="max-width: 100%;" alt="Python version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
         <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
         <a href="https://github.com/reczoo/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/reczoo/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
         </div>
         <hr/>
@@ -107,15 +107,15 @@
         + :star: [Benchmark settings and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr)
         + :star: [Benchmark leaderboard for CTR prediction](https://openbenchmark.github.io/BARS/CTR/leaderboard)
         
         ## Dependencies
         
         FuxiCTR has the following dependencies:
         
-        + python 3.6+
+        + python 3.9+
         + pytorch 1.10+ (required only for Torch models)
         + tensorflow 2.1+ (required only for TF models)
         
         Please install other required packages via `pip install -r requirements.txt`.
         
         ## Quick Start
         
@@ -177,15 +177,14 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.3 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.3.0 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
@@ -220,15 +220,15 @@
 abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | ##
 Benchmarking We have benchmarked FuxiCTR models on a set of open datasets as
 follows: + :star: [Benchmark datasets for CTR prediction](https://github.com/
 reczoo/Datasets?tab=readme-ov-file#ctr-prediction) + :star: [Benchmark settings
 and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr) + :
 star: [Benchmark leaderboard for CTR prediction](https://
 openbenchmark.github.io/BARS/CTR/leaderboard) ## Dependencies FuxiCTR has the
-following dependencies: + python 3.6+ + pytorch 1.10+ (required only for Torch
+following dependencies: + python 3.9+ + pytorch 1.10+ (required only for Torch
 models) + tensorflow 2.1+ (required only for TF models) Please install other
 required packages via `pip install -r requirements.txt`. ## Quick Start 1. Run
 the demo examples Examples are provided in the demo directory to show some
 basic usage of FuxiCTR. Users can run the examples for quick start and to
 understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
 python example2_DeepFM_with_h5_input.py ``` 2. Run a model on tiny data Users
 can easily run each model in the model zoo following the commands below, which
@@ -269,13 +269,12 @@
 and practice in recommender systems, please reach out via our WeChat group. !
 [Scan QR code](https://openbenchmark.github.io/BARS/_images/wechat.jpg)
 Keywords: ctr prediction,recommender systems,ctr,cvr,pytorch Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.6 Description-Content-Type:
-text/markdown
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
+Content-Type: text/markdown
```

### Comparing `fuxictr-2.2.3/README.md` & `fuxictr-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
 <img src="https://cdn.jsdelivr.net/gh/reczoo/FuxiCTR@main/docs/img/logo.png" alt="Logo" width="260"/>
 </div>
 
 <div align="center">
-<a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
+<a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.9+-blue" style="max-width: 100%;" alt="Python version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
 <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
 <a href="https://github.com/reczoo/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/reczoo/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
 </div>
 <hr/>
@@ -98,15 +98,15 @@
 + :star: [Benchmark settings and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr)
 + :star: [Benchmark leaderboard for CTR prediction](https://openbenchmark.github.io/BARS/CTR/leaderboard)
 
 ## Dependencies
 
 FuxiCTR has the following dependencies:
 
-+ python 3.6+
++ python 3.9+
 + pytorch 1.10+ (required only for Torch models)
 + tensorflow 2.1+ (required only for TF models)
 
 Please install other required packages via `pip install -r requirements.txt`.
 
 ## Quick Start
```

#### html2text {}

```diff
@@ -215,15 +215,15 @@
 abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | ##
 Benchmarking We have benchmarked FuxiCTR models on a set of open datasets as
 follows: + :star: [Benchmark datasets for CTR prediction](https://github.com/
 reczoo/Datasets?tab=readme-ov-file#ctr-prediction) + :star: [Benchmark settings
 and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr) + :
 star: [Benchmark leaderboard for CTR prediction](https://
 openbenchmark.github.io/BARS/CTR/leaderboard) ## Dependencies FuxiCTR has the
-following dependencies: + python 3.6+ + pytorch 1.10+ (required only for Torch
+following dependencies: + python 3.9+ + pytorch 1.10+ (required only for Torch
 models) + tensorflow 2.1+ (required only for TF models) Please install other
 required packages via `pip install -r requirements.txt`. ## Quick Start 1. Run
 the demo examples Examples are provided in the demo directory to show some
 basic usage of FuxiCTR. Users can run the examples for quick start and to
 understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
 python example2_DeepFM_with_h5_input.py ``` 2. Run a model on tiny data Users
 can easily run each model in the model zoo following the commands below, which
```

### Comparing `fuxictr-2.2.3/fuxictr/autotuner.py` & `fuxictr-2.3.0/fuxictr/autotuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,17 @@
 
     # enumerate dataset para combinations
     dataset_dict = {k: tune_dict[k] if k in tune_dict else [v] for k, v in dataset_dict.items()}
     dataset_para_keys = list(dataset_dict.keys())
     dataset_para_combs = dict()
     for idx, values in enumerate(itertools.product(*map(dataset_dict.get, dataset_para_keys))):
         dataset_params = dict(zip(dataset_para_keys, values))
-        if dataset_params["data_format"] == "npz":
+        if (dataset_params["data_format"] == "npz" or
+           (dataset_params["data_format"] == "parquet" and 
+            dataset_params["rebuild_dataset"] == False)):
             dataset_para_combs[dataset_id] = dataset_params
         else:
             hash_id = hashlib.md5("".join(sorted(print_to_json(dataset_params))).encode("utf-8")).hexdigest()[0:8]
             dataset_para_combs[dataset_id + "_{}".format(hash_id)] = dataset_params
 
     # dump dataset para combinations to config file
     dataset_config = os.path.join(config_dir, "dataset_config.yaml")
```

### Comparing `fuxictr-2.2.3/fuxictr/datasets/avazu.py` & `fuxictr-2.3.0/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/datasets/criteo.py` & `fuxictr-2.3.0/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/datasets/kkbox.py` & `fuxictr-2.3.0/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/features.py` & `fuxictr-2.3.0/fuxictr/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
     def load(self, json_file, params):
         logging.info("Load feature_map from json: " + json_file)
         with io.open(json_file, "r", encoding="utf-8") as fd:
             feature_map = json.load(fd) #, object_pairs_hook=OrderedDict
         if feature_map["dataset_id"] != self.dataset_id:
             raise RuntimeError("dataset_id={} does not match feature_map!".format(self.dataset_id))
-        self.num_fields = feature_map["num_fields"]
         self.labels = feature_map.get("labels", [])
         self.total_features = feature_map.get("total_features", 0)
         self.input_length = feature_map.get("input_length", 0)
         self.group_id = feature_map.get("group_id", None)
         self.default_emb_dim = params.get("embedding_dim", None)
         self.features = OrderedDict((k, v) for x in feature_map["features"] for k, v in x.items())
+        self.num_fields = self.get_num_fields()
         if params.get("use_features", None):
             self.features = OrderedDict((x, self.features[x]) for x in params["use_features"])
         if params.get("feature_specs", None):
             self.update_feature_specs(params["feature_specs"])
         self.set_column_index()
 
     def update_feature_specs(self, feature_specs):
```

### Comparing `fuxictr-2.2.3/fuxictr/metrics.py` & `fuxictr-2.3.0/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.3.0/fuxictr/preprocess/build_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,90 +44,95 @@
         valid_ddf = train_ddf.loc[instance_IDs[train_size:], :].reset_index()
         instance_IDs = instance_IDs[0:train_size]
     if valid_size > 0 or test_size > 0:
         train_ddf = train_ddf.loc[instance_IDs, :].reset_index()
     return train_ddf, valid_ddf, test_ddf
 
 
-def save_npz(darray_dict, data_path):
-    logging.info("Saving data to npz: " + data_path)
-    os.makedirs(os.path.dirname(data_path), exist_ok=True)
-    np.savez(data_path, **darray_dict)
-
-
 def transform_block(feature_encoder, df_block, filename):
-    darray_dict = feature_encoder.transform(df_block)
-    save_npz(darray_dict, os.path.join(feature_encoder.data_dir, filename))
+    df_block = feature_encoder.transform(df_block)
+    data_path = os.path.join(feature_encoder.data_dir, filename)
+    logging.info("Saving data to parquet: " + data_path)
+    os.makedirs(os.path.dirname(data_path), exist_ok=True)
+    df_block.to_parquet(data_path, index=False, engine="pyarrow")
 
 
 def transform(feature_encoder, ddf, filename, block_size=0):
     ddf = ddf.collect().to_pandas()
     if block_size > 0:
         pool = mp.Pool(mp.cpu_count() // 2)
         block_id = 0
         for idx in range(0, len(ddf), block_size):
             df_block = ddf.iloc[idx:(idx + block_size)]
             pool.apply_async(
                 transform_block,
-                args=(feature_encoder,
-                      df_block,
-                      '{}/part_{:05d}.npz'.format(filename, block_id))
+                args=(feature_encoder, df_block,
+                      '{}/part_{:05d}.parquet'.format(filename, block_id))
             )
             block_id += 1
         pool.close()
         pool.join()
     else:
         transform_block(feature_encoder, ddf, filename)
 
 
-def build_dataset(feature_encoder, train_data=None, valid_data=None, test_data=None, valid_size=0, 
-                  test_size=0, split_type="sequential", data_block_size=0, **kwargs):
+def build_dataset(feature_encoder, train_data=None, valid_data=None, test_data=None,
+                  valid_size=0, test_size=0, split_type="sequential", data_block_size=0,
+                  rebuild_dataset=True, **kwargs):
     """ Build feature_map and transform data """
+    if rebuild_dataset:
+        feature_map_path = os.path.join(feature_encoder.data_dir, "feature_map.json")
+        if os.path.exists(feature_map_path):
+            logging.warn(f"Skip rebuilding {feature_map_path}. " 
+                + "Please delete it manually if rebuilding is required.")
 
-    feature_map_json = os.path.join(feature_encoder.data_dir, "feature_map.json")
-    if os.path.exists(feature_map_json):
-        logging.warn("Skip rebuilding {}. Please delete it manually if rebuilding is required." \
-                     .format(feature_map_json))
-    else:
-        # Load csv data
-        train_ddf = feature_encoder.read_csv(train_data, **kwargs)
+        # Load data files
+        train_ddf = feature_encoder.read_data(train_data, **kwargs)
         valid_ddf = None
         test_ddf = None
 
         # Split data for train/validation/test
         if valid_size > 0 or test_size > 0:
-            valid_ddf = feature_encoder.read_csv(valid_data, **kwargs)
-            test_ddf = feature_encoder.read_csv(test_data, **kwargs)
+            valid_ddf = feature_encoder.read_data(valid_data, **kwargs)
+            test_ddf = feature_encoder.read_data(test_data, **kwargs)
+            # TODO: check split_train_test in lazy mode
             train_ddf, valid_ddf, test_ddf = split_train_test(train_ddf, valid_ddf, test_ddf, 
                                                               valid_size, test_size, split_type)
         
         # fit and transform train_ddf
         train_ddf = feature_encoder.preprocess(train_ddf)
-        feature_encoder.fit(train_ddf, **kwargs)
+        feature_encoder.fit(train_ddf, rebuild_dataset=True, **kwargs)
         transform(feature_encoder, train_ddf, 'train', block_size=data_block_size)
         del train_ddf
         gc.collect()
 
         # Transfrom valid_ddf
         if valid_ddf is None and (valid_data is not None):
-            valid_ddf = feature_encoder.read_csv(valid_data, **kwargs)
+            valid_ddf = feature_encoder.read_data(valid_data, **kwargs)
         if valid_ddf is not None:
             valid_ddf = feature_encoder.preprocess(valid_ddf)
             transform(feature_encoder, valid_ddf, 'valid', block_size=data_block_size)
             del valid_ddf
             gc.collect()
 
         # Transfrom test_ddf
         if test_ddf is None and (test_data is not None):
-            test_ddf = feature_encoder.read_csv(test_data, **kwargs)
+            test_ddf = feature_encoder.read_data(test_data, **kwargs)
         if test_ddf is not None:
             test_ddf = feature_encoder.preprocess(test_ddf)
             transform(feature_encoder, test_ddf, 'test', block_size=data_block_size)
             del test_ddf
             gc.collect()
         logging.info("Transform csv data to npz done.")
+
+        train_data, valid_data, test_data = (
+            os.path.join(feature_encoder.data_dir, "train"), \
+            os.path.join(feature_encoder.data_dir, "valid"), \
+            os.path.join(feature_encoder.data_dir, "test") if (
+                test_data or test_size > 0) else None
+        )
+    
+    else: # skip rebuilding data but only compute feature_map.json
+        feature_encoder.fit(train_ddf=None, rebuild_dataset=False, **kwargs)
     
     # Return processed data splits
-    return os.path.join(feature_encoder.data_dir, "train"), \
-           os.path.join(feature_encoder.data_dir, "valid"), \
-           os.path.join(feature_encoder.data_dir, "test") if (
-           test_data or test_size > 0) else None
+    return train_data, valid_data, test_data
```

### Comparing `fuxictr-2.2.3/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.3.0/fuxictr/preprocess/feature_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,22 +63,26 @@
                     _col = col.copy()
                     _col["name"] = _name
                     full_feature_cols.append(_col)
             else:
                 full_feature_cols.append(col)
         return full_feature_cols
 
-    def read_csv(self, data_path, sep=",", n_rows=None, **kwargs):
-        logging.info("Reading file: " + data_path)
+    def read_data(self, data_path, data_format="csv", sep=",", n_rows=None, **kwargs):
+        if not data_path.endswith(data_format):
+            data_path = os.path.join(data_path, "*.{data_format}")
+        logging.info("Reading files: " + data_path)
         file_names = sorted(glob.glob(data_path))
         assert len(file_names) > 0, f"Invalid data path: {data_path}"
-        # Require python >= 3.8 for use polars to scan multiple csv files
-        file_names = file_names[0]
-        ddf = pl.scan_csv(source=file_names, separator=sep, dtypes=self.dtype_dict,
-                          low_memory=False, n_rows=n_rows)
+        dfs = [
+            pl.scan_csv(source=file_name, separator=sep, dtypes=self.dtype_dict,
+                        low_memory=False, n_rows=n_rows)
+            for file_name in file_names
+        ]
+        ddf = pl.concat(dfs)
         return ddf
 
     def preprocess(self, ddf):
         logging.info("Preprocess feature columns...")
         all_cols = self.label_cols + self.feature_cols[::-1]
         for col in all_cols:
             name = col["name"]
@@ -91,22 +95,26 @@
                 preprocess_fn = getattr(self, preprocess_args[0])
                 ddf = preprocess_fn(ddf, name, *preprocess_args[1:-1])
                 ddf = ddf.with_columns(pl.col(name).cast(self.dtype_dict[name]))
         active_cols = [col["name"] for col in all_cols if col.get("active") != False]
         ddf = ddf.select(active_cols)
         return ddf
 
-    def fit(self, train_ddf, min_categr_count=1, num_buckets=10, **kwargs):    
+    def fit(self, train_ddf, min_categr_count=1, num_buckets=10, rebuild_dataset=True, **kwargs):    
         logging.info("Fit feature processor...")
+        self.rebuild_dataset = rebuild_dataset
         for col in self.feature_cols:
             name = col["name"]
             if col["active"]:
                 logging.info("Processing column: {}".format(col))
-                col_series = train_ddf.select(name).collect().to_series().to_pandas()
-                if col["type"] == "meta": # e.g. group_id
+                col_series = (
+                    train_ddf.select(name).collect().to_series().to_pandas() if self.rebuild_dataset
+                    else None
+                )
+                if col["type"] == "meta": # e.g. set group_id in gAUC
                     self.fit_meta_col(col)
                 elif col["type"] == "numeric":
                     self.fit_numeric_col(col, col_series)
                 elif col["type"] == "categorical":
                     self.fit_categorical_col(col, col_series,
                                              min_categr_count=min_categr_count,
                                              num_buckets=num_buckets)
@@ -150,17 +158,17 @@
                 else:
                     self.feature_map.total_features += self.feature_map.features[name]["vocab_size"]
                 if "pretrained_emb" not in spec: # "oov_idx" not used without pretrained_emb
                     del self.feature_map.features[name]["oov_idx"]
 
         self.feature_map.num_fields = self.feature_map.get_num_fields()
         self.feature_map.set_column_index()
+        self.feature_map.save(self.json_file)
         self.save_pickle(self.pickle_file)
         self.save_vocab(self.vocab_file)
-        self.feature_map.save(self.json_file)
         logging.info("Set feature processor done.")
 
     def fit_meta_col(self, col):
         name = col["name"]
         feature_type = col["type"]
         self.feature_map.features[name] = {"type": feature_type}
         if col.get("remap", True):
@@ -174,15 +182,16 @@
         feature_source = col.get("source", "")
         self.feature_map.features[name] = {"source": feature_source,
                                                 "type": feature_type}
         if "feature_encoder" in col:
             self.feature_map.features[name]["feature_encoder"] = col["feature_encoder"]
         if "normalizer" in col:
             normalizer = Normalizer(col["normalizer"])
-            normalizer.fit(col_series.dropna().values)
+            if self.rebuild_dataset:
+                normalizer.fit(col_series.dropna().values)
             self.processor_dict[name + "::normalizer"] = normalizer
 
     def fit_categorical_col(self, col, col_series, min_categr_count=1, num_buckets=10):
         name = col["name"]
         feature_type = col["type"]
         feature_source = col.get("source", "")
         min_categr_count = col.get("min_categr_count", min_categr_count)
@@ -192,17 +201,23 @@
             self.feature_map.features[name]["feature_encoder"] = col["feature_encoder"]
         if "embedding_dim" in col:
             self.feature_map.features[name]["embedding_dim"] = col["embedding_dim"]
         if "emb_output_dim" in col:
             self.feature_map.features[name]["emb_output_dim"] = col["emb_output_dim"]
         if "category_processor" not in col:
             tokenizer = Tokenizer(min_freq=min_categr_count, 
-                                  na_value=col.get("fill_na", ""), 
+                                  na_value=col.get("fill_na", ""),
                                   remap=col.get("remap", True))
-            tokenizer.fit_on_texts(col_series)
+            if self.rebuild_dataset:
+                tokenizer.fit_on_texts(col_series)
+            else:
+                if "vocab_size" in col:
+                    tokenizer.update_vocab(range(col["vocab_size"] - 1))
+                else:
+                    raise ValueError(f"{name}: vocab_size is required when rebuild_dataset=False")
             if "share_embedding" in col:
                 self.feature_map.features[name]["share_embedding"] = col["share_embedding"]
                 tknzr_name = col["share_embedding"] + "::tokenizer"
                 # update vocab of both tokenizers
                 self.processor_dict[tknzr_name] = tokenizer.merge_vocab(self.processor_dict[tknzr_name])
                 self.feature_map.features[col["share_embedding"]] \
                                 .update({"oov_idx": self.processor_dict[tknzr_name].vocab["__OOV__"],
@@ -213,18 +228,19 @@
                                                     "vocab_size": tokenizer.vocab_size()})
         else:
             category_processor = col["category_processor"]
             self.feature_map.features[name]["category_processor"] = category_processor
             if category_processor == "quantile_bucket": # transform numeric value to bucket
                 num_buckets = col.get("num_buckets", num_buckets)
                 qtf = sklearn_preprocess.QuantileTransformer(n_quantiles=num_buckets + 1)
-                qtf.fit(col_series.values)
-                boundaries = qtf.quantiles_[1:-1]
+                if self.rebuild_dataset:
+                    qtf.fit(col_series.values)
+                    boundaries = qtf.quantiles_[1:-1]
+                    self.processor_dict[name + "::boundaries"] = boundaries
                 self.feature_map.features[name]["vocab_size"] = num_buckets
-                self.processor_dict[name + "::boundaries"] = boundaries
             elif category_processor == "hash_bucket":
                 num_buckets = col.get("num_buckets", num_buckets)
                 self.feature_map.features[name]["vocab_size"] = num_buckets
                 self.processor_dict[name + "::num_buckets"] = num_buckets
             else:
                 raise NotImplementedError("category_processor={} not supported.".format(category_processor))
 
@@ -245,15 +261,21 @@
         splitter = col.get("splitter")
         na_value = col.get("fill_na", "")
         max_len = col.get("max_len", 0)
         padding = col.get("padding", "post") # "post" or "pre"
         tokenizer = Tokenizer(min_freq=min_categr_count, splitter=splitter, 
                               na_value=na_value, max_len=max_len, padding=padding,
                               remap=col.get("remap", True))
-        tokenizer.fit_on_texts(col_series)
+        if self.rebuild_dataset:
+            tokenizer.fit_on_texts(col_series)
+        else:
+            if "vocab_size" in col:
+                tokenizer.update_vocab(range(col["vocab_size"] - 1))
+            else:
+                raise ValueError(f"{name}: vocab_size is required when rebuild_dataset=False")
         if "share_embedding" in col:
             self.feature_map.features[name]["share_embedding"] = col["share_embedding"]
             tknzr_name = col["share_embedding"] + "::tokenizer"
             # update vocab of both tokenizers
             self.processor_dict[tknzr_name] = tokenizer.merge_vocab(self.processor_dict[tknzr_name])
             self.feature_map.features[col["share_embedding"]] \
                             .update({"oov_idx": self.processor_dict[tknzr_name].vocab["__OOV__"],
@@ -261,48 +283,44 @@
         self.processor_dict[name + "::tokenizer"] = tokenizer
         self.feature_map.features[name].update({"padding_idx": 0,
                                                 "oov_idx": tokenizer.vocab["__OOV__"],
                                                 "max_len": tokenizer.max_len,
                                                 "vocab_size": tokenizer.vocab_size()})
 
     def transform(self, ddf):
-        logging.info("Transform feature columns with ID mapping...")
-        data_dict = dict()
+        logging.info("Transform feature columns to IDs...")
         for feature, feature_spec in self.feature_map.features.items():
             if feature in ddf.columns:
                 feature_type = feature_spec["type"]
                 col_series = ddf[feature]
                 if feature_type == "meta":
                     if feature + "::tokenizer" in self.processor_dict:
                         tokenizer = self.processor_dict[feature + "::tokenizer"]
-                        data_dict[feature] = tokenizer.encode_meta(col_series)
+                        ddf[feature] = tokenizer.encode_meta(col_series)
                         # Update vocab in tokenizer
                         self.processor_dict[feature + "::tokenizer"] = tokenizer
-                    else:
-                        data_dict[feature] = col_series.values
                 elif feature_type == "numeric":
-                    col_values = col_series.values
                     normalizer = self.processor_dict.get(feature + "::normalizer")
                     if normalizer:
-                         col_values = normalizer.transform(col_values)
-                    data_dict[feature] = col_values
+                        ddf[feature] = normalizer.transform(col_series.values)
                 elif feature_type == "categorical":
                     category_processor = feature_spec.get("category_processor")
                     if category_processor is None:
-                        data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_category(col_series)
+                        ddf[feature] = (
+                            self.processor_dict.get(feature + "::tokenizer")
+                            .encode_category(col_series)
+                        )
                     elif category_processor == "numeric_bucket":
                         raise NotImplementedError
                     elif category_processor == "hash_bucket":
                         raise NotImplementedError
                 elif feature_type == "sequence":
-                    data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_sequence(col_series)
-        for label in self.feature_map.labels:
-            if label in ddf.columns:
-                data_dict[label] = ddf[label].values
-        return data_dict
+                    ddf[feature] = (self.processor_dict.get(feature + "::tokenizer")
+                                    .encode_sequence(col_series))
+        return ddf
 
     def load_pickle(self, pickle_file=None):
         """ Load feature processor from cache """
         if pickle_file is None:
             pickle_file = self.pickle_file
         logging.info("Load feature_processor from pickle: " + pickle_file)
         if os.path.exists(pickle_file):
```

### Comparing `fuxictr-2.2.3/fuxictr/preprocess/normalizer.py` & `fuxictr-2.3.0/fuxictr/preprocess/normalizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/preprocess/tokenizer.py` & `fuxictr-2.3.0/fuxictr/preprocess/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import numpy as np
 import h5py
 from tqdm import tqdm
 import polars as pl
 from keras_preprocessing.sequence import pad_sequences
 from concurrent.futures import ProcessPoolExecutor, as_completed
 import multiprocessing as mp
+from ..utils import load_pretrain_emb
 
 
 class Tokenizer(object):
     def __init__(self, max_features=None, na_value="", min_freq=1, splitter=None, remap=True,
                  lower=False, max_len=0, padding="pre"):
         self._max_features = max_features
         self._na_value = na_value
@@ -92,15 +93,15 @@
     def vocab_size(self):
         return max(self.vocab.values()) + 1 # In case that keys start from 1
 
     def update_vocab(self, word_list):
         new_words = 0
         for word in word_list:
             if word not in self.vocab:
-                self.vocab[word] = self.vocab["__OOV__"] + new_words
+                self.vocab[word] = self.vocab.get("__OOV__", 0) + new_words
                 new_words += 1
         if new_words > 0:
             self.vocab["__OOV__"] = self.vocab_size()
 
     def encode_meta(self, series):
         word_counts = dict(series.value_counts())
         if len(self.vocab) == 0:
@@ -118,24 +119,20 @@
         series = series.map(
             lambda text: [self.vocab.get(x, self.vocab["__OOV__"]) if x != self._na_value \
             else self.vocab["__PAD__"] for x in text.split(self._splitter)]
         )
         seqs = pad_sequences(series.to_list(), maxlen=self.max_len,
                              value=self.vocab["__PAD__"],
                              padding=self.padding, truncating=self.padding)
-        return np.array(seqs)
+        return seqs.tolist()
     
     def load_pretrained_vocab(self, feature_dtype, pretrain_path, expand_vocab=True):
-        if pretrain_path.endswith(".h5"):
-            with h5py.File(pretrain_path, 'r') as hf:
-                keys = hf["key"][:]
-                # in case mismatch of dtype between int and str
-                keys = keys.astype(feature_dtype)
-        elif pretrain_path.endswith(".npz"):
-            keys = np.load(pretrain_path)["key"]
+        keys = load_pretrain_emb(pretrain_path, keys=["key"])
+        # in case mismatch of dtype between int and str
+        keys = keys.astype(feature_dtype)
         # Update vocab with pretrained keys in case new tokens appear in validation or test set
         # Do NOT update OOV index here since it is used in PretrainedEmbedding
         if expand_vocab:
             vocab_size = self.vocab_size()
             for word in keys:
                 if word not in self.vocab:
                     self.vocab[word] = vocab_size
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_block_dataloader.py` & `fuxictr-2.3.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,78 +14,87 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
 import numpy as np
 from itertools import chain
-import torch
-from torch.utils import data
+from torch.utils.data.dataloader import default_collate
+from torch.utils.data import IterDataPipe, DataLoader, get_worker_info
 import glob
+import os
 
 
-class BlockDataPipe(data.IterDataPipe):
-    def __init__(self, block_datapipe, feature_map):
+class NpzIterDataPipe(IterDataPipe):
+    def __init__(self, data_blocks, feature_map):
         self.feature_map = feature_map
-        self.block_datapipe = block_datapipe
+        self.data_blocks = data_blocks
         
     def load_data(self, data_path):
         data_dict = np.load(data_path)
-        data_arrays = []
         all_cols = list(self.feature_map.features.keys()) + self.feature_map.labels
-        for col in all_cols:
-            array = data_dict[col]
-            if array.ndim == 1:
-                data_arrays.append(array.reshape(-1, 1))
-            else:
-                data_arrays.append(array)
-        data_tensor = torch.from_numpy(np.hstack(data_arrays))
-        return data_tensor
+        data_arrays = [data_dict[col] for col in all_cols]
+        return np.column_stack(data_arrays)
 
     def read_block(self, data_block):
         darray = self.load_data(data_block)
         for idx in range(darray.shape[0]):
             yield darray[idx, :]
 
     def __iter__(self):
-        worker_info = data.get_worker_info()
+        worker_info = get_worker_info()
         if worker_info is None: # single-process data loading
-            block_list = self.block_datapipe
+            block_list = self.data_blocks
         else: # in a worker process
             block_list = [
                 block
-                for idx, block in enumerate(self.block_datapipe)
+                for idx, block in enumerate(self.data_blocks)
                 if idx % worker_info.num_workers == worker_info.id
             ]
         return chain.from_iterable(map(self.read_block, block_list))
 
 
-class NpzBlockDataLoader(data.DataLoader):
-    def __init__(self, feature_map, data_path, batch_size=32, shuffle=False,
+class NpzBlockDataLoader(DataLoader):
+    def __init__(self, feature_map, data_path, split="train", batch_size=32, shuffle=False,
                  num_workers=1, buffer_size=100000, **kwargs):
-        data_blocks = glob.glob(data_path + "/*.npz")
+        if not data_path.endswith("npz"):
+            data_path = os.path.join(data_path, "*.npz")
+        data_blocks = sorted(glob.glob(data_path)) # sort by part name
         assert len(data_blocks) > 0, f"invalid data_path: {data_path}"
-        if len(data_blocks) > 1:
-            data_blocks.sort() # sort by part name
         self.data_blocks = data_blocks
         self.num_blocks = len(self.data_blocks)
         self.feature_map = feature_map
         self.batch_size = batch_size
         self.num_batches, self.num_samples = self.count_batches_and_samples()
-        datapipe = BlockDataPipe(data_blocks, feature_map)
+        datapipe = NpzIterDataPipe(self.data_blocks, feature_map)
         if shuffle:
             datapipe = datapipe.shuffle(buffer_size=buffer_size)
-        else:
-            num_workers = 1 # multiple workers cannot keep the order of data reading 
-        super(NpzBlockDataLoader, self).__init__(dataset=datapipe, batch_size=batch_size,
-                                                 num_workers=num_workers)
+        elif split == "test":
+            num_workers = 1 # multiple workers cannot keep the order of data reading
+        super().__init__(dataset=datapipe,
+                         batch_size=batch_size,
+                         num_workers=num_workers,
+                         collate_fn=BatchCollator(feature_map))
 
     def __len__(self):
         return self.num_batches
 
     def count_batches_and_samples(self):
         num_samples = 0
         for block_path in self.data_blocks:
             block_size = np.load(block_path)[self.feature_map.labels[0]].shape[0]
             num_samples += block_size
         num_batches = int(np.ceil(num_samples / self.batch_size))
         return num_batches, num_samples
+
+
+class BatchCollator(object):
+    def __init__(self, feature_map):
+        self.feature_map = feature_map
+
+    def __call__(self, batch):
+        batch_tensor = default_collate(batch)
+        all_cols = list(self.feature_map.features.keys()) + self.feature_map.labels
+        batch_dict = dict()
+        for col in all_cols:
+            batch_dict[col] = batch_tensor[:, self.feature_map.get_column_index(col)]
+        return batch_dict
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_dataloader.py` & `fuxictr-2.3.0/fuxictr/pytorch/dataloaders/parquet_dataloader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # =========================================================================
-# Copyright (C) 2022. Huawei Technologies Co., Ltd. All rights reserved.
+# Copyright (C) 2024. FuxiCTR Authors. All rights reserved.
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,49 +12,65 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
 import numpy as np
-from torch.utils import data
-import torch
+from torch.utils.data import Dataset, DataLoader
+from torch.utils.data.dataloader import default_collate
+import pandas as pd
+import polars as pl
 
 
-class Dataset(data.Dataset):
+class ParquetDataset(Dataset):
     def __init__(self, feature_map, data_path):
         self.feature_map = feature_map
         self.darray = self.load_data(data_path)
         
     def __getitem__(self, index):
         return self.darray[index, :]
     
     def __len__(self):
         return self.darray.shape[0]
 
     def load_data(self, data_path):
-        data_dict = np.load(data_path) # dict of arrays
-        data_arrays = []
+        df = pl.read_parquet(data_path)
         all_cols = list(self.feature_map.features.keys()) + self.feature_map.labels
+        data_arrays = []
         for col in all_cols:
-            array = data_dict[col]
-            if array.ndim == 1:
-                data_arrays.append(array.reshape(-1, 1))
+            if df[col].dtype != pl.List:
+                array = np.array(df[col])
             else:
-                data_arrays.append(array)
-        data_tensor = torch.from_numpy(np.hstack(data_arrays))
-        return data_tensor
+                array = np.array(df[col].to_list())
+            data_arrays.append(array)
+        return np.column_stack(data_arrays)
 
 
-class NpzDataLoader(data.DataLoader):
-    def __init__(self, feature_map, data_path, batch_size=32, shuffle=False, num_workers=1, **kwargs):
-        if not data_path.endswith(".npz"):
-            data_path += ".npz"
-        self.dataset = Dataset(feature_map, data_path)
-        super(NpzDataLoader, self).__init__(dataset=self.dataset, batch_size=batch_size,
-                                         shuffle=shuffle, num_workers=num_workers)
+class ParquetDataLoader(DataLoader):
+    def __init__(self, feature_map, data_path, batch_size=32, shuffle=False,
+                 num_workers=1, **kwargs):
+        if not data_path.endswith(".parquet"):
+            data_path += ".parquet"
+        self.dataset = ParquetDataset(feature_map, data_path)
+        super().__init__(dataset=self.dataset, batch_size=batch_size,
+                         shuffle=shuffle, num_workers=num_workers,
+                         collate_fn=BatchCollator(feature_map))
         self.num_samples = len(self.dataset)
         self.num_blocks = 1
-        self.num_batches = int(np.ceil(self.num_samples * 1.0 / self.batch_size))
+        self.num_batches = int(np.ceil(self.num_samples / self.batch_size))
 
     def __len__(self):
         return self.num_batches
+
+
+class BatchCollator(object):
+    def __init__(self, feature_map):
+        self.feature_map = feature_map
+
+    def __call__(self, batch):
+        batch_tensor = default_collate(batch)
+        all_cols = list(self.feature_map.features.keys()) + self.feature_map.labels
+        batch_dict = dict()
+        for col in all_cols:
+            batch_dict[col] = batch_tensor[:, self.feature_map.get_column_index(col)]
+        return batch_dict
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/rank_dataloader.py` & `fuxictr-2.3.0/fuxictr/pytorch/dataloaders/rank_dataloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,37 +13,57 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
 from .npz_block_dataloader import NpzBlockDataLoader
 from .npz_dataloader import NpzDataLoader
+from .parquet_block_dataloader import ParquetBlockDataLoader
+from .parquet_dataloader import ParquetDataLoader
 import logging
 
 
 class RankDataLoader(object):
     def __init__(self, feature_map, stage="both", train_data=None, valid_data=None, test_data=None,
-                 batch_size=32, shuffle=True, streaming=False, **kwargs):
+                 batch_size=32, shuffle=True, streaming=False, data_format="npz", **kwargs):
         logging.info("Loading datasets...")
         train_gen = None
         valid_gen = None
         test_gen = None
-        DataLoader = NpzBlockDataLoader if streaming else NpzDataLoader
+        if kwargs.get("data_loader"):
+            DataLoader = kwargs["data_loader"]
+        else:
+            if data_format == "npz":
+                DataLoader = NpzBlockDataLoader if streaming else NpzDataLoader
+            else: # ["parquet", "csv"]
+                DataLoader = ParquetBlockDataLoader if streaming else ParquetDataLoader
         self.stage = stage
         if stage in ["both", "train"]:
-            train_gen = DataLoader(feature_map, train_data, batch_size=batch_size, shuffle=shuffle, **kwargs)
-            logging.info("Train samples: total/{:d}, blocks/{:d}".format(train_gen.num_samples, train_gen.num_blocks))     
+            train_gen = DataLoader(feature_map, train_data, split="train", batch_size=batch_size,
+                                   shuffle=shuffle, **kwargs)
+            logging.info(
+                "Train samples: total/{:d}, blocks/{:d}"
+                .format(train_gen.num_samples, train_gen.num_blocks)
+            )     
             if valid_data:
-                valid_gen = DataLoader(feature_map, valid_data, batch_size=batch_size, shuffle=False, **kwargs)
-                logging.info("Validation samples: total/{:d}, blocks/{:d}".format(valid_gen.num_samples, valid_gen.num_blocks))
+                valid_gen = DataLoader(feature_map, valid_data, split="valid",
+                                       batch_size=batch_size, shuffle=False, **kwargs)
+                logging.info(
+                    "Validation samples: total/{:d}, blocks/{:d}"
+                    .format(valid_gen.num_samples, valid_gen.num_blocks)
+                )
 
         if stage in ["both", "test"]:
             if test_data:
-                test_gen = DataLoader(feature_map, test_data, batch_size=batch_size, shuffle=False, **kwargs)
-                logging.info("Test samples: total/{:d}, blocks/{:d}".format(test_gen.num_samples, test_gen.num_blocks))
+                test_gen = DataLoader(feature_map, test_data, split="test", batch_size=batch_size,
+                                      shuffle=False, **kwargs)
+                logging.info(
+                    "Test samples: total/{:d}, blocks/{:d}"
+                    .format(test_gen.num_samples, test_gen.num_blocks)
+                )
         self.train_gen, self.valid_gen, self.test_gen = train_gen, valid_gen, test_gen
 
     def make_iterator(self):
         if self.stage == "train":
             logging.info("Loading train and validation data done.")
             return self.train_gen, self.valid_gen
         elif self.stage == "test":
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import torch
 from torch import nn
 import os
 import numpy as np
 from collections import OrderedDict
 from .pretrained_embedding import PretrainedEmbedding
 from fuxictr.pytorch.torch_utils import get_initializer
+from fuxictr.utils import not_in_whitelist
 from fuxictr.pytorch import layers
 
 
 class FeatureEmbedding(nn.Module):
     def __init__(self, 
                  feature_map, 
                  embedding_dim,
@@ -140,45 +141,39 @@
         elif self.required_feature_columns and (feature not in self.required_feature_columns):
             return False
         elif self.not_required_feature_columns and (feature in self.not_required_feature_columns):
             return False
         else:
             return True
 
-    def dict2tensor(self, embedding_dict, feature_list=[], feature_source=[], feature_type=[], flatten_emb=False):
-        if type(feature_source) != list:
-            feature_source = [feature_source]
-        if type(feature_type) != list:
-            feature_type = [feature_type]
+    def dict2tensor(self, embedding_dict, flatten_emb=False, feature_list=[], feature_source=[],
+                    feature_type=[]):
         feature_emb_list = []
         for feature, feature_spec in self._feature_map.features.items():
-            if feature_source and feature_spec["source"] not in feature_source:
+            if feature_list and not_in_whitelist(feature, feature_list):
                 continue
-            if feature_type and feature_spec["type"] not in feature_type:
+            if feature_source and not_in_whitelist(feature_spec["source"], feature_source):
                 continue
-            if feature_list and feature not in feature_list:
+            if feature_type and not_in_whitelist(feature_spec["type"], feature_type):
                 continue
             if feature in embedding_dict:
                 feature_emb_list.append(embedding_dict[feature])
         if flatten_emb:
             feature_emb = torch.cat(feature_emb_list, dim=-1)
         else:
             feature_emb = torch.stack(feature_emb_list, dim=1)
         return feature_emb
 
     def forward(self, inputs, feature_source=[], feature_type=[]):
-        if type(feature_source) != list:
-            feature_source = [feature_source]
-        if type(feature_type) != list:
-            feature_type = [feature_type]
         feature_emb_dict = OrderedDict()
-        for feature, feature_spec in self._feature_map.features.items():
-            if feature_source and feature_spec["source"] not in feature_source:
+        for feature in inputs.keys():
+            feature_spec = self._feature_map.features[feature]
+            if feature_source and not_in_whitelist(feature_spec["source"], feature_source):
                 continue
-            if feature_type and feature_spec["type"] not in feature_type:
+            if feature_type and not_in_whitelist(feature_spec["type"], feature_type):
                 continue
             if feature in self.embedding_layers:
                 if feature_spec["type"] == "numeric":
                     inp = inputs[feature].float().view(-1, 1)
                     embeddings = self.embedding_layers[feature](inp)
                 elif feature_spec["type"] == "categorical":
                     inp = inputs[feature].long()
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 
 import torch
 from torch import nn
-import h5py
 import os
 import io
 import json
 import numpy as np
 import logging
+from ....utils import load_pretrain_emb
 
 
 class PretrainedEmbedding(nn.Module):
     def __init__(self,
                  feature_name,
                  feature_spec,
                  pretrain_path,
@@ -62,25 +62,14 @@
             self.proj = nn.Linear(pretrain_dim + embedding_dim, embedding_dim, bias=False)
 
     def reset_parameters(self, embedding_initializer):
         if self.pretrain_usage in ["sum", "concat"]:
             nn.init.zeros_(self.id_embedding.weight) # set oov token embeddings to zeros
             embedding_initializer(self.id_embedding.weight[1:self.oov_idx, :])
 
-    def get_pretrained_embedding(self, pretrain_path):
-        logging.info("Loading pretrained_emb: {}".format(pretrain_path))
-        if pretrain_path.endswith("h5"):
-            with h5py.File(pretrain_path, 'r') as hf:
-                keys = hf["key"][:]
-                embeddings = hf["value"][:]
-        elif pretrain_path.endswith("npz"):
-            npz = np.load(pretrain_path)
-            keys, embeddings = npz["key"], npz["value"]
-        return keys, embeddings
-
     def load_feature_vocab(self, vocab_path, feature_name):
         with io.open(vocab_path, "r", encoding="utf-8") as fd:
             vocab = json.load(fd)
             vocab_type = type(list(vocab.items())[1][0]) # get key dtype
         return vocab[feature_name], vocab_type
 
     def load_pretrained_embedding(self, vocab_size, pretrain_dim, pretrain_path, vocab_path,
@@ -90,15 +79,16 @@
                                        padding_idx=padding_idx)
         if freeze:
             embedding_matrix = np.zeros((vocab_size, pretrain_dim))
         else:
             embedding_matrix = np.random.normal(loc=0, scale=1.e-4, size=(vocab_size, pretrain_dim))
             if padding_idx:
                 embedding_matrix[padding_idx, :] = np.zeros(pretrain_dim) # set as zero for PAD
-        keys, embeddings = self.get_pretrained_embedding(pretrain_path)
+        logging.info("Loading pretrained_emb: {}".format(pretrain_path))
+        keys, embeddings = load_pretrain_emb(pretrain_path, keys=["key", "value"])
         assert embeddings.shape[-1] == pretrain_dim, f"pretrain_dim={pretrain_dim} not correct."
         vocab, vocab_type = self.load_feature_vocab(vocab_path, feature_name)
         keys = keys.astype(vocab_type) # ensure the same dtype between pretrained keys and vocab keys
         for idx, word in enumerate(keys):
             if word in vocab:
                 embedding_matrix[vocab[word]] = embeddings[idx]
         embedding_layer.weight = torch.nn.Parameter(torch.from_numpy(embedding_matrix).float())
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.3.0/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.3.0/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/models/rank_model.py` & `fuxictr-2.3.0/fuxictr/pytorch/models/rank_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # =========================================================================
+# Copyright (C) 2023. FuxiCTR Authors. All rights reserved.
 # Copyright (C) 2022. Huawei Technologies Co., Ltd. All rights reserved.
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -18,15 +19,15 @@
 import torch.nn as nn
 import numpy as np
 import torch
 import os, sys
 import logging
 from fuxictr.metrics import evaluate_metrics
 from fuxictr.pytorch.torch_utils import get_device, get_optimizer, get_loss, get_regularizer
-from fuxictr.utils import Monitor
+from fuxictr.utils import Monitor, not_in_whitelist
 from tqdm import tqdm
 
 
 class BaseModel(nn.Module):
     def __init__(self, 
                  feature_map, 
                  model_id="BaseModel", 
@@ -98,34 +99,35 @@
             # initialize layers with customized reset_parameters
             if hasattr(m, 'reset_custom_params'):
                 m.reset_custom_params()
         self.apply(reset_default_params)
         self.apply(reset_custom_params)
 
     def get_inputs(self, inputs, feature_source=None):
-        if feature_source and type(feature_source) == str:
-            feature_source = [feature_source]
         X_dict = dict()
-        for feature, spec in self.feature_map.features.items():
-            if (feature_source is not None) and (spec["source"] not in feature_source):
+        for feature in inputs.keys():
+            if feature in self.feature_map.labels:
                 continue
+            spec = self.feature_map.features[feature]
             if spec["type"] == "meta":
                 continue
-            X_dict[feature] = inputs[:, self.feature_map.get_column_index(feature)].to(self.device)
+            if feature_source and not_in_whitelist(spec["source"], feature_source):
+                continue
+            X_dict[feature] = inputs[feature].to(self.device)
         return X_dict
 
     def get_labels(self, inputs):
         """ Please override get_labels() when using multiple labels!
         """
         labels = self.feature_map.labels
-        y = inputs[:, self.feature_map.get_column_index(labels[0])].to(self.device)
+        y = inputs[labels[0]].to(self.device)
         return y.float().view(-1, 1)
                 
     def get_group_id(self, inputs):
-        return inputs[:, self.feature_map.get_column_index(self.feature_map.group_id)]
+        return inputs[self.feature_map.group_id]
 
     def model_to_device(self):
         self.to(device=self.device)
 
     def lr_decay(self, factor=0.1, min_lr=1e-6):
         for param_group in self.optimizer.param_groups:
             reduced_lr = max(param_group["lr"] * factor, min_lr)
```

### Comparing `fuxictr-2.2.3/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.3.0/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.3.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.3.0/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/models/rank_model.py` & `fuxictr-2.3.0/fuxictr/tensorflow/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.3.0/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.3/fuxictr/utils.py` & `fuxictr-2.3.0/fuxictr/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 import os
 import logging
 import logging.config
 import yaml
 import glob
 import json
+import h5py
+import numpy as np
+import pandas as pd
 from collections import OrderedDict
 
 
 def load_config(config_dir, experiment_id):
     params = load_model_config(config_dir, experiment_id)
     data_params = load_dataset_config(config_dir, params['dataset_id'])
     params.update(data_params)
@@ -86,21 +89,48 @@
     if sort_keys:
         new_data = OrderedDict(sorted(new_data.items(), key=lambda x: x[0]))
     return json.dumps(new_data, indent=4)
 
 def print_to_list(data):
     return ' - '.join('{}: {:.6f}'.format(k, v) for k, v in data.items())
 
+
 class Monitor(object):
     def __init__(self, kv):
         if isinstance(kv, str):
             kv = {kv: 1}
         self.kv_pairs = kv
 
     def get_value(self, logs):
         value = 0
         for k, v in self.kv_pairs.items():
             value += logs.get(k, 0) * v
         return value
 
     def get_metrics(self):
         return list(self.kv_pairs.keys())
+
+
+def load_pretrain_emb(pretrain_path, keys=["key", "value"]):
+    if type(keys) != list:
+        keys = [keys]
+    if pretrain_path.endswith("h5"):
+        with h5py.File(pretrain_path, 'r') as hf:
+            values = [hf[k][:] for k in keys]
+    elif pretrain_path.endswith("npz"):
+        npz = np.load(pretrain_path)
+        values = [npz[k] for k in keys]
+    elif pretrain_path.endswith("parquet"):
+        df = pd.read_parquet(pretrain_path)
+        values = [df[k].values for k in keys]
+    else:
+        raise ValueError(f"Embedding format not supported: {pretrain_path}")
+    return values[0] if len(values) == 1 else values
+
+
+def not_in_whitelist(element, whitelist=[]):
+    if not whitelist:
+        return False
+    elif type(whitelist) == list:
+        return element not in whitelist
+    else:
+        return element != whitelist
```

### Comparing `fuxictr-2.2.3/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.3.0/fuxictr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.3
+Version: 2.3.0
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
         <img src="https://cdn.jsdelivr.net/gh/reczoo/FuxiCTR@main/docs/img/logo.png" alt="Logo" width="260"/>
         </div>
         
         <div align="center">
-        <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
+        <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.9+-blue" style="max-width: 100%;" alt="Python version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
         <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
         <a href="https://github.com/reczoo/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/reczoo/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
         </div>
         <hr/>
@@ -107,15 +107,15 @@
         + :star: [Benchmark settings and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr)
         + :star: [Benchmark leaderboard for CTR prediction](https://openbenchmark.github.io/BARS/CTR/leaderboard)
         
         ## Dependencies
         
         FuxiCTR has the following dependencies:
         
-        + python 3.6+
+        + python 3.9+
         + pytorch 1.10+ (required only for Torch models)
         + tensorflow 2.1+ (required only for TF models)
         
         Please install other required packages via `pip install -r requirements.txt`.
         
         ## Quick Start
         
@@ -177,15 +177,14 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.3 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.3.0 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
@@ -220,15 +220,15 @@
 abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | ##
 Benchmarking We have benchmarked FuxiCTR models on a set of open datasets as
 follows: + :star: [Benchmark datasets for CTR prediction](https://github.com/
 reczoo/Datasets?tab=readme-ov-file#ctr-prediction) + :star: [Benchmark settings
 and running steps](https://github.com/reczoo/BARS/tree/main/ranking/ctr) + :
 star: [Benchmark leaderboard for CTR prediction](https://
 openbenchmark.github.io/BARS/CTR/leaderboard) ## Dependencies FuxiCTR has the
-following dependencies: + python 3.6+ + pytorch 1.10+ (required only for Torch
+following dependencies: + python 3.9+ + pytorch 1.10+ (required only for Torch
 models) + tensorflow 2.1+ (required only for TF models) Please install other
 required packages via `pip install -r requirements.txt`. ## Quick Start 1. Run
 the demo examples Examples are provided in the demo directory to show some
 basic usage of FuxiCTR. Users can run the examples for quick start and to
 understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
 python example2_DeepFM_with_h5_input.py ``` 2. Run a model on tiny data Users
 can easily run each model in the model zoo following the commands below, which
@@ -269,13 +269,12 @@
 and practice in recommender systems, please reach out via our WeChat group. !
 [Scan QR code](https://openbenchmark.github.io/BARS/_images/wechat.jpg)
 Keywords: ctr prediction,recommender systems,ctr,cvr,pytorch Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.6 Description-Content-Type:
-text/markdown
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
+Content-Type: text/markdown
```

### Comparing `fuxictr-2.2.3/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.3.0/fuxictr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 fuxictr/preprocess/normalizer.py
 fuxictr/preprocess/tokenizer.py
 fuxictr/pytorch/__init__.py
 fuxictr/pytorch/torch_utils.py
 fuxictr/pytorch/dataloaders/__init__.py
 fuxictr/pytorch/dataloaders/npz_block_dataloader.py
 fuxictr/pytorch/dataloaders/npz_dataloader.py
+fuxictr/pytorch/dataloaders/parquet_block_dataloader.py
+fuxictr/pytorch/dataloaders/parquet_dataloader.py
 fuxictr/pytorch/dataloaders/rank_dataloader.py
 fuxictr/pytorch/layers/__init__.py
 fuxictr/pytorch/layers/activations.py
 fuxictr/pytorch/layers/pooling.py
 fuxictr/pytorch/layers/attentions/__init__.py
 fuxictr/pytorch/layers/attentions/dot_product_attention.py
 fuxictr/pytorch/layers/attentions/squeeze_excitation.py
```

### Comparing `fuxictr-2.2.3/setup.py` & `fuxictr-2.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.2.3",
+    version="2.3.0",
     author="RECZOO",
     author_email="reczoo@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/reczoo/FuxiCTR",
     download_url='https://github.com/reczoo/FuxiCTR/tags',
     packages=setuptools.find_packages(
         exclude=["model_zoo", "tests", "data", "docs", "demo"]),
     include_package_data=True,
     python_requires=">=3.6",
-    install_requires=["pandas", "numpy", "h5py", "PyYAML>=5.1", "scikit-learn", "tqdm"],
+    install_requires=["keras_preprocessing", "pandas", "PyYAML>=5.1", "scikit-learn",
+                      "numpy", "h5py", "tqdm", "pyarrow", "polars"],
     classifiers=(
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ),
     license="Apache-2.0 License",
```

