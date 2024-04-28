# Comparing `tmp/kubeflow-training-1.7.0rc0.tar.gz` & `tmp/kubeflow-training-1.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeflow-training-1.7.0rc0.tar", last modified: Mon Aug  7 13:02:53 2023, max compression
+gzip compressed data, was "kubeflow-training-1.8.0rc0.tar", last modified: Sun Apr 28 17:15:21 2024, max compression
```

## Comparing `kubeflow-training-1.7.0rc0.tar` & `kubeflow-training-1.8.0rc0.tar`

### file list

```diff
@@ -1,98 +1,107 @@
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.053903 kubeflow-training-1.7.0rc0/
--rw-r--r--   0 johnu.george   (502) staff       (20)     1172 2023-08-07 13:02:53.053446 kubeflow-training-1.7.0rc0/PKG-INFO
--rw-r--r--   0 johnu.george   (502) staff       (20)     4650 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/README.md
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.936905 kubeflow-training-1.7.0rc0/kubeflow/
--rw-r--r--   0 johnu.george   (502) staff       (20)       64 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/__init__.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.942718 kubeflow-training-1.7.0rc0/kubeflow/training/
--rw-r--r--   0 johnu.george   (502) staff       (20)     3289 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/__init__.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.944333 kubeflow-training-1.7.0rc0/kubeflow/training/api/
--rw-r--r--   0 johnu.george   (502) staff       (20)       87 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    59023 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api/training_client.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    26201 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api_client.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    12396 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/configuration.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.946778 kubeflow-training-1.7.0rc0/kubeflow/training/constants/
--rw-r--r--   0 johnu.george   (502) staff       (20)      576 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/constants/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3478 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/constants/constants.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3728 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/exceptions.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.991722 kubeflow-training-1.7.0rc0/kubeflow/training/models/
--rw-r--r--   0 johnu.george   (502) staff       (20)     2825 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    14020 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     8041 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7372 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7331 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6884 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     8054 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6861 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6267 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7822 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7412 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7037 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6216 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7062 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7550 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3887 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5455 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7157 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    10117 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_run_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6941 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6937 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7261 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6976 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4816 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    12263 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/rest.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.995394 kubeflow-training-1.7.0rc0/kubeflow/training/utils/
--rw-r--r--   0 johnu.george   (502) staff       (20)      576 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/utils/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     9600 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/utils/utils.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.000849 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/
--rw-r--r--   0 johnu.george   (502) staff       (20)     1172 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/PKG-INFO
--rw-r--r--   0 johnu.george   (502) staff       (20)     3675 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/SOURCES.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/dependency_links.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/not-zip-safe
--rw-r--r--   0 johnu.george   (502) staff       (20)      135 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/requires.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)       14 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/top_level.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)       38 2023-08-07 13:02:53.054072 kubeflow-training-1.7.0rc0/setup.cfg
--rw-r--r--   0 johnu.george   (502) staff       (20)     2256 2023-08-07 07:01:49.000000 kubeflow-training-1.7.0rc0/setup.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.026085 kubeflow-training-1.7.0rc0/test/
--rw-r--r--   0 johnu.george   (502) staff       (20)        0 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)      213 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/conftest.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.052162 kubeflow-training-1.7.0rc0/test/e2e/
--rw-r--r--   0 johnu.george   (502) staff       (20)        0 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1004 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/constants.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6838 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mpijob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     8176 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mxjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5227 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_paddlejob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6033 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_pytorchjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5188 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_tfjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6232 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_xgboostjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3180 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/utils.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2077 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1741 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_condition.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2308 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3820 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7378 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2841 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3711 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7135 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3492 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1736 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4075 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7931 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3796 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4619 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     9204 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4290 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1486 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1566 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1649 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2024 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_run_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1761 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3768 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7265 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3513 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3743 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7148 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3486 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.179813 kubeflow-training-1.8.0rc0/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1089 2024-04-28 17:15:21.179685 kubeflow-training-1.8.0rc0/PKG-INFO
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4726 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/README.md
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.162749 kubeflow-training-1.8.0rc0/kubeflow/
+-rw-r--r--   0 johnu.george   (502) staff       (20)       65 2024-04-28 12:20:08.000000 kubeflow-training-1.8.0rc0/kubeflow/__init__.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.164577 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/
+-rw-r--r--   0 johnu.george   (502) staff       (20)        0 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)      192 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/abstract_dataset_provider.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)      202 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/abstract_model_provider.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)      159 2024-04-28 11:57:21.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/constants.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3460 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/hugging_face.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2430 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/s3.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1617 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/storage_initializer/storage.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.165505 kubeflow-training-1.8.0rc0/kubeflow/training/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3339 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/__init__.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.166696 kubeflow-training-1.8.0rc0/kubeflow/training/api/
+-rw-r--r--   0 johnu.george   (502) staff       (20)       87 2024-04-28 12:20:07.000000 kubeflow-training-1.8.0rc0/kubeflow/training/api/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    56045 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/training/api/training_client.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6235 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/training/api/training_client_test.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    26201 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/api_client.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    12396 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/configuration.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.167203 kubeflow-training-1.8.0rc0/kubeflow/training/constants/
+-rw-r--r--   0 johnu.george   (502) staff       (20)      576 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/kubeflow/training/constants/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6235 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/training/constants/constants.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3728 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/exceptions.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.172347 kubeflow-training-1.8.0rc0/kubeflow/training/models/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2825 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    14020 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8041 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7372 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7331 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6884 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8054 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6861 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6267 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7822 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7412 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7037 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6216 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7062 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7550 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3887 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     5455 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7157 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    10117 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_run_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6941 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6937 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7261 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6976 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4816 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    12263 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/kubeflow/training/rest.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.172666 kubeflow-training-1.8.0rc0/kubeflow/training/utils/
+-rw-r--r--   0 johnu.george   (502) staff       (20)      576 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/kubeflow/training/utils/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    14472 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/kubeflow/training/utils/utils.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.173527 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1089 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/PKG-INFO
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4038 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/SOURCES.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)        1 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/dependency_links.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)        1 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/not-zip-safe
+-rw-r--r--   0 johnu.george   (502) staff       (20)      210 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/requires.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)       14 2024-04-28 17:15:21.000000 kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/top_level.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)       38 2024-04-28 17:15:21.179852 kubeflow-training-1.8.0rc0/setup.cfg
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2301 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/setup.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.177426 kubeflow-training-1.8.0rc0/test/
+-rw-r--r--   0 johnu.george   (502) staff       (20)        0 2024-04-28 12:20:08.000000 kubeflow-training-1.8.0rc0/test/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)      214 2024-04-28 12:20:08.000000 kubeflow-training-1.8.0rc0/test/conftest.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2024-04-28 17:15:21.179363 kubeflow-training-1.8.0rc0/test/e2e/
+-rw-r--r--   0 johnu.george   (502) staff       (20)        0 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/test/e2e/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1015 2024-03-14 09:08:53.000000 kubeflow-training-1.8.0rc0/test/e2e/constants.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7591 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_mpijob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8913 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_mxjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6012 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_paddlejob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     9358 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_pytorchjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6045 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_tfjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7075 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/test_e2e_xgboostjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3160 2024-04-28 15:52:17.000000 kubeflow-training-1.8.0rc0/test/e2e/utils.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2077 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1741 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_job_condition.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2308 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_job_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3820 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7378 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2841 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3711 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7135 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3492 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1736 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4075 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7931 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3796 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4619 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     9204 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4290 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1486 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1566 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_replica_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1649 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_replica_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2024 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_run_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1761 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3768 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7265 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3513 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3743 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7148 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3486 2024-04-28 17:13:58.000000 kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py
```

### Comparing `kubeflow-training-1.7.0rc0/PKG-INFO` & `kubeflow-training-1.8.0rc0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: kubeflow-training
-Version: 1.7.0rc0
+Version: 1.8.0rc0
 Summary: Training Operator Python SDK
