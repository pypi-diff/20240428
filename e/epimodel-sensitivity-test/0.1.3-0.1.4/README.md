# Comparing `tmp/epimodel_sensitivity_test-0.1.3.tar.gz` & `tmp/epimodel_sensitivity_test-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epimodel_sensitivity_test-0.1.3.tar", last modified: Sun Apr 28 20:12:29 2024, max compression
+gzip compressed data, was "epimodel_sensitivity_test-0.1.4.tar", last modified: Sun Apr 28 20:18:45 2024, max compression
```

## Comparing `epimodel_sensitivity_test-0.1.3.tar` & `epimodel_sensitivity_test-0.1.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/
--rw-rw-rw-   0        0        0     2153 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.867556 epimodel_sensitivity_test-0.1.3/data/
--rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/data/age_distribution.xls
--rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/data/contact_matrices.xls
--rw-rw-rw-   0        0        0     3079 2024-04-05 11:27:45.000000 epimodel_sensitivity_test-0.1.3/data/model_parameters.json
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.883182 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-28 20:12:29.000000 epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.883182 epimodel_sensitivity_test-0.1.3/examples/
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/
--rw-rw-rw-   0        0        0      845 2024-04-28 16:22:42.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      619 2024-04-08 14:26:10.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      963 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
--rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/simulation_seihr.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.898810 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/
--rw-rw-rw-   0        0        0      548 2024-04-28 12:23:52.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      371 2024-04-28 10:08:14.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/model_seir.py
--rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/sampler_seir.py
--rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/seir_no_ag_main.py
--rw-rw-rw-   0        0        0     1542 2024-04-12 10:17:04.000000 epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/simulation_seir.py
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/
--rw-rw-rw-   0        0        0     1966 2024-04-28 12:45:38.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/contact_main.py
--rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sampler_contact.py
--rw-rw-rw-   0        0        0     3148 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sensitivity_model_contact.py
--rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/simulation_contact.py
--rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.3/examples/test.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.914435 epimodel_sensitivity_test-0.1.3/examples/utils/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/utils/__init__.py
--rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/utils/dataloader_16_ag.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/
--rw-rw-rw-   0        0        0     1574 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sampler_vaccinated.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
--rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/simulation_vacc.py
--rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/vaccinated_main.py
--rw-rw-rw-   0        0        0       42 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1269 2024-04-28 20:11:08.000000 epimodel_sensitivity_test-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.930061 epimodel_sensitivity_test-0.1.3/src/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/model/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/model/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/model/epidemic_model.py
--rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.3/src/model/matrix_generator.py
--rw-rw-rw-   0        0        0     4134 2024-04-28 15:52:31.000000 epimodel_sensitivity_test-0.1.3/src/model/model_base.py
--rw-rw-rw-   0        0        0     4715 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.3/src/model/r0.py
--rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.3/src/plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/sensitivity/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/__init__.py
--rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/prcc.py
--rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/sampler_base.py
--rw-rw-rw-   0        0        0     4874 2024-04-28 12:24:21.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/sensitivity_model_base.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.945686 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/__init__.py
--rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/output_generator.py
--rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/r0calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:29.961312 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/
--rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/__init__.py
--rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/final_size_calc.py
--rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/peak_calc.py
--rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/target_calc_base.py
--rw-rw-rw-   0        0        0     8511 2024-04-28 15:52:59.000000 epimodel_sensitivity_test-0.1.3/src/simulation_base.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.824957 epimodel_sensitivity_test-0.1.4/
+-rw-rw-rw-   0        0        0     2153 2024-04-28 20:18:45.824957 epimodel_sensitivity_test-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.730741 epimodel_sensitivity_test-0.1.4/data/
+-rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.4/data/age_distribution.xls
+-rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.4/data/contact_matrices.xls
+-rw-rw-rw-   0        0        0     3079 2024-04-05 11:27:45.000000 epimodel_sensitivity_test-0.1.4/data/model_parameters.json
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.746368 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/
+-rw-rw-rw-   0        0        0     2153 2024-04-28 20:18:45.000000 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2423 2024-04-28 20:18:45.000000 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 20:18:45.000000 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-28 20:18:45.000000 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-28 20:18:45.000000 epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.746368 epimodel_sensitivity_test-0.1.4/examples/
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.755302 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.758334 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/configs/
+-rw-rw-rw-   0        0        0      845 2024-04-28 16:22:42.000000 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      619 2024-04-08 14:26:10.000000 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      963 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
+-rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/simulation_seihr.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.762452 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.762452 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/configs/
+-rw-rw-rw-   0        0        0      548 2024-04-28 12:23:52.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      371 2024-04-28 10:08:14.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/model_seir.py
+-rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/sampler_seir.py
+-rw-rw-rw-   0        0        0      714 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/seir_no_ag_main.py
+-rw-rw-rw-   0        0        0     1542 2024-04-12 10:17:04.000000 epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/simulation_seir.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.762452 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.778078 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1966 2024-04-28 12:45:38.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      406 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/contact_main.py
+-rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/sampler_contact.py
+-rw-rw-rw-   0        0        0     3148 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/sensitivity_model_contact.py
+-rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/simulation_contact.py
+-rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.4/examples/test.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.778078 epimodel_sensitivity_test-0.1.4/examples/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/utils/__init__.py
+-rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/utils/dataloader_16_ag.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.778078 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.793706 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1574 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/sampler_vaccinated.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
+-rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/simulation_vacc.py
+-rw-rw-rw-   0        0        0      428 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/vaccinated_main.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 20:18:45.824957 epimodel_sensitivity_test-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-28 20:17:49.000000 epimodel_sensitivity_test-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.793706 epimodel_sensitivity_test-0.1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/src/dataloader.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.809330 epimodel_sensitivity_test-0.1.4/src/model/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.4/src/model/__init__.py
+-rw-rw-rw-   0        0        0     1205 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/src/model/epidemic_model.py
+-rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.4/src/model/matrix_generator.py
+-rw-rw-rw-   0        0        0     4134 2024-04-28 15:52:31.000000 epimodel_sensitivity_test-0.1.4/src/model/model_base.py
+-rw-rw-rw-   0        0        0     4715 2024-04-28 12:20:37.000000 epimodel_sensitivity_test-0.1.4/src/model/r0.py
+-rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.4/src/plotter.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.809330 epimodel_sensitivity_test-0.1.4/src/sensitivity/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/prcc.py
+-rw-rw-rw-   0        0        0     4593 2024-04-08 14:28:40.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/sampler_base.py
+-rw-rw-rw-   0        0        0     4874 2024-04-28 12:24:21.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/sensitivity_model_base.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.824957 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/output_generator.py
+-rw-rw-rw-   0        0        0     1608 2024-04-08 14:34:22.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/r0calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-28 20:18:45.824957 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/
+-rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/final_size_calc.py
+-rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/peak_calc.py
+-rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/target_calc_base.py
+-rw-rw-rw-   0        0        0     8511 2024-04-28 15:52:59.000000 epimodel_sensitivity_test-0.1.4/src/simulation_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.3/PKG-INFO` & `epimodel_sensitivity_test-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel_sensitivity_test
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.3/README.md` & `epimodel_sensitivity_test-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/data/age_distribution.xls` & `epimodel_sensitivity_test-0.1.4/data/age_distribution.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/data/contact_matrices.xls` & `epimodel_sensitivity_test-0.1.4/data/contact_matrices.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/data/model_parameters.json` & `epimodel_sensitivity_test-0.1.4/data/model_parameters.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/PKG-INFO` & `epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel-sensitivity-test
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.3/epimodel_sensitivity_test.egg-info/SOURCES.txt` & `epimodel_sensitivity_test-0.1.4/epimodel_sensitivity_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/configs/sampling_config.json` & `epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/configs/sampling_config.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/seihr_2_ag_main.py` & `epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/seihr_2_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIHR_2_age_groups/simulation_seihr.py` & `epimodel_sensitivity_test-0.1.4/examples/SEIHR_2_age_groups/simulation_seihr.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/seir_no_ag_main.py` & `epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/seir_no_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/SEIR_no_age_groups/simulation_seir.py` & `epimodel_sensitivity_test-0.1.4/examples/SEIR_no_age_groups/simulation_seir.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sampler_contact.py` & `epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/sampler_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/sensitivity_model_contact.py` & `epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/sensitivity_model_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/contact_sensitivity/simulation_contact.py` & `epimodel_sensitivity_test-0.1.4/examples/contact_sensitivity/simulation_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/utils/dataloader_16_ag.py` & `epimodel_sensitivity_test-0.1.4/examples/utils/dataloader_16_ag.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sampler_vaccinated.py` & `epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/sampler_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py` & `epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/examples/vaccinated_sensitivity/simulation_vacc.py` & `epimodel_sensitivity_test-0.1.4/examples/vaccinated_sensitivity/simulation_vacc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/setup.py` & `epimodel_sensitivity_test-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epimodel_sensitivity_test',
-    version='0.1.3',
+    version='0.1.4',
     author='Kolos Kovács',
     author_email='kovkol21@gmail.com',
     description='Efficient sensitivity analysis and evaluation of epidemiological models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KKol21/epimodel_sensitivity',
     packages=find_packages(),
