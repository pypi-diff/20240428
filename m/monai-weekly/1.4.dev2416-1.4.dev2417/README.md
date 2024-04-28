# Comparing `tmp/monai_weekly-1.4.dev2416.tar.gz` & `tmp/monai_weekly-1.4.dev2417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai_weekly-1.4.dev2416.tar", last modified: Sun Apr 21 02:14:43 2024, max compression
+gzip compressed data, was "monai_weekly-1.4.dev2417.tar", last modified: Sun Apr 28 02:16:31 2024, max compression
```

## Comparing `monai_weekly-1.4.dev2416.tar` & `monai_weekly-1.4.dev2417.tar`

### file list

```diff
@@ -1,1186 +1,1186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.873867 monai_weekly-1.4.dev2416/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-21 02:14:43.873867 monai_weekly-1.4.dev2416/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.877867 monai_weekly-1.4.dev2416/monai/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-21 02:13:06.000000 monai_weekly-1.4.dev2416/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.661863 monai_weekly-1.4.dev2416/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.661863 monai_weekly-1.4.dev2416/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 02:14:43.877867 monai_weekly-1.4.dev2416/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.661863 monai_weekly-1.4.dev2416/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.661863 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.665864 monai_weekly-1.4.dev2416/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.669864 monai_weekly-1.4.dev2416/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.673864 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.677864 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.677864 monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.677864 monai_weekly-1.4.dev2416/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.677864 monai_weekly-1.4.dev2416/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.681864 monai_weekly-1.4.dev2416/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.681864 monai_weekly-1.4.dev2416/monai/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.685864 monai_weekly-1.4.dev2416/monai/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    79098 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    61767 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/ultrasound_confidence_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.685864 monai_weekly-1.4.dev2416/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.685864 monai_weekly-1.4.dev2416/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.685864 monai_weekly-1.4.dev2416/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)    33623 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.689864 monai_weekly-1.4.dev2416/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.693864 monai_weekly-1.4.dev2416/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.693864 monai_weekly-1.4.dev2416/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.697864 monai_weekly-1.4.dev2416/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/cldice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    19427 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.701864 monai_weekly-1.4.dev2416/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/mmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.701864 monai_weekly-1.4.dev2416/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.709864 monai_weekly-1.4.dev2416/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/pos_embed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.709864 monai_weekly-1.4.dev2416/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.717865 monai_weekly-1.4.dev2416/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22089 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/nets/voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)    49607 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.717865 monai_weekly-1.4.dev2416/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.721865 monai_weekly-1.4.dev2416/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/regularization/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/regularization/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/signal/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/signal/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.725865 monai_weekly-1.4.dev2416/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    91619 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.729865 monai_weekly-1.4.dev2416/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/tf32.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.733865 monai_weekly-1.4.dev2416/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.865867 monai_weekly-1.4.dev2416/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35592 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 02:14:43.000000 monai_weekly-1.4.dev2416/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-21 02:14:43.877867 monai_weekly-1.4.dev2416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:14:43.865867 monai_weekly-1.4.dev2416/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_push_to_hf_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cldice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_clip_intensity_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_clip_intensity_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_fid_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_mmd_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_multiscalessim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_diffusion_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_distance_transform_edt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_freeze_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gdsdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_perceptual_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_simulate_low_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_simulate_low_resolutiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_fillemptyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_soft_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_squeeze_unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    23815 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_ultrasound_confidence_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-21 02:13:03.000000 monai_weekly-1.4.dev2416/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-04-21 02:13:04.000000 monai_weekly-1.4.dev2416/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.863603 monai_weekly-1.4.dev2417/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-28 02:16:31.863603 monai_weekly-1.4.dev2417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.863603 monai_weekly-1.4.dev2417/monai/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-28 02:15:07.000000 monai_weekly-1.4.dev2417/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.659605 monai_weekly-1.4.dev2417/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.659605 monai_weekly-1.4.dev2417/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-28 02:16:31.863603 monai_weekly-1.4.dev2417/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.659605 monai_weekly-1.4.dev2417/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40110 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.663605 monai_weekly-1.4.dev2417/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.667605 monai_weekly-1.4.dev2417/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.671605 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.675605 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.675605 monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.675605 monai_weekly-1.4.dev2417/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.675605 monai_weekly-1.4.dev2417/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.679605 monai_weekly-1.4.dev2417/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.679605 monai_weekly-1.4.dev2417/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.683605 monai_weekly-1.4.dev2417/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79098 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61767 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/ultrasound_confidence_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.683605 monai_weekly-1.4.dev2417/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.683605 monai_weekly-1.4.dev2417/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.683605 monai_weekly-1.4.dev2417/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33623 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.687605 monai_weekly-1.4.dev2417/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.691604 monai_weekly-1.4.dev2417/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.691604 monai_weekly-1.4.dev2417/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.695604 monai_weekly-1.4.dev2417/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/cldice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.699604 monai_weekly-1.4.dev2417/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.699604 monai_weekly-1.4.dev2417/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.703604 monai_weekly-1.4.dev2417/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/pos_embed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.707604 monai_weekly-1.4.dev2417/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.711604 monai_weekly-1.4.dev2417/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27339 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/nets/voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49645 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.715604 monai_weekly-1.4.dev2417/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.715604 monai_weekly-1.4.dev2417/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.715604 monai_weekly-1.4.dev2417/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/regularization/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/regularization/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.719604 monai_weekly-1.4.dev2417/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/signal/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/signal/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.723604 monai_weekly-1.4.dev2417/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.723604 monai_weekly-1.4.dev2417/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.723604 monai_weekly-1.4.dev2417/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91658 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.727604 monai_weekly-1.4.dev2417/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/tf32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.727604 monai_weekly-1.4.dev2417/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.855603 monai_weekly-1.4.dev2417/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35592 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 02:16:31.000000 monai_weekly-1.4.dev2417/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-28 02:16:31.863603 monai_weekly-1.4.dev2417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:31.855603 monai_weekly-1.4.dev2417/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_push_to_hf_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cldice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_clip_intensity_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_clip_intensity_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_fid_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_mmd_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_multiscalessim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_diffusion_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_distance_transform_edt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_freeze_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gdsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_perceptual_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_simulate_low_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_simulate_low_resolutiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_fillemptyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_soft_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_squeeze_unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_ultrasound_confidence_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-04-28 02:15:02.000000 monai_weekly-1.4.dev2417/versioneer.py
```

### Comparing `monai_weekly-1.4.dev2416/LICENSE` & `monai_weekly-1.4.dev2417/LICENSE`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/PKG-INFO` & `monai_weekly-1.4.dev2417/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2416
+Version: 1.4.dev2417
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai_weekly-1.4.dev2416/README.md` & `monai_weekly-1.4.dev2417/README.md`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/__init__.py` & `monai_weekly-1.4.dev2417/monai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,8 +89,8 @@
     if hasattr(torch.cuda.device_count, "cache_clear"):
         torch.cuda.device_count.cache_clear()
 except BaseException:
     from .utils.misc import MONAIEnvVars
 
     if MONAIEnvVars.debug():
         raise
-__commit_id__ = "03a5fa695ad02fcb916d5495e84f8f01883806e2"
+__commit_id__ = "6a130cc7f659efe66cf651369e35d4a93b2ec28a"
```

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/__init__.py` & `monai_weekly-1.4.dev2417/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm.cpp` & `monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm.h` & `monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cpu.cpp` & `monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cuda.cu` & `monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai_weekly-1.4.dev2417/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/_extensions/loader.py` & `monai_weekly-1.4.dev2417/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/__main__.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/auto_runner.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/auto_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/bundle_gen.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/bundle_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/data_analyzer.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/ensemble_builder.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/hpo_gen.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/transforms.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/auto3dseg/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/datasets.py` & `monai_weekly-1.4.dev2417/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepedit/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepedit/interaction.py` & `monai_weekly-1.4.dev2417/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepedit/transforms.py` & `monai_weekly-1.4.dev2417/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepgrow/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepgrow/dataset.py` & `monai_weekly-1.4.dev2417/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepgrow/interaction.py` & `monai_weekly-1.4.dev2417/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/deepgrow/transforms.py` & `monai_weekly-1.4.dev2417/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/metrics/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/metrics/coco.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/metrics/matching.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/networks/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/networks/retinanet_detector.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/networks/retinanet_network.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/transforms/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/transforms/array.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/transforms/box_ops.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/transforms/dictionary.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/ATSS_matcher.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/anchor_utils.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/box_coder.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/box_selector.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/detector_utils.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/hard_negative_sampler.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/detection/utils/predict_utils.py` & `monai_weekly-1.4.dev2417/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/mmars/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/mmars/mmars.py` & `monai_weekly-1.4.dev2417/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/mmars/model_desc.py` & `monai_weekly-1.4.dev2417/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nnunet/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nnunet/__main__.py` & `monai_weekly-1.4.dev2417/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nnunet/nnunetv2_runner.py` & `monai_weekly-1.4.dev2417/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nnunet/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nuclick/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/nuclick/transforms.py` & `monai_weekly-1.4.dev2417/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/engines/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/engines/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/handlers/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/handlers/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/inferers/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/inferers/inferer.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/losses/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/losses/hovernet_loss.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/metrics/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/metrics/lesion_froc.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/array.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/array.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/transforms/stain/dictionary.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/pathology/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/complex_utils.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/fastmri_reader.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/mri_utils.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/networks/nets/varnet.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/array.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/reconstruction/transforms/dictionary.py` & `monai_weekly-1.4.dev2417/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/tcia/__init__.py` & `monai_weekly-1.4.dev2417/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/tcia/label_desc.py` & `monai_weekly-1.4.dev2417/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/tcia/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/apps/utils.py` & `monai_weekly-1.4.dev2417/monai/apps/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,20 @@
             See also: :py:data:`monai.apps.utils.SUPPORTED_HASH_TYPES`.
 
     """
     if val is None:
         logger.info(f"Expected {hash_type} is None, skip {hash_type} check for file {filepath}.")
         return True
     actual_hash_func = look_up_option(hash_type.lower(), SUPPORTED_HASH_TYPES)
-    actual_hash = actual_hash_func()
+
+    if sys.version_info >= (3, 9):
+        actual_hash = actual_hash_func(usedforsecurity=False)  # allows checks on FIPS enabled machines
+    else:
+        actual_hash = actual_hash_func()
+
     try:
         with open(filepath, "rb") as f:
             for chunk in iter(lambda: f.read(1024 * 1024), b""):
                 actual_hash.update(chunk)
     except Exception as e:
         logger.error(f"Exception in check_hash: {e}")
         return False
```

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/algo_gen.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/analyzer.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/operations.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/seg_summarizer.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/auto3dseg/utils.py` & `monai_weekly-1.4.dev2417/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/__init__.py` & `monai_weekly-1.4.dev2417/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/__main__.py` & `monai_weekly-1.4.dev2417/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/config_item.py` & `monai_weekly-1.4.dev2417/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/config_parser.py` & `monai_weekly-1.4.dev2417/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/properties.py` & `monai_weekly-1.4.dev2417/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/reference_resolver.py` & `monai_weekly-1.4.dev2417/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/scripts.py` & `monai_weekly-1.4.dev2417/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/utils.py` & `monai_weekly-1.4.dev2417/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/bundle/workflows.py` & `monai_weekly-1.4.dev2417/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/config/__init__.py` & `monai_weekly-1.4.dev2417/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/config/deviceconfig.py` & `monai_weekly-1.4.dev2417/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/config/type_definitions.py` & `monai_weekly-1.4.dev2417/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/__init__.py` & `monai_weekly-1.4.dev2417/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/box_utils.py` & `monai_weekly-1.4.dev2417/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/csv_saver.py` & `monai_weekly-1.4.dev2417/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/dataloader.py` & `monai_weekly-1.4.dev2417/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/dataset.py` & `monai_weekly-1.4.dev2417/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/dataset_summary.py` & `monai_weekly-1.4.dev2417/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/decathlon_datalist.py` & `monai_weekly-1.4.dev2417/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/fft_utils.py` & `monai_weekly-1.4.dev2417/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/folder_layout.py` & `monai_weekly-1.4.dev2417/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/grid_dataset.py` & `monai_weekly-1.4.dev2417/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/image_dataset.py` & `monai_weekly-1.4.dev2417/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/image_reader.py` & `monai_weekly-1.4.dev2417/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/image_writer.py` & `monai_weekly-1.4.dev2417/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/iterable_dataset.py` & `monai_weekly-1.4.dev2417/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/itk_torch_bridge.py` & `monai_weekly-1.4.dev2417/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/meta_obj.py` & `monai_weekly-1.4.dev2417/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/meta_tensor.py` & `monai_weekly-1.4.dev2417/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/samplers.py` & `monai_weekly-1.4.dev2417/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/synthetic.py` & `monai_weekly-1.4.dev2417/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/test_time_augmentation.py` & `monai_weekly-1.4.dev2417/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/thread_buffer.py` & `monai_weekly-1.4.dev2417/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/torchscript_utils.py` & `monai_weekly-1.4.dev2417/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/ultrasound_confidence_map.py` & `monai_weekly-1.4.dev2417/monai/data/ultrasound_confidence_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/utils.py` & `monai_weekly-1.4.dev2417/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/video_dataset.py` & `monai_weekly-1.4.dev2417/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/wsi_datasets.py` & `monai_weekly-1.4.dev2417/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/data/wsi_reader.py` & `monai_weekly-1.4.dev2417/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/engines/__init__.py` & `monai_weekly-1.4.dev2417/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/engines/evaluator.py` & `monai_weekly-1.4.dev2417/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/engines/trainer.py` & `monai_weekly-1.4.dev2417/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/engines/utils.py` & `monai_weekly-1.4.dev2417/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/engines/workflow.py` & `monai_weekly-1.4.dev2417/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/__init__.py` & `monai_weekly-1.4.dev2417/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/client/__init__.py` & `monai_weekly-1.4.dev2417/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/client/client_algo.py` & `monai_weekly-1.4.dev2417/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/client/monai_algo.py` & `monai_weekly-1.4.dev2417/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/utils/__init__.py` & `monai_weekly-1.4.dev2417/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/utils/constants.py` & `monai_weekly-1.4.dev2417/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/utils/exchange_object.py` & `monai_weekly-1.4.dev2417/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/fl/utils/filters.py` & `monai_weekly-1.4.dev2417/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/__init__.py` & `monai_weekly-1.4.dev2417/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/checkpoint_loader.py` & `monai_weekly-1.4.dev2417/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/checkpoint_saver.py` & `monai_weekly-1.4.dev2417/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/classification_saver.py` & `monai_weekly-1.4.dev2417/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/clearml_handlers.py` & `monai_weekly-1.4.dev2417/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/confusion_matrix.py` & `monai_weekly-1.4.dev2417/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/decollate_batch.py` & `monai_weekly-1.4.dev2417/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/earlystop_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/garbage_collector.py` & `monai_weekly-1.4.dev2417/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/hausdorff_distance.py` & `monai_weekly-1.4.dev2417/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/ignite_metric.py` & `monai_weekly-1.4.dev2417/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/logfile_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/lr_schedule_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/mean_dice.py` & `monai_weekly-1.4.dev2417/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/mean_iou.py` & `monai_weekly-1.4.dev2417/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/metric_logger.py` & `monai_weekly-1.4.dev2417/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/metrics_reloaded_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/metrics_saver.py` & `monai_weekly-1.4.dev2417/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/mlflow_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/nvtx_handlers.py` & `monai_weekly-1.4.dev2417/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/panoptic_quality.py` & `monai_weekly-1.4.dev2417/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/parameter_scheduler.py` & `monai_weekly-1.4.dev2417/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/postprocessing.py` & `monai_weekly-1.4.dev2417/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/probability_maps.py` & `monai_weekly-1.4.dev2417/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/regression_metrics.py` & `monai_weekly-1.4.dev2417/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/roc_auc.py` & `monai_weekly-1.4.dev2417/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/smartcache_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/stats_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/surface_distance.py` & `monai_weekly-1.4.dev2417/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/tensorboard_handlers.py` & `monai_weekly-1.4.dev2417/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/utils.py` & `monai_weekly-1.4.dev2417/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/handlers/validation_handler.py` & `monai_weekly-1.4.dev2417/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/inferers/__init__.py` & `monai_weekly-1.4.dev2417/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/inferers/inferer.py` & `monai_weekly-1.4.dev2417/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/inferers/merger.py` & `monai_weekly-1.4.dev2417/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/inferers/splitter.py` & `monai_weekly-1.4.dev2417/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/inferers/utils.py` & `monai_weekly-1.4.dev2417/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/__init__.py` & `monai_weekly-1.4.dev2417/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/adversarial_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/barlow_twins.py` & `monai_weekly-1.4.dev2417/monai/losses/barlow_twins.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/cldice.py` & `monai_weekly-1.4.dev2417/monai/losses/cldice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/contrastive.py` & `monai_weekly-1.4.dev2417/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/deform.py` & `monai_weekly-1.4.dev2417/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/dice.py` & `monai_weekly-1.4.dev2417/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/ds_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/focal_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/giou_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/hausdorff_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/hausdorff_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/image_dissimilarity.py` & `monai_weekly-1.4.dev2417/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/multi_scale.py` & `monai_weekly-1.4.dev2417/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/perceptual.py` & `monai_weekly-1.4.dev2417/monai/losses/perceptual.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
                 pretrained_path=pretrained_path,
                 pretrained_state_dict_key=pretrained_state_dict_key,
             )
         else:
             self.perceptual_function = LPIPS(pretrained=pretrained, net=network_type, verbose=False)
         self.is_fake_3d = is_fake_3d
         self.fake_3d_ratio = fake_3d_ratio
+        self.channel_wise = channel_wise
 
     def _calculate_axis_loss(self, input: torch.Tensor, target: torch.Tensor, spatial_axis: int) -> torch.Tensor:
         """
         Calculate perceptual loss in one of the axis used in the 2.5D approach. After the slices of one spatial axis
         is transformed into different instances in the batch, we compute the loss using the 2D approach.
 
         Args:
```

### Comparing `monai_weekly-1.4.dev2416/monai/losses/spatial_mask.py` & `monai_weekly-1.4.dev2417/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/spectral_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/ssim_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/sure_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/tversky.py` & `monai_weekly-1.4.dev2417/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/losses/unified_focal_loss.py` & `monai_weekly-1.4.dev2417/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/__init__.py` & `monai_weekly-1.4.dev2417/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/active_learning_metrics.py` & `monai_weekly-1.4.dev2417/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/confusion_matrix.py` & `monai_weekly-1.4.dev2417/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/cumulative_average.py` & `monai_weekly-1.4.dev2417/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/f_beta_score.py` & `monai_weekly-1.4.dev2417/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/fid.py` & `monai_weekly-1.4.dev2417/monai/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/froc.py` & `monai_weekly-1.4.dev2417/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/generalized_dice.py` & `monai_weekly-1.4.dev2417/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/hausdorff_distance.py` & `monai_weekly-1.4.dev2417/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/loss_metric.py` & `monai_weekly-1.4.dev2417/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/meandice.py` & `monai_weekly-1.4.dev2417/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/meaniou.py` & `monai_weekly-1.4.dev2417/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/metric.py` & `monai_weekly-1.4.dev2417/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/mmd.py` & `monai_weekly-1.4.dev2417/monai/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/panoptic_quality.py` & `monai_weekly-1.4.dev2417/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/regression.py` & `monai_weekly-1.4.dev2417/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/rocauc.py` & `monai_weekly-1.4.dev2417/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/surface_dice.py` & `monai_weekly-1.4.dev2417/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/surface_distance.py` & `monai_weekly-1.4.dev2417/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/utils.py` & `monai_weekly-1.4.dev2417/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/metrics/wrapper.py` & `monai_weekly-1.4.dev2417/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/__init__.py` & `monai_weekly-1.4.dev2417/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/acti_norm.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/activation.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/aspp.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/backbone_fpn_utils.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/convolutions.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/crf.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/denseblock.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/dints_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/downsample.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/dynunet_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/encoder.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/fcn.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/feature_pyramid_network.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/fft_utils_t.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/localnet_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/mlp.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/patchembedding.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/pos_embed_utils.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/pos_embed_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/regunet_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/segresnet_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/selfattention.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/squeeze_and_excitation.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/text_embedding.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/transformerblock.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/unetr_block.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/upsample.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/blocks/warp.py` & `monai_weekly-1.4.dev2417/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/__init__.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/conjugate_gradient.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/convutils.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/drop_path.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/factories.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/filtering.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/gmm.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/simplelayers.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/spatial_transforms.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/utils.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/layers/weight_init.py` & `monai_weekly-1.4.dev2417/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/__init__.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 from .quicknat import Quicknat
 from .regressor import Regressor
 from .regunet import GlobalNet, LocalNet, RegUNet
 from .resnet import (
     ResNet,
     ResNetBlock,
     ResNetBottleneck,
+    ResNetEncoder,
+    ResNetFeatures,
     get_medicalnet_pretrained_resnet_args,
     get_pretrained_resnet_medicalnet,
     resnet10,
     resnet18,
     resnet34,
     resnet50,
     resnet101,
```

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/ahnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/attentionunet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/autoencoder.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/basic_unet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/basic_unetplusplus.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/classifier.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/daf3d.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/densenet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/dints.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/dynunet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/efficientnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/flexible_unet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/flexible_unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from torch import nn
 
 from monai.networks.blocks import BaseEncoder, UpSample
 from monai.networks.layers.factories import Conv
 from monai.networks.layers.utils import get_act_layer
 from monai.networks.nets import EfficientNetEncoder
 from monai.networks.nets.basic_unet import UpCat
+from monai.networks.nets.resnet import ResNetEncoder
 from monai.utils import InterpolateMode, optional_import
 
 __all__ = ["FlexibleUNet", "FlexUNet", "FLEXUNET_BACKBONE", "FlexUNetEncoderRegister"]
 
 
 class FlexUNetEncoderRegister:
     """
@@ -74,14 +75,15 @@
                 "parameter": parameter_list[cnt],
             }
             self.register_dict[name_string] = cur_dict
 
 
 FLEXUNET_BACKBONE = FlexUNetEncoderRegister()
 FLEXUNET_BACKBONE.register_class(EfficientNetEncoder)
+FLEXUNET_BACKBONE.register_class(ResNetEncoder)
 
 
 class UNetDecoder(nn.Module):
     """
     UNet Decoder.
     This class refers to `segmentation_models.pytorch
     <https://github.com/qubvel/segmentation_models.pytorch>`_.
@@ -234,28 +236,29 @@
         upsample: str = "nontrainable",
         pre_conv: str = "default",
         interp_mode: str = "nearest",
         is_pad: bool = True,
     ) -> None:
         """
         A flexible implement of UNet, in which the backbone/encoder can be replaced with
-        any efficient network. Currently the input must have a 2 or 3 spatial dimension
+        any efficient or residual network. Currently the input must have a 2 or 3 spatial dimension
         and the spatial size of each dimension must be a multiple of 32 if is_pad parameter
         is False.
         Please notice each output of backbone must be 2x downsample in spatial dimension
         of last output. For example, if given a 512x256 2D image and a backbone with 4 outputs.
         Spatial size of each encoder output should be 256x128, 128x64, 64x32 and 32x16.
 
         Args:
             in_channels: number of input channels.
             out_channels: number of output channels.
-            backbone: name of backbones to initialize, only support efficientnet right now,
-                can be from [efficientnet-b0,..., efficientnet-b8, efficientnet-l2].
-            pretrained: whether to initialize pretrained ImageNet weights, only available
-                for spatial_dims=2 and batch norm is used, default to False.
+            backbone: name of backbones to initialize, only support efficientnet and resnet right now,
+                can be from [efficientnet-b0, ..., efficientnet-b8, efficientnet-l2, resnet10, ..., resnet200].
+            pretrained: whether to initialize pretrained weights. ImageNet weights are available for efficient networks
+                if spatial_dims=2 and batch norm is used. MedicalNet weights are available for residual networks
+                if spatial_dims=3 and in_channels=1. Default to False.
             decoder_channels: number of output channels for all feature maps in decoder.
                 `len(decoder_channels)` should equal to `len(encoder_channels) - 1`,default
                 to (256, 128, 64, 32, 16).
             spatial_dims: number of spatial dimensions, default to 2.
             norm: normalization type and arguments, default to ("batch", {"eps": 1e-3,
                 "momentum": 0.1}).
             act: activation type and arguments, default to ("relu", {"inplace": True}).