-Home-page: https://github.com/kubeflow/training-operator/sdk/python
+Home-page: https://github.com/kubeflow/training-operator/tree/master/sdk/python
 Author: Kubeflow Authors
 Author-email: hejinchi@cn.ibm.com
 License: Apache License Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+Provides-Extra: huggingface
 
 Training Operator Python SDK
-
```

### Comparing `kubeflow-training-1.7.0rc0/README.md` & `kubeflow-training-1.8.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 
 ## Getting Started
 
-Please follow the [sample](examples/kubeflow-tfjob-sdk.ipynb) to create, update and delete TFJob.
+Please follow the [Getting Started guide](https://www.kubeflow.org/docs/components/training/overview/#getting-started)
+or check Training Operator [examples](../../examples).
 
 ## Documentation for API Endpoints
 
 TODO(andreyvelich): These docs are outdated. Please track this issue for the status:
 https://github.com/kubeflow/katib/issues/2081
 
 Class | Method | Description
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/__init__.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.7.0rc0"
+__version__ = "1.8.0rc0"
 
 # import apis into sdk package
 
 # import ApiClient
 from kubeflow.training.api_client import ApiClient
 from kubeflow.training.configuration import Configuration
 from kubeflow.training.exceptions import OpenApiException
@@ -52,7 +52,8 @@
 from kubeflow.training.models.kubeflow_org_v1_tf_job_list import KubeflowOrgV1TFJobList
 from kubeflow.training.models.kubeflow_org_v1_tf_job_spec import KubeflowOrgV1TFJobSpec
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job import KubeflowOrgV1XGBoostJob
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_list import KubeflowOrgV1XGBoostJobList
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_spec import KubeflowOrgV1XGBoostJobSpec
 
 from kubeflow.training.api.training_client import TrainingClient
+from kubeflow.training.constants import constants
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/api_client.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.7.0rc0/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/configuration.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -320,16 +320,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v1.7.0rc0\n"\
-               "SDK Package Version: 1.7.0rc0".\
+               "Version of the API: v1.8.0rc0\n"\
+               "SDK Package Version: 1.8.0rc0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/constants/__init__.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/exceptions.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/__init__.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # Import Kubernetes models.
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_run_policy.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_run_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/rest.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow/training/utils/__init__.py` & `kubeflow-training-1.8.0rc0/kubeflow/training/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/PKG-INFO` & `kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: kubeflow-training
-Version: 1.7.0rc0
+Version: 1.8.0rc0
 Summary: Training Operator Python SDK
-Home-page: https://github.com/kubeflow/training-operator/sdk/python
+Home-page: https://github.com/kubeflow/training-operator/tree/master/sdk/python
 Author: Kubeflow Authors
 Author-email: hejinchi@cn.ibm.com
 License: Apache License Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+Provides-Extra: huggingface
 
 Training Operator Python SDK
-
```

### Comparing `kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/SOURCES.txt` & `kubeflow-training-1.8.0rc0/kubeflow_training.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 README.md
 setup.py
 kubeflow/__init__.py
+kubeflow/storage_initializer/__init__.py
+kubeflow/storage_initializer/abstract_dataset_provider.py
+kubeflow/storage_initializer/abstract_model_provider.py
+kubeflow/storage_initializer/constants.py
+kubeflow/storage_initializer/hugging_face.py
+kubeflow/storage_initializer/s3.py
+kubeflow/storage_initializer/storage.py
 kubeflow/training/__init__.py
 kubeflow/training/api_client.py
 kubeflow/training/configuration.py
 kubeflow/training/exceptions.py
 kubeflow/training/rest.py
 kubeflow/training/api/__init__.py
 kubeflow/training/api/training_client.py
+kubeflow/training/api/training_client_test.py
 kubeflow/training/constants/__init__.py
 kubeflow/training/constants/constants.py
 kubeflow/training/models/__init__.py
 kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
 kubeflow/training/models/kubeflow_org_v1_job_condition.py
 kubeflow/training/models/kubeflow_org_v1_job_status.py
 kubeflow/training/models/kubeflow_org_v1_mpi_job.py
```

### Comparing `kubeflow-training-1.7.0rc0/setup.py` & `kubeflow-training-1.8.0rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,53 +10,60 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
-TESTS_REQUIRES = ["pytest", "pytest-tornasync", "mypy"]
+TESTS_REQUIRES = [
+    "pytest",
+    "pytest-tornasync",
+    "mypy",
+    "black==24.3.0",
+    "flake==4.0.1",
+]
 
 REQUIRES = [
     "certifi>=14.05.14",
     "six>=1.10",
     "setuptools>=21.0.0",
     "urllib3>=1.15.1",
-    "kubernetes>=23.6.0",
+    "kubernetes>=27.2.0",
     "retrying>=1.3.3",
 ]
 
 setuptools.setup(
     name="kubeflow-training",
-    version="1.7.0rc0",
+    version="1.8.0rc0",
     author="Kubeflow Authors",
     author_email="hejinchi@cn.ibm.com",
     license="Apache License Version 2.0",
-    url="https://github.com/kubeflow/training-operator/sdk/python",
+    url="https://github.com/kubeflow/training-operator/tree/master/sdk/python",
     description="Training Operator Python SDK",
     long_description="Training Operator Python SDK",
     packages=setuptools.find_packages(include=("kubeflow*")),
     package_data={},
     include_package_data=False,
     zip_safe=False,
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=REQUIRES,
     tests_require=TESTS_REQUIRES,
-    extras_require={"test": TESTS_REQUIRES},
+    extras_require={
+        "test": TESTS_REQUIRES,
+        "huggingface": ["transformers==4.37.2", "peft==0.3.0"],
+    },
 )
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/constants.py` & `kubeflow-training-1.8.0rc0/test/e2e/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 # limitations under the License.
 
 TEST_GANG_SCHEDULER_NAME_ENV_KEY = "GANG_SCHEDULER_NAME"
 TEST_GANG_SCHEDULER_NAME_SCHEDULER_PLUGINS = "scheduler-plugins"
 TEST_GANG_SCHEDULER_NAME_VOLCANO = "volcano"
 TEST_GANG_SCHEDULER_NAME_NONE = "none"
 
-GANG_SCHEDULERS = {TEST_GANG_SCHEDULER_NAME_SCHEDULER_PLUGINS, TEST_GANG_SCHEDULER_NAME_VOLCANO}
+GANG_SCHEDULERS = {
+    TEST_GANG_SCHEDULER_NAME_SCHEDULER_PLUGINS,
+    TEST_GANG_SCHEDULER_NAME_VOLCANO,
+}
 NONE_GANG_SCHEDULERS = {TEST_GANG_SCHEDULER_NAME_NONE, ""}
 
 DEFAULT_SCHEDULER_PLUGINS_NAME = "scheduler-plugins-scheduler"
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mpijob.py` & `kubeflow-training-1.8.0rc0/test/e2e/test_e2e_mpijob.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
-from typing import Tuple
+from typing import Tuple, Optional
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ResourceRequirements
 
@@ -27,132 +27,150 @@
 from kubeflow.training import KubeflowOrgV1ReplicaSpec
 from kubeflow.training import KubeflowOrgV1MPIJob
 from kubeflow.training import KubeflowOrgV1MPIJobSpec
 from kubeflow.training import KubeflowOrgV1RunPolicy
 from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
-from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
+import test.e2e.utils as utils
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("kubeflow.training.api.training_client").setLevel(logging.DEBUG)
 
-TRAINING_CLIENT = TrainingClient()
-JOB_NAME = "mpijob-mxnet-ci-test"
+TRAINING_CLIENT = TrainingClient(job_kind=constants.MPIJOB_KIND)
+JOB_NAME = "mpijob-pytorch-ci-test"
 CONTAINER_NAME = "mpi"
-GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
+GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY, "")
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
+    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS,
+    reason="For gang-scheduling",
 )
 def test_sdk_e2e_with_gang_scheduling(job_namespace):
     launcher_container, worker_container = generate_containers()
 
     launcher = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[launcher_container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[worker_container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
-    mpijob = generate_mpijob(launcher, worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
-    patched_mpijob = generate_mpijob(launcher, worker, KubeflowOrgV1SchedulingPolicy(min_available=2), job_namespace)
-
-    TRAINING_CLIENT.create_mpijob(mpijob, job_namespace)
-    logging.info(f"List of created {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(job_namespace))
-
-    verify_unschedulable_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.MPIJOB_KIND,
+    mpijob = generate_mpijob(
+        job_namespace, launcher, worker, KubeflowOrgV1SchedulingPolicy(min_available=10)
     )
-
-    TRAINING_CLIENT.patch_mpijob(patched_mpijob, JOB_NAME, job_namespace)
-    logging.info(f"List of patched {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.MPIJOB_KIND,
-        CONTAINER_NAME,
+    patched_mpijob = generate_mpijob(
+        job_namespace, launcher, worker, KubeflowOrgV1SchedulingPolicy(min_available=2)
     )
 
-    TRAINING_CLIENT.delete_mpijob(JOB_NAME, job_namespace)
+    TRAINING_CLIENT.create_job(job=mpijob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_unschedulable_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MPIJob E2E fails. Exception: {e}")
+
+    TRAINING_CLIENT.update_job(patched_mpijob, JOB_NAME, job_namespace)
+    logging.info(f"List of updated {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MPIJob E2E fails. Exception: {e}")
+
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
+    GANG_SCHEDULER_NAME in GANG_SCHEDULERS,
+    reason="For plain scheduling",
 )
 def test_sdk_e2e(job_namespace):
     launcher_container, worker_container = generate_containers()
 
     launcher = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[launcher_container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[launcher_container]),
+        ),
     )
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[worker_container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[worker_container]),
+        ),
     )
 
-    mpijob = generate_mpijob(launcher, worker, job_namespace=job_namespace)
+    mpijob = generate_mpijob(job_namespace, launcher, worker)
 
-    TRAINING_CLIENT.create_mpijob(mpijob, job_namespace)
-    logging.info(f"List of created {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(job_namespace))
+    TRAINING_CLIENT.create_job(job=mpijob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MPIJob E2E fails. Exception: {e}")
 
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.MPIJOB_KIND,
-        CONTAINER_NAME,
-    )
-
-    TRAINING_CLIENT.delete_mpijob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 def generate_mpijob(
+    job_namespace: str,
     launcher: KubeflowOrgV1ReplicaSpec,
     worker: KubeflowOrgV1ReplicaSpec,
-    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
-    job_namespace: str = "default",
+    scheduling_policy: Optional[KubeflowOrgV1SchedulingPolicy] = None,
 ) -> KubeflowOrgV1MPIJob:
     return KubeflowOrgV1MPIJob(
-        api_version="kubeflow.org/v1",
-        kind="MPIJob",
+        api_version=constants.API_VERSION,
+        kind=constants.MPIJOB_KIND,
         metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1MPIJobSpec(
             slots_per_worker=1,
             run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
@@ -160,15 +178,15 @@
         ),
     )
 
 
 def generate_containers() -> Tuple[V1Container, V1Container]:
     launcher_container = V1Container(
         name=CONTAINER_NAME,
-        image="horovod/horovod:0.20.0-tf2.3.0-torch1.6.0-mxnet1.5.0-py3.7-cpu",
+        image="horovod/horovod:0.28.1",
         command=["mpirun"],
         args=[
             "-np",
             "1",
             "--allow-run-as-root",
             "-bind-to",
             "none",
@@ -180,23 +198,22 @@
             "PATH",
             "-mca",
             "pml",
             "ob1",
             "-mca",
             "btl",
             "^openib",
-            # "python", "/examples/tensorflow2_mnist.py"]
             "python",
-            "/examples/pytorch_mnist.py",
+            "/horovod/examples/pytorch/pytorch_mnist.py",
             "--epochs",
             "1",
         ],
         resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
     )
 
     worker_container = V1Container(
-        name="mpi",
-        image="horovod/horovod:0.20.0-tf2.3.0-torch1.6.0-mxnet1.5.0-py3.7-cpu",
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
+        name=CONTAINER_NAME,
+        image="horovod/horovod:0.28.1",
+        resources=V1ResourceRequirements(limits={"memory": "3Gi", "cpu": "1.2"}),
     )
 
     return launcher_container, worker_container
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mxjob.py` & `kubeflow-training-1.8.0rc0/test/e2e/test_e2e_mxjob.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
-from typing import Tuple
+from typing import Tuple, Optional
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ContainerPort
 from kubernetes.client import V1ResourceRequirements
@@ -28,152 +28,184 @@
 from kubeflow.training import KubeflowOrgV1ReplicaSpec
 from kubeflow.training import KubeflowOrgV1MXJob
 from kubeflow.training import KubeflowOrgV1MXJobSpec
 from kubeflow.training import KubeflowOrgV1RunPolicy
 from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
-from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
+import test.e2e.utils as utils
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("kubeflow.training.api.training_client").setLevel(logging.DEBUG)
 
-TRAINING_CLIENT = TrainingClient()
+TRAINING_CLIENT = TrainingClient(job_kind=constants.MXJOB_KIND)
 JOB_NAME = "mxjob-mnist-ci-test"
 CONTAINER_NAME = "mxnet"
-GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
+GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY, "")
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
+    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS,
+    reason="For gang-scheduling",
 )
 def test_sdk_e2e_with_gang_scheduling(job_namespace):
     worker_container, server_container, scheduler_container = generate_containers()
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[worker_container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
     server = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[server_container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
     scheduler = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[scheduler_container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
-    unschedulable_mxjob = generate_mxjob(scheduler, server, worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
-    schedulable_mxjob = generate_mxjob(scheduler, server, worker, KubeflowOrgV1SchedulingPolicy(min_available=3), job_namespace)
-
-    TRAINING_CLIENT.create_mxjob(unschedulable_mxjob, job_namespace)
-    logging.info(f"List of created {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
-
-    verify_unschedulable_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
+    unschedulable_mxjob = generate_mxjob(
         job_namespace,
-        constants.MXJOB_KIND,
+        scheduler,
+        server,
+        worker,
+        KubeflowOrgV1SchedulingPolicy(min_available=10),
     )
-
-    TRAINING_CLIENT.patch_mxjob(schedulable_mxjob, JOB_NAME, job_namespace)
-    logging.info(f"List of patched {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
+    schedulable_mxjob = generate_mxjob(
         job_namespace,
-        constants.MXJOB_KIND,
-        CONTAINER_NAME,
-    )
+        scheduler,
+        server,
+        worker,
+        KubeflowOrgV1SchedulingPolicy(min_available=3),
+    )
+
+    TRAINING_CLIENT.create_job(job=unschedulable_mxjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_unschedulable_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MXJob E2E fails. Exception: {e}")
+
+    TRAINING_CLIENT.update_job(schedulable_mxjob, JOB_NAME, job_namespace)
+    logging.info(f"List of updated {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MXJob E2E fails. Exception: {e}")
 
-    TRAINING_CLIENT.delete_mxjob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
+    GANG_SCHEDULER_NAME in GANG_SCHEDULERS,
+    reason="For plain scheduling",
 )
 def test_sdk_e2e(job_namespace):
     worker_container, server_container, scheduler_container = generate_containers()
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[worker_container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[worker_container]),
+        ),
     )
 
     server = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[server_container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[server_container]),
+        ),
     )
 
     scheduler = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[scheduler_container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[scheduler_container]),
+        ),
     )
 
