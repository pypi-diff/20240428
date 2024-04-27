# Comparing `tmp/fastai-2.7.8.tar.gz` & `tmp/fastai-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-2.7.8.tar", last modified: Tue Aug  2 19:20:01 2022, max compression
+gzip compressed data, was "fastai-2.7.9.tar", last modified: Wed Aug  3 23:16:31 2022, max compression
```

## Comparing `fastai-2.7.8.tar` & `fastai-2.7.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9471 2022-02-15 01:11:38.000000 fastai-2.7.8/CONTRIBUTING.md
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11357 2021-12-01 06:52:56.000000 fastai-2.7.8/LICENSE
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      177 2021-12-01 06:52:56.000000 fastai-2.7.8/MANIFEST.in
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     8614 2022-08-02 19:20:01.148054 fastai-2.7.8/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7660 2022-08-02 18:57:46.000000 fastai-2.7.8/README.md
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.144054 fastai-2.7.8/fastai/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       23 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)   196037 2022-08-02 18:55:43.000000 fastai-2.7.8/fastai/_modidx.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    44456 2022-07-04 06:30:25.000000 fastai-2.7.8/fastai/_nbdev.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     1574 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/_pytorch_doc.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      149 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/basics.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/callback/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      235 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/callback/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2694 2022-02-15 01:17:26.000000 fastai-2.7.8/fastai/callback/azureml.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5786 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/captum.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3321 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/comet.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9325 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3094 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/callback/data.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    10262 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/fp16.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11330 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/hook.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4815 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/mixup.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3774 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/neptune.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      608 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/preds.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5119 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/progress.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     1810 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/rnn.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    14296 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/schedule.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7275 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/callback/tensorboard.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7699 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/callback/tracker.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2675 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/callback/training.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    14911 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/callback/wandb.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5200 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/collab.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/data/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/data/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      140 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/data/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11043 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/data/block.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    24254 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/data/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9436 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/data/download_checks.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     6002 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/data/external.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11018 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/data/load.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    16769 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/data/transforms.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9785 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/distributed.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     6957 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/fp16_utils.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3439 2022-05-15 00:34:48.000000 fastai-2.7.8/fastai/imports.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7758 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/interpret.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    27260 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/layers.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    28907 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/learner.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11428 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/losses.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/medical/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/medical/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    15451 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/medical/imaging.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      195 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/medical/text.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    22630 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/metrics.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    18263 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/optimizer.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/tabular/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/tabular/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      136 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/tabular/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    16888 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/tabular/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2759 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/tabular/data.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2327 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/tabular/learner.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3719 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/tabular/model.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     6034 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/test_utils.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/text/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      137 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/text/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    17415 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    14528 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/data.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    13813 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/learner.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/text/models/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       42 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/models/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     8453 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/text/models/awdlstm.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     8209 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/text/models/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      516 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/torch_basics.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    34328 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/torch_core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      400 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/torch_imports.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/vision/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      206 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/vision/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    56498 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/vision/augment.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11213 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/core.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11536 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/vision/data.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    19445 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/gan.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    18596 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/learner.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.148054 fastai-2.7.8/fastai/vision/models/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       60 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/models/__init__.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       62 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/vision/models/all.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      309 2021-12-01 06:52:56.000000 fastai-2.7.8/fastai/vision/models/tvm.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4689 2022-08-02 18:55:41.000000 fastai-2.7.8/fastai/vision/models/unet.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     7725 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/models/xresnet.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4303 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/utils.py
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5142 2022-08-02 18:55:42.000000 fastai-2.7.8/fastai/vision/widgets.py
-drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2022-08-02 19:20:01.144054 fastai-2.7.8/fastai.egg-info/
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     8614 2022-08-02 19:20:00.000000 fastai-2.7.8/fastai.egg-info/PKG-INFO
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2101 2022-08-02 19:20:01.000000 fastai-2.7.8/fastai.egg-info/SOURCES.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-08-02 19:20:00.000000 fastai-2.7.8/fastai.egg-info/dependency_links.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      116 2022-08-02 19:20:00.000000 fastai-2.7.8/fastai.egg-info/entry_points.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2021-12-01 18:23:40.000000 fastai-2.7.8/fastai.egg-info/not-zip-safe
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      475 2022-08-02 19:20:01.000000 fastai-2.7.8/fastai.egg-info/requires.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        7 2022-08-02 19:20:01.000000 fastai-2.7.8/fastai.egg-info/top_level.txt
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     1301 2022-07-30 09:21:42.000000 fastai-2.7.8/settings.ini
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       38 2022-08-02 19:20:01.148054 fastai-2.7.8/setup.cfg
--rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2805 2022-07-30 09:21:42.000000 fastai-2.7.8/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.457292 fastai-2.7.9/
+-rw-r--r--   0 jhoward    (501) staff       (20)     9471 2022-07-23 05:45:27.000000 fastai-2.7.9/CONTRIBUTING.md
+-rw-r--r--   0 jhoward    (501) staff       (20)    11357 2022-07-23 05:45:27.000000 fastai-2.7.9/LICENSE
+-rw-r--r--   0 jhoward    (501) staff       (20)      177 2022-07-23 05:45:27.000000 fastai-2.7.9/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)     8594 2022-08-03 23:16:31.457131 fastai-2.7.9/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     7660 2022-08-01 21:42:25.000000 fastai-2.7.9/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.450830 fastai-2.7.9/fastai/
+-rw-r--r--   0 jhoward    (501) staff       (20)       23 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)   196037 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    44456 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/_nbdev.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1574 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/_pytorch_doc.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      149 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/basics.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.453471 fastai-2.7.9/fastai/callback/
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      235 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/callback/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     2694 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/callback/azureml.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5786 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/captum.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3321 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/comet.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     9325 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3094 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/data.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    10262 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/fp16.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11330 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/hook.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4815 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/mixup.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3774 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/neptune.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      608 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/preds.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5119 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/progress.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1810 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/rnn.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    14296 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/schedule.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     7275 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/callback/tensorboard.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     7699 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/tracker.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     2675 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/training.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    14911 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/callback/wandb.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5200 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/collab.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.454190 fastai-2.7.9/fastai/data/
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/data/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      140 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/data/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11043 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/data/block.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    24254 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/data/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     9436 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/data/download_checks.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6002 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/data/external.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11018 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/data/load.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    16769 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/data/transforms.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     9785 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/distributed.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6957 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/fp16_utils.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3439 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/imports.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     7758 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/interpret.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    27260 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/layers.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    28907 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/learner.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11428 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/losses.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.454450 fastai-2.7.9/fastai/medical/
+-rw-r--r--   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/medical/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    15451 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/medical/imaging.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      195 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/medical/text.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    22630 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/metrics.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    18263 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/optimizer.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.454976 fastai-2.7.9/fastai/tabular/
+-rw-r--r--   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/tabular/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      136 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/tabular/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    16888 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/tabular/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     2759 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/tabular/data.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     2327 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/tabular/learner.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3719 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/tabular/model.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     6034 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/test_utils.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.455434 fastai-2.7.9/fastai/text/
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/text/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      137 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/text/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    17415 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/text/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    14528 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/text/data.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    13813 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/text/learner.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.455697 fastai-2.7.9/fastai/text/models/
+-rw-r--r--   0 jhoward    (501) staff       (20)       42 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/text/models/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     8453 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/text/models/awdlstm.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     8209 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/text/models/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      516 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/torch_basics.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    34328 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/torch_core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      400 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/torch_imports.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.456522 fastai-2.7.9/fastai/vision/
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/vision/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      206 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/vision/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    56498 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/augment.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11205 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/vision/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    11536 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/vision/data.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    19445 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/gan.py
+-rw-r--r--   0 jhoward    (501) staff       (20)    18596 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/vision/learner.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.456977 fastai-2.7.9/fastai/vision/models/
+-rw-r--r--   0 jhoward    (501) staff       (20)       60 2022-08-03 23:16:01.000000 fastai-2.7.9/fastai/vision/models/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)       62 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/vision/models/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      309 2022-07-23 05:45:28.000000 fastai-2.7.9/fastai/vision/models/tvm.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4689 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/models/unet.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     7725 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/models/xresnet.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4303 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/utils.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5142 2022-08-03 23:16:00.000000 fastai-2.7.9/fastai/vision/widgets.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2022-08-03 23:16:31.451655 fastai-2.7.9/fastai.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)     8594 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     2101 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      116 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/entry_points.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2022-07-23 19:23:36.000000 fastai-2.7.9/fastai.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)      466 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        7 2022-08-03 23:16:31.000000 fastai-2.7.9/fastai.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)     1301 2022-08-02 22:00:23.000000 fastai-2.7.9/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2022-08-03 23:16:31.457328 fastai-2.7.9/setup.cfg
+-rw-r--r--   0 jhoward    (501) staff       (20)     2805 2022-07-26 23:47:05.000000 fastai-2.7.9/setup.py
```

### Comparing `fastai-2.7.8/CONTRIBUTING.md` & `fastai-2.7.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/LICENSE` & `fastai-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/PKG-INFO` & `fastai-2.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fastai
-Version: 2.7.8
+Version: 2.7.9
 Summary: fastai simplifies training fast and accurate neural nets using modern best practices
 Home-page: https://github.com/fastai/fastai/tree/master/
 Author: Jeremy Howard, Sylvain Gugger, and contributors
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: fastai,deep learning,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -199,9 +198,7 @@
     notebooks with `nbdev_update_lib`.
 
 ## Docker Containers
 
 For those interested in official docker containers for this project,
 they can be found
 [here](https://github.com/fastai/docker-containers#fastai).
-
-
```

### Comparing `fastai-2.7.8/README.md` & `fastai-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/_modidx.py` & `fastai-2.7.9/fastai/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 'recursive': 'True',
                 'requirements': 'fastdownload>=0.0.5,<2 fastcore>=1.4.5,<1.6 torchvision>=0.8.2 matplotlib pandas requests pyyaml fastprogress>=0.2.4 '
                                 'pillow>6.0.0 scikit-learn scipy spacy<4 packaging',
                 'status': '4',
                 'title': 'fastai',
                 'tst_flags': 'slow cpp cuda multicuda',
                 'user': 'fastai',
-                'version': '2.7.8'},
+                'version': '2.7.9'},
   'syms': { 'fastai.basics': {},
             'fastai.callback.all': {},
             'fastai.callback.azureml': { 'fastai.callback.azureml.AzureMLCallback': 'https://docs.fast.ai/callback.azureml.html#azuremlcallback',
                                          'fastai.callback.azureml.AzureMLCallback.after_batch': 'https://docs.fast.ai/callback.azureml.html#azuremlcallback.after_batch',
                                          'fastai.callback.azureml.AzureMLCallback.after_epoch': 'https://docs.fast.ai/callback.azureml.html#azuremlcallback.after_epoch',
                                          'fastai.callback.azureml.AzureMLCallback.before_fit': 'https://docs.fast.ai/callback.azureml.html#azuremlcallback.before_fit'},
             'fastai.callback.captum': { 'fastai.callback.captum.CaptumInterpretation': 'https://docs.fast.ai/callback.captum.html#captuminterpretation',
```

### Comparing `fastai-2.7.8/fastai/_nbdev.py` & `fastai-2.7.9/fastai/_nbdev.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/_pytorch_doc.py` & `fastai-2.7.9/fastai/_pytorch_doc.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/azureml.py` & `fastai-2.7.9/fastai/callback/azureml.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/captum.py` & `fastai-2.7.9/fastai/callback/captum.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/comet.py` & `fastai-2.7.9/fastai/callback/comet.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/core.py` & `fastai-2.7.9/fastai/callback/core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/data.py` & `fastai-2.7.9/fastai/callback/data.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/fp16.py` & `fastai-2.7.9/fastai/callback/fp16.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/hook.py` & `fastai-2.7.9/fastai/callback/hook.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/mixup.py` & `fastai-2.7.9/fastai/callback/mixup.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/neptune.py` & `fastai-2.7.9/fastai/callback/neptune.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/preds.py` & `fastai-2.7.9/fastai/callback/preds.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/progress.py` & `fastai-2.7.9/fastai/callback/progress.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/rnn.py` & `fastai-2.7.9/fastai/callback/rnn.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/schedule.py` & `fastai-2.7.9/fastai/callback/schedule.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/tensorboard.py` & `fastai-2.7.9/fastai/callback/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/tracker.py` & `fastai-2.7.9/fastai/callback/tracker.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/training.py` & `fastai-2.7.9/fastai/callback/training.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/callback/wandb.py` & `fastai-2.7.9/fastai/callback/wandb.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/collab.py` & `fastai-2.7.9/fastai/collab.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/block.py` & `fastai-2.7.9/fastai/data/block.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/core.py` & `fastai-2.7.9/fastai/data/core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/download_checks.py` & `fastai-2.7.9/fastai/data/download_checks.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/external.py` & `fastai-2.7.9/fastai/data/external.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/load.py` & `fastai-2.7.9/fastai/data/load.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/data/transforms.py` & `fastai-2.7.9/fastai/data/transforms.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/distributed.py` & `fastai-2.7.9/fastai/distributed.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/fp16_utils.py` & `fastai-2.7.9/fastai/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/imports.py` & `fastai-2.7.9/fastai/imports.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/interpret.py` & `fastai-2.7.9/fastai/interpret.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/layers.py` & `fastai-2.7.9/fastai/layers.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/learner.py` & `fastai-2.7.9/fastai/learner.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/losses.py` & `fastai-2.7.9/fastai/losses.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/medical/imaging.py` & `fastai-2.7.9/fastai/medical/imaging.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/metrics.py` & `fastai-2.7.9/fastai/metrics.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/optimizer.py` & `fastai-2.7.9/fastai/optimizer.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/tabular/core.py` & `fastai-2.7.9/fastai/tabular/core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/tabular/data.py` & `fastai-2.7.9/fastai/tabular/data.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/tabular/learner.py` & `fastai-2.7.9/fastai/tabular/learner.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/tabular/model.py` & `fastai-2.7.9/fastai/tabular/model.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/test_utils.py` & `fastai-2.7.9/fastai/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/text/core.py` & `fastai-2.7.9/fastai/text/core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/text/data.py` & `fastai-2.7.9/fastai/text/data.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/text/learner.py` & `fastai-2.7.9/fastai/text/learner.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/text/models/awdlstm.py` & `fastai-2.7.9/fastai/text/models/awdlstm.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/text/models/core.py` & `fastai-2.7.9/fastai/text/models/core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/torch_basics.py` & `fastai-2.7.9/fastai/torch_basics.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/torch_core.py` & `fastai-2.7.9/fastai/torch_core.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/augment.py` & `fastai-2.7.9/fastai/vision/augment.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/core.py` & `fastai-2.7.9/fastai/vision/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # %% ../nbs/07_vision.core.ipynb 7
 _all_ = ['Image','ToTensor']
 
 # %% ../nbs/07_vision.core.ipynb 8
 @patch
 def __repr__(x:Image.Image):
-    return "<%s.%s image mode=%s size=%dx%d at 0x%X>" % (x.__class__.__module__, x.__class__.__name__, x.mode, x.size[0], x.size[1])
+    return "<%s.%s image mode=%s size=%dx%d>" % (x.__class__.__module__, x.__class__.__name__, x.mode, x.size[0], x.size[1])
 
 # %% ../nbs/07_vision.core.ipynb 11
 imagenet_stats = ([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
 cifar_stats    = ([0.491, 0.482, 0.447], [0.247, 0.243, 0.261])
 mnist_stats    = ([0.131], [0.308])
 
 # %% ../nbs/07_vision.core.ipynb 13
```

### Comparing `fastai-2.7.8/fastai/vision/data.py` & `fastai-2.7.9/fastai/vision/data.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/gan.py` & `fastai-2.7.9/fastai/vision/gan.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/learner.py` & `fastai-2.7.9/fastai/vision/learner.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/models/unet.py` & `fastai-2.7.9/fastai/vision/models/unet.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/models/xresnet.py` & `fastai-2.7.9/fastai/vision/models/xresnet.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/utils.py` & `fastai-2.7.9/fastai/vision/utils.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai/vision/widgets.py` & `fastai-2.7.9/fastai/vision/widgets.py`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/fastai.egg-info/PKG-INFO` & `fastai-2.7.9/fastai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fastai
-Version: 2.7.8
+Version: 2.7.9
 Summary: fastai simplifies training fast and accurate neural nets using modern best practices
 Home-page: https://github.com/fastai/fastai/tree/master/
 Author: Jeremy Howard, Sylvain Gugger, and contributors
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: fastai,deep learning,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -199,9 +198,7 @@
     notebooks with `nbdev_update_lib`.
 
 ## Docker Containers
 
 For those interested in official docker containers for this project,
 they can be found
 [here](https://github.com/fastai/docker-containers#fastai).
-
-
```

### Comparing `fastai-2.7.8/fastai.egg-info/SOURCES.txt` & `fastai-2.7.9/fastai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-2.7.8/settings.ini` & `fastai-2.7.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [DEFAULT]
 lib_name = fastai
 user = fastai
 branch = master
-version = 2.7.8
+version = 2.7.9
 description = fastai simplifies training fast and accurate neural nets using modern best practices
 keywords = fastai, deep learning, machine learning
 author = Jeremy Howard, Sylvain Gugger, and contributors
 author_email = info@fast.ai
 license = apache2
 copyright = fast.ai
 status = 4
```

### Comparing `fastai-2.7.8/setup.py` & `fastai-2.7.9/setup.py`

 * *Files identical despite different names*