```

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/fullyconnectednet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/generator.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/highresnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/hovernet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/milmodel.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/netadapter.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/quicknat.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/regressor.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/regunet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/resnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/resnet.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from functools import partial
 from pathlib import Path
 from typing import Any
 
 import torch
 import torch.nn as nn
 
+from monai.networks.blocks.encoder import BaseEncoder
 from monai.networks.layers.factories import Conv, Norm, Pool
 from monai.networks.layers.utils import get_pool_layer
 from monai.utils import ensure_tuple_rep
 from monai.utils.module import look_up_option, optional_import
 
 hf_hub_download, _ = optional_import("huggingface_hub", name="hf_hub_download")
 EntryNotFoundError, _ = optional_import("huggingface_hub.utils._errors", name="EntryNotFoundError")
@@ -41,14 +42,27 @@
     "resnet34",
     "resnet50",
     "resnet101",
     "resnet152",
     "resnet200",
 ]
 
+
+resnet_params = {
+    # model_name: (block, layers, shortcut_type, bias_downsample, datasets23)
+    "resnet10": ("basic", [1, 1, 1, 1], "B", False, True),
+    "resnet18": ("basic", [2, 2, 2, 2], "A", True, True),
+    "resnet34": ("basic", [3, 4, 6, 3], "A", True, True),
+    "resnet50": ("bottleneck", [3, 4, 6, 3], "B", False, True),
+    "resnet101": ("bottleneck", [3, 4, 23, 3], "B", False, False),
+    "resnet152": ("bottleneck", [3, 8, 36, 3], "B", False, False),
+    "resnet200": ("bottleneck", [3, 24, 36, 3], "B", False, False),
+}
+
+
 logger = logging.getLogger(__name__)
 
 
 def get_inplanes():
     return [64, 128, 256, 512]
 
 
@@ -331,14 +345,128 @@
         x = x.view(x.size(0), -1)
         if self.fc is not None:
             x = self.fc(x)
 
         return x
 
 
+class ResNetFeatures(ResNet):
+
+    def __init__(self, model_name: str, pretrained: bool = True, spatial_dims: int = 3, in_channels: int = 1) -> None:
+        """Initialize resnet18 to resnet200 models as a backbone, the backbone can be used as an encoder for
+        segmentation and objection models.
+
+        Compared with the class `ResNet`, the only different place is the forward function.
+
+        Args:
+            model_name: name of model to initialize, can be from [resnet10, ..., resnet200].
+            pretrained: whether to initialize pretrained MedicalNet weights,
+                only available for spatial_dims=3 and in_channels=1.
+            spatial_dims: number of spatial dimensions of the input image.
+            in_channels: number of input channels for first convolutional layer.
+        """
+        if model_name not in resnet_params:
+            model_name_string = ", ".join(resnet_params.keys())
+            raise ValueError(f"invalid model_name {model_name} found, must be one of {model_name_string} ")
+
+        block, layers, shortcut_type, bias_downsample, datasets23 = resnet_params[model_name]
+
+        super().__init__(
+            block=block,
+            layers=layers,
+            block_inplanes=get_inplanes(),
+            spatial_dims=spatial_dims,
+            n_input_channels=in_channels,
+            conv1_t_stride=2,
+            shortcut_type=shortcut_type,
+            feed_forward=False,
+            bias_downsample=bias_downsample,
+        )
+        if pretrained:
+            if spatial_dims == 3 and in_channels == 1:
+                _load_state_dict(self, model_name, datasets23=datasets23)
+            else:
+                raise ValueError("Pretrained resnet models are only available for in_channels=1 and spatial_dims=3.")
+
+    def forward(self, inputs: torch.Tensor):
+        """
+        Args:
+            inputs: input should have spatially N dimensions
+            ``(Batch, in_channels, dim_0[, dim_1, ..., dim_N])``, N is defined by `dimensions`.
+
+        Returns:
+            a list of torch Tensors.
+        """
+        x = self.conv1(inputs)
+        x = self.bn1(x)
+        x = self.relu(x)
+
+        features = []
+        features.append(x)
+
+        if not self.no_max_pool:
+            x = self.maxpool(x)
+
+        x = self.layer1(x)
+        features.append(x)
+
+        x = self.layer2(x)
+        features.append(x)
+
+        x = self.layer3(x)
+        features.append(x)
+
+        x = self.layer4(x)
+        features.append(x)
+
+        return features
+
+
+class ResNetEncoder(ResNetFeatures, BaseEncoder):
+    """Wrap the original resnet to an encoder for flexible-unet."""
+
+    backbone_names = ["resnet10", "resnet18", "resnet34", "resnet50", "resnet101", "resnet152", "resnet200"]
+
+    @classmethod
+    def get_encoder_parameters(cls) -> list[dict]:
+        """Get the initialization parameter for resnet backbones."""
+        parameter_list = []
+        for backbone_name in cls.backbone_names:
+            parameter_list.append(
+                {"model_name": backbone_name, "pretrained": True, "spatial_dims": 3, "in_channels": 1}
+            )
+        return parameter_list
+
+    @classmethod
+    def num_channels_per_output(cls) -> list[tuple[int, ...]]:
+        """Get number of resnet backbone output feature maps channel."""
+        return [
+            (64, 64, 128, 256, 512),
+            (64, 64, 128, 256, 512),
+            (64, 64, 128, 256, 512),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+        ]
+
+    @classmethod
+    def num_outputs(cls) -> list[int]:
+        """Get number of resnet backbone output feature maps.
+
+        Since every backbone contains the same 5 output feature maps, the number list should be `[5] * 7`.
+        """
+        return [5] * 7
+
+    @classmethod
+    def get_encoder_names(cls) -> list[str]:
+        """Get names of resnet backbones."""
+        return cls.backbone_names
+
+
 def _resnet(
     arch: str,
     block: type[ResNetBlock | ResNetBottleneck],
     layers: list[int],
     block_inplanes: list[int],
     pretrained: bool | str,
     progress: bool,
@@ -473,15 +601,15 @@
         progress (bool): If True, displays a progress bar of the download to stderr
     """
     return _resnet("resnet200", ResNetBottleneck, [3, 24, 36, 3], get_inplanes(), pretrained, progress, **kwargs)
 
 
 def get_pretrained_resnet_medicalnet(resnet_depth: int, device: str = "cpu", datasets23: bool = True):
     """
-    Donwlad resnet pretrained weights from https://huggingface.co/TencentMedicalNet
+    Download resnet pretrained weights from https://huggingface.co/TencentMedicalNet
 
     Args:
         resnet_depth: depth of the pretrained model. Supported values are 10, 18, 34, 50, 101, 152 and 200
         device: device on which the returned state dict will be loaded. "cpu" or "cuda" for example.
         datasets23: if True, get the weights trained on more datasets (23).
                     Not all depths are available. If not, standard weights are returned.
 
@@ -529,15 +657,28 @@
     logger.info(f"{filename} downloaded")
     return checkpoint.get("state_dict")
 
 
 def get_medicalnet_pretrained_resnet_args(resnet_depth: int):
     """
     Return correct shortcut_type and bias_downsample
-    for pretrained MedicalNet weights according to resnet depth
+    for pretrained MedicalNet weights according to resnet depth.
     """
     # After testing
     # False: 10, 50, 101, 152, 200
     # Any: 18, 34
     bias_downsample = -1 if resnet_depth in [18, 34] else 0  # 18, 10, 34
     shortcut_type = "A" if resnet_depth in [18, 34] else "B"
     return bias_downsample, shortcut_type
+
+
+def _load_state_dict(model: nn.Module, model_name: str, datasets23: bool = True) -> None:
+    search_res = re.search(r"resnet(\d+)", model_name)
+    if search_res:
+        resnet_depth = int(search_res.group(1))
+        datasets23 = model_name.endswith("_23datasets")
+    else:
+        raise ValueError("model_name argument should contain resnet depth. Example: resnet18 or resnet18_23datasets.")
+
+    model_state_dict = get_pretrained_resnet_medicalnet(resnet_depth, device="cpu", datasets23=datasets23)
+    model_state_dict = {key.replace("module.", ""): value for key, value in model_state_dict.items()}
+    model.load_state_dict(model_state_dict)
```

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/segresnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/segresnet_ds.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/senet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/swin_unetr.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/torchvision_fc.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/transchex.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/unet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/unetr.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/varautoencoder.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/vit.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/vitautoenc.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/vnet.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/nets/voxelmorph.py` & `monai_weekly-1.4.dev2417/monai/networks/nets/voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/networks/utils.py` & `monai_weekly-1.4.dev2417/monai/networks/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,14 +982,15 @@
                     )
                 ]
                 trt_model = torch_tensorrt.compile(
                     ir_model,
                     inputs=input_placeholder,
                     enabled_precisions=convert_precision,
                     device=target_device,
+                    ir="torchscript",
                     **kwargs,
                 )
 
     # verify the outputs between the TensorRT model and PyTorch model
     if verify:
         if inputs is None:
             raise ValueError("Missing input data for verification.")
```

### Comparing `monai_weekly-1.4.dev2416/monai/optimizers/__init__.py` & `monai_weekly-1.4.dev2417/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/optimizers/lr_finder.py` & `monai_weekly-1.4.dev2417/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/optimizers/lr_scheduler.py` & `monai_weekly-1.4.dev2417/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/optimizers/novograd.py` & `monai_weekly-1.4.dev2417/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/optimizers/utils.py` & `monai_weekly-1.4.dev2417/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/adaptors.py` & `monai_weekly-1.4.dev2417/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/compose.py` & `monai_weekly-1.4.dev2417/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/croppad/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/croppad/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/croppad/batch.py` & `monai_weekly-1.4.dev2417/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/croppad/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/croppad/functional.py` & `monai_weekly-1.4.dev2417/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/intensity/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/intensity/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/intensity/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/inverse.py` & `monai_weekly-1.4.dev2417/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/inverse_batch_transform.py` & `monai_weekly-1.4.dev2417/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/io/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/io/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/io/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/lazy/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/lazy/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/lazy/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/lazy/functional.py` & `monai_weekly-1.4.dev2417/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/lazy/utils.py` & `monai_weekly-1.4.dev2417/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/meta_utility/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/meta_utility/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/nvtx.py` & `monai_weekly-1.4.dev2417/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/post/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/post/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/regularization/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/regularization/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/regularization/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/regularization/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/regularization/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/signal/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/signal/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/signal/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/signal/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/smooth_field/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/smooth_field/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/smooth_field/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/spatial/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/spatial/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/spatial/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/spatial/functional.py` & `monai_weekly-1.4.dev2417/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/traits.py` & `monai_weekly-1.4.dev2417/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/transform.py` & `monai_weekly-1.4.dev2417/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utility/__init__.py` & `monai_weekly-1.4.dev2417/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utility/array.py` & `monai_weekly-1.4.dev2417/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utility/dictionary.py` & `monai_weekly-1.4.dev2417/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utils.py` & `monai_weekly-1.4.dev2417/monai/transforms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2186,15 +2186,15 @@
     distances_original, indices_original = distances, indices
     distances, indices = None, None
     if use_cp:
         distances_, indices_ = None, None
         if return_distances:
             dtype = torch.float64 if float64_distances else torch.float32
             if distances is None:
-                distances = torch.zeros_like(img, dtype=dtype)  # type: ignore
+                distances = torch.zeros_like(img, memory_format=torch.contiguous_format, dtype=dtype)  # type: ignore
             else:
                 if not isinstance(distances, torch.Tensor) and distances.device != img.device:
                     raise TypeError("distances must be a torch.Tensor on the same device as img")
                 if not distances.dtype == dtype:
                     raise TypeError("distances must be a torch.Tensor of dtype float32 or float64")
             distances_ = convert_to_cupy(distances)
         if return_indices:
```

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utils_create_transform_ims.py` & `monai_weekly-1.4.dev2417/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/transforms/utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2417/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/__init__.py` & `monai_weekly-1.4.dev2417/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/aliases.py` & `monai_weekly-1.4.dev2417/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/component_store.py` & `monai_weekly-1.4.dev2417/monai/utils/component_store.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/decorators.py` & `monai_weekly-1.4.dev2417/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/deprecate_utils.py` & `monai_weekly-1.4.dev2417/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/dist.py` & `monai_weekly-1.4.dev2417/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/enums.py` & `monai_weekly-1.4.dev2417/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/jupyter_utils.py` & `monai_weekly-1.4.dev2417/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/misc.py` & `monai_weekly-1.4.dev2417/monai/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,15 @@
 
     @staticmethod
     def doc_images() -> str | None:
         return os.environ.get("MONAI_DOC_IMAGES")
 
     @staticmethod
     def algo_hash() -> str | None:
-        return os.environ.get("MONAI_ALGO_HASH", "def5f26")
+        return os.environ.get("MONAI_ALGO_HASH", "07acb39")
 
     @staticmethod
     def trace_transform() -> str | None:
         return os.environ.get("MONAI_TRACE_TRANSFORM", "1")
 
     @staticmethod
     def eval_expr() -> str | None:
```

### Comparing `monai_weekly-1.4.dev2416/monai/utils/module.py` & `monai_weekly-1.4.dev2417/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/nvtx.py` & `monai_weekly-1.4.dev2417/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/profiling.py` & `monai_weekly-1.4.dev2417/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/state_cacher.py` & `monai_weekly-1.4.dev2417/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/tf32.py` & `monai_weekly-1.4.dev2417/monai/utils/tf32.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/utils/type_conversion.py` & `monai_weekly-1.4.dev2417/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/__init__.py` & `monai_weekly-1.4.dev2417/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/class_activation_maps.py` & `monai_weekly-1.4.dev2417/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/gradient_based.py` & `monai_weekly-1.4.dev2417/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/img2tensorboard.py` & `monai_weekly-1.4.dev2417/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/occlusion_sensitivity.py` & `monai_weekly-1.4.dev2417/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/utils.py` & `monai_weekly-1.4.dev2417/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai/visualize/visualizer.py` & `monai_weekly-1.4.dev2417/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai_weekly.egg-info/PKG-INFO` & `monai_weekly-1.4.dev2417/monai_weekly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2416
+Version: 1.4.dev2417
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai_weekly-1.4.dev2416/monai_weekly.egg-info/SOURCES.txt` & `monai_weekly-1.4.dev2417/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/monai_weekly.egg-info/requires.txt` & `monai_weekly-1.4.dev2417/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/pyproject.toml` & `monai_weekly-1.4.dev2417/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/setup.cfg` & `monai_weekly-1.4.dev2417/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/setup.py` & `monai_weekly-1.4.dev2417/setup.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_acn_block.py` & `monai_weekly-1.4.dev2417/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_activations.py` & `monai_weekly-1.4.dev2417/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_activationsd.py` & `monai_weekly-1.4.dev2417/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_adaptors.py` & `monai_weekly-1.4.dev2417/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_add_coordinate_channels.py` & `monai_weekly-1.4.dev2417/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_add_coordinate_channelsd.py` & `monai_weekly-1.4.dev2417/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_add_extreme_points_channel.py` & `monai_weekly-1.4.dev2417/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_add_extreme_points_channeld.py` & `monai_weekly-1.4.dev2417/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_adjust_contrast.py` & `monai_weekly-1.4.dev2417/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_adjust_contrastd.py` & `monai_weekly-1.4.dev2417/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_adn.py` & `monai_weekly-1.4.dev2417/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_adversarial_loss.py` & `monai_weekly-1.4.dev2417/tests/test_adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_affine.py` & `monai_weekly-1.4.dev2417/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_affine_grid.py` & `monai_weekly-1.4.dev2417/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_affine_transform.py` & `monai_weekly-1.4.dev2417/tests/test_affine_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,36 +129,25 @@
         with self.assertRaises(ValueError):
             affine = torch.as_tensor(affine, device=torch.device("cpu:0"), dtype=torch.float32)
             to_norm_affine(affine, src_size, dst_size, align_corners)
 
 
 class TestAffineTransform(unittest.TestCase):
 
-    def test_affine_shift(self):
-        affine = torch.as_tensor([[1.0, 0.0, 0.0], [0.0, 1.0, -1.0]])
+    @parameterized.expand(
+        [
+            (torch.as_tensor([[1.0, 0.0, 0.0], [0.0, 1.0, -1.0]]), [[[[0, 4, 1, 3], [0, 7, 6, 8], [0, 3, 5, 3]]]]),
+            (torch.as_tensor([[1.0, 0.0, -1.0], [0.0, 1.0, -1.0]]), [[[[0, 0, 0, 0], [0, 4, 1, 3], [0, 7, 6, 8]]]]),
+            (torch.as_tensor([[1.0, 0.0, -1.0], [0.0, 1.0, 0.0]]), [[[[0, 0, 0, 0], [4, 1, 3, 2], [7, 6, 8, 5]]]]),
+        ]
+    )
+    def test_affine_transforms(self, affine, expected):
         image = torch.as_tensor([[[[4.0, 1.0, 3.0, 2.0], [7.0, 6.0, 8.0, 5.0], [3.0, 5.0, 3.0, 6.0]]]])
         out = AffineTransform(align_corners=False)(image, affine)
         out = out.detach().cpu().numpy()
-        expected = [[[[0, 4, 1, 3], [0, 7, 6, 8], [0, 3, 5, 3]]]]
-        np.testing.assert_allclose(out, expected, atol=1e-5, rtol=_rtol)
-
-    def test_affine_shift_1(self):
-        affine = torch.as_tensor([[1.0, 0.0, -1.0], [0.0, 1.0, -1.0]])
-        image = torch.as_tensor([[[[4.0, 1.0, 3.0, 2.0], [7.0, 6.0, 8.0, 5.0], [3.0, 5.0, 3.0, 6.0]]]])
-        out = AffineTransform(align_corners=False)(image, affine)
-        out = out.detach().cpu().numpy()
-        expected = [[[[0, 0, 0, 0], [0, 4, 1, 3], [0, 7, 6, 8]]]]
-        np.testing.assert_allclose(out, expected, atol=1e-5, rtol=_rtol)
-
-    def test_affine_shift_2(self):
-        affine = torch.as_tensor([[1.0, 0.0, -1.0], [0.0, 1.0, 0.0]])
-        image = torch.as_tensor([[[[4.0, 1.0, 3.0, 2.0], [7.0, 6.0, 8.0, 5.0], [3.0, 5.0, 3.0, 6.0]]]])
-        out = AffineTransform(align_corners=False)(image, affine)
-        out = out.detach().cpu().numpy()
-        expected = [[[[0, 0, 0, 0], [4, 1, 3, 2], [7, 6, 8, 5]]]]
         np.testing.assert_allclose(out, expected, atol=1e-5, rtol=_rtol)
 
     def test_zoom(self):
         affine = torch.as_tensor([[1.0, 0.0, 0.0], [0.0, 2.0, 0.0]])
         image = torch.arange(1.0, 13.0).view(1, 1, 3, 4).to(device=torch.device("cpu:0"))
         out = AffineTransform((3, 2), align_corners=False)(image, affine)
         expected = [[[[1, 3], [5, 7], [9, 11]]]]
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_affined.py` & `monai_weekly-1.4.dev2417/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ahnet.py` & `monai_weekly-1.4.dev2417/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_alias.py` & `monai_weekly-1.4.dev2417/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_anchor_box.py` & `monai_weekly-1.4.dev2417/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_apply.py` & `monai_weekly-1.4.dev2417/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_apply_filter.py` & `monai_weekly-1.4.dev2417/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_arraydataset.py` & `monai_weekly-1.4.dev2417/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_as_channel_last.py` & `monai_weekly-1.4.dev2417/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_as_channel_lastd.py` & `monai_weekly-1.4.dev2417/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_as_discrete.py` & `monai_weekly-1.4.dev2417/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_as_discreted.py` & `monai_weekly-1.4.dev2417/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_atss_box_matcher.py` & `monai_weekly-1.4.dev2417/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_attentionunet.py` & `monai_weekly-1.4.dev2417/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_auto3dseg.py` & `monai_weekly-1.4.dev2417/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_auto3dseg_bundlegen.py` & `monai_weekly-1.4.dev2417/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_auto3dseg_ensemble.py` & `monai_weekly-1.4.dev2417/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_auto3dseg_hpo.py` & `monai_weekly-1.4.dev2417/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_autoencoder.py` & `monai_weekly-1.4.dev2417/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_avg_merger.py` & `monai_weekly-1.4.dev2417/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_barlow_twins_loss.py` & `monai_weekly-1.4.dev2417/tests/test_barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_basic_unet.py` & `monai_weekly-1.4.dev2417/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_basic_unetplusplus.py` & `monai_weekly-1.4.dev2417/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bending_energy.py` & `monai_weekly-1.4.dev2417/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bilateral_approx_cpu.py` & `monai_weekly-1.4.dev2417/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bilateral_approx_cuda.py` & `monai_weekly-1.4.dev2417/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bilateral_precise.py` & `monai_weekly-1.4.dev2417/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_blend_images.py` & `monai_weekly-1.4.dev2417/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_border_pad.py` & `monai_weekly-1.4.dev2417/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_border_padd.py` & `monai_weekly-1.4.dev2417/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bounding_rect.py` & `monai_weekly-1.4.dev2417/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bounding_rectd.py` & `monai_weekly-1.4.dev2417/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_box_coder.py` & `monai_weekly-1.4.dev2417/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_box_transform.py` & `monai_weekly-1.4.dev2417/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_box_utils.py` & `monai_weekly-1.4.dev2417/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_ckpt_export.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_ckpt_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,17 @@
                 cmd += ["--use_trace", use_trace, "--input_shape", "[1, 1, 96, 96, 96]"]
             command_line_tests(cmd)
             self.assertTrue(os.path.exists(ts_file))
 
             _, metadata, extra_files = load_net_with_metadata(
                 ts_file, more_extra_files=["inference.json", "def_args.json"]
             )
-            self.assertTrue("schema" in metadata)
-            self.assertTrue("meta_file" in json.loads(extra_files["def_args.json"]))
-            self.assertTrue("network_def" in json.loads(extra_files["inference.json"]))
+            self.assertIn("schema", metadata)
+            self.assertIn("meta_file", json.loads(extra_files["def_args.json"]))
+            self.assertIn("network_def", json.loads(extra_files["inference.json"]))
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
     def test_default_value(self, key_in_ckpt, use_trace):
         config_file = os.path.join(os.path.dirname(__file__), "testing_data", "inference.json")
         with tempfile.TemporaryDirectory() as tempdir:
             def_args = {"meta_file": "will be replaced by `meta_file` arg"}
             def_args_file = os.path.join(tempdir, "def_args.yaml")
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_download.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_get_data.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_get_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,42 +47,43 @@
 class TestGetBundleData(unittest.TestCase):
 
     @parameterized.expand([TEST_CASE_3, TEST_CASE_4])
     @skip_if_quick
     def test_get_all_bundles_list(self, params):
         with skip_if_downloading_fails():
             output = get_all_bundles_list(**params)
-            self.assertTrue(isinstance(output, list))
-            self.assertTrue(isinstance(output[0], tuple))
+            self.assertIsInstance(output, list)
+            self.assertIsInstance(output[0], tuple)
             self.assertTrue(len(output[0]) == 2)
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_5])
     @skip_if_quick
     def test_get_bundle_versions(self, params):
         with skip_if_downloading_fails():
             output = get_bundle_versions(**params)
-            self.assertTrue(isinstance(output, dict))
-            self.assertTrue("latest_version" in output and "all_versions" in output)
-            self.assertTrue("0.1.0" in output["all_versions"])
+            self.assertIsInstance(output, dict)
+            self.assertIn("latest_version", output)
+            self.assertIn("all_versions", output)
+            self.assertIn("0.1.0", output["all_versions"])
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     @skip_if_quick
     def test_get_bundle_info(self, params):
         with skip_if_downloading_fails():
             output = get_bundle_info(**params)
