# Comparing `tmp/lineagex-0.0.8.tar.gz` & `tmp/lineagex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.8.tar", max compression
+gzip compressed data, was "lineagex-0.0.9.tar", max compression
```

## Comparing `lineagex-0.0.8.tar` & `lineagex-0.0.9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0       55 2023-12-20 01:48:18.829734 lineagex-0.0.8/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.8/lineagex/app.js
--rw-r--r--   0        0        0    32352 2024-01-15 04:26:54.512880 lineagex-0.0.8/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    37505 2024-01-16 08:26:08.606107 lineagex-0.0.8/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     2127 2023-12-20 01:58:27.010957 lineagex-0.0.8/lineagex/example.py
--rw-r--r--   0        0        0       75 2022-10-26 09:03:26.188175 lineagex-0.0.8/lineagex/examples/dependency_example/a_table.sql
--rw-r--r--   0        0        0      251 2022-12-02 00:51:03.820262 lineagex-0.0.8/lineagex/examples/dependency_example/aa_table.sql
--rw-r--r--   0        0        0      523 2022-07-21 07:17:33.218837 lineagex-0.0.8/lineagex/examples/dependency_example/basic_patient_info.sql
--rw-r--r--   0        0        0       25 2023-05-24 02:27:29.985792 lineagex-0.0.8/lineagex/examples/dependency_example/from_aa_table.sql
--rw-r--r--   0        0        0       92 2022-10-26 09:03:35.427267 lineagex-0.0.8/lineagex/examples/dependency_example/no_dob.sql
--rw-r--r--   0        0        0       46 2023-05-23 21:49:30.792377 lineagex-0.0.8/lineagex/examples/github_example/desktop.ini
--rw-r--r--   0        0        0       77 2023-05-14 05:13:01.960169 lineagex-0.0.8/lineagex/examples/github_example/table1.sql
--rw-r--r--   0        0        0       76 2023-05-14 05:13:16.805234 lineagex-0.0.8/lineagex/examples/github_example/table2.sql
--rw-r--r--   0        0        0     2984 2023-05-17 19:49:22.688529 lineagex-0.0.8/lineagex/examples/mimic-iii/code_status.sql
--rw-r--r--   0        0        0    31332 2023-05-17 19:49:22.688529 lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql
--rw-r--r--   0        0        0    18975 2023-05-17 19:49:22.688529 lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql
--rw-r--r--   0        0        0    10347 2023-05-17 19:49:22.689529 lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql
--rw-r--r--   0        0        0     2938 2023-05-17 19:49:22.689529 lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql
--rw-r--r--   0        0        0     2925 2023-05-17 19:49:22.689529 lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql
--rw-r--r--   0        0        0     3506 2023-05-23 23:50:36.510324 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/heightweight.sql
--rw-r--r--   0        0        0     3891 2023-05-17 19:49:22.689529 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_detail.sql
--rw-r--r--   0        0        0     1396 2023-05-17 19:49:22.690529 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_hours.sql
--rw-r--r--   0        0        0     1808 2023-05-17 19:49:22.690529 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_times.sql
--rw-r--r--   0        0        0     6521 2023-05-17 19:49:22.690529 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/note_counts.sql
--rw-r--r--   0        0        0      143 2023-05-17 19:49:22.690529 lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/weight_durations.sql
--rw-r--r--   0        0        0    63797 2023-05-17 19:49:22.691529 lineagex-0.0.8/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz
--rw-r--r--   0        0        0     2172 2023-05-17 19:49:22.690529 lineagex-0.0.8/lineagex/examples/mimic-iii/diagnosis/README.md
--rw-r--r--   0        0        0     7140 2023-05-17 19:49:22.691529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/adenosine_durations.sql
--rw-r--r--   0        0        0     6273 2023-05-17 19:49:22.692529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql
--rw-r--r--   0        0        0     7217 2023-05-17 19:49:22.692529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/central_line_durations.sql
--rw-r--r--   0        0        0     6331 2023-05-17 19:49:22.692529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/crrt_durations.sql
--rw-r--r--   0        0        0     7521 2023-05-17 19:49:22.692529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql
--rw-r--r--   0        0        0     7051 2023-05-17 19:49:22.692529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql
--rw-r--r--   0        0        0     7526 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dopamine_dose.sql
--rw-r--r--   0        0        0     7056 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dopamine_durations.sql
--rw-r--r--   0        0        0     8067 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql
--rw-r--r--   0        0        0     7110 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql
--rw-r--r--   0        0        0     6979 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/isuprel_durations.sql
--rw-r--r--   0        0        0     6991 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/milrinone_durations.sql
--rw-r--r--   0        0        0     9660 2023-05-17 19:49:22.693529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql
--rw-r--r--   0        0        0     8192 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql
--rw-r--r--   0        0        0     7080 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql
--rw-r--r--   0        0        0     7541 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql
--rw-r--r--   0        0        0     7086 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql
--rw-r--r--   0        0        0     7531 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql
--rw-r--r--   0        0        0     7003 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql
--rw-r--r--   0        0        0     9595 2023-05-17 19:49:22.694529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql
--rw-r--r--   0        0        0     5576 2023-05-17 19:49:22.695529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/ventilation_classification.sql
--rw-r--r--   0        0        0     4521 2023-05-17 19:49:22.695529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/ventilation_durations.sql
--rw-r--r--   0        0        0     6839 2023-05-17 19:49:22.695529 lineagex-0.0.8/lineagex/examples/mimic-iii/durations/weight_durations.sql
--rw-r--r--   0        0        0     2346 2023-05-17 19:49:22.695529 lineagex-0.0.8/lineagex/examples/mimic-iii/echo_data.sql
--rw-r--r--   0        0        0     5885 2023-05-23 23:51:44.365020 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql
--rw-r--r--   0        0        0     5385 2023-05-23 23:24:51.648101 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql
--rw-r--r--   0        0        0      139 2023-05-17 19:49:22.696529 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/first_day_sofa.sql
--rw-r--r--   0        0        0     5015 2023-05-17 19:49:22.696529 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql
--rw-r--r--   0        0        0     2415 2023-05-17 19:49:22.696529 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/height_first_day.sql
--rw-r--r--   0        0        0     9180 2023-05-17 19:49:22.696529 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/labs_first_day.sql
--rw-r--r--   0        0        0     9357 2023-05-17 19:49:22.697528 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql
--rw-r--r--   0        0        0     2205 2023-05-17 19:49:22.697528 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql
--rw-r--r--   0        0        0     1148 2023-05-17 19:49:22.697528 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql
--rw-r--r--   0        0        0     5200 2023-05-17 19:49:22.697528 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql
--rw-r--r--   0        0        0     3766 2023-05-17 19:49:22.697528 lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/weight_first_day.sql
--rw-r--r--   0        0        0     3117 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql
--rw-r--r--   0        0        0     4388 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql
--rw-r--r--   0        0        0     2669 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql
--rw-r--r--   0        0        0     2500 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql
--rw-r--r--   0        0        0     1555 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql
--rw-r--r--   0        0        0      135 2023-05-17 19:49:22.698529 lineagex-0.0.8/lineagex/examples/mimic-iii/measurement/urine_output.sql
--rw-r--r--   0        0        0      171 2023-05-17 19:49:22.699531 lineagex-0.0.8/lineagex/examples/mimic-iii/medication/norepinephrine_equivalent_dose.sql
--rw-r--r--   0        0        0      143 2023-05-17 19:49:22.699531 lineagex-0.0.8/lineagex/examples/mimic-iii/medication/vasoactive_agent.sql
--rw-r--r--   0        0        0     1411 2023-05-17 19:49:22.699531 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql
--rw-r--r--   0        0        0     3085 2023-05-17 19:49:22.699531 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql
--rw-r--r--   0        0        0     2229 2023-05-17 19:49:22.699531 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql
--rw-r--r--   0        0        0     2223 2023-05-17 19:49:22.700528 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql
--rw-r--r--   0        0        0     3287 2023-05-17 19:49:22.700528 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql
--rw-r--r--   0        0        0     4829 2023-05-17 19:49:22.700528 lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/meld.sql
--rw-r--r--   0        0        0     3516 2023-05-17 19:49:22.701529 lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/angus.sql
--rw-r--r--   0        0        0     1035 2023-05-17 19:49:22.701529 lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/explicit.sql
--rw-r--r--   0        0        0     3954 2023-05-17 19:49:22.701529 lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/martin.sql
--rw-r--r--   0        0        0      125 2023-05-17 19:49:22.701529 lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/sepsis3.sql
--rw-r--r--   0        0        0    28187 2023-05-17 19:49:22.702529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/apsiii.sql
--rw-r--r--   0        0        0     7370 2023-05-17 19:49:22.702529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/lods.sql
--rw-r--r--   0        0        0     6878 2023-05-17 19:49:22.702529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/mlods.sql
--rw-r--r--   0        0        0     9670 2023-05-17 19:49:22.702529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/oasis.sql
--rw-r--r--   0        0        0     2594 2023-05-17 19:49:22.703529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/qsofa.sql
--rw-r--r--   0        0        0    10867 2023-05-17 19:49:22.703529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/saps.sql
--rw-r--r--   0        0        0    12484 2023-05-17 19:49:22.703529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sapsii.sql
--rw-r--r--   0        0        0     3790 2023-05-17 19:49:22.703529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sirs.sql
--rw-r--r--   0        0        0    10302 2023-05-17 19:49:22.704529 lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sofa.sql
--rw-r--r--   0        0        0     8176 2023-05-17 19:49:22.704529 lineagex-0.0.8/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql
--rw-r--r--   0        0        0     4490 2023-05-17 19:49:22.704529 lineagex-0.0.8/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql
--rw-r--r--   0        0        0    14187 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/comorbidity/charlson.sql
--rw-r--r--   0        0        0     6645 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql
--rw-r--r--   0        0        0     1645 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/age.sql
--rw-r--r--   0        0        0     1816 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_detail.sql
--rw-r--r--   0        0        0     1732 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql
--rw-r--r--   0        0        0      803 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_times.sql
--rw-r--r--   0        0        0     3921 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/weight_durations.sql
--rw-r--r--   0        0        0     2030 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_bg.sql
--rw-r--r--   0        0        0     2039 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql
--rw-r--r--   0        0        0     1758 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql
--rw-r--r--   0        0        0      757 2023-05-17 19:49:22.832517 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_height.sql
--rw-r--r--   0        0        0     7164 2023-05-17 19:49:22.833516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_lab.sql
--rw-r--r--   0        0        0      715 2023-05-17 19:49:22.833516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql
--rw-r--r--   0        0        0     9485 2023-05-17 19:49:22.833516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql
--rw-r--r--   0        0        0      686 2023-05-17 19:49:22.833516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql
--rw-r--r--   0        0        0     1389 2023-05-17 19:49:22.833516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql
--rw-r--r--   0        0        0      987 2023-05-17 19:49:22.834516 lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_weight.sql
--rw-r--r--   0        0        0     8614 2023-05-17 19:49:22.834516 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/bg.sql
--rw-r--r--   0        0        0     7196 2023-05-17 19:49:22.834516 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/blood_differential.sql
--rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.835515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql
--rw-r--r--   0        0        0     3165 2023-05-17 19:49:22.835515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/chemistry.sql
--rw-r--r--   0        0        0     1310 2023-05-17 19:49:22.835515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/coagulation.sql
--rw-r--r--   0        0        0     1578 2023-05-17 19:49:22.835515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql
--rw-r--r--   0        0        0     2136 2023-05-17 19:49:22.835515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql
--rw-r--r--   0        0        0     1835 2023-05-17 19:49:22.836515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/enzyme.sql
--rw-r--r--   0        0        0     4839 2023-05-18 04:41:01.815148 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/gcs.sql
--rw-r--r--   0        0        0     1443 2023-05-17 19:49:22.836515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/height.sql
--rw-r--r--   0        0        0      770 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/icp.sql
--rw-r--r--   0        0        0      654 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/inflammation.sql
--rw-r--r--   0        0        0      116 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/kdigo_uo.sql
--rw-r--r--   0        0        0     3793 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql
--rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/rhythm.sql
--rw-r--r--   0        0        0     1323 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/urine_output.sql
--rw-r--r--   0        0        0     4550 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql
--rw-r--r--   0        0        0     3415 2023-05-17 19:49:22.837515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql
--rw-r--r--   0        0        0     3709 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/vitalsign.sql
--rw-r--r--   0        0        0    10373 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/antibiotic.sql
--rw-r--r--   0        0        0      493 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/dobutamine.sql
--rw-r--r--   0        0        0      486 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/dopamine.sql
--rw-r--r--   0        0        0      499 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/epinephrine.sql
--rw-r--r--   0        0        0      471 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/milrinone.sql
--rw-r--r--   0        0        0      561 2023-05-17 19:49:22.838515 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/neuroblock.sql
--rw-r--r--   0        0        0      865 2023-05-17 19:49:22.839516 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/norepinephrine.sql
--rw-r--r--   0        0        0     1644 2023-05-17 19:49:22.839516 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql
--rw-r--r--   0        0        0      601 2023-05-17 19:49:22.839516 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/phenylephrine.sql
--rw-r--r--   0        0        0     4576 2023-05-17 19:49:22.839516 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql
--rw-r--r--   0        0        0      722 2023-05-17 19:49:22.839516 lineagex-0.0.8/lineagex/examples/mimic-iv/medication/vasopressin.sql
--rw-r--r--   0        0        0     2036 2023-05-17 19:49:22.840515 lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql
--rw-r--r--   0        0        0     5580 2023-05-17 19:49:22.840515 lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql
--rw-r--r--   0        0        0     3802 2023-05-17 19:49:22.840515 lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql
--rw-r--r--   0        0        0     5701 2023-05-17 19:49:22.840515 lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/meld.sql
--rw-r--r--   0        0        0      675 2023-05-17 19:49:22.831516 lineagex-0.0.8/lineagex/examples/mimic-iv/README.md
--rw-r--r--   0        0        0    33864 2023-05-17 19:49:22.841515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/apsiii.sql
--rw-r--r--   0        0        0     7695 2023-05-17 19:49:22.842515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/lods.sql
--rw-r--r--   0        0        0    11246 2023-05-17 19:49:22.842515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/oasis.sql
--rw-r--r--   0        0        0    17903 2023-05-17 19:49:22.842515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/sapsii.sql
--rw-r--r--   0        0        0     3517 2023-05-17 19:49:22.842515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/sirs.sql
--rw-r--r--   0        0        0    12603 2023-05-17 19:49:22.842515 lineagex-0.0.8/lineagex/examples/mimic-iv/score/sofa.sql
--rw-r--r--   0        0        0     2994 2023-05-17 19:49:22.843516 lineagex-0.0.8/lineagex/examples/mimic-iv/sepsis/sepsis3.sql
--rw-r--r--   0        0        0     6418 2023-05-17 19:49:22.843516 lineagex-0.0.8/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql
--rw-r--r--   0        0        0     6011 2023-05-17 19:49:22.843516 lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/crrt.sql
--rw-r--r--   0        0        0     4777 2023-05-17 19:49:22.843516 lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/invasive_line.sql
--rw-r--r--   0        0        0    13683 2023-05-18 23:24:29.938626 lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/rrt.sql
--rw-r--r--   0        0        0     9285 2023-05-17 19:49:22.843516 lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/ventilation.sql
--rw-r--r--   0        0        0     2594 2023-12-20 02:04:37.027268 lineagex-0.0.8/lineagex/lineagex.py
--rw-r--r--   0        0        0     5257 2024-01-17 04:06:33.265046 lineagex-0.0.8/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    14603 2024-01-15 04:31:56.690721 lineagex-0.0.8/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7650 2024-01-16 04:26:29.929435 lineagex-0.0.8/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1456 2023-12-20 01:48:18.839662 lineagex-0.0.8/lineagex/stack.py
--rw-r--r--   0        0        0     7665 2024-01-16 08:26:29.295666 lineagex-0.0.8/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.8/lineagex/vendor.js
--rw-r--r--   0        0        0      448 2024-01-17 07:05:45.270324 lineagex-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3388 2023-05-29 23:23:52.325162 lineagex-0.0.8/README.md
--rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 lineagex-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-12-20 01:48:18.829734 lineagex-0.0.9/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.9/lineagex/app.js
+-rw-r--r--   0        0        0    32352 2024-01-15 04:26:54.512880 lineagex-0.0.9/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    37505 2024-01-16 08:26:08.606107 lineagex-0.0.9/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     2127 2023-12-20 01:58:27.010957 lineagex-0.0.9/lineagex/example.py
+-rw-r--r--   0        0        0       75 2022-10-26 09:03:26.188175 lineagex-0.0.9/lineagex/examples/dependency_example/a_table.sql
+-rw-r--r--   0        0        0      251 2022-12-02 00:51:03.820262 lineagex-0.0.9/lineagex/examples/dependency_example/aa_table.sql
+-rw-r--r--   0        0        0      523 2022-07-21 07:17:33.218837 lineagex-0.0.9/lineagex/examples/dependency_example/basic_patient_info.sql
+-rw-r--r--   0        0        0       25 2023-05-24 02:27:29.985792 lineagex-0.0.9/lineagex/examples/dependency_example/from_aa_table.sql
+-rw-r--r--   0        0        0       92 2022-10-26 09:03:35.427267 lineagex-0.0.9/lineagex/examples/dependency_example/no_dob.sql
+-rw-r--r--   0        0        0       46 2023-05-23 21:49:30.792377 lineagex-0.0.9/lineagex/examples/github_example/desktop.ini
+-rw-r--r--   0        0        0       77 2023-05-14 05:13:01.960169 lineagex-0.0.9/lineagex/examples/github_example/table1.sql
+-rw-r--r--   0        0        0       76 2023-05-14 05:13:16.805234 lineagex-0.0.9/lineagex/examples/github_example/table2.sql
+-rw-r--r--   0        0        0     2984 2023-05-17 19:49:22.688529 lineagex-0.0.9/lineagex/examples/mimic-iii/code_status.sql
+-rw-r--r--   0        0        0    31332 2023-05-17 19:49:22.688529 lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql
+-rw-r--r--   0        0        0    18975 2023-05-17 19:49:22.688529 lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql
+-rw-r--r--   0        0        0    10347 2023-05-17 19:49:22.689529 lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql
+-rw-r--r--   0        0        0     2938 2023-05-17 19:49:22.689529 lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql
+-rw-r--r--   0        0        0     2925 2023-05-17 19:49:22.689529 lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql
+-rw-r--r--   0        0        0     3506 2023-05-23 23:50:36.510324 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/heightweight.sql
+-rw-r--r--   0        0        0     3891 2023-05-17 19:49:22.689529 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1396 2023-05-17 19:49:22.690529 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_hours.sql
+-rw-r--r--   0        0        0     1808 2023-05-17 19:49:22.690529 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     6521 2023-05-17 19:49:22.690529 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/note_counts.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.690529 lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/weight_durations.sql
+-rw-r--r--   0        0        0    63797 2023-05-17 19:49:22.691529 lineagex-0.0.9/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz
+-rw-r--r--   0        0        0     2172 2023-05-17 19:49:22.690529 lineagex-0.0.9/lineagex/examples/mimic-iii/diagnosis/README.md
+-rw-r--r--   0        0        0     7140 2023-05-17 19:49:22.691529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/adenosine_durations.sql
+-rw-r--r--   0        0        0     6273 2023-05-17 19:49:22.692529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql
+-rw-r--r--   0        0        0     7217 2023-05-17 19:49:22.692529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/central_line_durations.sql
+-rw-r--r--   0        0        0     6331 2023-05-17 19:49:22.692529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/crrt_durations.sql
+-rw-r--r--   0        0        0     7521 2023-05-17 19:49:22.692529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql
+-rw-r--r--   0        0        0     7051 2023-05-17 19:49:22.692529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql
+-rw-r--r--   0        0        0     7526 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dopamine_dose.sql
+-rw-r--r--   0        0        0     7056 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dopamine_durations.sql
+-rw-r--r--   0        0        0     8067 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql
+-rw-r--r--   0        0        0     7110 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql
+-rw-r--r--   0        0        0     6979 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/isuprel_durations.sql
+-rw-r--r--   0        0        0     6991 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/milrinone_durations.sql
+-rw-r--r--   0        0        0     9660 2023-05-17 19:49:22.693529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql
+-rw-r--r--   0        0        0     8192 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql
+-rw-r--r--   0        0        0     7080 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql
+-rw-r--r--   0        0        0     7541 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql
+-rw-r--r--   0        0        0     7086 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql
+-rw-r--r--   0        0        0     7531 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql
+-rw-r--r--   0        0        0     7003 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql
+-rw-r--r--   0        0        0     9595 2023-05-17 19:49:22.694529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql
+-rw-r--r--   0        0        0     5576 2023-05-17 19:49:22.695529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/ventilation_classification.sql
+-rw-r--r--   0        0        0     4521 2023-05-17 19:49:22.695529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/ventilation_durations.sql
+-rw-r--r--   0        0        0     6839 2023-05-17 19:49:22.695529 lineagex-0.0.9/lineagex/examples/mimic-iii/durations/weight_durations.sql
+-rw-r--r--   0        0        0     2346 2023-05-17 19:49:22.695529 lineagex-0.0.9/lineagex/examples/mimic-iii/echo_data.sql
+-rw-r--r--   0        0        0     5885 2023-05-23 23:51:44.365020 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql
+-rw-r--r--   0        0        0     5385 2023-05-23 23:24:51.648101 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql
+-rw-r--r--   0        0        0      139 2023-05-17 19:49:22.696529 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0     5015 2023-05-17 19:49:22.696529 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql
+-rw-r--r--   0        0        0     2415 2023-05-17 19:49:22.696529 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/height_first_day.sql
+-rw-r--r--   0        0        0     9180 2023-05-17 19:49:22.696529 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/labs_first_day.sql
+-rw-r--r--   0        0        0     9357 2023-05-17 19:49:22.697528 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql
+-rw-r--r--   0        0        0     2205 2023-05-17 19:49:22.697528 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql
+-rw-r--r--   0        0        0     1148 2023-05-17 19:49:22.697528 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql
+-rw-r--r--   0        0        0     5200 2023-05-17 19:49:22.697528 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql
+-rw-r--r--   0        0        0     3766 2023-05-17 19:49:22.697528 lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/weight_first_day.sql
+-rw-r--r--   0        0        0     3117 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql
+-rw-r--r--   0        0        0     4388 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql
+-rw-r--r--   0        0        0     2669 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql
+-rw-r--r--   0        0        0     2500 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql
+-rw-r--r--   0        0        0     1555 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql
+-rw-r--r--   0        0        0      135 2023-05-17 19:49:22.698529 lineagex-0.0.9/lineagex/examples/mimic-iii/measurement/urine_output.sql
+-rw-r--r--   0        0        0      171 2023-05-17 19:49:22.699531 lineagex-0.0.9/lineagex/examples/mimic-iii/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.699531 lineagex-0.0.9/lineagex/examples/mimic-iii/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0     1411 2023-05-17 19:49:22.699531 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     3085 2023-05-17 19:49:22.699531 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     2229 2023-05-17 19:49:22.699531 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql
+-rw-r--r--   0        0        0     2223 2023-05-17 19:49:22.700528 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql
+-rw-r--r--   0        0        0     3287 2023-05-17 19:49:22.700528 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     4829 2023-05-17 19:49:22.700528 lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/meld.sql
+-rw-r--r--   0        0        0     3516 2023-05-17 19:49:22.701529 lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/angus.sql
+-rw-r--r--   0        0        0     1035 2023-05-17 19:49:22.701529 lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/explicit.sql
+-rw-r--r--   0        0        0     3954 2023-05-17 19:49:22.701529 lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/martin.sql
+-rw-r--r--   0        0        0      125 2023-05-17 19:49:22.701529 lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0    28187 2023-05-17 19:49:22.702529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/apsiii.sql
+-rw-r--r--   0        0        0     7370 2023-05-17 19:49:22.702529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/lods.sql
+-rw-r--r--   0        0        0     6878 2023-05-17 19:49:22.702529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/mlods.sql
+-rw-r--r--   0        0        0     9670 2023-05-17 19:49:22.702529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/oasis.sql
+-rw-r--r--   0        0        0     2594 2023-05-17 19:49:22.703529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/qsofa.sql
+-rw-r--r--   0        0        0    10867 2023-05-17 19:49:22.703529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/saps.sql
+-rw-r--r--   0        0        0    12484 2023-05-17 19:49:22.703529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sapsii.sql
+-rw-r--r--   0        0        0     3790 2023-05-17 19:49:22.703529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sirs.sql
+-rw-r--r--   0        0        0    10302 2023-05-17 19:49:22.704529 lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sofa.sql
+-rw-r--r--   0        0        0     8176 2023-05-17 19:49:22.704529 lineagex-0.0.9/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql
+-rw-r--r--   0        0        0     4490 2023-05-17 19:49:22.704529 lineagex-0.0.9/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql
+-rw-r--r--   0        0        0    14187 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/comorbidity/charlson.sql
+-rw-r--r--   0        0        0     6645 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql
+-rw-r--r--   0        0        0     1645 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/age.sql
+-rw-r--r--   0        0        0     1816 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1732 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql
+-rw-r--r--   0        0        0      803 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     3921 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/weight_durations.sql
+-rw-r--r--   0        0        0     2030 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_bg.sql
+-rw-r--r--   0        0        0     2039 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql
+-rw-r--r--   0        0        0     1758 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql
+-rw-r--r--   0        0        0      757 2023-05-17 19:49:22.832517 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_height.sql
+-rw-r--r--   0        0        0     7164 2023-05-17 19:49:22.833516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_lab.sql
+-rw-r--r--   0        0        0      715 2023-05-17 19:49:22.833516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql
+-rw-r--r--   0        0        0     9485 2023-05-17 19:49:22.833516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0      686 2023-05-17 19:49:22.833516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql
+-rw-r--r--   0        0        0     1389 2023-05-17 19:49:22.833516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql
+-rw-r--r--   0        0        0      987 2023-05-17 19:49:22.834516 lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_weight.sql
+-rw-r--r--   0        0        0     8614 2023-05-17 19:49:22.834516 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/bg.sql
+-rw-r--r--   0        0        0     7196 2023-05-17 19:49:22.834516 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/blood_differential.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.835515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql
+-rw-r--r--   0        0        0     3165 2023-05-17 19:49:22.835515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/chemistry.sql
+-rw-r--r--   0        0        0     1310 2023-05-17 19:49:22.835515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/coagulation.sql
+-rw-r--r--   0        0        0     1578 2023-05-17 19:49:22.835515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql
+-rw-r--r--   0        0        0     2136 2023-05-17 19:49:22.835515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql
+-rw-r--r--   0        0        0     1835 2023-05-17 19:49:22.836515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/enzyme.sql
+-rw-r--r--   0        0        0     4839 2023-05-18 04:41:01.815148 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/gcs.sql
+-rw-r--r--   0        0        0     1443 2023-05-17 19:49:22.836515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/height.sql
+-rw-r--r--   0        0        0      770 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/icp.sql
+-rw-r--r--   0        0        0      654 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/inflammation.sql
+-rw-r--r--   0        0        0      116 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/kdigo_uo.sql
+-rw-r--r--   0        0        0     3793 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/rhythm.sql
+-rw-r--r--   0        0        0     1323 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/urine_output.sql
+-rw-r--r--   0        0        0     4550 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql
+-rw-r--r--   0        0        0     3415 2023-05-17 19:49:22.837515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql
+-rw-r--r--   0        0        0     3709 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/vitalsign.sql
+-rw-r--r--   0        0        0    10373 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/antibiotic.sql
+-rw-r--r--   0        0        0      493 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/dobutamine.sql
+-rw-r--r--   0        0        0      486 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/dopamine.sql
+-rw-r--r--   0        0        0      499 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/epinephrine.sql
+-rw-r--r--   0        0        0      471 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/milrinone.sql
+-rw-r--r--   0        0        0      561 2023-05-17 19:49:22.838515 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/neuroblock.sql
+-rw-r--r--   0        0        0      865 2023-05-17 19:49:22.839516 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/norepinephrine.sql
+-rw-r--r--   0        0        0     1644 2023-05-17 19:49:22.839516 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      601 2023-05-17 19:49:22.839516 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/phenylephrine.sql
+-rw-r--r--   0        0        0     4576 2023-05-17 19:49:22.839516 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0      722 2023-05-17 19:49:22.839516 lineagex-0.0.9/lineagex/examples/mimic-iv/medication/vasopressin.sql
+-rw-r--r--   0        0        0     2036 2023-05-17 19:49:22.840515 lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     5580 2023-05-17 19:49:22.840515 lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     3802 2023-05-17 19:49:22.840515 lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     5701 2023-05-17 19:49:22.840515 lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/meld.sql
+-rw-r--r--   0        0        0      675 2023-05-17 19:49:22.831516 lineagex-0.0.9/lineagex/examples/mimic-iv/README.md
+-rw-r--r--   0        0        0    33864 2023-05-17 19:49:22.841515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/apsiii.sql
+-rw-r--r--   0        0        0     7695 2023-05-17 19:49:22.842515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/lods.sql
+-rw-r--r--   0        0        0    11246 2023-05-17 19:49:22.842515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/oasis.sql
+-rw-r--r--   0        0        0    17903 2023-05-17 19:49:22.842515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/sapsii.sql
+-rw-r--r--   0        0        0     3517 2023-05-17 19:49:22.842515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/sirs.sql
+-rw-r--r--   0        0        0    12603 2023-05-17 19:49:22.842515 lineagex-0.0.9/lineagex/examples/mimic-iv/score/sofa.sql
+-rw-r--r--   0        0        0     2994 2023-05-17 19:49:22.843516 lineagex-0.0.9/lineagex/examples/mimic-iv/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0     6418 2023-05-17 19:49:22.843516 lineagex-0.0.9/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql
+-rw-r--r--   0        0        0     6011 2023-05-17 19:49:22.843516 lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/crrt.sql
+-rw-r--r--   0        0        0     4777 2023-05-17 19:49:22.843516 lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/invasive_line.sql
+-rw-r--r--   0        0        0    13683 2023-05-18 23:24:29.938626 lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/rrt.sql
+-rw-r--r--   0        0        0     9285 2023-05-17 19:49:22.843516 lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/ventilation.sql
+-rw-r--r--   0        0        0     2594 2023-12-20 02:04:37.027268 lineagex-0.0.9/lineagex/lineagex.py
+-rw-r--r--   0        0        0     6008 2024-01-17 08:46:02.760113 lineagex-0.0.9/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    15341 2024-01-17 08:46:08.539181 lineagex-0.0.9/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7650 2024-01-16 04:26:29.929435 lineagex-0.0.9/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1456 2023-12-20 01:48:18.839662 lineagex-0.0.9/lineagex/stack.py
+-rw-r--r--   0        0        0     7665 2024-01-16 08:26:29.295666 lineagex-0.0.9/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.9/lineagex/vendor.js
+-rw-r--r--   0        0        0      448 2024-01-17 08:46:58.135511 lineagex-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3388 2023-05-29 23:23:52.325162 lineagex-0.0.9/README.md
+-rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 lineagex-0.0.9/PKG-INFO
```

### Comparing `lineagex-0.0.8/lineagex/app.js` & `lineagex-0.0.9/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/ColumnLineage.py` & `lineagex-0.0.9/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.9/lineagex/ColumnLineageNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/example.py` & `lineagex-0.0.9/lineagex/example.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/dependency_example/basic_patient_info.sql` & `lineagex-0.0.9/lineagex/examples/dependency_example/basic_patient_info.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/code_status.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/code_status.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/heightweight.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/heightweight.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_detail.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_detail.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_hours.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_hours.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/icustay_times.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/icustay_times.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/demographics/note_counts.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/demographics/note_counts.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz` & `lineagex-0.0.9/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/diagnosis/README.md` & `lineagex-0.0.9/lineagex/examples/mimic-iii/diagnosis/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/adenosine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/adenosine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/central_line_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/central_line_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/crrt_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/crrt_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dopamine_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dopamine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/dopamine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/dopamine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/isuprel_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/isuprel_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/milrinone_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/milrinone_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/ventilation_classification.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/ventilation_classification.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/ventilation_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/ventilation_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/durations/weight_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/durations/weight_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/echo_data.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/echo_data.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/height_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/height_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/labs_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/labs_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/firstday/weight_first_day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/firstday/weight_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/organfailure/meld.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/organfailure/meld.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/angus.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/angus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/explicit.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/explicit.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/sepsis/martin.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/sepsis/martin.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/apsiii.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/apsiii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/lods.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/lods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/mlods.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/mlods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/oasis.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/oasis.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/qsofa.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/qsofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/saps.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/saps.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sapsii.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sapsii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sirs.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sirs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/severityscores/sofa.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/severityscores/sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/comorbidity/charlson.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/comorbidity/charlson.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/age.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/age.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_detail.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_detail.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/icustay_times.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/icustay_times.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/demographics/weight_durations.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/demographics/weight_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_bg.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_bg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_height.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_height.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_lab.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_lab.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/firstday/first_day_weight.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/firstday/first_day_weight.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/bg.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/bg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/blood_differential.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/blood_differential.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/chemistry.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/chemistry.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/coagulation.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/coagulation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/enzyme.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/enzyme.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/gcs.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/gcs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/height.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/height.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/icp.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/icp.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/inflammation.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/inflammation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/rhythm.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/rhythm.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/urine_output.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/measurement/vitalsign.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/measurement/vitalsign.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/antibiotic.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/antibiotic.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/neuroblock.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/neuroblock.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/norepinephrine.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/norepinephrine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/phenylephrine.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/phenylephrine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/medication/vasopressin.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/medication/vasopressin.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/organfailure/meld.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/organfailure/meld.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/README.md` & `lineagex-0.0.9/lineagex/examples/mimic-iv/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/apsiii.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/apsiii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/lods.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/lods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/oasis.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/oasis.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/sapsii.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/sapsii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/sirs.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/sirs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/score/sofa.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/score/sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/sepsis/sepsis3.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/sepsis/sepsis3.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/crrt.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/crrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/invasive_line.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/invasive_line.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/rrt.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/rrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/examples/mimic-iv/treatment/ventilation.sql` & `lineagex-0.0.9/lineagex/examples/mimic-iv/treatment/ventilation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/lineagex.py` & `lineagex-0.0.9/lineagex/lineagex.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/LineageXNoConn.py` & `lineagex-0.0.9/lineagex/LineageXNoConn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,85 @@
+import time
 from typing import List
 from typing import Optional
 
 from sqlglot import exp, expressions, parse_one
 
 from .ColumnLineageNoConn import ColumnLineageNoConn
 from .SqlToDict import SqlToDict
 from .utils import produce_json
 
 
