# Comparing `tmp/epimodel_sensitivity_test-0.1.2.tar.gz` & `tmp/epimodel_sensitivity_test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epimodel_sensitivity_test-0.1.2.tar", last modified: Mon Apr  8 21:22:29 2024, max compression
+gzip compressed data, was "epimodel_sensitivity_test-0.1.3.tar", last modified: Sun Apr 28 20:12:29 2024, max compression
```

## Comparing `epimodel_sensitivity_test-0.1.2.tar` & `epimodel_sensitivity_test-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.633086 epimodel_sensitivity_test-0.1.2/
--rw-rw-rw-   0        0        0     2153 2024-04-08 21:22:29.632091 epimodel_sensitivity_test-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.491679 epimodel_sensitivity_test-0.1.2/data/
--rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.2/data/age_distribution.xls
--rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.2/data/contact_matrices.xls
--rw-rw-rw-   0        0        0     3079 2024-04-05 11:27:45.000000 epimodel_sensitivity_test-0.1.2/data/model_parameters.json
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.515223 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-04-08 21:22:29.000000 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2024-04-08 21:22:29.000000 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 21:22:29.000000 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-08 21:22:29.000000 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-08 21:22:29.000000 epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.517270 epimodel_sensitivity_test-0.1.2/examples/
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.523463 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.526517 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/configs/
--rw-rw-rw-   0        0        0     1239 2024-04-05 12:44:04.000000 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      619 2024-04-08 14:26:10.000000 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      963 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
--rw-rw-rw-   0        0        0     1694 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/simulation_seihr.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.536581 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.557057 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/configs/
--rw-rw-rw-   0        0        0      863 2024-04-08 14:52:25.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      490 2024-04-08 13:37:47.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      691 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/model_seir.py
--rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/sampler_seir.py
--rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/seir_no_ag_main.py
--rw-rw-rw-   0        0        0     1345 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/simulation_seir.py
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.567127 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.572182 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/configs/
--rw-rw-rw-   0        0        0     2790 2024-04-05 12:25:11.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/contact_main.py
--rw-rw-rw-   0        0        0      562 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/sampler_contact.py
--rw-rw-rw-   0        0        0     3171 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/sensitivity_model_contact.py
--rw-rw-rw-   0        0        0     3752 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/simulation_contact.py
--rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.2/examples/test.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.575230 epimodel_sensitivity_test-0.1.2/examples/utils/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/utils/__init__.py
--rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/utils/dataloader_16_ag.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.584382 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.589472 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/configs/
--rw-rw-rw-   0        0        0     2278 2024-04-05 11:24:43.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/sampler_vaccinated.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
--rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/simulation_vacc.py
--rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/vaccinated_main.py
--rw-rw-rw-   0        0        0       42 2024-04-08 21:22:29.633086 epimodel_sensitivity_test-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1269 2024-04-08 21:22:17.000000 epimodel_sensitivity_test-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.596545 epimodel_sensitivity_test-0.1.2/src/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/src/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.606746 epimodel_sensitivity_test-0.1.2/src/model/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.2/src/model/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/src/model/epidemic_model.py
--rw-rw-rw-   0        0        0    10205 2024-04-05 22:37:32.000000 epimodel_sensitivity_test-0.1.2/src/model/matrix_generator.py
--rw-rw-rw-   0        0        0     3963 2024-04-05 10:30:29.000000 epimodel_sensitivity_test-0.1.2/src/model/model_base.py
--rw-rw-rw-   0        0        0     4707 2024-04-05 16:11:25.000000 epimodel_sensitivity_test-0.1.2/src/model/r0.py
--rw-rw-rw-   0        0        0     5440 2024-04-06 17:24:37.000000 epimodel_sensitivity_test-0.1.2/src/plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.614862 epimodel_sensitivity_test-0.1.2/src/sensitivity/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/__init__.py
--rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/prcc.py
--rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/sampler_base.py
--rw-rw-rw-   0        0        0     4893 2024-04-08 14:52:25.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/sensitivity_model_base.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.620941 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/__init__.py
--rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/output_generator.py
--rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/r0calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:22:29.630058 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/
--rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/__init__.py
--rw-rw-rw-   0        0        0      906 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/final_size_calc.py
--rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/peak_calc.py
--rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/target_calc_base.py
--rw-rw-rw-   0        0        0     8381 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.2/src/simulation_base.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/
+-rw-rw-rw-   0        0        0     2153 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.867556 epimodel_sensitivity_test-0.1.3/data/
+-rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/data/age_distribution.xls
+-rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/data/contact_matrices.xls
+-rw-rw-rw-   0        0        0     3079 2024-04-05 11:27:45.000000 epimodel_sensitivity_test-0.1.3/data/model_parameters.json
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.883182 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/
+-rw-rw-rw-   0        0        0     2153 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2423 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.883182 epimodel_sensitivity_test-0.1.3/examples/
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/
+-rw-rw-rw-   0        0        0      845 2024-04-28 16:22:42.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      619 2024-04-08 14:26:10.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      963 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
+-rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/simulation_seihr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/
+-rw-rw-rw-   0        0        0      548 2024-04-28 12:23:52.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      371 2024-04-28 10:08:14.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/model_seir.py
+-rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/sampler_seir.py
+-rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/seir_no_ag_main.py
+-rw-rw-rw-   0        0        0     1542 2024-04-12 10:17:04.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/simulation_seir.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1966 2024-04-28 12:45:38.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/contact_main.py
+-rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sampler_contact.py
+-rw-rw-rw-   0        0        0     3148 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sensitivity_model_contact.py
+-rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/simulation_contact.py
+-rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.3/examples/test.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/utils/__init__.py
+-rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/utils/dataloader_16_ag.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1574 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sampler_vaccinated.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
+-rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/simulation_vacc.py
+-rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/vaccinated_main.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2024-04-28 20:11:08.000000 epimodel_sensitivity_test-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/src/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/dataloader.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/model/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/model/__init__.py
+-rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/model/epidemic_model.py
+-rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.3/src/model/matrix_generator.py
+-rw-rw-rw-   0        0        0     4134 2024-04-28 15:52:31.000000 epimodel_sensitivity_test-0.1.3/src/model/model_base.py
+-rw-rw-rw-   0        0        0     4715 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.3/src/model/r0.py
+-rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.3/src/plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/sensitivity/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/prcc.py
+-rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/sampler_base.py
+-rw-rw-rw-   0        0        0     4874 2024-04-28 12:24:21.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/sensitivity_model_base.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/output_generator.py
+-rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/r0calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/
+-rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/final_size_calc.py
+-rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/peak_calc.py
+-rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/target_calc_base.py
+-rw-rw-rw-   0        0        0     8511 2024-04-28 15:52:59.000000 epimodel_sensitivity_test-0.1.3/src/simulation_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.2/PKG-INFO` & `epimodel_sensitivity_test-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel_sensitivity_test
-Version: 0.1.2
+Version: 0.1.3
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.2/README.md` & `epimodel_sensitivity_test-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/data/age_distribution.xls` & `epimodel_sensitivity_test-0.1.3/data/age_distribution.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/data/contact_matrices.xls` & `epimodel_sensitivity_test-0.1.3/data/contact_matrices.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/data/model_parameters.json` & `epimodel_sensitivity_test-0.1.3/data/model_parameters.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/PKG-INFO` & `epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel-sensitivity-test
-Version: 0.1.2
+Version: 0.1.3
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.2/epimodel_sensitivity_test.egg-info/SOURCES.txt` & `epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/model_struct.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8000000000000002%*

 * *Differences: {"'states'": "{'s': {delete: ['n_substates']}, 'e': {delete: ['n_substates']}, 'i': {'type': "*

 * *             "'infected', delete: ['n_substates']}, 'h': {delete: ['type']}, 'r': {delete: "*

 * *             "['n_substates']}}",*

 * * "'transition'": "{0: {delete: ['distr', 'type']}, 1: {delete: ['type']}, 2: {delete: ['type']}, "*

 * *                 "3: {delete: ['distr', 'type']}}",*

 * * "'transmission_rules'": "{0: {'source': 's', 'actors-params': OrderedDict([('i', None)]), delete: "*

 * *                         "['infection' […]*

```diff
@@ -1,73 +1,56 @@
 {
     "states": {
         "e": {
-            "n_substates": 1,
             "type": "infected"
         },
         "h": {
-            "n_substates": 1,
-            "type": "recovering"
+            "n_substates": 1
         },
         "i": {
-            "n_substates": 1,
-            "type": "infectious"
+            "type": "infected"
         },
         "r": {
-            "n_substates": 1,
             "type": "recovered"
         },
         "s": {
-            "n_substates": 1,
             "type": "susceptible"
         }
     },
     "transition": [
         {
-            "distr": null,
             "param": "gamma",
             "source": "i",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         },
         {
             "distr": [
                 "eta_"
             ],
             "param": "alpha",
             "source": "e",
-            "target": "i",
-            "type": "basic"
+            "target": "i"
         },
         {
             "distr": [
                 "eta"
             ],
             "param": "alpha",
             "source": "e",
-            "target": "h",
-            "type": "basic"
+            "target": "h"
         },
         {
-            "distr": null,
             "param": "gamma",
             "source": "h",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         }
     ],
     "transmission_rules": [
         {
-            "infection": {
-                "actors-params": {
-                    "i": "beta"
-                },
-                "infection_params": []
-            },
-            "source": {
-                "name": "s",
-                "params": []
+            "actors-params": {
+                "i": null
             },
+            "source": "s",
             "target": "e"
         }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/configs/sampling_config.json` & `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/sampling_config.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/seihr_2_ag_main.py` & `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/seihr_2_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIHR_2_age_groups/simulation_seihr.py` & `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/simulation_seihr.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/model_struct.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6444444444444445%*

 * *Differences: {"'states'": "{'s': {delete: ['n_substates']}, 'e': {'n_substates': 3}, 'i': {'type': 'infected', "*

 * *             "'n_substates': 5}, 'r': {delete: ['n_substates']}, 'ic': OrderedDict(), 'icr': "*

 * *             "OrderedDict(), 'h': OrderedDict(), 'd': OrderedDict([('type', 'dead')]), 'v': "*

 * *             "OrderedDict([('type', 'recovered')])}",*

 * * "'transition'": "{0: {'distr': ['h_'], delete: ['type']}, 8: {delete: ['distr', 'type']}, insert: "*

 * *                 "[(1, OrderedDict([('source', 'icr'), ('target', 'r […]*

```diff
@@ -1,51 +1,100 @@
 {
     "states": {
+        "d": {
+            "type": "dead"
+        },
         "e": {
-            "n_substates": 1,
+            "n_substates": 3,
             "type": "infected"
         },
+        "h": {},
         "i": {
-            "n_substates": 1,
-            "type": "infectious"
+            "n_substates": 5,
+            "type": "infected"
         },
+        "ic": {},
+        "icr": {},
         "r": {
-            "n_substates": 1,
             "type": "recovered"
         },
         "s": {
-            "n_substates": 1,
             "type": "susceptible"
+        },
+        "v": {
+            "type": "recovered"
         }
     },
     "transition": [
         {
-            "distr": null,
+            "distr": [
+                "h_"
+            ],
+            "param": "gamma",
+            "source": "i",
+            "target": "r"
+        },
+        {
+            "param": "gamma_cr",
+            "source": "icr",
+            "target": "r"
+        },
+        {
+            "distr": [
+                "h",
+                "xi"
+            ],
             "param": "gamma",
             "source": "i",
-            "target": "r",
-            "type": "basic"
+            "target": "ic"
+        },
+        {
+            "distr": [
+                "mu"
+            ],
+            "param": "gamma_c",
+            "source": "ic",
+            "target": "d"
+        },
+        {
+            "source": "s",
+            "target": "v",
+            "type": "vaccination"
+        },
+        {
+            "distr": [
+                "h",
+                "xi_"
+            ],
+            "param": "gamma",
+            "source": "i",
+            "target": "h"
+        },
+        {
+            "param": "gamma_h",
+            "source": "h",
+            "target": "r"
+        },
+        {
+            "distr": [
+                "mu_"
+            ],
+            "param": "gamma_c",
+            "source": "ic",
+            "target": "icr"
         },
         {
-            "distr": null,
             "param": "alpha",
             "source": "e",
-            "target": "i",
-            "type": "basic"
+            "target": "i"
         }
     ],
     "transmission_rules": [
         {
-            "infection": {
-                "actors-params": {
-                    "i": null
-                },
-                "infection_params": []
-            },
-            "source": {
-                "name": "s",
-                "params": []
+            "actors-params": {
+                "i": null
             },
+            "source": "s",
             "target": "e"
         }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/seir_no_ag_main.py` & `epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/seir_no_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/SEIR_no_age_groups/simulation_seir.py` & `epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/simulation_seir.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import torch
 import os
 
+import torch
+
 from examples.SEIR_no_age_groups.model_seir import SEIRModel
 from examples.SEIR_no_age_groups.sampler_seir import SamplerSEIR
 from src.dataloader import PROJECT_PATH
 from src.simulation_base import SimulationBase
 
 
 class SimulationSEIR(SimulationBase):
@@ -15,17 +16,23 @@
         self.folder_name = os.path.join(self.folder_name, "sens_data_SEIR_no_ag")
 
         # Initalize model
         self.model = SEIRModel(sim_obj=self)
 
     def run_sampling(self):
         for variable_params in self.variable_param_combinations:
-            susc = torch.Tensor(list(variable_params["susc"].values())[0], device=self.device)
+            susc = self.tensorize(param=variable_params["susc"])
             self.params.update({"susc": susc})
             base_r0 = variable_params["r0"]
             beta = self.get_beta_from_r0(base_r0)
             self.params["beta"] = beta
 
             self.model.initialize_matrices()
 
             param_generator = SamplerSEIR(sim_obj=self, variable_params=variable_params)
             param_generator.run()
+
+    def tensorize(self, param):
+        if isinstance(param, dict):
+            return torch.Tensor(list(param.values())[0], device=self.device)
+        else:
+            return torch.Tensor(param, device=self.device)
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/model_struct.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'states'": "{'s': {delete: ['n_substates']}, 'ip': {'type': 'infected', delete: "*

 * *             "['n_substates']}, 'ia': {'type': 'infected'}, 'is': {'type': 'infected'}, 'ic': "*

 * *             "{replace: OrderedDict()}, 'icr': {replace: OrderedDict()}, 'h': {replace: "*

 * *             "OrderedDict()}, 'r': {delete: ['n_substates']}, 'd': {delete: ['n_substates']}, "*

 * *             "delete: ['v']}",*

 * * "'transition'": "{0: {delete: ['distr', 'type']}, 1: {delete: ['type']}, 2: {delete: ['distr', "*

 * *                  […]*

```diff
@@ -1,160 +1,122 @@
 {
     "states": {
         "d": {
-            "n_substates": 1,
             "type": "dead"
         },
-        "h": {
-            "n_substates": 1,
-            "type": "recovering"
-        },
+        "h": {},
         "ia": {
             "n_substates": 3,
-            "type": "infectious"
-        },
-        "ic": {
-            "n_substates": 1,
-            "type": "recovering"
-        },
-        "icr": {
-            "n_substates": 1,
-            "type": "recovering"
+            "type": "infected"
         },
+        "ic": {},
+        "icr": {},
         "ip": {
-            "n_substates": 1,
-            "type": "infectious"
+            "type": "infected"
         },
         "is": {
             "n_substates": 3,
-            "type": "infectious"
+            "type": "infected"
         },
         "l": {
             "n_substates": 2,
             "type": "infected"
         },
         "r": {
-            "n_substates": 1,
             "type": "recovered"
         },
         "s": {
-            "n_substates": 1,
             "type": "susceptible"
-        },
-        "v": {
-            "n_substates": 1,
-            "type": "recovered"
         }
     },
     "transition": [
         {
-            "distr": [],
             "param": "alpha_l",
             "source": "l",
-            "target": "ip",
-            "type": "basic"
+            "target": "ip"
         },
         {
             "distr": [
                 "p"
             ],
             "param": "alpha_p",
             "source": "ip",
-            "target": "ia",
-            "type": "basic"
+            "target": "ia"
         },
         {
-            "distr": null,
             "param": "gamma_a",
             "source": "ia",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         },
         {
             "distr": [
                 "p_"
             ],
             "param": "alpha_p",
             "source": "ip",
-            "target": "is",
-            "type": "basic"
+            "target": "is"
         },
         {
             "distr": [
                 "h_"
             ],
             "param": "gamma_s",
             "source": "is",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         },
         {
-            "distr": null,
             "param": "gamma_cr",
             "source": "icr",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         },
         {
             "distr": [
                 "h",
                 "xi"
             ],
             "param": "gamma_s",
             "source": "is",
-            "target": "ic",
-            "type": "basic"
+            "target": "ic"
         },
         {
             "distr": [
                 "mu"
             ],
             "param": "gamma_c",
             "source": "ic",
-            "target": "d",
-            "type": "basic"
+            "target": "d"
         },
         {
             "distr": [
                 "h",
                 "xi_"
             ],
             "param": "gamma_s",
             "source": "is",
-            "target": "h",
-            "type": "basic"
+            "target": "h"
         },
         {
-            "distr": null,
             "param": "gamma_h",
             "source": "h",
-            "target": "r",
-            "type": "basic"
+            "target": "r"
         },
         {
             "distr": [
                 "mu_"
             ],
             "param": "gamma_c",
             "source": "ic",
-            "target": "icr",
-            "type": "basic"
+            "target": "icr"
         }
     ],
     "transmission_rules": [
         {
-            "infection": {
-                "actors-params": {
-                    "ia": "inf_a",
-                    "ip": null,
-                    "is": null
-                },
-                "infection_params": []
-            },
-            "source": {
-                "name": "s",
-                "params": []
+            "actors-params": {
+                "ia": "inf_a",
+                "ip": null,
+                "is": null
             },
+            "source": "s",
             "target": "l"
         }
     ]
 }
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/sampler_contact.py` & `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sampler_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
         self.lhs_bounds_dict = {
             "contacts": np.array([np.full(fill_value=0.1, shape=self.sim_obj.upper_tri_size),
                                   np.full(fill_value=1, shape=self.sim_obj.upper_tri_size)]),
         }
 
     def run(self):
         lhs_table = self._get_lhs_table()
-        self._get_sim_output(lhs_table)
+        self._get_sim_output(lhs_table=lhs_table)
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/sensitivity_model_contact.py` & `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sensitivity_model_contact.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,43 +21,39 @@
 
         self.base_r0 = base_r0
         self.s_mtx = self.n_age * self.n_comp
         self.upper_tri_size = sim_obj.upper_tri_size
 
     def get_solution(self, y0, t_eval, **kwargs):
         lhs_table = kwargs["lhs_table"]
-        cm_samples = self.get_contacts_from_lhs(lhs_table)
-        betas = self._get_betas_from_contacts(cm_samples)
-        self.A = self._get_A_from_betas(betas)
-        self.T = self._get_T_from_contacts(cm_samples)
+        cm_samples = self.get_contacts_from_lhs(lhs_table=lhs_table)
+        betas = self._get_betas_from_contacts(cm_samples=cm_samples)
+        self.T = self._get_T_from_contacts(cm_samples=cm_samples, betas=betas)
         if self.is_vaccinated:
             odefun = self.get_vaccinated_ode(lhs_table.shape[0])
         else:
             odefun = self.get_basic_ode()
         return self.get_sol_from_ode(y0, t_eval, odefun)
 
-    def _get_A_from_betas(self, betas):
-        lhs_dict = {"beta": betas}
-        return self.get_matrix_from_lhs(lhs_dict=lhs_dict, matrix_name="A")
-
-    def _get_T_from_contacts(self, cm_samples: torch.Tensor):
+    def _get_T_from_contacts(self, cm_samples: torch.Tensor, betas: torch.Tensor):
         T = torch.zeros((cm_samples.size(0), self.s_mtx, self.s_mtx)).to(self.device)
-        for idx, cm in enumerate(cm_samples):
-            T[idx, :, :] = self.matrix_generator.get_T(cm)
+        for idx, (beta, cm) in enumerate(zip(cm_samples, betas)):
+            self.matrix_generator.ps.update({"beta": beta})
+            T[idx, :, :] = self.matrix_generator.get_T(cm=cm)
         return T
 
-    def _get_betas_from_contacts(self, cm_samples):
-        r0gen = R0Generator(self.data, **self.sim_obj.model_struct)
+    def _get_betas_from_contacts(self, cm_samples: torch.Tensor):
+        r0gen = R0Generator(data=self.data, **self.sim_obj.model_struct)
         betas = [self.base_r0 / r0gen.get_eig_val(contact_mtx=cm,
                                                   susceptibles=self.sim_obj.susceptibles.flatten(),
                                                   population=self.sim_obj.population)
                  for cm in cm_samples]
         return torch.tensor(betas, device=self.device)
 
-    def get_contacts_from_lhs(self, lhs_table):
+    def get_contacts_from_lhs(self, lhs_table: np.ndarray):
         contact_sim = torch.zeros((lhs_table.shape[0], self.sim_obj.n_age, self.sim_obj.n_age))
         for idx, sample in enumerate(lhs_table):
             contact_sim[idx, :, :] = get_contact_matrix_from_upper_triu(rvector=sample,
                                                                         age_vector=self.sim_obj.population.flatten())
         return contact_sim
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/contact_sensitivity/simulation_contact.py` & `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/simulation_contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 
         This method generates Latin Hypercube Sampling (LHS) samples of vaccine distributions for each parameter
         combination. The LHS tables and simulation results are saved in separate files in the 'sens_data_contact/lhs'
         and 'sens_data_contact/simulations' directories, respectively.
 
         """
         for variable_params in self.variable_param_combinations:
+            # Get beta based on base reproduction number
             base_r0 = variable_params["r0"]
-            beta = self.get_beta_from_r0(base_r0)
+            beta = self.get_beta_from_r0(base_r0=base_r0)
             self.params.update({"beta": beta})
+
             # Generate matrices used in model representation
             self.model = ContactModel(sim_obj=self, base_r0=base_r0)
             self.model.initialize_matrices()
 
             param_generator = SamplerContact(sim_obj=self, variable_params=variable_params)
             param_generator.run()
```

### Comparing `epimodel_sensitivity_test-0.1.2/examples/utils/dataloader_16_ag.py` & `epimodel_sensitivity_test-0.1.3/examples/utils/dataloader_16_ag.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/sampler_vaccinated.py` & `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sampler_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py` & `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/examples/vaccinated_sensitivity/simulation_vacc.py` & `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/simulation_vacc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/setup.py` & `epimodel_sensitivity_test-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epimodel_sensitivity_test',
-    version='0.1.2',
+    version='0.1.3',
     author='Kolos Kovács',
     author_email='kovkol21@gmail.com',
     description='Efficient sensitivity analysis and evaluation of epidemiological models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KKol21/epimodel_sensitivity',
     packages=find_packages(),
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/dataloader.py` & `epimodel_sensitivity_test-0.1.3/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/model/epidemic_model.py` & `epimodel_sensitivity_test-0.1.3/src/model/epidemic_model.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/model/matrix_generator.py` & `epimodel_sensitivity_test-0.1.3/src/model/matrix_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,39 @@
         n_comp: The number of compartments.
         c_idx: A dictionary containing the indices of different compartments.
 
     """
     trans_matrix = torch.zeros((n_age * n_comp, n_age * n_comp))
     for age_group in range(n_age):
         for state, data in states_dict.items():
-            n_states = data["n_substates"]
+            n_states = data.get("n_substates", 1)
             trans_param = parameters[get_trans_param(state, trans_data)]
             diag_idx = age_group * n_comp + c_idx[f'{state}_0']
             block_slice = slice(diag_idx, diag_idx + n_states)
             # Fill in transition block of each transitional state
             trans_matrix[block_slice, block_slice] = generate_transition_block(trans_param, n_states)
     return trans_matrix
 
 
 def get_susc_mul(tms_rule, data):
     susc_mul = torch.ones(data.n_age).to(data.device)
-    for susc_param in tms_rule["source"]["params"]:
+    for susc_param in tms_rule.get("susc_params", []):
         susc_mul *= data["params"][susc_param]
     return susc_mul
 
 
 def get_inf_mul(tms_rule, data):
     inf_mul = torch.ones(data.n_age).to(data.device)
-    for inf_param in tms_rule["infection"]["infection_params"]:
+    for inf_param in tms_rule.get("infection_params", []):
         inf_mul *= data["params"][inf_param]
     return inf_mul
 
 
 def get_distr_mul(distr: List[str], params: dict):
-    if distr is None:
+    if not distr:
         return 1
     result = 1
     for distr_param in distr:
         if distr_param[-1] == "_":
             result *= 1 - params[distr_param[:-1]]
         else:
             result *= params[distr_param]
@@ -162,62 +162,69 @@
             Torch.Tensor: When multiplied with y, the resulting tensor contains the rate of transmission for
             the susceptibles of age group i at the indices of compartments s^i and e_0^i
         """
         A = torch.zeros((self.n_eq, self.n_eq)).to(self.device)
         idx = self.idx
 
         for tms in self.tms_rules:
-            source = f"{tms['source']['name']}_0"
+            source = f"{tms['source']}_0"
             target = f"{tms['target']}_0"
             susc_mul = get_susc_mul(tms_rule=tms, data=self.data)
             transmission_rate = susc_mul / self.population
             A[idx(source), idx(source)] = - transmission_rate
             A[idx(source), idx(target)] = transmission_rate
         return A
 
     def get_T(self, cm=None) -> torch.Tensor:
         T = torch.zeros((self.n_eq, self.n_eq)).to(self.device)
         if cm is None:
             cm = self.cm
         for tms in self.tms_rules:
-            source = f"{tms['source']['name']}_0"
+            source = f"{tms['source']}_0"
             target = f"{tms['target']}_0"
             inf_mul = get_inf_mul(tms_rule=tms, data=self.data)
-            infection_spread_rate = self.ps["beta"] * cm.T * inf_mul.unsqueeze(0)  # Broadcast inf_mul to columns
-            for actor in tms["infection"]["actors-params"].keys():
-                for substate in get_substates(n_substates=self.state_data[actor]["n_substates"],
+            infection_spread_rate = self.ps["beta"] * torch.atleast_2d(cm).T * inf_mul.unsqueeze(0)  # Broadcast inf_mul to columns
+            for actor in tms["actors-params"].keys():
+                for substate in get_substates(n_substates=self.state_data[actor].get("n_substates", 1),
                                               comp_name=actor):
                     T[self._get_comp_slice(substate), self._get_comp_slice(source)] = infection_spread_rate
                     T[self._get_comp_slice(substate), self._get_comp_slice(target)] = infection_spread_rate
         return T
 
     def get_B(self) -> torch.Tensor:
         ps = self.ps
         state_data = self.state_data
         trans_data = self.trans_data
+
         # B is the tensor representing the first-order elements of the ODE system. We begin by
         # filling in the transition blocks of the intermediate states
-        intermediate_states = {state: data for state, data in state_data.items()
-                               if data["type"] not in ["susceptible",
-                                                       "recovered",
-                                                       "dead"]}
+        def is_inter(state_data):
+            return state_data.get("type", "") not in ["susceptible",
+                                                     "recovered",
+                                                     "dead"]
+
+        intermediate_states = {state: data
+                               for state, data in state_data.items()
+                               if is_inter(state_data=data)}
         B = generate_transition_matrix(states_dict=intermediate_states, trans_data=trans_data, parameters=ps,
                                        n_age=self.n_age, n_comp=self.n_comp, c_idx=self.c_idx).to(self.device)
 
         # Fill in the rest of the first-order terms
         idx = self.idx
-        end_state = {state: f"{state}_{data['n_substates'] - 1}" for state, data in state_data.items()}
-        for trans in [trans for trans in trans_data if trans["type"] == "basic"]:
+        end_state = {state: f"{state}_{data.get('n_substates', 1) - 1}"
+                     for state, data in state_data.items()}
+        for trans in [trans for trans in trans_data if trans.get("type", "basic") == "basic"]:
             # Iterate over the linear transitions
             trans_param = ps[trans["param"]]
             # Multiply the transition parameter by the distribution(s) given
-            trans_param = trans_param * get_distr_mul(trans["distr"], self.ps) # Throws shape error with *= in some cases
+            trans_param = trans_param * get_distr_mul(trans.get("distr"),
+                                                      self.ps)  # Throws shape error with *= in some cases
             source = end_state[trans["source"]]
             target = f"{trans['target']}_0"
-            n_substates = state_data[trans["source"]]["n_substates"]
+            n_substates = state_data[trans["source"]].get("n_substates", 1)
             B[idx(source), idx(target)] = trans_param * n_substates
         return B
 
     def get_V_1(self, daily_vac=None) -> torch.Tensor:
         if daily_vac is None:
             daily_vac = self.ps["daily_vac"]
         V_1 = torch.zeros((self.n_eq, self.n_eq)).to(self.device)
@@ -245,8 +252,8 @@
         Returns:
             slice: A slice representing the indices of the compartment.
 
         """
         return slice(self.c_idx[comp], self.n_eq, self.n_comp)
 
     def get_end_state(self, comp: str) -> str:
-        return f"{comp}_{self.state_data[comp]['n_substates'] - 1}"
+        return f"{comp}_{self.state_data[comp].get('n_substates', 1) - 1}"
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/model/model_base.py` & `epimodel_sensitivity_test-0.1.3/src/model/model_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.compartments = self.get_compartments()
         self.n_comp = len(self.compartments)
         self.ps = data.params
         self.device = data.device
 
         self.c_idx = {comp: idx for idx, comp in enumerate(self.compartments)}
         self.n_eq = self.n_age * self.n_comp
-        self.is_vaccinated = "vaccination" in [trans["type"] for trans in self.trans_data]
+        self.is_vaccinated = "vaccination" in [trans.get("type") for trans in self.trans_data]
 
         from src.model.matrix_generator import MatrixGenerator
         self.matrix_generator = MatrixGenerator(model=self, cm=data.cm)
 
         self.A = None
         self.T = None
         self.B = None
@@ -62,46 +62,48 @@
         dt0 = torch.full((y0.shape[0],), 1).to(self.device)
 
         return solver.solve(problem, dt0=dt0)
 
     def get_compartments(self) -> list:
         compartments = []
         for name, data in self.state_data.items():
-            compartments += get_substates(data["n_substates"], name)
+            compartments += get_substates(data.get("n_substates", 1), name)
         return compartments
 
     def get_initial_values_from_dict(self, init_val_dict: dict) -> torch.FloatTensor:
         """
 
         This method retrieves the initial values for the model based
         on the provided values in the corresponding configuration json.
 
         Returns:
             torch.Tensor: Initial values of the model.
 
         """
         iv = torch.zeros(self.n_eq).to(self.device)
-        iv[self.idx('s_0')] = self.population
+        susc_state = [state for state, data in self.state_data.items()
+                      if data.get("type") == "susceptible"][0] + "_0"
+        iv[self.idx(susc_state)] = self.population
         for comp, comp_iv in init_val_dict.items():
             comp_iv = torch.FloatTensor(comp_iv, device=self.device)
             iv[self.idx(f"{comp}_0")] = comp_iv
-            iv[self.idx('s_0')] -= comp_iv
+            iv[self.idx(susc_state)] -= comp_iv
         return iv
 
     def idx(self, state: str) -> torch.BoolTensor:
         return torch.arange(self.n_eq) % self.n_comp == self.c_idx[state]
 
     def aggregate_by_age(self, solution, comp):
         """
 
         This method aggregates the solution by age for a compartment by summing the solution
         values of individual substates for each age group.
 
         """
-        substates = get_substates(n_substates=self.state_data[comp]["n_substates"], comp_name=comp)
+        substates = get_substates(n_substates=self.state_data[comp].get("n_substates", 1), comp_name=comp)
         return torch.stack(
             tensors=[solution[:, self.idx(state)].sum(dim=1) for state in substates],
             dim=0).sum(dim=0)
 
 
 def get_substates(n_substates, comp_name):
     """
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/model/r0.py` & `epimodel_sensitivity_test-0.1.3/src/model/r0.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,21 @@
         self.i = {self.inf_states[index]: index for index in torch.arange(0, self.n_states)}
         self.s_mtx = self.n_age * self.n_states
 
         self._get_e()
 
     def isinf_state(self, state):
         return state in [state for state, data in self.state_data.items() if
-                         data["type"] in ["infected", "infectious"]]
+                         data.get("type") == "infected"]
 
     def get_infected_states(self):
         states = []
         for state, data in self.state_data.items():
             if self.isinf_state(state):
-                states += get_substates(data["n_substates"], state)
+                states += get_substates(data.get("n_substates", 1), state)
         return states
 
     def _idx(self, state: str) -> bool:
         return torch.arange(self.n_age * self.n_states) % self.n_states == self.i[state]
 
     def get_eig_val(self, susceptibles: torch.Tensor, population: torch.Tensor,
                     contact_mtx: torch.Tensor) -> float:
@@ -59,26 +59,26 @@
         """
         isinf = self.isinf_state
         inf_state_dict = {state: data for state, data in self.state_data.items() if isinf(state=state)}
         trans_mtx = generate_transition_matrix(states_dict=inf_state_dict, trans_data=self.trans_data,
                                                parameters=self.params, n_age=self.n_age,
                                                n_comp=self.n_states, c_idx=self.i).to(self.device)
 
-        end_state_dict = {state: f"{state}_{data['n_substates'] - 1}"
+        end_state_dict = {state: f"{state}_{data.get('n_substates', 1) - 1}"
                           for state, data in self.state_data.items()}
         inf_trans = [trans for trans in self.trans_data if
                      isinf(state=trans['source']) and isinf(state=trans['target'])]
         idx = self._idx
 
         for trans in inf_trans:
             source = end_state_dict[trans['source']]
             target = f"{trans['target']}_0"
             param = self.params[trans['param']]
-            n_substates = self.state_data[trans['source']]["n_substates"]
-            distr = get_distr_mul(distr=trans["distr"], params=self.params)
+            n_substates = self.state_data[trans['source']].get("n_substates", 1)
+            distr = get_distr_mul(distr=trans.get("distr"), params=self.params)
             trans_mtx[idx(source), idx(target)] = param * distr * n_substates
         return torch.linalg.inv(trans_mtx)
 
     def _get_f(self, contact_mtx: torch.Tensor) -> torch.Tensor:
         """
        Compute the matrix representing the rate of infection.
 
@@ -92,18 +92,18 @@
         s_mtx = self.s_mtx
         n_states = self.n_states
         f = torch.zeros((s_mtx, s_mtx)).to(self.device)
 
         for tms in self.tms_rules:
             susc_mul = get_susc_mul(tms_rule=tms, data=self.data)
             inf_mul = get_inf_mul(tms_rule=tms, data=self.data)
-            for actor in tms["infection"]["actors-params"]:
-                for substate in get_substates(n_substates=self.state_data[actor]["n_substates"],
+            for actor in tms["actors-params"]:
+                for substate in get_substates(n_substates=self.state_data[actor].get("n_substates", 1),
                                               comp_name=actor):
-                    f[i[substate]:s_mtx:n_states, i[f"{tms['target']}_0"]:s_mtx:n_states] =\
+                    f[i[substate]:s_mtx:n_states, i[f"{tms['target']}_0"]:s_mtx:n_states] = \
                         susc_mul * contact_mtx.T * inf_mul.unsqueeze(0)
         return f
 
     def _get_e(self):
         block = torch.zeros(self.n_states, ).to(self.device)
         block[0] = 1
         self.e = block
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/plotter.py` & `epimodel_sensitivity_test-0.1.3/src/plotter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,109 @@
 import os
 
+import networkx as nx
 import numpy as np
 from matplotlib import pyplot as plt, colors
 from matplotlib.cm import ScalarMappable
 from matplotlib.ticker import LogLocator, LogFormatter
 from matplotlib.tri import Triangulation
 
 from examples.contact_sensitivity.sensitivity_model_contact import get_rectangular_matrix_from_upper_triu
 
 
+def visualize_transmission_graph(state_data, trans_data, tms_rules):
+    plt.figure(figsize=(10, 8))
+    G = nx.DiGraph()
+
+    # Add nodes
+    def get_node_label(node):
+        if n_substates := state_data[node].get("n_substates"):
+            return f"{node}$^{{{n_substates}}}$"
+        return node
+
+    for node, data in state_data.items():
+        G.add_node(get_node_label(node))
+
+    # Add edges from transitions
+    def get_edge_label(trans):
+        if trans.get("distr"):
+            distr_muls = \
+                [distr
+                 if distr[-1] != "_"
+                 else f"(1 - {distr[:-1]})"
+                 for distr in trans["distr"]]
+            return " * ".join(distr_muls + [trans["param"]])
+        return trans.get("param", trans.get("type"))
+
+    trans_edges = [(get_node_label(transition["source"]),
+                    get_node_label(transition["target"]),
+                    get_edge_label(transition))
+                   for transition in trans_data]
+    for edge in trans_edges:
+        source, target, param = edge
+        G.add_edge(source, target, param=param)
+
+    # Add transmission rules as edges
+    tms_edges = []
+    tms_edges_unpar = []
+    for rule in tms_rules:
+        source = get_node_label(rule["source"])
+        target = get_node_label(rule["target"])
+        G.add_edge(source, target, param="beta")  # TODO: susc mul, inf mul
+        for actor, param in rule["actors-params"].items():
+            actor = get_node_label(actor)
+            if param is not None:
+                tms_edges.append((actor, source, param))
+            else:
+                tms_edges_unpar.append((actor, source))
+
+    if len(state_data) > 4:
+        pos = nx.kamada_kawai_layout(G)
+        pos = nx.arf_layout(G, pos=pos)
+    else:
+        pos = nx.circular_layout(G)
+    #pos = nx.multipartite_layout(G)  #requires manual partitioning
+    nx.draw(G, pos, with_labels=True, node_size=500, node_color="skyblue", font_size=10, arrowsize=10)
+
+    # Draw full edges with labels
+    labels = nx.get_edge_attributes(G, 'param')
+    nx.draw_networkx_edge_labels(G, pos, edge_labels=labels, font_size=7)
+
+    # Draw dashed edges and label
+    dashed_edge_labels = {(edge[0], edge[1]): edge[2] for edge in tms_edges}
+    nx.draw_networkx_edges(G, pos, edgelist=tms_edges + tms_edges_unpar,
+                           width=1, style=":")
+    nx.draw_networkx_edge_labels(G, pos, edge_labels=dashed_edge_labels, font_size=7)
+
+    plt.title("Transmission Graph")
+    plt.show()
+
+
 def generate_tornado_plot(sim_obj, labels, prcc: np.ndarray, p_val, filename: str, title=None):
     """
     Generate a tornado plot to visualize the Partial Rank Correlation Coefficient (PRCC) values.
     """
     prcc = np.round(prcc, 3)
+    prcc = np.atleast_1d(prcc)
     ys = range(len(labels))[::-1]
 
     p_val_colors = ['green', 'yellow', 'red']
     thresholds = [0, 0.01, 0.1, 1]
     cmap = colors.ListedColormap(p_val_colors)
     norm = colors.BoundaryNorm(boundaries=thresholds, ncolors=cmap.N, clip=True)
 
     sm = ScalarMappable(cmap=cmap, norm=norm)
     sm.set_array([])
     cbar = plt.colorbar(sm, orientation='vertical', shrink=0.7, pad=0.02, ax=plt.gca())
     cbar.set_label('p-values')
 
     # Plot the bars one by one
     for y, value in zip(ys, prcc):
-        facecolor = cmap(norm((p_val[len(prcc) - 1 - y])))
+        p = p_val[len(prcc) - 1 - y] if p_val.ndim > 0 else p_val
+        facecolor = cmap(norm((p)))
         plt.broken_barh(
             [(value if value < 0 else 0, abs(value))],
             (y - 0.4, 0.8),
             facecolors=[facecolor, facecolor],
             edgecolors=['black', 'black'],
             linewidth=1,
         )
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/prcc.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/prcc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/sampler_base.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/sampler_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/sensitivity_model_base.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/sensitivity_model_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,28 +84,28 @@
 
     def generate_3D_matrices(self, samples: torch.Tensor):
         spb = self.sim_obj.sampled_params_boundaries
         if spb is None:
             return
         # Params in B
         distr_params = [distr for trans in self.trans_data
-                        if trans["distr"] is not None
-                        for distr in trans["distr"]]
+                        if trans.get("distr")
+                        for distr in trans.get("distr")]
         trans_params = [trans["param"] for trans in self.trans_data]
         linear_params = [param for param in spb
                          if param in trans_params + distr_params]
         # Params in T_1
-        susc_params = [param for tms_rule in self.tms_rules for param in tms_rule["source"]["params"]]
+        susc_params = [param for tms_rule in self.tms_rules for param in tms_rule.get("susc_params", [])]
         transmission_params_left = [param for param in spb if param in susc_params]
         # Params in T_2
         actor_params = [param for tms_rule in self.tms_rules
-                        for param in tms_rule["infection"]["actors-params"].values()]
+                        for param in tms_rule["actors-params"].values()]
         inf_params = actor_params + [param for tms_rule in self.tms_rules
-                                     for param in tms_rule["infection"]["infection_params"]]
-        transmission_params_right = [param for param in spb if param in inf_params] + ["beta"]
+                                     for param in tms_rule.get("infection_params", [])]
+        transmission_params_right = [param for param in spb if param in inf_params + ["beta"]]
 
         pci = get_params_col_idx(sampled_params_boundaries=spb)
 
         tpl_lhs = get_lhs_dict(transmission_params_left, samples, pci)
         tpr_lhs = get_lhs_dict(transmission_params_right, samples, pci)
         lp_lhs = get_lhs_dict(linear_params, samples, pci)
         self.A = self.get_matrix_from_lhs(tpl_lhs, "A") if len(tpl_lhs) > 0 else self.matrix_generator.get_A()
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/output_generator.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/output_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/r0calculator.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/r0calculator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/final_size_calc.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/final_size_calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     def metric(self, sol, comp: str):
         return sol[:, -1, self.model.idx(f"{comp}_0")].sum(axis=1)
 
     def stopping_condition(self, **kwargs):
         last_val = kwargs["solutions"][:, -1, :]  # solutions.shape = (len(indices), t_limit, n_comp)
         inf_sum = torch.zeros(last_val.shape[0], device=self.model.device)
         for state, data in self.model.state_data.items():
-            if data["type"] in ["infectious"]:
+            if data.get("type") in ["infected"]:
                 inf_sum += self.model.aggregate_by_age(solution=last_val, comp=state)
         finished = inf_sum < 1e-2
         return finished, last_val
```

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/peak_calc.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/peak_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/sensitivity/target_calc/sol_based/target_calc_base.py` & `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/target_calc_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.2/src/simulation_base.py` & `epimodel_sensitivity_test-0.1.3/src/simulation_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         self.data = data
         self.device = data.device
         self.model = None
 
         self._load_simulation_data()
         self._load_config(config_path)
         self._load_model_structure(model_struct_path)
+        from src.plotter import visualize_transmission_graph
+        visualize_transmission_graph(**self.model_struct)
 
     @property
     def susceptibles(self):
         return self.model.get_initial_values()[self.model.idx("s_0")]
 
     def _load_simulation_data(self):
         self.params = self.data.params
@@ -118,50 +120,47 @@
         r0generator = R0Generator(self.data, **self.model_struct)
         if isinstance(base_r0, tuple):
             base_r0 = base_r0[0]
         return base_r0 / r0generator.get_eig_val(contact_mtx=self.cm,
                                                  susceptibles=self.susceptibles.reshape(1, -1),
                                                  population=self.population)
 
-    def calculate_prcc(self, filename):
+    def calculate_prcc(self, filename: str, target: str) -> None:
         """
 
         Calculates PRCC (Partial Rank Correlation Coefficient) values from saved LHS tables and simulation results.
 
         This method reads the saved LHS tables and simulation results for each parameter combination and calculates
         the PRCC values. The PRCC values are saved in separate files in the 'sens_data_"folder_name"/prcc' directory.
 
         """
         folder_name = self.folder_name
         os.makedirs(os.path.join(folder_name, "prcc"), exist_ok=True)
-        if "r0" == filename[-2:]:  # remove _r0
-            filename_without_target = filename[:-3]
-        else:  # remove _comp_sup / _comp_max
-            filename_without_target = filename[:filename[:filename.rfind("_")].rfind("_")]
-        lhs_path = os.path.join(folder_name, f"lhs/lhs_{filename_without_target}.csv")
-        output_path = os.path.join(folder_name, f"simulations/simulations_{filename}.csv")
+        lhs_path = os.path.join(folder_name, f"lhs/lhs_{filename}.csv")
+        output_path = os.path.join(folder_name, f"simulations/simulations_{filename}_{target}.csv")
         lhs_table = np.loadtxt(lhs_path)
         sim_output = np.loadtxt(output_path)
 
         prcc = get_prcc_values(np.c_[lhs_table, sim_output.T])
 
-        prcc_path = os.path.join(folder_name, f"prcc/prcc_{filename}.csv")
+        prcc_path = os.path.join(folder_name, f"prcc/prcc_{filename}_{target}.csv")
         np.savetxt(fname=prcc_path, X=prcc)
 
     def calculate_p_values(self, filename, significance=0.05):
         p_values_dir = os.path.join(self.folder_name, 'p_values')
         os.makedirs(p_values_dir, exist_ok=True)
 
         prcc_path = os.path.join(self.folder_name, f"prcc/prcc_{filename}.csv")
         prcc = np.loadtxt(fname=prcc_path)
 
         t = prcc * np.sqrt((self.n_samples - 2 - self.n_age) / (1 - prcc ** 2))
         # p-value for 2-sided test
         dof = self.n_samples - 2 - self.n_age
         p_values = 2 * (1 - ss.t.cdf(x=abs(t), df=dof))
+        p_values = np.atleast_1d(p_values)
 
         p_values_path = os.path.join(self.folder_name, f"p_values/p_values_{filename}.csv")
         np.savetxt(fname=p_values_path, X=p_values)
 
         is_first = True
         if len(p_values) < 30:
             for idx, p_val in enumerate(p_values):
@@ -209,14 +208,16 @@
         generate_tornado_plot(sim_obj=self,
                               labels=labels,
                               prcc=prcc,
                               p_val=p_val,
                               filename=filename)
 
     def calculate_all_prcc(self):
-        self.run_func_for_all_configs(self.calculate_prcc)
+        for variable_params, target in itertools.product(self.variable_param_combinations, self.target_vars):
+            filename = self.get_filename(variable_params)
+            self.calculate_prcc(filename=filename, target=target)
 
     def calculate_all_p_values(self):
         self.run_func_for_all_configs(self.calculate_p_values)
 
     def plot_all_prcc(self):
         self.run_func_for_all_configs(self.plot_prcc)
```