-            self.assertTrue(isinstance(output, dict))
+            self.assertIsInstance(output, dict)
             for key in ["id", "name", "size", "download_count", "browser_download_url"]:
                 self.assertTrue(key in output)
 
     @parameterized.expand([TEST_CASE_5, TEST_CASE_6])
     @skip_if_quick
     def test_get_bundle_info_monaihosting(self, params):
         with skip_if_downloading_fails():
             output = get_bundle_info(**params)
-            self.assertTrue(isinstance(output, dict))
+            self.assertIsInstance(output, dict)
             for key in ["name", "browser_download_url"]:
                 self.assertTrue(key in output)
 
     @parameterized.expand([TEST_CASE_FAKE_TOKEN_1, TEST_CASE_FAKE_TOKEN_2])
     @skip_if_quick
     def test_fake_token(self, params):
         with skip_if_downloading_fails():
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_init_bundle.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_onnx_export.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_push_to_hf_hub.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_trt_export.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_trt_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,17 +87,17 @@
                 cmd += ["--dynamic_batch", str(dynamic_batch)]
             command_line_tests(cmd)
             self.assertTrue(os.path.exists(ts_file))
 
             _, metadata, extra_files = load_net_with_metadata(
                 ts_file, more_extra_files=["inference.json", "def_args.json"]
             )
-            self.assertTrue("schema" in metadata)
-            self.assertTrue("meta_file" in json.loads(extra_files["def_args.json"]))
-            self.assertTrue("network_def" in json.loads(extra_files["inference.json"]))
+            self.assertIn("schema", metadata)
+            self.assertIn("meta_file", json.loads(extra_files["def_args.json"]))
+            self.assertIn("network_def", json.loads(extra_files["inference.json"]))
 
     @parameterized.expand([TEST_CASE_3, TEST_CASE_4])
     @unittest.skipUnless(
         has_onnx and has_torchtrt and has_tensorrt, "Onnx and TensorRT are required for onnx-trt conversion!"
     )
     def test_onnx_trt_export(self, convert_precision, input_shape, dynamic_batch):
         meta_file = os.path.join(os.path.dirname(__file__), "testing_data", "metadata.json")
@@ -125,14 +125,14 @@
                 cmd += ["--dynamic_batch", str(dynamic_batch)]
             command_line_tests(cmd)
             self.assertTrue(os.path.exists(ts_file))
 
             _, metadata, extra_files = load_net_with_metadata(
                 ts_file, more_extra_files=["inference.json", "def_args.json"]
             )
-            self.assertTrue("schema" in metadata)
-            self.assertTrue("meta_file" in json.loads(extra_files["def_args.json"]))
-            self.assertTrue("network_def" in json.loads(extra_files["inference.json"]))
+            self.assertIn("schema", metadata)
+            self.assertIn("meta_file", json.loads(extra_files["def_args.json"]))
+            self.assertIn("network_def", json.loads(extra_files["inference.json"]))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_utils.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_verify_metadata.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_verify_net.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_bundle_workflow.py` & `monai_weekly-1.4.dev2417/tests/test_bundle_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,19 @@
         trainer.parser.update(
             pairs={"validate#evaluator#postprocessing": "$@validate#postprocessing if @val_interval > 0 else None"}
         )
         trainer.initialize()
         self.assertListEqual(trainer.check_properties(), [])
         # test read / write the properties
         dataset = trainer.train_dataset
-        self.assertTrue(isinstance(dataset, Dataset))
+        self.assertIsInstance(dataset, Dataset)
         inferer = trainer.train_inferer
-        self.assertTrue(isinstance(inferer, SimpleInferer))
+        self.assertIsInstance(inferer, SimpleInferer)
         # test optional properties get
-        self.assertTrue(trainer.train_key_metric is None)
+        self.assertIsNone(trainer.train_key_metric)
         trainer.train_dataset = deepcopy(dataset)
         trainer.train_inferer = deepcopy(inferer)
         # test optional properties set
         trainer.train_key_metric = "set optional properties"
 
         # should initialize and parse again as changed the bundle content
         trainer.initialize()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_cachedataset.py` & `monai_weekly-1.4.dev2417/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cachedataset_parallel.py` & `monai_weekly-1.4.dev2417/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cachedataset_persistent_workers.py` & `monai_weekly-1.4.dev2417/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cachentransdataset.py` & `monai_weekly-1.4.dev2417/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_call_dist.py` & `monai_weekly-1.4.dev2417/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cast_to_type.py` & `monai_weekly-1.4.dev2417/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cast_to_typed.py` & `monai_weekly-1.4.dev2417/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_center_scale_crop.py` & `monai_weekly-1.4.dev2417/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_center_scale_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_center_spatial_crop.py` & `monai_weekly-1.4.dev2417/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_center_spatial_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_channel_pad.py` & `monai_weekly-1.4.dev2417/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_check_hash.py` & `monai_weekly-1.4.dev2417/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_check_missing_files.py` & `monai_weekly-1.4.dev2417/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_classes_to_indices.py` & `monai_weekly-1.4.dev2417/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_classes_to_indicesd.py` & `monai_weekly-1.4.dev2417/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cldice_loss.py` & `monai_weekly-1.4.dev2417/tests/test_cldice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_clip_intensity_percentiles.py` & `monai_weekly-1.4.dev2417/tests/test_clip_intensity_percentiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,46 +14,45 @@
 
 import torch
 from parameterized import parameterized
 
 from monai.transforms import ClipIntensityPercentiles
 from monai.transforms.utils import soft_clip
 from monai.transforms.utils_pytorch_numpy_unification import clip, percentile
-from monai.utils.type_conversion import convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, NumpyImageTestCase3D, assert_allclose
 
 
 class TestClipIntensityPercentiles2D(NumpyImageTestCase2D):
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (5, 95))
-        expected = clip(convert_to_tensor(im), lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        expected = clip(im, lower, upper)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (0, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (5, 100))
         expected = clip(im, lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
         lower, upper = percentile(im, (5, 95))
@@ -85,15 +84,15 @@
     def test_channel_wise(self, p):
         clipper = ClipIntensityPercentiles(upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper(im)
         for i, c in enumerate(im):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
-            assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+            assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     def test_ill_sharpness_factor(self):
         with self.assertRaises(ValueError):
             ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=0.0)
 
     def test_ill_lower_percentile(self):
         with self.assertRaises(ValueError):
@@ -117,33 +116,33 @@
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (5, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (0, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
         lower, upper = percentile(im, (5, 100))
         expected = clip(im, lower, upper)
-        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
         lower, upper = percentile(im, (5, 95))
@@ -175,12 +174,12 @@
     def test_channel_wise(self, p):
         clipper = ClipIntensityPercentiles(upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper(im)
         for i, c in enumerate(im):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
-            assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+            assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_clip_intensity_percentilesd.py` & `monai_weekly-1.4.dev2417/tests/test_clip_intensity_percentilesd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,49 +15,48 @@
 
 import torch
 from parameterized import parameterized
 
 from monai.transforms import ClipIntensityPercentilesd
 from monai.transforms.utils import soft_clip
 from monai.transforms.utils_pytorch_numpy_unification import clip, percentile
-from monai.utils.type_conversion import convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, NumpyImageTestCase3D, assert_allclose
 
 
 class TestClipIntensityPercentilesd2D(NumpyImageTestCase2D):
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (5, 95))
-        expected = clip(convert_to_tensor(im), lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        expected = clip(im, lower, upper)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (0, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (5, 100))
         expected = clip(im, lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
@@ -93,15 +92,15 @@
         key = "img"
         clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper({key: im})
         for i, c in enumerate(im):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
-            assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+            assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     def test_ill_sharpness_factor(self):
         key = "img"
         with self.assertRaises(ValueError):
             ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, sharpness_factor=0.0)
 
     def test_ill_lower_percentile(self):
@@ -131,35 +130,35 @@
     def test_hard_clipping_two_sided(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (5, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (0, 95))
         expected = clip(im, lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
         lower, upper = percentile(im, (5, 100))
         expected = clip(im, lower, upper)
-        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+        assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
@@ -195,12 +194,12 @@
         key = "img"
         clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper({key: im})
         for i, c in enumerate(im):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
-            assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-7, atol=0)
+            assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_complex_utils.py` & `monai_weekly-1.4.dev2417/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_component_locator.py` & `monai_weekly-1.4.dev2417/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_component_store.py` & `monai_weekly-1.4.dev2417/tests/test_component_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,25 +44,25 @@
         test_obj1 = object()
         test_obj2 = object()
 
         self.cs.add("test_obj1", "Test object", test_obj1)
         self.cs.add("test_obj2", "Test object", test_obj2)
 
         self.assertEqual(len(self.cs), 2)
-        self.assertTrue("test_obj1" in self.cs)
-        self.assertTrue("test_obj2" in self.cs)
+        self.assertIn("test_obj1", self.cs)
+        self.assertIn("test_obj2", self.cs)
 
     def test_add_def(self):
-        self.assertFalse("test_func" in self.cs)
+        self.assertNotIn("test_func", self.cs)
 
         @self.cs.add_def("test_func", "Test function")
         def test_func():
             return 123
 
-        self.assertTrue("test_func" in self.cs)
+        self.assertIn("test_func", self.cs)
 
         self.assertEqual(len(self.cs), 1)
         self.assertEqual(list(self.cs), [("test_func", test_func)])
 
         self.assertEqual(self.cs.test_func, test_func)
         self.assertEqual(self.cs["test_func"], test_func)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_compose.py` & `monai_weekly-1.4.dev2417/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compose_get_number_conversions.py` & `monai_weekly-1.4.dev2417/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_confusion_matrix.py` & `monai_weekly-1.4.dev2417/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_f_beta.py` & `monai_weekly-1.4.dev2417/tests/test_compute_f_beta.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 import torch
+from parameterized import parameterized
 
 from monai.metrics import FBetaScore
 from tests.utils import assert_allclose
 
 _device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 
@@ -29,34 +30,29 @@
         y_pred = torch.tensor([[1, 1, 1], [1, 1, 1], [1, 1, 1]], device=_device)
         y = torch.tensor([[1, 0, 1], [0, 1, 0], [1, 0, 1]], device=_device)
         metric(y_pred=y_pred, y=y)
         result = metric.aggregate()[0]
         assert_allclose(result, torch.Tensor([0.714286]), atol=1e-6, rtol=1e-6)
         np.testing.assert_equal(result.device, y_pred.device)
 
-    def test_expecting_success2(self):
-        metric = FBetaScore(beta=0.5)
-        metric(
-            y_pred=torch.Tensor([[1, 1, 1], [1, 1, 1], [1, 1, 1]]), y=torch.Tensor([[1, 0, 1], [0, 1, 0], [1, 0, 1]])
-        )
-        assert_allclose(metric.aggregate()[0], torch.Tensor([0.609756]), atol=1e-6, rtol=1e-6)
-
-    def test_expecting_success3(self):
-        metric = FBetaScore(beta=2)
-        metric(
-            y_pred=torch.Tensor([[1, 1, 1], [1, 1, 1], [1, 1, 1]]), y=torch.Tensor([[1, 0, 1], [0, 1, 0], [1, 0, 1]])
-        )
-        assert_allclose(metric.aggregate()[0], torch.Tensor([0.862069]), atol=1e-6, rtol=1e-6)
-
-    def test_denominator_is_zero(self):
-        metric = FBetaScore(beta=2)
-        metric(
-            y_pred=torch.Tensor([[1, 1, 1], [1, 1, 1], [1, 1, 1]]), y=torch.Tensor([[0, 0, 0], [0, 0, 0], [0, 0, 0]])
-        )
-        assert_allclose(metric.aggregate()[0], torch.Tensor([0.0]), atol=1e-6, rtol=1e-6)
+    @parameterized.expand(
+        [
+            (0.5, torch.Tensor([[1, 0, 1], [0, 1, 0], [1, 0, 1]]), torch.Tensor([0.609756])),  # success_beta_0_5
+            (2, torch.Tensor([[1, 0, 1], [0, 1, 0], [1, 0, 1]]), torch.Tensor([0.862069])),  # success_beta_2
+            (
+                2,  # success_beta_2, denominator_zero
+                torch.Tensor([[0, 0, 0], [0, 0, 0], [0, 0, 0]]),
+                torch.Tensor([0.0]),
+            ),
+        ]
+    )
+    def test_success_and_zero(self, beta, y, expected_score):
+        metric = FBetaScore(beta=beta)
+        metric(y_pred=torch.Tensor([[1, 1, 1], [1, 1, 1], [1, 1, 1]]), y=y)
+        assert_allclose(metric.aggregate()[0], expected_score, atol=1e-6, rtol=1e-6)
 
     def test_number_of_dimensions_less_than_2_should_raise_error(self):
         metric = FBetaScore()
         with self.assertRaises(ValueError):
             metric(y_pred=torch.Tensor([1, 1, 1]), y=torch.Tensor([0, 0, 0]))
 
     def test_with_nan_values(self):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_fid_metric.py` & `monai_weekly-1.4.dev2417/tests/test_compute_fid_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_froc.py` & `monai_weekly-1.4.dev2417/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_generalized_dice.py` & `monai_weekly-1.4.dev2417/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_ho_ver_maps.py` & `monai_weekly-1.4.dev2417/tests/test_compute_ho_ver_maps.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,14 @@
 @unittest.skipUnless(has_skimage, "Requires scikit-image library.")
 class ComputeHoVerMapsTests(unittest.TestCase):
 
     @parameterized.expand(TESTS)
     def test_horizontal_certical_maps(self, in_type, arguments, mask, hv_mask):
         input_image = in_type(mask)
         result = ComputeHoVerMaps(**arguments)(input_image)
-        self.assertTrue(isinstance(result, torch.Tensor))
-        self.assertTrue(str(result.dtype).split(".")[1] == arguments.get("dtype", "float32"))
+        self.assertIsInstance(result, torch.Tensor)
+        self.assertEqual(str(result.dtype).split(".")[1], arguments.get("dtype", "float32"))
         assert_allclose(result, hv_mask, type_test="tensor")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_ho_ver_maps_d.py` & `monai_weekly-1.4.dev2417/tests/test_compute_ho_ver_maps_d.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,14 @@
     @parameterized.expand(TESTS)
     def test_horizontal_certical_maps(self, in_type, arguments, mask, hv_mask):
         hv_key = list(hv_mask.keys())[0]
         input_image = {}
         for k in mask.keys():
             input_image[k] = in_type(mask[k])
         result = ComputeHoVerMapsd(keys="mask", **arguments)(input_image)[hv_key]
-        self.assertTrue(isinstance(result, torch.Tensor))
-        self.assertTrue(str(result.dtype).split(".")[1] == arguments.get("dtype", "float32"))
+        self.assertIsInstance(result, torch.Tensor)
+        self.assertEqual(str(result.dtype).split(".")[1], arguments.get("dtype", "float32"))
         assert_allclose(result, hv_mask[hv_key], type_test="tensor")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_meandice.py` & `monai_weekly-1.4.dev2417/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_meaniou.py` & `monai_weekly-1.4.dev2417/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_mmd_metric.py` & `monai_weekly-1.4.dev2417/tests/test_compute_mmd_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_multiscalessim_metric.py` & `monai_weekly-1.4.dev2417/tests/test_compute_multiscalessim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_panoptic_quality.py` & `monai_weekly-1.4.dev2417/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_regression_metrics.py` & `monai_weekly-1.4.dev2417/tests/test_compute_regression_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,30 +66,32 @@
                     in_tensor = torch.rand((batch,) + (base,) * (spatial - 1)).to(device)
 
                     # iterate over regression metrics, check shape for diff. reduction func
                     for mt_fn in metrics:
                         mt = mt_fn(reduction="mean")
                         mt(in_tensor, in_tensor)
                         out_tensor = mt.aggregate()
-                        self.assertTrue(len(out_tensor.shape) == 1)
+                        self.assertEqual(len(out_tensor.shape), 1)
 
                         mt = mt_fn(reduction="sum")
                         mt(in_tensor, in_tensor)
                         out_tensor = mt.aggregate()
-                        self.assertTrue(len(out_tensor.shape) == 0)
+                        self.assertEqual(len(out_tensor.shape), 0)
 
                         mt = mt_fn(reduction="sum")  # test reduction arg overriding
                         mt(in_tensor, in_tensor)
                         out_tensor = mt.aggregate(reduction="mean_channel")
-                        self.assertTrue(len(out_tensor.shape) == 1 and out_tensor.shape[0] == batch)
+                        self.assertEqual(len(out_tensor.shape), 1)
+                        self.assertEqual(out_tensor.shape[0], batch)
 
                         mt = mt_fn(reduction="sum_channel")
                         mt(in_tensor, in_tensor)
                         out_tensor = mt.aggregate()
-                        self.assertTrue(len(out_tensor.shape) == 1 and out_tensor.shape[0] == batch)
+                        self.assertEqual(len(out_tensor.shape), 1)
+                        self.assertEqual(out_tensor.shape[0], batch)
 
     def test_compare_numpy(self):
         set_determinism(seed=123)
         device = "cuda" if torch.cuda.is_available() else "cpu"
 
         # regression metrics to check + truth metric function in numpy
         metrics = [MSEMetric, MAEMetric, RMSEMetric, partial(PSNRMetric, max_val=1.0)]
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_roc_auc.py` & `monai_weekly-1.4.dev2417/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_compute_variance.py` & `monai_weekly-1.4.dev2417/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_concat_itemsd.py` & `monai_weekly-1.4.dev2417/tests/test_concat_itemsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,37 +26,37 @@
     def test_tensor_values(self):
         device = torch.device("cuda:0") if torch.cuda.is_available() else torch.device("cpu:0")
         input_data = {
             "img1": torch.tensor([[0, 1], [1, 2]], device=device),
             "img2": torch.tensor([[0, 1], [1, 2]], device=device),
         }
         result = ConcatItemsd(keys=["img1", "img2"], name="cat_img")(input_data)
-        self.assertTrue("cat_img" in result)
+        self.assertIn("cat_img", result)
         result["cat_img"] += 1
         assert_allclose(result["img1"], torch.tensor([[0, 1], [1, 2]], device=device))
         assert_allclose(result["cat_img"], torch.tensor([[1, 2], [2, 3], [1, 2], [2, 3]], device=device))
 
     def test_metatensor_values(self):
         device = torch.device("cuda:0") if torch.cuda.is_available() else torch.device("cpu:0")
         input_data = {
             "img1": MetaTensor([[0, 1], [1, 2]], device=device),
             "img2": MetaTensor([[0, 1], [1, 2]], device=device),
         }
         result = ConcatItemsd(keys=["img1", "img2"], name="cat_img")(input_data)
-        self.assertTrue("cat_img" in result)
-        self.assertTrue(isinstance(result["cat_img"], MetaTensor))
+        self.assertIn("cat_img", result)
+        self.assertIsInstance(result["cat_img"], MetaTensor)
         self.assertEqual(result["img1"].meta, result["cat_img"].meta)
         result["cat_img"] += 1
         assert_allclose(result["img1"], torch.tensor([[0, 1], [1, 2]], device=device))
         assert_allclose(result["cat_img"], torch.tensor([[1, 2], [2, 3], [1, 2], [2, 3]], device=device))
 
     def test_numpy_values(self):
         input_data = {"img1": np.array([[0, 1], [1, 2]]), "img2": np.array([[0, 1], [1, 2]])}
         result = ConcatItemsd(keys=["img1", "img2"], name="cat_img")(input_data)
-        self.assertTrue("cat_img" in result)
+        self.assertIn("cat_img", result)
         result["cat_img"] += 1
         np.testing.assert_allclose(result["img1"], np.array([[0, 1], [1, 2]]))
         np.testing.assert_allclose(result["cat_img"], np.array([[1, 2], [2, 3], [1, 2], [2, 3]]))
 
     def test_single_numpy(self):
         input_data = {"img": np.array([[0, 1], [1, 2]])}
         result = ConcatItemsd(keys="img", name="cat_img")(input_data)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_config_item.py` & `monai_weekly-1.4.dev2417/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_config_parser.py` & `monai_weekly-1.4.dev2417/tests/test_config_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     @parameterized.expand([TEST_CASE_2])
     def test_function(self, config):
         parser = ConfigParser(config=config, globals={"TestClass": TestClass})
         for id in config:
             if id in ("compute", "cls_compute"):
                 parser[f"{id}#_mode_"] = "callable"
             func = parser.get_parsed_content(id=id)
-            self.assertTrue(id in parser.ref_resolver.resolved_content)
+            self.assertIn(id, parser.ref_resolver.resolved_content)
             if id == "error_func":
                 with self.assertRaises(TypeError):
                     func(1, 2)
                 continue
             self.assertEqual(func(1, 2), 3)
 
     @parameterized.expand([TEST_CASE_3])
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_conjugate_gradient.py` & `monai_weekly-1.4.dev2417/tests/test_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_contrastive_loss.py` & `monai_weekly-1.4.dev2417/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_data_type.py` & `monai_weekly-1.4.dev2417/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_to_multi_channel.py` & `monai_weekly-1.4.dev2417/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_to_multi_channeld.py` & `monai_weekly-1.4.dev2417/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_to_onnx.py` & `monai_weekly-1.4.dev2417/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_to_torchscript.py` & `monai_weekly-1.4.dev2417/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convert_to_trt.py` & `monai_weekly-1.4.dev2417/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_convolutions.py` & `monai_weekly-1.4.dev2417/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_copy_itemsd.py` & `monai_weekly-1.4.dev2417/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_copy_model_state.py` & `monai_weekly-1.4.dev2417/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_correct_crop_centers.py` & `monai_weekly-1.4.dev2417/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_create_cross_validation_datalist.py` & `monai_weekly-1.4.dev2417/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_create_grid_and_affine.py` & `monai_weekly-1.4.dev2417/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_crf_cpu.py` & `monai_weekly-1.4.dev2417/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_crf_cuda.py` & `monai_weekly-1.4.dev2417/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_crop_foreground.py` & `monai_weekly-1.4.dev2417/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_crop_foregroundd.py` & `monai_weekly-1.4.dev2417/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cross_validation.py` & `monai_weekly-1.4.dev2417/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_csv_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_csv_iterable_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_csv_saver.py` & `monai_weekly-1.4.dev2417/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cucim_dict_transform.py` & `monai_weekly-1.4.dev2417/tests/test_cucim_dict_transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,16 +76,16 @@
             TEST_CASE_SCALE_INTENSITY_1,
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_numpy_single(self, params, input, expected):
         input = {"image": input}
         output = CuCIMd(keys="image", **params)(input)["image"]
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, np.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, np.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -94,16 +94,16 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_numpy_batch(self, params, input, expected):
         input = {"image": input[cp.newaxis, ...]}
         expected = expected[cp.newaxis, ...]
         output = CuCIMd(keys="image", **params)(input)["image"]
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, np.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, np.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -112,16 +112,16 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_cupy_single(self, params, input, expected):
         input = {"image": cp.asarray(input)}
         expected = cp.asarray(expected)
         output = CuCIMd(keys="image", **params)(input)["image"]
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, cp.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, cp.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -130,14 +130,14 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_cupy_batch(self, params, input, expected):
         input = {"image": cp.asarray(input)[cp.newaxis, ...]}
         expected = cp.asarray(expected)[cp.newaxis, ...]
         output = CuCIMd(keys="image", **params)(input)["image"]
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, cp.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, cp.ndarray)
         cp.testing.assert_allclose(output, expected)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_cucim_transform.py` & `monai_weekly-1.4.dev2417/tests/test_cucim_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             TEST_CASE_ROTATE_1,
             TEST_CASE_SCALE_INTENSITY_1,
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_numpy_single(self, params, input, expected):
         output = CuCIM(**params)(input)
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, np.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, np.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -93,16 +93,16 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_numpy_batch(self, params, input, expected):
         input = input[cp.newaxis, ...]
         expected = expected[cp.newaxis, ...]
         output = CuCIM(**params)(input)
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, np.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, np.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -111,16 +111,16 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_cupy_single(self, params, input, expected):
         input = cp.asarray(input)
         expected = cp.asarray(expected)
         output = CuCIM(**params)(input)
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, cp.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, cp.ndarray)
         cp.testing.assert_allclose(output, expected)
 
     @parameterized.expand(
         [
             TEST_CASE_COLOR_JITTER_1,
             TEST_CASE_COLOR_JITTER_2,
             TEST_CASE_FLIP_1,
@@ -129,14 +129,14 @@
             TEST_CASE_ZOOM_1,
         ]
     )
     def test_tramsforms_cupy_batch(self, params, input, expected):
         input = cp.asarray(input)[cp.newaxis, ...]
         expected = cp.asarray(expected)[cp.newaxis, ...]
         output = CuCIM(**params)(input)
-        self.assertTrue(output.dtype == expected.dtype)
-        self.assertTrue(isinstance(output, cp.ndarray))
+        self.assertEqual(output.dtype, expected.dtype)
+        self.assertIsInstance(output, cp.ndarray)
         cp.testing.assert_allclose(output, expected)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_cumulative.py` & `monai_weekly-1.4.dev2417/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cumulative_average.py` & `monai_weekly-1.4.dev2417/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cumulative_average_dist.py` & `monai_weekly-1.4.dev2417/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_cv2_dist.py` & `monai_weekly-1.4.dev2417/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_daf3d.py` & `monai_weekly-1.4.dev2417/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_data_stats.py` & `monai_weekly-1.4.dev2417/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_data_statsd.py` & `monai_weekly-1.4.dev2417/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dataloader.py` & `monai_weekly-1.4.dev2417/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dataset_func.py` & `monai_weekly-1.4.dev2417/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dataset_summary.py` & `monai_weekly-1.4.dev2417/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_decathlondataset.py` & `monai_weekly-1.4.dev2417/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_decollate.py` & `monai_weekly-1.4.dev2417/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deepedit_interaction.py` & `monai_weekly-1.4.dev2417/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deepedit_transforms.py` & `monai_weekly-1.4.dev2417/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deepgrow_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deepgrow_interaction.py` & `monai_weekly-1.4.dev2417/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deepgrow_transforms.py` & `monai_weekly-1.4.dev2417/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_delete_itemsd.py` & `monai_weekly-1.4.dev2417/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_denseblock.py` & `monai_weekly-1.4.dev2417/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_densenet.py` & `monai_weekly-1.4.dev2417/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_deprecated.py` & `monai_weekly-1.4.dev2417/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_detect_envelope.py` & `monai_weekly-1.4.dev2417/tests/test_detect_envelope.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     )
     def test_value_error(self, arguments, image, method):
         if method == "__init__":
             self.assertRaises(ValueError, DetectEnvelope, **arguments)
         elif method == "__call__":
             self.assertRaises(ValueError, DetectEnvelope(**arguments), image)
         else:
-            raise ValueError("Expected raising method invalid. Should be __init__ or __call__.")
+            self.fail("Expected raising method invalid. Should be __init__ or __call__.")
 
 
 @SkipIfModule("torch.fft")
 class TestHilbertTransformNoFFTMod(unittest.TestCase):
 
     def test_no_fft_module_error(self):
         self.assertRaises(OptionalImportError, DetectEnvelope(), np.random.rand(1, 10))
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_detection_coco_metrics.py` & `monai_weekly-1.4.dev2417/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_detector_boxselector.py` & `monai_weekly-1.4.dev2417/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_detector_utils.py` & `monai_weekly-1.4.dev2417/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dev_collate.py` & `monai_weekly-1.4.dev2417/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dice_ce_loss.py` & `monai_weekly-1.4.dev2417/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dice_focal_loss.py` & `monai_weekly-1.4.dev2417/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dice_loss.py` & `monai_weekly-1.4.dev2417/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_diffusion_loss.py` & `monai_weekly-1.4.dev2417/tests/test_diffusion_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dints_cell.py` & `monai_weekly-1.4.dev2417/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dints_mixop.py` & `monai_weekly-1.4.dev2417/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dints_network.py` & `monai_weekly-1.4.dev2417/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_discriminator.py` & `monai_weekly-1.4.dev2417/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_distance_transform_edt.py` & `monai_weekly-1.4.dev2417/tests/test_distance_transform_edt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_divisible_pad.py` & `monai_weekly-1.4.dev2417/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_divisible_padd.py` & `monai_weekly-1.4.dev2417/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_download_and_extract.py` & `monai_weekly-1.4.dev2417/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_download_url_yandex.py` & `monai_weekly-1.4.dev2417/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_downsample_block.py` & `monai_weekly-1.4.dev2417/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_drop_path.py` & `monai_weekly-1.4.dev2417/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ds_loss.py` & `monai_weekly-1.4.dev2417/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dvf2ddf.py` & `monai_weekly-1.4.dev2417/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dynunet.py` & `monai_weekly-1.4.dev2417/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_dynunet_block.py` & `monai_weekly-1.4.dev2417/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_efficientnet.py` & `monai_weekly-1.4.dev2417/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensemble_evaluator.py` & `monai_weekly-1.4.dev2417/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensure_channel_first.py` & `monai_weekly-1.4.dev2417/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensure_channel_firstd.py` & `monai_weekly-1.4.dev2417/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensure_tuple.py` & `monai_weekly-1.4.dev2417/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensure_type.py` & `monai_weekly-1.4.dev2417/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ensure_typed.py` & `monai_weekly-1.4.dev2417/tests/test_ensure_typed.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,58 +29,58 @@
             test_datas.append(test_datas[-1].cuda())
         for test_data in test_datas:
             for dtype in ("tensor", "NUMPY"):
                 result = EnsureTyped(
                     keys="data", data_type=dtype, dtype=np.float32 if dtype == "NUMPY" else None, device="cpu"
                 )({"data": test_data})["data"]
                 if dtype == "NUMPY":
-                    self.assertTrue(result.dtype == np.float32)
-                self.assertTrue(isinstance(result, torch.Tensor if dtype == "tensor" else np.ndarray))
+                    self.assertEqual(result.dtype, np.float32)
+                self.assertIsInstance(result, torch.Tensor if dtype == "tensor" else np.ndarray)
                 assert_allclose(result, test_data, type_test=False)
                 self.assertTupleEqual(result.shape, (2, 2))
 
     def test_single_input(self):
         test_datas = [5, 5.0, False, np.asarray(5), torch.tensor(5)]
         if torch.cuda.is_available():
             test_datas.append(test_datas[-1].cuda())
         for test_data in test_datas:
             for dtype in ("tensor", "numpy"):
                 result = EnsureTyped(keys="data", data_type=dtype)({"data": test_data})["data"]
-                self.assertTrue(isinstance(result, torch.Tensor if dtype == "tensor" else np.ndarray))
+                self.assertIsInstance(result, torch.Tensor if dtype == "tensor" else np.ndarray)
                 if isinstance(test_data, bool):
                     self.assertFalse(result)
                 else:
                     assert_allclose(result, test_data, type_test=False)
                 self.assertEqual(result.ndim, 0)
 
     def test_string(self):
         for dtype in ("tensor", "numpy"):
             # string input
             result = EnsureTyped(keys="data", data_type=dtype)({"data": "test_string"})["data"]
-            self.assertTrue(isinstance(result, str))
+            self.assertIsInstance(result, str)
             self.assertEqual(result, "test_string")
             # numpy array of string
             result = EnsureTyped(keys="data", data_type=dtype)({"data": np.array(["test_string"])})["data"]
-            self.assertTrue(isinstance(result, np.ndarray))
+            self.assertIsInstance(result, np.ndarray)
             self.assertEqual(result[0], "test_string")
 
     def test_list_tuple(self):
         for dtype in ("tensor", "numpy"):
             result = EnsureTyped(keys="data", data_type=dtype, wrap_sequence=False, track_meta=True)(
                 {"data": [[1, 2], [3, 4]]}
             )["data"]
-            self.assertTrue(isinstance(result, list))
-            self.assertTrue(isinstance(result[0][1], MetaTensor if dtype == "tensor" else np.ndarray))
+            self.assertIsInstance(result, list)
+            self.assertIsInstance(result[0][1], MetaTensor if dtype == "tensor" else np.ndarray)
             assert_allclose(result[1][0], torch.as_tensor(3), type_test=False)
             # tuple of numpy arrays
             result = EnsureTyped(keys="data", data_type=dtype, wrap_sequence=False)(
                 {"data": (np.array([1, 2]), np.array([3, 4]))}
             )["data"]
-            self.assertTrue(isinstance(result, tuple))
-            self.assertTrue(isinstance(result[0], torch.Tensor if dtype == "tensor" else np.ndarray))
+            self.assertIsInstance(result, tuple)
+            self.assertIsInstance(result[0], torch.Tensor if dtype == "tensor" else np.ndarray)
             assert_allclose(result[1], torch.as_tensor([3, 4]), type_test=False)
 
     def test_dict(self):
         # simulate complicated input data
         test_data = {
             "img": np.array([1.0, 2.0], dtype=np.float32),
             "meta": {"dims": 3, "size": np.array([1, 2, 3]), "path": "temp/test"},
@@ -88,24 +88,24 @@
         }
         for dtype in ("tensor", "numpy"):
             trans = EnsureTyped(keys=["data", "label"], data_type=dtype, dtype=[np.float32, np.int8], device="cpu")(
                 {"data": test_data, "label": test_data}
             )
             for key in ("data", "label"):
                 result = trans[key]
-                self.assertTrue(isinstance(result, dict))
-                self.assertTrue(isinstance(result["img"], torch.Tensor if dtype == "tensor" else np.ndarray))
-                self.assertTrue(isinstance(result["meta"]["size"], torch.Tensor if dtype == "tensor" else np.ndarray))
+                self.assertIsInstance(result, dict)
+                self.assertIsInstance(result["img"], torch.Tensor if dtype == "tensor" else np.ndarray)
+                self.assertIsInstance(result["meta"]["size"], torch.Tensor if dtype == "tensor" else np.ndarray)
                 self.assertEqual(result["meta"]["path"], "temp/test")
                 self.assertEqual(result["extra"], None)
                 assert_allclose(result["img"], torch.as_tensor([1.0, 2.0]), type_test=False)
                 assert_allclose(result["meta"]["size"], torch.as_tensor([1, 2, 3]), type_test=False)
             if dtype == "numpy":
-                self.assertTrue(trans["data"]["img"].dtype == np.float32)
-                self.assertTrue(trans["label"]["img"].dtype == np.int8)
+                self.assertEqual(trans["data"]["img"].dtype, np.float32)
+                self.assertEqual(trans["label"]["img"].dtype, np.int8)
             else:
-                self.assertTrue(trans["data"]["img"].dtype == torch.float32)
-                self.assertTrue(trans["label"]["img"].dtype == torch.int8)
+                self.assertEqual(trans["data"]["img"].dtype, torch.float32)
+                self.assertEqual(trans["label"]["img"].dtype, torch.int8)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_enum_bound_interp.py` & `monai_weekly-1.4.dev2417/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_eval_mode.py` & `monai_weekly-1.4.dev2417/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_evenly_divisible_all_gather_dist.py` & `monai_weekly-1.4.dev2417/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_factorized_increase.py` & `monai_weekly-1.4.dev2417/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_factorized_reduce.py` & `monai_weekly-1.4.dev2417/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fastmri_reader.py` & `monai_weekly-1.4.dev2417/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fft_utils.py` & `monai_weekly-1.4.dev2417/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fg_bg_to_indices.py` & `monai_weekly-1.4.dev2417/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fg_bg_to_indicesd.py` & `monai_weekly-1.4.dev2417/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_file_basename.py` & `monai_weekly-1.4.dev2417/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fill_holes.py` & `monai_weekly-1.4.dev2417/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fill_holesd.py` & `monai_weekly-1.4.dev2417/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fl_exchange_object.py` & `monai_weekly-1.4.dev2417/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fl_monai_algo.py` & `monai_weekly-1.4.dev2417/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fl_monai_algo_dist.py` & `monai_weekly-1.4.dev2417/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fl_monai_algo_stats.py` & `monai_weekly-1.4.dev2417/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_flatten_sub_keysd.py` & `monai_weekly-1.4.dev2417/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_flexible_unet.py` & `monai_weekly-1.4.dev2417/tests/test_flexible_unet.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 from monai.networks import eval_mode
 from monai.networks.blocks.encoder import BaseEncoder
 from monai.networks.nets import (
     FLEXUNET_BACKBONE,
     EfficientNetBNFeatures,
     FlexibleUNet,
     FlexUNetEncoderRegister,
-    ResNet,
-    ResNetBlock,
-    ResNetBottleneck,
+    ResNetEncoder,
+    ResNetFeatures,
 )
 from monai.utils import optional_import
-from tests.utils import skip_if_downloading_fails, skip_if_quick
+from tests.utils import SkipIfNoModule, skip_if_downloading_fails, skip_if_quick
 
 torchvision, has_torchvision = optional_import("torchvision")
 PIL, has_pil = optional_import("PIL")
 
 
 class DummyEncoder(BaseEncoder):
 
@@ -55,109 +54,14 @@
         return [6, 4, 4, 4]
 
     @classmethod
     def get_encoder_names(cls):
         return ["encoder_wrong_channels", "encoder_no_param1", "encoder_no_param2", "encoder_no_param3"]
 
 
-class ResNetEncoder(ResNet, BaseEncoder):
-    backbone_names = ["resnet10", "resnet18", "resnet34", "resnet50", "resnet101", "resnet152", "resnet200"]
-    output_feature_channels = [(64, 128, 256, 512)] * 3 + [(256, 512, 1024, 2048)] * 4
-    parameter_layers = [
-        [1, 1, 1, 1],
-        [2, 2, 2, 2],
-        [3, 4, 6, 3],
-        [3, 4, 6, 3],
-        [3, 4, 23, 3],
-        [3, 8, 36, 3],
-        [3, 24, 36, 3],
-    ]
-
-    def __init__(self, in_channels, pretrained, **kargs):
-        super().__init__(**kargs, n_input_channels=in_channels)
-        if pretrained:
-            # Author of paper zipped the state_dict on googledrive,
-            # so would need to download, unzip and read (2.8gb file for a ~150mb state dict).
-            # Would like to load dict from url but need somewhere to save the state dicts.
-            raise NotImplementedError(
-                "Currently not implemented. You need to manually download weights provided by the paper's author"
-                " and load then to the model with `state_dict`. See https://github.com/Tencent/MedicalNet"
-            )
-
-    @staticmethod
-    def get_inplanes():
-        return [64, 128, 256, 512]
-
-    @classmethod
-    def get_encoder_parameters(cls) -> list[dict]:
-        """
-        Get parameter list to initialize encoder networks.
-        Each parameter dict must have `spatial_dims`, `in_channels`
-        and `pretrained` parameters.
-        """
-        parameter_list = []
-        res_type: type[ResNetBlock] | type[ResNetBottleneck]
-        for backbone in range(len(cls.backbone_names)):
-            if backbone < 3:
-                res_type = ResNetBlock
-            else:
-                res_type = ResNetBottleneck
-            parameter_list.append(
-                {
-                    "block": res_type,
-                    "layers": cls.parameter_layers[backbone],
-                    "block_inplanes": ResNetEncoder.get_inplanes(),
-                    "spatial_dims": 2,
-                    "in_channels": 3,
-                    "pretrained": False,
-                }
-            )
-        return parameter_list
-
-    @classmethod
-    def num_channels_per_output(cls):
-        """
-        Get number of output features' channel.
-        """
-        return cls.output_feature_channels
-
-    @classmethod
-    def num_outputs(cls):
-        """
-        Get number of output feature.
-        """
-        return [4] * 7
-
-    @classmethod
-    def get_encoder_names(cls):
-        """
-        Get the name string of backbones which will be used to initialize flexible unet.
-        """
-        return cls.backbone_names
-
-    def forward(self, x: torch.Tensor):
-        feature_list = []
-        x = self.conv1(x)
-        x = self.bn1(x)
-        x = self.relu(x)
-        if not self.no_max_pool:
-            x = self.maxpool(x)
-        x = self.layer1(x)
-        feature_list.append(x)
-        x = self.layer2(x)
-        feature_list.append(x)
-        x = self.layer3(x)
-        feature_list.append(x)
-        x = self.layer4(x)
-        feature_list.append(x)
-
-        return feature_list
-
-
-FLEXUNET_BACKBONE.register_class(ResNetEncoder)
 FLEXUNET_BACKBONE.register_class(DummyEncoder)
 
 
 def get_model_names():
     return [f"efficientnet-b{d}" for d in range(8)]
 
 
@@ -200,17 +104,15 @@
                                 (batch, num_classes) + (input_shape,) * spatial_dim,
                             ]
                         )
     return ret_tests
 
 
 def make_error_case():
-    error_dummy_backbones = DummyEncoder.get_encoder_names()
-    error_resnet_backbones = ResNetEncoder.get_encoder_names()
-    error_backbones = error_dummy_backbones + error_resnet_backbones
+    error_backbones = DummyEncoder.get_encoder_names()
     error_param_list = []
     for backbone in error_backbones:
         error_param_list.append(
             [{"in_channels": 3, "out_channels": 2, "backbone": backbone, "pretrained": True, "spatial_dims": 3}]
         )
     return error_param_list
 
@@ -228,15 +130,15 @@
     batches=[1, 4],
     pretrained=[False],
     in_channels=3,
     num_classes=10,
     norm="instance",
 )
 CASES_3D = make_shape_cases(
-    models=[SEL_MODELS[0]],
+    models=[SEL_MODELS[0], SEL_MODELS[2]],
     spatial_dims=[3],
     batches=[1],
     pretrained=[False],
     in_channels=3,
     num_classes=10,
     norm="batch",
 )