-    mxjob = generate_mxjob(scheduler, server, worker, job_namespace=job_namespace)
-
-    TRAINING_CLIENT.create_mxjob(mxjob, job_namespace)
-    logging.info(f"List of created {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
+    mxjob = generate_mxjob(job_namespace, scheduler, server, worker)
 
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.MXJOB_KIND,
-        CONTAINER_NAME,
-    )
+    TRAINING_CLIENT.create_job(job=mxjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"MXJob E2E fails. Exception: {e}")
 
-    TRAINING_CLIENT.delete_mxjob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 def generate_mxjob(
+    job_namespace: str,
     scheduler: KubeflowOrgV1ReplicaSpec,
     server: KubeflowOrgV1ReplicaSpec,
     worker: KubeflowOrgV1ReplicaSpec,
-    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
-    job_namespace: str = "default",
+    scheduling_policy: Optional[KubeflowOrgV1SchedulingPolicy] = None,
 ) -> KubeflowOrgV1MXJob:
     return KubeflowOrgV1MXJob(
-        api_version="kubeflow.org/v1",
-        kind="MXJob",
+        api_version=constants.API_VERSION,
+        kind=constants.MXJOB_KIND,
         metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1MXJobSpec(
             job_mode="MXTrain",
             run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
@@ -185,40 +217,37 @@
         ),
     )
 
 
 def generate_containers() -> Tuple[V1Container, V1Container, V1Container]:
     worker_container = V1Container(
         name=CONTAINER_NAME,
-        # TODO (tenzen-y): Replace the below image with the kubeflow hosted image
-        image="docker.io/johnugeorge/mxnet:1.9.1_cpu_py3",
+        image="docker.io/kubeflow/mxnet-gpu:latest",
         command=["/usr/local/bin/python3"],
         args=[
-            "incubator-mxnet/example/image-classification/train_mnist.py",
+            "/mxnet/mxnet/example/image-classification/train_mnist.py",
             "--num-epochs",
             "1",
             "--num-examples",
             "1000",
             "--kv-store",
             "dist_sync",
         ],
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
+        resources=V1ResourceRequirements(limits={"memory": "2Gi", "cpu": "0.8"}),
     )
 
     server_container = V1Container(
         name=CONTAINER_NAME,
-        # TODO (tenzen-y): Replace the below image with the kubeflow hosted image
-        image="docker.io/johnugeorge/mxnet:1.9.1_cpu_py3",
+        image="docker.io/kubeflow/mxnet-gpu:latest",
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
     )
 
     scheduler_container = V1Container(
         name=CONTAINER_NAME,
-        # TODO (tenzen-y): Replace the below image with the kubeflow hosted image
-        image="docker.io/johnugeorge/mxnet:1.9.1_cpu_py3",
+        image="docker.io/kubeflow/mxnet-gpu:latest",
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
     )
 
     return worker_container, server_container, scheduler_container
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_paddlejob.py` & `kubeflow-training-1.8.0rc0/test/e2e/test_e2e_paddlejob.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
+from typing import Optional
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ResourceRequirements
 