+def parse_one_sql(sql):
+    dialects = ["postgres", "oracle", "mysql", ""]
+    parsed_sql = None
+    for dialect in dialects:
+        try:
+            parsed_sql = parse_one(sql, read=dialect)
+        except Exception as e:
+            continue
+
+        if parsed_sql is not None:
+            break
+    return parsed_sql
+
+
 class LineageXNoConn:
     def __init__(
         self,
         sql: Optional[str] = "",
         dialect: str = "postgres",
         target_schema: Optional[str] = "public",
         search_path_schema: Optional[str] = "public",
     ) -> None:
         self.output_dict = {}
+        self.parsed = 0
         self.target_schema = target_schema
         search_path_schema = [x.strip() for x in search_path_schema.split(",")]
         search_path_schema.append(target_schema)
         self.sql_files_dict = SqlToDict(sql, search_path_schema).sql_files_dict
         self.dialect = dialect
         self.input_table_dict = {}
         self.finished_list = []
         self._find_lineage_no_conn()
 
     def _find_lineage_no_conn(self):
         """
         The driver function to extract the table lineage information
         :return: output an interactive html for the table lineage information
         """
+        not_parsed = 0
+        start_time = time.time()
         for name, sql in self.sql_files_dict.items():
             try:
-                sql_ast = parse_one(sql, read=self.dialect)
+                # sql_ast = parse_one(sql, read=self.dialect)
+                sql_ast = parse_one_sql(sql=sql)
                 all_tables = self._resolve_table(part_ast=sql_ast)
                 for t in all_tables:
                     if t in self.sql_files_dict.keys() and t not in self.finished_list:
                         self._run_lineage_no_conn(name=t, sql=self.sql_files_dict[t])
                         self.finished_list.append(t)
                 if name not in self.finished_list:
                     self._run_lineage_no_conn(name=name, sql=sql)
                     self.finished_list.append(name)
             except Exception as e:
                 print("{} is not processed because it countered {}".format(name, e))
