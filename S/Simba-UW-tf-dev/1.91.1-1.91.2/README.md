# Comparing `tmp/Simba-UW-tf-dev-1.91.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.91.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.91.1.tar", last modified: Fri Apr 26 15:19:41 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.91.2.tar", last modified: Sun Apr 28 19:28:53 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.91.1.tar` & `Simba-UW-tf-dev-1.91.2.tar`

### file list

```diff
@@ -1,651 +1,650 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.91.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9544 2024-04-26 00:11:08.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2024-04-26 15:16:18.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.91.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.91.1/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-26 14:51:05.000000 Simba-UW-tf-dev-1.91.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.91.1/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.91.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35776 2024-04-26 13:39:55.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   169619 2024-04-22 13:26:42.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73186 2024-04-25 23:55:15.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    61924 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17995 2024-04-26 15:16:18.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.91.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.1/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7727 2024-04-26 14:59:04.000000 Simba-UW-tf-dev-1.91.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    52940 2024-04-25 19:17:22.000000 Simba-UW-tf-dev-1.91.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79462 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.91.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46271 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.91.1/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    22833 2024-04-26 11:33:33.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11716 2024-04-25 20:20:54.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10604 2024-04-25 23:58:57.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21805 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13623 2024-04-25 20:03:22.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13509 2024-04-26 00:07:47.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24604 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17513 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.91.1/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    13086 2024-04-26 13:42:13.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.91.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.91.1/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.91.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    20088 2024-04-26 11:11:36.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15408 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   119697 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.91.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.91.1/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    23493 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-26 15:19:40.000000 Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.91.1/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.91.1/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.91.1/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.91.1/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.91.1/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.1/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3910 2024-04-25 13:56:16.000000 Simba-UW-tf-dev-1.91.1/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.91.1/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.1/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-26 15:19:37.000000 Simba-UW-tf-dev-1.91.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-26 15:19:41.000000 Simba-UW-tf-dev-1.91.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.91.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.91.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.91.2/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-26 14:51:05.000000 Simba-UW-tf-dev-1.91.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.91.2/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.91.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35776 2024-04-26 13:39:55.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   169619 2024-04-22 13:26:42.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73186 2024-04-25 23:55:15.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    61924 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.91.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.2/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7727 2024-04-26 14:59:04.000000 Simba-UW-tf-dev-1.91.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    52940 2024-04-25 19:17:22.000000 Simba-UW-tf-dev-1.91.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79462 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.91.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.91.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.91.2/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10739 2024-04-27 15:48:36.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    22833 2024-04-28 19:27:01.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11728 2024-04-27 15:46:13.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21805 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13623 2024-04-25 20:03:22.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11661 2024-04-26 19:34:31.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24604 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17513 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16085 2024-04-26 17:26:59.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.91.2/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.91.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.91.2/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.91.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18547 2024-04-28 19:25:10.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15408 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   119697 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.91.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.91.2/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    23451 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-28 19:28:52.000000 Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.91.2/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.91.2/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.91.2/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.91.2/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.91.2/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.2/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.91.2/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.91.2/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.2/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-28 19:28:50.000000 Simba-UW-tf-dev-1.91.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-28 19:28:53.000000 Simba-UW-tf-dev-1.91.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.91.1/PKG-INFO` & `Simba-UW-tf-dev-1.91.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.91.1
+Version: 1.91.2
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 __author__ = "Simon Nilsson"
 
 import os
+import threading
 from tkinter import *
 from typing import Union
-import threading
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.plotting.probability_plot_creator import \
     TresholdPlotCreatorSingleProcess
 from simba.plotting.probability_plot_creator_mp import \
     TresholdPlotCreatorMultiprocess
 from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu,
                                         Entry_Box)
 from simba.utils.checks import check_int
 from simba.utils.enums import Formats, Keys, Links, Paths
-from simba.utils.read_write import (check_if_filepath_list_is_empty, get_file_name_info_in_directory)
 from simba.utils.lookups import get_color_dict
-
-
+from simba.utils.read_write import (check_if_filepath_list_is_empty,
+                                    get_file_name_info_in_directory)
 
 STYLE_WIDTH = 'width'
 STYLE_HEIGHT = 'height'
 STYLE_FONT_SIZE = 'font size'
 STYLE_LINE_WIDTH = 'line width'
 STYLE_YMAX = 'y_max'
 STYLE_COLOR = 'color'
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,84 @@
-__author__ = "Simon Nilsson"
+__author__ = "Tzuk Polinsky"
 
-import threading
+import os
 from tkinter import *
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
-from simba.plotting.clf_validator import ClassifierValidationClips
-from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu,
-                                        Entry_Box)
-from simba.utils.checks import check_int
-from simba.utils.enums import Formats, Keys, Links, Options
+from simba.plotting.directing_animals_to_bodypart_visualizer import \
+    DirectingAnimalsToBodyPartVisualizer
+from simba.plotting.directing_animals_visualizer import \
+    DirectingOtherAnimalsVisualizer
+from simba.plotting.directing_animals_visualizer_mp import \
+    DirectingOtherAnimalsVisualizerMultiprocess
+from simba.ui.tkinter_functions import CreateLabelFrameWithIcon, DropDownMenu
+from simba.utils.enums import Formats, Keys, Links, Paths
+from simba.utils.errors import AnimalNumberError
 from simba.utils.read_write import get_file_name_info_in_directory
 
 
-class ClassifierValidationPopUp(PopUpMixin, ConfigReader):
+class DirectingAnimalToBodyPartVisualizerPopUp(PopUpMixin, ConfigReader):
     def __init__(self, config_path: str):
-        PopUpMixin.__init__(self, title="SIMBA CLASSIFIER VALIDATION CLIPS")
         ConfigReader.__init__(self, config_path=config_path)
-        color_names = list(self.colors_dict.keys())
-        self.one_vid_per_bout_var = BooleanVar(value=False)
-        self.one_vid_per_video_var = BooleanVar(value=True)
+        PopUpMixin.__init__(self, title="CREATE ANIMAL DIRECTION TO BODY PART VIDEOS")
+        self.color_lst = list(self.colors_dict.keys())
+        self.color_lst.insert(0, "Random")
+        self.size_lst = list(range(1, 11))
+        self.data_path = os.path.join(self.project_path, Paths.OUTLIER_CORRECTED.value)
         self.files_found_dict = get_file_name_info_in_directory(
-            directory=self.machine_results_dir, file_type=self.file_type
+            directory=self.data_path, file_type=self.file_type
         )
-        self.settings_frm = CreateLabelFrameWithIcon(
+
+        self.show_pose_var = BooleanVar(value=True)
+        self.merge_directionality_lines_var = BooleanVar(value=False)
+        self.multiprocess_var = BooleanVar(value=False)
+
+        self.style_settings_frm = CreateLabelFrameWithIcon(
             parent=self.main_frm,
-            header="SETTINGS",
+            header="STYLE SETTINGS",
             icon_name=Keys.DOCUMENTATION.value,
-            icon_link=Links.CLF_VALIDATION.value,
-        )
-        self.seconds_entry = Entry_Box(
-            self.settings_frm, "SECONDS PADDING: ", "20", validation="numeric"
-        )
-        self.clf_dropdown = DropDownMenu(
-            self.settings_frm, "CLASSIFIER: ", self.clf_names, "20"
-        )
-        self.clr_dropdown = DropDownMenu(
-            self.settings_frm, "TEXT COLOR: ", color_names, "20"
-        )
-        self.highlight_clr_dropdown = DropDownMenu(
-            self.settings_frm, "HIGHLIGHT TEXT COLOR: ", ["None"] + color_names, "20"
-        )
-        self.video_speed_dropdown = DropDownMenu(
-            self.settings_frm, "VIDEO SPEED: ", Options.SPEED_OPTIONS.value, "20"
-        )
-        self.clf_dropdown.setChoices(self.clf_names[0])
-        self.clr_dropdown.setChoices("Cyan")
-        self.seconds_entry.entry_set(val=2)
-        self.highlight_clr_dropdown.setChoices("None")
-        self.video_speed_dropdown.setChoices(1.0)
-        self.individual_bout_clips_cb = Checkbutton(
-            self.settings_frm,
-            text="CREATE ONE CLIP PER BOUT",
-            variable=self.one_vid_per_bout_var,
-        )
-        self.individual_clip_per_video_cb = Checkbutton(
-            self.settings_frm,
-            text="CREATE ONE CLIP PER VIDEO",
-            variable=self.one_vid_per_video_var,
+            icon_link=Links.DIRECTING_ANIMALS_PLOTS.value,
         )
+        self.show_pose_cb = Checkbutton(
+            self.style_settings_frm,
+            text="Show pose-estimated body-parts",
+            variable=self.show_pose_var,
+        )
+        self.merge_directionality_lines_cb = Checkbutton(
+            self.style_settings_frm,
+            text="Polyfill direction lines",
+            variable=self.merge_directionality_lines_var,
+        )
+        self.direction_clr_dropdown = DropDownMenu(
+            self.style_settings_frm, "Direction color:", self.color_lst, "16"
+        )
+        self.pose_size_dropdown = DropDownMenu(
+            self.style_settings_frm, "Pose circle size:", self.size_lst, "16"
+        )
+        self.line_thickness = DropDownMenu(
+            self.style_settings_frm, "Line thickness:", self.size_lst, "16"
+        )
+        self.line_thickness.setChoices(choice=4)
+        self.pose_size_dropdown.setChoices(choice=3)
+        self.direction_clr_dropdown.setChoices(choice="Random")
+        # multiprocess_cb = Checkbutton(
+        #     self.style_settings_frm,
+        #     text="Multi-process (faster)",
+        #     variable=self.multiprocess_var,
+        #     command=lambda: self.enable_dropdown_from_checkbox(
+        #         check_box_var=self.multiprocess_var,
+        #         dropdown_menus=[self.multiprocess_dropdown],
+        #     ),
+        # )
+        # self.multiprocess_dropdown = DropDownMenu(
+        #     self.style_settings_frm, "CPU cores:", list(range(2, self.cpu_cnt)), "12"
+        # )
+        # self.multiprocess_dropdown.setChoices(2)
+        # self.multiprocess_dropdown.disable()
 
         self.run_frm = LabelFrame(
             self.main_frm,
             text="RUN",
             font=Formats.LABELFRAME_HEADER_FORMAT.value,
             pady=5,
             padx=5,
@@ -76,15 +92,15 @@
             padx=5,
             fg="black",
         )
         self.run_single_video_btn = Button(
             self.run_single_video_frm,
             text="Create single video",
             fg="blue",
-            command=lambda: self.run(multiple_videos=False),
+            command=lambda: self.__create_directionality_plots(multiple_videos=False),
         )
         self.single_video_dropdown = DropDownMenu(
             self.run_single_video_frm,
             "Video:",
             list(self.files_found_dict.keys()),
             "12",
         )
@@ -99,55 +115,59 @@
         )
         self.run_multiple_video_btn = Button(
             self.run_multiple_videos,
             text="Create multiple videos ({} video(s) found)".format(
                 str(len(list(self.files_found_dict.keys())))
             ),
             fg="blue",
-            command=lambda: self.run(multiple_videos=True),
+            command=lambda: self.__create_directionality_plots(multiple_videos=True),
         )
-        self.settings_frm.grid(row=0, sticky=NW)
-        self.seconds_entry.grid(row=0, sticky=NW)
-        self.clf_dropdown.grid(row=1, sticky=NW)
-        self.clr_dropdown.grid(row=2, sticky=NW)
-        self.highlight_clr_dropdown.grid(row=3, sticky=NW)
-        self.video_speed_dropdown.grid(row=4, sticky=NW)
-        self.individual_bout_clips_cb.grid(row=5, column=0, sticky=NW)
-        self.individual_clip_per_video_cb.grid(row=6, column=0, sticky=NW)
+
+        self.style_settings_frm.grid(row=0, column=0, sticky=NW)
+        self.show_pose_cb.grid(row=0, column=0, sticky=NW)
+        self.merge_directionality_lines_cb.grid(row=2, column=0, sticky=NW)
+        self.direction_clr_dropdown.grid(row=3, column=0, sticky=NW)
+        self.pose_size_dropdown.grid(row=4, column=0, sticky=NW)
+        self.line_thickness.grid(row=5, column=0, sticky=NW)
+        # multiprocess_cb.grid(row=6, column=0, sticky=NW)
+        # self.multiprocess_dropdown.grid(row=6, column=1, sticky=NW)
 
         self.run_frm.grid(row=1, column=0, sticky=NW)
         self.run_single_video_frm.grid(row=0, column=0, sticky=NW)
         self.run_single_video_btn.grid(row=0, column=0, sticky=NW)
         self.single_video_dropdown.grid(row=0, column=1, sticky=NW)
         self.run_multiple_videos.grid(row=1, column=0, sticky=NW)
         self.run_multiple_video_btn.grid(row=0, column=0, sticky=NW)
 
-        # self.main_frm.mainloop()
-
-    def run(self, multiple_videos: bool):
-        check_int(name="CLIP SECONDS", value=self.seconds_entry.entry_get)
-        if self.highlight_clr_dropdown.getChoices() == "None":
-            highlight_clr = None
-        else:
-            highlight_clr = self.colors_dict[self.highlight_clr_dropdown.getChoices()]
+    def __create_directionality_plots(self, multiple_videos: bool):
         if multiple_videos:
             data_paths = list(self.files_found_dict.values())
         else:
             data_paths = [
                 self.files_found_dict[self.single_video_dropdown.getChoices()]
             ]
 
-        clf_validator = ClassifierValidationClips(
-            config_path=self.config_path,
-            window=int(self.seconds_entry.entry_get),
-            clf_name=self.clf_dropdown.getChoices(),
-            clips=self.one_vid_per_bout_var.get(),
-            text_clr=self.colors_dict[self.clr_dropdown.getChoices()],
-            highlight_clr=highlight_clr,
-            video_speed=float(self.video_speed_dropdown.getChoices()),
-            concat_video=self.one_vid_per_video_var.get(),
-            data_paths=data_paths,
-        )
-        threading.Thread(target=clf_validator.run()).start()
-
-
-# _ = ClassifierValidationPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
+        style_attr = {
+            "Show_pose": self.show_pose_var.get(),
+            "Pose_circle_size": int(self.pose_size_dropdown.getChoices()),
+            "Direction_color": self.direction_clr_dropdown.getChoices(),
+            "Direction_thickness": int(self.line_thickness.getChoices()),
+            "Polyfill": self.merge_directionality_lines_var.get(),
+        }
+
+        for data_path in data_paths:
+            # if not self.multiprocess_var.get():
+            directing_other_animal_visualizer = DirectingAnimalsToBodyPartVisualizer(
+                config_path=self.config_path,
+                data_path=data_path,
+                style_attr=style_attr,
+            )
+            # else:
+            #     directing_other_animal_visualizer = (
+            #         DirectingOtherAnimalsVisualizerMultiprocess(
+            #             config_path=self.config_path,
+            #             data_path=data_path,
+            #             style_attr=style_attr,
+            #             core_cnt=int(self.multiprocess_dropdown.getChoices()),
+            #         )
+            #     )
+            directing_other_animal_visualizer.run()
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,178 @@
-__author__ = "Tzuk Polinsky"
+__author__ = "Simon Nilsson"
 
-import os
+import threading
 from tkinter import *
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
-from simba.plotting.directing_animals_to_bodypart_visualizer import \
-    DirectingAnimalsToBodyPartVisualizer
-from simba.plotting.directing_animals_visualizer import \
-    DirectingOtherAnimalsVisualizer
-from simba.plotting.directing_animals_visualizer_mp import \
-    DirectingOtherAnimalsVisualizerMultiprocess
-from simba.ui.tkinter_functions import CreateLabelFrameWithIcon, DropDownMenu
-from simba.utils.enums import Formats, Keys, Links, Paths
-from simba.utils.errors import AnimalNumberError
-from simba.utils.read_write import get_file_name_info_in_directory
+from simba.plotting.single_run_model_validation_video import \
+    ValidateModelOneVideo
+from simba.plotting.single_run_model_validation_video_mp import \
+    ValidateModelOneVideoMultiprocess
+from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu,
+                                        Entry_Box)
+from simba.utils.checks import check_float, check_int
+from simba.utils.enums import Formats, Keys, Links, Options
+from simba.utils.read_write import check_file_exist_and_readable, str_2_bool
 
 
-class DirectingAnimalToBodyPartVisualizerPopUp(PopUpMixin, ConfigReader):
-    def __init__(self, config_path: str):
+class ValidationVideoPopUp(PopUpMixin, ConfigReader):
+    def __init__(self, config_path: str, simba_main_frm: object):
+        PopUpMixin.__init__(self, title="CREATE VALIDATION VIDEO")
         ConfigReader.__init__(self, config_path=config_path)
-        PopUpMixin.__init__(self, title="CREATE ANIMAL DIRECTION TO BODY PART VIDEOS")
-        self.color_lst = list(self.colors_dict.keys())
-        self.color_lst.insert(0, "Random")
-        self.size_lst = list(range(1, 11))
-        self.data_path = os.path.join(self.project_path, Paths.OUTLIER_CORRECTED.value)
-        self.files_found_dict = get_file_name_info_in_directory(
-            directory=self.data_path, file_type=self.file_type
-        )
-
-        self.show_pose_var = BooleanVar(value=True)
-        self.merge_directionality_lines_var = BooleanVar(value=False)
-        self.multiprocess_var = BooleanVar(value=False)
+        self.feature_file_path = simba_main_frm.csvfile.file_path
+        self.model_path = simba_main_frm.modelfile.file_path
+        self.discrimination_threshold = simba_main_frm.dis_threshold.entry_get
+        self.shortest_bout = simba_main_frm.min_behaviorbout.entry_get
 
-        self.style_settings_frm = CreateLabelFrameWithIcon(
+        style_frm = CreateLabelFrameWithIcon(
             parent=self.main_frm,
             header="STYLE SETTINGS",
             icon_name=Keys.DOCUMENTATION.value,
-            icon_link=Links.DIRECTING_ANIMALS_PLOTS.value,
+            icon_link=Links.OUT_OF_SAMPLE_VALIDATION.value,
+        )
+        self.default_style_var = BooleanVar(value=True)
+        default_style_cb = Checkbutton(
+            style_frm,
+            text="AUTO-COMPUTE STYLES",
+            variable=self.default_style_var,
+            command=lambda: self.enable_entrybox_from_checkbox(
+                check_box_var=self.default_style_var,
+                entry_boxes=[self.font_size_eb, self.spacing_eb, self.circle_size],
+                reverse=True,
+            ),
+        )
+        self.font_size_eb = Entry_Box(
+            style_frm, "Font size: ", "25", validation="numeric"
+        )
+        self.spacing_eb = Entry_Box(
+            style_frm, "Text spacing: ", "25", validation="numeric"
+        )
+        self.circle_size = Entry_Box(
+            style_frm, "Circle size: ", "25", validation="numeric"
+        )
+        self.font_size_eb.entry_set(val=1)
+        self.spacing_eb.entry_set(val=10)
+        self.circle_size.entry_set(val=5)
+        self.enable_entrybox_from_checkbox(
+            check_box_var=self.default_style_var,
+            entry_boxes=[self.font_size_eb, self.spacing_eb, self.circle_size],
+            reverse=True,
         )
-        self.show_pose_cb = Checkbutton(
-            self.style_settings_frm,
-            text="Show pose-estimated body-parts",
-            variable=self.show_pose_var,
-        )
-        self.merge_directionality_lines_cb = Checkbutton(
-            self.style_settings_frm,
-            text="Polyfill direction lines",
-            variable=self.merge_directionality_lines_var,
-        )
-        self.direction_clr_dropdown = DropDownMenu(
-            self.style_settings_frm, "Direction color:", self.color_lst, "16"
-        )
-        self.pose_size_dropdown = DropDownMenu(
-            self.style_settings_frm, "Pose circle size:", self.size_lst, "16"
-        )
-        self.line_thickness = DropDownMenu(
-            self.style_settings_frm, "Line thickness:", self.size_lst, "16"
-        )
-        self.line_thickness.setChoices(choice=4)
-        self.pose_size_dropdown.setChoices(choice=3)
-        self.direction_clr_dropdown.setChoices(choice="Random")
-        # multiprocess_cb = Checkbutton(
-        #     self.style_settings_frm,
-        #     text="Multi-process (faster)",
-        #     variable=self.multiprocess_var,
-        #     command=lambda: self.enable_dropdown_from_checkbox(
-        #         check_box_var=self.multiprocess_var,
-        #         dropdown_menus=[self.multiprocess_dropdown],
-        #     ),
-        # )
-        # self.multiprocess_dropdown = DropDownMenu(
-        #     self.style_settings_frm, "CPU cores:", list(range(2, self.cpu_cnt)), "12"
-        # )
-        # self.multiprocess_dropdown.setChoices(2)
-        # self.multiprocess_dropdown.disable()
 
-        self.run_frm = LabelFrame(
+        tracking_frm = LabelFrame(
             self.main_frm,
-            text="RUN",
-            font=Formats.LABELFRAME_HEADER_FORMAT.value,
-            pady=5,
-            padx=5,
-            fg="black",
-        )
-        self.run_single_video_frm = LabelFrame(
-            self.run_frm,
-            text="SINGLE VIDEO",
+            text="TRACKING OPTIONS",
             font=Formats.LABELFRAME_HEADER_FORMAT.value,
-            pady=5,
-            padx=5,
-            fg="black",
-        )
-        self.run_single_video_btn = Button(
-            self.run_single_video_frm,
-            text="Create single video",
-            fg="blue",
-            command=lambda: self.__create_directionality_plots(multiple_videos=False),
-        )
-        self.single_video_dropdown = DropDownMenu(
-            self.run_single_video_frm,
-            "Video:",
-            list(self.files_found_dict.keys()),
-            "12",
-        )
-        self.single_video_dropdown.setChoices(list(self.files_found_dict.keys())[0])
-        self.run_multiple_videos = LabelFrame(
-            self.run_frm,
-            text="MULTIPLE VIDEO",
+        )
+        self.show_pose_dropdown = DropDownMenu(
+            tracking_frm, "Show pose:", Options.BOOL_STR_OPTIONS.value, "20"
+        )
+        self.show_animal_names_dropdown = DropDownMenu(
+            tracking_frm, "Show animal names:", Options.BOOL_STR_OPTIONS.value, "20"
+        )
+        self.show_pose_dropdown.setChoices(Options.BOOL_STR_OPTIONS.value[0])
+        self.show_animal_names_dropdown.setChoices(Options.BOOL_STR_OPTIONS.value[1])
+
+        multiprocess_frame = LabelFrame(
+            self.main_frm,
+            text="MULTI-PROCESS SETTINGS",
             font=Formats.LABELFRAME_HEADER_FORMAT.value,
-            pady=5,
-            padx=5,
-            fg="black",
-        )
-        self.run_multiple_video_btn = Button(
-            self.run_multiple_videos,
-            text="Create multiple videos ({} video(s) found)".format(
-                str(len(list(self.files_found_dict.keys())))
+        )
+        self.multiprocess_var = BooleanVar(value=False)
+        self.multiprocess_cb = Checkbutton(
+            multiprocess_frame,
+            text="Multiprocess videos (faster)",
+            variable=self.multiprocess_var,
+            command=lambda: self.enable_dropdown_from_checkbox(
+                check_box_var=self.multiprocess_var,
+                dropdown_menus=[self.multiprocess_dropdown],
             ),
-            fg="blue",
-            command=lambda: self.__create_directionality_plots(multiple_videos=True),
         )
+        self.multiprocess_dropdown = DropDownMenu(
+            multiprocess_frame, "CPU cores:", list(range(2, self.cpu_cnt)), "12"
+        )
+        self.multiprocess_dropdown.setChoices(2)
+        self.multiprocess_dropdown.disable()
 
-        self.style_settings_frm.grid(row=0, column=0, sticky=NW)
-        self.show_pose_cb.grid(row=0, column=0, sticky=NW)
-        self.merge_directionality_lines_cb.grid(row=2, column=0, sticky=NW)
-        self.direction_clr_dropdown.grid(row=3, column=0, sticky=NW)
-        self.pose_size_dropdown.grid(row=4, column=0, sticky=NW)
-        self.line_thickness.grid(row=5, column=0, sticky=NW)
-        # multiprocess_cb.grid(row=6, column=0, sticky=NW)
-        # self.multiprocess_dropdown.grid(row=6, column=1, sticky=NW)
-
-        self.run_frm.grid(row=1, column=0, sticky=NW)
-        self.run_single_video_frm.grid(row=0, column=0, sticky=NW)
-        self.run_single_video_btn.grid(row=0, column=0, sticky=NW)
-        self.single_video_dropdown.grid(row=0, column=1, sticky=NW)
-        self.run_multiple_videos.grid(row=1, column=0, sticky=NW)
-        self.run_multiple_video_btn.grid(row=0, column=0, sticky=NW)
-
-    def __create_directionality_plots(self, multiple_videos: bool):
-        if multiple_videos:
-            data_paths = list(self.files_found_dict.values())
-        else:
-            data_paths = [
-                self.files_found_dict[self.single_video_dropdown.getChoices()]
-            ]
-
-        style_attr = {
-            "Show_pose": self.show_pose_var.get(),
-            "Pose_circle_size": int(self.pose_size_dropdown.getChoices()),
-            "Direction_color": self.direction_clr_dropdown.getChoices(),
-            "Direction_thickness": int(self.line_thickness.getChoices()),
-            "Polyfill": self.merge_directionality_lines_var.get(),
+        gantt_frm = LabelFrame(
+            self.main_frm,
+            text="GANTT SETTINGS",
+            font=Formats.LABELFRAME_HEADER_FORMAT.value,
+        )
+        self.gantt_dropdown = DropDownMenu(
+            gantt_frm, "GANTT TYPE:", Options.GANTT_VALIDATION_OPTIONS.value, "12"
+        )
+        self.gantt_dropdown.setChoices(Options.GANTT_VALIDATION_OPTIONS.value[0])
+
+        style_frm.grid(row=0, column=0, sticky=NW)
+        default_style_cb.grid(row=0, column=0, sticky=NW)
+        self.font_size_eb.grid(row=1, column=0, sticky=NW)
+        self.spacing_eb.grid(row=2, column=0, sticky=NW)
+        self.circle_size.grid(row=3, column=0, sticky=NW)
+
+        tracking_frm.grid(row=1, column=0, sticky=NW)
+        self.show_pose_dropdown.grid(row=0, column=0, sticky=NW)
+        self.show_animal_names_dropdown.grid(row=1, column=0, sticky=NW)
+
+        multiprocess_frame.grid(row=2, column=0, sticky=NW)
+        self.multiprocess_cb.grid(row=0, column=0, sticky=NW)
+        self.multiprocess_dropdown.grid(row=0, column=1, sticky=NW)
+        gantt_frm.grid(row=3, column=0, sticky=NW)
+        self.gantt_dropdown.grid(row=0, column=0, sticky=NW)
+
+        self.create_run_frm(run_function=self.run)
+        self.main_frm.mainloop()
+
+    def run(self):
+        settings = {
+            "pose": str_2_bool(self.show_pose_dropdown.getChoices()),
+            "animal_names": str_2_bool(self.show_animal_names_dropdown.getChoices()),
         }
+        settings["styles"] = None
+        if not self.default_style_var.get():
+            settings["styles"] = {}
+            check_float(name="FONT SIZE", value=self.font_size_eb.entry_get)
+            check_float(name="CIRCLE SIZE", value=self.circle_size.entry_get)
+            check_float(name="SPACE SCALE", value=self.spacing_eb.entry_get)
+            settings["styles"]["circle size"] = int(self.circle_size.entry_get)
+            settings["styles"]["font size"] = int(self.font_size_eb.entry_get)
+            settings["styles"]["space_scale"] = int(self.spacing_eb.entry_get)
+        check_int(name="MINIMUM BOUT LENGTH", value=self.shortest_bout)
+        check_float(
+            name="DISCRIMINATION THRESHOLD", value=self.discrimination_threshold
+        )
+        check_file_exist_and_readable(file_path=self.feature_file_path)
+        check_file_exist_and_readable(file_path=self.model_path)
+
+        create_gantt = self.gantt_dropdown.getChoices()
+        if create_gantt.strip() == "Gantt chart: final frame only (slightly faster)":
+            create_gantt = 1
+        elif create_gantt.strip() == "Gantt chart: video":
+            create_gantt = 2
+        else:
+            create_gantt = None
 
-        for data_path in data_paths:
-            # if not self.multiprocess_var.get():
-            directing_other_animal_visualizer = DirectingAnimalsToBodyPartVisualizer(
+        if not self.multiprocess_var.get():
+            validation_video_creator = ValidateModelOneVideo(
+                config_path=self.config_path,
+                feature_file_path=self.feature_file_path,
+                model_path=self.model_path,
+                discrimination_threshold=float(self.discrimination_threshold),
+                shortest_bout=int(self.shortest_bout),
+                settings=settings,
+                create_gantt=create_gantt,
+            )
+
+        else:
+            validation_video_creator = ValidateModelOneVideoMultiprocess(
                 config_path=self.config_path,
-                data_path=data_path,
-                style_attr=style_attr,
+                feature_file_path=self.feature_file_path,
+                model_path=self.model_path,
+                discrimination_threshold=float(self.discrimination_threshold),
+                shortest_bout=int(self.shortest_bout),
+                cores=int(self.multiprocess_dropdown.getChoices()),
+                settings=settings,
+                create_gantt=create_gantt,
             )
-            # else:
-            #     directing_other_animal_visualizer = (
-            #         DirectingOtherAnimalsVisualizerMultiprocess(
-            #             config_path=self.config_path,
-            #             data_path=data_path,
-            #             style_attr=style_attr,
-            #             core_cnt=int(self.multiprocess_dropdown.getChoices()),
-            #         )
-            #     )
-            directing_other_animal_visualizer.run()
+        threading.Thread(target=validation_video_creator.run()).start()
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 __author__ = "Simon Nilsson"
 
 import os
+import threading
 from tkinter import *
 from typing import Union
-import threading
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
-from simba.third_party_label_appenders.third_party_appender import ThirdPartyLabelAppender
-from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu, FolderSelect)
+from simba.third_party_label_appenders.third_party_appender import \
+    ThirdPartyLabelAppender
+from simba.ui.tkinter_functions import (CreateLabelFrameWithIcon, DropDownMenu,
+                                        FolderSelect)
 from simba.utils.checks import check_if_dir_exists
 from simba.utils.enums import Formats, Keys, Links, Options
 from simba.utils.lookups import get_third_party_appender_file_formats
 
 
 class ThirdPartyAnnotatorAppenderPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.91.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.91.2/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.91.2/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.91.2/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.91.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.91.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.91.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.91.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.91.2/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.91.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.91.2/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 __author__ = "Simon Nilsson"
 
 import os
 from copy import deepcopy
-from typing import Union, Dict, Optional
+from typing import Dict, Optional, Union
+
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 import pandas as pd
+
 from simba.mixins.config_reader import ConfigReader
-from simba.third_party_label_appenders.tools import (check_stop_events_prior_to_start_events,
-                                                     fix_uneven_start_stop_count,
-                                                     read_bento_files,
-                                                     read_boris_annotation_files,
-                                                     read_deepethogram_files,
-                                                     read_ethovision_files,
-                                                     read_observer_files,
-                                                     read_solomon_files)
-from simba.utils.checks import (check_if_dir_exists,check_if_filepath_list_is_empty, check_str, check_instance)
+from simba.third_party_label_appenders.tools import (
+    check_stop_events_prior_to_start_events, fix_uneven_start_stop_count,
+    read_bento_files, read_boris_annotation_files, read_deepethogram_files,
+    read_ethovision_files, read_observer_files, read_solomon_files)
+from simba.utils.checks import (check_if_dir_exists,
+                                check_if_filepath_list_is_empty,
+                                check_instance, check_str)
 from simba.utils.enums import Methods
-from simba.utils.errors import (ThirdPartyAnnotationEventCountError,
-                                ThirdPartyAnnotationFileNotFoundError,
-                                ThirdPartyAnnotationOverlapError,
-                                ThirdPartyAnnotationsAdditionalClfError,
-                                ThirdPartyAnnotationsMissingAnnotationsError,
-                                ThirdPartyAnnotationsOutsidePoseEstimationDataError)
+from simba.utils.errors import (
+    ThirdPartyAnnotationEventCountError, ThirdPartyAnnotationFileNotFoundError,
+    ThirdPartyAnnotationOverlapError, ThirdPartyAnnotationsAdditionalClfError,
+    ThirdPartyAnnotationsMissingAnnotationsError,
+    ThirdPartyAnnotationsOutsidePoseEstimationDataError)
 from simba.utils.printing import stdout_success
-from simba.utils.read_write import (get_fn_ext,
-                                    read_df,
-                                    write_df,
-                                    find_files_of_filetypes_in_directory)
-from simba.utils.warnings import (ThirdPartyAnnotationEventCountWarning,
-                                  ThirdPartyAnnotationFileNotFoundWarning,
-                                  ThirdPartyAnnotationOverlapWarning,
-                                  ThirdPartyAnnotationsAdditionalClfWarning,
-                                  ThirdPartyAnnotationsMissingAnnotationsWarning,
-                                  ThirdPartyAnnotationsOutsidePoseEstimationDataWarning)
+from simba.utils.read_write import (find_files_of_filetypes_in_directory,
+                                    get_fn_ext, read_df, write_df)
+from simba.utils.warnings import (
+    ThirdPartyAnnotationEventCountWarning,
+    ThirdPartyAnnotationFileNotFoundWarning,
+    ThirdPartyAnnotationOverlapWarning,
+    ThirdPartyAnnotationsAdditionalClfWarning,
+    ThirdPartyAnnotationsMissingAnnotationsWarning,
+    ThirdPartyAnnotationsOutsidePoseEstimationDataWarning)
 
 BORIS = "BORIS"
 DEEPETHOGRAM = "DEEPETHOGRAM"
 ETHOVISION = "ETHOVISION"
 OBSERVER = "OBSERVER"
 SOLOMON = "SOLOMON"
 BENTO = "BENTO"
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.91.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,15 +993,15 @@
             results.append(sample)
         else:
             results.append(sample.sample(n=n, replace=False))
     return pd.concat(results, axis=0)
 
 
 def get_mode(x: np.ndarray) -> Union[float, int]:
-    """Get the mode (most frequent value) within an aarray"""
+    """Get the mode (most frequent value) within an array"""
     check_valid_array(
         source=f"{get_mode.__name__} x",
         data=x,
         accepted_dtypes=(np.float32, np.float64, np.int32, np.int64, np.int8),
     )
     values, counts = np.unique(x, return_counts=True)
     return counts.argmax()
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.91.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.91.2/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.91.2/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/gantt_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,23 @@
         self.timer.stop_timer()
         stdout_success(
             msg="All gantt visualizations created in project_folder/frames/output/gantt_plots directory",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
+# test = GanttCreatorSingleProcess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/RAT_NOR/project_folder/project_config.ini',
+#                                 frame_setting=False,
+#                                 video_setting=False,
+#                                 files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/RAT_NOR/project_folder/csv/machine_results/2022-06-20_NOB_DOT_4.csv'],
+#                                 last_frm_setting=True,
+#                                 style_attr={'width': 640, 'height': 480, 'font size': 10, 'font rotation': 65})
+# test.run()
+
+
 # style_attr = {'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45}
 # test = GanttCreatorSingleProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
 #                                  frame_setting=False,
 #                                  video_setting=True,
 #                                  last_frm_setting=True,
 #                                  style_attr=style_attr,
 #                                  files_found=['/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location/Testing_Video_3.csv'])
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/gantt_creator_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                     self.gantt_plot_dir, f"{self.video_name}.mp4"
                 )
 
             if self.last_frm_setting:
                 self.make_gantt_plot(
                     data_df=self.data_df,
                     bouts_df=self.bouts_df,
-                    clf_names=self.clf_names,
+                    clf_names=self.clf_names[::-1],
                     fps=self.fps,
                     style_attr=self.style_attr,
                     video_name=self.video_name,
                     save_path=os.path.join(
                         self.gantt_plot_dir, f"{self.video_name}_final_image.png"
                     ),
                 )
@@ -195,15 +195,15 @@
                     constants = functools.partial(
                         self.gantt_creator_mp,
                         video_setting=self.video_setting,
                         frame_setting=self.frame_setting,
                         video_save_dir=self.temp_folder,
                         frame_folder_dir=self.save_frame_folder_dir,
                         bouts_df=self.bouts_df,
-                        clf_names=self.clf_names,
+                        clf_names=self.clf_names[::-1],
                         fps=self.fps,
                         rotation=self.y_rotation,
                         colors=self.colours,
                         color_tuple=self.colour_tuple_x,
                         font_size=self.y_fontsize,
                         width=self.out_width,
                         height=self.out_height,
@@ -242,20 +242,20 @@
         self.timer.stop_timer()
         stdout_success(
             msg=f"Gantt visualizations for {len(self.files_found)} videos created in project_folder/frames/output/gantt_plots directory",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
 
-# test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/project_config.ini',
-#                                 frame_setting=True,
-#                                 video_setting=False,
-#                                 files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/beepboop174/project_folder/csv/machine_results/Trial    10.csv'],
+# test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/RAT_NOR/project_folder/project_config.ini',
+#                                 frame_setting=False,
+#                                 video_setting=True,
+#                                 files_found=['/Users/simon/Desktop/envs/simba/troubleshooting/RAT_NOR/project_folder/csv/machine_results/2022-06-20_NOB_DOT_4.csv'],
 #                                 cores=5,
-#                                 last_frm_setting=False,
+#                                 last_frm_setting=True,
 #                                 style_attr={'width': 640, 'height': 480, 'font size': 10, 'font rotation': 65})
 # test.run()
 
 
 # style_attr = {'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45}
 # test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                                  frame_setting=False,
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/probability_plot_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 __author__ = "Simon Nilsson"
 
 import os
-from typing import Dict, List, Union, Optional, Any
+from typing import Any, Dict, List, Optional, Union
+
 import cv2
 import numpy as np
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
-from simba.utils.checks import (check_that_column_exist, check_file_exist_and_readable, check_valid_lst, check_if_keys_exist_in_dict, check_str, check_all_file_names_are_represented_in_video_log)
+from simba.utils.checks import (
+    check_all_file_names_are_represented_in_video_log,
+    check_file_exist_and_readable, check_if_keys_exist_in_dict, check_str,
+    check_that_column_exist, check_valid_lst)
 from simba.utils.enums import Formats
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 
-
 STYLE_WIDTH = 'width'
 STYLE_HEIGHT = 'height'
 STYLE_FONT_SIZE = 'font size'
 STYLE_LINE_WIDTH = 'line width'
 STYLE_YMAX = 'y_max'
 STYLE_COLOR = 'color'
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 __author__ = "Simon Nilsson"
 
 import functools
 import multiprocessing
 import os
 import platform
 import shutil
-from typing import Any, Dict, List, Optional, Union, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.checks import (
-    check_all_file_names_are_represented_in_video_log, check_int, check_str,
-    check_that_column_exist, check_valid_lst, check_if_keys_exist_in_dict)
+    check_all_file_names_are_represented_in_video_log,
+    check_if_keys_exist_in_dict, check_int, check_str, check_that_column_exist,
+    check_valid_lst)
 from simba.utils.enums import Formats
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import SimbaTimer, stdout_success
 from simba.utils.read_write import (concatenate_videos_in_folder,
                                     find_core_cnt, get_fn_ext, read_df)
 
-
 STYLE_WIDTH = 'width'
 STYLE_HEIGHT = 'height'
 STYLE_FONT_SIZE = 'font size'
 STYLE_LINE_WIDTH = 'line width'
 STYLE_YMAX = 'y_max'
 STYLE_COLOR = 'color'
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/clf_validator_mp.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 from typing import List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
-from simba.utils.checks import (
-    check_all_file_names_are_represented_in_video_log, check_int,
-    check_that_column_exist)
+from simba.utils.checks import (check_int,
+                                check_that_column_exist,
+                                check_valid_lst,
+                                check_float,
+                                check_str,
+                                check_if_valid_rgb_tuple)
 from simba.utils.data import detect_bouts
 from simba.utils.enums import Formats, TagNames, TextOptions
 from simba.utils.errors import NoFilesFoundError, NoSpecifiedOutputError
 from simba.utils.printing import SimbaTimer, log_event, stdout_success
 from simba.utils.read_write import (concatenate_videos_in_folder,
                                     find_core_cnt, get_fn_ext,
                                     get_video_meta_data, read_df, remove_files)
@@ -24,27 +27,25 @@
 
 SPACE_SCALE = 60
 RADIUS_SCALE = 12
 RESOLUTION_SCALE = 1500
 FONT_SCALE = 1.5
 
 
-def val_clip_createror_mp(
-    data: np.ndarray,
-    video_path: str,
-    scalers: dict,
-    bout_total_cnt: int,
-    fps: float,
-    video_meta_data: dict,
-    clf_name: str,
-    p_data: pd.Series,
-    clf_data: pd.Series,
-    highlight_clr: tuple,
-    text_clr: tuple,
-):
+def val_clip_createror_mp(data: np.ndarray,
+                          video_path: str,
+                          scalers: dict,
+                          bout_total_cnt: int,
+                          fps: float,
+                          video_meta_data: dict,
+                          clf_name: str,
+                          p_data: pd.Series,
+                          clf_data: pd.Series,
+                          highlight_clr: tuple,
+                          text_clr: tuple):
     def __insert_inter_frms(
         bg_color: Tuple[int, int, int] = (49, 32, 189),
         fg_color: Tuple[int, int, int] = (0, 0, 0),
     ):
         """
         Helper to create N blank frames separating the classified event bouts with defined BGR colors.
         """
@@ -205,201 +206,131 @@
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md#classifier-validation>`_.
 
     Examples
     ----------
     >>> _ = ClassifierValidationClipsMultiprocess(config_path='MyProjectConfigPath', window=5, clf_name='Attack', text_clr=(255,255,0), clips=False, concat_video=True).run()
     """
 
-    def __init__(
-        self,
-        config_path: str,
-        window: int,
-        clf_name: str,
-        clips: bool,
-        data_paths: List[Union[str, os.PathLike]],
-        text_clr: Tuple[int, int, int],
-        concat_video: bool = False,
-        video_speed: float = 1.0,
-        highlight_clr: Optional[Tuple[int, int, int]] = None,
-        core_cnt: Optional[int] = -1,
-    ):
-        super().__init__(config_path=config_path)
-        log_event(
-            logger_name=str(__class__.__name__),
-            log_type=TagNames.CLASS_INIT.value,
-            msg=self.create_log_msg_from_init_args(locals=locals()),
-        )
+    def __init__(self,
+                 config_path: str,
+                 window: int,
+                 clf_name: str,
+                 clips: bool,
+                 data_paths: List[Union[str, os.PathLike]],
+                 text_clr: Tuple[int, int, int],
+                 concat_video: bool = False,
+                 video_speed: float = 1.0,
+                 highlight_clr: Optional[Tuple[int, int, int]] = None,
+                 core_cnt: Optional[int] = -1):
+
+
+        ConfigReader.__init__(self, config_path=config_path)
+
         if (not clips) and (not concat_video):
-            raise NoSpecifiedOutputError(
-                msg="Please select to create clips and/or a concatenated video",
-                source=self.__class__.__name__,
-            )
+            raise NoSpecifiedOutputError(msg="Please select to create clips and/or a concatenated video", source=self.__class__.__name__)
 
         check_int(name="Time window", value=window, min_value=0)
-        check_int(
-            name="CORE COUNT",
-            value=core_cnt,
-            min_value=-1,
-            max_value=find_core_cnt()[0],
-            raise_error=True,
-        )
-        if core_cnt == -1:
-            core_cnt = find_core_cnt()[0]
+        check_if_valid_rgb_tuple(data=text_clr)
+        if highlight_clr is not None: check_if_valid_rgb_tuple(data=highlight_clr)
+        check_valid_lst(data=data_paths, source=f'{self.__class__.__name__} data_paths', min_len=1)
+        check_str(name=f'{self.__class__.__name__} clf_name', value=clf_name, options=self.clf_names)
+        check_float(name=f'{self.__class__.__name__} video_speed', value=video_speed, min_value=10e-6)
+        check_int(name="CORE COUNT",value=core_cnt,min_value=-1,max_value=find_core_cnt()[0],raise_error=True,)
+        if core_cnt == -1:core_cnt = find_core_cnt()[0]
         self.core_cnt = core_cnt
         self.window, self.clf_name = int(window), clf_name
-        self.clips, self.concat_video, self.video_speed, self.highlight_clr = (
-            clips,
-            concat_video,
-            video_speed,
-            highlight_clr,
-        )
+        self.clips, self.concat_video, self.video_speed, self.highlight_clr = clips, concat_video, video_speed, highlight_clr
         self.p_col = f"Probability_{self.clf_name}"
         self.text_clr, self.data_paths = text_clr, data_paths
         self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
         self.font = TextOptions.FONT.value
         if not os.path.exists(self.clf_validation_dir):
             os.makedirs(self.clf_validation_dir)
-        if len(self.data_paths) == 0:
-            raise NoFilesFoundError(
-                msg="No data found in the project_folder/csv/machine_results directory",
-                source=self.__class__.__name__,
-            )
-        print(f"Processing {str(len(self.data_paths))} files...")
+        print(f"Processing {len(self.data_paths)} files...")
 
     def run(self):
-        """
-        Method to generate clips. Results are saved in the ``project_folder/frames/output/classifier_validation directory``
-        directory of the SimBA project.
-        """
-
-        check_all_file_names_are_represented_in_video_log(
-            video_info_df=self.video_info_df, data_paths=self.data_paths
-        )
-
         for file_cnt, file_path in enumerate(self.data_paths):
             video_timer = SimbaTimer(start=True)
             self.data_df = read_df(file_path, self.file_type)
-            check_that_column_exist(
-                df=self.data_df, column_name=self.p_col, file_name=file_path
-            )
+            check_that_column_exist(df=self.data_df, column_name=self.p_col, file_name=file_path)
             _, file_name, _ = get_fn_ext(file_path)
-            self.video_path = self.find_video_of_file(
-                video_dir=self.video_dir, filename=file_name, raise_error=True
-            )
+            self.video_path = self.find_video_of_file(video_dir=self.video_dir, filename=file_name, raise_error=True)
             self.video_info = get_video_meta_data(video_path=self.video_path)
             self.fps = int(self.video_info["fps"])
             self.video_fps = int(self.fps * self.video_speed)
-            if self.video_fps < 1:
-                self.video_fps = 1
+            if self.video_fps < 1: self.video_fps = 1
             self.max_dim = max(self.video_info["width"], self.video_info["height"])
             self.circle_scale = int(RADIUS_SCALE / (RESOLUTION_SCALE / self.max_dim))
             self.font_size = float(FONT_SCALE / (RESOLUTION_SCALE / self.max_dim))
             self.spacing_scale = int(SPACE_SCALE / (RESOLUTION_SCALE / self.max_dim))
-            clf_bouts = detect_bouts(
-                data_df=self.data_df, target_lst=[self.clf_name], fps=self.fps
-            ).reset_index(drop=True)
+            clf_bouts = detect_bouts(data_df=self.data_df, target_lst=[self.clf_name], fps=self.fps).reset_index(drop=True)
             if len(clf_bouts) == 0:
-                NoDataFoundWarning(
-                    msg=f"Skipping video {file_name}: No classified behavior detected...",
-                    source=self.__class__.__name__,
-                )
+                NoDataFoundWarning(msg=f"Skipping video {file_name}: No classified behavior {self.clf_name} detected...", source=self.__class__.__name__)
                 continue
 
             clip_data = []
             for i, (bout_cnt, bout) in enumerate(clf_bouts.iterrows()):
                 self.bout_cnt = bout_cnt
                 event_start_frm, event_end_frm = bout["Start_frame"], bout["End_frame"]
-                start_window = int(
-                    event_start_frm - (int(self.video_info["fps"]) * self.window)
-                )
-                end_window = int(
-                    event_end_frm + (int(self.video_info["fps"]) * self.window)
-                )
+                start_window = int(event_start_frm - (int(self.video_info["fps"]) * self.window))
+                end_window = int(event_end_frm + (int(self.video_info["fps"]) * self.window))
                 if end_window > len(self.data_df):
                     end_window = len(self.data_df)
                 if start_window < 0:
                     start_window = 0
-                self.save_path = os.path.join(
-                    self.clf_validation_dir,
-                    self.clf_name + f"_{bout_cnt}_{file_name}.mp4",
-                )
+                self.save_path = os.path.join(self.clf_validation_dir, self.clf_name + f"_{bout_cnt}_{file_name}.mp4")
                 clip_data.append([bout_cnt, start_window, end_window, self.save_path])
             clip_data = np.array(clip_data)
-            print(
-                f"Creating validation video, multiprocessing (chunksize: {self.multiprocess_chunksize}, cores: {self.core_cnt})..."
-            )
-            with multiprocessing.Pool(
-                self.core_cnt, maxtasksperchild=self.maxtasksperchild
-            ) as pool:
-                constants = functools.partial(
-                    val_clip_createror_mp,
-                    video_path=self.video_path,
-                    scalers={
-                        "circle": self.circle_scale,
-                        "font": self.font_size,
-                        "space": self.spacing_scale,
-                    },
-                    fps=self.video_fps,
-                    clf_name=self.clf_name,
-                    bout_total_cnt=len(clf_bouts),
-                    video_meta_data=self.video_info,
-                    p_data=self.data_df[self.p_col].astype(np.float32),
-                    clf_data=self.data_df[self.clf_name].astype(np.float32),
-                    highlight_clr=self.highlight_clr,
-                    text_clr=self.text_clr,
-                )
+            print(f"Creating validation video, multiprocessing (chunksize: {self.multiprocess_chunksize}, cores: {self.core_cnt})...")
+            with multiprocessing.Pool(self.core_cnt, maxtasksperchild=self.maxtasksperchild) as pool:
+                constants = functools.partial(val_clip_createror_mp,
+                                              video_path=self.video_path,
+                                              scalers={"circle": self.circle_scale,"font": self.font_size,"space": self.spacing_scale},
+                                              fps=self.video_fps,
+                                              clf_name=self.clf_name,
+                                              bout_total_cnt=len(clf_bouts),
+                                              video_meta_data=self.video_info,
+                                              p_data=self.data_df[self.p_col].astype(np.float32),
+                                              clf_data=self.data_df[self.clf_name].astype(np.float32),
+                                              highlight_clr=self.highlight_clr,
+                                              text_clr=self.text_clr)
 
                 for cnt, result in enumerate(
-                    pool.imap(
-                        constants, clip_data, chunksize=self.multiprocess_chunksize
-                    )
-                ):
+                    pool.imap(constants, clip_data, chunksize=self.multiprocess_chunksize)):
                     print(f"Bout {cnt+1} complete...")
                 pool.terminate()
                 pool.join()
 
             if self.concat_video:
                 print(f"Joining {file_name} multiprocessed video...")
-                concat_video_save_path = os.path.join(
-                    self.clf_validation_dir,
-                    f"{self.clf_name}_{file_name}_all_events.mp4",
-                )
+                concat_video_save_path = os.path.join(self.clf_validation_dir, f"{self.clf_name}_{file_name}_all_events.mp4")
                 file_paths = list(clip_data[:, 3])
-                concatenate_videos_in_folder(
-                    in_folder=self.clf_validation_dir,
-                    save_path=concat_video_save_path,
-                    substring=None,
-                    file_paths=file_paths,
-                    remove_splits=False,
-                )
+                concatenate_videos_in_folder(in_folder=self.clf_validation_dir,
+                                             save_path=concat_video_save_path,
+                                             substring=None,
+                                             file_paths=file_paths,
+                                             remove_splits=False)
             if not self.clips:
                 remove_files(file_paths=list(clip_data[:, 3]))
             video_timer.stop_timer()
-            stdout_success(
-                msg=f"Validation clips for video {file_name} complete!",
-                elapsed_time=video_timer.elapsed_time_str,
-            )
+            stdout_success(msg=f"Validation clips for video {file_name} complete!", elapsed_time=video_timer.elapsed_time_str)
 
         self.timer.stop_timer()
-        stdout_success(
-            msg=f"All video clips complete and saved in {self.clf_validation_dir}!",
-            elapsed_time=self.timer.elapsed_time_str,
-        )
+        stdout_success(msg=f"All video clips complete and saved in {self.clf_validation_dir}!", elapsed_time=self.timer.elapsed_time_str)
 
 
-# test = ClassifierValidationClipsMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+# test = ClassifierValidationClipsMultiprocess(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                              window=1,
 #                                              clf_name='Attack',
 #                                              clips=True,
 #                                              concat_video=True,
 #                                              highlight_clr=(255, 0, 0),
 #                                              video_speed=0.5,
 #                                              text_clr=(0, 0, 255),
-#                                              data_paths=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv',
-#                                                          '/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_2.csv'])
+#                                              data_paths=['/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'])
 # test.run()
 
 # test = ClassifierValidationClips(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
 #                                  window=1,
 #                                  clf_name='Attack',
 #                                  clips=False,
 #                                  concat_video=True,
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.91.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.91.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.91.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.91.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 import multiprocessing
 import platform
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_supplement_mixin import \
     FeatureExtractionSupplemental
 from simba.mixins.geometry_mixin import GeometryMixin
-from simba.utils.checks import (check_float, check_int, check_str,
-                                check_valid_lst, check_video_has_rois, check_all_file_names_are_represented_in_video_log)
+from simba.utils.checks import (
+    check_all_file_names_are_represented_in_video_log, check_float, check_int,
+    check_str, check_valid_lst, check_video_has_rois)
 from simba.utils.errors import (AnimalNumberError, InvalidInputError,
                                 NoFilesFoundError, ROICoordinatesNotFoundError)
 from simba.utils.printing import stdout_success
-from simba.utils.read_write import (get_fn_ext, read_df, read_data_paths)
-
+from simba.utils.read_write import get_fn_ext, read_data_paths, read_df
 from simba.utils.warnings import NoFileFoundWarning
 
 TAIL_END = "tail_end"
 
 
 class SpontaneousAlternationCalculator(ConfigReader):
     """
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.91.2/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.91.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.91.2/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.91.2/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.91.2/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.91.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.91.2/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.91.2/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,47 +40,36 @@
 
     :example:
     >>> test = ROIAnalyzer(config_path = r"/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini", calculate_distances=True, detailed_bout_data=True, body_parts=['Nose_1', 'Nose_2'], threshold=0.0)
     >>> test.run()
     >>> test.save()
     """
 
-    def __init__(
-        self,
-        config_path: Union[str, os.PathLike],
-        data_path: Optional[Union[str, os.PathLike, List[str]]] = None,
-        detailed_bout_data: Optional[bool] = False,
-        calculate_distances: Optional[bool] = False,
-        threshold: Optional[float] = 0.0,
-        body_parts: Optional[List[str]] = None,
-    ):
+    def __init__(self,
+                 config_path: Union[str, os.PathLike],
+                 data_path: Optional[Union[str, os.PathLike, List[str]]] = None,
+                 detailed_bout_data: Optional[bool] = False,
+                 calculate_distances: Optional[bool] = False,
+                 threshold: Optional[float] = 0.0,
+                 body_parts: Optional[List[str]] = None):
 
         check_file_exist_and_readable(file_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         if not os.path.isfile(self.roi_coordinates_path):
-            raise ROICoordinatesNotFoundError(
-                expected_file_path=self.roi_coordinates_path
-            )
+            raise ROICoordinatesNotFoundError(expected_file_path=self.roi_coordinates_path)
         self.read_roi_data()
         FeatureExtractionMixin.__init__(self)
         if detailed_bout_data and (not os.path.exists(self.detailed_roi_data_dir)):
             os.makedirs(self.detailed_roi_data_dir)
-        self.data_paths = read_data_paths(
-            path=data_path,
-            default=self.outlier_corrected_paths,
-            default_name=self.outlier_corrected_dir,
-            file_type=self.file_type,
-        )
+        self.data_paths = read_data_paths(path=data_path,
+                                          default=self.outlier_corrected_paths,
+                                          default_name=self.outlier_corrected_dir,
+                                          file_type=self.file_type)
 
-        check_float(
-            name="Body-part probability threshold",
-            value=threshold,
-            min_value=0.0,
-            max_value=1.0,
-        )
+        check_float(name="Body-part probability threshold", value=threshold, min_value=0.0, max_value=1.0)
         check_valid_lst(
             data=body_parts,
             source=f"{self.__class__.__name__} body-parts",
             valid_dtypes=(str,),
         )
         if len(set(body_parts)) != len(body_parts):
             raise CountError(
@@ -96,114 +85,64 @@
             self.bp_lk[animal] = bp
         self.roi_headers = [v for k, v in self.bp_dict.items()]
         self.roi_headers = [item for sublist in self.roi_headers for item in sublist]
         self.calculate_distances, self.threshold = calculate_distances, threshold
         self.detailed_bout_data = detailed_bout_data
 
     def run(self):
-        check_all_file_names_are_represented_in_video_log(
-            video_info_df=self.video_info_df, data_paths=self.data_paths
-        )
-        self.movements_df = pd.DataFrame(
-            columns=["VIDEO", "ANIMAL", "SHAPE", "MEASUREMENT", "VALUE"]
-        )
-        self.entry_results = pd.DataFrame(
-            columns=["VIDEO", "ANIMAL", "SHAPE", "ENTRY COUNT"]
-        )
-        self.time_results = pd.DataFrame(
-            columns=["VIDEO", "ANIMAL", "SHAPE", "TIME (S)"]
-        )
+        check_all_file_names_are_represented_in_video_log(video_info_df=self.video_info_df, data_paths=self.data_paths)
+        self.movements_df = pd.DataFrame(columns=["VIDEO", "ANIMAL", "SHAPE", "MEASUREMENT", "VALUE"])
+        self.entry_results = pd.DataFrame(columns=["VIDEO", "ANIMAL", "SHAPE", "ENTRY COUNT"])
+        self.time_results = pd.DataFrame(columns=["VIDEO", "ANIMAL", "SHAPE", "TIME (S)"])
         self.roi_bout_results = []
+        self.detailed_df = None
         for file_cnt, file_path in enumerate(self.data_paths):
             _, video_name, _ = get_fn_ext(file_path)
             print(f"Analysing ROI data for video {video_name}...")
-            video_settings, pix_per_mm, self.fps = self.read_video_info(
-                video_name=video_name
-            )
-            self.roi_dict, video_shape_names = slice_roi_dict_for_video(
-                data=self.roi_dict, video_name=video_name
-            )
+            video_settings, pix_per_mm, self.fps = self.read_video_info(video_name=video_name)
+            self.sliced_roi_dict, video_shape_names = slice_roi_dict_for_video(data=self.roi_dict, video_name=video_name)
             if video_shape_names == 0:
-                NoDataFoundWarning(
-                    msg=f"Skipping video {video_name}: No user-defined ROI data found for this video..."
-                )
+                NoDataFoundWarning(msg=f"Skipping video {video_name}: No user-defined ROI data found for this video...")
                 continue
             else:
                 self.data_df = read_df(file_path, self.file_type).reset_index(drop=True)
                 if len(self.bp_headers) != len(self.data_df.columns):
-                    raise MissingColumnsError(
-                        msg=f"The data file {file_path} contains {len(self.data_df.columns)} body-part columns, but the project is made for {len(self.bp_headers)} body-part columns as suggested by the {self.body_parts_path} file",
-                        source=self.__class__.__name__,
-                    )
+                    raise MissingColumnsError(msg=f"The data file {file_path} contains {len(self.data_df.columns)} body-part columns, but the project is made for {len(self.bp_headers)} body-part columns as suggested by the {self.body_parts_path} file", source=self.__class__.__name__)
                 self.data_df.columns = self.bp_headers
-                check_that_column_exist(
-                    df=self.data_df, column_name=self.roi_headers, file_name=file_path
-                )
+                check_that_column_exist(df=self.data_df, column_name=self.roi_headers, file_name=file_path)
                 for animal_name, bp_names in self.bp_dict.items():
-                    animal_df = self.data_df[self.bp_dict[animal_name]].reset_index(
-                        drop=True
-                    )
+                    animal_df = self.data_df[self.bp_dict[animal_name]].reset_index(drop=True)
                     animal_bout_results = {}
-                    for _, row in self.roi_dict[Keys.ROI_RECTANGLES.value].iterrows():
-                        roi_coords = np.array(
-                            [
-                                [row["topLeftX"], row["topLeftY"]],
-                                [row["Bottom_right_X"], row["Bottom_right_Y"]],
-                            ]
-                        )
-                        animal_df[row["Name"]] = (
-                            FeatureExtractionMixin.framewise_inside_rectangle_roi(
-                                bp_location=animal_df.values[:, 0:2],
-                                roi_coords=roi_coords,
-                            )
-                        )
-                        animal_df.loc[
-                            animal_df[bp_names[2]] < self.threshold, row["Name"]
-                        ] = 0
-                        roi_bouts = detect_bouts(
-                            data_df=animal_df, target_lst=[row["Name"]], fps=self.fps
-                        )
+                    for _, row in self.sliced_roi_dict[Keys.ROI_RECTANGLES.value].iterrows():
+                        roi_coords = np.array([[row["topLeftX"], row["topLeftY"]], [row["Bottom_right_X"], row["Bottom_right_Y"]]])
+                        animal_df[row["Name"]] = (FeatureExtractionMixin.framewise_inside_rectangle_roi(bp_location=animal_df.values[:, 0:2], roi_coords=roi_coords))
+                        animal_df.loc[animal_df[bp_names[2]] < self.threshold, row["Name"]] = 0
+                        roi_bouts = detect_bouts(data_df=animal_df, target_lst=[row["Name"]], fps=self.fps)
                         roi_bouts["ANIMAL"] = animal_name
                         roi_bouts["VIDEO"] = video_name
                         self.roi_bout_results.append(roi_bouts)
                         animal_bout_results[row["Name"]] = roi_bouts
-                        self.entry_results.loc[len(self.entry_results)] = [
-                            video_name,
-                            animal_name,
-                            row["Name"],
-                            len(roi_bouts),
-                        ]
-                        self.time_results.loc[len(self.time_results)] = [
-                            video_name,
-                            animal_name,
-                            row["Name"],
-                            roi_bouts["Bout_time"].sum(),
-                        ]
-                    for _, row in self.roi_dict[Keys.ROI_CIRCLES.value].iterrows():
+                        self.entry_results.loc[len(self.entry_results)] = [video_name,animal_name,row["Name"],len(roi_bouts)]
+                        self.time_results.loc[len(self.time_results)] = [video_name,animal_name,row["Name"],roi_bouts["Bout_time"].sum()]
+                    for _, row in self.sliced_roi_dict[Keys.ROI_CIRCLES.value].iterrows():
+
                         center_x, center_y = row["centerX"], row["centerY"]
                         animal_df[f'{row["Name"]}_distance'] = (FeatureExtractionMixin.framewise_euclidean_distance_roi(location_1=animal_df.values[:, 0:2], location_2=np.array([center_x, center_y]), px_per_mm=1))
                         animal_df[row["Name"]] = 0
                         animal_df.loc[animal_df[f'{row["Name"]}_distance'] <= row["radius"], row["Name"]] = 1
                         animal_df.loc[animal_df[bp_names[2]] < self.threshold, row["Name"]] = 0
                         roi_bouts = detect_bouts(data_df=animal_df, target_lst=[row["Name"]], fps=self.fps)
                         roi_bouts["ANIMAL"] = animal_name
                         roi_bouts["VIDEO"] = video_name
                         self.roi_bout_results.append(roi_bouts)
                         animal_bout_results[row["Name"]] = roi_bouts
                         self.entry_results.loc[len(self.entry_results)] = [video_name, animal_name, row["Name"], len(roi_bouts)]
-                        self.time_results.loc[len(self.time_results)] = [
-                            video_name,
-                            animal_name,
-                            row["Name"],
-                            roi_bouts["Bout_time"].sum(),
-                        ]
-                    for _, row in self.roi_dict[Keys.ROI_POLYGONS.value].iterrows():
-                        roi_coords = np.array(
-                            list(zip(row["vertices"][:, 0], row["vertices"][:, 1]))
-                        )
+                        self.time_results.loc[len(self.time_results)] = [video_name,animal_name,row["Name"],roi_bouts["Bout_time"].sum()]
+                    for _, row in self.sliced_roi_dict[Keys.ROI_POLYGONS.value].iterrows():
+                        roi_coords = np.array(list(zip(row["vertices"][:, 0], row["vertices"][:, 1])))
                         animal_df[row["Name"]] = (
                             FeatureExtractionMixin.framewise_inside_polygon_roi(
                                 bp_location=animal_df.values[:, 0:2],
                                 roi_coords=roi_coords,
                             )
                         )
                         animal_df.loc[
@@ -278,75 +217,41 @@
                                 self.movements_df.loc[len(self.movements_df)] = [
                                     video_name,
                                     animal_name,
                                     roi_name,
                                     "Average velocity (cm/s)",
                                     np.average(velocities),
                                 ]
-
-        self.detailed_df = pd.concat(self.roi_bout_results, axis=0)
-        self.detailed_df = self.detailed_df.rename(
-            columns={
-                "Event": "SHAPE NAME",
-                "Start_time": "START TIME",
-                "End Time": "END TIME",
-                "Start_frame": "START FRAME",
-                "End_frame": "END FRAME",
-                "Bout_time": "DURATION (S)",
-            }
-        )
-        self.detailed_df["BODY-PART"] = self.detailed_df["ANIMAL"].map(self.bp_lk)
-        self.detailed_df = self.detailed_df[
-            [
-                "VIDEO",
-                "ANIMAL",
-                "BODY-PART",
-                "SHAPE NAME",
-                "START TIME",
-                "END TIME",
-                "START FRAME",
-                "END FRAME",
-                "DURATION (S)",
-            ]
-        ]
+        if len(self.roi_bout_results) > 1:
+            self.detailed_df = pd.concat(self.roi_bout_results, axis=0)
+            self.detailed_df = self.detailed_df.rename(columns={"Event": "SHAPE NAME", "Start_time": "START TIME", "End Time": "END TIME", "Start_frame": "START FRAME", "End_frame": "END FRAME", "Bout_time": "DURATION (S)"})
+            self.detailed_df["BODY-PART"] = self.detailed_df["ANIMAL"].map(self.bp_lk)
+            self.detailed_df = self.detailed_df[["VIDEO", "ANIMAL", "BODY-PART", "SHAPE NAME", "START TIME", "END TIME", "START FRAME", "END FRAME", "DURATION (S)"]]
 
     def save(self):
         self.entry_results["BODY-PART"] = self.entry_results["ANIMAL"].map(self.bp_lk)
         self.time_results["BODY-PART"] = self.time_results["ANIMAL"].map(self.bp_lk)
-        self.entry_results = self.entry_results[
-            ["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "ENTRY COUNT"]
-        ]
-        self.time_results = self.time_results[
-            ["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "TIME (S)"]
-        ]
-        self.entry_results.to_csv(
-            os.path.join(self.logs_path, f'{"ROI_entry_data"}_{self.datetime}.csv')
+        self.entry_results = self.entry_results[["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "ENTRY COUNT"]]
+        self.time_results = self.time_results[["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "TIME (S)"]]
+        self.entry_results.to_csv(os.path.join(self.logs_path, f'{"ROI_entry_data"}_{self.datetime}.csv')
         )
         self.time_results.to_csv(
             os.path.join(self.logs_path, f'{"ROI_time_data"}_{self.datetime}.csv')
         )
-        if self.detailed_bout_data:
-            detailed_path = os.path.join(
-                self.logs_path, f'{"Detailed_ROI_data"}_{self.datetime}.csv'
-            )
+        if self.detailed_bout_data and self.detailed_df is not None:
+            detailed_path = os.path.join(self.logs_path, f'{"Detailed_ROI_data"}_{self.datetime}.csv')
             self.detailed_df.to_csv(detailed_path)
             print(f"Detailed ROI data saved at {detailed_path}...")
         if self.calculate_distances:
-            movement_path = os.path.join(
-                self.logs_path, f'{"ROI_movement_data"}_{self.datetime}.csv'
-            )
+            movement_path = os.path.join(self.logs_path, f'{"ROI_movement_data"}_{self.datetime}.csv')
             self.movements_df["BODY-PART"] = self.movements_df["ANIMAL"].map(self.bp_lk)
-            self.movements_df = self.movements_df[
-                ["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "MEASUREMENT", "VALUE"]
-            ]
+            self.movements_df = self.movements_df[["VIDEO", "ANIMAL", "BODY-PART", "SHAPE", "MEASUREMENT", "VALUE"]]
             self.movements_df.to_csv(movement_path)
             print(f"ROI aggregate movement data saved at {movement_path}...")
-        stdout_success(
-            msg=f"ROI time and ROI entry saved in the {self.logs_path} directory in CSV format."
-        )
+        stdout_success(msg=f"ROI time and ROI entry saved in the {self.logs_path} directory in CSV format.")
 
 
 # test = ROIAnalyzer(config_path = r"/Users/simon/Desktop/envs/simba/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
 #                    data_path=None,
 #                    calculate_distances=True,
 #                    detailed_bout_data=True,
 #                    body_parts=['Nose_1', 'Nose_2'],
```

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.91.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.91.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.91.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.91.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.91.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.91.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.91.2/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.91.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.91.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.91.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.91.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.91.2/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.91.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.91.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.91.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.91.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.91.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.91.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.91.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.91.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.91.1
+Version: 1.91.2
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -598,9 +598,8 @@
 tests/test_outlier_correctors.py
 tests/test_roi_tools.py
 tests/test_stats.py
 tests/test_thirdparty_appenders.py
 tests/test_train_model_mixin.py
 tests/test_utils_data.py
 tests/test_validation_clips.py
-tests/test_video_processors.py
-tests/test_visualize_directing_animals.py
+tests/test_video_processors.py
```

### Comparing `Simba-UW-tf-dev-1.91.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.91.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/LICENSE` & `Simba-UW-tf-dev-1.91.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.91.2/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.91.2/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_stats.py` & `Simba-UW-tf-dev-1.91.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.91.2/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.91.2/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.91.2/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.91.2/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.91.2/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.91.2/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.91.2/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.91.2/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.91.2/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.91.2/tests/test_roi_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,13 +55,13 @@
     assert results['area_cm'] == expected_area
 
 @pytest.mark.parametrize("polygon_dict, px_mm, expected_area", [({'vertices': np.array([[0, 2], [200, 98], [100, 876], [10, 702]])}, 5, 45.29)])
 def test_polygon_size_calc(polygon_dict, px_mm, expected_area):
     results = polygon_size_calc(polygon_dict=polygon_dict, px_mm=px_mm)
     assert results['area_cm'] == expected_area
 
-
-@pytest.mark.parametrize("bin_length, threshold", [(10, 0.00), (1, 0.50)])
-def test_roi_timbin_calculator(config_path_args, bin_length, threshold):
-    timebin_calculator = ROITimebinCalculator(config_path=config_path_args.param, bin_length=bin_length, body_parts=['Nose_1'], threshold=threshold)
-    timebin_calculator.run()
-    timebin_calculator.save()
+#
+# @pytest.mark.parametrize("bin_length, threshold", [(10, 0.00), (1, 0.50)])
+# def test_roi_timbin_calculator(config_path_args, bin_length, threshold):
+#     timebin_calculator = ROITimebinCalculator(config_path=config_path_args.param, bin_length=bin_length, body_parts=['Nose_1'], threshold=threshold)
+#     timebin_calculator.run()
+#     timebin_calculator.save()
```

### Comparing `Simba-UW-tf-dev-1.91.1/README.md` & `Simba-UW-tf-dev-1.91.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.1/setup.py` & `Simba-UW-tf-dev-1.91.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.91.1",
+    version="1.91.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