@@ -26,112 +27,124 @@
 from kubeflow.training import KubeflowOrgV1ReplicaSpec
 from kubeflow.training import KubeflowOrgV1PaddleJob
 from kubeflow.training import KubeflowOrgV1PaddleJobSpec
 from kubeflow.training import KubeflowOrgV1RunPolicy
 from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
-from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
+import test.e2e.utils as utils
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("kubeflow.training.api.training_client").setLevel(logging.DEBUG)
 
-TRAINING_CLIENT = TrainingClient()
+TRAINING_CLIENT = TrainingClient(job_kind=constants.PADDLEJOB_KIND)
 JOB_NAME = "paddlejob-cpu-ci-test"
 CONTAINER_NAME = "paddle"
-GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
+GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY, "")
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
+    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS,
+    reason="For gang-scheduling",
 )
 def test_sdk_e2e_with_gang_scheduling(job_namespace):
     container = generate_container()
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=2,
         restart_policy="OnFailure",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
                 containers=[container],
-            )
+            ),
         ),
     )
 
-    unschedulable_paddlejob = generate_paddlejob(worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
-    schedulable_paddlejob = generate_paddlejob(worker, KubeflowOrgV1SchedulingPolicy(min_available=2), job_namespace)
-
-    TRAINING_CLIENT.create_paddlejob(unschedulable_paddlejob, job_namespace)
-    logging.info(f"List of created {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
-
-    verify_unschedulable_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PADDLEJOB_KIND,
+    unschedulable_paddlejob = generate_paddlejob(
+        job_namespace, worker, KubeflowOrgV1SchedulingPolicy(min_available=10)
     )
-
-    TRAINING_CLIENT.patch_paddlejob(schedulable_paddlejob, JOB_NAME, job_namespace)
-    logging.info(f"List of patched {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PADDLEJOB_KIND,
-        CONTAINER_NAME,
+    schedulable_paddlejob = generate_paddlejob(
+        job_namespace, worker, KubeflowOrgV1SchedulingPolicy(min_available=2)
     )
 
-    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, job_namespace)
+    TRAINING_CLIENT.create_job(job=unschedulable_paddlejob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_unschedulable_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"PaddleJob E2E fails. Exception: {e}")
+
+    TRAINING_CLIENT.update_job(schedulable_paddlejob, JOB_NAME, job_namespace)
+    logging.info(f"List of updated {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"PaddleJob E2E fails. Exception: {e}")
+
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
+    GANG_SCHEDULER_NAME in GANG_SCHEDULERS,
+    reason="For plain scheduling",
 )
 def test_sdk_e2e(job_namespace):
     container = generate_container()
 
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=2,
         restart_policy="OnFailure",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[container])),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[container]),
