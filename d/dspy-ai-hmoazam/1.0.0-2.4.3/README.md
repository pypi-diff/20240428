# Comparing `tmp/dspy-ai-hmoazam-1.0.0.tar.gz` & `tmp/dspy-ai-hmoazam-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspy-ai-hmoazam-1.0.0.tar", last modified: Sat Apr 27 22:14:06 2024, max compression
+gzip compressed data, was "dspy-ai-hmoazam-2.4.3.tar", last modified: Sat Apr 27 22:06:32 2024, max compression
```

## Comparing `dspy-ai-hmoazam-1.0.0.tar` & `dspy-ai-hmoazam-2.4.3.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.865090 dspy-ai-hmoazam-1.0.0/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1085 2024-04-27 21:13:59.000000 dspy-ai-hmoazam-1.0.0/LICENSE
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    36084 2024-04-27 22:14:06.864911 dspy-ai-hmoazam-1.0.0/PKG-INFO
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    35291 2024-04-27 21:13:59.000000 dspy-ai-hmoazam-1.0.0/README.md
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.824001 dspy-ai-hmoazam-1.0.0/dsp/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1532 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/__init__.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.824670 dspy-ai-hmoazam-1.0.0/dsp/evaluation/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/evaluation/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2586 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/evaluation/utils.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.830989 dspy-ai-hmoazam-1.0.0/dsp/modules/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      760 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4439 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/anthropic.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    10296 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/aws_models.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4525 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/aws_providers.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     9513 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/azure_openai.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3135 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1018 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/cache_utils.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3008 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/clarifai.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3313 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/cohere.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2156 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/colbertv2.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5278 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/databricks.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3788 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/dummy_lm.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.831444 dspy-ai-hmoazam-1.0.0/dsp/modules/finetuning/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       26 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    15071 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4552 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/google.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5992 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/googlevertexai.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     8562 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/gpt3.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4859 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/groq_client.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     8119 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/hf.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    17704 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/hf_client.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2087 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/hf_server.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3721 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/lm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3655 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/mistral.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6751 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/ollama.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3152 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/pyserini.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      693 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/sbert.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     7787 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/modules/sentence_vectorizer.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.833182 dspy-ai-hmoazam-1.0.0/dsp/primitives/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      145 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5185 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/compiler.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5789 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/demonstrate.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2471 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/inspect.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     8432 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/predict.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1439 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/primitives.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2727 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/primitives/search.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.834212 dspy-ai-hmoazam-1.0.0/dsp/templates/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       76 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/templates/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    10226 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/templates/template_v2.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2334 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/templates/template_v3.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1900 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/templates/utils.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.835885 dspy-ai-hmoazam-1.0.0/dsp/utils/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      123 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4903 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/ann_utils.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     7110 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/dpr.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5933 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/metrics.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3215 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/settings.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2828 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/settings_v2.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5623 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dsp/utils/utils.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.836143 dspy-ai-hmoazam-1.0.0/dspy/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1059 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/__init__.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.837193 dspy-ai-hmoazam-1.0.0/dspy/adapters/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/adapters/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/adapters/basic_adapter.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/adapters/vicuna_adapter.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.839710 dspy-ai-hmoazam-1.0.0/dspy/datasets/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      122 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2986 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/colors.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4949 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/dataloader.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4098 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/dataset.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2618 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/gsm8k.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3286 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/datasets/hotpotqa.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.840792 dspy-ai-hmoazam-1.0.0/dspy/evaluate/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      127 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/evaluate/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1421 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    10081 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/evaluate/evaluate.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      882 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/evaluate/metrics.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.841463 dspy-ai-hmoazam-1.0.0/dspy/experimental/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       57 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/__init__.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.843321 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       26 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      834 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/config.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      527 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5543 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     9723 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      599 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4237 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/experimental/synthetic_data.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.843854 dspy-ai-hmoazam-1.0.0/dspy/functional/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       94 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/functional/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    19499 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-1.0.0/dspy/functional/functional.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.847870 dspy-ai-hmoazam-1.0.0/dspy/predict/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      348 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1842 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/aggregation.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3589 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/chain_of_thought.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1527 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1017 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/knn.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6117 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/langchain.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1659 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       58 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/parameter.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5580 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/predict.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     7603 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/program_of_thought.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4458 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/react.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2827 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/predict/retry.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.850581 dspy-ai-hmoazam-1.0.0/dspy/primitives/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      132 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    11407 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/assertions.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     7779 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/box.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3471 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/example.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2647 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/module.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2807 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/prediction.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3366 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/program.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    25710 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/primitives/python_interpreter.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.856887 dspy-ai-hmoazam-1.0.0/dspy/retrieve/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       30 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    17405 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/azureaisearch_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4812 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3275 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6604 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3897 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0 hanna.moazam   (502) staff       (20)     6605 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3459 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3998 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/milvus_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3774 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6213 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5930 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    10476 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3271 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2425 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/ragatouille_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1442 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/retrieve.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5659 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4491 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      438 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1678 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/retrieve/you_rm.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.857801 dspy-ai-hmoazam-1.0.0/dspy/signatures/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       46 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/signatures/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2758 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/signatures/field.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    14464 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/signatures/signature.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.862134 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      390 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     9532 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    17739 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1359 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/ensemble.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     6292 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/finetune.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      879 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    31087 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     8130 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/random_search.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     2673 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3878 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    11876 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       57 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3208 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      948 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/teleprompt/vanilla.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.863058 dspy-ai-hmoazam-1.0.0/dspy/utils/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       46 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/utils/__init__.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     5643 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/utils/dummies.py
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     3193 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-1.0.0/dspy/utils/logging.py
-drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:14:06.864447 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/
--rw-r--r--   0 hanna.moazam   (502) staff       (20)    36084 2024-04-27 22:14:06.000000 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/PKG-INFO
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     4006 2024-04-27 22:14:06.000000 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/SOURCES.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-27 22:14:06.000000 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/dependency_links.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)      345 2024-04-27 22:14:06.000000 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/requires.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)        9 2024-04-27 22:14:06.000000 dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/top_level.txt
--rw-r--r--   0 hanna.moazam   (502) staff       (20)       38 2024-04-27 22:14:06.865138 dspy-ai-hmoazam-1.0.0/setup.cfg
--rw-r--r--   0 hanna.moazam   (502) staff       (20)     1503 2024-04-27 22:12:54.000000 dspy-ai-hmoazam-1.0.0/setup.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.830128 dspy-ai-hmoazam-2.4.3/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1085 2024-04-27 21:13:59.000000 dspy-ai-hmoazam-2.4.3/LICENSE
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    36218 2024-04-27 22:06:32.829861 dspy-ai-hmoazam-2.4.3/PKG-INFO
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    35291 2024-04-27 21:13:59.000000 dspy-ai-hmoazam-2.4.3/README.md
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.777577 dspy-ai-hmoazam-2.4.3/dsp/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1532 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/__init__.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.778107 dspy-ai-hmoazam-2.4.3/dsp/evaluation/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/evaluation/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2586 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/evaluation/utils.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.784663 dspy-ai-hmoazam-2.4.3/dsp/modules/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      760 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4439 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/anthropic.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    10296 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/aws_models.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4525 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/aws_providers.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     9513 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/azure_openai.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3135 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/azurecognitivesearch.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1018 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/cache_utils.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3008 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/clarifai.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3313 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/cohere.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2156 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/colbertv2.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5278 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/databricks.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3788 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/dummy_lm.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.785190 dspy-ai-hmoazam-2.4.3/dsp/modules/finetuning/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       26 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/finetuning/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    15071 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/finetuning/finetune_hf.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4552 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/google.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5992 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/googlevertexai.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     8562 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/gpt3.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4859 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/groq_client.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     8119 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/hf.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    17704 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/hf_client.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2087 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/hf_server.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3721 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/lm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3655 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/mistral.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     6751 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/ollama.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3152 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/pyserini.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      693 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/sbert.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     7787 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/modules/sentence_vectorizer.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.786962 dspy-ai-hmoazam-2.4.3/dsp/primitives/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      145 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5185 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/compiler.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5789 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/demonstrate.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2471 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/inspect.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     8432 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/predict.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1439 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/primitives.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2727 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/primitives/search.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.787933 dspy-ai-hmoazam-2.4.3/dsp/templates/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       76 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/templates/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    10226 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/templates/template_v2.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2334 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/templates/template_v3.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1900 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/templates/utils.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.789665 dspy-ai-hmoazam-2.4.3/dsp/utils/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      123 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4903 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/ann_utils.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     7110 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/dpr.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5933 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/metrics.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3215 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/settings.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2828 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/settings_v2.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5623 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dsp/utils/utils.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.789923 dspy-ai-hmoazam-2.4.3/dspy/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1059 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/__init__.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.790969 dspy-ai-hmoazam-2.4.3/dspy/adapters/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/adapters/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/adapters/basic_adapter.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/adapters/chatml_adapter.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/adapters/llamachat_adapter.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/adapters/vicuna_adapter.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.792506 dspy-ai-hmoazam-2.4.3/dspy/datasets/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      122 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2986 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/colors.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4949 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/dataloader.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4098 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/dataset.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2618 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/gsm8k.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3286 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/datasets/hotpotqa.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.793517 dspy-ai-hmoazam-2.4.3/dspy/evaluate/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      127 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/evaluate/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1421 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/evaluate/auto_evaluation.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    10081 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/evaluate/evaluate.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      882 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/evaluate/metrics.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.794223 dspy-ai-hmoazam-2.4.3/dspy/experimental/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       57 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/__init__.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.797945 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       26 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      834 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/config.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      527 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5543 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/signatures.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     9723 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/synthesizer.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      599 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/utils.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4237 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/experimental/synthetic_data.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.798963 dspy-ai-hmoazam-2.4.3/dspy/functional/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       94 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/functional/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    19499 2024-04-27 21:14:00.000000 dspy-ai-hmoazam-2.4.3/dspy/functional/functional.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.806258 dspy-ai-hmoazam-2.4.3/dspy/predict/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      348 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1842 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/aggregation.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3589 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/chain_of_thought.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1527 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/chain_of_thought_with_hint.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1017 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/knn.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     6117 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/langchain.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1659 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/multi_chain_comparison.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       58 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/parameter.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5580 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/predict.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     7603 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/program_of_thought.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4458 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/react.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2827 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/predict/retry.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.810944 dspy-ai-hmoazam-2.4.3/dspy/primitives/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      132 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    11407 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/assertions.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     7779 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/box.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3471 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/example.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2647 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/module.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2807 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/prediction.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3366 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/program.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    25710 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/primitives/python_interpreter.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.820974 dspy-ai-hmoazam-2.4.3/dspy/retrieve/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       30 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    17405 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/azureaisearch_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4812 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/chromadb_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3275 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/clarifai_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     6604 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/databricks_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3897 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/deeplake_rm.py
+-rwxr-xr-x   0 hanna.moazam   (502) staff       (20)     6605 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/faiss_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3459 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/marqo_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3998 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/milvus_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3774 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/mongodb_atlas_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     6213 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/neo4j_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5930 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/pgvector_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    10476 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/pinecone_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3271 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/qdrant_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2425 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/ragatouille_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1442 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/retrieve.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5659 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/vectara_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4491 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/weaviate_rm.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      438 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/weaviate_rm_test.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1678 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/retrieve/you_rm.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.822177 dspy-ai-hmoazam-2.4.3/dspy/signatures/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       46 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/signatures/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2758 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/signatures/field.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    14464 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/signatures/signature.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.826485 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      390 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     9532 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/bootstrap.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    17739 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/copro_optimizer.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1359 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/ensemble.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     6292 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/finetune.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      879 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/knn_fewshot.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    31087 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/mipro_optimizer.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     8130 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/random_search.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     2673 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3878 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt_bayesian.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    11876 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt_typed.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       57 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/teleprompt.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3208 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/teleprompt_optuna.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      948 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/teleprompt/vanilla.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.827305 dspy-ai-hmoazam-2.4.3/dspy/utils/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       46 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/utils/__init__.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     5643 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/utils/dummies.py
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     3193 2024-04-27 21:14:01.000000 dspy-ai-hmoazam-2.4.3/dspy/utils/logging.py
+drwxr-xr-x   0 hanna.moazam   (502) staff       (20)        0 2024-04-27 22:06:32.829336 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)    36218 2024-04-27 22:06:32.000000 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/PKG-INFO
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     4021 2024-04-27 22:06:32.000000 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/SOURCES.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        1 2024-04-27 22:06:32.000000 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/dependency_links.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)      714 2024-04-27 22:06:32.000000 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/requires.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)        9 2024-04-27 22:06:32.000000 dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/top_level.txt
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     7330 2024-04-27 21:18:48.000000 dspy-ai-hmoazam-2.4.3/pyproject.toml
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)       38 2024-04-27 22:06:32.830204 dspy-ai-hmoazam-2.4.3/setup.cfg
+-rw-r--r--   0 hanna.moazam   (502) staff       (20)     1503 2024-04-27 22:03:55.000000 dspy-ai-hmoazam-2.4.3/setup.py
```

### Comparing `dspy-ai-hmoazam-1.0.0/LICENSE` & `dspy-ai-hmoazam-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/PKG-INFO` & `dspy-ai-hmoazam-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: dspy-ai-hmoazam
-Version: 1.0.0
+Version: 2.4.3
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
-Author-email: okhattab@stanford.edu
+Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
+Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: anthropic
+Provides-Extra: milvus
+Provides-Extra: aws
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
 <p align="left">
