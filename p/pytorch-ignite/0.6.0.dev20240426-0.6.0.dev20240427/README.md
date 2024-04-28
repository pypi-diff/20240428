# Comparing `tmp/pytorch-ignite-0.6.0.dev20240426.tar.gz` & `tmp/pytorch-ignite-0.6.0.dev20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.6.0.dev20240426.tar", last modified: Fri Apr 26 00:13:22 2024, max compression
+gzip compressed data, was "pytorch-ignite-0.6.0.dev20240427.tar", last modified: Sat Apr 27 00:13:26 2024, max compression
```

## Comparing `pytorch-ignite-0.6.0.dev20240426.tar` & `pytorch-ignite-0.6.0.dev20240427.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.148133 pytorch-ignite-0.6.0.dev20240426/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-26 00:13:22.148133 pytorch-ignite-0.6.0.dev20240426/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.124133 pytorch-ignite-0.6.0.dev20240426/ignite/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 00:11:03.000000 pytorch-ignite-0.6.0.dev20240426/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.124133 pytorch-ignite-0.6.0.dev20240426/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.124133 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.124133 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.128133 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.128133 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.132133 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.132133 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.132133 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.132133 pytorch-ignite-0.6.0.dev20240426/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.136133 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/fbresearch_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    68285 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.144133 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.144133 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/multilabel_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mutual_information.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.144133 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/recall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.148133 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/pearson_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:13:22.148133 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 00:13:22.000000 pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-26 00:13:22.148133 pytorch-ignite-0.6.0.dev20240426/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 00:10:39.000000 pytorch-ignite-0.6.0.dev20240426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.771983 pytorch-ignite-0.6.0.dev20240427/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-27 00:13:26.771983 pytorch-ignite-0.6.0.dev20240427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.743984 pytorch-ignite-0.6.0.dev20240427/ignite/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 00:11:15.000000 pytorch-ignite-0.6.0.dev20240427/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.743984 pytorch-ignite-0.6.0.dev20240427/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.743984 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.747984 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.747984 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.747984 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.751984 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.751984 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.751984 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.755983 pytorch-ignite-0.6.0.dev20240427/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.759983 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/fbresearch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68285 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.763983 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.763983 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/multilabel_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mutual_information.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.763983 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.767984 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/pearson_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:13:26.767984 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 00:13:26.000000 pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-27 00:13:26.771983 pytorch-ignite-0.6.0.dev20240427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-27 00:10:57.000000 pytorch-ignite-0.6.0.dev20240427/setup.py
```

### Comparing `pytorch-ignite-0.6.0.dev20240426/LICENSE` & `pytorch-ignite-0.6.0.dev20240427/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/PKG-INFO` & `pytorch-ignite-0.6.0.dev20240427/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240426
+Version: 0.6.0.dev20240427
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.6.0.dev20240426/README.md` & `pytorch-ignite-0.6.0.dev20240427/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/base/mixins.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/common.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/auto.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/launcher.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/distributed/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/engine/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/engine/deterministic.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/engine/engine.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/engine/events.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/engine/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/base_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/clearml_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/fbresearch_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/fbresearch_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/mlflow_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/neptune_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/polyaxon_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/stores.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/tensorboard_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/time_limit.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/timing.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/tqdm_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/visdom_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/handlers/wandb_logger.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/accumulation.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/accuracy.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/average_precision.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/classification_report.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/cohen_kappa.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/cosine_similarity.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/entropy.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/fbeta.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/frequency.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/gpu_info.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/js_divergence.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/js_divergence.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import torch
 import torch.nn.functional as F
+from packaging.version import Version
 
 from ignite.exceptions import NotComputableError
 from ignite.metrics.kl_divergence import KLDivergence
 from ignite.metrics.metric import sync_all_reduce
 
 __all__ = ["JSDivergence"]
 
+TORCH_VERSION_GE_160 = Version(torch.__version__) >= Version("1.6.0")
+
 
 class JSDivergence(KLDivergence):
     r"""Calculates the mean of `Jensen-Shannon (JS) divergence
     <https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence>`_.
 
     .. math::
        \begin{align*}
@@ -67,21 +70,31 @@
 
         .. testoutput::
 
            0.16266516844431558
     """
 
     def _update(self, y_pred: torch.Tensor, y: torch.Tensor) -> None:
-        m_prob = (F.softmax(y_pred, dim=1) + F.softmax(y, dim=1)) / 2
+        y_pred_prob = F.softmax(y_pred, dim=1)
+        y_prob = F.softmax(y, dim=1)
+        m_prob = (y_pred_prob + y_prob) / 2
         m_log = m_prob.log()
-        y_pred = F.log_softmax(y_pred, dim=1)
-        y = F.log_softmax(y, dim=1)
-        self._sum_of_kl += (
-            F.kl_div(m_log, y_pred, log_target=True, reduction="sum")
-            + F.kl_div(m_log, y, log_target=True, reduction="sum")
-        ).to(self._device)
+
+        if TORCH_VERSION_GE_160:
+            # log_target option can be used from 1.6.0
+            y_pred_log = F.log_softmax(y_pred, dim=1)
+            y_log = F.log_softmax(y, dim=1)
+            self._sum_of_kl += (
+                F.kl_div(m_log, y_pred_log, log_target=True, reduction="sum")
+                + F.kl_div(m_log, y_log, log_target=True, reduction="sum")
+            ).to(self._device)
+        else:
+            # y_pred and y are expected to be probabilities
+            self._sum_of_kl += (
+                F.kl_div(m_log, y_pred_prob, reduction="sum") + F.kl_div(m_log, y_prob, reduction="sum")
+            ).to(self._device)
 
     @sync_all_reduce("_sum_of_kl", "_num_examples")
     def compute(self) -> float:
         if self._num_examples == 0:
             raise NotComputableError("JSDivergence must have at least one example before it can be computed.")
         return self._sum_of_kl.item() / (self._num_examples * 2)
```

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/kl_divergence.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/kl_divergence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Sequence
 
 import torch
 import torch.nn.functional as F
+from packaging.version import Version
 
 from ignite.exceptions import NotComputableError
 from ignite.metrics.metric import Metric, reinit__is_reduced, sync_all_reduce
 
 __all__ = ["KLDivergence"]
 
+TORCH_VERSION_GE_160 = Version(torch.__version__) >= Version("1.6.0")
+
 
 class KLDivergence(Metric):
     r"""Calculates the mean of `Kullback-Leibler (KL) divergence
     <https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence>`_.
 
     .. math:: D_\text{KL}(\mathbf{p}_i \| \mathbf{q}_i) = \sum_{c=1}^C p_{i,c} \log \frac{p_{i,c}}{q_{i,c}}
 
@@ -87,16 +90,24 @@
             raise ValueError(f"y_pred must be in the shape of (B, C) or (B, C, ...), got {y_pred.shape}.")
 
         self._num_examples += y_pred.shape[0]
         self._update(y_pred, y)
 
     def _update(self, y_pred: torch.Tensor, y: torch.Tensor) -> None:
         y_pred = F.log_softmax(y_pred, dim=1)
-        y = F.log_softmax(y, dim=1)
-        kl_sum = F.kl_div(y_pred, y, log_target=True, reduction="sum")
+
+        if TORCH_VERSION_GE_160:
+            # log_target option can be used from 1.6.0
+            y = F.log_softmax(y, dim=1)
+            kl_sum = F.kl_div(y_pred, y, log_target=True, reduction="sum")
+        else:
+            # y is expected to be a probability tensor
+            y = F.softmax(y, dim=1)
+            kl_sum = F.kl_div(y_pred, y, reduction="sum")
+
         self._sum_of_kl += kl_sum.to(self._device)
 
     @sync_all_reduce("_sum_of_kl", "_num_examples")
     def compute(self) -> float:
         if self._num_examples == 0:
             raise NotComputableError("KLDivergence must have at least one example before it can be computed.")
         return self._sum_of_kl.item() / self._num_examples
```

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/loss.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/metric.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/mutual_information.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/mutual_information.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/precision.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/precision_recall_curve.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/psnr.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/recall.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/__init__.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/_base.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/pearson_correlation.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/r2_score.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/roc_auc.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/running_average.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/ssim.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/ignite/utils.py` & `pytorch-ignite-0.6.0.dev20240427/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/pyproject.toml` & `pytorch-ignite-0.6.0.dev20240427/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.6.0.dev20240426
+Version: 0.6.0.dev20240427
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.6.0.dev20240426/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.6.0.dev20240427/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/setup.cfg` & `pytorch-ignite-0.6.0.dev20240427/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.6.0.dev20240426/setup.py` & `pytorch-ignite-0.6.0.dev20240427/setup.py`

 * *Files identical despite different names*