+                not_parsed += 1
                 continue
         self._guess_schema_name()
+        print(
+            "{} SQLs are parsed, {} SQLs are not parsed, took a total of {:.1f} seconds".format(
+                self.parsed, not_parsed, time.time() - start_time
+            )
+        )
         produce_json(self.output_dict)
 
     def _run_lineage_no_conn(self, name: Optional[str] = "", sql: Optional[str] = ""):
         print(name, " processing")
+        self.parsed += 1
         col_lineage = ColumnLineageNoConn(
             sql=sql, dialect=self.dialect, input_table_dict=self.input_table_dict
         )
         # if len(name.split(".")) == 1:
         #     self.output_dict[self.target_schema + "." + name] = {
         #         "tables": col_lineage.table_list,
         #         "columns": col_lineage.column_dict,
```

### Comparing `lineagex-0.0.8/lineagex/LineageXWithConn.py` & `lineagex-0.0.9/lineagex/LineageXWithConn.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     def __init__(
         self,
         sql: Optional[Union[List, str]] = None,
         target_schema: Optional[str] = "public",
         conn_string: Optional[str] = "",
         search_path_schema: Optional[str] = "public",
     ) -> None:
+        self.parsed = 0
+        self.not_parsed = 0
         self.transaction_time = 0
         self.part_tables = None
         self.df = None
         self.schema = target_schema
         self.search_schema = target_schema + "," + search_path_schema
         self.new_view_list = []
         self.s = Stack()