```

### Comparing `dspy-ai-hmoazam-1.0.0/README.md` & `dspy-ai-hmoazam-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/__init__.py` & `dspy-ai-hmoazam-2.4.3/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/evaluation/utils.py` & `dspy-ai-hmoazam-2.4.3/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/__init__.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/anthropic.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/anthropic.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/aws_models.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/aws_models.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/aws_providers.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/aws_providers.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/azure_openai.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/azure_openai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/azurecognitivesearch.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/azurecognitivesearch.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/cache_utils.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/cache_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/clarifai.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/cohere.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/cohere.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/colbertv2.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/databricks.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/databricks.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/dummy_lm.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/dummy_lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/google.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/googlevertexai.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/googlevertexai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/gpt3.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/gpt3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/groq_client.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/groq_client.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/hf.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/hf_client.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/hf_client.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/hf_server.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/lm.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/lm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/mistral.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/mistral.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/ollama.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/pyserini.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/sbert.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/modules/sentence_vectorizer.py` & `dspy-ai-hmoazam-2.4.3/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/compiler.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/demonstrate.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/inspect.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/predict.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/primitives.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/primitives/search.py` & `dspy-ai-hmoazam-2.4.3/dsp/primitives/search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/templates/template_v2.py` & `dspy-ai-hmoazam-2.4.3/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/templates/template_v3.py` & `dspy-ai-hmoazam-2.4.3/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/templates/utils.py` & `dspy-ai-hmoazam-2.4.3/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/ann_utils.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/dpr.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/metrics.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/settings.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/settings_v2.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dsp/utils/utils.py` & `dspy-ai-hmoazam-2.4.3/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/__init__.py` & `dspy-ai-hmoazam-2.4.3/dspy/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/datasets/colors.py` & `dspy-ai-hmoazam-2.4.3/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/datasets/dataloader.py` & `dspy-ai-hmoazam-2.4.3/dspy/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/datasets/dataset.py` & `dspy-ai-hmoazam-2.4.3/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/datasets/gsm8k.py` & `dspy-ai-hmoazam-2.4.3/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/datasets/hotpotqa.py` & `dspy-ai-hmoazam-2.4.3/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/evaluate/auto_evaluation.py` & `dspy-ai-hmoazam-2.4.3/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/evaluate/evaluate.py` & `dspy-ai-hmoazam-2.4.3/dspy/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/evaluate/metrics.py` & `dspy-ai-hmoazam-2.4.3/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/config.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/signatures.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/synthesizer.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/synthesizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthesizer/utils.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/experimental/synthetic_data.py` & `dspy-ai-hmoazam-2.4.3/dspy/experimental/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/functional/functional.py` & `dspy-ai-hmoazam-2.4.3/dspy/functional/functional.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/aggregation.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/chain_of_thought.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/knn.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/langchain.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/multi_chain_comparison.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/predict.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/predict.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/program_of_thought.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/program_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/react.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/react.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/predict/retry.py` & `dspy-ai-hmoazam-2.4.3/dspy/predict/retry.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/assertions.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/assertions.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/box.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/example.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/example.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/module.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/module.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/prediction.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/program.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/primitives/python_interpreter.py` & `dspy-ai-hmoazam-2.4.3/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/azureaisearch_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/azureaisearch_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/chromadb_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/chromadb_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/clarifai_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/clarifai_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/databricks_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/databricks_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/deeplake_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/deeplake_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/faiss_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/faiss_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/marqo_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/milvus_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/milvus_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/neo4j_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/pgvector_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/pgvector_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/pinecone_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/qdrant_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/qdrant_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/ragatouille_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/ragatouille_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/retrieve.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/retrieve.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/vectara_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/weaviate_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/weaviate_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/retrieve/you_rm.py` & `dspy-ai-hmoazam-2.4.3/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/signatures/field.py` & `dspy-ai-hmoazam-2.4.3/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/signatures/signature.py` & `dspy-ai-hmoazam-2.4.3/dspy/signatures/signature.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/bootstrap.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/copro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/ensemble.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/finetune.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/mipro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/random_search.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/random_search.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/teleprompt/vanilla.py` & `dspy-ai-hmoazam-2.4.3/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/utils/dummies.py` & `dspy-ai-hmoazam-2.4.3/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy/utils/logging.py` & `dspy-ai-hmoazam-2.4.3/dspy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/PKG-INFO` & `dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: dspy-ai-hmoazam
-Version: 1.0.0
+Version: 2.4.3
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
-Author-email: okhattab@stanford.edu
+Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
+Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: anthropic
+Provides-Extra: milvus
+Provides-Extra: aws
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
 <p align="left">
```

### Comparing `dspy-ai-hmoazam-1.0.0/dspy_ai_hmoazam.egg-info/SOURCES.txt` & `dspy-ai-hmoazam-2.4.3/dspy_ai_hmoazam.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 dsp/__init__.py
 dsp/evaluation/__init__.py
 dsp/evaluation/utils.py
 dsp/modules/__init__.py
 dsp/modules/anthropic.py
 dsp/modules/aws_models.py
```

### Comparing `dspy-ai-hmoazam-1.0.0/setup.py` & `dspy-ai-hmoazam-2.4.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai-hmoazam",	
-    version="1.0.0",	
+    version="2.4.1",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",
```