@@ -341,32 +243,47 @@
             "in_channels": 3,
             "out_channels": 10,
             "backbone": SEL_MODELS[0],
             "pretrained": True,
             "spatial_dims": 2,
             "norm": ("batch", {"eps": 1e-3, "momentum": 0.01}),
         },
+        EfficientNetBNFeatures,
         {
             "in_channels": 3,
             "num_classes": 10,
             "model_name": SEL_MODELS[0],
             "pretrained": True,
             "spatial_dims": 2,
             "norm": ("batch", {"eps": 1e-3, "momentum": 0.01}),
         },
         ["_conv_stem.weight"],
-    )
+    ),
+    (
+        {
+            "in_channels": 1,
+            "out_channels": 10,
+            "backbone": SEL_MODELS[2],
+            "pretrained": True,
+            "spatial_dims": 3,
+            "norm": ("batch", {"eps": 1e-3, "momentum": 0.01}),
+        },
+        ResNetFeatures,
+        {"model_name": SEL_MODELS[2], "pretrained": True, "spatial_dims": 3, "in_channels": 1},
+        ["conv1.weight"],
+    ),
 ]
 
 CASE_ERRORS = make_error_case()
 
 # Verify Register class with string type
 CASE_REGISTER_ENCODER = ["EfficientNetEncoder", "monai.networks.nets.EfficientNetEncoder"]
 
 
+@SkipIfNoModule("hf_hub_download")
 @skip_if_quick
 class TestFLEXIBLEUNET(unittest.TestCase):
 
     @parameterized.expand(CASES_2D + CASES_3D + CASES_VARIATIONS)
     def test_shape(self, input_param, input_shape, expected_shape):
         device = "cuda" if torch.cuda.is_available() else "cpu"
 
@@ -377,27 +294,27 @@
         with eval_mode(net):
             result = net(torch.randn(input_shape).to(device))
 
         # check output shape
         self.assertEqual(result.shape, expected_shape)
 
     @parameterized.expand(CASES_PRETRAIN)
-    def test_pretrain(self, input_param, efficient_input_param, weight_list):
+    def test_pretrain(self, flexunet_input_param, feature_extractor_class, feature_extractor_input_param, weight_list):
         device = "cuda" if torch.cuda.is_available() else "cpu"
 
         with skip_if_downloading_fails():
-            net = FlexibleUNet(**input_param).to(device)
+            net = FlexibleUNet(**flexunet_input_param).to(device)
 
         with skip_if_downloading_fails():
-            eff_net = EfficientNetBNFeatures(**efficient_input_param).to(device)
+            feature_extractor_net = feature_extractor_class(**feature_extractor_input_param).to(device)
 
         for weight_name in weight_list:
-            if weight_name in net.encoder.state_dict() and weight_name in eff_net.state_dict():
+            if weight_name in net.encoder.state_dict() and weight_name in feature_extractor_net.state_dict():
                 net_weight = net.encoder.state_dict()[weight_name]
-                download_weight = eff_net.state_dict()[weight_name]
+                download_weight = feature_extractor_net.state_dict()[weight_name]
                 weight_diff = torch.abs(net_weight - download_weight)
                 diff_sum = torch.sum(weight_diff)
                 # check if a weight in weight_list equals to the downloaded weight.
                 self.assertLess(abs(diff_sum.item() - 0), 1e-8)
 
     @parameterized.expand(CASE_ERRORS)
     def test_error_raise(self, input_param):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_flip.py` & `monai_weekly-1.4.dev2417/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_flipd.py` & `monai_weekly-1.4.dev2417/tests/test_flipd.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,12 +74,12 @@
             with self.assertRaisesRegex(ValueError, "MetaTensor"):
                 xform.inverse(res)
 
     @unittest.skipIf(not config.USE_META_DICT, "not using meta dict")
     def test_meta_dict(self):
         xform = Flipd("image", [0, 1])
         res = xform({"image": torch.zeros(1, 3, 4)})