@@ -36,14 +38,15 @@
         self._run_table_lineage()
 
     def _run_table_lineage(self) -> None:
         """
         The driver function to extract the table lineage information
         :return: output an interactive html for the table lineage information
         """
+        start_time = time.time()
         self.part_tables, self.schema_list = self._get_part_tables()
         # If the input is a list with no SELECT , assume it to be a list of views/schema
         if isinstance(self.sql, List) and not any(
             "SELECT " in s.upper() for s in self.sql
         ):
             cur = self.conn.cursor()
             cur.execute("""SET search_path TO {};""".format(self.search_schema))
@@ -97,52 +100,63 @@
                         search_schema=self.search_schema,
                     )
                     self.output_dict[name] = {
                         "tables": col_lineage.table_list,
                         "columns": col_lineage.column_dict,
                         "table_name": name,
                     }
+                    self.parsed += 1
                 except Exception as e:
                     print("{} is not processed because it countered {}".format(name, e))
+                    self.not_parsed += 1
                     continue
         # path or a list of SQL that at least one element contains
         else:
             self.sql_files_dict = SqlToDict(self.sql, self.schema_list).sql_files_dict
             for name, sql in self.sql_files_dict.items():
                 try:
                     if name not in self.finished_list:
                         self._explain_sql(name=name, sql=sql)
                     else:
                         continue
                 except Exception as e:
                     print("{} is not processed because it countered {}".format(name, e))