@@ -23,15 +23,14 @@
     data_files=[("data", ["data/age_distribution.xls",
                           "data/contact_matrices.xls",
                           "data/model_parameters.json"])],
     install_requires=[
         "smt~=1.3.0",
         "tqdm==4.51.0",
         "xlrd==1.2.0",
-        "torch~=2.0.0",
         "torchode~=0.1.8",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `epimodel_sensitivity_test-0.1.3/src/dataloader.py` & `epimodel_sensitivity_test-0.1.4/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/model/epidemic_model.py` & `epimodel_sensitivity_test-0.1.4/src/model/epidemic_model.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/model/matrix_generator.py` & `epimodel_sensitivity_test-0.1.4/src/model/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/model/model_base.py` & `epimodel_sensitivity_test-0.1.4/src/model/model_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/model/r0.py` & `epimodel_sensitivity_test-0.1.4/src/model/r0.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/plotter.py` & `epimodel_sensitivity_test-0.1.4/src/plotter.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/prcc.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/prcc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/sampler_base.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/sampler_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/sensitivity_model_base.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/sensitivity_model_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/output_generator.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/output_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/r0calculator.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/r0calculator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/final_size_calc.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/final_size_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/peak_calc.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/peak_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/sensitivity/target_calc/sol_based/target_calc_base.py` & `epimodel_sensitivity_test-0.1.4/src/sensitivity/target_calc/sol_based/target_calc_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.3/src/simulation_base.py` & `epimodel_sensitivity_test-0.1.4/src/simulation_base.py`

 * *Files identical despite different names*