-        self.assertTrue(res["image"].applied_operations == res["image_transforms"])
+        self.assertEqual(res["image"].applied_operations, res["image_transforms"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_focal_loss.py` & `monai_weekly-1.4.dev2417/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_folder_layout.py` & `monai_weekly-1.4.dev2417/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_foreground_mask.py` & `monai_weekly-1.4.dev2417/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_foreground_maskd.py` & `monai_weekly-1.4.dev2417/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fourier.py` & `monai_weekly-1.4.dev2417/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fpn_block.py` & `monai_weekly-1.4.dev2417/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_freeze_layers.py` & `monai_weekly-1.4.dev2417/tests/test_freeze_layers.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,27 +36,27 @@
         set_determinism(0)
         model = _TestModelOne(10, 20, 3)
         model.to(device)
         freeze_layers(model, "class")
 
         for name, param in model.named_parameters():
             if "class_layer" in name:
-                self.assertEqual(param.requires_grad, False)
+                self.assertFalse(param.requires_grad)
             else:
-                self.assertEqual(param.requires_grad, True)
+                self.assertTrue(param.requires_grad)
 
     @parameterized.expand(TEST_CASES)
     def test_exclude_vars(self, device):
         set_determinism(0)
         model = _TestModelTwo(10, 20, 10, 4)
         model.to(device)
         freeze_layers(model, exclude_vars="class")
 
         for name, param in model.named_parameters():
             if "class_layer" in name:
-                self.assertEqual(param.requires_grad, True)
+                self.assertTrue(param.requires_grad)
             else:
-                self.assertEqual(param.requires_grad, False)
+                self.assertFalse(param.requires_grad)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_from_engine_hovernet.py` & `monai_weekly-1.4.dev2417/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_fullyconnectednet.py` & `monai_weekly-1.4.dev2417/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian_filter.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian_sharpen.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian_sharpend.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian_smooth.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gaussian_smoothd.py` & `monai_weekly-1.4.dev2417/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gdsdataset.py` & `monai_weekly-1.4.dev2417/tests/test_gdsdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generalized_dice_focal_loss.py` & `monai_weekly-1.4.dev2417/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generalized_dice_loss.py` & `monai_weekly-1.4.dev2417/tests/test_generalized_dice_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,25 +180,25 @@
         prediction = torch.ones((1, 1, 1, 3))
         target = torch.ones((1, 1, 1, 3))
         prediction.requires_grad = True
         target.requires_grad = True
 
         generalized_dice_loss = GeneralizedDiceLoss()
         loss = generalized_dice_loss(prediction, target)
-        self.assertNotEqual(loss.grad_fn, None)
+        self.assertIsNotNone(loss.grad_fn)
 
     def test_batch(self):
         prediction = torch.zeros(2, 3, 3, 3)
         target = torch.zeros(2, 3, 3, 3)
         prediction.requires_grad = True
         target.requires_grad = True
 
         generalized_dice_loss = GeneralizedDiceLoss(batch=True)
         loss = generalized_dice_loss(prediction, target)
-        self.assertNotEqual(loss.grad_fn, None)
+        self.assertIsNotNone(loss.grad_fn)
 
     def test_script(self):
         loss = GeneralizedDiceLoss()
         test_input = torch.ones(2, 1, 8, 8)
         test_script_save(loss, test_input, test_input)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_generalized_wasserstein_dice_loss.py` & `monai_weekly-1.4.dev2417/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_distance_map.py` & `monai_weekly-1.4.dev2417/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_distance_mapd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_border.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_borderd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_centroid.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_centroidd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_contour.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_contourd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_type.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_instance_typed.py` & `monai_weekly-1.4.dev2417/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_label_classes_crop_centers.py` & `monai_weekly-1.4.dev2417/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_param_groups.py` & `monai_weekly-1.4.dev2417/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_pos_neg_label_crop_centers.py` & `monai_weekly-1.4.dev2417/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_spatial_bounding_box.py` & `monai_weekly-1.4.dev2417/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_succinct_contour.py` & `monai_weekly-1.4.dev2417/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_succinct_contourd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_watershed_markers.py` & `monai_weekly-1.4.dev2417/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_watershed_markersd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_watershed_mask.py` & `monai_weekly-1.4.dev2417/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generate_watershed_maskd.py` & `monai_weekly-1.4.dev2417/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_generator.py` & `monai_weekly-1.4.dev2417/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_get_equivalent_dtype.py` & `monai_weekly-1.4.dev2417/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_get_extreme_points.py` & `monai_weekly-1.4.dev2417/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_get_layers.py` & `monai_weekly-1.4.dev2417/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_get_package_version.py` & `monai_weekly-1.4.dev2417/tests/test_get_package_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from monai.utils.module import get_package_version
 
 
 class TestGetVersion(unittest.TestCase):
 
     def test_default(self):
         output = get_package_version("42foobarnoexist")
-        self.assertTrue("UNKNOWN" in output)
+        self.assertIn("UNKNOWN", output)
 
         output = get_package_version("numpy")
-        self.assertFalse("UNKNOWN" in output)
+        self.assertNotIn("UNKNOWN", output)
 
     def test_msg(self):
         output = get_package_version("42foobarnoexist", "test")
-        self.assertTrue("test" in output)
+        self.assertIn("test", output)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_get_unique_labels.py` & `monai_weekly-1.4.dev2417/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gibbs_noise.py` & `monai_weekly-1.4.dev2417/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gibbs_noised.py` & `monai_weekly-1.4.dev2417/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_giou_loss.py` & `monai_weekly-1.4.dev2417/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_global_mutual_information_loss.py` & `monai_weekly-1.4.dev2417/tests/test_global_mutual_information_loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from __future__ import annotations
 
 import os
 import unittest
 
 import numpy as np
 import torch
+from parameterized import parameterized
 
 from monai import transforms
 from monai.losses.image_dissimilarity import GlobalMutualInformationLoss
 from tests.utils import SkipIfBeforePyTorchVersion, download_url_or_skip_test, skip_if_quick, testing_data_config
 
 device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
@@ -112,29 +113,38 @@
                 a2 = a2.clone().unsqueeze(0).unsqueeze(0).to(device)
                 result = loss_fn(a2, a1).detach().cpu().numpy()
                 np.testing.assert_allclose(result, expected_value, rtol=0.08, atol=0.05)
 
 
 class TestGlobalMutualInformationLossIll(unittest.TestCase):
 
-    def test_ill_shape(self):
+    @parameterized.expand(
+        [
+            (torch.ones((1, 2), dtype=torch.float), torch.ones((1, 3), dtype=torch.float)),  # mismatched_simple_dims
+            (
+                torch.ones((1, 3, 3), dtype=torch.float),
+                torch.ones((1, 3), dtype=torch.float),
+            ),  # mismatched_advanced_dims
+        ]
+    )
+    def test_ill_shape(self, input1, input2):
         loss = GlobalMutualInformationLoss()
-        with self.assertRaisesRegex(ValueError, ""):
-            loss.forward(torch.ones((1, 2), dtype=torch.float), torch.ones((1, 3), dtype=torch.float, device=device))
-        with self.assertRaisesRegex(ValueError, ""):
-            loss.forward(torch.ones((1, 3, 3), dtype=torch.float), torch.ones((1, 3), dtype=torch.float, device=device))
+        with self.assertRaises(ValueError):
+            loss.forward(input1, input2)
 
-    def test_ill_opts(self):
+    @parameterized.expand(
+        [
+            (0, "mean", ValueError, ""),  # num_bins_zero
+            (-1, "mean", ValueError, ""),  # num_bins_negative
+            (64, "unknown", ValueError, ""),  # reduction_unknown
+            (64, None, ValueError, ""),  # reduction_none
+        ]
+    )
+    def test_ill_opts(self, num_bins, reduction, expected_exception, expected_message):
         pred = torch.ones((1, 3, 3, 3, 3), dtype=torch.float, device=device)
         target = torch.ones((1, 3, 3, 3, 3), dtype=torch.float, device=device)
-        with self.assertRaisesRegex(ValueError, ""):
-            GlobalMutualInformationLoss(num_bins=0)(pred, target)
-        with self.assertRaisesRegex(ValueError, ""):
-            GlobalMutualInformationLoss(num_bins=-1)(pred, target)
-        with self.assertRaisesRegex(ValueError, ""):
-            GlobalMutualInformationLoss(reduction="unknown")(pred, target)
-        with self.assertRaisesRegex(ValueError, ""):
-            GlobalMutualInformationLoss(reduction=None)(pred, target)
+        with self.assertRaisesRegex(expected_exception, expected_message):
+            GlobalMutualInformationLoss(num_bins=num_bins, reduction=reduction)(pred, target)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_globalnet.py` & `monai_weekly-1.4.dev2417/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_gmm.py` & `monai_weekly-1.4.dev2417/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_distortion.py` & `monai_weekly-1.4.dev2417/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_distortiond.py` & `monai_weekly-1.4.dev2417/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_patch.py` & `monai_weekly-1.4.dev2417/tests/test_grid_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         splitter = GridPatch(**input_parameters)
         output = splitter(image)
         self.assertEqual(len(output), len(expected))
         if "path" in expected_meta[0]:
             self.assertTrue(output.meta["path"] == expected_meta[0]["path"])
         for output_patch, expected_patch, expected_patch_meta in zip(output, expected, expected_meta):
             assert_allclose(output_patch, expected_patch, type_test=False)
-            self.assertTrue(isinstance(output_patch, MetaTensor))
-            self.assertTrue(output_patch.meta["location"] == expected_patch_meta["location"])
+            self.assertIsInstance(output_patch, MetaTensor)
+            self.assertEqual(output_patch.meta["location"], expected_patch_meta["location"])
             self.assertTrue(output_patch.meta["spatial_shape"], list(output_patch.shape[1:]))
             if "path" in expected_meta[0]:
-                self.assertTrue(output_patch.meta["path"] == expected_patch_meta["path"])
+                self.assertEqual(output_patch.meta["path"], expected_patch_meta["path"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_patchd.py` & `monai_weekly-1.4.dev2417/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_pull.py` & `monai_weekly-1.4.dev2417/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_split.py` & `monai_weekly-1.4.dev2417/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_grid_splitd.py` & `monai_weekly-1.4.dev2417/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_checkpoint_loader.py` & `monai_weekly-1.4.dev2417/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_checkpoint_saver.py` & `monai_weekly-1.4.dev2417/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_classification_saver.py` & `monai_weekly-1.4.dev2417/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_classification_saver_dist.py` & `monai_weekly-1.4.dev2417/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_clearml_image.py` & `monai_weekly-1.4.dev2417/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_clearml_stats.py` & `monai_weekly-1.4.dev2417/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_confusion_matrix.py` & `monai_weekly-1.4.dev2417/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_confusion_matrix_dist.py` & `monai_weekly-1.4.dev2417/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_decollate_batch.py` & `monai_weekly-1.4.dev2417/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_early_stop.py` & `monai_weekly-1.4.dev2417/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_garbage_collector.py` & `monai_weekly-1.4.dev2417/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_hausdorff_distance.py` & `monai_weekly-1.4.dev2417/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_ignite_metric.py` & `monai_weekly-1.4.dev2417/tests/test_handler_ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_logfile.py` & `monai_weekly-1.4.dev2417/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_lr_scheduler.py` & `monai_weekly-1.4.dev2417/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_mean_dice.py` & `monai_weekly-1.4.dev2417/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_mean_iou.py` & `monai_weekly-1.4.dev2417/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_metric_logger.py` & `monai_weekly-1.4.dev2417/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_metrics_reloaded.py` & `monai_weekly-1.4.dev2417/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_metrics_saver.py` & `monai_weekly-1.4.dev2417/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_metrics_saver_dist.py` & `monai_weekly-1.4.dev2417/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_mlflow.py` & `monai_weekly-1.4.dev2417/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_nvtx.py` & `monai_weekly-1.4.dev2417/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_panoptic_quality.py` & `monai_weekly-1.4.dev2417/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_parameter_scheduler.py` & `monai_weekly-1.4.dev2417/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_post_processing.py` & `monai_weekly-1.4.dev2417/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_prob_map_producer.py` & `monai_weekly-1.4.dev2417/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_regression_metrics.py` & `monai_weekly-1.4.dev2417/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_regression_metrics_dist.py` & `monai_weekly-1.4.dev2417/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_rocauc.py` & `monai_weekly-1.4.dev2417/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_rocauc_dist.py` & `monai_weekly-1.4.dev2417/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_smartcache.py` & `monai_weekly-1.4.dev2417/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_stats.py` & `monai_weekly-1.4.dev2417/tests/test_handler_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         log_handler.close()
         has_key_word = re.compile(f".*{key_to_print}.*")
         content_count = 0
         for line in output_str.split("\n"):
             if has_key_word.match(line):
                 content_count += 1
         if epoch_log is True:
-            self.assertTrue(content_count == max_epochs)
+            self.assertEqual(content_count, max_epochs)
         else:
-            self.assertTrue(content_count == 2)  # 2 = len([1, 2]) from event_filter
+            self.assertEqual(content_count, 2)  # 2 = len([1, 2]) from event_filter
 
     @parameterized.expand([[True], [get_event_filter([1, 3])]])
     def test_loss_print(self, iteration_log):
         log_stream = StringIO()
         log_handler = logging.StreamHandler(log_stream)
         log_handler.setLevel(logging.INFO)
         key_to_handler = "test_logging"
@@ -112,17 +112,17 @@
         log_handler.close()
         has_key_word = re.compile(f".*{key_to_print}.*")
         content_count = 0
         for line in output_str.split("\n"):
             if has_key_word.match(line):
                 content_count += 1
         if iteration_log is True:
-            self.assertTrue(content_count == num_iters * max_epochs)
+            self.assertEqual(content_count, num_iters * max_epochs)
         else:
-            self.assertTrue(content_count == 2)  # 2 = len([1, 3]) from event_filter
+            self.assertEqual(content_count, 2)  # 2 = len([1, 3]) from event_filter
 
     def test_loss_dict(self):
         log_stream = StringIO()
         log_handler = logging.StreamHandler(log_stream)
         log_handler.setLevel(logging.INFO)
         key_to_handler = "test_logging"
         key_to_print = "myLoss1"
@@ -146,15 +146,15 @@
         output_str = log_stream.getvalue()
         log_handler.close()
         has_key_word = re.compile(f".*{key_to_print}.*")
         content_count = 0
         for line in output_str.split("\n"):
             if has_key_word.match(line):
                 content_count += 1
-        self.assertTrue(content_count > 0)
+        self.assertGreater(content_count, 0)
 
     def test_loss_file(self):
         key_to_handler = "test_logging"
         key_to_print = "myLoss"
 
         with tempfile.TemporaryDirectory() as tempdir:
             filename = os.path.join(tempdir, "test_loss_stats.log")
@@ -180,15 +180,15 @@
             with open(filename) as f:
                 output_str = f.read()
                 has_key_word = re.compile(f".*{key_to_print}.*")
                 content_count = 0
                 for line in output_str.split("\n"):
                     if has_key_word.match(line):
                         content_count += 1
-                self.assertTrue(content_count > 0)
+                self.assertGreater(content_count, 0)
 
     def test_exception(self):
         # set up engine
         def _train_func(engine, batch):
             raise RuntimeError("test exception.")
 
         engine = Engine(_train_func)
@@ -235,15 +235,15 @@
         output_str = log_stream.getvalue()
         log_handler.close()
         has_key_word = re.compile(".*State values.*")
         content_count = 0
         for line in output_str.split("\n"):
             if has_key_word.match(line):
                 content_count += 1
-        self.assertTrue(content_count > 0)
+        self.assertGreater(content_count, 0)
 
     def test_default_logger(self):
         log_stream = StringIO()
         log_handler = logging.StreamHandler(log_stream)
         log_handler.setLevel(logging.INFO)
         key_to_print = "myLoss"
 
@@ -270,12 +270,12 @@
         output_str = log_stream.getvalue()
         log_handler.close()
         has_key_word = re.compile(f".*{key_to_print}.*")
         content_count = 0
         for line in output_str.split("\n"):
             if has_key_word.match(line):
                 content_count += 1
-        self.assertTrue(content_count > 0)
+        self.assertGreater(content_count, 0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_surface_distance.py` & `monai_weekly-1.4.dev2417/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_tb_image.py` & `monai_weekly-1.4.dev2417/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_tb_stats.py` & `monai_weekly-1.4.dev2417/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_handler_validation.py` & `monai_weekly-1.4.dev2417/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hardnegsampler.py` & `monai_weekly-1.4.dev2417/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hashing.py` & `monai_weekly-1.4.dev2417/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hausdorff_distance.py` & `monai_weekly-1.4.dev2417/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hausdorff_loss.py` & `monai_weekly-1.4.dev2417/tests/test_hausdorff_loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,25 +215,20 @@
         chn_input = torch.ones((1, 1, 3))
         chn_target = torch.ones((1, 1, 3))
         with self.assertRaisesRegex(ValueError, ""):
             HausdorffDTLoss(reduction="unknown")(chn_input, chn_target)
         with self.assertRaisesRegex(ValueError, ""):
             HausdorffDTLoss(reduction=None)(chn_input, chn_target)
 
-    def test_input_warnings(self):
+    @parameterized.expand([(False, False, False), (False, True, False), (False, False, True)])
+    def test_input_warnings(self, include_background, softmax, to_onehot_y):
         chn_input = torch.ones((1, 1, 1, 3))
         chn_target = torch.ones((1, 1, 1, 3))
         with self.assertWarns(Warning):
-            loss = HausdorffDTLoss(include_background=False)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = HausdorffDTLoss(softmax=True)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = HausdorffDTLoss(to_onehot_y=True)
+            loss = HausdorffDTLoss(include_background=include_background, softmax=softmax, to_onehot_y=to_onehot_y)
             loss.forward(chn_input, chn_target)
 
 
 @skipUnless(has_scipy, "Scipy required")
 class TesLogtHausdorffDTLoss(unittest.TestCase):
 
     @parameterized.expand(TEST_CASES_LOG, doc_func=_describe_test_case)
@@ -252,23 +247,18 @@
         chn_input = torch.ones((1, 1, 3))
         chn_target = torch.ones((1, 1, 3))
         with self.assertRaisesRegex(ValueError, ""):
             LogHausdorffDTLoss(reduction="unknown")(chn_input, chn_target)
         with self.assertRaisesRegex(ValueError, ""):
             LogHausdorffDTLoss(reduction=None)(chn_input, chn_target)
 
-    def test_input_warnings(self):
+    @parameterized.expand([(False, False, False), (False, True, False), (False, False, True)])
+    def test_input_warnings(self, include_background, softmax, to_onehot_y):
         chn_input = torch.ones((1, 1, 1, 3))
         chn_target = torch.ones((1, 1, 1, 3))
         with self.assertWarns(Warning):
-            loss = LogHausdorffDTLoss(include_background=False)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = LogHausdorffDTLoss(softmax=True)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = LogHausdorffDTLoss(to_onehot_y=True)
+            loss = LogHausdorffDTLoss(include_background=include_background, softmax=softmax, to_onehot_y=to_onehot_y)
             loss.forward(chn_input, chn_target)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_header_correct.py` & `monai_weekly-1.4.dev2417/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_highresnet.py` & `monai_weekly-1.4.dev2417/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hilbert_transform.py` & `monai_weekly-1.4.dev2417/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_histogram_normalize.py` & `monai_weekly-1.4.dev2417/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_histogram_normalized.py` & `monai_weekly-1.4.dev2417/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet_instance_map_post_processing.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet_instance_map_post_processingd.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet_loss.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet_nuclear_type_post_processing.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai_weekly-1.4.dev2417/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_identity.py` & `monai_weekly-1.4.dev2417/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_identityd.py` & `monai_weekly-1.4.dev2417/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_image_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_image_filter.py` & `monai_weekly-1.4.dev2417/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_image_rw.py` & `monai_weekly-1.4.dev2417/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_img2tensorboard.py` & `monai_weekly-1.4.dev2417/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_init_reader.py` & `monai_weekly-1.4.dev2417/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_autorunner.py` & `monai_weekly-1.4.dev2417/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_bundle_run.py` & `monai_weekly-1.4.dev2417/tests/test_integration_bundle_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,30 +131,28 @@
 
         cmd = ["coverage", "run", "-m", "monai.bundle"]
         # test both CLI entry "run" and "run_workflow"
         expected_condition = "successfully added scripts fold!"
         command_run = cmd + ["run", "training", "--config_file", config_file, "--meta_file", meta_file]
         completed_process = subprocess.run(command_run, check=True, capture_output=True, text=True)
         output = repr(completed_process.stdout).replace("\\n", "\n").replace("\\t", "\t")  # Get the captured output
-        print(output)
 
-        self.assertTrue(expected_condition in output)
+        self.assertIn(expected_condition, output)
         command_run_workflow = cmd + [
             "run_workflow",
             "--run_id",
             "training",
             "--config_file",
             config_file,
             "--meta_file",
             meta_file,
         ]
         completed_process = subprocess.run(command_run_workflow, check=True, capture_output=True, text=True)
         output = repr(completed_process.stdout).replace("\\n", "\n").replace("\\t", "\t")  # Get the captured output
-        print(output)
-        self.assertTrue(expected_condition in output)
+        self.assertIn(expected_condition, output)
 
         # test missing meta file
         self.assertIn("ERROR", command_line_tests(cmd + ["run", "training", "--config_file", config_file]))
 
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     def test_shape(self, config_file, expected_shape):
         test_image = np.random.rand(*expected_shape)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_classification_2d.py` & `monai_weekly-1.4.dev2417/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_determinism.py` & `monai_weekly-1.4.dev2417/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_fast_train.py` & `monai_weekly-1.4.dev2417/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_gpu_customization.py` & `monai_weekly-1.4.dev2417/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_lazy_samples.py` & `monai_weekly-1.4.dev2417/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_nnunetv2_runner.py` & `monai_weekly-1.4.dev2417/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_segmentation_3d.py` & `monai_weekly-1.4.dev2417/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_sliding_window.py` & `monai_weekly-1.4.dev2417/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_stn.py` & `monai_weekly-1.4.dev2417/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_unet_2d.py` & `monai_weekly-1.4.dev2417/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_workers.py` & `monai_weekly-1.4.dev2417/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_workflows.py` & `monai_weekly-1.4.dev2417/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_integration_workflows_gan.py` & `monai_weekly-1.4.dev2417/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_intensity_stats.py` & `monai_weekly-1.4.dev2417/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_intensity_statsd.py` & `monai_weekly-1.4.dev2417/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_inverse.py` & `monai_weekly-1.4.dev2417/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_inverse_array.py` & `monai_weekly-1.4.dev2417/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_inverse_collation.py` & `monai_weekly-1.4.dev2417/tests/test_inverse_collation.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         for item in loader:
             if isinstance(item, dict):
                 np.testing.assert_array_equal(item["image"].shape, item["label"].shape)
                 continue
             d = decollate_batch(item)
             self.assertTrue(len(d) <= self.batch_size)
             for b in d:
-                self.assertTrue(isinstance(b["image"], MetaTensor))
+                self.assertIsInstance(b["image"], MetaTensor)
                 np.testing.assert_array_equal(
                     b["image"].applied_operations[-1]["orig_size"], b["label"].applied_operations[-1]["orig_size"]
                 )
                 np.testing.assert_array_equal(
                     b["image"].applied_operations[-1].get("_do_transform"),
                     b["label"].applied_operations[-1].get("_do_transform"),
                 )
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_invert.py` & `monai_weekly-1.4.dev2417/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_invertd.py` & `monai_weekly-1.4.dev2417/tests/test_invertd.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,14 @@
         reverted_name = item["label_inverted"].meta["filename_or_obj"]
         original_name = data[-1]["label"]
         self.assertEqual(reverted_name, original_name)
         print("invert diff", reverted.size - n_good)
         # 25300: 2 workers (cpu, non-macos)
         # 1812: 0 workers (gpu or macos)
         # 1821: windows torch 1.10.0
-        self.assertTrue((reverted.size - n_good) < 40000, f"diff.  {reverted.size - n_good}")
+        self.assertLess((reverted.size - n_good), 40000, f"diff.  {reverted.size - n_good}")
 
         set_determinism(seed=None)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_is_supported_format.py` & `monai_weekly-1.4.dev2417/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_iterable_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_itk_torch_bridge.py` & `monai_weekly-1.4.dev2417/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_itk_writer.py` & `monai_weekly-1.4.dev2417/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_k_space_spike_noise.py` & `monai_weekly-1.4.dev2417/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_k_space_spike_noised.py` & `monai_weekly-1.4.dev2417/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_keep_largest_connected_component.py` & `monai_weekly-1.4.dev2417/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_keep_largest_connected_componentd.py` & `monai_weekly-1.4.dev2417/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_kspace_mask.py` & `monai_weekly-1.4.dev2417/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_filter.py` & `monai_weekly-1.4.dev2417/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_filterd.py` & `monai_weekly-1.4.dev2417/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_quality_score.py` & `monai_weekly-1.4.dev2417/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_to_contour.py` & `monai_weekly-1.4.dev2417/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_to_contourd.py` & `monai_weekly-1.4.dev2417/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_to_mask.py` & `monai_weekly-1.4.dev2417/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_label_to_maskd.py` & `monai_weekly-1.4.dev2417/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lambda.py` & `monai_weekly-1.4.dev2417/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lambdad.py` & `monai_weekly-1.4.dev2417/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lesion_froc.py` & `monai_weekly-1.4.dev2417/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_list_data_collate.py` & `monai_weekly-1.4.dev2417/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_list_to_dict.py` & `monai_weekly-1.4.dev2417/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lltm.py` & `monai_weekly-1.4.dev2417/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lmdbdataset.py` & `monai_weekly-1.4.dev2417/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lmdbdataset_dist.py` & `monai_weekly-1.4.dev2417/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_load_decathlon_datalist.py` & `monai_weekly-1.4.dev2417/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_load_image.py` & `monai_weekly-1.4.dev2417/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_load_imaged.py` & `monai_weekly-1.4.dev2417/tests/test_load_imaged.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             r = result[key]
             self.assertTupleEqual(r.shape, expected_shape)
             if track_meta:
                 self.assertIsInstance(r, MetaTensor)
                 self.assertTrue(hasattr(r, "affine"))
                 self.assertIsInstance(r.affine, torch.Tensor)
                 self.assertEqual(r.meta["space"], "RAS")
-                self.assertTrue("qform_code" not in r.meta)
+                self.assertNotIn("qform_code", r.meta)
             else:
                 self.assertIsInstance(r, torch.Tensor)
                 self.assertNotIsInstance(r, MetaTensor)
                 self.assertFalse(hasattr(r, "affine"))
 
 
 if __name__ == "__main__":
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_load_spacing_orientation.py` & `monai_weekly-1.4.dev2417/tests/test_load_spacing_orientation.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         res_dict = Spacingd(keys="image", pixdim=(1, 0.2, 1), diagonal=True, padding_mode="zeros")(data_dict)
         t1 = time.time()
         print(f"time monai: {t1 - t}")
         anat = nibabel.Nifti1Image(np.asarray(data_dict["image"][0]), data_dict["image"].meta["original_affine"])
         ref = resample_to_output(anat, (1, 0.2, 1), order=1)
         t2 = time.time()
         print(f"time scipy: {t2 - t1}")
-        self.assertTrue(t2 >= t1)
+        self.assertGreaterEqual(t2, t1)
         np.testing.assert_allclose(res_dict["image"].affine, ref.affine)
         np.testing.assert_allclose(res_dict["image"].shape[1:], ref.shape)
         np.testing.assert_allclose(ref.get_fdata(), res_dict["image"][0], atol=0.05)
 
     @parameterized.expand(FILES)
     def test_load_spacingd_rotate(self, filename):
         data_dict = self.load_image(filename)
@@ -64,15 +64,15 @@
         res_dict = Spacingd(keys="image", pixdim=(1, 2, 3), diagonal=True, padding_mode="zeros")(data_dict)
         t1 = time.time()
         print(f"time monai: {t1 - t}")
         anat = nibabel.Nifti1Image(np.asarray(data_dict["image"][0]), data_dict["image"].meta["original_affine"])
         ref = resample_to_output(anat, (1, 2, 3), order=1)
         t2 = time.time()
         print(f"time scipy: {t2 - t1}")
-        self.assertTrue(t2 >= t1)
+        self.assertGreaterEqual(t2, t1)
         np.testing.assert_allclose(res_dict["image"].affine, ref.affine)
         if "anatomical" not in filename:
             np.testing.assert_allclose(res_dict["image"].shape[1:], ref.shape)
             np.testing.assert_allclose(ref.get_fdata(), res_dict["image"][0], atol=0.05)
         else:
             # different from the ref implementation (shape computed by round
             # instead of ceil)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_loader_semaphore.py` & `monai_weekly-1.4.dev2417/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_local_normalized_cross_correlation_loss.py` & `monai_weekly-1.4.dev2417/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_localnet.py` & `monai_weekly-1.4.dev2417/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_localnet_block.py` & `monai_weekly-1.4.dev2417/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_look_up_option.py` & `monai_weekly-1.4.dev2417/tests/test_look_up_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def test_default(self):
         output = look_up_option("not here", {"a", "b"}, default=None)
         self.assertEqual(output, None)
 
     def test_str_enum(self):
         output = look_up_option("C", {"A", "B"}, default=None)
-        self.assertEqual(output, None)
+        self.assertIsNone(output)
         self.assertEqual(list(_CaseStrEnum), ["A", "B"])
         self.assertEqual(_CaseStrEnum.MODE_A, "A")
         self.assertEqual(str(_CaseStrEnum.MODE_A), "A")
         self.assertEqual(look_up_option("A", _CaseStrEnum), "A")
 
     def test_no_found(self):
         with self.assertRaisesRegex(ValueError, "Unsupported"):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_loss_metric.py` & `monai_weekly-1.4.dev2417/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lr_finder.py` & `monai_weekly-1.4.dev2417/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_lr_scheduler.py` & `monai_weekly-1.4.dev2417/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_make_nifti.py` & `monai_weekly-1.4.dev2417/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_map_binary_to_indices.py` & `monai_weekly-1.4.dev2417/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_map_classes_to_indices.py` & `monai_weekly-1.4.dev2417/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_map_label_value.py` & `monai_weekly-1.4.dev2417/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_map_label_valued.py` & `monai_weekly-1.4.dev2417/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_map_transform.py` & `monai_weekly-1.4.dev2417/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mask_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mask_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_masked_dice_loss.py` & `monai_weekly-1.4.dev2417/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_masked_loss.py` & `monai_weekly-1.4.dev2417/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_masked_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_matshow3d.py` & `monai_weekly-1.4.dev2417/tests/test_matshow3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         )
         image_path = os.path.join(testing_dir, "anatomical.nii")
         xforms.set_random_state(0)
         ims = xforms({keys: image_path})
         fig, mat = matshow3d(
             [im[keys] for im in ims], title=f"testing {keys}", figsize=(2, 2), frames_per_row=5, every_n=2, show=False
         )
-        self.assertTrue(mat.dtype == np.float32)
+        self.assertEqual(mat.dtype, np.float32)
 
         with tempfile.TemporaryDirectory() as tempdir:
             tempimg = f"{tempdir}/matshow3d_patch_test.png"
             fig.savefig(tempimg)
             comp = compare_images(f"{testing_dir}/matshow3d_patch_test.png", tempimg, 5e-2, in_decorator=True)
             if comp:
                 print("not none comp: ", comp)  # matplotlib 3.2.2
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_mean_ensemble.py` & `monai_weekly-1.4.dev2417/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mean_ensembled.py` & `monai_weekly-1.4.dev2417/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_median_smooth.py` & `monai_weekly-1.4.dev2417/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_median_smoothd.py` & `monai_weekly-1.4.dev2417/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mednistdataset.py` & `monai_weekly-1.4.dev2417/tests/test_mednistdataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             ]
         )
 
         def _test_dataset(dataset):
             self.assertEqual(len(dataset), int(MEDNIST_FULL_DATASET_LENGTH * dataset.test_frac))
             self.assertTrue("image" in dataset[0])
             self.assertTrue("label" in dataset[0])
-            self.assertTrue(isinstance(dataset[0]["image"], MetaTensor))
+            self.assertIsInstance(dataset[0]["image"], MetaTensor)
             self.assertTupleEqual(dataset[0]["image"].shape, (1, 64, 64))
 
         with skip_if_downloading_fails():
             data = MedNISTDataset(
                 root_dir=testing_dir, transform=transform, section="test", download=True, copy_cache=False
             )
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_meta_affine.py` & `monai_weekly-1.4.dev2417/tests/test_meta_affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,27 +156,27 @@
         ref_2 = _create_itk_obj(output[0], output.affine)
         assert_allclose(output.pixdim, np.asarray(ref_2.GetSpacing()), type_test=False)
         expected = _resample_to_affine(ref_1, ref_2)
         # compare ref_2 and expected results from itk
         diff = np.abs(itk.GetArrayFromImage(ref_2) - itk.GetArrayFromImage(expected))
         avg_diff = np.mean(diff)
 
-        self.assertTrue(avg_diff < atol, f"{xform_cls} avg_diff: {avg_diff}, tol: {atol}")
+        self.assertLess(avg_diff, atol, f"{xform_cls} avg_diff: {avg_diff}, tol: {atol}")
 
     @parameterized.expand(TEST_CASES_DICT)
     def test_linear_consistent_dict(self, xform_cls, input_dict, atol):
         """xform cls testing itk consistency"""
         img = LoadImaged(keys, image_only=True, simple_keys=True)({keys[0]: FILE_PATH, keys[1]: FILE_PATH_1})
         img = EnsureChannelFirstd(keys)(img)
         ref_1 = {k: _create_itk_obj(img[k][0], img[k].affine) for k in keys}
         output = self.run_transform(img, xform_cls, input_dict)
         ref_2 = {k: _create_itk_obj(output[k][0], output[k].affine) for k in keys}
         expected = {k: _resample_to_affine(ref_1[k], ref_2[k]) for k in keys}
         # compare ref_2 and expected results from itk
         diff = {k: np.abs(itk.GetArrayFromImage(ref_2[k]) - itk.GetArrayFromImage(expected[k])) for k in keys}
         avg_diff = {k: np.mean(diff[k]) for k in keys}
         for k in keys:
-            self.assertTrue(avg_diff[k] < atol, f"{xform_cls} avg_diff: {avg_diff}, tol: {atol}")
+            self.assertLess(avg_diff[k], atol, f"{xform_cls} avg_diff: {avg_diff}, tol: {atol}")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_meta_tensor.py` & `monai_weekly-1.4.dev2417/tests/test_meta_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,17 +218,17 @@
         orig_affine = ims[0].meta.pop("affine")
         stacked_affine = stacked.meta.pop("affine")
         assert_allclose(orig_affine, stacked_affine)
         self.assertEqual(stacked.meta, ims[0].meta)
 
     def test_get_set_meta_fns(self):
         set_track_meta(False)
-        self.assertEqual(get_track_meta(), False)
+        self.assertFalse(get_track_meta())
         set_track_meta(True)
-        self.assertEqual(get_track_meta(), True)
+        self.assertTrue(get_track_meta())
 
     @parameterized.expand(TEST_DEVICES)
     def test_torchscript(self, device):
         shape = (1, 3, 10, 8)
         im, _ = self.get_im(shape, device=device)
         conv = torch.nn.Conv2d(im.shape[1], 5, 3)
         conv.to(device)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_metatensor_integration.py` & `monai_weekly-1.4.dev2417/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_metrics_reloaded.py` & `monai_weekly-1.4.dev2417/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_milmodel.py` & `monai_weekly-1.4.dev2417/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mlp.py` & `monai_weekly-1.4.dev2417/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mmar_download.py` & `monai_weekly-1.4.dev2417/tests/test_mmar_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self.assertEqual(output.__class__.__name__, expected_name)
         x = next(output.parameters())  # verify the first element
         np.testing.assert_allclose(x[0][0].detach().cpu().numpy(), expected_val, rtol=1e-3, atol=1e-3)
 
     def test_unique(self):
         # model ids are unique
         keys = sorted(m["id"] for m in MODEL_DESC)
-        self.assertTrue(keys == sorted(set(keys)))
+        self.assertEqual(keys, sorted(set(keys)))
 
     def test_search(self):
         self.assertEqual(_get_val({"a": 1, "b": 2}, key="b"), 2)
         self.assertEqual(_get_val({"a": {"c": {"c": 4}}, "b": {"c": 2}}, key="b"), {"c": 2})
         self.assertEqual(_get_val({"a": {"c": 4}, "b": {"c": 2}}, key="c"), 4)
         self.assertEqual(_get_val({"a": {"c": None}, "b": {"c": 2}}, key="c"), 2)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_module_list.py` & `monai_weekly-1.4.dev2417/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_monai_env_vars.py` & `monai_weekly-1.4.dev2417/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_monai_utils_misc.py` & `monai_weekly-1.4.dev2417/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_mri_utils.py` & `monai_weekly-1.4.dev2417/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_multi_scale.py` & `monai_weekly-1.4.dev2417/tests/test_multi_scale.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,25 +54,32 @@
 class TestMultiScale(unittest.TestCase):
 
     @parameterized.expand(TEST_CASES)
     def test_shape(self, input_param, input_data, expected_val):
         result = MultiScaleLoss(**input_param).forward(**input_data)
         np.testing.assert_allclose(result.detach().cpu().numpy(), expected_val, rtol=1e-5)
 
-    def test_ill_opts(self):
-        with self.assertRaisesRegex(ValueError, ""):
-            MultiScaleLoss(loss=dice_loss, kernel="none")
-        with self.assertRaisesRegex(ValueError, ""):
-            MultiScaleLoss(loss=dice_loss, scales=[-1])(
-                torch.ones((1, 1, 3), device=device), torch.ones((1, 1, 3), device=device)
-            )
-        with self.assertRaisesRegex(ValueError, ""):
-            MultiScaleLoss(loss=dice_loss, scales=[-1], reduction="none")(
-                torch.ones((1, 1, 3), device=device), torch.ones((1, 1, 3), device=device)
-            )
+    @parameterized.expand(
+        [
+            ({"loss": dice_loss, "kernel": "none"}, None, None),  # kernel_none
+            ({"loss": dice_loss, "scales": [-1]}, torch.ones((1, 1, 3)), torch.ones((1, 1, 3))),  # scales_negative
+            (
+                {"loss": dice_loss, "scales": [-1], "reduction": "none"},
+                torch.ones((1, 1, 3)),
+                torch.ones((1, 1, 3)),
+            ),  # scales_negative_reduction_none
+        ]
+    )
+    def test_ill_opts(self, kwargs, input, target):
+        if input is None and target is None:
+            with self.assertRaisesRegex(ValueError, ""):
+                MultiScaleLoss(**kwargs)
+        else:
+            with self.assertRaisesRegex(ValueError, ""):
+                MultiScaleLoss(**kwargs)(input, target)
 
     def test_script(self):
         input_param, input_data, expected_val = TEST_CASES[0]
         loss = MultiScaleLoss(**input_param)
         test_script_save(loss, input_data["y_pred"], input_data["y_true"])
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_net_adapter.py` & `monai_weekly-1.4.dev2417/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_network_consistency.py` & `monai_weekly-1.4.dev2417/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nifti_endianness.py` & `monai_weekly-1.4.dev2417/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nifti_header_revise.py` & `monai_weekly-1.4.dev2417/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nifti_rw.py` & `monai_weekly-1.4.dev2417/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_normalize_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_normalize_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_npzdictitemdataset.py` & `monai_weekly-1.4.dev2417/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nrrd_reader.py` & `monai_weekly-1.4.dev2417/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nuclick_transforms.py` & `monai_weekly-1.4.dev2417/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_numpy_reader.py` & `monai_weekly-1.4.dev2417/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nvtx_decorator.py` & `monai_weekly-1.4.dev2417/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_nvtx_transform.py` & `monai_weekly-1.4.dev2417/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_occlusion_sensitivity.py` & `monai_weekly-1.4.dev2417/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_one_of.py` & `monai_weekly-1.4.dev2417/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_optim_novograd.py` & `monai_weekly-1.4.dev2417/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_optional_import.py` & `monai_weekly-1.4.dev2417/tests/test_optional_import.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
+from parameterized import parameterized
+
 from monai.utils import OptionalImportError, exact_version, optional_import
 
 
 class TestOptionalImport(unittest.TestCase):
 
-    def test_default(self):
-        my_module, flag = optional_import("not_a_module")
+    @parameterized.expand(["not_a_module", "torch.randint"])
+    def test_default(self, import_module):
+        my_module, flag = optional_import(import_module)
         self.assertFalse(flag)
         with self.assertRaises(OptionalImportError):
             my_module.test
 
-        my_module, flag = optional_import("torch.randint")
-        with self.assertRaises(OptionalImportError):
-            self.assertFalse(flag)
-            print(my_module.test)
-
     def test_import_valid(self):
         my_module, flag = optional_import("torch")
         self.assertTrue(flag)
         print(my_module.randint(1, 2, (1, 2)))
 
     def test_import_wrong_number(self):
         my_module, flag = optional_import("torch", "42")
@@ -43,26 +41,17 @@
             my_module.randint(1, 2, (1, 2))
         with self.assertRaisesRegex(ValueError, "invalid literal"):
             my_module, flag = optional_import("torch", "test")  # version should be number.number
             my_module.nn
             self.assertTrue(flag)
             print(my_module.randint(1, 2, (1, 2)))
 
-    def test_import_good_number(self):
-        my_module, flag = optional_import("torch", "0")
-        my_module.nn
-        self.assertTrue(flag)
-        print(my_module.randint(1, 2, (1, 2)))
-
-        my_module, flag = optional_import("torch", "0.0.0.1")
-        my_module.nn
-        self.assertTrue(flag)
-        print(my_module.randint(1, 2, (1, 2)))
-
-        my_module, flag = optional_import("torch", "1.1.0")
+    @parameterized.expand(["0", "0.0.0.1", "1.1.0"])
+    def test_import_good_number(self, version_number):
+        my_module, flag = optional_import("torch", version_number)
         my_module.nn
         self.assertTrue(flag)
         print(my_module.randint(1, 2, (1, 2)))
 
     def test_import_exact(self):
         my_module, flag = optional_import("torch", "0", exact_version)
         with self.assertRaisesRegex(OptionalImportError, "exact_version"):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_ori_ras_lps.py` & `monai_weekly-1.4.dev2417/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_orientation.py` & `monai_weekly-1.4.dev2417/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_orientationd.py` & `monai_weekly-1.4.dev2417/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_p3d_block.py` & `monai_weekly-1.4.dev2417/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pad_collation.py` & `monai_weekly-1.4.dev2417/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pad_mode.py` & `monai_weekly-1.4.dev2417/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_partition_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_partition_dataset_classes.py` & `monai_weekly-1.4.dev2417/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_patch_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_patch_inferer.py` & `monai_weekly-1.4.dev2417/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_patchembedding.py` & `monai_weekly-1.4.dev2417/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pathology_he_stain.py` & `monai_weekly-1.4.dev2417/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pathology_he_stain_dict.py` & `monai_weekly-1.4.dev2417/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pathology_prob_nms.py` & `monai_weekly-1.4.dev2417/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_perceptual_loss.py` & `monai_weekly-1.4.dev2417/tests/test_perceptual_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,17 +109,15 @@
         with self.assertRaises(ValueError):
             loss(tensor, target)
 
     def test_1d(self):
         with self.assertRaises(NotImplementedError):
             PerceptualLoss(spatial_dims=1)
 
-    def test_medicalnet_on_2d_data(self):
+    @parameterized.expand(["medicalnet_resnet10_23datasets", "medicalnet_resnet50_23datasets"])
+    def test_medicalnet_on_2d_data(self, network_type):
         with self.assertRaises(ValueError):
-            PerceptualLoss(spatial_dims=2, network_type="medicalnet_resnet10_23datasets")
-
-        with self.assertRaises(ValueError):
-            PerceptualLoss(spatial_dims=2, network_type="medicalnet_resnet50_23datasets")
+            PerceptualLoss(spatial_dims=2, network_type=network_type)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_persistentdataset.py` & `monai_weekly-1.4.dev2417/tests/test_persistentdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,12 +161,12 @@
         """
         shape = (1, 10, 9, 8)
         im = np.arange(0, np.prod(shape)).reshape(shape)
         with tempfile.TemporaryDirectory() as path:
             im1 = PersistentDataset([im], Identity(), cache_dir=path, hash_transform=json_hashing)[0]
             im2 = PersistentDataset([im], Flip(1), cache_dir=path, hash_transform=json_hashing)[0]
             l2 = ((im1 - im2) ** 2).sum() ** 0.5
-            self.assertTrue(l2 > 1)
+            self.assertGreater(l2, 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_persistentdataset_dist.py` & `monai_weekly-1.4.dev2417/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_phl_cpu.py` & `monai_weekly-1.4.dev2417/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_phl_cuda.py` & `monai_weekly-1.4.dev2417/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pil_reader.py` & `monai_weekly-1.4.dev2417/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_plot_2d_or_3d_image.py` & `monai_weekly-1.4.dev2417/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_png_rw.py` & `monai_weekly-1.4.dev2417/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_polyval.py` & `monai_weekly-1.4.dev2417/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_prepare_batch_default_dist.py` & `monai_weekly-1.4.dev2417/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_prepare_batch_extra_input.py` & `monai_weekly-1.4.dev2417/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_prepare_batch_hovernet.py` & `monai_weekly-1.4.dev2417/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_preset_filters.py` & `monai_weekly-1.4.dev2417/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_print_info.py` & `monai_weekly-1.4.dev2417/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_print_transform_backends.py` & `monai_weekly-1.4.dev2417/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_probnms.py` & `monai_weekly-1.4.dev2417/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_probnmsd.py` & `monai_weekly-1.4.dev2417/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_profiling.py` & `monai_weekly-1.4.dev2417/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_pytorch_version_after.py` & `monai_weekly-1.4.dev2417/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_query_memory.py` & `monai_weekly-1.4.dev2417/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_quicknat.py` & `monai_weekly-1.4.dev2417/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_adjust_contrast.py` & `monai_weekly-1.4.dev2417/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_adjust_contrastd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_affine.py` & `monai_weekly-1.4.dev2417/tests/test_rand_affine.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,19 +148,18 @@
         result = g(**input_data)
         g.rand_affine_grid.affine = torch.eye(4, dtype=torch.float64)  # reset affine
         test_resampler_lazy(g, result, input_param, input_data, seed=123, rtol=_rtol)
         if input_param.get("cache_grid", False):
             self.assertTrue(g._cached_grid is not None)
         assert_allclose(result, expected_val, rtol=_rtol, atol=1e-4, type_test="tensor")
 
-    def test_ill_cache(self):
+    @parameterized.expand([(None,), ((1, 1, -1),)])
+    def test_ill_cache(self, spatial_size):
         with self.assertWarns(UserWarning):
-            RandAffine(cache_grid=True)
-        with self.assertWarns(UserWarning):
-            RandAffine(cache_grid=True, spatial_size=(1, 1, -1))
+            RandAffine(cache_grid=True, spatial_size=spatial_size)
 
     @parameterized.expand(TEST_CASES_SKIPPED_CONSISTENCY)
     def test_skipped_transform_consistency(self, im, in_dtype):
         t1 = RandAffine(prob=0)
         t2 = RandAffine(prob=1, spatial_size=(10, 11))
 
         im, *_ = convert_data_type(im, dtype=in_dtype)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_affine_grid.py` & `monai_weekly-1.4.dev2417/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_affined.py` & `monai_weekly-1.4.dev2417/tests/test_rand_affined.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 expected_output = resampler(**call_param)
                 test_resampler_lazy(
                     resampler, expected_output, lazy_init_param, call_param, seed=123, output_key=key, rtol=_rtol
                 )
             resampler.lazy = False
 
         if input_param.get("cache_grid", False):
-            self.assertTrue(g.rand_affine._cached_grid is not None)
+            self.assertIsNotNone(g.rand_affine._cached_grid)
         for key in res:
             if isinstance(key, str) and key.endswith("_transforms"):
                 continue
             result = res[key]
             if track_meta:
                 self.assertIsInstance(result, MetaTensor)
                 self.assertEqual(len(result.applied_operations), 1)
@@ -268,18 +268,15 @@
 
         res_inv = g.inverse(res)
         for k, v in res_inv.items():
             self.assertIsInstance(v, MetaTensor)
             self.assertEqual(len(v.applied_operations), 0)
             self.assertTupleEqual(v.shape, input_data[k].shape)
 
-    def test_ill_cache(self):
+    @parameterized.expand([(None,), ((2, -1),)])  # spatial size is None  # spatial size is dynamic
+    def test_ill_cache(self, spatial_size):
         with self.assertWarns(UserWarning):
-            # spatial size is None
-            RandAffined(device=device, spatial_size=None, prob=1.0, cache_grid=True, keys=("img", "seg"))
-        with self.assertWarns(UserWarning):
-            # spatial size is dynamic
-            RandAffined(device=device, spatial_size=(2, -1), prob=1.0, cache_grid=True, keys=("img", "seg"))
+            RandAffined(device=device, spatial_size=spatial_size, prob=1.0, cache_grid=True, keys=("img", "seg"))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_axis_flip.py` & `monai_weekly-1.4.dev2417/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_axis_flipd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_bias_field.py` & `monai_weekly-1.4.dev2417/tests/test_rand_bias_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def test_output_shape(self, class_args, img_shape):
         for p in TEST_NDARRAYS:
             for degree in [1, 2, 3]:
                 bias_field = RandBiasField(degree=degree, **class_args)
                 img = p(np.random.rand(*img_shape))
                 output = bias_field(img)
                 np.testing.assert_equal(output.shape, img_shape)
-                self.assertTrue(output.dtype in (np.float32, torch.float32))
+                self.assertIn(output.dtype, (np.float32, torch.float32))
 
                 img_zero = np.zeros([*img_shape])
                 output_zero = bias_field(img_zero)
                 np.testing.assert_equal(output_zero, img_zero)
 
     @parameterized.expand([TEST_CASES_2D_ZERO_RANGE])
     def test_zero_range(self, class_args, img_shape):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_bias_fieldd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_coarse_dropout.py` & `monai_weekly-1.4.dev2417/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_coarse_dropoutd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_coarse_shuffle.py` & `monai_weekly-1.4.dev2417/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_coarse_shuffled.py` & `monai_weekly-1.4.dev2417/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_crop_by_label_classes.py` & `monai_weekly-1.4.dev2417/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_crop_by_label_classesd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_crop_by_pos_neg_label.py` & `monai_weekly-1.4.dev2417/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai_weekly-1.4.dev2417/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_cucim_dict_transform.py` & `monai_weekly-1.4.dev2417/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_cucim_transform.py` & `monai_weekly-1.4.dev2417/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_deform_grid.py` & `monai_weekly-1.4.dev2417/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_elastic_2d.py` & `monai_weekly-1.4.dev2417/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_elastic_3d.py` & `monai_weekly-1.4.dev2417/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_elasticd_2d.py` & `monai_weekly-1.4.dev2417/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_elasticd_3d.py` & `monai_weekly-1.4.dev2417/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_flip.py` & `monai_weekly-1.4.dev2417/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_flipd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_noise.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_noised.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_sharpen.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_sharpend.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_smooth.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gaussian_smoothd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gibbs_noise.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_gibbs_noised.py` & `monai_weekly-1.4.dev2417/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_grid_distortion.py` & `monai_weekly-1.4.dev2417/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_grid_distortiond.py` & `monai_weekly-1.4.dev2417/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_grid_patch.py` & `monai_weekly-1.4.dev2417/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_grid_patchd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_histogram_shift.py` & `monai_weekly-1.4.dev2417/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_histogram_shiftd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_k_space_spike_noise.py` & `monai_weekly-1.4.dev2417/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_k_space_spike_noised.py` & `monai_weekly-1.4.dev2417/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_lambda.py` & `monai_weekly-1.4.dev2417/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_lambdad.py` & `monai_weekly-1.4.dev2417/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rician_noise.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rician_noised.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rotate.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rotate90.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rotate90d.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_rotated.py` & `monai_weekly-1.4.dev2417/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_crop.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_intensity_fixed_meand.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_scale_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_shift_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_shift_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_simulate_low_resolution.py` & `monai_weekly-1.4.dev2417/tests/test_rand_simulate_low_resolution.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_simulate_low_resolutiond.py` & `monai_weekly-1.4.dev2417/tests/test_rand_simulate_low_resolutiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop.py` & `monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop_samples.py` & `monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_spatial_crop_samplesd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_spatial_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_std_shift_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_std_shift_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_weighted_crop.py` & `monai_weekly-1.4.dev2417/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_weighted_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_weighted_cropd.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 class TestRandWeightedCrop(unittest.TestCase):
 
     @parameterized.expand(TESTS)
     def test_rand_weighted_cropd(self, _, init_params, input_data, expected_shape, expected_centers):
         crop = RandWeightedCropd(**init_params)
         crop.set_random_state(10)
         result = crop(input_data)
-        self.assertTrue(len(result) == init_params["num_samples"])
+        self.assertEqual(len(result), init_params["num_samples"])
         _len = len(tuple(input_data.keys()))
         self.assertTupleEqual(tuple(result[0].keys())[:_len], tuple(input_data.keys()))
 
     @parameterized.expand(TESTS)
     def test_pending_ops(self, _, input_param, input_data, expected_shape, expected_centers):
         crop = RandWeightedCropd(**input_param)
         # non-lazy
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_zoom.py` & `monai_weekly-1.4.dev2417/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rand_zoomd.py` & `monai_weekly-1.4.dev2417/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_randidentity.py` & `monai_weekly-1.4.dev2417/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_random_order.py` & `monai_weekly-1.4.dev2417/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_randomizable.py` & `monai_weekly-1.4.dev2417/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_randomizable_transform_type.py` & `monai_weekly-1.4.dev2417/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_randtorchvisiond.py` & `monai_weekly-1.4.dev2417/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rankfilter_dist.py` & `monai_weekly-1.4.dev2417/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_recon_net_utils.py` & `monai_weekly-1.4.dev2417/tests/test_recon_net_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         result = reshape_batch_channel_to_channel_dim(result, batch_size)
         self.assertEqual(result.shape, test_data.shape)
 
     @parameterized.expand(TEST_NORMALIZE)
     def test_complex_normalize(self, test_data):
         result, mean, std = complex_normalize(test_data)
         result = result * std + mean
-        self.assertTrue((((result - test_data) ** 2).mean() ** 0.5).item() < 1e-5)
+        self.assertLess((((result - test_data) ** 2).mean() ** 0.5).item(), 1e-5)
 
     @parameterized.expand(TEST_PAD)
     def test_pad(self, test_data):
         result, padding_sizes = divisible_pad_t(test_data, k=16)
         result = inverse_divisible_pad_t(result, padding_sizes)
         assert_allclose(result, test_data)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_reference_based_normalize_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_reference_based_spatial_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_reference_resolver.py` & `monai_weekly-1.4.dev2417/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_reg_loss_integration.py` & `monai_weekly-1.4.dev2417/tests/test_reg_loss_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,12 +95,12 @@
             loss_val = loss(**{k: loss_input[k] for k in forward_args})
             if it == 0:
                 init_loss = loss_val
 
             # backward pass
             loss_val.backward()
             optimizer.step()
-        self.assertTrue(init_loss > loss_val, "loss did not decrease")
+        self.assertGreater(init_loss, loss_val, "loss did not decrease")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_regularization.py` & `monai_weekly-1.4.dev2417/tests/test_regularization.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_regunet.py` & `monai_weekly-1.4.dev2417/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_regunet_block.py` & `monai_weekly-1.4.dev2417/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_remove_repeated_channel.py` & `monai_weekly-1.4.dev2417/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_remove_repeated_channeld.py` & `monai_weekly-1.4.dev2417/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_remove_small_objects.py` & `monai_weekly-1.4.dev2417/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_repeat_channel.py` & `monai_weekly-1.4.dev2417/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_repeat_channeld.py` & `monai_weekly-1.4.dev2417/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_replace_module.py` & `monai_weekly-1.4.dev2417/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_require_pkg.py` & `monai_weekly-1.4.dev2417/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resample.py` & `monai_weekly-1.4.dev2417/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resample_backends.py` & `monai_weekly-1.4.dev2417/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resample_datalist.py` & `monai_weekly-1.4.dev2417/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resample_to_match.py` & `monai_weekly-1.4.dev2417/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resample_to_matchd.py` & `monai_weekly-1.4.dev2417/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resampler.py` & `monai_weekly-1.4.dev2417/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resize.py` & `monai_weekly-1.4.dev2417/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resize_with_pad_or_crop.py` & `monai_weekly-1.4.dev2417/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resize_with_pad_or_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resized.py` & `monai_weekly-1.4.dev2417/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_resnet.py` & `monai_weekly-1.4.dev2417/tests/test_retinanet_detector.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,268 +7,199 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import copy
-import os
-import re
-import sys
+import random
 import unittest
-from typing import TYPE_CHECKING
 
 import torch
 from parameterized import parameterized
 
-from monai.networks import eval_mode
-from monai.networks.nets import (
-    ResNet,
-    get_medicalnet_pretrained_resnet_args,
-    get_pretrained_resnet_medicalnet,
-    resnet10,
-    resnet18,
-    resnet34,
-    resnet50,
-    resnet101,
-    resnet152,
-    resnet200,
-)
-from monai.networks.nets.resnet import ResNetBlock
+from monai.apps.detection.networks.retinanet_detector import RetinaNetDetector, retinanet_resnet50_fpn_detector
+from monai.apps.detection.utils.anchor_utils import AnchorGeneratorWithAnchorShape
+from monai.networks import eval_mode, train_mode
 from monai.utils import optional_import
-from tests.utils import equal_state_dict, skip_if_downloading_fails, skip_if_no_cuda, skip_if_quick, test_script_save
+from tests.utils import SkipIfBeforePyTorchVersion, skip_if_quick, test_script_save
 
-if TYPE_CHECKING:
-    import torchvision
+_, has_torchvision = optional_import("torchvision")
 
-    has_torchvision = True
-else:
-    torchvision, has_torchvision = optional_import("torchvision")
-
-has_hf_modules = "huggingface_hub" in sys.modules and "huggingface_hub.utils._errors" in sys.modules
-
-# from torchvision.models import ResNet50_Weights, resnet50
-
-device = "cuda" if torch.cuda.is_available() else "cpu"
+num_anchors = 7
 
 TEST_CASE_1 = [  # 3D, batch 3, 2 input channel
     {
         "pretrained": False,
         "spatial_dims": 3,
         "n_input_channels": 2,
         "num_classes": 3,
         "conv1_t_size": 7,
         "conv1_t_stride": (2, 2, 2),
     },
     (3, 2, 32, 64, 48),
-    (3, 3),
 ]
 
 TEST_CASE_2 = [  # 2D, batch 2, 1 input channel
     {
         "pretrained": False,
         "spatial_dims": 2,
         "n_input_channels": 1,
         "num_classes": 3,
         "conv1_t_size": [7, 7],
         "conv1_t_stride": [2, 2],
     },
     (2, 1, 32, 64),
-    (2, 3),
 ]
 
 TEST_CASE_2_A = [  # 2D, batch 2, 1 input channel, shortcut type A
     {
         "pretrained": False,
         "spatial_dims": 2,
         "n_input_channels": 1,
         "num_classes": 3,
         "shortcut_type": "A",
         "conv1_t_size": (7, 7),
         "conv1_t_stride": 2,
     },
     (2, 1, 32, 64),
-    (2, 3),
 ]
 
 TEST_CASE_3 = [  # 1D, batch 1, 2 input channels
     {
         "pretrained": False,
         "spatial_dims": 1,
         "n_input_channels": 2,
         "num_classes": 3,
         "conv1_t_size": [3],
         "conv1_t_stride": 1,
     },
     (1, 2, 32),
-    (1, 3),
 ]
 
 TEST_CASE_3_A = [  # 1D, batch 1, 2 input channels
     {"pretrained": False, "spatial_dims": 1, "n_input_channels": 2, "num_classes": 3, "shortcut_type": "A"},
     (1, 2, 32),
-    (1, 3),
 ]
 
 TEST_CASE_4 = [  # 2D, batch 2, 1 input channel
     {"pretrained": False, "spatial_dims": 2, "n_input_channels": 1, "num_classes": 3, "feed_forward": False},
     (2, 1, 32, 64),
-    ((2, 512), (2, 2048)),
-]
-
-TEST_CASE_5 = [  # 1D, batch 1, 2 input channels
-    {
-        "block": "basic",
-        "layers": [1, 1, 1, 1],
-        "block_inplanes": [64, 128, 256, 512],
-        "spatial_dims": 1,
-        "n_input_channels": 2,
-        "num_classes": 3,
-        "conv1_t_size": [3],
-        "conv1_t_stride": 1,
-    },
-    (1, 2, 32),
-    (1, 3),
-]
-
-TEST_CASE_5_A = [  # 1D, batch 1, 2 input channels
-    {
-        "block": ResNetBlock,
-        "layers": [1, 1, 1, 1],
-        "block_inplanes": [64, 128, 256, 512],
-        "spatial_dims": 1,
-        "n_input_channels": 2,
-        "num_classes": 3,
-        "conv1_t_size": [3],
-        "conv1_t_stride": 1,
-    },
-    (1, 2, 32),
-    (1, 3),
-]
-
-TEST_CASE_6 = [  # 1D, batch 1, 2 input channels
-    {
-        "block": "bottleneck",
-        "layers": [3, 4, 6, 3],
-        "block_inplanes": [64, 128, 256, 512],
-        "spatial_dims": 1,
-        "n_input_channels": 2,
-        "num_classes": 3,
-        "conv1_t_size": [3],
-        "conv1_t_stride": 1,
-    },
-    (1, 2, 32),
-    (1, 3),
-]
-
-TEST_CASE_7 = [  # 1D, batch 1, 2 input channels, bias_downsample
-    {
-        "block": "bottleneck",
-        "layers": [3, 4, 6, 3],
-        "block_inplanes": [64, 128, 256, 512],
-        "spatial_dims": 1,
-        "n_input_channels": 2,
-        "num_classes": 3,
-        "conv1_t_size": [3],
-        "conv1_t_stride": 1,
-        "bias_downsample": False,  # set to False if pretrained=True (PR #5477)
-    },
-    (1, 2, 32),
-    (1, 3),
 ]
 
 TEST_CASES = []
-PRETRAINED_TEST_CASES = []
-for case in [TEST_CASE_1, TEST_CASE_2, TEST_CASE_3, TEST_CASE_2_A, TEST_CASE_3_A]:
-    for model in [resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200]:
-        TEST_CASES.append([model, *case])
-        PRETRAINED_TEST_CASES.append([model, *case])
-for case in [TEST_CASE_5, TEST_CASE_5_A, TEST_CASE_6, TEST_CASE_7]:
-    TEST_CASES.append([ResNet, *case])
+TEST_CASES = [TEST_CASE_1, TEST_CASE_2, TEST_CASE_2_A]
 
-TEST_SCRIPT_CASES = [
-    [model, *TEST_CASE_1] for model in [resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200]
-]
+TEST_CASES_TS = [TEST_CASE_1]
 
 
-class TestResNet(unittest.TestCase):
+class NaiveNetwork(torch.nn.Module):
 
-    def setUp(self):
-        self.tmp_ckpt_filename = os.path.join("tests", "monai_unittest_tmp_ckpt.pth")
+    def __init__(self, spatial_dims, num_classes, **kwargs):
+        super().__init__()
+        self.spatial_dims = spatial_dims
+        self.num_classes = num_classes
+        self.num_anchors = 1
+        self.cls_key = "cls"
+        self.box_reg_key = "box_reg"
+        self.size_divisible = 1
+
+    def forward(self, images):
+        out_cls_shape = (images.shape[0], self.num_classes * self.num_anchors) + images.shape[-self.spatial_dims :]
+        out_box_reg_shape = (images.shape[0], 2 * self.spatial_dims * self.num_anchors) + images.shape[
+            -self.spatial_dims :
+        ]
+        return {self.cls_key: [torch.randn(out_cls_shape)], self.box_reg_key: [torch.randn(out_box_reg_shape)]}
+
+
+@SkipIfBeforePyTorchVersion((1, 11))
+@unittest.skipUnless(has_torchvision, "Requires torchvision")
+@skip_if_quick
+class TestRetinaNetDetector(unittest.TestCase):
 
-    def tearDown(self):
-        if os.path.exists(self.tmp_ckpt_filename):
-            try:
-                os.remove(self.tmp_ckpt_filename)
-            except BaseException:
-                pass
+    @parameterized.expand(TEST_CASES)
+    def test_retina_detector_resnet_backbone_shape(self, input_param, input_shape):
+        returned_layers = [1]
+        anchor_generator = AnchorGeneratorWithAnchorShape(
+            feature_map_scales=(1, 2), base_anchor_shapes=((8,) * input_param["spatial_dims"],)
+        )
+        detector = retinanet_resnet50_fpn_detector(
+            **input_param, anchor_generator=anchor_generator, returned_layers=returned_layers
+        )
+
+        with eval_mode(detector):
+            input_data = torch.randn(input_shape)
+            result = detector.forward(input_data)
+            assert len(result) == len(result)
+
+            input_data = [torch.randn(input_shape[1:]) for _ in range(random.randint(1, 9))]
+            result = detector.forward(input_data)
+            assert len(result) == len(result)
+
+        detector.set_atss_matcher()
+        detector.set_hard_negative_sampler(10, 0.5)
+        for num_gt_box in [0, 3]:  # test for both empty and non-empty boxes
+            gt_box_start = torch.randint(2, (num_gt_box, input_param["spatial_dims"])).to(torch.float16)
+            gt_box_end = gt_box_start + torch.randint(1, 10, (num_gt_box, input_param["spatial_dims"]))
+            one_target = {
+                "boxes": torch.cat((gt_box_start, gt_box_end), dim=1),
+                "labels": torch.randint(input_param["num_classes"], (num_gt_box,)),
+            }
+            with train_mode(detector):
+                input_data = torch.randn(input_shape)
+                targets = [one_target] * len(input_data)
+                result = detector.forward(input_data, targets)
+
+                input_data = [torch.randn(input_shape[1:]) for _ in range(random.randint(1, 9))]
+                targets = [one_target] * len(input_data)
+                result = detector.forward(input_data, targets)
 
     @parameterized.expand(TEST_CASES)
-    def test_resnet_shape(self, model, input_param, input_shape, expected_shape):
-        net = model(**input_param).to(device)
-        with eval_mode(net):
-            result = net.forward(torch.randn(input_shape).to(device))
-            if input_param.get("feed_forward", True):
-                self.assertEqual(result.shape, expected_shape)
-            else:
-                self.assertTrue(result.shape in expected_shape)
-
-    @parameterized.expand(PRETRAINED_TEST_CASES)
-    @skip_if_quick
-    @skip_if_no_cuda
-    def test_resnet_pretrained(self, model, input_param, input_shape, expected_shape):
-        net = model(**input_param).to(device)
-        # Save ckpt
-        torch.save(net.state_dict(), self.tmp_ckpt_filename)
-
-        cp_input_param = copy.copy(input_param)
-        # Custom pretrained weights
-        cp_input_param["pretrained"] = self.tmp_ckpt_filename
-        pretrained_net = model(**cp_input_param)
-        equal_state_dict(net.state_dict(), pretrained_net.state_dict())
-
-        if has_hf_modules:
-            # True flag
-            cp_input_param["pretrained"] = True
-            resnet_depth = int(re.search(r"resnet(\d+)", model.__name__).group(1))
-
-            bias_downsample, shortcut_type = get_medicalnet_pretrained_resnet_args(resnet_depth)
-
-            # With orig. test cases
-            if (
-                input_param.get("spatial_dims", 3) == 3
-                and input_param.get("n_input_channels", 3) == 1
-                and input_param.get("feed_forward", True) is False
-                and input_param.get("shortcut_type", "B") == shortcut_type
-                and (
-                    input_param.get("bias_downsample", True) == bool(bias_downsample) if bias_downsample != -1 else True
-                )
-            ):
-                model(**cp_input_param)
-            else:
-                with self.assertRaises(NotImplementedError):
-                    model(**cp_input_param)
-
-            # forcing MedicalNet pretrained download for 3D tests cases
-            cp_input_param["n_input_channels"] = 1
-            cp_input_param["feed_forward"] = False
-            cp_input_param["shortcut_type"] = shortcut_type
-            cp_input_param["bias_downsample"] = bool(bias_downsample) if bias_downsample != -1 else True
-            if cp_input_param.get("spatial_dims", 3) == 3:
-                with skip_if_downloading_fails():
-                    pretrained_net = model(**cp_input_param).to(device)
-                    medicalnet_state_dict = get_pretrained_resnet_medicalnet(resnet_depth, device=device)
-                    medicalnet_state_dict = {
-                        key.replace("module.", ""): value for key, value in medicalnet_state_dict.items()
-                    }
-                    equal_state_dict(pretrained_net.state_dict(), medicalnet_state_dict)
-
-    @parameterized.expand(TEST_SCRIPT_CASES)
-    def test_script(self, model, input_param, input_shape, expected_shape):
-        net = model(**input_param)
-        test_data = torch.randn(input_shape)
-        test_script_save(net, test_data)
+    def test_naive_retina_detector_shape(self, input_param, input_shape):
+        anchor_generator = AnchorGeneratorWithAnchorShape(
+            feature_map_scales=(1,), base_anchor_shapes=((8,) * input_param["spatial_dims"],)
+        )
+        detector = RetinaNetDetector(network=NaiveNetwork(**input_param), anchor_generator=anchor_generator)
+
+        with eval_mode(detector):
+            input_data = torch.randn(input_shape)
+            result = detector.forward(input_data)
+            assert len(result) == len(result)
+
+            input_data = [torch.randn(input_shape[1:]) for _ in range(random.randint(1, 9))]
+            result = detector.forward(input_data)
+            assert len(result) == len(result)
+
+        detector.set_atss_matcher()
+        detector.set_hard_negative_sampler(10, 0.5)
+        gt_box_start = torch.randint(2, (3, input_param["spatial_dims"])).to(torch.float16)
+        gt_box_end = gt_box_start + torch.randint(1, 10, (3, input_param["spatial_dims"]))
+        one_target = {
+            "boxes": torch.cat((gt_box_start, gt_box_end), dim=1),
+            "labels": torch.randint(input_param["num_classes"], (3,)),
+        }
+        with train_mode(detector):
+            input_data = torch.randn(input_shape)
+            targets = [one_target] * len(input_data)
+            result = detector.forward(input_data, targets)
+
+            input_data = [torch.randn(input_shape[1:]) for _ in range(random.randint(1, 9))]
+            targets = [one_target] * len(input_data)
+            result = detector.forward(input_data, targets)
+
+    @parameterized.expand(TEST_CASES_TS)
+    def test_script(self, input_param, input_shape):
+        # test whether support torchscript
+        returned_layers = [1]
+        anchor_generator = AnchorGeneratorWithAnchorShape(
+            feature_map_scales=(1, 2), base_anchor_shapes=((8,) * input_param["spatial_dims"],)
+        )
+        detector = retinanet_resnet50_fpn_detector(
+            **input_param, anchor_generator=anchor_generator, returned_layers=returned_layers
+        )
+        with eval_mode(detector):
+            input_data = torch.randn(input_shape)
+            test_script_save(detector.network, input_data)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_retinanet.py` & `monai_weekly-1.4.dev2417/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_retinanet_predict_utils.py` & `monai_weekly-1.4.dev2417/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rotate.py` & `monai_weekly-1.4.dev2417/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rotate90.py` & `monai_weekly-1.4.dev2417/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rotate90d.py` & `monai_weekly-1.4.dev2417/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_rotated.py` & `monai_weekly-1.4.dev2417/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_safe_dtype_range.py` & `monai_weekly-1.4.dev2417/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_saliency_inferer.py` & `monai_weekly-1.4.dev2417/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sample_slices.py` & `monai_weekly-1.4.dev2417/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sampler_dist.py` & `monai_weekly-1.4.dev2417/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_save_classificationd.py` & `monai_weekly-1.4.dev2417/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_save_image.py` & `monai_weekly-1.4.dev2417/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_save_imaged.py` & `monai_weekly-1.4.dev2417/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_save_state.py` & `monai_weekly-1.4.dev2417/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_savitzky_golay_filter.py` & `monai_weekly-1.4.dev2417/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_savitzky_golay_smooth.py` & `monai_weekly-1.4.dev2417/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_savitzky_golay_smoothd.py` & `monai_weekly-1.4.dev2417/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity_range.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity_range_percentiles.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity_range_percentilesd.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensity_ranged.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_scale_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_se_block.py` & `monai_weekly-1.4.dev2417/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_se_blocks.py` & `monai_weekly-1.4.dev2417/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_seg_loss_integration.py` & `monai_weekly-1.4.dev2417/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_segresnet.py` & `monai_weekly-1.4.dev2417/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_segresnet_block.py` & `monai_weekly-1.4.dev2417/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_segresnet_ds.py` & `monai_weekly-1.4.dev2417/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_select_cross_validation_folds.py` & `monai_weekly-1.4.dev2417/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_select_itemsd.py` & `monai_weekly-1.4.dev2417/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_selfattention.py` & `monai_weekly-1.4.dev2417/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_senet.py` & `monai_weekly-1.4.dev2417/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_separable_filter.py` & `monai_weekly-1.4.dev2417/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_set_determinism.py` & `monai_weekly-1.4.dev2417/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_set_visible_devices.py` & `monai_weekly-1.4.dev2417/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_shift_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_shift_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_shuffle_buffer.py` & `monai_weekly-1.4.dev2417/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_continuouswavelet.py` & `monai_weekly-1.4.dev2417/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_fillempty.py` & `monai_weekly-1.4.dev2417/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_fillemptyd.py` & `monai_weekly-1.4.dev2417/tests/test_signal_fillemptyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_add_gaussiannoise.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_add_sine.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_add_sine_partial.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_add_squarepulse.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_add_squarepulse_partial.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_drop.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_scale.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_rand_shift.py` & `monai_weekly-1.4.dev2417/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_signal_remove_frequency.py` & `monai_weekly-1.4.dev2417/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_simple_aspp.py` & `monai_weekly-1.4.dev2417/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_simulatedelay.py` & `monai_weekly-1.4.dev2417/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_simulatedelayd.py` & `monai_weekly-1.4.dev2417/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_skip_connection.py` & `monai_weekly-1.4.dev2417/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_slice_inferer.py` & `monai_weekly-1.4.dev2417/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sliding_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2417/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sliding_window_hovernet_inference.py` & `monai_weekly-1.4.dev2417/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sliding_window_inference.py` & `monai_weekly-1.4.dev2417/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sliding_window_splitter.py` & `monai_weekly-1.4.dev2417/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_smartcachedataset.py` & `monai_weekly-1.4.dev2417/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_smooth_field.py` & `monai_weekly-1.4.dev2417/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sobel_gradient.py` & `monai_weekly-1.4.dev2417/tests/test_sobel_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
             TEST_CASE_KERNEL_NON_NORMALIZED_0,
             TEST_CASE_KERNEL_NON_NORMALIZED_1,
             TEST_CASE_KERNEL_NON_NORMALIZED_2,
         ]
     )
     def test_sobel_kernels(self, arguments, expected_kernels):
         sobel = SobelGradients(**arguments)
-        self.assertTrue(sobel.kernel_diff.dtype == expected_kernels[0].dtype)
-        self.assertTrue(sobel.kernel_smooth.dtype == expected_kernels[0].dtype)
+        self.assertEqual(sobel.kernel_diff.dtype, expected_kernels[0].dtype)
+        self.assertEqual(sobel.kernel_smooth.dtype, expected_kernels[0].dtype)
         assert_allclose(sobel.kernel_diff, expected_kernels[0])
         assert_allclose(sobel.kernel_smooth, expected_kernels[1])
 
     @parameterized.expand(
         [
             TEST_CASE_ERROR_0,
             TEST_CASE_ERROR_1,
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_sobel_gradientd.py` & `monai_weekly-1.4.dev2417/tests/test_sobel_gradientd.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,16 +183,16 @@
             TEST_CASE_KERNEL_NON_NORMALIZED_0,
             TEST_CASE_KERNEL_NON_NORMALIZED_1,
             TEST_CASE_KERNEL_NON_NORMALIZED_2,
         ]
     )
     def test_sobel_kernels(self, arguments, expected_kernels):
         sobel = SobelGradientsd(**arguments)
-        self.assertTrue(sobel.kernel_diff.dtype == expected_kernels[0].dtype)
-        self.assertTrue(sobel.kernel_smooth.dtype == expected_kernels[0].dtype)
+        self.assertEqual(sobel.kernel_diff.dtype, expected_kernels[0].dtype)
+        self.assertEqual(sobel.kernel_smooth.dtype, expected_kernels[0].dtype)
         assert_allclose(sobel.kernel_diff, expected_kernels[0])
         assert_allclose(sobel.kernel_smooth, expected_kernels[1])
 
     @parameterized.expand(
         [
             TEST_CASE_ERROR_0,
             TEST_CASE_ERROR_1,
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_soft_clip.py` & `monai_weekly-1.4.dev2417/tests/test_soft_clip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_some_of.py` & `monai_weekly-1.4.dev2417/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spacing.py` & `monai_weekly-1.4.dev2417/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spacingd.py` & `monai_weekly-1.4.dev2417/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_combine_transforms.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_crop.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_cropd.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_pad.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_padd.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_resample.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spatial_resampled.py` & `monai_weekly-1.4.dev2417/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_spectral_loss.py` & `monai_weekly-1.4.dev2417/tests/test_spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_splitdim.py` & `monai_weekly-1.4.dev2417/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_splitdimd.py` & `monai_weekly-1.4.dev2417/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_squeeze_unsqueeze.py` & `monai_weekly-1.4.dev2417/tests/test_squeeze_unsqueeze.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_squeezedim.py` & `monai_weekly-1.4.dev2417/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_squeezedimd.py` & `monai_weekly-1.4.dev2417/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ssim_loss.py` & `monai_weekly-1.4.dev2417/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_ssim_metric.py` & `monai_weekly-1.4.dev2417/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_state_cacher.py` & `monai_weekly-1.4.dev2417/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_std_shift_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_std_shift_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_str2bool.py` & `monai_weekly-1.4.dev2417/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_str2list.py` & `monai_weekly-1.4.dev2417/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_subpixel_upsample.py` & `monai_weekly-1.4.dev2417/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_sure_loss.py` & `monai_weekly-1.4.dev2417/tests/test_sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_surface_dice.py` & `monai_weekly-1.4.dev2417/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_surface_distance.py` & `monai_weekly-1.4.dev2417/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_swin_unetr.py` & `monai_weekly-1.4.dev2417/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_synthetic.py` & `monai_weekly-1.4.dev2417/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_tciadataset.py` & `monai_weekly-1.4.dev2417/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_testtimeaugmentation.py` & `monai_weekly-1.4.dev2417/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_text_encoding.py` & `monai_weekly-1.4.dev2417/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_thread_buffer.py` & `monai_weekly-1.4.dev2417/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_threadcontainer.py` & `monai_weekly-1.4.dev2417/tests/test_threadcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         con = ThreadContainer(trainer)
         con.start()
         time.sleep(1)  # wait for trainer to start
 
         self.assertTrue(con.is_alive)
         self.assertIsNotNone(con.status())
-        self.assertTrue(len(con.status_dict) > 0)
+        self.assertGreater(len(con.status_dict), 0)
 
         con.join()
 
     @SkipIfNoModule("ignite")
     @SkipIfNoModule("matplotlib")
     def test_plot(self):
         set_determinism(0)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_threshold_intensity.py` & `monai_weekly-1.4.dev2417/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_threshold_intensityd.py` & `monai_weekly-1.4.dev2417/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_timedcall_dist.py` & `monai_weekly-1.4.dev2417/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_contiguous.py` & `monai_weekly-1.4.dev2417/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_cupy.py` & `monai_weekly-1.4.dev2417/tests/test_to_cupy.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,49 +58,49 @@
         cp.testing.assert_allclose(result, test_data)
 
     def test_numpy_input_dtype(self):
         test_data = np.array([[1, 2], [3, 4]], dtype=np.float32)
         test_data = np.rot90(test_data)
         self.assertFalse(test_data.flags["C_CONTIGUOUS"])
         result = ToCupy(np.uint8)(test_data)
-        self.assertTrue(result.dtype == cp.uint8)
-        self.assertTrue(isinstance(result, cp.ndarray))
+        self.assertEqual(result.dtype, cp.uint8)
+        self.assertIsInstance(result, cp.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         cp.testing.assert_allclose(result, test_data)
 
     def test_tensor_input(self):
         test_data = torch.tensor([[1, 2], [3, 4]], dtype=torch.float32)
         test_data = test_data.rot90()
         self.assertFalse(test_data.is_contiguous())
         result = ToCupy()(test_data)
-        self.assertTrue(result.dtype == cp.float32)
-        self.assertTrue(isinstance(result, cp.ndarray))
+        self.assertEqual(result.dtype, cp.float32)
+        self.assertIsInstance(result, cp.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         cp.testing.assert_allclose(result, test_data)
 
     @skip_if_no_cuda
     def test_tensor_cuda_input(self):
         test_data = torch.tensor([[1, 2], [3, 4]], dtype=torch.float32).cuda()
         test_data = test_data.rot90()
         self.assertFalse(test_data.is_contiguous())
         result = ToCupy()(test_data)
-        self.assertTrue(result.dtype == cp.float32)
-        self.assertTrue(isinstance(result, cp.ndarray))
+        self.assertEqual(result.dtype, cp.float32)
+        self.assertIsInstance(result, cp.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         cp.testing.assert_allclose(result, test_data)
 
     @skip_if_no_cuda
     def test_tensor_cuda_input_dtype(self):
         test_data = torch.tensor([[1, 2], [3, 4]], dtype=torch.uint8).cuda()
         test_data = test_data.rot90()
         self.assertFalse(test_data.is_contiguous())
 
         result = ToCupy(dtype="float32")(test_data)
-        self.assertTrue(result.dtype == cp.float32)
-        self.assertTrue(isinstance(result, cp.ndarray))
+        self.assertEqual(result.dtype, cp.float32)
+        self.assertIsInstance(result, cp.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         cp.testing.assert_allclose(result, test_data)
 
     def test_list_tuple(self):
         test_data = [[1, 2], [3, 4]]
         result = ToCupy(wrap_sequence=True)(test_data)
         cp.testing.assert_allclose(result, cp.asarray(test_data))
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_cupyd.py` & `monai_weekly-1.4.dev2417/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_device.py` & `monai_weekly-1.4.dev2417/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_deviced.py` & `monai_weekly-1.4.dev2417/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_from_meta_tensord.py` & `monai_weekly-1.4.dev2417/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_numpy.py` & `monai_weekly-1.4.dev2417/tests/test_to_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,44 +28,44 @@
 
     @skipUnless(HAS_CUPY, "CuPy is required.")
     def test_cupy_input(self):
         test_data = cp.array([[1, 2], [3, 4]])
         test_data = cp.rot90(test_data)
         self.assertFalse(test_data.flags["C_CONTIGUOUS"])
         result = ToNumpy()(test_data)
-        self.assertTrue(isinstance(result, np.ndarray))
+        self.assertIsInstance(result, np.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         assert_allclose(result, test_data.get(), type_test=False)
 
     def test_numpy_input(self):
         test_data = np.array([[1, 2], [3, 4]])
         test_data = np.rot90(test_data)
         self.assertFalse(test_data.flags["C_CONTIGUOUS"])
         result = ToNumpy(dtype="float32")(test_data)
-        self.assertTrue(isinstance(result, np.ndarray))
-        self.assertTrue(result.dtype == np.float32)
+        self.assertIsInstance(result, np.ndarray)
+        self.assertEqual(result.dtype, np.float32)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         assert_allclose(result, test_data, type_test=False)
 
     def test_tensor_input(self):
         test_data = torch.tensor([[1, 2], [3, 4]])
         test_data = test_data.rot90()
         self.assertFalse(test_data.is_contiguous())
         result = ToNumpy(dtype=torch.uint8)(test_data)
-        self.assertTrue(isinstance(result, np.ndarray))
+        self.assertIsInstance(result, np.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         assert_allclose(result, test_data, type_test=False)
 
     @skip_if_no_cuda
     def test_tensor_cuda_input(self):
         test_data = torch.tensor([[1, 2], [3, 4]]).cuda()
         test_data = test_data.rot90()
         self.assertFalse(test_data.is_contiguous())
         result = ToNumpy()(test_data)
-        self.assertTrue(isinstance(result, np.ndarray))
+        self.assertIsInstance(result, np.ndarray)
         self.assertTrue(result.flags["C_CONTIGUOUS"])
         assert_allclose(result, test_data, type_test=False)
 
     def test_list_tuple(self):
         test_data = [[1, 2], [3, 4]]
         result = ToNumpy()(test_data)
         assert_allclose(result, np.asarray(test_data), type_test=False)
@@ -73,14 +73,14 @@
         result = ToNumpy(wrap_sequence=False)(test_data)
         self.assertIsInstance(result, tuple)
         assert_allclose(result, ((np.asarray(1), np.asarray(2)), (np.asarray(3), np.asarray(4))))
 
     def test_single_value(self):
         for test_data in [5, np.array(5), torch.tensor(5)]:
             result = ToNumpy(dtype=np.uint8)(test_data)
-            self.assertTrue(isinstance(result, np.ndarray))
+            self.assertIsInstance(result, np.ndarray)
             assert_allclose(result, np.asarray(test_data), type_test=False)
             self.assertEqual(result.ndim, 0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_numpyd.py` & `monai_weekly-1.4.dev2417/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_onehot.py` & `monai_weekly-1.4.dev2417/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_pil.py` & `monai_weekly-1.4.dev2417/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_pild.py` & `monai_weekly-1.4.dev2417/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_tensor.py` & `monai_weekly-1.4.dev2417/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_to_tensord.py` & `monai_weekly-1.4.dev2417/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_torchscript_utils.py` & `monai_weekly-1.4.dev2417/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_torchvision.py` & `monai_weekly-1.4.dev2417/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_torchvision_fc_model.py` & `monai_weekly-1.4.dev2417/tests/test_torchvision_fc_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,13 +191,13 @@
 
     def test_get_module(self):
         net = UNet(spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32, 64), strides=(2, 2, 2, 2))
         self.assertEqual(look_up_named_module("", net), net)
         mod = look_up_named_module("model.1.submodule.1.submodule.1.submodule.0.conv", net)
         self.assertTrue(str(mod).startswith("Conv2d"))
         self.assertIsInstance(set_named_module(net, "model", torch.nn.Identity()).model, torch.nn.Identity)
-        self.assertEqual(look_up_named_module("model.1.submodule.1.submodule.1.submodule.conv", net), None)
-        self.assertEqual(look_up_named_module("test attribute", net), None)
+        self.assertIsNone(look_up_named_module("model.1.submodule.1.submodule.1.submodule.conv", net))
+        self.assertIsNone(look_up_named_module("test attribute", net))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_torchvisiond.py` & `monai_weekly-1.4.dev2417/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_traceable_transform.py` & `monai_weekly-1.4.dev2417/tests/test_traceable_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
 class TestTraceable(unittest.TestCase):
 
     def test_default(self):
         expected_key = "_transforms"
         a = _TraceTest()
         for x in a.transform_info_keys():
-            self.assertTrue(x in a.get_transform_info())
+            self.assertIn(x, a.get_transform_info())
         self.assertEqual(a.trace_key(), expected_key)
 
         data = {"image": "test"}
         data = a(data)  # adds to the stack
-        self.assertTrue(isinstance(data[expected_key], list))
+        self.assertIsInstance(data[expected_key], list)
         self.assertEqual(data[expected_key][0]["class"], "_TraceTest")
 
         data = a(data)  # adds to the stack
         self.assertEqual(len(data[expected_key]), 2)
         self.assertEqual(data[expected_key][-1]["class"], "_TraceTest")
 
         with self.assertRaises(IndexError):
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_train_mode.py` & `monai_weekly-1.4.dev2417/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_trainable_bilateral.py` & `monai_weekly-1.4.dev2417/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_trainable_joint_bilateral.py` & `monai_weekly-1.4.dev2417/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_transchex.py` & `monai_weekly-1.4.dev2417/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_transform.py` & `monai_weekly-1.4.dev2417/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_transformerblock.py` & `monai_weekly-1.4.dev2417/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_transpose.py` & `monai_weekly-1.4.dev2417/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_transposed.py` & `monai_weekly-1.4.dev2417/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_tversky_loss.py` & `monai_weekly-1.4.dev2417/tests/test_tversky_loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,25 +161,20 @@
         chn_input = torch.ones((1, 1, 3))
         chn_target = torch.ones((1, 1, 3))
         with self.assertRaisesRegex(ValueError, ""):
             TverskyLoss(reduction="unknown")(chn_input, chn_target)
         with self.assertRaisesRegex(ValueError, ""):
             TverskyLoss(reduction=None)(chn_input, chn_target)
 
-    def test_input_warnings(self):
+    @parameterized.expand([(False, False, False), (False, True, False), (False, False, True)])
+    def test_input_warnings(self, include_background, softmax, to_onehot_y):
         chn_input = torch.ones((1, 1, 3))
         chn_target = torch.ones((1, 1, 3))
         with self.assertWarns(Warning):
-            loss = TverskyLoss(include_background=False)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = TverskyLoss(softmax=True)
-            loss.forward(chn_input, chn_target)
-        with self.assertWarns(Warning):
-            loss = TverskyLoss(to_onehot_y=True)
+            loss = TverskyLoss(include_background=include_background, softmax=softmax, to_onehot_y=to_onehot_y)
             loss.forward(chn_input, chn_target)
 
     def test_script(self):
         loss = TverskyLoss()
         test_input = torch.ones(2, 1, 8, 8)
         test_script_save(loss, test_input, test_input)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_unet.py` & `monai_weekly-1.4.dev2417/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_unetr.py` & `monai_weekly-1.4.dev2417/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_unetr_block.py` & `monai_weekly-1.4.dev2417/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_unified_focal_loss.py` & `monai_weekly-1.4.dev2417/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_upsample_block.py` & `monai_weekly-1.4.dev2417/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2417/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_varautoencoder.py` & `monai_weekly-1.4.dev2417/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_varnet.py` & `monai_weekly-1.4.dev2417/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_version.py` & `monai_weekly-1.4.dev2417/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_video_datasets.py` & `monai_weekly-1.4.dev2417/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vis_cam.py` & `monai_weekly-1.4.dev2417/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vis_gradbased.py` & `monai_weekly-1.4.dev2417/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vis_gradcam.py` & `monai_weekly-1.4.dev2417/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vit.py` & `monai_weekly-1.4.dev2417/tests/test_vit.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,83 +65,48 @@
     @parameterized.expand(TEST_CASE_Vit)
     def test_shape(self, input_param, input_shape, expected_shape):
         net = ViT(**input_param)
         with eval_mode(net):
             result, _ = net(torch.randn(input_shape))
             self.assertEqual(result.shape, expected_shape)
 
-    def test_ill_arg(self):
+    @parameterized.expand(
+        [
+            (1, (128, 128, 128), (16, 16, 16), 128, 3072, 12, 12, "conv", False, 5.0),
+            (1, (32, 32, 32), (64, 64, 64), 512, 3072, 12, 8, "perceptron", False, 0.3),
+            (1, (96, 96, 96), (8, 8, 8), 512, 3072, 12, 14, "conv", False, 0.3),
+            (1, (97, 97, 97), (4, 4, 4), 768, 3072, 12, 8, "perceptron", True, 0.3),
+            (4, (96, 96, 96), (16, 16, 16), 768, 3072, 12, 12, "perc", False, 0.3),
+        ]
+    )
+    def test_ill_arg(
+        self,
+        in_channels,
+        img_size,
+        patch_size,
+        hidden_size,
+        mlp_dim,
+        num_layers,
+        num_heads,
+        pos_embed,
+        classification,
+        dropout_rate,
+    ):
         with self.assertRaises(ValueError):
             ViT(
-                in_channels=1,
-                img_size=(128, 128, 128),
-                patch_size=(16, 16, 16),
-                hidden_size=128,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=12,
-                pos_embed="conv",
-                classification=False,
-                dropout_rate=5.0,
-            )
-
-        with self.assertRaises(ValueError):
-            ViT(
-                in_channels=1,
-                img_size=(32, 32, 32),
-                patch_size=(64, 64, 64),
-                hidden_size=512,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=8,
-                pos_embed="perceptron",
-                classification=False,
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViT(
-                in_channels=1,
-                img_size=(96, 96, 96),
-                patch_size=(8, 8, 8),
-                hidden_size=512,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=14,
-                pos_embed="conv",
-                classification=False,
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViT(
-                in_channels=1,
-                img_size=(97, 97, 97),
-                patch_size=(4, 4, 4),
-                hidden_size=768,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=8,
-                pos_embed="perceptron",
-                classification=True,
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViT(
-                in_channels=4,
-                img_size=(96, 96, 96),
-                patch_size=(16, 16, 16),
-                hidden_size=768,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=12,
-                pos_embed="perc",
-                classification=False,
-                dropout_rate=0.3,
+                in_channels=in_channels,
+                img_size=img_size,
+                patch_size=patch_size,
+                hidden_size=hidden_size,
+                mlp_dim=mlp_dim,
+                num_layers=num_layers,
+                num_heads=num_heads,
+                pos_embed=pos_embed,
+                classification=classification,
+                dropout_rate=dropout_rate,
             )
 
     @parameterized.expand(TEST_CASE_Vit)
     @SkipIfBeforePyTorchVersion((1, 9))
     def test_script(self, input_param, input_shape, _):
         net = ViT(**(input_param))
         net.eval()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_vitautoenc.py` & `monai_weekly-1.4.dev2417/tests/test_vitautoenc.py`

 * *Files 23% similar despite different names*

```diff
@@ -78,89 +78,36 @@
     @skip_if_windows
     def test_shape(self, input_param, input_shape, expected_shape):
         net = ViTAutoEnc(**input_param)
         with eval_mode(net):
             result, _ = net(torch.randn(input_shape))
             self.assertEqual(result.shape, expected_shape)
 
-    def test_ill_arg(self):
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=1,
-                img_size=(128, 128, 128),
-                patch_size=(16, 16, 16),
-                hidden_size=128,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=12,
-                pos_embed="conv",
-                dropout_rate=5.0,
-            )
-
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=1,
-                img_size=(32, 32, 32),
-                patch_size=(64, 64, 64),
-                hidden_size=512,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=8,
-                pos_embed="perceptron",
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=1,
-                img_size=(96, 96, 96),
-                patch_size=(8, 8, 8),
-                hidden_size=512,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=14,
-                pos_embed="conv",
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=1,
-                img_size=(97, 97, 97),
-                patch_size=(4, 4, 4),
-                hidden_size=768,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=8,
-                pos_embed="perceptron",
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=4,
-                img_size=(96, 96, 96),
-                patch_size=(16, 16, 16),
-                hidden_size=768,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=12,
-                pos_embed="perc",
-                dropout_rate=0.3,
-            )
-
-        with self.assertRaises(ValueError):
-            ViTAutoEnc(
-                in_channels=4,
-                img_size=(96, 96, 96),
-                patch_size=(9, 9, 9),
-                hidden_size=768,
-                mlp_dim=3072,
-                num_layers=12,
-                num_heads=12,
-                pos_embed="perc",
-                dropout_rate=0.3,
+    @parameterized.expand(
+        [
+            (1, (32, 32, 32), (64, 64, 64), 512, 3072, 12, 8, "perceptron", 0.3),  # img_size_too_large_for_patch_size
+            (1, (96, 96, 96), (8, 8, 8), 512, 3072, 12, 14, "conv", 0.3),  # num_heads_out_of_bound
+            (1, (97, 97, 97), (4, 4, 4), 768, 3072, 12, 8, "perceptron", 0.3),  # img_size_not_divisible_by_patch_size
+            (4, (96, 96, 96), (16, 16, 16), 768, 3072, 12, 12, "perc", 0.3),  # invalid_pos_embed
+            (4, (96, 96, 96), (9, 9, 9), 768, 3072, 12, 12, "perc", 0.3),  # patch_size_not_divisible
+            # Add more test cases as needed
+        ]
+    )
+    def test_ill_arg(
+        self, in_channels, img_size, patch_size, hidden_size, mlp_dim, num_layers, num_heads, pos_embed, dropout_rate
+    ):
+        with self.assertRaises(ValueError):
+            ViTAutoEnc(
+                in_channels=in_channels,
+                img_size=img_size,
+                patch_size=patch_size,
+                hidden_size=hidden_size,
+                mlp_dim=mlp_dim,
+                num_layers=num_layers,
+                num_heads=num_heads,
+                pos_embed=pos_embed,
+                dropout_rate=dropout_rate,
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_vnet.py` & `monai_weekly-1.4.dev2417/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vote_ensemble.py` & `monai_weekly-1.4.dev2417/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_vote_ensembled.py` & `monai_weekly-1.4.dev2417/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_voxelmorph.py` & `monai_weekly-1.4.dev2417/tests/test_voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_warp.py` & `monai_weekly-1.4.dev2417/tests/test_warp.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def test_itk_benchmark(self):
         img, ddf = load_img_and_sample_ddf()
         monai_result = monai_warp(img, ddf)
         itk_result = itk_warp(img, ddf)
         relative_diff = np.mean(
             np.divide(monai_result - itk_result, itk_result, out=np.zeros_like(itk_result), where=(itk_result != 0))
         )
-        self.assertTrue(relative_diff < 0.01)
+        self.assertLess(relative_diff, 0.01)
 
     @parameterized.expand(TEST_CASES, skip_on_empty=True)
     def test_resample(self, input_param, input_data, expected_val):
         warp_layer = Warp(**input_param)
         result = warp_layer(**input_data)
         np.testing.assert_allclose(result.cpu().numpy(), expected_val.cpu().numpy(), rtol=1e-4, atol=1e-4)
```

### Comparing `monai_weekly-1.4.dev2416/tests/test_watershed.py` & `monai_weekly-1.4.dev2417/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_watershedd.py` & `monai_weekly-1.4.dev2417/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_weight_init.py` & `monai_weekly-1.4.dev2417/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_weighted_random_sampler_dist.py` & `monai_weekly-1.4.dev2417/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_with_allow_missing_keys.py` & `monai_weekly-1.4.dev2417/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_write_metrics_reports.py` & `monai_weekly-1.4.dev2417/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_wsi_sliding_window_splitter.py` & `monai_weekly-1.4.dev2417/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_wsireader.py` & `monai_weekly-1.4.dev2417/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_zarr_avg_merger.py` & `monai_weekly-1.4.dev2417/tests/test_zarr_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_zipdataset.py` & `monai_weekly-1.4.dev2417/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_zoom.py` & `monai_weekly-1.4.dev2417/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_zoom_affine.py` & `monai_weekly-1.4.dev2417/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/tests/test_zoomd.py` & `monai_weekly-1.4.dev2417/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2416/versioneer.py` & `monai_weekly-1.4.dev2417/versioneer.py`

 * *Files identical despite different names*