+                    self.not_parsed += 1
                     continue
         produce_json(
             output_dict=self.output_dict,
             engine=self.conn,
             search_schema=self.search_schema,
         )
         self._delete_view()
         self.conn.close()
-        #print("total transaction time: ", self.transaction_time)
+        print(
+            "{} SQLs are parsed, {} SQLs are not parsed, took a total of {:.1f} seconds, total transaction time is {:.1f}".format(
+                self.parsed,
+                self.not_parsed,
+                time.time() - start_time,
+                self.transaction_time,
+            )
+        )
+        # print("total transaction time: ", self.transaction_time)
 
     def _delete_view(self) -> None:
         """
         Delete all temporary tables in the new_view_list
         :return: None
         """
         # reverse it just in case to drop dependencies first
         self.new_view_list = self.new_view_list[::-1]
         start_time = time.time()
         cur = self.conn.cursor()
         for i in self.new_view_list:
             cur.execute("""DROP TABLE {} CASCADE""".format(i))
             print(i + " dropped")
         cur.close()
-        self.transaction_time += (time.time() - start_time)
+        self.transaction_time += time.time() - start_time
 
     def _create_view(self, name: Optional[str] = "", sql: Optional[str] = "") -> None:
         """
         Create temporary tables with no data from the given sql
         :param name: name of the table
         :param sql: the sql for the table
         :param conn: the psycopg2 connection it was using
@@ -163,15 +177,15 @@
         else:
             cur.execute(
                 """CREATE TABLE {}.{} AS {} WITH NO DATA;""".format(
                     self.schema, name, sql
                 )
             )
         cur.close()
-        self.transaction_time += (time.time() - start_time)
+        self.transaction_time += time.time() - start_time
         print(self.schema + "." + name + " created")
 
     def _get_plan(self, sql: Optional[str] = "") -> dict:
         """
         Get the plan by providing the sql
         :param sql: the sql for getting the plan
         :return: the physical plan of the sql