+        ),
     )
 
-    paddlejob = generate_paddlejob(worker, job_namespace=job_namespace)
-
-    TRAINING_CLIENT.create_paddlejob(paddlejob, job_namespace)
-    logging.info(f"List of created {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
+    paddlejob = generate_paddlejob(job_namespace, worker)
 
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PADDLEJOB_KIND,
-        CONTAINER_NAME,
-    )
+    TRAINING_CLIENT.create_job(job=paddlejob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"PaddleJob E2E fails. Exception: {e}")
 
-    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 def generate_paddlejob(
+    job_namespace: str,
     worker: KubeflowOrgV1ReplicaSpec,
-    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
-    job_namespace: str = "default",
+    scheduling_policy: Optional[KubeflowOrgV1SchedulingPolicy] = None,
 ) -> KubeflowOrgV1PaddleJob:
     return KubeflowOrgV1PaddleJob(
-        api_version="kubeflow.org/v1",
-        kind="PaddleJob",
+        api_version=constants.API_VERSION,
+        kind=constants.PADDLEJOB_KIND,
         metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1PaddleJobSpec(
             run_policy=KubeflowOrgV1RunPolicy(
                 scheduling_policy=scheduling_policy,
                 clean_pod_policy="None",
             ),
             paddle_replica_specs={"Worker": worker},
@@ -141,9 +154,9 @@
 
 def generate_container() -> V1Container:
     return V1Container(
         name=CONTAINER_NAME,
         image="docker.io/paddlepaddle/paddle:2.4.0rc0-cpu",
         command=["python"],
         args=["-m", "paddle.distributed.launch", "run_check"],
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
+        resources=V1ResourceRequirements(limits={"memory": "2Gi", "cpu": "0.8"}),
     )
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_pytorchjob.py` & `kubeflow-training-1.8.0rc0/test/e2e/test_e2e_tfjob.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,160 +11,158 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
+from typing import Optional
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
 from kubeflow.training import KubeflowOrgV1ReplicaSpec
-from kubeflow.training import KubeflowOrgV1PyTorchJob
-from kubeflow.training import KubeflowOrgV1PyTorchJobSpec
 from kubeflow.training import KubeflowOrgV1RunPolicy
+from kubeflow.training import KubeflowOrgV1TFJob
+from kubeflow.training import KubeflowOrgV1TFJobSpec
 from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
-from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
+import test.e2e.utils as utils
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("kubeflow.training.api.training_client").setLevel(logging.DEBUG)
 
-TRAINING_CLIENT = TrainingClient()
-JOB_NAME = "pytorchjob-mnist-ci-test"
-CONTAINER_NAME = "pytorch"
-GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
+
+TRAINING_CLIENT = TrainingClient(job_kind=constants.TFJOB_KIND)
+JOB_NAME = "tfjob-mnist-ci-test"
+CONTAINER_NAME = "tensorflow"
+GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY, "")
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
+    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS,
+    reason="For gang-scheduling",
 )
 def test_sdk_e2e_with_gang_scheduling(job_namespace):
     container = generate_container()
 