@@ -180,15 +194,15 @@
         cur = self.conn.cursor()
         cur.execute("""SET search_path TO {};""".format(self.search_schema))
         cur.execute(
             """EXPLAIN (VERBOSE TRUE, FORMAT JSON, COSTS FALSE) {}""".format(sql)
         )
         log_plan = cur.fetchall()
         cur.close()
-        self.transaction_time += (time.time() - start_time)
+        self.transaction_time += time.time() - start_time
         while True:
             if isinstance(log_plan, list) or isinstance(log_plan, tuple):
                 log_plan = log_plan[0]
             elif isinstance(log_plan, dict):
                 log_plan = log_plan["Plan"]
                 break
         return log_plan
@@ -240,22 +254,27 @@
                 plan=self._get_plan(sql=sql),
                 sql=sql,
                 columns=cols,
                 conn=self.conn,
                 part_tables=self.part_tables,
                 search_schema=self.search_schema,
             )
-            if name.isnumeric() or name.find("_DELETION_") != -1 or name.find("_INSERTION_") != -1:
+            if (
+                name.isnumeric()
+                or name.find("_DELETION_") != -1
+                or name.find("_INSERTION_") != -1
+            ):
                 table_name = name
             self.output_dict[table_name] = {
                 "tables": col_lineage.table_list,
                 "columns": col_lineage.column_dict,
                 "table_name": table_name,
             }
             self.finished_list.append(name)