-    master = KubeflowOrgV1ReplicaSpec(
-        replicas=1,
-        restart_policy="OnFailure",
-        template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-            spec=V1PodSpec(
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-                containers=[container],
-            )
-        ),
-    )
-
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="OnFailure",
+        restart_policy="Never",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
                 containers=[container],
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
-    unschedulable_pytorchjob = generate_pytorchjob(master, worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
-    schedulable_pytorchjob = generate_pytorchjob(master, worker, KubeflowOrgV1SchedulingPolicy(min_available=2), job_namespace)
-
-    TRAINING_CLIENT.create_pytorchjob(unschedulable_pytorchjob, job_namespace)
-    logging.info(f"List of created {constants.PYTORCHJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
-
-    verify_unschedulable_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PYTORCHJOB_KIND,
-    )
-
-    TRAINING_CLIENT.patch_pytorchjob(schedulable_pytorchjob, JOB_NAME, job_namespace)
-    logging.info(f"List of patched {constants.PYTORCHJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PYTORCHJOB_KIND,
-        CONTAINER_NAME,
-        timeout=900,
+    unschedulable_tfjob = generate_tfjob(
+        job_namespace, worker, KubeflowOrgV1SchedulingPolicy(min_available=10)
+    )
+    schedulable_tfjob = generate_tfjob(
+        job_namespace, worker, KubeflowOrgV1SchedulingPolicy(min_available=1)
     )
 
-    TRAINING_CLIENT.delete_pytorchjob(JOB_NAME, job_namespace)
+    TRAINING_CLIENT.create_job(job=unschedulable_tfjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_unschedulable_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"TFJob E2E fails. Exception: {e}")
+
+    TRAINING_CLIENT.update_job(schedulable_tfjob, JOB_NAME, job_namespace)
+    logging.info(f"List of updated {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"TFJob E2E fails. Exception: {e}")
+
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
+    GANG_SCHEDULER_NAME in GANG_SCHEDULERS,
+    reason="For plain scheduling",
 )
 def test_sdk_e2e(job_namespace):
     container = generate_container()
 
-    master = KubeflowOrgV1ReplicaSpec(
-        replicas=1,
-        restart_policy="OnFailure",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[container])),
-    )
-
     worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="OnFailure",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[container])),