+            self.parsed += 1
             while not self.s.isEmpty():
                 if self.s.peek() in self.sql_files_dict.keys():
                     sql = self.sql_files_dict[self.s.peek()]
                     return self._explain_sql(name=self.s.pop(), sql=sql)
                 else:
                     print("no sql file for the dependencies")
             return
@@ -288,19 +307,22 @@
                     return self._explain_sql(name=table_name, sql=sql)
                 else:
                     print(
                         name
                         + " is skipped because it is missing dependency table "
                         + table_name
                     )
+                    self.not_parsed += 1
                     return
             else:
                 print(e)
+                self.not_parsed += 1
         except Exception as e:
             print(e)
+            self.not_parsed += 1
 
     def _check_db_connection(self, conn_string: Optional[str] = "") -> connection:
         """
         Check if the conn_string is good
         :return: the sqlalchemy engine
         """
         try:
```

### Comparing `lineagex-0.0.8/lineagex/SqlToDict.py` & `lineagex-0.0.9/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/stack.py` & `lineagex-0.0.9/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/utils.py` & `lineagex-0.0.9/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/lineagex/vendor.js` & `lineagex-0.0.9/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/README.md` & `lineagex-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.8/PKG-INFO` & `lineagex-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.8
+Version: 0.0.9
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