+        restart_policy="Never",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[container]),
+        ),
     )
 
-    pytorchjob = generate_pytorchjob(master, worker, job_namespace=job_namespace)
+    tfjob = generate_tfjob(job_namespace, worker)
 
-    TRAINING_CLIENT.create_pytorchjob(pytorchjob, job_namespace)
-    logging.info(f"List of created {constants.PYTORCHJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
+    TRAINING_CLIENT.create_job(job=tfjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
 
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.PYTORCHJOB_KIND,
-        CONTAINER_NAME,
-        timeout=900,
-    )
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"TFJob E2E fails. Exception: {e}")
 
-    TRAINING_CLIENT.delete_pytorchjob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
-def generate_pytorchjob(
-    master: KubeflowOrgV1ReplicaSpec,
+def generate_tfjob(
+    job_namespace: str,
     worker: KubeflowOrgV1ReplicaSpec,
-    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
-    job_namespace: str = "default",
-) -> KubeflowOrgV1PyTorchJob:
-    return KubeflowOrgV1PyTorchJob(
-        api_version="kubeflow.org/v1",
-        kind="PyTorchJob",
+    scheduling_policy: Optional[KubeflowOrgV1SchedulingPolicy] = None,
+) -> KubeflowOrgV1TFJob:
+    return KubeflowOrgV1TFJob(
+        api_version=constants.API_VERSION,
+        kind=constants.TFJOB_KIND,
         metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
-        spec=KubeflowOrgV1PyTorchJobSpec(
+        spec=KubeflowOrgV1TFJobSpec(
             run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
-            pytorch_replica_specs={"Master": master, "Worker": worker},
+            tf_replica_specs={"Worker": worker},
         ),
     )
 
 
 def generate_container() -> V1Container:
     return V1Container(
         name=CONTAINER_NAME,
-        image="gcr.io/kubeflow-ci/pytorch-dist-mnist-test:v1.0",
-        args=["--backend", "gloo"],
-        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
+        image="gcr.io/kubeflow-ci/tf-mnist-with-summaries:1.0",
+        command=[
+            "python",
+            "/var/tf_mnist/mnist_with_summaries.py",
+            "--log_dir=/train/logs",
+            "--learning_rate=0.01",
+            "--batch_size=150",
+        ],
+        resources=V1ResourceRequirements(limits={"memory": "4Gi", "cpu": "1.6"}),
     )
```

### Comparing `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_tfjob.py` & `kubeflow-training-1.8.0rc0/test/e2e/test_e2e_xgboostjob.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,140 +11,184 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
+from typing import Optional
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
 from kubeflow.training import KubeflowOrgV1ReplicaSpec
+from kubeflow.training import KubeflowOrgV1XGBoostJob
+from kubeflow.training import KubeflowOrgV1XGBoostJobSpec
 from kubeflow.training import KubeflowOrgV1RunPolicy
-from kubeflow.training import KubeflowOrgV1TFJob
-from kubeflow.training import KubeflowOrgV1TFJobSpec
 from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
-from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
+import test.e2e.utils as utils
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
-logging.getLogger().setLevel(logging.INFO)
+logging.getLogger("kubeflow.training.api.training_client").setLevel(logging.DEBUG)
 
-TRAINING_CLIENT = TrainingClient()
-JOB_NAME = "tfjob-mnist-ci-test"
-CONTAINER_NAME = "tensorflow"
-GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
+TRAINING_CLIENT = TrainingClient(job_kind=constants.XGBOOSTJOB_KIND)
+JOB_NAME = "xgboostjob-iris-ci-test"
+CONTAINER_NAME = "xgboost"
+GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY, "")
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
+    GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS,
+    reason="For gang-scheduling",
 )
 def test_sdk_e2e_with_gang_scheduling(job_namespace):
     container = generate_container()
 
-    worker = KubeflowOrgV1ReplicaSpec(
+    master = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
+        restart_policy="OnFailure",
         template=V1PodTemplateSpec(
-            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
             spec=V1PodSpec(
                 containers=[container],
-                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            )
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
         ),
     )
 
-    unschedulable_tfjob = generate_tfjob(worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
-    schedulable_tfjob = generate_tfjob(worker, KubeflowOrgV1SchedulingPolicy(min_available=1), job_namespace)
-
-    TRAINING_CLIENT.create_tfjob(unschedulable_tfjob, job_namespace)
-    logging.info(f"List of created {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
-
-    verify_unschedulable_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.TFJOB_KIND,
+    worker = KubeflowOrgV1ReplicaSpec(
+        replicas=1,
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(
+                containers=[container],
+                scheduler_name=utils.get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            ),
+        ),
     )
 
-    TRAINING_CLIENT.patch_tfjob(schedulable_tfjob, JOB_NAME, job_namespace)
-    logging.info(f"List of patched {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT,
-        JOB_NAME,
-        job_namespace,
-        constants.TFJOB_KIND,
-        CONTAINER_NAME,
+    unschedulable_xgboostjob = generate_xgboostjob(
+        job_namespace, master, worker, KubeflowOrgV1SchedulingPolicy(min_available=10)
     )
+    schedulable_xgboostjob = generate_xgboostjob(
+        job_namespace, master, worker, KubeflowOrgV1SchedulingPolicy(min_available=2)
+    )
+
+    TRAINING_CLIENT.create_job(job=unschedulable_xgboostjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_unschedulable_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"XGBoostJob E2E fails. Exception: {e}")
+
+    TRAINING_CLIENT.update_job(schedulable_xgboostjob, JOB_NAME, job_namespace)
+    logging.info(f"List of updated {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"XGBoostJob E2E fails. Exception: {e}")
 
-    TRAINING_CLIENT.delete_tfjob(JOB_NAME, job_namespace)
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
-    GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
+    GANG_SCHEDULER_NAME in GANG_SCHEDULERS,
+    reason="For plain scheduling",
 )
 def test_sdk_e2e(job_namespace):
     container = generate_container()
 
-    worker = KubeflowOrgV1ReplicaSpec(
+    master = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
-        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
-                                   spec=V1PodSpec(containers=[container])),
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[container]),
+        ),
     )
 
-    tfjob = generate_tfjob(worker, job_namespace=job_namespace)
-
-    TRAINING_CLIENT.create_tfjob(tfjob, job_namespace)
-    logging.info(f"List of created {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
-
-    verify_job_e2e(
-        TRAINING_CLIENT, JOB_NAME, job_namespace, constants.TFJOB_KIND, CONTAINER_NAME,
+    worker = KubeflowOrgV1ReplicaSpec(
+        replicas=1,
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(
+                annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}
+            ),
+            spec=V1PodSpec(containers=[container]),
+        ),
     )
 
-    TRAINING_CLIENT.delete_tfjob(JOB_NAME, job_namespace)
-
+    xgboostjob = generate_xgboostjob(job_namespace, master, worker)
 
-def generate_tfjob(
+    TRAINING_CLIENT.create_job(job=xgboostjob, namespace=job_namespace)
+    logging.info(f"List of created {TRAINING_CLIENT.job_kind}s")
+    logging.info(TRAINING_CLIENT.list_jobs(job_namespace))
+
+    try:
+        utils.verify_job_e2e(TRAINING_CLIENT, JOB_NAME, job_namespace, wait_timeout=900)
+    except Exception as e:
+        utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+        TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+        raise Exception(f"XGBoostJob E2E fails. Exception: {e}")
+
+    utils.print_job_results(TRAINING_CLIENT, JOB_NAME, job_namespace)
+    TRAINING_CLIENT.delete_job(JOB_NAME, job_namespace)
+
+
+def generate_xgboostjob(
+    job_namespace: str,
+    master: KubeflowOrgV1ReplicaSpec,
     worker: KubeflowOrgV1ReplicaSpec,
-    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
-    job_namespace: str = "default",
-) -> KubeflowOrgV1TFJob:
-    return KubeflowOrgV1TFJob(
-        api_version="kubeflow.org/v1",
-        kind="TFJob",
+    scheduling_policy: Optional[KubeflowOrgV1SchedulingPolicy] = None,
+) -> KubeflowOrgV1XGBoostJob:
+    return KubeflowOrgV1XGBoostJob(
+        api_version=constants.API_VERSION,
+        kind=constants.XGBOOSTJOB_KIND,
         metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
-        spec=KubeflowOrgV1TFJobSpec(
+        spec=KubeflowOrgV1XGBoostJobSpec(
             run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
-            tf_replica_specs={"Worker": worker},
+            xgb_replica_specs={"Master": master, "Worker": worker},
         ),
     )
 
 
 def generate_container() -> V1Container:
     return V1Container(
         name=CONTAINER_NAME,
-        image="gcr.io/kubeflow-ci/tf-mnist-with-summaries:1.0",
-        command=[
-            "python",
-            "/var/tf_mnist/mnist_with_summaries.py",
-            "--log_dir=/train/logs",
-            "--learning_rate=0.01",
-            "--batch_size=150",
+        image="docker.io/kubeflow/xgboost-dist-iris:latest",
+        args=[
+            "--job_type=Train",
+            "--xgboost_parameter=objective:multi:softprob,num_class:3",
+            "--n_estimators=10",
+            "--learning_rate=0.1",
+            "--model_path=/tmp/xgboost-model",
+            "--model_storage_type=local",
         ],
-        resources=V1ResourceRequirements(limits={"memory": "2Gi", "cpu": "0.75"}),
+        resources=V1ResourceRequirements(limits={"memory": "2Gi", "cpu": "0.8"}),
     )
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_elastic_policy.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_elastic_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_condition.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_job_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_status.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_replica_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_status.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_replica_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_run_policy.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_run_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py` & `kubeflow-training-1.8.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.7.0rc0
+    The version of the OpenAPI document: v1.8.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

